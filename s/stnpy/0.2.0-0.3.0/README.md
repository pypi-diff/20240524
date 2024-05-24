# Comparing `tmp/stnpy-0.2.0.tar.gz` & `tmp/stnpy-0.3.0.tar.gz`

## Comparing `stnpy-0.2.0.tar` & `stnpy-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 stnpy-0.2.0/publish.sh
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/.gitignore
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/other.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/stnpy.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/workspace.xml
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 stnpy-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stnpy-0.2.0/src/stnpy/__init__.py
--rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 stnpy-0.2.0/src/stnpy/stn.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 stnpy-0.2.0/tst/test.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 stnpy-0.2.0/tst/resources/STN_R_easy_results.csv
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 stnpy-0.2.0/tst/resources/easy.txt
--rw-r--r--   0        0        0 56290609 2020-02-02 00:00:00.000000 stnpy-0.2.0/tst/resources/stn.csv
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 stnpy-0.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 stnpy-0.2.0/LICENSE
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 stnpy-0.2.0/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 stnpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 stnpy-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 stnpy-0.3.0/publish.sh
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/other.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/stnpy.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    12434 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 stnpy-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stnpy-0.3.0/src/stnpy/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 stnpy-0.3.0/src/stnpy/stn.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 stnpy-0.3.0/tst/test.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 stnpy-0.3.0/tst/resources/STN_R_easy_results.csv
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 stnpy-0.3.0/tst/resources/easy.txt
+-rw-r--r--   0        0        0 56290609 2020-02-02 00:00:00.000000 stnpy-0.3.0/tst/resources/stn.csv
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 stnpy-0.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 stnpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 stnpy-0.3.0/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 stnpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 stnpy-0.3.0/PKG-INFO
```

### Comparing `stnpy-0.2.0/.idea/workspace.xml` & `stnpy-0.3.0/.idea/workspace.xml`

 * *Files 14% similar despite different names*

#### Comparing `stnpy-0.2.0/.idea/workspace.xml` & `stnpy-0.3.0/.idea/workspace.xml`

```diff
@@ -1,19 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="00025ca8-29d7-4bd3-ab21-b1b38045bd82" name="Changes" comment="Amended">
-      <change afterPath="$PROJECT_DIR$/publish.sh" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/stnpy/stn.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/stnpy/stn.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tst/test.py" beforeDir="false" afterPath="$PROJECT_DIR$/tst/test.py" afterDir="false"/>
-    </list>
+    <list default="true" id="00025ca8-29d7-4bd3-ab21-b1b38045bd82" name="Changes" comment="Added in an &quot;altered nshared&quot; metric."/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -32,29 +27,29 @@
   &quot;associatedIndex&quot;: 7
 }</component>
   <component name="ProjectId" id="2daPBAA6b5N6byYrU8HGvft4CRL"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "Python.stn.executor": "Run",
-    "Python.test.executor": "Run",
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "/home/lauren/git/stnpy",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;Python.stn.executor&quot;: &quot;Run&quot;,
+    &quot;Python.test.executor&quot;: &quot;Run&quot;,
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/home/lauren/git/stnpy&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tst/resources"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tst"/>
     </key>
@@ -133,15 +128,17 @@
       <workItem from="1710489173929" duration="784000"/>
       <workItem from="1710511220071" duration="3399000"/>
       <workItem from="1710583485728" duration="1875000"/>
       <workItem from="1714998854455" duration="20998000"/>
       <workItem from="1715092221967" duration="4175000"/>
       <workItem from="1715262883215" duration="15580000"/>
       <workItem from="1715586395480" duration="8252000"/>
-      <workItem from="1715602400920" duration="1205000"/>
+      <workItem from="1715602400920" duration="1665000"/>
+      <workItem from="1715604467102" duration="178000"/>
+      <workItem from="1715871104218" duration="12000"/>
     </task>
     <task id="LOCAL-00001" summary="Bug fixes
 
 Sometimes when importing the STN data, the import function will struggle due to being unable to guess the type of the columns. Seeing as the columns are fixed type, I have specified them on import. But, I've also given the option to pass them on invocation.">
       <option name="closed" value="true"/>
       <created>1710244240647</created>
       <option name="number" value="00001"/>
@@ -208,15 +205,23 @@
       <option name="closed" value="true"/>
       <created>1715590603638</created>
       <option name="number" value="00008"/>
       <option name="presentableId" value="LOCAL-00008"/>
       <option name="project" value="LOCAL"/>
       <updated>1715590603638</updated>
     </task>
