# Comparing `tmp/schelp_watch-0.0.1.tar.gz` & `tmp/schelp_watch-0.0.2.tar.gz`

## Comparing `schelp_watch-0.0.1.tar` & `schelp_watch-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     8540 2020-02-02 00:00:00.000000 schelp_watch-0.0.1/schelp_watch/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 schelp_watch-0.0.1/schelp_watch/__main__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 schelp_watch-0.0.1/.gitignore
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 schelp_watch-0.0.1/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 schelp_watch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 schelp_watch-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     7807 2020-02-02 00:00:00.000000 schelp_watch-0.0.2/schelp_watch/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 schelp_watch-0.0.2/schelp_watch/__main__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 schelp_watch-0.0.2/.gitignore
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 schelp_watch-0.0.2/README.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 schelp_watch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 schelp_watch-0.0.2/PKG-INFO
```

### Comparing `schelp_watch-0.0.1/schelp_watch/__init__.py` & `schelp_watch-0.0.2/schelp_watch/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 import sys
 from os.path import relpath, abspath, join, dirname, splitext, exists
 from os import getcwd, walk
 import subprocess
 import logging
 from time import sleep
-from watchdog.observers import Observer
-from watchdog.events import PatternMatchingEventHandler
 from argparse import ArgumentParser
+from watchfiles import watch, Change
 
-patterns = ["*.schelp"]
-ignore_patterns = []
-ignore_directories = []
 
 class ScLang:
 
     def __init__(self, sclangCommand="sclang", sclangConfig=None):
         self.__sclang = None
         self.executable = sclangCommand
         self.config = sclangConfig
         self.showingHelpBrowser = False
 
-    def start (self, hide_sc_output=False):
+    def start(self, hide_sc_output=False):
         if self.running():
             return
 
         sclangArgs = [self.executable, "-i", "schelp-watch"]
-        if(self.config):
+        if self.config:
             sclangArgs += ["-al", self.config]
 
         out = subprocess.PIPE if hide_sc_output else None
         self.__sclang = subprocess.Popen(
-                sclangArgs,
-                bufsize=0,
-                stdin=subprocess.PIPE,
-                stdout=out,
-                stderr=subprocess.STDOUT,
-                encoding="utf-8",
-                close_fds=True)
+            sclangArgs,
+            bufsize=0,
+            stdin=subprocess.PIPE,
+            stdout=out,
+            stderr=subprocess.STDOUT,
+            encoding="utf-8",
+            close_fds=True)
         self.stdout = self.__sclang.stdout
         self.stdin = self.__sclang.stdin
 
     def stop(self):
         if self.running():
             self.stdin.close()
             self.__sclang.wait()
@@ -48,177 +44,169 @@
 
     def running(self):
         return (self.__sclang is not None) and (self.__sclang.poll() is None)
 
     def evaluate(self, code, silent=False):
         code = code + ("\x1b" if silent else "\x0c")
         self.stdin.write(code)
-        self.stdin.flush();
+        self.stdin.flush()
 
     def initSCDoc(self, helpSourceDir, helpTargetDir, extension):
         self.helpSourceDir = helpSourceDir
         # for extensions: add include path
         if extension:
             self.evaluate(f"LanguageConfig.addIncludePath(\"{helpSourceDir}\")")
         else:
-            self.evaluate(f'SCDoc.helpSourceDir = "{helpSourceDir}"');
+            self.evaluate(f'SCDoc.helpSourceDir = "{helpSourceDir}"')
 
         if helpTargetDir:
-            self.evaluate(f'SCDoc.helpTargetDir = "{helpTargetDir}"');
+            self.evaluate(f'SCDoc.helpTargetDir = "{helpTargetDir}"')
         else:
             self.makeTemporaryHelpTarget()
 
-        self.evaluate("SCDoc.indexAllDocuments(false)");
+        self.evaluate("SCDoc.indexAllDocuments(false)")
 
     def makeTemporaryHelpTarget(self):
         self.evaluate('''
-          var target = PathName.tmp +/+ "schelp-watch";
-          if (File.exists(target)) { File.deleteAll(target) };
-          File.copy(SCDoc.helpTargetDir, target);
-          SCDoc.helpTargetDir = target;
-          "SCDoc temporary target: %".format(SCDoc.helpTargetDir)
+var target = PathName.tmp +/+ "schelp-watch";
+if (File.exists(target)) { File.deleteAll(target) };
+File.copy(SCDoc.helpTargetDir, target);
+SCDoc.helpTargetDir = target;
+"SCDoc temporary target: %".format(SCDoc.helpTargetDir)
           ''')
 
     def recompileScHelp(self, path):
