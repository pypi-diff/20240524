# Comparing `tmp/ktoolbox-0.6.0.tar.gz` & `tmp/ktoolbox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktoolbox-0.6.0.tar", max compression
+gzip compressed data, was "ktoolbox-0.7.0.tar", max compression
```

## Comparing `ktoolbox-0.6.0.tar` & `ktoolbox-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1533 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/LICENSE
--rw-r--r--   0        0        0     5054 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/README.md
--rw-r--r--   0        0        0      166 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/__init__.py
--rw-r--r--   0        0        0      475 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/__main__.py
--rw-r--r--   0        0        0      949 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/_enum.py
--rw-r--r--   0        0        0      103 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/action/__init__.py
--rw-r--r--   0        0        0      192 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/action/base.py
--rw-r--r--   0        0        0     1187 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/action/fetch.py
--rw-r--r--   0        0        0     7470 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/action/job.py
--rw-r--r--   0        0        0     3252 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/action/search.py
--rw-r--r--   0        0        0     3085 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/action/utils.py
--rw-r--r--   0        0        0      172 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/__init__.py
--rw-r--r--   0        0        0     4143 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/base.py
--rw-r--r--   0        0        0       31 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/misc/__init__.py
--rw-r--r--   0        0        0      483 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/misc/get_app_version.py
--rw-r--r--   0        0        0       71 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/model/__init__.py
--rw-r--r--   0        0        0      405 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/model/announcement.py
--rw-r--r--   0        0        0      581 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/model/creator.py
--rw-r--r--   0        0        0      831 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/model/post.py
--rw-r--r--   0        0        0      116 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/posts/__init__.py
--rw-r--r--   0        0        0      780 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/posts/get_announcement.py
--rw-r--r--   0        0        0      988 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/posts/get_creator_post.py
--rw-r--r--   0        0        0      620 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/posts/get_creators.py
--rw-r--r--   0        0        0      761 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/posts/get_post.py
--rw-r--r--   0        0        0      836 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/api/utils.py
--rw-r--r--   0        0        0    10081 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/cli.py
--rw-r--r--   0        0        0     7926 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/configuration.py
--rw-r--r--   0        0        0       67 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/downloader/__init__.py
--rw-r--r--   0        0        0      200 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/downloader/base.py
--rw-r--r--   0        0        0     9705 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/downloader/downloader.py
--rw-r--r--   0        0        0     2913 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/downloader/utils.py
--rw-r--r--   0        0        0       43 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/job/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/job/model.py
--rw-r--r--   0        0        0     6817 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/job/runner.py
--rw-r--r--   0        0        0      719 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/model.py
--rw-r--r--   0        0        0     3709 2024-05-05 12:48:31.918896 ktoolbox-0.6.0/ktoolbox/utils.py
--rw-r--r--   0        0        0     1946 2024-05-05 12:48:31.922896 ktoolbox-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6418 1970-01-01 00:00:00.000000 ktoolbox-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-24 18:03:21.008424 ktoolbox-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5054 2024-05-24 18:03:21.008424 ktoolbox-0.7.0/README.md
+-rw-r--r--   0        0        0      166 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/__main__.py
+-rw-r--r--   0        0        0      949 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/_enum.py
+-rw-r--r--   0        0        0      103 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/action/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/action/base.py
+-rw-r--r--   0        0        0     1229 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/action/fetch.py
+-rw-r--r--   0        0        0     7558 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/action/job.py
+-rw-r--r--   0        0        0     3252 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/action/search.py
+-rw-r--r--   0        0        0     3847 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/action/utils.py
+-rw-r--r--   0        0        0      172 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/__init__.py
+-rw-r--r--   0        0        0     4143 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/base.py
+-rw-r--r--   0        0        0       31 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/misc/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/misc/get_app_version.py
+-rw-r--r--   0        0        0       71 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/model/__init__.py
+-rw-r--r--   0        0        0      405 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/model/announcement.py
+-rw-r--r--   0        0        0      581 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/model/creator.py
+-rw-r--r--   0        0        0      831 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/model/post.py
+-rw-r--r--   0        0        0      116 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/posts/__init__.py
+-rw-r--r--   0        0        0      780 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/posts/get_announcement.py
+-rw-r--r--   0        0        0      988 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/posts/get_creator_post.py
+-rw-r--r--   0        0        0      620 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/posts/get_creators.py
+-rw-r--r--   0        0        0      761 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/posts/get_post.py
+-rw-r--r--   0        0        0      836 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/api/utils.py
+-rw-r--r--   0        0        0    10081 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/cli.py
+-rw-r--r--   0        0        0     8529 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/configuration.py
+-rw-r--r--   0        0        0       67 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/downloader/__init__.py
+-rw-r--r--   0        0        0      200 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/downloader/base.py
+-rw-r--r--   0        0        0     9720 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/downloader/downloader.py
+-rw-r--r--   0        0        0     2913 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/downloader/utils.py
+-rw-r--r--   0        0        0       43 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/job/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/job/model.py
+-rw-r--r--   0        0        0     6817 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/job/runner.py
+-rw-r--r--   0        0        0      719 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/model.py
+-rw-r--r--   0        0        0     3709 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/ktoolbox/utils.py
+-rw-r--r--   0        0        0     1946 2024-05-24 18:03:21.012424 ktoolbox-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6418 1970-01-01 00:00:00.000000 ktoolbox-0.7.0/PKG-INFO
```

### Comparing `ktoolbox-0.6.0/LICENSE` & `ktoolbox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/README.md` & `ktoolbox-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/_enum.py` & `ktoolbox-0.7.0/ktoolbox/_enum.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/action/fetch.py` & `ktoolbox-0.7.0/ktoolbox/action/fetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     Fetch posts from a creator
 
     :param service: The service where the post is located
     :param creator_id: The ID of the creator
     :param o: Result offset, stepping of 50 is enforced
     :return: Async generator of several list of posts
