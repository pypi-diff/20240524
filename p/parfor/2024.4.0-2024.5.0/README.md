# Comparing `tmp/parfor-2024.4.0.tar.gz` & `tmp/parfor-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parfor-2024.4.0.tar", max compression
+gzip compressed data, was "parfor-2024.5.0.tar", max compression
```

## Comparing `parfor-2024.4.0.tar` & `parfor-2024.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2024.4.0/LICENSE
--rw-r--r--   0        0        0     5132 2023-09-08 15:19:34.988686 parfor-2024.4.0/README.md
--rw-r--r--   0        0        0    27640 2024-04-26 16:29:27.585609 parfor-2024.4.0/parfor/__init__.py
--rw-r--r--   0        0        0     4283 2024-04-15 13:16:29.130534 parfor-2024.4.0/parfor/pickler.py
--rw-r--r--   0        0        0      603 2024-04-26 16:32:11.817505 parfor-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0     5915 1970-01-01 00:00:00.000000 parfor-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2021-03-19 08:42:10.072818 parfor-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     5711 2024-05-24 14:54:49.226658 parfor-2024.5.0/README.md
+-rw-r--r--   0        0        0    28025 2024-05-24 14:54:50.062661 parfor-2024.5.0/parfor/__init__.py
+-rw-r--r--   0        0        0     4283 2024-04-15 13:16:29.130534 parfor-2024.5.0/parfor/pickler.py
+-rw-r--r--   0        0        0      603 2024-05-24 14:41:51.587735 parfor-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 parfor-2024.5.0/PKG-INFO
```

### Comparing `parfor-2024.4.0/LICENSE` & `parfor-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parfor-2024.4.0/README.md` & `parfor-2024.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,25 @@
 Tested on linux, Windows and OSX with python 3.10.
 
 ## Why is parfor better than just using multiprocessing?
 - Easy to use
 - Using dill instead of pickle: a lot more objects can be used when parallelizing
 - Progress bars are built-in
 
+## How it works
+The work you want parfor to do is divided over a number of processes. These processes are started by parfor and put
+together in a pool. This pool is reused when you want parfor to do more work, or shut down when no new work arrives
+within 10 minutes.
+
+A handle to each bit of work is put in a queue from which the workers take work. The objects needed to do the work are
+stored in a memory manager in serialized form (using dill) and the manager hands out an object to a worker when the
+worker is requesting it. The manager deletes objects automatically when they're not needed anymore.
+
+When the work is done the result is sent back for collection in the main process.
+
 ## Installation
 `pip install parfor`
 
 ## Usage
 Parfor decorates a functions and returns the result of that function evaluated in parallel for each iteration of
 an iterator.
 
@@ -37,21 +48,19 @@
 ### Optional:
     args:   tuple with other unnamed arguments to fun
     kwargs: dict with other named arguments to fun
     total:  give the length of the iterator in cases where len(iterator) results in an error
     desc:   string with description of the progress bar
     bar:    bool enable progress bar,
                 or a callback function taking the number of passed iterations as an argument
-    pbar:   bool enable buffer indicator bar, or a callback function taking the queue size as an argument
-    rP:     ratio workers to cpu cores, default: 1
-    nP:     number of workers, default, None, overrides rP if not None
     serial: execute in series instead of parallel if True, None (default): let pmap decide
-    qsize:  maximum size of the task queue
     length: deprecated alias for total
-    **bar_kwargs: keywords arguments for tqdm.tqdm
+    n_processes: number of processes to use,
+        the parallel pool will be restarted if the current pool does not have the right number of processes
+    **bar_kwargs: keyword arguments for tqdm.tqdm
 
 ### Return
     list with results from applying the function 'fun' to each iteration of the iterable / iterator
 
 ## Examples
 ### Normal serial for loop
     <<
@@ -145,15 +154,15 @@
     def fun(im):
         return np.mean(im)
         
     >> [list with means of the images]
     
 # Extra's
 ## `pmap`
-The function parfor decorates, use it like `map`.
+The function parfor decorates, it's used similarly to `map`.
 
 ## `Chunks`
 Split a long iterator in bite-sized chunks to parallelize
 
 ## `ParPool`
 More low-level accessibility to parallel execution. Submit tasks and request the result at any time,
 (although necessarily submit first, then request a specific task), use different functions and function