+        path = relpath(path, self.helpSourceDir)
+        logging.info("reloading %s", path)
+
         sccode = f'''
-            var entry = SCDoc.parseFileMetaData("{self.helpSourceDir}","{path}");
-            SCDoc.parseAndRender(entry);
+var entry = SCDoc.parseFileMetaData("{self.helpSourceDir}","{path}");
+if (entry.notNil) {{
+    SCDoc.parseAndRender(entry);
+    {'HelpBrowser.goTo(entry.destPath)' if self.showingHelpBrowser else ''}
+}} {{
+    warn("{path}: entry not found")
+}}
         '''
-        if self.showingHelpBrowser:
-            sccode = sccode + 'HelpBrowser.goTo(entry.destPath);'
         self.evaluate(sccode)
 
     def openHelp(self):
         self.showingHelpBrowser = True
         self.evaluate("HelpBrowser.instance")
 
 
-class ScHelpHandler(PatternMatchingEventHandler):
-
-    def __init__(self, sclang, helpSourceDir, wait_for_process=True):
-        super(ScHelpHandler, self).__init__(patterns, ignore_patterns,
-                                                ignore_directories)
-        self.wait_for_process = wait_for_process
-        self.sclang = sclang
-        self.helpSourceDir = helpSourceDir
-
-    def on_any_event(self, event):
-        from string import Template
-
-        if event.is_directory:
-            return
-
-        if event.event_type not in ['created','modified','moved']:
-            return
-
-        file_path = event.dest_path if event.event_type == 'moved' else event.src_path
-        if splitext(file_path)[1] != ".schelp":
-            return
-
-        relative_path = relpath(file_path, self.helpSourceDir)
-        logging.info("(%s) %s", event.event_type, relative_path);
-        self.sclang.recompileScHelp(relative_path)
-
 def detectBuildMode(path):
-    sclangCommand = join(path, "lang", "sclang")
-    sclangConfig = join(path, "build_sclang.cfg")
-    helpSourceDir = join(path, "..", "HelpSource")
-    found = [exists(p) for p in [sclangCommand, sclangConfig, helpSourceDir]]
-    return not False in found
+    '''
+    check if path looks like we are working at the supercollider git repo
+    '''
+    for p in [
+        join(path, "lang", "sclang"),
+        join(path, "build_sclang.cfg"),
+        join(path, "..", "HelpSource")
+    ]:
+        if not exists(p):
+            return False
+    return True
+
 
 def has_schelp_files(path):
-    for root,_,files in walk(path):
+    for root, _, files in walk(path):
         for f in files:
             if f.endswith(".schelp"):
                 print(f"found some at {root}")
                 return True
     return False
 
+
 def parse_arguments():
     parser = ArgumentParser(description='''
 Watches .schelp files, rebuilding and previewing Help files on source changes.
 It can be used in build mode (for editing help files in SuperCollider's main repo), or extension mode (for Quarks and Extensions help files). If no mode is provided, schelp-watch will try to detect it automatically.
     ''')
 
     arg_group_mode = parser.add_mutually_exclusive_group()
     arg_group_mode.add_argument('--build', '-b', dest="mode", action="store_const", const="build",
-        help='specify "build mode": will find sclang, config and HelpSource from PATH (useful to work on sc main codebase). Use it when editing help files in sc main repo')
+                                help='specify "build mode": will find sclang, config and HelpSource from PATH (useful to work on sc main codebase). Use it when editing help files in sc main repo')
     arg_group_mode.add_argument('--extension', '-e', dest="mode", action="store_const", const="extension",
-        help='specify "extension mode": adds PATH to SuperCollider default HelpSource paths. Use it when editing Quarks and Extensions.')
+                                help='specify "extension mode": adds PATH to SuperCollider default HelpSource paths. Use it when editing Quarks and Extensions.')
 
     parser.add_argument('path', metavar="PATH", type=str, nargs="?", default=getcwd(),
                         help="in build mode: build folder; in extension mode: extension folder (default: current directory)")
 
     parser.add_argument('--target', metavar="helpTarget", type=str,
-            help='Optional: where to save compiled HelpFiles (default: make a temporary folder)')
+                        help='Optional: where to save compiled HelpFiles (default: make a temporary folder)')
     parser.add_argument('--sclang', metavar="sclangCommand", type=str, default="sclang",
-            help='Optional: sclang command (default: sclang)')
+                        help='Optional: sclang command (default: sclang)')
     parser.add_argument('--config', metavar="sclangConfig", type=str,
-            help='Optional: sclang config file')
+                        help='Optional: sclang config file')
     parser.add_argument('--quiet', '-q', action="store_true",
-            help='hide sclang output')
+                        help='hide sclang output')
     parser.add_argument('--no-preview', '-n', action="store_true",
-            help='write to target, but don\'t open HelpBrowser')
+                        help='write to target, but don\'t open HelpBrowser')
 
     return parser.parse_args()
 
