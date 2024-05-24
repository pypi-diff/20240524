# Comparing `tmp/keepvariable-1.2.8.tar.gz` & `tmp/keepvariable-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.2.8.tar", last modified: Fri Sep 15 10:38:45 2023, max compression
+gzip compressed data, was "keepvariable-1.2.9.tar", last modified: Sat Sep 23 17:06:52 2023, max compression
```

## Comparing `keepvariable-1.2.8.tar` & `keepvariable-1.2.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-09-15 10:38:45.276204 keepvariable-1.2.8/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.8/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-09-15 10:38:45.276204 keepvariable-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-09-15 10:38:45.258252 keepvariable-1.2.8/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.8/keepvariable/__init__.py
--rw-rw-rw-   0        0        0       36 2023-09-13 11:45:53.000000 keepvariable-1.2.8/keepvariable/credentials.py
--rw-rw-rw-   0        0        0    32003 2023-09-13 17:11:31.000000 keepvariable-1.2.8/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.8/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0     1907 2023-09-13 11:53:14.000000 keepvariable-1.2.8/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-09-15 10:38:45.275206 keepvariable-1.2.8/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-09-15 10:38:44.000000 keepvariable-1.2.8/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-09-15 10:38:45.000000 keepvariable-1.2.8/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-15 10:38:44.000000 keepvariable-1.2.8/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-09-15 10:38:44.000000 keepvariable-1.2.8/keepvariable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-09-15 10:38:45.000000 keepvariable-1.2.8/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1120 2023-09-10 22:09:35.000000 keepvariable-1.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-15 10:38:45.276204 keepvariable-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-09-15 10:37:13.000000 keepvariable-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-23 17:06:52.939385 keepvariable-1.2.9/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-09-23 17:06:52.938387 keepvariable-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-09-23 17:06:52.932403 keepvariable-1.2.9/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.9/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-09-13 11:45:53.000000 keepvariable-1.2.9/keepvariable/credentials.py
+-rw-rw-rw-   0        0        0    30080 2023-09-23 17:05:07.000000 keepvariable-1.2.9/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.9/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1907 2023-09-13 11:53:14.000000 keepvariable-1.2.9/keepvariable/kv_redis_example.py
+-rw-rw-rw-   0        0        0     2827 2023-09-23 17:05:07.000000 keepvariable-1.2.9/keepvariable/utils.py
+drwxrwxrwx   0        0        0        0 2023-09-23 17:06:52.938387 keepvariable-1.2.9/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-09-23 17:06:52.000000 keepvariable-1.2.9/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-09-23 17:06:52.000000 keepvariable-1.2.9/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-23 17:06:52.000000 keepvariable-1.2.9/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-09-23 17:06:52.000000 keepvariable-1.2.9/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-09-23 17:06:52.000000 keepvariable-1.2.9/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1120 2023-09-10 22:09:35.000000 keepvariable-1.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-09-23 17:06:52.939385 keepvariable-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-09-23 17:06:11.000000 keepvariable-1.2.9/setup.py
```

### Comparing `keepvariable-1.2.8/LICENSE` & `keepvariable-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.8/PKG-INFO` & `keepvariable-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.2.8/README.md` & `keepvariable-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.8/keepvariable/keepvariable_core.py` & `keepvariable-1.2.9/keepvariable/keepvariable_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import numpy as np
 import pandas as pd
 import redis
 from redis.client import Pipeline as RedisPipeline
 from redis.commands.search.query import Query
 from redis.lock import Lock as RedisLock
 
+from keepvariable.utils import access_element_by_path
+
 
 def get_definition(jump_frames, *args, **kwargs):
     """Return the definition of a function or a class from inside."""
     frame = inspect.currentframe()
     frame = inspect.getouterframes(frame)[jump_frames]
     try:
         string = inspect.getframeinfo(frame[0]).code_context[0].strip()
