# Comparing `tmp/scratchattach-1.7.2.tar.gz` & `tmp/scratchattach-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.7.2.tar", last modified: Sat Apr 20 02:26:20 2024, max compression
+gzip compressed data, was "scratchattach-1.7.3.tar", last modified: Fri May 24 21:33:04 2024, max compression
```

## Comparing `scratchattach-1.7.2.tar` & `scratchattach-1.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 02:26:20.714368 scratchattach-1.7.2/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.7.2/LICENSE
--rw-rw-rw-   0        0        0     4267 2024-04-20 02:26:20.714368 scratchattach-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     3534 2024-04-20 01:08:36.000000 scratchattach-1.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 02:26:20.699364 scratchattach-1.7.2/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.7.2/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    23277 2024-04-20 01:53:15.000000 scratchattach-1.7.2/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    25382 2024-04-20 02:25:56.000000 scratchattach-1.7.2/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.7.2/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.7.2/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.7.2/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.7.2/scratchattach/project.py
--rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.7.2/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.7.2/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.7.2/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:26:20.713367 scratchattach-1.7.2/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4267 2024-04-20 02:26:20.000000 scratchattach-1.7.2/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-20 02:26:20.000000 scratchattach-1.7.2/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 02:26:20.000000 scratchattach-1.7.2/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-20 02:26:20.000000 scratchattach-1.7.2/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 02:26:20.000000 scratchattach-1.7.2/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 02:26:20.714368 scratchattach-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-20 02:26:07.000000 scratchattach-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 21:33:04.123737 scratchattach-1.7.3/
+-rw-rw-rw-   0        0        0     1101 2024-05-24 21:30:03.000000 scratchattach-1.7.3/LICENSE
+-rw-rw-rw-   0        0        0     4271 2024-05-24 21:33:04.123602 scratchattach-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3534 2024-05-24 21:30:03.000000 scratchattach-1.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 21:33:04.081643 scratchattach-1.7.3/scratchattach/
+-rw-rw-rw-   0        0        0     2797 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    23277 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    25382 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31477 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22608 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20669 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    38179 2024-05-24 21:30:03.000000 scratchattach-1.7.3/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-05-24 21:33:04.121608 scratchattach-1.7.3/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4271 2024-05-24 21:33:03.000000 scratchattach-1.7.3/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-05-24 21:33:03.000000 scratchattach-1.7.3/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 21:33:03.000000 scratchattach-1.7.3/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-24 21:33:03.000000 scratchattach-1.7.3/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 21:33:03.000000 scratchattach-1.7.3/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 21:33:04.124598 scratchattach-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2024-05-24 21:31:00.000000 scratchattach-1.7.3/setup.py
```

### Comparing `scratchattach-1.7.2/LICENSE` & `scratchattach-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/PKG-INFO` & `scratchattach-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.7.2
-Summary: An Scratch API Wrapper for scra tch.mit.edu
+Version: 1.7.3
+Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
-Author-email: timkrome2006@gmail.com
+Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scratchattach-1.7.2/README.md` & `scratchattach-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/scratchattach/__init__.py` & `scratchattach-1.7.3/scratchattach/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from .cloud import *
-from .user import *
-from .session import *
-from .project import *
-from .studio import *
-from .cloud_requests import *
-from .forum import *
-from .encoder import *
-
-def get_news(*, limit=10, offset=0):
-    return requests.get(f"https://api.scratch.mit.edu/news?limit={limit}&offset={offset}").json()
-
-def featured_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_projects"]
-
-def featured_studios():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_studios"]
-
-def top_loved():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_loved_projects"]
-
-def top_remixed():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_remixed_projects"]
-
-def newest_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_newest_projects"]
-
-def curated_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["curator_top_projects"]
-
-def design_studio_projects():
-    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["scratch_design_studio"]
-
-def search_posts(*, query, order="newest", page=0):
-    try:
-        data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
-        return_data = []
-        for o in data:
-            a = forum.ForumPost(id = o["id"])
-            a._update_from_dict(o)
-            return_data.append(a)
-        return return_data
-    except Exception:
-        return []
-
-def total_site_stats():
-    data = requests.get("https://scratch.mit.edu/statistics/data/daily/").json()
-    data.pop("_TS")
-    return data
-
-def monthly_site_traffic():
-    data = requests.get("https://scratch.mit.edu/statistics/data/monthly-ga/").json()
-    data.pop("_TS")
-    return data
-
-def country_counts():
-    return requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["country_distribution"]
-
-def age_distribution():
-    data = requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["age_distribution_data"][0]["values"]
-    return_data = {}
-    for value in data:
-        return_data[value["x"]] = value["y"]
-    return return_data
-
-def get_health():
-    return requests.get("https://api.scratch.mit.edu/health").json()
-
-def get_csrf_token():
-    """
-    Generates a scratchcsrftoken using Scratch's API.
-
-    Returns:
-        str: The generated scratchcsrftoken
-    """
-    return requests.get(
-        "https://scratch.mit.edu/csrf_token/"
-    ).headers["set-cookie"].split(";")[3][len(" Path=/, scratchcsrftoken="):]
+from .cloud import *
+from .user import *
+from .session import *
+from .project import *
+from .studio import *
+from .cloud_requests import *
+from .forum import *
+from .encoder import *
+
+def get_news(*, limit=10, offset=0):
+    return requests.get(f"https://api.scratch.mit.edu/news?limit={limit}&offset={offset}").json()
+
+def featured_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_projects"]
+
+def featured_studios():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_featured_studios"]
+
+def top_loved():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_loved_projects"]
+
+def top_remixed():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_most_remixed_projects"]
+
+def newest_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["community_newest_projects"]
+
+def curated_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["curator_top_projects"]
+
+def design_studio_projects():
+    return requests.get("https://api.scratch.mit.edu/proxy/featured").json()["scratch_design_studio"]
+
+def search_posts(*, query, order="newest", page=0):
+    try:
+        data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
+        return_data = []
+        for o in data:
+            a = forum.ForumPost(id = o["id"])
+            a._update_from_dict(o)
+            return_data.append(a)
+        return return_data
+    except Exception:
+        return []
+
+def total_site_stats():
+    data = requests.get("https://scratch.mit.edu/statistics/data/daily/").json()
+    data.pop("_TS")
+    return data
+
+def monthly_site_traffic():
+    data = requests.get("https://scratch.mit.edu/statistics/data/monthly-ga/").json()
+    data.pop("_TS")
+    return data
+
+def country_counts():
+    return requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["country_distribution"]
+
+def age_distribution():
+    data = requests.get("https://scratch.mit.edu/statistics/data/monthly/").json()["age_distribution_data"][0]["values"]
+    return_data = {}
+    for value in data:
+        return_data[value["x"]] = value["y"]
+    return return_data
+
+def get_health():
+    return requests.get("https://api.scratch.mit.edu/health").json()
+
+def get_csrf_token():
+    """
+    Generates a scratchcsrftoken using Scratch's API.
+
+    Returns:
+        str: The generated scratchcsrftoken
+    """
+    return requests.get(
+        "https://scratch.mit.edu/csrf_token/"
+    ).headers["set-cookie"].split(";")[3][len(" Path=/, scratchcsrftoken="):]
```

### Comparing `scratchattach-1.7.2/scratchattach/cloud.py` & `scratchattach-1.7.3/scratchattach/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/scratchattach/cloud_requests.py` & `scratchattach-1.7.3/scratchattach/cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/scratchattach/encoder.py` & `scratchattach-1.7.3/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/scratchattach/exceptions.py` & `scratchattach-1.7.3/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/scratchattach/forum.py` & `scratchattach-1.7.3/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.7.2/scratchattach/project.py` & `scratchattach-1.7.3/scratchattach/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,21 @@
             if len(r) != 40:
                 comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