+
 def main():
+
     logging.addLevelName(logging.WARNING, f"\033[1;33m{logging.getLevelName(logging.WARNING)}\033[1;0m")
     logging.addLevelName(logging.INFO, f"\033[1;34m{logging.getLevelName(logging.INFO)}\033[1;0m")
     logging.addLevelName(logging.ERROR, f"\033[1;31m{logging.getLevelName(logging.ERROR)}\033[1;0m")
     logging.basicConfig(level=logging.INFO,
                         format='[%(asctime)s] %(levelname)s %(message)s',
                         datefmt='%H:%M:%S')
 
     args = parse_arguments()
     srcDir = abspath(args.path)
+
     mode = args.mode
+    # autodetect build mode for srcDir or srcDir/build
     if mode is None:
         build = detectBuildMode(srcDir)
         if not build and detectBuildMode(join(srcDir, "build")):
             build = True
             srcDir = join(srcDir, "build")
         mode = 'build' if build else 'extension'
-
     logging.info(f"Starting in {mode} mode at '{srcDir}'")
 
     if mode == "build":
+        helpSourceDir = join(srcDir, "..", "HelpSource")
         sclangCommand = join(srcDir, "lang", "sclang")
         sclangConfig = join(srcDir, "build_sclang.cfg")
-        helpSourceDir = join(srcDir, "..", "HelpSource")
     else:
-        logging.info(f"looking for schelp files...")
+        logging.info("looking for schelp files...")
         if not has_schelp_files(srcDir):
-            logging.error("couldn't find any .schelp file in {srcDir}")
+            logging.error(f"couldn't find any .schelp file in {srcDir}")
             exit(1)
         helpSourceDir = srcDir
         sclangCommand = args.sclang
         sclangConfig = args.config
 
     helpTargetDir = abspath(args.target) if args.target else None
-
     logging.info(f"HelpSource: {helpSourceDir}");
+
     if sclangConfig is not None:
         logging.info(f"sclang config: {sclangConfig}")
     logging.info("Starting sclang ({})".format(sclangCommand));
     sclang = ScLang(sclangCommand, sclangConfig)
     sclang.start(args.quiet)
+
     logging.info("Initializing SCDoc");
     sclang.initSCDoc(helpSourceDir, helpTargetDir, mode == 'extension')
     if not args.quiet:
         logging.info("Opening SC Help");
         sclang.openHelp()
 
-    # file watcher loop
-    handler = ScHelpHandler(sclang, helpSourceDir)
-    observer = Observer()
-    observer.schedule(handler, helpSourceDir, recursive=True)
-    observer.start()
-    try:
-        while True:
-            sleep(1)
-    except KeyboardInterrupt:
-        observer.stop()
-    observer.join()
+    def schelp_filter(change, path):
+        return path.endswith(".schelp") and change != Change.deleted
+
+    for changes in watch(helpSourceDir,
+                         watch_filter=schelp_filter,
+                         recursive=True, raise_interrupt=False):
+        print(changes)
+        paths = set(p for _, p in changes)
+        for p in paths:
+            sclang.recompileScHelp(p)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `schelp_watch-0.0.1/README.md` & `schelp_watch-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # schelp-watch
 Live preview and autoreload for editing SuperCollider HelpFiles.
 
+## Installation
+```
+pipx install schelp-watch
+```
+
 ## How it works
 schelp-watch runs a sclang process (with default config), to rebuild Help files whenever their source changes. It won't pollute your current HelpFiles cache, because by default it compiles to a temporary one.
 
 The intended workflow is to freely edit HelpSources, and quickly see how they look in SuperCollider HelpBrowser. It can be used for editing SuperCollider main repo's HelpFiles, and as well for Extensions and Quarks.
 
-## Dependencies
-- Python 3
-- [watchdog](https://github.com/gorakhargosh/watchdog/) `$ pip install watchdog`
-
 ## Usage
-From version 2, schelp-watch can be used with no arguments. Just cwd to your Extension folder, or to your supercollider's main repo clone, and run:
+schelp-watch can be used with no arguments. Just cd to your Extension folder, or to your supercollider's main repo clone, and run:
 ```