@@ -185,15 +187,17 @@
         :rtype: Any
         """
         if additional_params is None:
             additional_params = {}
 
         if isinstance(value, type(None)):
             value = {"object_type": "NoneType"}  # Redis does not natively support None values
-        elif isinstance(value, list) or isinstance(value, bool) or isinstance(value, dict) or isinstance(value, int) or isinstance(value, float):
+        elif isinstance(value, list) or isinstance(value, bool) or isinstance(
+            value, dict
+        ) or isinstance(value, int) or isinstance(value, float):
             value = json.dumps(value)
         elif isinstance(value, pd.DataFrame):
             value = self._json_serialize_dataframe(value)
             # Old implementation
             # TODO: Keep for now, delete in following commits
             # data = value.values.tolist()
             # columns = list(value.columns)
@@ -384,32 +388,38 @@
         Keys are Redis Path strings, allowing access to specific elements withing JSON document
         More info: https://redis.io/docs/stack/json/path/
         :type params: dict
 
         e.g.
         params = {"$.is_saved"=true, "$.status"=SomeEnum.COMPLETED.value}
         """
-        for json_xpath, value in params.items():
-            element, last_element, last_index = self._extract_object_from_path(name, json_xpath)
-            if last_index:
-                element[last_element][last_index] = value
+        json_obj = self.decode_loaded_value(self.storage[name]) if name in self.storage else {}
+
+        for json_path, value in params.items():
+            element, final_key = access_element_by_path(json_obj, json_path)
+            if element is None:
+                json_obj = value
+            elif final_key is None:
+                element = value
             else:
-                element[last_element] = value
+                element[final_key] = value
+
+        self.set(name, json_obj)
 
     def query(
         self,
         *,
         text_params: Optional[dict[str, tuple]] = None,
         tag_params: Optional[dict[str, tuple]] = None,
         entity_key: str,
-        index_name: str="index",
+        index_name: str = "index",
         field_to_sort_by: Optional[str] = None,
         asc=True,
         paginate: Optional[tuple[int, int]] = None,
-        ignored_keywords: list = ["index","pk","lock"],
+        ignored_keywords: list[str] = None,
         **kwargs,
     ) -> dict[str, dict]:
         """Simplified alternative to RedisSearch. Allows to search and sort by values of specified fields.
 
         :param text_params: key name to a tuple of values mapping, e.g. {'status': ('pipel', ...), ...}
         :type text_params: dict[str, tuple]
         :param tag_params: key name to a tuple of values mapping, e.g. {'status': ('QUEUED', ...), ...}
@@ -419,137 +429,95 @@
         :param asc: True if sort in ascending order, defaults to True
         :type asc: bool, optional
         :param paginate: pagination params in for of a tuple - (offset, limit), defaults to None
         :type paginate: Optional[tuple[int, int]], optional
         :return: [('jobs:43', job_dict), ...]
         :rtype: list[tuple]
         """
-        def occurence_of_ignored_keywords(record_name, ignored_keywords):
-            """checks validity of filtered records - omits ignored_keywords pk, lock, ..."""
-            
-            are_ignored_keywords_occuring=any([x in record_name for x in ignored_keywords])
-            return(are_ignored_keywords_occuring)
-            
-            
-        
-        found_records: dict[str, dict] = {
-            record_name: value for record_name, value in self.storage.items() if entity_key in record_name and not occurence_of_ignored_keywords(record_name,ignored_keywords)
-        }  # {'records:43': record_dict, ...}
+
+        def occurence_of_ignored_keywords(record_name: str, ignored_keywords: list[str]) -> bool:
+            """Check validity of filtered records - omit ignored_keywords: pk, lock, ..."""
+            are_ignored_keywords_occuring = any(x in record_name for x in ignored_keywords)
+            return (are_ignored_keywords_occuring)
+
+        if ignored_keywords is None:
+            ignored_keywords = ["index", "pk", "lock"]
+
+        found_records: list[tuple[str, dict]] = [
+            (record_name, self.decode_loaded_value(value))
+            for record_name, value in self.storage.items() if entity_key in record_name and
+            not occurence_of_ignored_keywords(record_name, ignored_keywords)
+        ]  # e.g. [('jobs:43', job_dict), ...]
 
         # TAG search
         if tag_params is not None:
             for field, values in tag_params.items():
-                found_records = {
-                    record_id: record for record_id, record in found_records.items()
+                found_records = [
+                    (record_id, record) for record_id, record in found_records
                     if record.get(field) and record.get(field) in values
-                }
+                ]
 
         # TEXT search
         if text_params is not None:
             for field, values in text_params.items():
                 for value in values:
-                    # E.g. value = "QUEU", record.get(field) = "QUEUED"
+                    # E.g. value = "QUEU", job.get(field) = "QUEUED"
                     found_records = {
-                        record_id: record for record_id, record in found_records.items()
+                        (record_id, record) for record_id, record in found_records
                         if record.get(field) and value in record.get(field)
                     }
 
         if field_to_sort_by:
-            found_records_list = sorted(found_records.items(), key=lambda x: x[1][field_to_sort_by])
+            found_records = sorted(found_records, key=lambda x: x[1][field_to_sort_by])
             if not asc:
-                found_records_list.reverse()
-            found_records = dict(found_records_list)
+                found_records.reverse()
         if paginate:
             start = paginate[0]
             end = paginate[0] + paginate[1]
-            #print("FOUND_RECORDS",found_records)
             found_records = found_records[start:end]
 
-        return found_records
+        return dict(found_records)
 
     def arrlen(self, name: str, path: str, **kwargs) -> Optional[int]:
         try:
-            element, last_element, last_index = self._extract_object_from_path(name, path)
-            if last_index:
-                return len(element[last_element][last_index])
+            json_obj = self.decode_loaded_value(self.storage[name]) if name in self.storage else {}
+
+            element, final_key = access_element_by_path(json_obj, path)
+            if element is None:
+                return len(json_obj)
+            elif final_key is None:
+                return len(element)
             else:
-                return len(element[last_element])
+                return len(element[final_key])
         except (KeyError, IndexError) as e:
             raise AssertionError(
                 "Nested object does not exist - most probably due to incorrect path arg"
             ) from e
 
     def arrappend(self, name: str, path: str, objects: Iterable, **kwargs) -> Optional[int]:
         try:
-            element, last_element, last_index = self._extract_object_from_path(name, path)
-            if last_index:
-                for obj in objects:
-                    element[last_element][last_index].append(obj)
-                return len(element[last_element][last_index])
+            json_obj = self.decode_loaded_value(self.storage[name]) if name in self.storage else {}
+
+            element, final_key = access_element_by_path(json_obj, path)
+            if element is None:
+                json_obj.extend(objects)
+                array_length = len(json_obj)
+            elif final_key is None:
+                element.extend(objects)
+                array_length = len(element)
             else:
-                for obj in objects:
-                    element[last_element].append(obj)
-                return len(element[last_element])
+                element[final_key].extend(objects)
+                array_length = len(element[final_key])
         except (KeyError, IndexError) as e:
             raise AssertionError(
                 "Nested object does not exist - most probably due to incorrect path arg"
             ) from e
 