-    :raise FetchInterruptError
+    :raise FetchInterruptError: Exception for interrupt of data fetching
     """
     while True:
         ret = await get_creator_post(service=service, creator_id=creator_id, o=o)
         if ret:
             yield ret.data
             if len(ret.data) < SEARCH_STEP:
                 break
```

### Comparing `ktoolbox-0.6.0/ktoolbox/action/job.py` & `ktoolbox-0.7.0/ktoolbox/action/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import aiofiles
 from loguru import logger
 from pathvalidate import sanitize_filename, is_valid_filename
 
 from ktoolbox._enum import PostFileTypeEnum, DataStorageNameEnum
 from ktoolbox.action import ActionRet, fetch_creator_posts, FetchInterruptError
-from ktoolbox.action.utils import generate_post_path_name, filter_posts_by_date
+from ktoolbox.action.utils import generate_post_path_name, filter_posts_by_date, generate_filename
 from ktoolbox.api.model import Post, Attachment
 from ktoolbox.configuration import config, PostStructureConfiguration
 from ktoolbox.job import Job, CreatorIndices
 
 __all__ = ["create_job_from_post", "create_job_from_creator"]
 
 
@@ -64,15 +64,16 @@
                 )
         )) and not any(
             map(
                 lambda x: fnmatch(file_path_obj.name, x),
                 config.job.block_list
             )
         ):
-            alt_filename = f"{i + 1}{file_path_obj.suffix}" if config.job.sequential_filename else file_path_obj.name
+            basic_filename = f"{i + 1}{file_path_obj.suffix}" if config.job.sequential_filename else file_path_obj.name
+            alt_filename = generate_filename(post, basic_filename)
             jobs.append(
                 Job(
                     path=attachments_path,
                     alt_filename=alt_filename,
                     server_path=attachment.path,
                     type=PostFileTypeEnum.Attachment
                 )
```

### Comparing `ktoolbox-0.6.0/ktoolbox/action/search.py` & `ktoolbox-0.7.0/ktoolbox/action/search.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/action/utils.py` & `ktoolbox-0.7.0/ktoolbox/action/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,40 +4,61 @@
 from loguru import logger
 from pathvalidate import sanitize_filename
 
 from ktoolbox.api.model import Post
 from ktoolbox.configuration import config
 from ktoolbox.job import CreatorIndices
 
-__all__ = ["generate_post_path_name", "filter_posts_by_date", "filter_posts_by_indices"]
+__all__ = ["generate_post_path_name", "generate_filename", "filter_posts_by_date", "filter_posts_by_indices"]
+
+TIME_FORMAT = "%Y-%m-%d"
 
 
 def generate_post_path_name(post: Post) -> str:
     """Generate directory name for post to save."""
     if config.job.post_id_as_path or not post.title:
         return post.id
     else:
-        time_format = "%Y-%m-%d"
         try:
             return sanitize_filename(
                 config.job.post_dirname_format.format(
                     id=post.id,
                     user=post.user,
                     service=post.service,
                     title=post.title,
-                    added=post.added.strftime(time_format) if post.added else "",
-                    published=post.published.strftime(time_format) if post.published else "",
-                    edited=post.edited.strftime(time_format) if post.edited else ""
+                    added=post.added.strftime(TIME_FORMAT) if post.added else "",
+                    published=post.published.strftime(TIME_FORMAT) if post.published else "",
+                    edited=post.edited.strftime(TIME_FORMAT) if post.edited else ""
                 )
             )
         except KeyError as e:
             logger.error(f"`JobConfiguration.post_dirname_format` contains invalid key: {e}")
             exit(1)
 
 
+def generate_filename(post: Post, basic_name: str) -> str:
+    """Generate download filename"""
+    try:
+        return sanitize_filename(
+            config.job.filename_format.format(
+                basic_name,
+                id=post.id,
+                user=post.user,
+                service=post.service,
+                title=post.title,
+                added=post.added.strftime(TIME_FORMAT) if post.added else "",
+                published=post.published.strftime(TIME_FORMAT) if post.published else "",
+                edited=post.edited.strftime(TIME_FORMAT) if post.edited else ""
+            )
+        )
+    except KeyError as e:
+        logger.error(f"`JobConfiguration.filename_format` contains invalid key: {e}")
+        exit(1)
+
+
 def _match_post_date(
         post: Post,
         start_date: Optional[datetime],
         end_date: Optional[datetime]
 ) -> bool:
     """
     Check if the post date match the time range.