-    <option name="localTasksCounter" value="9"/>
+    <task id="LOCAL-00009" summary="Added in an &quot;altered nshared&quot; metric.">
+      <option name="closed" value="true"/>
+      <created>1715603633461</created>
+      <option name="number" value="00009"/>
+      <option name="presentableId" value="LOCAL-00009"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715603633461</updated>
+    </task>
+    <option name="localTasksCounter" value="10"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -236,25 +241,15 @@
     <MESSAGE value="General bug fixes
 
 - wasn't detecting if `best_fit` was present correctly
 - wasn't selecting indexes correctly"/>
     <MESSAGE value="Allowing &quot;close enough&quot; to best fit to be considered best"/>
     <MESSAGE value="Original"/>
     <MESSAGE value="Amended"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Amended"/>
-  </component>
-  <component name="XDebuggerManager">
-    <breakpoint-manager>
-      <breakpoints>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/src/stnpy/stn.py</url>
-          <line>201</line>
-          <option name="timeStamp" value="1"/>
-        </line-breakpoint>
-      </breakpoints>
-    </breakpoint-manager>
+    <MESSAGE value="Added in an &quot;altered nshared&quot; metric."/>
+    <option name="LAST_COMMIT_MESSAGE" value="Added in an &quot;altered nshared&quot; metric."/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/stnpy$test.coverage" NAME="test Coverage Results" MODIFIED="1715603587375" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tst"/>
     <SUITE FILE_PATH="coverage/stnpy$stn.coverage" NAME="stn Coverage Results" MODIFIED="1715343257343" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/stnpy"/>
   </component>
 </project>
```

### Comparing `stnpy-0.2.0/.idea/inspectionProfiles/Project_Default.xml` & `stnpy-0.3.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `stnpy-0.2.0/src/stnpy/stn.py` & `stnpy-0.3.0/src/stnpy/stn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from statistics import mean
 import numpy as np
 import pandas as pd
 import math
 import networkx as nx
 
+
 class StnPy:
     """
     Example of an STN input file as per the original paper:
 
     Run,Fitness1,Solution1,Fitness2,Solution2
     1,5.0,00620012,5.0,00500002
     1,3.0,00320061,1.0,00250083
@@ -90,15 +91,28 @@
                 create_using=nx.MultiDiGraph
             )
             for node in g.nodes:
                 if g.out_degree(node) == 0:
                     end_nodes.append(node)
                 if g.in_degree(node) == 0:
                     start_nodes.append(node)
+
+            # put run attributes together
+            nx.set_node_attributes(g, values=[run], name="run")
+            run_values = nx.get_node_attributes(g, name="run")
+            existing_values = nx.get_node_attributes(self.graph, name="run")
+            for node_id, run_list in run_values.items():
+                if node_id not in existing_values:
+                    existing_values[node_id] = run_list
+                else:
+                    expanded_list = run_list + existing_values[node_id]
+                    existing_values[node_id] = expanded_list
             self.graph.add_nodes_from(g.nodes)
+            nx.set_node_attributes(self.graph, values=existing_values, name="run")
+
             # `add_edges_from` doesn't honour multi-edges
             for source, target, key in g.edges:
                 if self.graph.has_edge(source, target, key):
                     weight = self.graph.edges[source, target, key]['weight']
                     self.graph.edges[source, target, key]['weight'] = weight + 1
                 else:
                     self.graph.add_edge(source, target, weight=1)
@@ -143,16 +157,16 @@
         return self.etotal
 
     def get_nbest(self):
         if not self._metric_exists(self.nbest):
             self.best_vertexes = [node for node in self.graph.nodes if self.graph.nodes[node]["type"] == "best"]
             self.nbest = len(self.best_vertexes)
             if self.nbest > 0:
-                self.best_strength = sum(
-                    [self.graph.in_degree(n, weight="weight") for n in self.best_vertexes]) / self.nruns
+                self.best_strength = \
+                    (sum([self.graph.in_degree(n, weight="weight") for n in self.best_vertexes]) / self.nruns)
             else:
                 self.best_strength = 0
         return self.nbest
 
     def get_nend(self):
         if not self._metric_exists(self.nend):
             end_vertexes = [node for node in self.graph.nodes if self.graph.nodes[node]["type"] == "end"]
@@ -172,32 +186,40 @@
         self.get_nbest()
         if not self._metric_exists(self.npaths):
             start_vertexes = [node for node in self.graph.nodes if self.graph.nodes[node]["type"] == "start"]
             if self.nbest > 0:
                 paths = []
                 for sn in start_vertexes:
                     for bn in self.best_vertexes:
-                        [paths.append(p) for p in nx.all_shortest_paths(self.graph, sn, target=bn)]
+                        try:
+                            paths += nx.all_shortest_paths(self.graph, sn, target=bn)
+                        except Exception as _:
+                            # no path from source to target
+                            continue
                 paths_len = [len(path) for path in paths]
                 self.npaths = len(paths)
                 self.plength = -1
                 if self.npaths > 0:
                     self.plength = mean(paths_len)
             else:
                 self.npaths = 0
                 self.plength = -1
         return self.npaths
 
     def get_plength(self):
         self.get_npaths()
         return self.plength
 
-    # this nshared is different from the one described in the paper. In the paper, nshared is only valid if more than
-    # one algorithm is being combined in one STN. However, the paper defines nshared to be the number of locations
-    # that are attractive to more than one algorithm, which I feel generalises just as well to the number of locations
-    # that were attractive to more than one individual.
-    #
-    # Therefore, this generalises to number of nodes with in-degree greater or equal to two
     def get_altered_nshared(self):
+        """
+        this nshared is different from the one described in the paper. In the paper, nshared is only valid if more than
+        one algorithm is being combined in one STN. However, the paper defines nshared to be the number of locations
+        that are attractive to more than one algorithm, which I feel generalises just as well to the number of locations
+        that were attractive to more than one run.
+
+        Therefore, this generalises to number of nodes that have been visited by more than one run.
+
+        :return: nshared as described above
+        """
         if not self._metric_exists(self.nshared):
-            self.nshared = len([node for node in self.graph.nodes if self.graph.in_degree(node, weight="weight") >= 2])
+            self.nshared = len([n for n, l in nx.get_node_attributes(self.graph, name="run").items() if len(l) > 1])
         return self.nshared
```

