# Comparing `tmp/GofileIOUploader-0.9.8.tar.gz` & `tmp/GofileIOUploader-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GofileIOUploader-0.9.8.tar", last modified: Sat Mar 30 19:58:14 2024, max compression
+gzip compressed data, was "GofileIOUploader-0.9.9.tar", last modified: Wed Apr  3 22:22:17 2024, max compression
```

## Comparing `GofileIOUploader-0.9.8.tar` & `GofileIOUploader-0.9.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-03-30 19:58:14.843777 GofileIOUploader-0.9.8/
--rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-03-28 21:55:26.000000 GofileIOUploader-0.9.8/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1001)     3276 2024-03-30 19:58:14.843777 GofileIOUploader-0.9.8/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)     2260 2024-03-30 17:01:47.000000 GofileIOUploader-0.9.8/README.md
--rw-r--r--   0 alex      (1000) alex      (1001)     1619 2024-03-30 17:04:28.000000 GofileIOUploader-0.9.8/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-03-30 19:58:14.843777 GofileIOUploader-0.9.8/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-03-30 19:58:14.843777 GofileIOUploader-0.9.8/src/
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-03-30 19:58:14.843777 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     3276 2024-03-30 19:58:14.000000 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      421 2024-03-30 19:58:14.000000 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-03-30 19:58:14.000000 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-03-30 19:58:14.000000 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-03-30 19:58:14.000000 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       16 2024-03-30 19:58:14.000000 GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-03-30 19:58:14.843777 GofileIOUploader-0.9.8/src/gofile_uploader/
--rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-03-30 16:59:15.000000 GofileIOUploader-0.9.8/src/gofile_uploader/__init__.py
--rwxr-xr-x   0 alex      (1000) alex      (1001)    14176 2024-03-30 17:01:47.000000 GofileIOUploader-0.9.8/src/gofile_uploader/gofile_uploader.py
--rw-r--r--   0 alex      (1000) alex      (1001)     2829 2024-03-29 14:49:47.000000 GofileIOUploader-0.9.8/src/gofile_uploader/types.py
--rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-03-30 16:54:50.000000 GofileIOUploader-0.9.8/src/gofile_uploader.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-03 22:22:17.181884 GofileIOUploader-0.9.9/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-03-28 21:55:26.000000 GofileIOUploader-0.9.9/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1001)     3276 2024-04-03 22:22:17.181884 GofileIOUploader-0.9.9/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)     2260 2024-03-30 17:01:47.000000 GofileIOUploader-0.9.9/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)     1619 2024-04-03 22:19:50.000000 GofileIOUploader-0.9.9/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-04-03 22:22:17.181884 GofileIOUploader-0.9.9/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-03 22:22:17.181884 GofileIOUploader-0.9.9/src/
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-03 22:22:17.181884 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     3276 2024-04-03 22:22:17.000000 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      421 2024-04-03 22:22:17.000000 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-04-03 22:22:17.000000 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-04-03 22:22:17.000000 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-04-03 22:22:17.000000 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       16 2024-04-03 22:22:17.000000 GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-04-03 22:22:17.181884 GofileIOUploader-0.9.9/src/gofile_uploader/
+-rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-03-30 16:59:15.000000 GofileIOUploader-0.9.9/src/gofile_uploader/__init__.py
+-rwxr-xr-x   0 alex      (1000) alex      (1001)    14511 2024-04-03 22:18:16.000000 GofileIOUploader-0.9.9/src/gofile_uploader/gofile_uploader.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     2829 2024-03-29 14:49:47.000000 GofileIOUploader-0.9.9/src/gofile_uploader/types.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-03-30 16:54:50.000000 GofileIOUploader-0.9.9/src/gofile_uploader.py
```

### Comparing `GofileIOUploader-0.9.8/LICENSE` & `GofileIOUploader-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GofileIOUploader-0.9.8/PKG-INFO` & `GofileIOUploader-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GofileIOUploader
-Version: 0.9.8
+Version: 0.9.9
 Summary: Gofile.io uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/gofile-uploader
 Project-URL: Repository, https://github.com/alexmi256/gofile-uploader.git
 Project-URL: Service, https://gofile.io
```

### Comparing `GofileIOUploader-0.9.8/README.md` & `GofileIOUploader-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `GofileIOUploader-0.9.8/pyproject.toml` & `GofileIOUploader-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GofileIOUploader"
-version = "0.9.8"
+version = "0.9.9"
 description = "Gofile.io uploader supporting parallel uploads"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["gofile", "upload", "storage", "parallel"]
 authors = [
     {name = "Alex Mi", email = "alexmi3.14@gmail.com"},
```

### Comparing `GofileIOUploader-0.9.8/src/GofileIOUploader.egg-info/PKG-INFO` & `GofileIOUploader-0.9.9/src/GofileIOUploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GofileIOUploader
-Version: 0.9.8
+Version: 0.9.9
 Summary: Gofile.io uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/gofile-uploader
 Project-URL: Repository, https://github.com/alexmi256/gofile-uploader.git
 Project-URL: Service, https://gofile.io
