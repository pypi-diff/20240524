# Comparing `tmp/python_115-0.0.8.tar.gz` & `tmp/python_115-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.tar", max compression
+gzip compressed data, was "python_115-0.0.8.1.tar", max compression
```

## Comparing `python_115-0.0.8.tar` & `python_115-0.0.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8/p115/component/cipher.py
--rwxr-xr-x   0        0        0   241057 2024-05-23 10:53:22.107922 python_115-0.0.8/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8/p115/component/exception.py
--rwxr-xr-x   0        0        0    56834 2024-05-22 18:10:09.814988 python_115-0.0.8/p115/component/fs.py
--rwxr-xr-x   0        0        0    48067 2024-05-22 14:42:11.490047 python_115-0.0.8/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12216 2024-05-22 18:05:34.938601 python_115-0.0.8/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8/p115/component/labellist.py
--rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8/p115/component/offline.py
--rwxr-xr-x   0        0        0     3877 2024-05-22 14:04:09.272894 python_115-0.0.8/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     4950 2024-05-22 14:04:19.641910 python_115-0.0.8/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8/p115/py.typed
--rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8/p115/tool/__init__.py
--rw-r--r--   0        0        0     1591 2024-05-23 14:39:19.584144 python_115-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8/readme.md
--rw-r--r--   0        0        0    36270 1970-01-01 00:00:00.000000 python_115-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.1/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.1/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.1/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.1/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.1/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.1/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.1/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.1/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.1/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.1/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   241090 2024-05-23 16:00:08.933463 python_115-0.0.8.1/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.1/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.1/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48067 2024-05-22 14:42:11.490047 python_115-0.0.8.1/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12217 2024-05-23 16:03:44.547969 python_115-0.0.8.1/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.1/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.1/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.1/p115/component/offline.py
+-rwxr-xr-x   0        0        0     3877 2024-05-22 14:04:09.272894 python_115-0.0.8.1/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     4950 2024-05-22 14:04:19.641910 python_115-0.0.8.1/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.1/p115/py.typed
+-rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.1/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-23 16:05:10.412650 python_115-0.0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.1/readme.md
+-rw-r--r--   0        0        0    36272 1970-01-01 00:00:00.000000 python_115-0.0.8.1/PKG-INFO
```

### Comparing `python_115-0.0.8/LICENSE` & `python_115-0.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/cmd/iterdir.py` & `python_115-0.0.8.1/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/cmd/qrcode.py` & `python_115-0.0.8.1/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/__init__.py` & `python_115-0.0.8.1/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/cipher.py` & `python_115-0.0.8.1/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/client.py` & `python_115-0.0.8.1/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     bytes_ensure_part_iter, bytes_ensure_part_async_iter, 
 )
 from hashtools import file_digest, file_digest_async
 from http_request import encode_multipart_data, encode_multipart_data_async, SupportsGeturl
 from http_response import get_content_length, get_filename, get_total_length, is_range_request
 from httpfile import RequestsFileReader # TODO: use urllib3 instead
 from httpx import AsyncClient, Client, Cookies, TimeoutException
-from httpx_request import request
+from httpx_request import request as httpx_request
 from iterutils import through, async_through, wrap_iter, wrap_aiter
 from multidict import CIMultiDict
 from qrcode import QRCode # type: ignore
 from startfile import startfile, startfile_async # type: ignore
 from urlopen import urlopen
 from yarl import URL
 
@@ -68,14 +68,16 @@
 
 RequestVarT = TypeVar("RequestVarT", dict, Callable)
 RSA_ENCODER: Final = P115RSACipher()
 ECDH_ENCODER: Final = P115ECDHCipher()
 CRE_SHARE_LINK_search = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?").search
 APP_VERSION: Final = "99.99.99.99"
 
+request = partial(httpx_request, parse=lambda _, content: loads(content))
+
 
 def to_base64(s: bytes | str, /) -> str:
     if isinstance(s, str):
         s = bytes(s, "utf-8")
     return str(b64encode(s), "ascii")
 
 
@@ -302,24 +304,22 @@
         ns.pop("async_session", None)
 
     def request(
         self, 
         /, 
         url: str, 
         method: str = "GET", 
-        parse: None | bool | Callable = lambda _, content: loads(content), 
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ):
         """帮助函数：可执行同步和异步的网络请求
         """
         return request(
             url, 
             method=method, 
-            parse=parse, 
             async_=async_, 
             session=self.async_session if async_ else self.session, # type: ignore
             **request_kwargs, 
         )
 
     ########## Login API ##########
 
@@ -3422,16 +3422,16 @@
         api = "https://proapi.115.com/app/share/downurl"
         def parse(resp, content: bytes) -> dict:
             resp = loads(content)
             if resp["state"]:
                 resp["data"] = loads(RSA_ENCODER.decode(resp["data"]))
             return resp
         request_kwargs["parse"] = parse