```

### Comparing `parfor-2024.4.0/parfor/__init__.py` & `parfor-2024.5.0/parfor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,21 +252,21 @@
 
 
 class ParPool:
     """ Parallel processing with addition of iterations at any time and request of that result any time after that.
         The target function and its argument can be changed at any time.
     """
     def __init__(self, fun: Callable[[Any, ...], Any] = None,
-                 args: tuple[Any] = None, kwargs: dict[str, Any] = None, bar: Bar = None):
+                 args: tuple[Any] = None, kwargs: dict[str, Any] = None, n_processes: int = None, bar: Bar = None):
         self.id = id(self)
         self.handle = 0
         self.tasks = {}
         self.bar = bar
         self.bar_lengths = {}
-        self.spool = PoolSingleton(self)
+        self.spool = PoolSingleton(n_processes, self)
         self.manager = self.spool.manager
         self.fun = fun
         self.args = args
         self.kwargs = kwargs
         self.is_started = False
         self.last_task = None
 
@@ -368,21 +368,22 @@
 
 class PoolSingleton:
     """ There can be only one pool at a time, but the pool can be restarted by calling close() and then constructing a
         new pool. The pool will close itself after 10 minutes of idle time. """
 
     instance = None
 
-    def __new__(cls, *args: Any, **kwargs: Any) -> PoolSingleton:
-        if cls.instance is not None:  # restart if any workers have shut down
-            if cls.instance.n_workers.value < cls.instance.n_processes:
+    def __new__(cls, n_processes: int = None, *args: Any, **kwargs: Any) -> PoolSingleton:
+        # restart if any workers have shut down or if we want to have a different number of processes
+        if cls.instance is not None:
+            if cls.instance.n_workers.value < cls.instance.n_processes or cls.instance.n_processes != n_processes:
                 cls.instance.close()
         if cls.instance is None or not cls.instance.is_alive:
             new = super().__new__(cls)
-            new.n_processes = cpu_count
+            new.n_processes = n_processes or cpu_count
             new.instance = new
             new.is_started = False
             ctx = Context()
             new.n_workers = ctx.Value('i', new.n_processes)
             new.event = ctx.Event()
             new.queue_in = ctx.Queue(3 * new.n_processes)
             new.queue_out = ctx.Queue(new.n_processes)
@@ -392,15 +393,15 @@
                                 Worker(new.shared_memory, new.queue_in, new.queue_out, new.n_workers, new.event))
             new.is_alive = True
             new.handle = 0
             new.pools = {}
             cls.instance = new
         return cls.instance
 
-    def __init__(self, parpool: Parpool = None) -> None:  # noqa
+    def __init__(self, n_processes: int = None, parpool: Parpool = None) -> None:  # noqa
         if parpool is not None:
             self.pools[parpool.id] = parpool
 
     def __getstate__(self) -> NoReturn:
         raise RuntimeError(f'Cannot pickle {self.__class__.__name__} object.')
 
     # def __del__(self):
@@ -453,15 +454,15 @@
                 if task.done:
                     handle, result = task.handle, task.result
                     pool.tasks.pop(handle)
                     return handle, result
 
     @classmethod
     def close(cls) -> None:
-        if hasattr(cls, 'instance') and cls.instance is not None:
+        if cls.instance is not None:
             instance = cls.instance
             cls.instance = None
 
             def empty_queue(queue):
                 try:
                     if not queue._closed:  # noqa
                         while not queue.empty():