-schelp
+schelp-watch
 ```
 It will detect build or extension mode, watch your .schelp files, run SC HelpBrowser and autoreload.
 
 ### build mode
 Use this for editing HelpSource in SuperCollider main repo:
 - it needs to find a `build` folder, if not provided with one
 - it will then use the `sclang` binary from that `build folder`, and also its `sclang_config` file.
@@ -62,10 +63,14 @@
                         Optional: sclang command (default: sclang)
   --config sclangConfig
                         Optional: sclang config file
   --quiet, -q           hide sclang output
   --no-preview, -n      write to target, but don't open HelpBrowser
 ```
 
+## Dependencies
+- Python 3
+- [watchfiles](https://github.com/samuelcolvin/watchfiles)
+
 ## Known issues
 - Still completely untested on mac and windows. Most certainly requires more work for those platforms.
 - The most "secure" way to use this tool is to make sure it's running an sclang instance that was compiled together with SCClassLibrary and HelpSource in use. This ensures sclang will be able to compile the class library, and SCDoc will be able to find all methods that are defined in the HelpSource. Errors can happen when, for instance, using an older version of sclang with the SCClassLibrary and/or HelpSource from git's develop branch. This is why this tool's `build mode` was introduced.
```

### Comparing `schelp_watch-0.0.1/pyproject.toml` & `schelp_watch-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 [project]
 name = "schelp-watch"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Gianluca Elia", email="elgiano@gmail.com" },
 ]
 description = "Live preview and autoreload for editing SuperCollider HelpFiles."
 readme = "README.md"
 license = "Unlicense"
 requires-python = ">=3.8"
-dependencies = [
-    "watchdog",
-]
+dependencies = [ "watchfiles" ]
 
 [project.scripts]
 schelp-watch = "schelp_watch:main"
 
 [project.urls]
 Homepage = "https://github.com/elgiano/schelp-watch"
 Issues = "https://github.com/elgiano/schelp-watch/issues"
```

### Comparing `schelp_watch-0.0.1/PKG-INFO` & `schelp_watch-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.3
 Name: schelp-watch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Live preview and autoreload for editing SuperCollider HelpFiles.
 Project-URL: Homepage, https://github.com/elgiano/schelp-watch
 Project-URL: Issues, https://github.com/elgiano/schelp-watch/issues
 Author-email: Gianluca Elia <elgiano@gmail.com>
 License-Expression: Unlicense
 Requires-Python: >=3.8
-Requires-Dist: watchdog
+Requires-Dist: watchfiles
 Description-Content-Type: text/markdown
 
 # schelp-watch
 Live preview and autoreload for editing SuperCollider HelpFiles.
 
+## Installation
+```
+pipx install schelp-watch
+```
+
 ## How it works
 schelp-watch runs a sclang process (with default config), to rebuild Help files whenever their source changes. It won't pollute your current HelpFiles cache, because by default it compiles to a temporary one.
 
 The intended workflow is to freely edit HelpSources, and quickly see how they look in SuperCollider HelpBrowser. It can be used for editing SuperCollider main repo's HelpFiles, and as well for Extensions and Quarks.
 
-## Dependencies
-- Python 3
-- [watchdog](https://github.com/gorakhargosh/watchdog/) `$ pip install watchdog`
-
 ## Usage
-From version 2, schelp-watch can be used with no arguments. Just cwd to your Extension folder, or to your supercollider's main repo clone, and run:
+schelp-watch can be used with no arguments. Just cd to your Extension folder, or to your supercollider's main repo clone, and run:
 ```
-schelp
+schelp-watch
 ```
 It will detect build or extension mode, watch your .schelp files, run SC HelpBrowser and autoreload.
 
 ### build mode
 Use this for editing HelpSource in SuperCollider main repo:
 - it needs to find a `build` folder, if not provided with one
 - it will then use the `sclang` binary from that `build folder`, and also its `sclang_config` file.
@@ -74,10 +75,14 @@
                         Optional: sclang command (default: sclang)
   --config sclangConfig
                         Optional: sclang config file
   --quiet, -q           hide sclang output
   --no-preview, -n      write to target, but don't open HelpBrowser
 ```
 
+## Dependencies
+- Python 3
+- [watchfiles](https://github.com/samuelcolvin/watchfiles)
+
 ## Known issues
 - Still completely untested on mac and windows. Most certainly requires more work for those platforms.
 - The most "secure" way to use this tool is to make sure it's running an sclang instance that was compiled together with SCClassLibrary and HelpSource in use. This ensures sclang will be able to compile the class library, and SCDoc will be able to find all methods that are defined in the HelpSource. Errors can happen when, for instance, using an older version of sclang with the SCClassLibrary and/or HelpSource from git's develop branch. This is why this tool's `build mode` was introduced.
```