-        data = RSA_ENCODER.encode(dumps(payload))
-        return self.request(api, "POST", data={"data": data}, async_=async_, **request_kwargs)
+        request_kwargs["data"] = RSA_ENCODER.encode(dumps(payload)).decode("ascii")
+        return self.request(api, "POST", async_=async_, **request_kwargs)
 
     @overload
     def share_download_url(
         self, 
         payload: dict, 
         /, 
         detail: bool = False, 
@@ -3566,18 +3566,18 @@
             payload = {"pickcode": payload}
         def parse(resp, content: bytes) -> dict:
             resp = loads(content)
             if resp["state"]:
                 resp["data"] = loads(RSA_ENCODER.decode(resp["data"]))
             return resp
         request_kwargs["parse"] = parse
+        request_kwargs["data"] = {"data": RSA_ENCODER.encode(dumps(payload)).decode("ascii")}
         return self.request(
             api, 
             "POST", 
-            data={"data": RSA_ENCODER.encode(dumps(payload))}, 
             async_=async_, 
             **request_kwargs, 
         )
 
     @overload
     def download_url(
         self,
```

### Comparing `python_115-0.0.8/p115/component/fs.py` & `python_115-0.0.8.1/p115/component/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 def normalize_info(
     info: Mapping, 
     keep_raw: bool = False, 
     **extra_data, 
 ) -> dict:
     if "fid" in info:
         fid = info["fid"]
-        parent_id = info["id"]
+        parent_id = info["cid"]
         is_dir = False
     else:
-        fid = info["id"]
+        fid = info["cid"]
         parent_id = info["pid"]
         is_dir = True
     info2 =  {
         "name": info["n"], 
         "is_directory": is_dir, 
         "size": info.get("s"), 
         "id": int(fid), 
@@ -382,15 +382,15 @@
     ) -> dict:
         resp = check_response(self.client.fs_files({
             "cid": id, 
             "limit": limit, 
             "offset": offset, 
             "show_dir": 1, 
         }))
-        if id and int(resp["path"][-1]["id"]) != id:
+        if id and int(resp["path"][-1]["cid"]) != id:
             raise NotADirectoryError(errno.ENOTDIR, f"{id} is not a directory")
         return resp
 
     @check_response
     def fs_search(self, payload: str | dict, /) -> dict:
         return self.client.fs_search(payload)
 
@@ -932,15 +932,15 @@
                 )
         return self.attr(dst_attr["id"])
 
     def _dir_get_ancestors(self, id: int, /) -> list[dict]:
         ls = [{"name": "", "id": 0, "parent_id": 0, "is_directory": True}]
         if id:
             ls.extend(
-                {"name": p["name"], "id": int(p["id"]), "parent_id": int(p["pid"]), "is_directory": True} 
+                {"name": p["name"], "id": int(p["cid"]), "parent_id": int(p["pid"]), "is_directory": True} 
                 for p in self.fs_files(id, limit=1)["path"][1:]
             )
         return ls
 
     def desc(
         self, 
         id_or_path: IDOrPathType = "", 
@@ -1129,15 +1129,15 @@
         exists = False
         for name in patht:
             try:
                 attr = get_attr([name], pid)
             except FileNotFoundError:
                 exists = False
                 resp = self.fs_mkdir(name, pid)
-                pid = int(resp["id"])
+                pid = int(resp["cid"])
                 attr = get_attr(pid)
             else:
                 exists = True
                 if not attr["is_directory"]:
                     raise NotADirectoryError(errno.ENOTDIR, f"{path!r} (in {pid!r}): there is a superior non-directory")
                 pid = attr["id"]
         if not exist_ok and exists:
@@ -1174,15 +1174,15 @@
                     raise NotADirectoryError(errno.ENOTDIR, f"{attr['id']!r} ({name!r} in {pid!r}) not a directory")
                 pid = attr["id"]
         else:
             raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) already exists")
         if i < len(patht):
             raise FileNotFoundError(errno.ENOENT, f"{path!r} (in {pid!r}) missing superior directory")
         resp = self.fs_mkdir(name, pid)
-        return self.attr(int(resp["id"]))
+        return self.attr(int(resp["cid"]))
 
     def move(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: Optional[int] = None,
```

### Comparing `python_115-0.0.8/p115/component/fs_base.py` & `python_115-0.0.8.1/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/fs_share.py` & `python_115-0.0.8.1/p115/component/fs_share.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,29 +33,29 @@
 def normalize_info(
     info: Mapping, 
     keep_raw: bool = False, 
     **extra_data, 
 ) -> dict:
     if "fid" in info:
         fid = info["fid"]
-        parent_id = info["id"]
+        parent_id = info["cid"]
         is_dir = False
     else:
-        fid = info["id"]
+        fid = info["cid"]
         parent_id = info["pid"]
         is_dir = True
     info2 =  {
         "name": info["n"], 
         "is_directory": is_dir, 
         "size": info.get("s"), 
         "id": int(fid), 
         "parent_id": int(parent_id), 
         "sha1": info.get("sha"), 
     }
-    timestamp = info2["timestamp"] = int(info2["t"])
+    timestamp = info2["timestamp"] = int(info["t"])
     info2["time"] = datetime.fromtimestamp(timestamp)
     if "pc" in info:
         info2["pickcode"] = info["pc"]
     if "fl" in info:
         info2["labels"] = info["fl"]
     if "c" in info:
         info2["violated"] = bool(info["c"])
```

### Comparing `python_115-0.0.8/p115/component/fs_zip.py` & `python_115-0.0.8.1/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/labellist.py` & `python_115-0.0.8.1/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/offline.py` & `python_115-0.0.8.1/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/recyclebin.py` & `python_115-0.0.8.1/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/component/sharing.py` & `python_115-0.0.8.1/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/p115/tool/__init__.py` & `python_115-0.0.8.1/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/pyproject.toml` & `python_115-0.0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8"
+version = "0.0.8.1"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8/readme.md` & `python_115-0.0.8.1/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8/PKG-INFO` & `python_115-0.0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