@@ -545,15 +546,15 @@
         with self.n_workers:
             self.n_workers.value -= 1
 
 
 def pmap(fun: Callable[[Iteration, Any, ...], Result], iterable: Iterable[Iteration] = None,
          args: tuple[Any, ...] = None, kwargs: dict[str, Any] = None, total: int = None, desc: str = None,
          bar: Bar | bool = True, terminator: Callable[[], None] = None, serial: bool = None, length: int = None,
-         **bar_kwargs: Any) -> list[Result]:
+         n_processes: int = None, **bar_kwargs: Any) -> list[Result]:
     """ map a function fun to each iteration in iterable
         use as a function: pmap
         use as a decorator: parfor
         best use: iterable is a generator and length is given to this function as 'total'
 
         required:
             fun:    function taking arguments: iteration from  iterable, other arguments defined in args & kwargs
@@ -563,14 +564,16 @@
             kwargs: dict with other named arguments to fun
             total:  give the length of the iterator in cases where len(iterator) results in an error
             desc:   string with description of the progress bar
             bar:    bool enable progress bar,
                         or a callback function taking the number of passed iterations as an argument
             serial: execute in series instead of parallel if True, None (default): let pmap decide
             length: deprecated alias for total
+            n_processes: number of processes to use,
+                the parallel pool will be restarted if the current pool does not have the right number of processes
             **bar_kwargs: keywords arguments for tqdm.tqdm
 
         output:
             list with results from applying the function \'fun\' to each iteration of the iterable / iterator
 
         examples:
             << from time import sleep
@@ -650,15 +653,15 @@
             return sum([chunk_fun(c, *args, **kwargs) for c in tqdm(iterable, **bar_kwargs)], [])
     else:   # parallel case
         with ExitStack() as stack:
             if callable(bar):
                 bar = stack.enter_context(ExternalBar(callback=bar))
             else:
                 bar = stack.enter_context(tqdm(**bar_kwargs))
-            with ParPool(chunk_fun, args, kwargs, bar) as p:
+            with ParPool(chunk_fun, args, kwargs, n_processes, bar) as p:
                 for i, (j, l) in enumerate(zip(iterable, iterable.lengths)):  # add work to the queue
                     p(j, handle=i, barlength=iterable.lengths[i])
                     if bar.total is None or bar.total < i+1:
                         bar.total = i+1
                 if is_chunked:
                     return [p[i] for i in range(len(iterable))]
                 else:
```

### Comparing `parfor-2024.4.0/parfor/pickler.py` & `parfor-2024.5.0/parfor/pickler.py`

 * *Files identical despite different names*

### Comparing `parfor-2024.4.0/pyproject.toml` & `parfor-2024.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parfor"
-version = "2024.4.0"
+version = "2024.5.0"
 description = "A package to mimic the use of parfor as done in Matlab."
 authors = ["Wim Pomp <wimpomp@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["parfor", "concurrency", "multiprocessing", "parallel"]
 repository = "https://github.com/wimpomp/parfor"
```

### Comparing `parfor-2024.4.0/PKG-INFO` & `parfor-2024.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parfor
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: A package to mimic the use of parfor as done in Matlab.
 Home-page: https://github.com/wimpomp/parfor
 License: GPLv3
 Keywords: parfor,concurrency,multiprocessing,parallel
 Author: Wim Pomp
 Author-email: wimpomp@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -31,14 +31,25 @@
 Tested on linux, Windows and OSX with python 3.10.
 
 ## Why is parfor better than just using multiprocessing?
 - Easy to use
 - Using dill instead of pickle: a lot more objects can be used when parallelizing
 - Progress bars are built-in
 
+## How it works
+The work you want parfor to do is divided over a number of processes. These processes are started by parfor and put
+together in a pool. This pool is reused when you want parfor to do more work, or shut down when no new work arrives
+within 10 minutes.
+
+A handle to each bit of work is put in a queue from which the workers take work. The objects needed to do the work are
+stored in a memory manager in serialized form (using dill) and the manager hands out an object to a worker when the
+worker is requesting it. The manager deletes objects automatically when they're not needed anymore.
+
+When the work is done the result is sent back for collection in the main process.
+
 ## Installation
 `pip install parfor`
 
 ## Usage
 Parfor decorates a functions and returns the result of that function evaluated in parallel for each iteration of
 an iterator.
 
@@ -59,21 +70,19 @@
 ### Optional:
     args:   tuple with other unnamed arguments to fun
     kwargs: dict with other named arguments to fun
     total:  give the length of the iterator in cases where len(iterator) results in an error
     desc:   string with description of the progress bar
     bar:    bool enable progress bar,
                 or a callback function taking the number of passed iterations as an argument
-    pbar:   bool enable buffer indicator bar, or a callback function taking the queue size as an argument
-    rP:     ratio workers to cpu cores, default: 1
-    nP:     number of workers, default, None, overrides rP if not None
     serial: execute in series instead of parallel if True, None (default): let pmap decide
-    qsize:  maximum size of the task queue
     length: deprecated alias for total
-    **bar_kwargs: keywords arguments for tqdm.tqdm
+    n_processes: number of processes to use,
+        the parallel pool will be restarted if the current pool does not have the right number of processes
+    **bar_kwargs: keyword arguments for tqdm.tqdm
 
 ### Return
     list with results from applying the function 'fun' to each iteration of the iterable / iterator
 
 ## Examples
 ### Normal serial for loop
     <<
@@ -167,15 +176,15 @@
     def fun(im):
         return np.mean(im)
         
     >> [list with means of the images]
     
 # Extra's
 ## `pmap`
-The function parfor decorates, use it like `map`.
+The function parfor decorates, it's used similarly to `map`.
 
 ## `Chunks`
 Split a long iterator in bite-sized chunks to parallelize
 
 ## `ParPool`
 More low-level accessibility to parallel execution. Submit tasks and request the result at any time,
 (although necessarily submit first, then request a specific task), use different functions and function
```