+    def get_comment(self, comment_id):
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self.author}/projects/{self.id}/comments/{comment_id}",
+            headers=self._headers,
+            cookies=self._cookies
+        ).json()
+        return r
     def love(self):
         """
         Posts a love on the project. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_project`
         """
         if self._session is None:
             raise(exceptions.Unauthenticated)
             return
```

### Comparing `scratchattach-1.7.2/scratchattach/session.py` & `scratchattach-1.7.3/scratchattach/session.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,550 +1,550 @@
-#----- Connecting to a Scratch account
-
-import json
-import re
-import requests
-import warnings
-
-from . import user
-from . import cloud
-from . import project
-from . import exceptions
-from . import studio
-from . import forum
-
-headers = {
-    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
-    "x-csrftoken": "a",
-    "x-requested-with": "XMLHttpRequest",
-    "referer": "https://scratch.mit.edu",
-}
-
-class Session():
-
-    '''
-    Represents a Scratch log in / session. Stores authentication data (session id and xtoken).
-
-    Attributes:
-
-    :.session_id: The session id associated with the login
-
-    :.xtoken: The xtoken associated with the login
-
-    :.email: The email address associated with the logged in account
-
-    :.new_scratcher: Returns True if the associated account is a Scratcher
-
-    :.mute_status: Information about commenting restrictions of the associated account
-
-    :.banned: Returns True if the associated account is banned
-    '''
-    
-    def __init__(self, session_id, *, username=None):
-
-        self.session_id = str(session_id)
-        self._username = username
-        self._headers = headers
-        self._cookies = {
-            "scratchsessionsid" : self.session_id,
-            "scratchcsrftoken" : "a",
-            "scratchlanguage" : "en",
-            "accept": "application/json",
-            "Content-Type": "application/json",
-        }
-        self._get_xtoken()
-        try:
-            self._headers.pop("Cookie")
-        except Exception: pass
-
-    def _get_csrftoken(self):
-        r = requests.get("https://scratch.mit.edu/csrf_token/").headers
-        print(r)
-        csrftoken = r["Set-Cookie"].split("scratchcsrftoken=")[1].split(";")[0]
-        self._headers["x-csrftoken"] = csrftoken
-        self._cookies["scratchcsrftoken"] = csrftoken
-
-    def _get_xtoken(self):
-
-        # this will fetch the account token
-        try:
-            response = json.loads(requests.post(
-                "https://scratch.mit.edu/session",
-                headers = {
-                    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
-                    "x-csrftoken": "a",
-                    "x-requested-with": "XMLHttpRequest",
-                    "referer": "https://scratch.mit.edu",
-                },
-                cookies = {
-                    "scratchsessionsid" : self.session_id,
-                    "scratchcsrftoken" : "a",
-                    "scratchlanguage" : "en"
-                }
-            ).text)
-
-            self.xtoken = response['user']['token']
-            self._headers["X-Token"] = self.xtoken
-            self.email = response["user"]["email"]
-            self.new_scratcher = response["permissions"]["new_scratcher"]
-            self.mute_status = response["permissions"]["mute_status"]
-            self._username = response["user"]["username"]
-            self.banned = response["user"]["banned"]
-            if self.banned:
-                warnings.warn(f"Warning: The account {self._username} you logged in to is BANNED. Some features may not work properly.")
-
-        except Exception:
-            if self._username is None:
-                print("Warning: Logged in, but couldn't fetch XToken.\nSome features (including cloud variables) will not work properly. To get cloud variables to work, provide a username argument: Session('session_id', username='username')\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
-            else:
-                print(f"Warning: Logged in as {self._username}, but couldn't fetch XToken. Cloud variables will still work, but other features may not work properly.\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
-            self.xtoken = ""
-
-    def get_linked_user(self):
-        '''
-        Gets the user associated with the log in / session.
-
-        Returns:
-            scratchattach.user.User: Object representing the user associated with the log in / session.
-        '''
-        if not "_user" in self.__dict__:
-            self._user = self.connect_user(self._username)
-        return self._user
-
-    def mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
-        '''
-        Gets the projects from the "My stuff" page.
-
-        Args:
-            ordering (str): Possible values for this parameter are "all", "shared", "unshared" and "trashed"
-        
-        Keyword Arguments:
-            page (int): The page of the "My Stuff" projects that should be returned
-            sort_by (str): The key the projects should be sorted based on. Possible values for this parameter are "" (then the projects are sorted based on last modified), "view_count", love_count", "remixers_count" (then the projects are sorted based on remix count) and "title" (then the projects are sorted based on title)
-            descending (boolean): Determines if the element with the highest key value (the key is specified in the sort_by argument) should be returned first. Defaults to True.
-      
-        Returns:
-            list<dict>: A list with the projects from the "My Stuff" page, each project is represented by a dict.
-        '''
-        if descending:
-            ascsort = ""
-            descsort = sort_by
-        else:
-            ascsort = sort_by
-            descsort = ""
-        try:
-            targets = requests.get(
-                f"https://scratch.mit.edu/site-api/projects/{ordering}/?page={page}&ascsort={ascsort}&descsort={descsort}",
-                headers = headers,
-                cookies = self._cookies,
-            ).json()
-            projects = []
-            for target in targets:
-                projects.append(
-                    dict(
-                        author = self._username,
-                        created = target["fields"]["datetime_created"],
-                        last_modified = target["fields"]["datetime_modified"],
-                        share_date = target["fields"]["datetime_shared"],
-                        shared = target["fields"]["isPublished"],
-                        id = target["pk"],
-                        thumbnail_url = "https://uploads.scratch.mit.edu"+target["fields"]["uncached_thumbnail_url"][1:],
-                        favorites = target["fields"]["favorite_count"],
-                        loves = target["fields"]["love_count"],
-                        remixes = target["fields"]["remixers_count"],
-                        views = target["fields"]["view_count"],
-                        thumbnail_name = target["fields"]["thumbnail"],
-                        title = target["fields"]["title"],
-                        url = "https://scratch.mit.edu/projects/" + str(target["pk"]),
-                        comment_count = target["fields"]["commenters_count"],
-                    )
-                )
-            return projects
-        except Exception:
-            raise(exceptions.FetchError)
-
-    def get_mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
-        '''
-        Alternate name for :meth:`scratchattach.session.Session.mystuff_projects`. See the documentation of this function.
-        '''
-        return self.mystuff_projects(ordering, page=page, sort_by=sort_by, descending=descending)
-
-    def messages(self, *, limit=40, offset=0):
-        '''
-        Returns the messages.
-
-        Returns:
-            list<dict>: List that contains all messages as dicts.
-        '''
-        return requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/messages?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies,
-        ).json()
-
-    def clear_messages(self):
-        '''
-        Clears all messages.
-        '''
-        return requests.post(
-            "https://scratch.mit.edu/site-api/messages/messages-clear/",
-            headers = self._headers,
-            cookies = self._cookies,
-        ).text
-
-    def message_count(self):
-        '''
-        Returns the message count.
-
-        Returns:
-            int: message count
-        '''
-        return json.loads(requests.get(f"https://api.scratch.mit.edu/users/{self._username}/messages/count/", headers = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.3c6 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',}).text)["count"]
-
-    def get_feed(self, *, limit=20, offset=0):
-        '''
-        Returns the "What's happening" section (frontpage).
-
-        Returns:
-            list<dict>: List that contains all "What's happening" entries as dicts
-        '''
-        return requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/users/activity?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-
-    '''def create_project(self): # not working
-
-        try:
-
-            return self.connect_project(requests.post(
-                "https://projects.scratch.mit.edu/",
-                headers = headers,
-                cookies = self._cookies
-            ).json()["content-name"])
-        except Exception:
-            raise(exceptions.FetchError)
-    ''' 
-    ''' # these APIs are always empty
-    def created_by_followed_users(self, *, limit=40, offset=0):
-        r = requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/users/projects?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-        projects = []
-
-        for project in r:
-            p = project.Project()
-            p._update_from_dict(project)
-            projects.append(p)
-        return projects
-
-    def added_to_followed_studios(self, *, limit=40, offset=0):
-        r = requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/studios/projects?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-        projects = []
-
-        for project in r:
-            p = project.Project()
-            p._update_from_dict(project)
-            projects.append(p)
-        return projects
-    '''
-
-    def loved_by_followed_users(self, *, limit=40, offset=0):
-        '''
-        Returns the "Projects loved by Scratchers I'm following" section (frontpage).
-
-        Returns:
-            list<scratchattach.project.Project>: List that contains all "Projects loved by Scratchers I'm following" entries as Project objects
-        '''
-        r = requests.get(
-            f"https://api.scratch.mit.edu/users/{self._username}/following/users/loves?limit={limit}&offset={offset}",
-            headers = self._headers,
-            cookies = self._cookies
-        ).json()
-        projects = []
-
-        for project_dict in r:
-            p = project.Project(_session = self)
-            p._update_from_dict(project_dict)
-            projects.append(p)
-        return projects
-
-    def search_projects(self, *, query="", mode="trending", language="en", limit=40, offset=0):
-        '''
-        Uses the Scratch search to search projects.
-
-        Keyword arguments:
-            query (str): The query that will be searched.
-            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
-            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different results.)
-            limit (int): Max. amount of returned projects.
-            offset (int): Offset of the first returned project.
-
-        Returns:
-            list<scratchattach.project.Project>: List that contains the search results.
-        '''
-        r = requests.get(f"https://api.scratch.mit.edu/search/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
-        projects = []
-
-        for project_dict in r:
-            p = project.Project(_session = self)
-            p._update_from_dict(project_dict)
-            projects.append(p)
-        return projects
-    def explore_projects(self, *, query="*", mode="trending", language="en", limit=40, offset=0):
-        '''
-        Gets projects from the explore page.
-
-        Keyword arguments:
-            query (str): Specifies the tag of the explore page. To get the projects from the "All" tag, set this argument to "*".
-            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
-            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different explore pages.)
-            limit (int): Max. amount of returned projects.
-            offset (int): Offset of the first returned project.
-
-        Returns:
-            list<scratchattach.project.Project>: List that contains the explore page projects.
-        '''
-        r = requests.get(f"https://api.scratch.mit.edu/explore/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
-        projects = []
-
-        for project_dict in r:
-            p = project.Project(_session = self)
-            p._update_from_dict(project_dict)
-            projects.append(p)
-        return projects
-
-
-    def backpack(self,limit=20, offset=0):
-        '''
-        Lists the assets that are in the backpack of the user associated with the session.
-
-        Returns:
-            list<dict>: List that contains the backpack items as dicts
-        '''
-        return requests.get(
-            f"https://backpack.scratch.mit.edu/{self._username}?limit={limit}&offset={offset}",
-            headers = self._headers,
-        ).json()
-
-    def delete_from_backpack(self, asset_id):
-        '''
-        Deletes an asset from the backpack.
-
-        Args:
-            asset_id: ID of the asset that will be deleted.
-        '''
-        return requests.delete(
-            f"https://backpack.scratch.mit.edu/{self._username}/{asset_id}",
-            headers = self._headers,
-        ).json()
-
-    def connect_cloud(self, project_id_arg=None, *, project_id=None):
-        '''
-        Connects to the cloud variables of a project.
-
-        Args:
-            project_id (str): ID of the project that will be connected to.
-
-        Returns:
-            scratchattach.cloud.CloudConnection: An object that represents the created connection and allows you to set cloud variables
-        '''
-        if project_id is None:
-            project_id = project_id_arg
-        if project_id is None:
-            return None
-
-        return cloud.CloudConnection(username = self._username, session_id = self.session_id, project_id = int(project_id))
-
-    def connect_tw_cloud(self, project_id_arg=None, *, project_id=None, purpose="", contact=""):
-        return cloud.connect_tw_cloud(project_id_arg, project_id=project_id, purpose=purpose, contact=contact)
-
-    def connect_user(self, username):
-        """
-        Gets a user.
-
-        Args:
-            username (str): Username of the requested user
-
-        Returns:
-            scratchattach.user.User: An object that represents the requested user and allows you to perform actions on the user (like user.follow)
-        """
-        try:
-            _user = user.User(username=username, _session=self)
-            if _user.update() == "429":
-                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
-            return _user
-        except KeyError:
-            return None
-        except Exception as e:
-            raise(e)
-
-    def connect_project(self, project_id):
-        """
-        Gets a project.
-
-        Args:
-            project_id (int): ID of the requested project
-
-        Returns:
-            scratchattach.project.Project: An object that represents the requested project and allows you to perform actions on the project (like project.love)
-        """
-        try:
-            _project = project.Project(id=int(project_id), _session=self)
-            u = _project.update()
-            if u == "429":
-                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
-            if not u:
-                _project = project.PartialProject(id=int(project_id))
-            return _project
-        except KeyError:
-            return None
-        except Exception as e:
-            raise(e)
-
-    def connect_studio(self, studio_id):
-        """
-        Gets a studio.
-
-        Args:
-            studio_id (int): ID of the requested studio
-
-        Returns:
-            scratchattach.studio.Studio: An object that represents the requested studio and allows you to perform actions on the studio (like studio.follow)
-        """
-        try:
-            _studio = studio.Studio(id=int(studio_id), _session=self)
-            if _studio.update() == "429":
-                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
-            return _studio
-        except KeyError:
-            return None
-        except Exception as e:
-            raise(e)
-
-    def connect_topic(self, topic_id):
-        """
-        Gets a forum topic. Data fetched from ScratchDB.
-
-        Args:
-            topic_id (int): ID of the requested forum topic (can be found in the browser URL bar)
-
-        Returns:
-            scratchattach.forum.ForumTopic: An object that represents the requested forum topic
-        """
-
-        try:
-            topic = forum.ForumTopic(id=int(topic_id), _session=self)
-            topic.update()
-            return topic
-        except KeyError:
-            return None
-
-    def connect_topic_list(self, category_name, *, page=0, include_deleted=False):
-        """
-        Gets the topics from a forum category. Data fetched from ScratchDB.
-
-        Args:
-            category_name (str): Name of the forum category
-        
-        Keyword Arguments:
-            page (str): Page of the category topics that should be returned
-            include_deleted (boolean): Whether deleted topics should be returned too
-
-        Returns:
-            list<scratchattach.forum.ForumTopic>: A list containing the forum topics from the specified category
-        """
-        category_name.replace(" ", "%20")
-        if include_deleted:
-            filter = 0
-        else:
-            filter = 1
-        try:
-            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/category/topics/{category_name}/{page}?detail=1&filter={filter}").json()
-            return_data = []
-            for topic in data:
-                t = forum.ForumTopic(id = topic["id"], _session=self)
-                t._update_from_dict(topic)
-                return_data.append(t)
-            return return_data
-        except Exception:
-            return None
-
-    def connect_post(self, post_id):
-
-        """
-        Gets a forum post. Data fetched from ScratchDB.
-
-        Args:
-            post_id (int): ID of the requested forum post
-
-        Returns:
-            scratchattach.forum.ForumPost: An object that represents the requested forum post
-        """
-
-        try:
-            post = forum.ForumPost(id=int(post_id), _session=self)
-            post.update()
-            return post
-        except KeyError:
-            return None
-
-    def search_posts(self, *, query, order="newest", page=0):
-        try:
-            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
-            return_data = []
-            for o in data:
-                a = forum.ForumPost(id = o["id"], _session = self._session)
-                a._update_from_dict(o)
-                return_data.append(a)
-            return return_data
-        except Exception:
-            return []
-
-    def upload_asset(asset):
-        data = asset if isinstance(asset, bytes) else open(asset, "rb").read()
-
-        if isinstance(asset, str):
-            file_ext = pathlib.Path(asset).suffix
-
-        requests.post(
-            f"https://assets.scratch.mit.edu/{hashlib.md5(data).hexdigest()}.{file_ext}",
-            headers=self._headers,
-            data=data,
-        )
-    
-# ------ #
-
-def login(username, password):
-    """
-    Creates a session / log in to the Scratch website with the specified username and password. 
-
-    This method will first create a session id, then it will fetch the xtoken and other information using the created session id.
-    If the log in fails, it will raise scratchattach.exceptions.LoginFailure.
-    If the login succeeds but fetching the xtoken fails, it will not raise an exception but display a warning. If the accout logged in to is banned, it will also display a warning.
-
-    Args:
-        username (str)
-        password (str)
-    
-    Returns:
-        scratchattach.session.Session: An object that represents the created log in / session
-    """
-    data = json.dumps({"username": username, "password": password})
-    _headers = headers
-    _headers["Cookie"] = "scratchcsrftoken=a;scratchlanguage=en;"
-    request = requests.post(
-        "https://scratch.mit.edu/login/", data=data, headers=_headers
-    )
-    try:
-        session_id = str(re.search('"(.*)"', request.headers["Set-Cookie"]).group())
-    except Exception:
-        raise exceptions.LoginFailure("Either the provided authentication data is wrong or your network is banned from Scratch.\n\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress. In this case, try logging in with your session id: https://github.com/TimMcCool/scratchattach/wiki#logging-in")
-    session = Session(session_id, username=username)
-    return session
+#----- Connecting to a Scratch account
+
+import json
+import re
+import requests
+import warnings
+
+from . import user
+from . import cloud
+from . import project
+from . import exceptions
+from . import studio
+from . import forum
+
+headers = {
+    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
+    "x-csrftoken": "a",
+    "x-requested-with": "XMLHttpRequest",
+    "referer": "https://scratch.mit.edu",
+}
+
+class Session():
+
+    '''
+    Represents a Scratch log in / session. Stores authentication data (session id and xtoken).
+
+    Attributes:
+
+    :.session_id: The session id associated with the login
+
+    :.xtoken: The xtoken associated with the login
+
+    :.email: The email address associated with the logged in account
+
+    :.new_scratcher: Returns True if the associated account is a Scratcher
+
+    :.mute_status: Information about commenting restrictions of the associated account
+
+    :.banned: Returns True if the associated account is banned
+    '''
+    
+    def __init__(self, session_id, *, username=None):
+
+        self.session_id = str(session_id)
+        self._username = username
+        self._headers = headers
+        self._cookies = {
+            "scratchsessionsid" : self.session_id,
+            "scratchcsrftoken" : "a",
+            "scratchlanguage" : "en",
+            "accept": "application/json",
+            "Content-Type": "application/json",
+        }
+        self._get_xtoken()
+        try:
+            self._headers.pop("Cookie")
+        except Exception: pass
+
+    def _get_csrftoken(self):
+        r = requests.get("https://scratch.mit.edu/csrf_token/").headers
+        print(r)
+        csrftoken = r["Set-Cookie"].split("scratchcsrftoken=")[1].split(";")[0]
+        self._headers["x-csrftoken"] = csrftoken
+        self._cookies["scratchcsrftoken"] = csrftoken
+
+    def _get_xtoken(self):
+
+        # this will fetch the account token
+        try:
+            response = json.loads(requests.post(
+                "https://scratch.mit.edu/session",
+                headers = {
+                    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',
+                    "x-csrftoken": "a",
+                    "x-requested-with": "XMLHttpRequest",
+                    "referer": "https://scratch.mit.edu",
+                },
+                cookies = {
+                    "scratchsessionsid" : self.session_id,
+                    "scratchcsrftoken" : "a",
+                    "scratchlanguage" : "en"
+                }
+            ).text)
+
+            self.xtoken = response['user']['token']
+            self._headers["X-Token"] = self.xtoken
+            self.email = response["user"]["email"]
+            self.new_scratcher = response["permissions"]["new_scratcher"]
+            self.mute_status = response["permissions"]["mute_status"]
+            self._username = response["user"]["username"]
+            self.banned = response["user"]["banned"]
+            if self.banned:
+                warnings.warn(f"Warning: The account {self._username} you logged in to is BANNED. Some features may not work properly.")
+
+        except Exception:
+            if self._username is None:
+                print("Warning: Logged in, but couldn't fetch XToken.\nSome features (including cloud variables) will not work properly. To get cloud variables to work, provide a username argument: Session('session_id', username='username')\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
+            else:
+                print(f"Warning: Logged in as {self._username}, but couldn't fetch XToken. Cloud variables will still work, but other features may not work properly.\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress.")
+            self.xtoken = ""
+
+    def get_linked_user(self):
+        '''
+        Gets the user associated with the log in / session.
+
+        Returns:
+            scratchattach.user.User: Object representing the user associated with the log in / session.
+        '''
+        if not "_user" in self.__dict__:
+            self._user = self.connect_user(self._username)
+        return self._user
+
+    def mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
+        '''
+        Gets the projects from the "My stuff" page.
+
+        Args:
+            ordering (str): Possible values for this parameter are "all", "shared", "unshared" and "trashed"
+        
+        Keyword Arguments:
+            page (int): The page of the "My Stuff" projects that should be returned
+            sort_by (str): The key the projects should be sorted based on. Possible values for this parameter are "" (then the projects are sorted based on last modified), "view_count", love_count", "remixers_count" (then the projects are sorted based on remix count) and "title" (then the projects are sorted based on title)
+            descending (boolean): Determines if the element with the highest key value (the key is specified in the sort_by argument) should be returned first. Defaults to True.
+      
+        Returns:
+            list<dict>: A list with the projects from the "My Stuff" page, each project is represented by a dict.
+        '''
+        if descending:
+            ascsort = ""
+            descsort = sort_by
+        else:
+            ascsort = sort_by
+            descsort = ""
+        try:
+            targets = requests.get(
+                f"https://scratch.mit.edu/site-api/projects/{ordering}/?page={page}&ascsort={ascsort}&descsort={descsort}",
+                headers = headers,
+                cookies = self._cookies,
+            ).json()
+            projects = []
+            for target in targets:
+                projects.append(
+                    dict(
+                        author = self._username,
+                        created = target["fields"]["datetime_created"],
+                        last_modified = target["fields"]["datetime_modified"],
+                        share_date = target["fields"]["datetime_shared"],
+                        shared = target["fields"]["isPublished"],
+                        id = target["pk"],
+                        thumbnail_url = "https://uploads.scratch.mit.edu"+target["fields"]["uncached_thumbnail_url"][1:],
+                        favorites = target["fields"]["favorite_count"],
+                        loves = target["fields"]["love_count"],
+                        remixes = target["fields"]["remixers_count"],
+                        views = target["fields"]["view_count"],
+                        thumbnail_name = target["fields"]["thumbnail"],
+                        title = target["fields"]["title"],
+                        url = "https://scratch.mit.edu/projects/" + str(target["pk"]),
+                        comment_count = target["fields"]["commenters_count"],
+                    )
+                )
+            return projects
+        except Exception:
+            raise(exceptions.FetchError)
+
+    def get_mystuff_projects(self, ordering, *, page=1, sort_by="", descending=True):
+        '''
+        Alternate name for :meth:`scratchattach.session.Session.mystuff_projects`. See the documentation of this function.
+        '''
+        return self.mystuff_projects(ordering, page=page, sort_by=sort_by, descending=descending)
+
+    def messages(self, *, limit=40, offset=0):
+        '''
+        Returns the messages.
+
+        Returns:
+            list<dict>: List that contains all messages as dicts.
+        '''
+        return requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/messages?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies,
+        ).json()
+
+    def clear_messages(self):
+        '''
+        Clears all messages.
+        '''
+        return requests.post(
+            "https://scratch.mit.edu/site-api/messages/messages-clear/",
+            headers = self._headers,
+            cookies = self._cookies,
+        ).text
+
+    def message_count(self):
+        '''
+        Returns the message count.
+
+        Returns:
+            int: message count
+        '''
+        return json.loads(requests.get(f"https://api.scratch.mit.edu/users/{self._username}/messages/count/", headers = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.3c6 (KHTML, like Gecko) Chrome/75.0.3770.142 Safari/537.36',}).text)["count"]
+
+    def get_feed(self, *, limit=20, offset=0):
+        '''
+        Returns the "What's happening" section (frontpage).
+
+        Returns:
+            list<dict>: List that contains all "What's happening" entries as dicts
+        '''
+        return requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/users/activity?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+
+    '''def create_project(self): # not working
+
+        try:
+
+            return self.connect_project(requests.post(
+                "https://projects.scratch.mit.edu/",
+                headers = headers,
+                cookies = self._cookies
+            ).json()["content-name"])
+        except Exception:
+            raise(exceptions.FetchError)
+    ''' 
+    ''' # these APIs are always empty
+    def created_by_followed_users(self, *, limit=40, offset=0):
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/users/projects?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+        projects = []
+
+        for project in r:
+            p = project.Project()
+            p._update_from_dict(project)
+            projects.append(p)
+        return projects
+
+    def added_to_followed_studios(self, *, limit=40, offset=0):
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/studios/projects?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+        projects = []
+
+        for project in r:
+            p = project.Project()
+            p._update_from_dict(project)
+            projects.append(p)
+        return projects
+    '''
+
+    def loved_by_followed_users(self, *, limit=40, offset=0):
+        '''
+        Returns the "Projects loved by Scratchers I'm following" section (frontpage).
+
+        Returns:
+            list<scratchattach.project.Project>: List that contains all "Projects loved by Scratchers I'm following" entries as Project objects
+        '''
+        r = requests.get(
+            f"https://api.scratch.mit.edu/users/{self._username}/following/users/loves?limit={limit}&offset={offset}",
+            headers = self._headers,
+            cookies = self._cookies
+        ).json()
+        projects = []
+
+        for project_dict in r:
+            p = project.Project(_session = self)
+            p._update_from_dict(project_dict)
+            projects.append(p)
+        return projects
+
+    def search_projects(self, *, query="", mode="trending", language="en", limit=40, offset=0):
+        '''
+        Uses the Scratch search to search projects.
+
+        Keyword arguments:
+            query (str): The query that will be searched.
+            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
+            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different results.)
+            limit (int): Max. amount of returned projects.
+            offset (int): Offset of the first returned project.
+
+        Returns:
+            list<scratchattach.project.Project>: List that contains the search results.
+        '''
+        r = requests.get(f"https://api.scratch.mit.edu/search/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
+        projects = []
+
+        for project_dict in r:
+            p = project.Project(_session = self)
+            p._update_from_dict(project_dict)
+            projects.append(p)
+        return projects
+    def explore_projects(self, *, query="*", mode="trending", language="en", limit=40, offset=0):
+        '''
+        Gets projects from the explore page.
+
+        Keyword arguments:
+            query (str): Specifies the tag of the explore page. To get the projects from the "All" tag, set this argument to "*".
+            mode (str): Has to be one of these values: "trending", "popular" or "recent". Defaults to "trending".
+            language (str): A language abbreviation, defaults to "en". (Depending on the language used on the Scratch website, Scratch displays you different explore pages.)
+            limit (int): Max. amount of returned projects.
+            offset (int): Offset of the first returned project.
+
+        Returns:
+            list<scratchattach.project.Project>: List that contains the explore page projects.
+        '''
+        r = requests.get(f"https://api.scratch.mit.edu/explore/projects?limit={limit}&offset={offset}&language={language}&mode={mode}&q={query}").json()
+        projects = []
+
+        for project_dict in r:
+            p = project.Project(_session = self)
+            p._update_from_dict(project_dict)
+            projects.append(p)
+        return projects
+
+
+    def backpack(self,limit=20, offset=0):
+        '''
+        Lists the assets that are in the backpack of the user associated with the session.
+
+        Returns:
+            list<dict>: List that contains the backpack items as dicts
+        '''
+        return requests.get(
+            f"https://backpack.scratch.mit.edu/{self._username}?limit={limit}&offset={offset}",
+            headers = self._headers,
+        ).json()
+
+    def delete_from_backpack(self, asset_id):
+        '''
+        Deletes an asset from the backpack.
+
+        Args:
+            asset_id: ID of the asset that will be deleted.
+        '''
+        return requests.delete(
+            f"https://backpack.scratch.mit.edu/{self._username}/{asset_id}",
+            headers = self._headers,
+        ).json()
+
+    def connect_cloud(self, project_id_arg=None, *, project_id=None):
+        '''
+        Connects to the cloud variables of a project.
+
+        Args:
+            project_id (str): ID of the project that will be connected to.
+
+        Returns:
+            scratchattach.cloud.CloudConnection: An object that represents the created connection and allows you to set cloud variables
+        '''
+        if project_id is None:
+            project_id = project_id_arg
+        if project_id is None:
+            return None
+
+        return cloud.CloudConnection(username = self._username, session_id = self.session_id, project_id = int(project_id))
+
+    def connect_tw_cloud(self, project_id_arg=None, *, project_id=None, purpose="", contact=""):
+        return cloud.connect_tw_cloud(project_id_arg, project_id=project_id, purpose=purpose, contact=contact)
+
+    def connect_user(self, username):
+        """
+        Gets a user.
+
+        Args:
+            username (str): Username of the requested user
+
+        Returns:
+            scratchattach.user.User: An object that represents the requested user and allows you to perform actions on the user (like user.follow)
+        """
+        try:
+            _user = user.User(username=username, _session=self)
+            if _user.update() == "429":
+                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
+            return _user
+        except KeyError:
+            return None
+        except Exception as e:
+            raise(e)
+
+    def connect_project(self, project_id):
+        """
+        Gets a project.
+
+        Args:
+            project_id (int): ID of the requested project
+
+        Returns:
+            scratchattach.project.Project: An object that represents the requested project and allows you to perform actions on the project (like project.love)
+        """
+        try:
+            _project = project.Project(id=int(project_id), _session=self)
+            u = _project.update()
+            if u == "429":
+                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
+            if not u:
+                _project = project.PartialProject(id=int(project_id))
+            return _project
+        except KeyError:
+            return None
+        except Exception as e:
+            raise(e)
+
+    def connect_studio(self, studio_id):
+        """
+        Gets a studio.
+
+        Args:
+            studio_id (int): ID of the requested studio
+
+        Returns:
+            scratchattach.studio.Studio: An object that represents the requested studio and allows you to perform actions on the studio (like studio.follow)
+        """
+        try:
+            _studio = studio.Studio(id=int(studio_id), _session=self)
+            if _studio.update() == "429":
+                raise(exceptions.Response429("Your network is blocked or rate-limited by Scratch.\nIf you're using an online IDE like replit.com, try running the code on your computer."))
+            return _studio
+        except KeyError:
+            return None
+        except Exception as e:
+            raise(e)
+
+    def connect_topic(self, topic_id):
+        """
+        Gets a forum topic. Data fetched from ScratchDB.
+
+        Args:
+            topic_id (int): ID of the requested forum topic (can be found in the browser URL bar)
+
+        Returns:
+            scratchattach.forum.ForumTopic: An object that represents the requested forum topic
+        """
+
+        try:
+            topic = forum.ForumTopic(id=int(topic_id), _session=self)
+            topic.update()
+            return topic
+        except KeyError:
+            return None
+
+    def connect_topic_list(self, category_name, *, page=0, include_deleted=False):
+        """
+        Gets the topics from a forum category. Data fetched from ScratchDB.
+
+        Args:
+            category_name (str): Name of the forum category
+        
+        Keyword Arguments:
+            page (str): Page of the category topics that should be returned
+            include_deleted (boolean): Whether deleted topics should be returned too
+
+        Returns:
+            list<scratchattach.forum.ForumTopic>: A list containing the forum topics from the specified category
+        """
+        category_name.replace(" ", "%20")
+        if include_deleted:
+            filter = 0
+        else:
+            filter = 1
+        try:
+            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/category/topics/{category_name}/{page}?detail=1&filter={filter}").json()
+            return_data = []
+            for topic in data:
+                t = forum.ForumTopic(id = topic["id"], _session=self)
+                t._update_from_dict(topic)
+                return_data.append(t)
+            return return_data
+        except Exception:
+            return None
+
+    def connect_post(self, post_id):
+
+        """
+        Gets a forum post. Data fetched from ScratchDB.
+
+        Args:
+            post_id (int): ID of the requested forum post
+
+        Returns:
+            scratchattach.forum.ForumPost: An object that represents the requested forum post
+        """
+
+        try:
+            post = forum.ForumPost(id=int(post_id), _session=self)
+            post.update()
+            return post
+        except KeyError:
+            return None
+
+    def search_posts(self, *, query, order="newest", page=0):
+        try:
+            data = requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={query}&o={order}&page={page}").json()["posts"]
+            return_data = []
+            for o in data:
+                a = forum.ForumPost(id = o["id"], _session = self._session)
+                a._update_from_dict(o)
+                return_data.append(a)
+            return return_data
+        except Exception:
+            return []
+
+    def upload_asset(asset):
+        data = asset if isinstance(asset, bytes) else open(asset, "rb").read()
+
+        if isinstance(asset, str):
+            file_ext = pathlib.Path(asset).suffix
+
+        requests.post(
+            f"https://assets.scratch.mit.edu/{hashlib.md5(data).hexdigest()}.{file_ext}",
+            headers=self._headers,
+            data=data,
+        )
+    
+# ------ #
+
+def login(username, password):
+    """
+    Creates a session / log in to the Scratch website with the specified username and password. 
+
+    This method will first create a session id, then it will fetch the xtoken and other information using the created session id.
+    If the log in fails, it will raise scratchattach.exceptions.LoginFailure.
+    If the login succeeds but fetching the xtoken fails, it will not raise an exception but display a warning. If the accout logged in to is banned, it will also display a warning.
+
+    Args:
+        username (str)
+        password (str)
+    
+    Returns:
+        scratchattach.session.Session: An object that represents the created log in / session
+    """
+    data = json.dumps({"username": username, "password": password})
+    _headers = headers
+    _headers["Cookie"] = "scratchcsrftoken=a;scratchlanguage=en;"
+    request = requests.post(
+        "https://scratch.mit.edu/login/", data=data, headers=_headers
+    )
+    try:
+        session_id = str(re.search('"(.*)"', request.headers["Set-Cookie"]).group())
+    except Exception:
+        raise exceptions.LoginFailure("Either the provided authentication data is wrong or your network is banned from Scratch.\n\nIf you're using an online IDE (like replit.com) Scratch possibly banned its IP adress. In this case, try logging in with your session id: https://github.com/TimMcCool/scratchattach/wiki#logging-in")
+    session = Session(session_id, username=username)
+    return session
```

### Comparing `scratchattach-1.7.2/scratchattach/studio.py` & `scratchattach-1.7.3/scratchattach/studio.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,19 @@
             if len(r) != 40:
                 comments = comments + r
                 break
             offset += 40
             comments = comments + r
         return comments
 
-
+    def get_comment(self, comment_id):
+        r = requests.get(
+            f"https://api.scratch.mit.edu/studios/{self.id}/comments/{comment_id}"
+        ).json()
+        return r
     def post_comment(self, content, *, parent_id="", commentee_id=""):
         """
         Posts a comment on the studio. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_studio`
 
         Args:
             content: Content of the comment that should be posted
 
@@ -285,30 +289,30 @@
         try:
             return requests.put(
                 f"https://scratch.mit.edu/site-api/users/curators-in/{self.id}/invite_curator/?usernames={curator}",
                 headers = headers,
                 cookies = self._cookies,
             ).json()
         except Exception:
-            raise(_exceptions.Unauthorized)
+            raise(exceptions.Unauthorized)
 
     def promote_curator(self, curator):
         """
         You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_studio`
         """
         if self._session is None:
             raise(exceptions.Unauthenticated)
         try:
             return requests.put(
                 f"https://scratch.mit.edu/site-api/users/curators-in/{self.id}/promote/?usernames={curator}",
                 headers = headers,
                 cookies = self._cookies
             ).json()
         except Exception:
-            raise(_exceptions.Unauthorized)
+            raise(exceptions.Unauthorized)
 
 
     def remove_curator(self, curator):
         """
         You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_studio`
         """
         if self._session is None:
@@ -316,15 +320,15 @@
         try:
             return requests.put(
                 f"https://scratch.mit.edu/site-api/users/curators-in/{self.id}/remove/?usernames={curator}",
                 headers = headers,
                 cookies = self._cookies
             ).json()
         except Exception:
-            raise(_exceptions.Unauthorized)
+            raise(exceptions.Unauthorized)
 
     def leave(self):
         """
         Removes yourself from the studio. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_studio`
         """
         if self._session is None:
             raise(exceptions.Unauthenticated)
```

### Comparing `scratchattach-1.7.2/scratchattach/user.py` & `scratchattach-1.7.3/scratchattach/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,36 @@
         except Exception: pass
         self._json_headers = self._headers
         self._json_headers["accept"] = "application/json"
         self._json_headers["Content-Type"] = "application/json"
 
     def __str__(self):
         return str(self.username)
+    
+    def does_exist(self):
+        """
+        Returns:
+            boolean : True if the user exists, False if the user is deleted, None if an error occured
+        """
+        if requests.get(f"https://scratch.mit.edu/users/{self.username}/").status_code == 200:
+            return True
+        if requests.get(f"https://scratch.mit.edu/users/{self.username}/").status_code == 404:
+            return False
+
+    def is_new_scratcher(self):
+        """
+        Returns:
+            boolean : True if the user has the New Scratcher status, else False
+        """
+        try:
+            res = requests.get(f"https://scratch.mit.edu/users/{self.username}/").text
+            group=res[res.rindex('<span class="group">'):][:70]
+            return "new scratcher" in group.lower()
+        except Exception:
+            return None
 
     def update(self):
         """
         Updates the attributes of the User object
         """
         r = requests.get(f"https://api.scratch.mit.edu/users/{self.username}/")
         if "429" in str(r):
@@ -483,14 +505,20 @@
             raise(exceptions.Unauthorized)
 
 
     def set_bio(self, text):
         """
         Sets the user's "About me" section. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
+        if self._session._username != self.username:
+            raise(exceptions.Unauthorized)
+            return
         requests.put(
             f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
             headers = self._json_headers,
             cookies = self._cookies,
             data = json.dumps(dict(
                 comments_allowed = True,
                 id = self.username,
@@ -501,14 +529,20 @@
             ))
         )
 
     def set_wiwo(self, text):
         """
         Sets the user's "What I'm working on" section. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
+        if self._session._username != self.username:
+            raise(exceptions.Unauthorized)
+            return
         requests.put(
             f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
             headers = self._json_headers,
             cookies = self._cookies,
             data = json.dumps(dict(
                 comments_allowed = True,
                 id = self.username,
@@ -525,33 +559,65 @@
 
         Args:
             project_id: Project id of the project that should be set as featured
 
         Keyword Args:
             label: The label that should appear above the featured project on the user's profile (Like "Featured project", "Featured tutorial", "My favorite things", etc.)
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
+        if self._session._username != self.username:
+            raise(exceptions.Unauthorized)
+            return
         requests.put(
             f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
             headers = self._json_headers,
             cookies = self._cookies,
             data = json.dumps({"featured_project":int(project_id),"featured_project_label":label})
         )
 
+    def set_forum_signature(self, text):
+        """
+        Sets the user's discuss forum signature. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
+        """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
+        if self._session._username != self.username:
+            raise(exceptions.Unauthorized)
+            return
+        headers = {
+            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+            'content-type': 'application/x-www-form-urlencoded',
+            'origin': 'https://scratch.mit.edu',
+            'referer': 'https://scratch.mit.edu/discuss/settings/TimMcCool/',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36',
+        }
+        data = {
+            'csrfmiddlewaretoken': 'a',
+            'signature': text,
+            'update': '',
+        }
+        response = requests.post(f'https://scratch.mit.edu/discuss/settings/{self.username}/', cookies=self._cookies, headers=headers, data=data)
 
     def post_comment(self, content, *, parent_id="", commentee_id=""):
         """
         Posts a comment on the user's profile. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
 
         Args:
             content: Content of the comment that should be posted
         
         Keyword Arguments:
             parent_id: ID of the comment you want to reply to. If you don't want to mention a user, don't put the argument.
             commentee_id: ID of the user that will be mentioned in your comment and will receive a message about your comment. If you don't want to mention a user, don't put the argument.
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
         data = {
         "commentee_id": commentee_id,
         "content": str(content),
         "parent_id": parent_id,
         }
         r = requests.post(
             f"https://scratch.mit.edu/site-api/comments/user/{self.username}/add/",
@@ -592,51 +658,63 @@
         return requests.get(f"https://scratch.mit.edu/messages/ajax/user-activity/?user={self.username}&max={limit}").text
 
 
     def follow(self):
         """
         Follows the user represented by the User object. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
         requests.put(
             f"https://scratch.mit.edu/site-api/users/followers/{self.username}/add/?usernames={self._session._username}",
             headers = headers,
             cookies = self._cookies,
         )
 
     def unfollow(self):
         """
         Unfollows the user represented by the User object. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
         requests.put(
             f"https://scratch.mit.edu/site-api/users/followers/{self.username}/remove/?usernames={self._session._username}",
             headers = headers,
             cookies = self._cookies,
         )
 
     def delete_comment(self, *, comment_id):
         """
         Deletes a comment. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
 
         Args:
             comment_id: The id of the comment that should be deleted
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
         return requests.post(
             f"https://scratch.mit.edu/site-api/comments/user/{self.username}/del/",
             headers = headers,
             cookies = self._cookies,
             data = json.dumps({"id":str(comment_id)})
         )
 
     def report_comment(self, *, comment_id):
         """
         Reports a comment to the Scratch team. You can only use this function if this object was created using :meth:`scratchattach.session.Session.connect_user`  
 
         Args:
             comment_id: The id of the comment that should be reported
         """
+        if self._session is None:
+            raise(exceptions.Unauthenticated)
+            return
         return requests.post(
             f"https://scratch.mit.edu/site-api/comments/user/{self.username}/rep/",
             headers = headers,
             cookies = self._cookies,
             data = json.dumps({"id":str(comment_id)})
         )
```

### Comparing `scratchattach-1.7.2/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.7.3/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.7.2
-Summary: An Scratch API Wrapper for scra tch.mit.edu
+Version: 1.7.3
+Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
-Author-email: timkrome2006@gmail.com
+Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scratchattach-1.7.2/setup.py` & `scratchattach-1.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.7.2'
-DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
+VERSION = '1.7.3'
+DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
     author="TimMcCool",
-    author_email="timkrome2006@gmail.com",
+    author_email="timmccool.scratch@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     packages=find_packages(),
     install_requires=["websocket-client","numpy","requests","bs4"],
     keywords=['scratch api', 'scratchattach', 'scratch api python', 'scratch python', 'scratch for python', 'scratch', 'scratch cloud', 'scratch cloud variables', 'scratch bot'],
     url='https://github.com/TimMcCool/scratchattach',
```