-    def _extract_object_from_path(self, name: str, path: str) -> tuple[Any, str, Optional[int]]:
-        """Recursively traverses a JSON document under 'name' to access the object defined by the 'path' argument.
-
-        :param name: key under which a JSON document is stored
-        :type name: str
-        :param path: Redis JSON path string e.g. "job.nodes[2].status"
-        :type path: str
-        :return: tuple[referenced object, key, index]
-        :rtype: tuple[dict, str, int]
-
-        As Python does not have pointers, we have to trick it by passing a reference.
-        We're returning a reference to the object 1 level above the final one dictated by the 'path' argument
-        Additionally, we are returning the key to the last value we want to access
-        And the index if that value is actually a list, so we can access that list
-        We can use these return values to access object described by 'path' in the original function
-
-        tuple[referenced_object, key, index] --> referenced_object[key][index] = ...
-        """
-        # Parsing sequence from 'path' string
-        # name = "cache"
-        # path = "$.A.B[2].C.D[5]"
-        # elements = ["$", "A", "B[2]", "C", "D[5]"]
-        # element_list = ["cache", "A", "B", "C", "D"]
-        # index_list = [None, None, 2, None, 5]
-        # Then iterate over pairs of both lists and recurrently dive into nested objects
-
-        # Parsing logic
-        elements = path.split(".")
-        pattern = r"\[(\d+)\]"  # Find any "[*]" group where * is one or more digits
-        element_list: list[str] = []
-        index_list: list[Optional[int]] = []
-        for element in elements:
-            if match := re.search(pattern, element):
-                group = match.group()
-                index_list.append(int(group[1:-1]))  # transform "[2]" -> 2
-                element_list.append(element.split("[")[0])  # transform "B[2]" -> "B"
-            else:
-                index_list.append(None)
-                element_list.append(element)
-
-        root = element_list.index("$")
-        element_list[root] = name
-
-        # Traversing logic
-        nested_object = self.storage
-        for element, index in zip(element_list[:-1], index_list[:-1]):
-            if index is not None:
-                nested_object = nested_object[element][index]
-            else:
-                nested_object = nested_object[element]
-
-        return nested_object, element_list[-1], index_list[-1]
+        self.set(name, json_obj)
+        return array_length
 
     def scan(self, match_string: str, *args, **kwargs) -> list[str]:
         """Find saved keys, matching their name with a given glob-style pattern. This command does not block the server, as it is based on a cursor-style iterator.
 
         :param match_string: string pattern to match keys against, e.g. 'jobs:*'
         :type match_string: str
         :return: list of found key names
@@ -562,15 +530,16 @@
 
     def delete(self, *names: str, **kwargs) -> int:
         return sum(1 for name in names if self.storage.pop(name, None))
 
 
 class KeepVariableRedisServer(AbstractKeepVariableServer):
     def __init__(
-        self, host="localhost", port=6379, db=0, username='default', password: Optional[str] = None
+        self, host: str = "localhost", port: int = 6379, db: int = 0, username: str = 'default',
+        password: Optional[str] = None
     ):
         self.host: str = host
         self.port: int = port
         self.db = db
         self.username: str = username
         self.password: Optional[str] = password
 
@@ -650,16 +619,17 @@
         with self.redis.pipeline() as pipe:
             for json_xpath, value in params.items():
                 pipe.json().set(name, json_xpath, value)
             pipe.execute()
 
     def query(
         self, *, text_params: Optional[dict[str, tuple]] = None,
-        tag_params: Optional[dict[str, tuple]] = None, entity_key: str, index_name: str="index",
-        field_to_sort_by: Optional[str] = None, asc=True, paginate: Optional[tuple[int, int]] = None, **kwargs
+        tag_params: Optional[dict[str, tuple]] = None, entity_key: str, index_name: str = "index",
+        field_to_sort_by: Optional[str] = None, asc=True,
+        paginate: Optional[tuple[int, int]] = None, **kwargs
     ) -> dict:
         """Simplified wrapper to RedisSearch. Allows to search and sort by a value of Redis TAG/TEXT fields.
 
         Simplistic on purpose, to avoid bloat. Additional functionality should be added in case of need.
         :param text_params: key name to a tuple of values mapping, e.g. {'status': ('pipel', ...), ...}
         :type text_params: dict[str, tuple]
         :param tag_params: key name to a tuple of values mapping, e.g. {'status': ('QUEUED', ...), ...}
@@ -700,16 +670,16 @@
         query_object = Query(final_query)
 
         if field_to_sort_by:
             query_object.sort_by(field_to_sort_by, asc=asc)
         if paginate:
             query_object.paging(*paginate)
 
-        assert len(entity_key)>0 #entity needs to be specified
-        index_key=entity_key+":"+index_name
+        assert len(entity_key) > 0  #entity needs to be specified
+        index_key = entity_key + ":" + index_name
         job_docs: list = self.redis.ft(index_key).search(query_object).docs
         return {job_doc.id: self.decode_loaded_value(job_doc.json) for job_doc in job_docs}
 
     def arrlen(self, name: str, path: str, *,
                pipeline: Optional[RedisPipeline] = None) -> Union[int, None, RedisPipeline]:
         if pipeline:
             return pipeline.json().arrlen(name, path)
```

### Comparing `keepvariable-1.2.8/keepvariable/kv_redis_example.py` & `keepvariable-1.2.9/keepvariable/kv_redis_example.py`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.8/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.2.9/keepvariable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.2.8/pyproject.toml` & `keepvariable-1.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.8/setup.py` & `keepvariable-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.2.8',
+    version='1.2.9',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```

