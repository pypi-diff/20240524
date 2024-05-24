# Comparing `tmp/pytransition-0.1.0.tar.gz` & `tmp/pytransition-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransition-0.1.0.tar", last modified: Mon May  6 12:31:23 2024, max compression
+gzip compressed data, was "pytransition-0.1.1.tar", last modified: Thu May 23 13:34:09 2024, max compression
```

## Comparing `pytransition-0.1.0.tar` & `pytransition-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:31:23.365790 pytransition-0.1.0/
--rw-rw-r--   0 scientist  (1000) scientist  (1000)     1080 2024-05-06 12:29:32.000000 pytransition-0.1.0/LICENSE
--rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-06 12:31:23.365790 pytransition-0.1.0/PKG-INFO
--rw-rw-r--   0 scientist  (1000) scientist  (1000)    18480 2024-05-06 12:29:32.000000 pytransition-0.1.0/README.md
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:31:23.365790 pytransition-0.1.0/pyTransition/
--rw-rw-r--   0 scientist  (1000) scientist  (1000)      198 2024-05-06 12:29:32.000000 pytransition-0.1.0/pyTransition/__init__.py
--rw-rw-r--   0 scientist  (1000) scientist  (1000)    12579 2024-05-06 12:29:32.000000 pytransition-0.1.0/pyTransition/transition.py
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:31:23.365790 pytransition-0.1.0/pyTransition.egg-info/
--rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-06 12:31:23.000000 pytransition-0.1.0/pyTransition.egg-info/PKG-INFO
--rw-rw-r--   0 scientist  (1000) scientist  (1000)      300 2024-05-06 12:31:23.000000 pytransition-0.1.0/pyTransition.egg-info/SOURCES.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)        1 2024-05-06 12:31:23.000000 pytransition-0.1.0/pyTransition.egg-info/dependency_links.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)       23 2024-05-06 12:31:23.000000 pytransition-0.1.0/pyTransition.egg-info/requires.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)       19 2024-05-06 12:31:23.000000 pytransition-0.1.0/pyTransition.egg-info/top_level.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)       38 2024-05-06 12:31:23.365790 pytransition-0.1.0/setup.cfg
--rw-rw-r--   0 scientist  (1000) scientist  (1000)     1720 2024-05-06 12:29:32.000000 pytransition-0.1.0/setup.py
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:31:23.365790 pytransition-0.1.0/tests/
--rw-rw-r--   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:29:32.000000 pytransition-0.1.0/tests/__init__.py
--rw-rw-r--   0 scientist  (1000) scientist  (1000)    11783 2024-05-06 12:29:32.000000 pytransition-0.1.0/tests/test_transition.py
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.898708 pytransition-0.1.1/
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)     1080 2024-05-06 12:29:32.000000 pytransition-0.1.1/LICENSE
+-rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-23 13:34:09.898708 pytransition-0.1.1/PKG-INFO
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)    18480 2024-05-06 12:29:32.000000 pytransition-0.1.1/README.md
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.894708 pytransition-0.1.1/pyTransition/
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)      198 2024-05-06 12:29:32.000000 pytransition-0.1.1/pyTransition/__init__.py
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)    14241 2024-05-22 21:47:02.000000 pytransition-0.1.1/pyTransition/transition.py
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.894708 pytransition-0.1.1/pyTransition.egg-info/
+-rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/PKG-INFO
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)      300 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/SOURCES.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)        1 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/dependency_links.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)       23 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/requires.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)       19 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/top_level.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)       38 2024-05-23 13:34:09.898708 pytransition-0.1.1/setup.cfg
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)     1720 2024-05-23 13:33:51.000000 pytransition-0.1.1/setup.py
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.894708 pytransition-0.1.1/tests/
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:29:32.000000 pytransition-0.1.1/tests/__init__.py
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)    12251 2024-05-22 21:47:02.000000 pytransition-0.1.1/tests/test_transition.py
```

### Comparing `pytransition-0.1.0/LICENSE` & `pytransition-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransition-0.1.0/PKG-INFO` & `pytransition-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTransition
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to interact with the Transition API.
 Author: Transition City
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pytransition-0.1.0/README.md` & `pytransition-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytransition-0.1.0/pyTransition/transition.py` & `pytransition-0.1.1/pyTransition/transition.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,30 +19,75 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import requests
 from datetime import time
 import json
+from urllib.parse import urlparse, urlunparse, urlencode, parse_qs
 
 
 class Transition:
     def __init__(self, url, username, password, token=None):
         if url is None or url == "":
             raise ValueError("URL cannot be empty.")
-        self.base_url = url
+
+        # Parse and normalize the URL
+        self.base_url = self.__normalize_url(url)
 
         # To instantiate Transition instance from token only
         if username is None and password is None and token is not None:
             self.token = token
 
         # To instantiate Transition instance from username and password authentication
         else:
             self.token = self.__request_token(username, password)
 