```

### Comparing `ktoolbox-0.6.0/ktoolbox/api/base.py` & `ktoolbox-0.7.0/ktoolbox/api/base.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/model/creator.py` & `ktoolbox-0.7.0/ktoolbox/api/model/creator.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/model/post.py` & `ktoolbox-0.7.0/ktoolbox/api/model/post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/posts/get_announcement.py` & `ktoolbox-0.7.0/ktoolbox/api/posts/get_announcement.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/posts/get_creator_post.py` & `ktoolbox-0.7.0/ktoolbox/api/posts/get_creator_post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/posts/get_creators.py` & `ktoolbox-0.7.0/ktoolbox/api/posts/get_creators.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/posts/get_post.py` & `ktoolbox-0.7.0/ktoolbox/api/posts/get_post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/api/utils.py` & `ktoolbox-0.7.0/ktoolbox/api/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/cli.py` & `ktoolbox-0.7.0/ktoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/configuration.py` & `ktoolbox-0.7.0/ktoolbox/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,18 +105,18 @@
     ├─ <Post data (post.json)>
     └─ attachments
        ├─ 1.png
        └─ 2.png
     ```
 
     :ivar attachments: Sub path of attachment directory
-    :ivar content_filepath: Sub path of post content HTML file
+    :ivar content_filepath: Sub path of post content file
     """
     attachments: Path = Path("attachments")
-    content_filepath: Path = Path("index.html")
+    content_filepath: Path = Path("content.txt")
 
 
 class JobConfiguration(BaseModel):
     """
     Download jobs Configuration
 
     - Available properties for ``post_dirname_format``
@@ -130,29 +130,36 @@
         | ``added``     | Date   |
         | ``published`` | Date   |
         | ``edited``    | Date   |
 
     :ivar count: Number of coroutines for concurrent download
     :ivar post_id_as_path: (**Deprecated**) Use post ID as post directory name
     :ivar post_dirname_format: Customize the post directory name format, you can use some of the \
-    [properties](/configuration/reference/#ktoolbox.configuration.JobConfiguration) in ``Post``. \
+    [properties][ktoolbox.configuration.JobConfiguration] in ``Post``. \
     e.g. ``[{published}]{id}`` > ``[2024-1-1]123123``, ``{user}_{published}_{title}`` > ``234234_2024-1-1_HelloWorld``
     :ivar post_structure: Post path structure
     :ivar mix_posts: Save all files from different posts at same path in creator directory. \
     It would not create any post directory, and ``CreatorIndices`` would not been recorded.
     :ivar sequential_filename: Rename attachments in numerical order, e.g. ``1.png``, ``2.png``, ...
+    :ivar filename_format: Customize the filename format by inserting an empty ``{}`` to represent the basic filename.
+    Similar to post_dirname_format, you can use some of the [properties][ktoolbox.configuration.JobConfiguration] \
+    in Post. For example: ``{title}_{}`` could result in filenames like \
+    ``HelloWorld_b4b41de2-8736-480d-b5c3-ebf0d917561b``, ``HelloWorld_af349b25-ac08-46d7-98fb-6ce99a237b90``, etc. \
+    You can also use it with ``sequential_filename``. For instance, \
+    ``[{published}]_{}`` could result in filenames like ``[2024-1-1]_1.png``, ``[2024-1-1]_2.png``, etc.
     :ivar allow_list: Download files which match these patterns (Unix shell-style), e.g. ``["*.png"]``
     :ivar block_list: Not to download files which match these patterns (Unix shell-style), e.g. ``["*.psd","*.zip"]``
     """
     count: int = 4
     post_id_as_path: bool = False
     post_dirname_format: str = "{title}"
     post_structure: PostStructureConfiguration = PostStructureConfiguration()
     mix_posts: bool = False
     sequential_filename: bool = False
+    filename_format: str = "{}"
     allow_list: Set[str] = set()
     block_list: Set[str] = set()
 
     # job_list_filepath: Optional[Path] = None
     # """Filepath for job list data saving, ``None`` for disable job list saving"""
 
     @field_validator("post_id_as_path")
```