```

### Comparing `GofileIOUploader-0.9.8/src/gofile_uploader/gofile_uploader.py` & `GofileIOUploader-0.9.9/src/gofile_uploader/gofile_uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,27 +60,32 @@
         if tsize is not None:
             self.total = tsize
         return self.update(b * bsize - self.n)  # also sets self.n = b * bsize
 
 
 class GofileIOAPI:
     def __init__(
-        self, token: Optional[str] = None, max_connections: int = 4, zone: Optional[Literal["eu", "na"]] = None
+        self,
+        token: Optional[str] = None,
+        max_connections: int = 4,
+        zone: Optional[Literal["eu", "na"]] = None,
+        retries: int = 1,
     ):
         self.token = token
         self.session_headers = {"Authorization": f"Bearer {self.token}"} if self.token else None
         self.session = aiohttp.ClientSession("https://api.gofile.io", headers=self.session_headers)
         self.zone = zone
         self.root_folder_id = None
         self.account_id = None
         self.is_premium = False
         self.make_public = False
         self.server_sessions = {}
         self.created_folders = {}
         self.sem = asyncio.Semaphore(max_connections)
+        self.retries = retries
 
     async def init(self):
         account_id = await self.get_account_id()
         self.account_id = account_id["data"]["id"]
 
         if self.token is not None:
             account = await self.get_account_details(self.account_id)
@@ -163,15 +168,15 @@
             if "status" not in response or response["status"] != "ok":
                 raise Exception(response)
             return response["data"]
 
     async def upload_file(self, file_path: Path, folder_id: Optional[str] = None, tqdm_index=1) -> list[str]:
         async with self.sem:
             retries = 0
-            while retries < 1:
+            while retries < self.retries:
                 try:
                     # TODO: Rate limit to one request every 10 seconds
                     servers = await self.get_servers(zone=self.zone)
 
                     server = next(iter(servers["data"]["servers"]))["name"]
                     if server not in self.server_sessions:
                         logger.info(f"Using new server connection to {server}")
@@ -224,16 +229,17 @@
 class GofileIOUploader:
     def __init__(
         self,
         token: Optional[str] = None,
         max_connections: int = 4,
         make_public: bool = False,
         zone: Optional[Literal["eu", "na"]] = None,
+        retries: int = 1,
     ):
-        self.api = GofileIOAPI(token, max_connections=max_connections, zone=zone)
+        self.api = GofileIOAPI(token, max_connections=max_connections, zone=zone, retries=retries)
         self.make_public = make_public
 
     async def init(self) -> None:
         try:
             if self.api.token is not None:
                 await self.api.init()
 
@@ -274,28 +280,26 @@
         folder_id = await self.get_folder_id(folder)
 
         if self.make_public and folder_id != self.api.root_folder_id:
             logger.info(f"Making folder {folder_id} public")
             await self.api.update_content(folder_id, "public", "true")
 
         responses = await self.api.upload_files(paths, folder_id)
-        if save:
+        if save and responses:
             file_name = f"gofile_upload_{int(time.time())}.csv"
             with open(file_name, "w", newline="") as csvfile:
                 logger.info(f"Saving uploaded files to {file_name}")
                 csv_writer = csv.writer(csvfile, dialect="excel")
-                csv_writer.writerows(responses)
+                csv_writer.writerows([x for x in responses if x])
         else:
             pprint(responses)
 
 
 def cli():
-    parser = argparse.ArgumentParser(
-        prog="gofile-upload", description="Gofile.io Uploader supporting parallel uploads"
-    )
+    parser = argparse.ArgumentParser(prog="gofile-upload", description="Gofile.io Uploader supporting parallel uploads")
     parser.add_argument("file", type=str, help="File or directory to look for files in to upload")
     parser.add_argument(
         "-t",
         "--token",
         type=str,
         default=os.getenv("GOFILE_TOKEN"),
         help="""API token for your account so that you can upload to a specific account/folder.
@@ -320,24 +324,31 @@
     )
     parser.add_argument(
         "--save",
         action=argparse.BooleanOptionalAction,
         default=True,
         help='Don\'t save uploaded file urls to a "gofile_upload_<unixtime>.csv" file',
     )
+    parser.add_argument(
+        "-r",
+        "--retries",
+        default=3,
+        type=int,
+        help="How many times to retry a failed upload",
+    )
     args = parser.parse_args()
 
     return args
 
 
 async def async_main() -> None:
     args = cli()
     logger.debug(args)
     gofile_client = GofileIOUploader(
-        args.token, max_connections=args.connections, make_public=args.public, zone=args.zone
+        args.token, max_connections=args.connections, make_public=args.public, zone=args.zone, retries=args.retries
     )
 
     try:
         await gofile_client.init()
         await gofile_client.upload_files(args.file, args.folder, args.save)
     finally:
         if not gofile_client.api.session.closed:
```

### Comparing `GofileIOUploader-0.9.8/src/gofile_uploader/types.py` & `GofileIOUploader-0.9.9/src/gofile_uploader/types.py`

 * *Files identical despite different names*