+    @staticmethod
+    def __normalize_url(url):
+        """Normalize the URL.
+
+        Remove extra characters from the URL
+        """
+        parsed_url = urlparse(url)
+        netloc = parsed_url.netloc.lower()
+
+        # Remove port number if we use the standard ones
+        if netloc.endswith(':80') and parsed_url.scheme == 'http':
+            netloc = netloc[:-3]
+        elif netloc.endswith(':443') and parsed_url.scheme == 'https':
+            netloc = netloc[:-4]
+
+        # Remove extra "/"
+        path = parsed_url.path.rstrip('/')
+        normalized_url = urlunparse((parsed_url.scheme, netloc, path, parsed_url.params, parsed_url.query, parsed_url.fragment))
+        return normalized_url
+
+    def build_url(self, path='', params=None):
+        """Construct the full URL with path and params
+
+        Args:
+            path (string): path to add the base url
+            params (dict): parameters to add to the request
+
+        Returns:
+            string: Full url to use in the request
+        """
+        if params is None:
+            params = {}
+
+        parsed_base_url = urlparse(self.base_url)
+        combined_path = parsed_base_url.path.rstrip('/') + '/' + path.lstrip('/')
+        query_params = parse_qs(parsed_base_url.query)
+        query_params.update(params)
+        query_string = urlencode(query_params, doseq=True)
+
+        new_url = urlunparse((parsed_base_url.scheme, parsed_base_url.netloc, combined_path, parsed_base_url.params, query_string, parsed_base_url.fragment))
+        return new_url
+
     def __build_authentication_body(self, username, password):
         """Builds the body for the token request.
 
         Args:
             username (string): user's username
             password (string): user's password
 
@@ -82,59 +127,59 @@
             username (string): user's username or email
             password (string): user's password
 
         Returns:
             string: the user's authentication token
         """
         body = self.__build_authentication_body(username, password)
-        response = requests.post(f"{self.base_url}/token", json=body)
+        response = requests.post(self.build_url('/token'), json=body)
         response.raise_for_status()
         return response.text
 
     def get_paths(self):
         """Gets all paths currently loaded in the Transition application
 
         Returns:
             geojson: Transition paths as a GeoJSON LineString FeatureCollection object
         """
         headers = self.__build_headers()
-        response = requests.get(f"{self.base_url}/api/v1/paths", headers=headers)
+        response = requests.get(self.build_url('/api/v1/paths'), headers=headers)
         response.raise_for_status()
         return response.json()
 
     def get_nodes(self):
         """Gets all nodes currently loaded in the Transition application
 
         Returns:
             geojson: Transition nodes as a GeoJSON Point FeatureCollection object
         """
         headers = self.__build_headers()
-        response = requests.get(f"{self.base_url}/api/v1/nodes", headers=headers)
+        response = requests.get(self.build_url('/api/v1/nodes'), headers=headers)
         response.raise_for_status()
         return response.json()
 
     def get_scenarios(self):
         """Gets all scenarios currently loaded in the Transition application
 
         Returns:
             List: List of Transition scenarios with their parameters
         """
         headers = self.__build_headers()
-        response = requests.get(f"{self.base_url}/api/v1/scenarios", headers=headers)
+        response = requests.get(self.build_url('/api/v1/scenarios'), headers=headers)
         response.raise_for_status()
         return response.json()
 
     def get_routing_modes(self):
         """Gets all routing modes currently available in the Transition application
 
         Returns:
             List: List of routing modes as a list of strings
         """
         headers = self.__build_headers()
-        response = requests.get(f"{self.base_url}/api/v1/routing-modes", headers=headers)
+        response = requests.get(self.build_url('/api/v1/routing-modes'), headers=headers)
         response.raise_for_status()
         return json.loads(response.text)
 
     def request_routing_result(
         self,
         modes,
         origin,
@@ -204,15 +249,15 @@
                 "geometry": {"type": "Point", "coordinates": destination},
             },
         }
 
         headers = self.__build_headers()
         params = {"withGeojson": "true" if with_geojson else "false"}
         response = requests.post(
-            f"{self.base_url}/api/v1/route", headers=headers, json=body, params=params
+            self.build_url('/api/v1/route', params=params), headers=headers, json=body
         )
         response.raise_for_status()
         return response.json()
 
     def request_accessibility_map(
         self,
         coordinates,
@@ -287,11 +332,11 @@
             },
             "scenarioId": scenario_id,
         }
 
         headers = self.__build_headers()
         params = {"withGeojson": "true" if with_geojson else "false"}
         response = requests.post(
-            f"{self.base_url}/api/v1/accessibility", headers=headers, json=body, params=params
+            self.build_url('/api/v1/accessibility', params=params), headers=headers, json=body
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `pytransition-0.1.0/pyTransition.egg-info/PKG-INFO` & `pytransition-0.1.1/pyTransition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTransition
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to interact with the Transition API.
 Author: Transition City
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pytransition-0.1.0/setup.py` & `pytransition-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name="pyTransition",
-    version="0.1.0",
+    version="0.1.1",
     description="A Python package to interact with the Transition API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Transition City",
     packages=find_packages(),
     install_requires=["requests", "requests_mock"],
     python_requires=">=3.6",
```

### Comparing `pytransition-0.1.0/tests/test_transition.py` & `pytransition-0.1.1/tests/test_transition.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,23 @@
         }
         with requests_mock.Mocker() as m:
             m.post(f"{self.test_url}/token", text=self.test_token, status_code=200)
             self.test_transition_instance = Transition(
                 self.test_url, self.test_username, self.test_password
             )
 
+    def test_url_cleanup(self):
+         with requests_mock.Mocker() as m:
+            m.post(f"{self.test_url}/token", text=self.test_token, status_code=200)
+
+            url_with_extra_chars = self.test_url+"/"
+            transition_instance = Transition(url_with_extra_chars, self.test_username, self.test_password)
+            self.assertEqual(transition_instance.base_url, self.test_url)
+            self.assertEqual(transition_instance.token, self.test_token)
+
     def test_creation_username_password(self):
         with requests_mock.Mocker() as m:
             m.post(f"{self.test_url}/token", text=self.test_token, status_code=200)
 
             transition_instance = Transition(self.test_url, self.test_username, self.test_password)
             self.assertEqual(transition_instance.base_url, self.test_url)
             self.assertEqual(transition_instance.token, self.test_token)
```