### Comparing `ktoolbox-0.6.0/ktoolbox/downloader/downloader.py` & `ktoolbox-0.7.0/ktoolbox/downloader/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         Start to download
 
         :param sync_callable: Sync callable for download finished
         :param async_callable: Async callable for download finished
         :param tqdm_class: ``tqdm`` class to replace default ``tqdm.asyncio.tqdm``
         :param progress: Show progress bar
         :return: ``DownloaderRet`` which contain the actual output filename
-        :raise CancelledError
+        :raise CancelledError: Job cancelled
         """
         # Get filename to check if file exists (First-time duplicate file check)
         # Check it before request to make progress more efficiency
         server_relpath = self._server_path[1:]
         server_relpath_without_params = urlparse(server_relpath).path
         server_path_filename = unquote(Path(server_relpath_without_params).name)
         # Priority order can be referenced from the constructor's documentation
```

### Comparing `ktoolbox-0.6.0/ktoolbox/downloader/utils.py` & `ktoolbox-0.7.0/ktoolbox/downloader/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/job/model.py` & `ktoolbox-0.7.0/ktoolbox/job/model.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/job/runner.py` & `ktoolbox-0.7.0/ktoolbox/job/runner.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/model.py` & `ktoolbox-0.7.0/ktoolbox/model.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/ktoolbox/utils.py` & `ktoolbox-0.7.0/ktoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox-0.6.0/pyproject.toml` & `ktoolbox-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ktoolbox"
-version = "0.6.0"
+version = "0.7.0"
 description = "A useful CLI tool for downloading posts in Kemono.party / .su"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.asia>"]
 readme = "README.md"
 homepage = "https://ktoolbox.readthedocs.io/"
 repository = "https://github.com/Ljzd-PRO/KToolBox"
 documentation = "https://ktoolbox.readthedocs.io/"
 
@@ -47,15 +47,15 @@
 mkdocs = "^1.5.3"
 mkdocs-static-i18n = "^1.2.0"
 mkdocs-material = "^9.4.14"
 mkdocstrings = {version="^0.24.0", extras=["python"]}
 mike = "^2.0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "==8.1.1"
+pytest = "==8.2.1"
 pytest-asyncio = "==0.23.5"
 pytest-cov = "==4.1.0"
 allpairspy = "==2.5.1"
 
 [tool.poetry.group.dev.dependencies]
 datamodel-code-generator = ">=0.22.1,<0.24.0"
```

### Comparing `ktoolbox-0.6.0/PKG-INFO` & `ktoolbox-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktoolbox
-Version: 0.6.0
+Version: 0.7.0
 Summary: A useful CLI tool for downloading posts in Kemono.party / .su
 Home-page: https://ktoolbox.readthedocs.io/
 Keywords: kemono,kemono.party,cli-app,downloader,os-independent
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ktoolbox Version: 0.6.0 Summary: A useful CLI tool
+Metadata-Version: 2.1 Name: ktoolbox Version: 0.7.0 Summary: A useful CLI tool
 for downloading posts in Kemono.party / .su Home-page: https://
 ktoolbox.readthedocs.io/ Keywords: kemono,kemono.party,cli-app,downloader,os-
 independent Author: Ljzd-PRO Author-email: ljzd@office.ljzd-pro.asia Requires-
 Python: >=3.8,<3.12 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