### Comparing `stnpy-0.2.0/tst/test.py` & `stnpy-0.3.0/tst/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     assert g.get_ntotal() == STN_R_values.loc[0]["ntotal"]
     assert g.get_etotal() == STN_R_values.loc[0]["etotal"]
     assert g.get_nbest() == STN_R_values.loc[0]["nend"]
     assert g.get_nend() == STN_R_values.loc[0]["nend"]
     assert round(g.get_best_strength(), 4) == STN_R_values.loc[0]["best-strength"]
     assert g.get_components() == STN_R_values.loc[0]["components"]
     assert g.get_plength() == STN_R_values.loc[0]["plength"]
-    assert g.get_altered_nshared() == 3
+    assert g.get_altered_nshared() == 5
     print("Correctness tests passed")
 
     # I've tested the STN R package and I disagree with it's output for npaths. It uses a distance matrix to calculate
     # the number of paths, but this is incorrect - it can at most count one path per starting node,  even if there are
     # many
     # assert g.get_npaths() == STN_R_values.loc[0]["npaths"]
 
@@ -39,15 +39,15 @@
     print("ntotal: ", g.get_ntotal(), ", etotal: ", g.get_etotal(), ", nbest: ", g.get_nbest(),
           ", nend: ", g.get_nend(), ", best-strength: ", g.get_best_strength(), ", components: ", g.get_components(),
           ", npaths: ", g.get_npaths(), ", plength: ", g.get_plength(), ", nshared: ", g.get_altered_nshared())
 
 
 def run_big_file():
     g = StnPy("resources/stn.csv")
-    g.get_data(delimiter=",", run_numbers=[1])
+    g.get_data(delimiter=",", run_numbers=[1, 2])
     g.create_stn(best_fit=0, use_best_fit_delta=True)
     print("ntotal: ", g.get_ntotal(), ", etotal: ", g.get_etotal(), ", nbest: ", g.get_nbest(),
           ", nend: ", g.get_nend(), ", best-strength: ", g.get_best_strength(), ", components: ", g.get_components(),
           ", npaths: ", g.get_npaths(), ", plength: ", g.get_plength(), ", nshared: ", g.get_altered_nshared())
 
 
 if __name__ == '__main__':
```

### Comparing `stnpy-0.2.0/tst/resources/stn.csv` & `stnpy-0.3.0/tst/resources/stn.csv`

 * *Files identical despite different names*

### Comparing `stnpy-0.2.0/.gitignore` & `stnpy-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stnpy-0.2.0/LICENSE` & `stnpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stnpy-0.2.0/README.md` & `stnpy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `stnpy-0.2.0/pyproject.toml` & `stnpy-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stnpy"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Lauren Hayward", email="hayward.lauren111@gmail.com" },
 ]
 description = "Python port of R STN library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `stnpy-0.2.0/PKG-INFO` & `stnpy-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stnpy
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python port of R STN library
 Project-URL: Homepage, https://github.com/runrunLauren/stnpy
 Project-URL: Bug Tracker, https://github.com/runrunLauren/stnpy/issues
 Author-email: Lauren Hayward <hayward.lauren111@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

