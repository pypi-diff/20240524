# Comparing `tmp/stellapy-0.2.1.tar.gz` & `tmp/stellapy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellapy-0.2.1.tar", max compression
+gzip compressed data, was "stellapy-0.3.0.tar", max compression
```

## Comparing `stellapy-0.2.1.tar` & `stellapy-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1099 2023-11-18 13:59:06.681154 stellapy-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1358 2024-02-17 16:00:18.917766 stellapy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6571 2024-01-22 04:47:01.625642 stellapy-0.2.1/README.md
--rw-r--r--   0        0        0     2244 2023-11-25 08:08:43.895208 stellapy-0.2.1/schema.json
--rw-r--r--   0        0        0        0 2023-08-13 15:03:07.759794 stellapy-0.2.1/stellapy/__init__.py
--rw-r--r--   0        0        0     5999 2024-01-22 04:47:01.726696 stellapy-0.2.1/stellapy/configuration.py
--rw-r--r--   0        0        0     6725 2024-01-06 12:50:56.675163 stellapy-0.2.1/stellapy/executor.py
--rw-r--r--   0        0        0      930 2023-11-22 17:32:55.552421 stellapy-0.2.1/stellapy/logger.py
--rw-r--r--   0        0        0     9782 2024-02-17 09:57:44.679614 stellapy-0.2.1/stellapy/reloader.py
--rw-r--r--   0        0        0     3423 2024-02-17 09:56:11.901533 stellapy-0.2.1/stellapy/stella.py
--rw-r--r--   0        0        0     3787 2024-01-04 14:48:30.611540 stellapy-0.2.1/stellapy/walker.py
--rw-r--r--   0        0        0     7881 1970-01-01 00:00:00.000000 stellapy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-05-20 06:11:00.985933 stellapy-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1382 2024-05-22 06:32:14.561028 stellapy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7418 2024-05-24 17:06:23.380459 stellapy-0.3.0/README.md
+-rw-r--r--   0        0        0     2088 2024-05-22 10:56:54.450162 stellapy-0.3.0/schema.json
+-rw-r--r--   0        0        0        0 2023-08-13 15:03:07.759794 stellapy-0.3.0/stellapy/__init__.py
+-rw-r--r--   0        0        0     5865 2024-05-22 15:46:36.572273 stellapy-0.3.0/stellapy/configuration.py
+-rw-r--r--   0        0        0     6757 2024-05-22 06:13:00.519454 stellapy-0.3.0/stellapy/executor.py
+-rw-r--r--   0        0        0      930 2023-11-22 17:32:55.552421 stellapy-0.3.0/stellapy/logger.py
+-rw-r--r--   0        0        0    12962 2024-05-24 17:03:34.892318 stellapy-0.3.0/stellapy/reloader.py
+-rw-r--r--   0        0        0     3404 2024-05-22 06:25:05.715876 stellapy-0.3.0/stellapy/stella.py
+-rw-r--r--   0        0        0     3733 2024-05-24 04:57:42.743895 stellapy-0.3.0/stellapy/walker.py
+-rw-r--r--   0        0        0     8768 1970-01-01 00:00:00.000000 stellapy-0.3.0/PKG-INFO
```

### Comparing `stellapy-0.2.1/LICENSE.txt` & `stellapy-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stellapy-0.2.1/pyproject.toml` & `stellapy-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stellapy"
-version = "0.2.1"
+version = "0.3.0"
 description = "Streamline your web dev experience with stella - reload for the terminal as well as browser."
 
 authors = ["Shravan Asati <dev.shravan@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/shravanasati/stellapy"
@@ -40,17 +40,18 @@
 
 [tool.poetry.scripts]
 stella = "stellapy.stella:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
-helium = "^4.0.0"
 rich = "^13.7.0"
 ruamel-yaml = "^0.18.5"
 gitignorefile = "^1.1.2"
 jsonschema = "^4.20.0"
+watchdog = "^4.0.0"
+selenium = "^4.21.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stellapy-0.2.1/README.md` & `stellapy-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,58 +2,58 @@
 
 ![stella_demo](assets/stella.gif)
 
 [![Downloads](https://pepy.tech/badge/stellapy)](https://pepy.tech/project/stellapy)
 
 stella is a command line utility made for streamlining web development experience. 
 It is able to reload server as well as the browser page on every file change.
-Although you can use it like any other live reload tool - with builtin `.gitignore` detection and following, along with several other features like multiple command execution, and the npm-scripts like interface.
+You can use it like any other live reload tool too - with builtin `.gitignore` detection and obedience, along with several other features like multiple command execution, and the npm-scripts like interface.
 
 <br>
 
 
 ## 📝 Table of Contents
 - [Installation](#%EF%B8%8F-installation)
 - [Motivation](#-motivation)
 - [How does stella work?](#%EF%B8%8F-how-does-stella-work)
 - [Usage](#-usage)
-- [Changelog](#-changelog)
 - [Versioning](#-versioning)
 - [Licensing](#-licensing)
 - [Contribution](#-contribution)
 
 
 <br>
 
 
 ## ⚡️ Installation
 
 Using [pipx](https://pypa.github.io/pipx/) (recommended):
 ```
 pipx install stellapy
+# pipx upgrade stellapy to upgrade
 ```
 
 On Windows:
 ```
-pip install stellapy
+pip install -U stellapy
 ```
 
 On Linux/MacOS:
 ```
-pip3 install stellapy
+pip3 install -U stellapy
 ```
 
 
 <br>
 
 
 
 ## 💫 Motivation
 
-I wanted a CLI that could live reload the browser page as well as live restart the server. I tried to find such a tool, but didn't find one. So I made stella - that could reload backend as well as frontend code. Also the builtin debug modes of web frameworks sucked.
+I wanted a CLI that could live reload the browser page as well as live restart the server. I tried to find such a tool, but didn't find one. So I made stella - that could reload backend as well as frontend code. Also the builtin "debug modes" of web frameworks sucked.
 
 <br>
 
 ## ⚙️ How does stella work?
 
 stella continuously watches for file changes in the project, while respecting the gitignore file and whenever a change is made, it kills the existing process and spawns a new process using subprocess. What about browser reload? It uses selenium to accomplish that.
 
@@ -88,30 +88,32 @@
 
 This yaml file comes with a schema which can be utilized by yaml language servers to provide autocompletion and validation to make sure the config is correct.
 
 ### Configuration
 
 Let's quickly go over the config options:
 
- - **`browser`**: This option specifies the browser to use when `url` is given. The only valid options for browser currently are `firefox` and `chrome`.
+ - **`browser`**: This option specifies the browser to use when `url` is given. The only valid options for browser currently are `firefox`, `chrome`, `edge` and `safari`.
 
  - **`include_only`**: The list of gitignore-style patterns to consider for live reload. This will be used along with the ignore file (`stella.ignore` or `.gitignore`) to match files. eg. `include_only: ["*.py", "*.env"]`.
 
- - **`poll_interval`**: The duration in **milliseconds** to poll the filesystem for changes.
+ - **`poll_interval`**: The duration in **milliseconds** to poll the filesystem for changes. This has been modified past v0.3.0 - it now signifies the threshold duration for which stella should accept changes.
 
  - **`browser_wait_interval`**: This is the duration in **milliseconds** between the execution of given command on the terminal and browser page refresh. This can be used in situations when the server takes some time before it is ready to listen on a given port.
 
- - **`follow_symlinks`**: Boolean value that indicates whether to follow symbolic links encountered in the filesystem.
+ <!-- - **`follow_symlinks`**: Boolean value that indicates whether to follow symbolic links encountered in the filesystem. -->
 
  - **`scripts`**: This the list of npm style scripts that take 4 parameters each.
 
     * `name`: Name of the script. To execute a certain script, use its name in the `stella run SCRIPT_NAME` command. The script named _default_ will be used in case SCRIPT_NAME is not provided. Note that this parameter is **case-insensitive**, for convenience.
 
     * `url`: The URL to listen to on the browser. Set it to an empty string (`''`) if you don't want live reload on the browser. eg. `localhost:8000`.
 
+      > Note: For chrome and edge, you URLs starting with `localhost` won't work, prepend the `url` with a scheme like `http://` or `file://`. Not tested on safari, but if you see `data;` in the address bar, this URL change should fix it.
+
     * `command`: A single command or a list of commands to execute on the terminal. eg.
       ```
       command: python3 app.py
       ```
 
       ```
       command: 
@@ -122,24 +124,21 @@
       If a list of commands are provided, the `shell` will be considered `true` even if it's `false`.
 
     * `shell`: **Boolean** value which indicates whether to execute commands inside a shell context (like bash, powershell, zsh...) or as an independent process. This is useful if you want to execute shell scripts directly without invoking the shell interpreter. On Windows, powershell is used as shell (instead of cmd). On Linux and MacOS, the shell used is determined by `SHELL` environment variable. If it's not present, `/bin/sh` will be used.
 
 
 ### Ignore
 
-Polling a filesystem for changes can be lengthy in case of big projects.
-Even worse when dependencies are vendored within the project, like python virtual environments or include directories in c/c++.
-
-Therefore, you can create a `stella.ignore` file in the project with gitignore-style patterns to exclude certain directories and files to consider.
+You can create a `stella.ignore` file in the project with gitignore-style patterns to exclude certain directories and files to watch.
 
 Otherwise, `.gitignore` also just works, and is the recommended way.
 
 However, `stella.ignore` will be the first one that will be searched for. If it's not found, stella will resort to `.gitignore`.
 
-Ignore patterns are cached once stella is started, similar to the stella configuration. If you change either of them, in order to see the desired changes, you need stop stella and run it again.
+Ignore patterns are cached once stella is started, similar to the stella configuration. If you change either of them, in order to see the desired changes, you need to either type `rc` and press enter or stop stella and run it again.
 
 
 ### run
 
 ```
 stella run SCRIPT_NAME
 stella run SCRIPT_NAME --config-file /path/to/config/stella.yml
@@ -150,25 +149,29 @@
 
 An optional `--config-file` (`-c` for short) flag can be used to specify the config file to be used. 
 Alternatively, an environment variable named `STELLA_CONFIG` can be set for the same.
 
 If not provided, stella will attempt to find `stella.yml` in the current directory or its parent folders until its found.
 
 
-While stella is running, you can input `rs` to restart the server and refresh the browser page manually, and `rb` only to refresh the browser page.
+While stella is running, you can input `rs` to restart the server and refresh the browser page manually, and `rb` to refresh the browser page.
+
+Since *v0.3.0*, you can also reload the stella configuration by typing `rc` and pressing enter. This will close the existing browser window and the running process, and restart the same script with the stella configuration.
+
+To stop stella, input `ex`. It will close the browser as well as kill the running process gracefully (it sends `SIGTERM` on Unix based systems and `CTRL_BREAK_EVENT` on Windows).
 
-To stop stella, input `ex`. It will close the browser as well as kill the running process gracefully.
+If an error is encountered on refreshing the browser page (an event which can happen often, primarily due to server taking a long time to restart or the command failed to execute successfully), stella will retry with the exponential backoff strategy (2^n) until the browser refresh is successfull or a new change is detected.
 
 <br>
 
 
 ## 📄 Licensing
 
 License © 2021-Present Shravan Asati
 
 This repository is licensed under the MIT license. See [LICENSE](LICENSE) for details.
 
 <br>
 
 ## 👥 Contribution
 
-Contribution is more than welcome. For more guidelines on contributing to stella, refer [CONTRIBUTING.md](CONTRIBUTING.md).
+Contribution is more than welcome. For more guidelines on contributing to stella, refer [CONTRIBUTING.md](CONTRIBUTING.md).
```

### Comparing `stellapy-0.2.1/schema.json` & `stellapy-0.3.0/schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985821759259258%*

 * *Differences: {"'definitions'": "{'Stella': {'properties': {'browser': {'enum': {insert: [(2, 'edge'), (3, "*

 * *                  "'safari')]}}, delete: ['follow_symlinks']}, 'required': {delete: [5]}}}"}*

```diff
@@ -44,26 +44,24 @@
         "Stella": {
             "additionalProperties": false,
             "properties": {
                 "browser": {
                     "description": "The browser to be used.",
                     "enum": [
                         "chrome",
-                        "firefox"
+                        "firefox",
+                        "edge",
+                        "safari"
                     ],
                     "type": "string"
                 },
                 "browser_wait_interval": {
                     "description": "The interval in milliseconds to wait to refresh browser window after executing command(s) on the terminal.",
                     "type": "number"
                 },
-                "follow_symlinks": {
-                    "description": "Whether to follow symbolic links encountered in the directory tree.",
-                    "type": "boolean"
-                },
                 "include_only": {
                     "description": "gitignore style include-only patterns.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
@@ -80,15 +78,14 @@
                 }
             },
             "required": [
                 "browser",
                 "include_only",
                 "poll_interval",
                 "browser_wait_interval",
-                "scripts",
-                "follow_symlinks"
+                "scripts"
             ],
             "title": "Stella",
             "type": "object"
         }
     }
 }
```

### Comparing `stellapy-0.2.1/stellapy/configuration.py` & `stellapy-0.3.0/stellapy/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,31 +47,28 @@
 
 @dataclass(slots=True, frozen=True)
 class Configuration:
     """
     Represents the stella configuration.
     """
 
-    # todo set custom browser drivers for extending browser support
     browser: str
     include_only: list[str]
     poll_interval: float  # milliseconds
     browser_wait_interval: float
-    follow_symlinks: bool
     scripts: list[Script]
 
     @classmethod
     def default(cls):
         return cls(
             browser="firefox",
             include_only=[],
             scripts=[Script("default", "", "echo 'hello'", True)],
             poll_interval=500,
             browser_wait_interval=1000,
-            follow_symlinks=False,
         )
 
     def to_yaml(self):
         yaml = YAML()
         s = StringIO()
         yaml.dump(data=asdict(self), stream=s)
         s.seek(0)
@@ -174,15 +171,15 @@
             "error",
             IMPROPER_CONFIG_HELP_TEXT,
         )
         exit(1)
     except ValidationError as ve:
         log(
             "error",
-            f"{IMPROPER_CONFIG_HELP_TEXT}\n\tvalidation error: {ve}",
+            f"{IMPROPER_CONFIG_HELP_TEXT}\nvalidation error: {ve}",
         )
         exit(1)
     except Exception as e:
         log("error", "fatal: an unknown error occcured")
         exception(e)
         exit(1)
```

### Comparing `stellapy-0.2.1/stellapy/executor.py` & `stellapy-0.3.0/stellapy/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 PWSH_PRESENT = _test_powershell()
 
 
 class Executor:
     """
-    base class for executing sys calls.
+    base class for executing processes.
     """
 
     def __init__(self, script: Script) -> None:
         self.__command, self.shell = self.build_command(script)
         self.command_to_display = (
             self.__command
             if isinstance(self.__command, str)
@@ -127,15 +127,17 @@
                 return f'powershell -Command "{joined_command}"', True
             elif WINDOWS and (not PWSH_PRESENT):
                 return joined_command, True
             else:
                 return joined_command, True
 
         else:
-            raise TypeError(f"invalid type of {script.command=}, {type(script.command)=}")
+            raise TypeError(
+                f"invalid type of {script.command=}, {type(script.command)=}"
+            )
 
     def start(self):
         try:
             if WINDOWS:
                 self.__process = subprocess.Popen(
                     self.__command,
                     stdout=sys.stdout,
```

### Comparing `stellapy-0.2.1/stellapy/logger.py` & `stellapy-0.3.0/stellapy/logger.py`

 * *Files identical despite different names*

### Comparing `stellapy-0.2.1/stellapy/reloader.py` & `stellapy-0.3.0/stellapy/reloader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,86 @@
-import os
+from dataclasses import dataclass
+from datetime import datetime, timedelta
 from logging import exception
-from threading import Thread
+from threading import Lock, Thread
 from time import sleep
+from typing import Any, Callable, Generic, TypeVar
 
-import helium
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium.common.exceptions import NoSuchElementException
+from watchdog.observers import Observer
 
-from stellapy.configuration import Configuration
+from stellapy.configuration import Configuration, load_configuration_handle_errors
 from stellapy.executor import Executor
 from stellapy.logger import log
-from stellapy.walker import get_file_content, walk
+from stellapy.walker import GitignoreMatchingEventHandler
+
+T = TypeVar("T")
+ActionFunc = Callable[["Trigger"], None]
+ErrorHandlerFunc = Callable[["Trigger", Exception], None]
+
+
+@dataclass(frozen=True)
+class Trigger(Generic[T]):
+    """
+    Similar to contexts in go, a trigger carries an action to perform at a certain datetime, along with an error handler and a value.
+    """
+
+    action: ActionFunc
+    when: datetime
+    error_handler: ErrorHandlerFunc | None
+    value: T
+
+    def __repr__(self) -> str:
+        return f"Trigger <action={self.action} when={self.when} error_handler={self.error_handler} value={self.value}>"
+
+
+class TriggerQueue:
+    """
+    A list of triggers offering some useful and thread-safe methods.
+    The type variable `T` is used for the value of Trigger.
+    """
+
+    def __init__(self) -> None:
+        self.triggers: list[Trigger[Any]] = []
+        self.__lock = Lock()
+
+    def add(self, trigger: Trigger[Any]):
+        """
+        Add a trigger to the queue.
+        """
+        with self.__lock:
+            self.triggers.append(trigger)
+
+    def execute_remaining(self):
+        """
+        Executes all the triggers that need to be executed, i.e., whose deadline has been reached.
+        """
+        now = datetime.now()
+        with self.__lock:
+            # store all ready triggers in a temp list
+            to_execute = [t for t in self.triggers if now >= t.when]
+            self.triggers = [t for t in self.triggers if t not in to_execute]
+
+        for trigger in to_execute:
+            try:
+                trigger.action(trigger)
+            except Exception as e:
+                if trigger.error_handler:
+                    trigger.error_handler(trigger, e)
+                else:
+                    raise e
+
+    def cancel_all(self):
+        """
+        Cancel all the scheduled triggers.
+        """
+        with self.__lock:
+            self.triggers.clear()
 
 
 class Reloader:
     """
     The `Reloader` class.
     """
 
@@ -31,216 +99,233 @@
                 f"didn't find any script named {script_name.lower()} in config located at `{config_file}`",
             )
             exit(1)
         self.config_file = config_file
         self.executor = Executor(self.script)
         self.url = self.script.url
         self.RELOAD_BROWSER = bool(self.url)
-        self.project_data = self.get_project_data()
 
-        # convert to seconds
-        self.poll_interval = self.config.poll_interval / 1000
-        self.browser_wait_interval = self.config.browser_wait_interval / 1000
+        # watchdog observer
+        self.observer = Observer()
+        self.observer.schedule(
+            GitignoreMatchingEventHandler(
+                self.config.include_only, self.config.poll_interval, self._restart
+            ),
+            ".",
+            recursive=True,
+        )
 
-    def get_project_data(self) -> dict:
-        """
-        Returns a dict with filenames mapped to their contents.
-        """
-        project_data = {}
-        for f in walk(self.config.include_only, self.config.follow_symlinks):
-            project_data.update({f: get_file_content(f)})
+        # trigger executor
+        self._finished = False  # used by trigger thread to look for exits
+        self.trigger_execution_interval = 0.1  # seconds
+        self.trigger_queue = TriggerQueue()
+        self.trigger_thread = Thread(target=self._trigger_executor)
+        self.trigger_thread.start()
 
-        return project_data
+        # convert to seconds
+        self.poll_interval = self.config.poll_interval / 1000
+        self.browser_wait_delta = timedelta(
+            milliseconds=self.config.browser_wait_interval
+        )
 
-    def detect_change(self) -> bool:
+    def _trigger_executor(self):
         """
-        Detects if a change has been done to the project. Also updates the project data if
-        new a change is detected.
+        Executes all the remaining triggers in the trigger queue until `self._finished`
+        is set to `True`.
         """
-        new_content = self.get_project_data()
-        if len(self.project_data.keys()) != len(new_content.keys()):
-            self.project_data = new_content
-            return True
+        while not self._finished:
+            self.trigger_queue.execute_remaining()
+            sleep(self.trigger_execution_interval)
+
+    def _start_browser(self):
+        # selenium driver
+        if self.config.browser not in ("firefox", "chrome", "safari", "edge"):
+            # this should never happen because of configuration validation
+            raise Exception(f"invalid browser={self.config.browser}")
+
+        match self.config.browser.lower():
+            case "firefox":
+                self.driver = webdriver.Firefox()
+            case "chrome":
+                self.driver = webdriver.Chrome()
+            case "safari":
+                self.driver = webdriver.Safari()
+            case "edge":
+                self.driver = webdriver.Edge()
+            case _:
+                raise Exception(f"unknown browser={self.config.browser}")
 
         try:
-            for k, v in self.project_data.items():
-                if new_content[k] != v:
-                    self.project_data = new_content
-                    return True
-
-        except KeyError:
-            self.project_data = new_content
-            return True
+            self.driver.get(self.url)
 
         except Exception as e:
-            print("FATAL ERROR: This should never happen.")
-            exception(e)
-            os._exit(1)
-
-        return False
+            se = str(e)
+            if "Message: unknown error: cannot find Chrome binary" in se:
+                log(
+                    "error",
+                    "chrome binary not found. either install chrome browser or configure stella browser to firefox.",
+                )
+                self.stop()
 
-    def start_browser(self):
-        browser = self.config.browser
-        if browser == "chrome":
-            try:
-                helium.start_chrome(self.url)
-            except Exception as e:
-                if "Message: unknown error: cannot find Chrome binary" in str(e):
-                    log(
-                        "error",
-                        "chrome binary not found. either install chrome browser or configure stella browser to firefox.",
+            elif "net::ERR_" in se or "Reached error page" in se:
+                log(
+                    "error",
+                    f"browser startup failed, retrying in {self._displayable_seconds_from_timedelta(self.browser_wait_delta)} seconds",
+                )
+                self.trigger_queue.add(
+                    Trigger(
+                        action=self._browser_reloader,
+                        when=datetime.now() + self.browser_wait_delta,
+                        error_handler=self._browser_reload_error_handler,
+                        value=self.browser_wait_delta,
                     )
-                    self.stop_server()
-
-                elif "Reached error page" in str(e):
-                    log("error", "app crashed, waiting for file changes to restart...")
+                )
 
-                else:
-                    log("error", f"an unknown error occurred: \n{e}")
-                    self.stop_server()
+            else:
+                log("error", f"an unknown error occurred: \n{e}")
+                self.stop()
 
-        elif browser == "firefox":
+    def _browser_reloader(self, _: Trigger[timedelta]):
+        """
+        A helper function used in browser reload triggers.
+        """
+        self.driver.refresh()
+        # firefox throws an error via selenium if the refresh wasn't successfull
+        # chrome and edge don't, so we can't call the error handler function (exponential backoff)
+        # even if the page wasn't loaded
+        # thus, check if the body tag has `neterror` class because it's always present
+        # when any browser(again, not tested for safari) shows the error page
+        # not sure how safari behaves, so we'll check for it too
+        if self.config.browser != "firefox":
             try:
-                helium.start_firefox(self.url)
-            except Exception as e:
-                if "Message: unknown error: cannot find Firefox binary" in str(e):
-                    log(
-                        "error",
-                        "firefox binary not found. either install chrome browser or configure stella to use firefox.",
-                    )
-                    self.stop_server()
-
-                elif "Message: Reached error page" in str(e):
-                    log("error", "app crashed, waiting for file changes to restart...")
-
-                else:
-                    log("error", f"an unknown error occurred: \n{e}")
-                    self.stop_server()
+                el = self.driver.find_element(By.CLASS_NAME, "neterror")
+            except NoSuchElementException:
+                return
+            else:
+                if el.tag_name == "body":
+                    raise Exception("failed to load page")
 
+    @staticmethod
+    def _displayable_seconds_from_timedelta(t: timedelta):
+        """
+        Helper function to return seconds from a timedelta object, because if t.seconds < 1,
+        then t.seconds is zero for a timedelta object.
+        """
+        if t.seconds > 0:
+            return t.seconds
         else:
-            log(
-                "error",
-                f"invalid browser specified: {browser}. stella supports only chrome and firefox. execute `stella config --browser chrome|firefox` for configuring the browser.",
+            return (t.microseconds) / 10e6
+
+    def _browser_reload_error_handler(self, t: Trigger[timedelta], e: Exception):
+        log(
+            "error",
+            f"browser reload didnt work, retrying in {self._displayable_seconds_from_timedelta(2*t.value)} seconds...",
+        )
+        self.trigger_queue.add(
+            Trigger(
+                action=t.action,
+                when=datetime.now() + 2 * t.value,
+                error_handler=self._browser_reload_error_handler,
+                value=2 * t.value,
             )
-            self.stop_server()
+        )
 
     def _restart(self):
-        try:
-            if self.detect_change():
-                log(
-                    "info",
-                    "detected changes in the project, reloading server and browser",
-                )
-                self.executor.re_execute()
-                sleep(self.browser_wait_interval)
-                if self.RELOAD_BROWSER:
-                    helium.refresh()
-
-            else:
-                sleep(self.poll_interval)
-        except Exception:
-            try:
-                log(
-                    "error",
-                    f"browser reload didnt work, retrying in {2 * self.browser_wait_interval} seconds...",
-                )
-                sleep(2 * self.browser_wait_interval)
-                if self.RELOAD_BROWSER:
-                    helium.refresh()
-            except Exception:
-                log(
-                    "error",
-                    "browser reload retry failed! make sure you've provided stella the correct url to listen at. waiting for file changes or `rb`/`rs` input to restart...",
-                )
-
-    def restart(self) -> None:
+        log(
+            "info",
+            "detected changes in the project, reloading server and browser",
+        )
+        # cancel all prev triggers, because we got a new change
+        self.trigger_queue.cancel_all()
+        self.executor.re_execute()
         if self.RELOAD_BROWSER:
-            self.start_browser()
-        while True:
-            self._restart()
+            self.trigger_queue.add(
+                Trigger[timedelta](
+                    action=self._browser_reloader,
+                    when=datetime.now() + self.browser_wait_delta,
+                    error_handler=self._browser_reload_error_handler,
+                    value=self.browser_wait_delta,
+                ),
+            )
 
     def manual_input(self) -> None:
         """
         Manual restart and exit.
         """
-        while True:
+        while not self._finished:
             try:
                 message = input().lower().strip()
             except EOFError:
                 break
+
             if message == "ex":
                 log("info", "stopping server")
-                self.stop_server()
+                self.stop()
 
             elif message == "rs":
                 log("info", "restarting the server")
-                try:
-                    self.executor.re_execute()
-                    if self.RELOAD_BROWSER:
-                        sleep(self.browser_wait_interval)
-                        helium.refresh()
-
-                except Exception:
-                    try:
-                        log(
-                            "error",
-                            f"browser reload didnt work, retrying in {2 * self.browser_wait_interval} seconds...",
-                        )
-                        sleep(2 * self.browser_wait_interval)
-                        if self.RELOAD_BROWSER:
-                            helium.refresh()
-                    except Exception:
-                        log(
-                            "error",
-                            "browser reload retry failed! make sure you've provided stella the correct url to listen at. waiting for file changes or `rb`/`rs` input to restart...",
+                self.trigger_queue.cancel_all()
+                self.executor.re_execute()
+                if self.RELOAD_BROWSER:
+                    self.trigger_queue.add(
+                        Trigger(
+                            action=self._browser_reloader,
+                            when=datetime.now() + self.browser_wait_delta,
+                            error_handler=self._browser_reload_error_handler,
+                            value=self.browser_wait_delta,
                         )
+                    )
 
             elif message == "rb":
                 if self.RELOAD_BROWSER:
                     try:
                         log("info", "trying to reload browser window")
-                        helium.refresh()
+                        self.driver.refresh()
                     except Exception:
                         log("error", "unable to refresh browser window")
                 else:
-                    log("stella", "no browser URL is configured, can't refresh")
+                    log(
+                        "stella",
+                        "no browser URL is configured, can't refresh browser window",
+                    )
 
-            # ! too much black magic required to have configuration reloaded
-            # ! it's because stop_server calls os._exit and that stops the entire progam because there
-            # ! is no way to gracefully stop the input thread
-            # ? maybe use timeout input or process
-            # elif message == "rc":
-            #     log(
-            #         "stella",
-            #         "attempting to reload configuration, stopping existing commands and browser windows",
-            #     )
-            #     self.stop_server()
-            #     cfg_file, new_config = load_configuration_handle_errors(
-            #         self.config_file
-            #     )
-            #     self.__init__(new_config, self.script.name, cfg_file)  # type: ignore
-            #     # ignore above because if self.script was None program would've already quit in __init__
-            #     self.executor.start()
-            #     self.restart()
+            elif message == "rc":
+                log(
+                    "stella",
+                    "attempting to reload configuration, stopping existing commands and browser windows",
+                )
+                self.stop()
+                cfg_file, new_config = load_configuration_handle_errors(
+                    self.config_file
+                )
+                self.__init__(new_config, self.script.name, cfg_file)  # type: ignore
+                # ignore above because if self.script was None program would've already quit in __init__
+                self.start()
 
-    def stop_server(self):
+    def stop(self):
         try:
+            self.trigger_queue.cancel_all()
             self.executor.close()
             if self.RELOAD_BROWSER:
-                helium.kill_browser()
+                if getattr(self, "driver", "!nope!") != "!nope!":
+                    # condition to check if driver was initialized
+                    self.driver.quit()
         except Exception as e:
             log(
                 "error",
                 "an error occured while stopping the server, this should never happen.",
             )
             exception(e)
         finally:
-            os._exit(0)
+            self._finished = True
+            if self.observer.is_alive():
+                self.observer.stop()
+                self.observer.join()
 
-    def start_server(self) -> None:
+    def start(self) -> None:
         """
         Starts the server. All reloading and stuff is done here.
         """
         log("stella", "starting stella")
         log(
             "stella",
             f"using config file located at `{self.config_file}`",
@@ -251,11 +336,17 @@
             f"executing `{self.executor.command_to_display if self.script else ''}` {browser_text if self.RELOAD_BROWSER else ''}",
         )
         browser_text = ", `rb` to refresh browser page"
         log(
             "stella",
             f"input `rs` to manually restart the server{browser_text if self.RELOAD_BROWSER else ''} & `ex` to stop the server",
         )
-        input_thread = Thread(target=self.manual_input)
+        # running the input thread as daemon would allow the program
+        #  to exit even if the input thread is still running
+        input_thread = Thread(target=self.manual_input, daemon=True)
         input_thread.start()
         self.executor.start()
-        self.restart()
+        if self.RELOAD_BROWSER:
+            self._start_browser()
+
+        self.observer.start()
+        # self.restart()
```

### Comparing `stellapy-0.2.1/stellapy/stella.py` & `stellapy-0.3.0/stellapy/stella.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import click
 
 from stellapy.configuration import Configuration, load_configuration_handle_errors
 from stellapy.logger import log
 from stellapy.reloader import Reloader
 
 NAME = "stella"
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 # , help = "The url to listen to on the browser. Example: localhost:5000", prompt = "Enter the URL to listen to on the browser"
 # , help = "The command to execute on a file change. Example: python3 app.py", prompt = "Enter the command to execute on a file change"
 
 
 @click.group("stella")
 @click.version_option(VERSION, prog_name=NAME)
@@ -49,25 +49,25 @@
     Alternatively, an environment variable named `STELLA_CONFIG` can also be set for the same.
     This is generally not required since stella automatically attempts to find `stella.yml` file in the
     current directory and its parents.
 
     Examples: \n
     $ stella run  // runs the default script from config \n
     $ stella run [script_name]  // runs the given script from config \n
-    $ stella run [script_name] --config-file /path/to/configfile.yml
+    $ stella run [script_name] --config-file /path/to/stella.yml
     """
     config_file_used, config = load_configuration_handle_errors(config_file)
     reloader = None
     try:
         reloader = Reloader(config, script, config_file_used)
-        reloader.start_server()
+        reloader.start()
     except KeyboardInterrupt:
         log("info", "stopping server")
         if reloader:
-            reloader.stop_server()
+            reloader.stop()
     except Exception as e:
         log("error", "fatal: unknown error in reloader")
         exception(e)
 
 
 @main.command("init")
 def init():
@@ -87,15 +87,15 @@
         with open("./stella.yml", "w", encoding="utf-8") as f:
             f.write(Configuration.default().to_yaml())
         log("info", "stella.yml file sucessfully written")
 
     except PermissionError:
         log(
             "error",
-            "unable to write stella.yml file in the current directory: not enough persmissions",
+            "unable to write stella.yml file in the current directory: not enough permissions",
         )
 
     except Exception as e:
         log("error", "an unknown error occured!")
         exception(e)
```

### Comparing `stellapy-0.2.1/stellapy/walker.py` & `stellapy-0.3.0/stellapy/walker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,76 @@
-import os
-from logging import exception
+from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Iterable
+from typing import Callable, Iterable
 
 import gitignorefile
-
-IGNORE_PATTERN = None
-INCLUDE_PATTERN = None
+from watchdog.events import (
+    EVENT_TYPE_CLOSED,
+    EVENT_TYPE_OPENED,
+    FileSystemEvent,
+    FileSystemEventHandler,
+)
 
 
 def get_ignore_include_patterns(include_only: Iterable[str] | None):
-    global IGNORE_PATTERN, INCLUDE_PATTERN
-    if IGNORE_PATTERN and INCLUDE_PATTERN:
-        # if they are already cached
-        return IGNORE_PATTERN, INCLUDE_PATTERN
-
     ignore_filepath = find_ignore_file()
     ignore_match = (
         gitignorefile.parse(ignore_filepath) if ignore_filepath else lambda _: False
     )
     include_match = (
         gitignorefile._IgnoreRules(
             [gitignorefile._rule_from_pattern(pattern) for pattern in include_only],
             ".",
         ).match
         if include_only
         else lambda _: True
     )
 
-    # compute patterns once and cache them
-    IGNORE_PATTERN = ignore_match
-    INCLUDE_PATTERN = include_match
-    return IGNORE_PATTERN, INCLUDE_PATTERN
+    return ignore_match, include_match
 
 
-def walk(include_only: Iterable[str] | None, follow_symlinks: bool):
+class GitignoreMatchingEventHandler(FileSystemEventHandler):
     """
-    The `walk` function recursively searches for all files in the project returns a list of
-    valid files.
+    Subclass of `watchdog.FileSystemEventHandler` which implements gitignore-style
+    pattern matching.
     """
 
-    try:
-        ignore_match, include_match = get_ignore_include_patterns(include_only)
-        # project_files = []
-        for root, _, files in os.walk(".", topdown=True, followlinks=follow_symlinks):
-            if ".git" in root or ignore_match(root):
-                continue
-
-            for file in files:
-                if ignore_match(root):
-                    continue
-                if include_match(file):
-                    yield os.path.join(root, file)
-                # project_files.append(os.path.join(root, file))
-
-        # return project_files
-
-    except Exception as e:
-        exception(e)
-        return []
-
-
-def get_file_content(filepath: str) -> str:
-    """
-    `get_file_content` returns the content of the file. Ignores binary files.
-    """
-    try:
-        with open(filepath, encoding="utf-8") as f:
-            fc = f.read()
-
-        return fc
-
-    except UnicodeDecodeError:
-        # binary file, ignore
-        return ""
-
-    except Exception as e:
-        exception(e)
-        return ""
+    def __init__(
+        self,
+        include_only: Iterable[str] | None,
+        poll_interval: float,
+        callback: Callable[[], None],
+    ) -> None:
+        super().__init__()
+        self.ignore_match, self.include_match = get_ignore_include_patterns(
+            include_only
+        )
+        self.poll_interval = poll_interval
+        self.callback_fn = callback
+        self.last_event_time = datetime.now()
+
+    def on_any_event(self, event: FileSystemEvent) -> None:
+        # only respond to events after a certain threshold
+        if datetime.now() - self.last_event_time > timedelta(
+            milliseconds=self.poll_interval
+        ):
+            super().on_any_event(event)
+            self.callback_fn()
+            self.last_event_time = datetime.now()
+
+    def dispatch(self, event: FileSystemEvent) -> None:
+        no_dispatch_conditions = {
+            self.ignore_match(event.src_path),
+            ".git" in event.src_path,
+            event.event_type in (EVENT_TYPE_OPENED, EVENT_TYPE_CLOSED),
+            not self.include_match(event.src_path),
+        }
+        if any(no_dispatch_conditions):
+            return
+        return super().dispatch(event)
 
 
 def find_ignore_file(base_dir: str | None = None) -> str | None:
     """
     Recursively tries to find the `stella.ignore` in current directory and its parents until it's found,
     if not, reverts to `.gitignore`.
     """
@@ -115,13 +104,13 @@
         return __find_file_recursively(filename, str(cwd.parent))
 
 
 if __name__ == "__main__":
     print(find_ignore_file())
     print(find_config_file())
     input()
-    for i in walk(["*.py"], False):
-        ...
-        print(i)
-        # input()
-        # print(get_file_content(i))
-        # input()
+    # for i in walk(["*.py"], False):
+    #     ...
+    #     print(i)
+    #     input()
+    #     print(get_file_content(i))
+    #     input()
```

### Comparing `stellapy-0.2.1/PKG-INFO` & `stellapy-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellapy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Streamline your web dev experience with stella - reload for the terminal as well as browser.
 Home-page: https://github.com/shravanasati/stellapy
 License: MIT
 Keywords: web dev,development,website,python,cli,stella,reloader,walker,executor,helium,selenium,automation
 Author: Shravan Asati
 Author-email: dev.shravan@protonmail.com
 Requires-Python: >=3.10,<4.0
@@ -19,74 +19,75 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: gitignorefile (>=1.1.2,<2.0.0)
-Requires-Dist: helium (>=4.0.0,<5.0.0)
 Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: ruamel-yaml (>=0.18.5,<0.19.0)
+Requires-Dist: selenium (>=4.21.0,<5.0.0)
+Requires-Dist: watchdog (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://github.com/shravanasati/stellapy#readme
 Project-URL: Repository, https://github.com/shravanasati/stellapy
 Description-Content-Type: text/markdown
 
 # stella
 
 ![stella_demo](assets/stella.gif)
 
 [![Downloads](https://pepy.tech/badge/stellapy)](https://pepy.tech/project/stellapy)
 
 stella is a command line utility made for streamlining web development experience. 
 It is able to reload server as well as the browser page on every file change.
-Although you can use it like any other live reload tool - with builtin `.gitignore` detection and following, along with several other features like multiple command execution, and the npm-scripts like interface.
+You can use it like any other live reload tool too - with builtin `.gitignore` detection and obedience, along with several other features like multiple command execution, and the npm-scripts like interface.
 
 <br>
 
 
 ## 📝 Table of Contents
 - [Installation](#%EF%B8%8F-installation)
 - [Motivation](#-motivation)
 - [How does stella work?](#%EF%B8%8F-how-does-stella-work)
 - [Usage](#-usage)
-- [Changelog](#-changelog)
 - [Versioning](#-versioning)
 - [Licensing](#-licensing)
 - [Contribution](#-contribution)
 
 
 <br>
 
 
 ## ⚡️ Installation
 
 Using [pipx](https://pypa.github.io/pipx/) (recommended):
 ```
 pipx install stellapy
+# pipx upgrade stellapy to upgrade
 ```
 
 On Windows:
 ```
-pip install stellapy
+pip install -U stellapy
 ```
 
 On Linux/MacOS:
 ```
-pip3 install stellapy
+pip3 install -U stellapy
 ```
 
 
 <br>
 
 
 
 ## 💫 Motivation
 
-I wanted a CLI that could live reload the browser page as well as live restart the server. I tried to find such a tool, but didn't find one. So I made stella - that could reload backend as well as frontend code. Also the builtin debug modes of web frameworks sucked.
+I wanted a CLI that could live reload the browser page as well as live restart the server. I tried to find such a tool, but didn't find one. So I made stella - that could reload backend as well as frontend code. Also the builtin "debug modes" of web frameworks sucked.
 
 <br>
 
 ## ⚙️ How does stella work?
 
 stella continuously watches for file changes in the project, while respecting the gitignore file and whenever a change is made, it kills the existing process and spawns a new process using subprocess. What about browser reload? It uses selenium to accomplish that.
 
@@ -121,30 +122,32 @@
 
 This yaml file comes with a schema which can be utilized by yaml language servers to provide autocompletion and validation to make sure the config is correct.
 
 ### Configuration
 
 Let's quickly go over the config options:
 
- - **`browser`**: This option specifies the browser to use when `url` is given. The only valid options for browser currently are `firefox` and `chrome`.
+ - **`browser`**: This option specifies the browser to use when `url` is given. The only valid options for browser currently are `firefox`, `chrome`, `edge` and `safari`.
 
  - **`include_only`**: The list of gitignore-style patterns to consider for live reload. This will be used along with the ignore file (`stella.ignore` or `.gitignore`) to match files. eg. `include_only: ["*.py", "*.env"]`.
 
- - **`poll_interval`**: The duration in **milliseconds** to poll the filesystem for changes.
+ - **`poll_interval`**: The duration in **milliseconds** to poll the filesystem for changes. This has been modified past v0.3.0 - it now signifies the threshold duration for which stella should accept changes.
 
  - **`browser_wait_interval`**: This is the duration in **milliseconds** between the execution of given command on the terminal and browser page refresh. This can be used in situations when the server takes some time before it is ready to listen on a given port.
 
- - **`follow_symlinks`**: Boolean value that indicates whether to follow symbolic links encountered in the filesystem.
+ <!-- - **`follow_symlinks`**: Boolean value that indicates whether to follow symbolic links encountered in the filesystem. -->
 
  - **`scripts`**: This the list of npm style scripts that take 4 parameters each.
 
     * `name`: Name of the script. To execute a certain script, use its name in the `stella run SCRIPT_NAME` command. The script named _default_ will be used in case SCRIPT_NAME is not provided. Note that this parameter is **case-insensitive**, for convenience.
 
     * `url`: The URL to listen to on the browser. Set it to an empty string (`''`) if you don't want live reload on the browser. eg. `localhost:8000`.
 
+      > Note: For chrome and edge, you URLs starting with `localhost` won't work, prepend the `url` with a scheme like `http://` or `file://`. Not tested on safari, but if you see `data;` in the address bar, this URL change should fix it.
+
     * `command`: A single command or a list of commands to execute on the terminal. eg.
       ```
       command: python3 app.py
       ```
 
       ```
       command: 
@@ -155,24 +158,21 @@
       If a list of commands are provided, the `shell` will be considered `true` even if it's `false`.
 
     * `shell`: **Boolean** value which indicates whether to execute commands inside a shell context (like bash, powershell, zsh...) or as an independent process. This is useful if you want to execute shell scripts directly without invoking the shell interpreter. On Windows, powershell is used as shell (instead of cmd). On Linux and MacOS, the shell used is determined by `SHELL` environment variable. If it's not present, `/bin/sh` will be used.
 
 
 ### Ignore
 
-Polling a filesystem for changes can be lengthy in case of big projects.
-Even worse when dependencies are vendored within the project, like python virtual environments or include directories in c/c++.
-
-Therefore, you can create a `stella.ignore` file in the project with gitignore-style patterns to exclude certain directories and files to consider.
+You can create a `stella.ignore` file in the project with gitignore-style patterns to exclude certain directories and files to watch.
 
 Otherwise, `.gitignore` also just works, and is the recommended way.
 
 However, `stella.ignore` will be the first one that will be searched for. If it's not found, stella will resort to `.gitignore`.
 
-Ignore patterns are cached once stella is started, similar to the stella configuration. If you change either of them, in order to see the desired changes, you need stop stella and run it again.
+Ignore patterns are cached once stella is started, similar to the stella configuration. If you change either of them, in order to see the desired changes, you need to either type `rc` and press enter or stop stella and run it again.
 
 
 ### run
 
 ```
 stella run SCRIPT_NAME
 stella run SCRIPT_NAME --config-file /path/to/config/stella.yml
@@ -183,17 +183,21 @@
 
 An optional `--config-file` (`-c` for short) flag can be used to specify the config file to be used. 
 Alternatively, an environment variable named `STELLA_CONFIG` can be set for the same.
 
 If not provided, stella will attempt to find `stella.yml` in the current directory or its parent folders until its found.
 
 
-While stella is running, you can input `rs` to restart the server and refresh the browser page manually, and `rb` only to refresh the browser page.
+While stella is running, you can input `rs` to restart the server and refresh the browser page manually, and `rb` to refresh the browser page.
+
+Since *v0.3.0*, you can also reload the stella configuration by typing `rc` and pressing enter. This will close the existing browser window and the running process, and restart the same script with the stella configuration.
 
-To stop stella, input `ex`. It will close the browser as well as kill the running process gracefully.
+To stop stella, input `ex`. It will close the browser as well as kill the running process gracefully (it sends `SIGTERM` on Unix based systems and `CTRL_BREAK_EVENT` on Windows).
+
+If an error is encountered on refreshing the browser page (an event which can happen often, primarily due to server taking a long time to restart or the command failed to execute successfully), stella will retry with the exponential backoff strategy (2^n) until the browser refresh is successfull or a new change is detected.
 
 <br>
 
 
 ## 📄 Licensing
 
 License © 2021-Present Shravan Asati
@@ -201,7 +205,8 @@
 This repository is licensed under the MIT license. See [LICENSE](LICENSE) for details.
 
 <br>
 
 ## 👥 Contribution
 
 Contribution is more than welcome. For more guidelines on contributing to stella, refer [CONTRIBUTING.md](CONTRIBUTING.md).
+
```

