# Comparing `tmp/media_tools-0.4.5.tar.gz` & `tmp/media_tools-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_tools-0.4.5.tar", max compression
+gzip compressed data, was "media_tools-0.4.6.tar", max compression
```

## Comparing `media_tools-0.4.5.tar` & `media_tools-0.4.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1068 2024-03-24 14:49:31.731787 media_tools-0.4.5/LICENSE
--rw-r--r--   0        0        0    13066 2024-03-24 14:49:31.731787 media_tools-0.4.5/README.md
--rw-r--r--   0        0        0        0 2024-03-24 14:49:31.766787 media_tools-0.4.5/media_tools/__init__.py
--rw-r--r--   0        0        0     1990 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/backup_lastfm_data.py
--rw-r--r--   0        0        0     3403 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/buy_most_played.py
--rwxr-xr-x   0        0        0     5419 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/clean_filenames.py
--rwxr-xr-x   0        0        0     3991 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/copy_from_playlist.py
--rw-r--r--   0        0        0     7703 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/mixcloud_upload.py
--rw-r--r--   0        0        0     5532 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/play_time.py
--rw-r--r--   0        0        0      647 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/util/__init__.py
--rw-r--r--   0        0        0     3630 2024-03-24 14:49:31.731787 media_tools-0.4.5/media_tools/util/audacious_tools.py
--rw-r--r--   0        0        0      719 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/base_filename_cleaner.py
--rw-r--r--   0        0        0       51 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/buying/__init__.py
--rw-r--r--   0        0        0     1486 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/buying/distributor.py
--rw-r--r--   0        0        0     2745 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/buying/last_fm.py
--rw-r--r--   0        0        0     1181 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/buying/retry_http.py
--rw-r--r--   0        0        0     2180 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/buying/track.py
--rw-r--r--   0        0        0     1098 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/buying/trackdb.py
--rw-r--r--   0        0        0     1526 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/command.py
--rw-r--r--   0        0        0     1124 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/dump_data.py
--rw-r--r--   0        0        0     2630 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/duplicate_string_remover.py
--rw-r--r--   0        0        0      844 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/extension_lowercaser.py
--rw-r--r--   0        0        0     2220 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/junk_remover.py
--rw-r--r--   0        0        0      828 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/lastfm_user.py
--rw-r--r--   0        0        0     1907 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/length_reader.py
--rw-r--r--   0        0        0      489 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/logging.py
--rw-r--r--   0        0        0      173 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/media_extensions.py
--rw-r--r--   0        0        0      418 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/mixcloud/__init__.py
--rw-r--r--   0        0        0      100 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/mixcloud/authorization_error.py
--rw-r--r--   0        0        0      599 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/mixcloud/constants.py
--rw-r--r--   0        0        0     6555 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/mixcloud/create_api_token.py
--rw-r--r--   0        0        0     1910 2024-03-24 14:49:31.732787 media_tools-0.4.5/media_tools/util/mixcloud/globals.py
--rw-r--r--   0        0        0    10737 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/mixcloud/mix.py
--rw-r--r--   0        0        0     1720 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/mixcloud/mix_path.py
--rw-r--r--   0        0        0     2405 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/mixcloud/multi_mix.py
--rw-r--r--   0        0        0     3536 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/mixcloud/oauth_parameter_receiver.py
--rw-r--r--   0        0        0     5810 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/numbering_fixer.py
--rw-r--r--   0        0        0     2996 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/playlist_copier.py
--rw-r--r--   0        0        0     3847 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/scrobbles.py
--rw-r--r--   0        0        0     2242 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/symlink_fixer.py
--rw-r--r--   0        0        0      702 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/undo_commands.py
--rw-r--r--   0        0        0     1080 2024-03-24 14:49:31.733787 media_tools-0.4.5/media_tools/util/util.py
--rw-r--r--   0        0        0     1534 2024-03-24 14:49:31.734787 media_tools-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    14194 1970-01-01 00:00:00.000000 media_tools-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 08:46:38.501137 media_tools-0.4.6/LICENSE
+-rw-r--r--   0        0        0    13066 2024-05-24 08:46:38.501137 media_tools-0.4.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 08:46:38.548137 media_tools-0.4.6/media_tools/__init__.py
+-rw-r--r--   0        0        0     1990 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/backup_lastfm_data.py
+-rw-r--r--   0        0        0     3403 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/buy_most_played.py
+-rwxr-xr-x   0        0        0     5419 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/clean_filenames.py
+-rwxr-xr-x   0        0        0     3991 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/copy_from_playlist.py
+-rw-r--r--   0        0        0     7703 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/mixcloud_upload.py
+-rw-r--r--   0        0        0     5532 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/play_time.py
+-rw-r--r--   0        0        0      647 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/util/__init__.py
+-rw-r--r--   0        0        0     3630 2024-05-24 08:46:38.502137 media_tools-0.4.6/media_tools/util/audacious_tools.py
+-rw-r--r--   0        0        0      719 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/base_filename_cleaner.py
+-rw-r--r--   0        0        0       51 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/buying/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/buying/distributor.py
+-rw-r--r--   0        0        0     2745 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/buying/last_fm.py
+-rw-r--r--   0        0        0     1181 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/buying/retry_http.py
+-rw-r--r--   0        0        0     2180 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/buying/track.py
+-rw-r--r--   0        0        0     1098 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/buying/trackdb.py
+-rw-r--r--   0        0        0     1526 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/command.py
+-rw-r--r--   0        0        0     1124 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/dump_data.py
+-rw-r--r--   0        0        0     2630 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/duplicate_string_remover.py
+-rw-r--r--   0        0        0      844 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/extension_lowercaser.py
+-rw-r--r--   0        0        0     2220 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/junk_remover.py
+-rw-r--r--   0        0        0      828 2024-05-24 08:46:38.503136 media_tools-0.4.6/media_tools/util/lastfm_user.py
+-rw-r--r--   0        0        0     1907 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/length_reader.py
+-rw-r--r--   0        0        0      489 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/logging.py
+-rw-r--r--   0        0        0      173 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/media_extensions.py
+-rw-r--r--   0        0        0      418 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/authorization_error.py
+-rw-r--r--   0        0        0      599 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/constants.py
+-rw-r--r--   0        0        0     6555 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/create_api_token.py
+-rw-r--r--   0        0        0     1910 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/globals.py
+-rw-r--r--   0        0        0    10737 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/mix.py
+-rw-r--r--   0        0        0     1720 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/mix_path.py
+-rw-r--r--   0        0        0     2405 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/multi_mix.py
+-rw-r--r--   0        0        0     3527 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/mixcloud/oauth_parameter_receiver.py
+-rw-r--r--   0        0        0     5810 2024-05-24 08:46:38.504137 media_tools-0.4.6/media_tools/util/numbering_fixer.py
+-rw-r--r--   0        0        0     2996 2024-05-24 08:46:38.505137 media_tools-0.4.6/media_tools/util/playlist_copier.py
+-rw-r--r--   0        0        0     3847 2024-05-24 08:46:38.505137 media_tools-0.4.6/media_tools/util/scrobbles.py
+-rw-r--r--   0        0        0     2242 2024-05-24 08:46:38.505137 media_tools-0.4.6/media_tools/util/symlink_fixer.py
+-rw-r--r--   0        0        0      702 2024-05-24 08:46:38.505137 media_tools-0.4.6/media_tools/util/undo_commands.py
+-rw-r--r--   0        0        0     1080 2024-05-24 08:46:38.505137 media_tools-0.4.6/media_tools/util/util.py
+-rw-r--r--   0        0        0     1534 2024-05-24 08:46:38.506137 media_tools-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    14194 1970-01-01 00:00:00.000000 media_tools-0.4.6/PKG-INFO
```

### Comparing `media_tools-0.4.5/LICENSE` & `media_tools-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/README.md` & `media_tools-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/backup_lastfm_data.py` & `media_tools-0.4.6/media_tools/backup_lastfm_data.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/buy_most_played.py` & `media_tools-0.4.6/media_tools/buy_most_played.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/clean_filenames.py` & `media_tools-0.4.6/media_tools/clean_filenames.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/copy_from_playlist.py` & `media_tools-0.4.6/media_tools/copy_from_playlist.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/mixcloud_upload.py` & `media_tools-0.4.6/media_tools/mixcloud_upload.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/play_time.py` & `media_tools-0.4.6/media_tools/play_time.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/__init__.py` & `media_tools-0.4.6/media_tools/util/__init__.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/audacious_tools.py` & `media_tools-0.4.6/media_tools/util/audacious_tools.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/base_filename_cleaner.py` & `media_tools-0.4.6/media_tools/util/base_filename_cleaner.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/buying/distributor.py` & `media_tools-0.4.6/media_tools/util/buying/distributor.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/buying/last_fm.py` & `media_tools-0.4.6/media_tools/util/buying/last_fm.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/buying/retry_http.py` & `media_tools-0.4.6/media_tools/util/buying/retry_http.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/buying/track.py` & `media_tools-0.4.6/media_tools/util/buying/track.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/buying/trackdb.py` & `media_tools-0.4.6/media_tools/util/buying/trackdb.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/command.py` & `media_tools-0.4.6/media_tools/util/command.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/dump_data.py` & `media_tools-0.4.6/media_tools/util/dump_data.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/duplicate_string_remover.py` & `media_tools-0.4.6/media_tools/util/duplicate_string_remover.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/extension_lowercaser.py` & `media_tools-0.4.6/media_tools/util/extension_lowercaser.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/junk_remover.py` & `media_tools-0.4.6/media_tools/util/junk_remover.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/lastfm_user.py` & `media_tools-0.4.6/media_tools/util/lastfm_user.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/length_reader.py` & `media_tools-0.4.6/media_tools/util/length_reader.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/constants.py` & `media_tools-0.4.6/media_tools/util/mixcloud/constants.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/create_api_token.py` & `media_tools-0.4.6/media_tools/util/mixcloud/create_api_token.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/globals.py` & `media_tools-0.4.6/media_tools/util/mixcloud/globals.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/mix.py` & `media_tools-0.4.6/media_tools/util/mixcloud/mix.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/mix_path.py` & `media_tools-0.4.6/media_tools/util/mixcloud/mix_path.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/multi_mix.py` & `media_tools-0.4.6/media_tools/util/mixcloud/multi_mix.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/mixcloud/oauth_parameter_receiver.py` & `media_tools-0.4.6/media_tools/util/mixcloud/oauth_parameter_receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         self.end_headers()
         self.wfile.write(
             bytes(f"""
     <html>
       <head><title>{title}</title></head>
       <body><p>{request_query}</p><p>{message}</p></body>
     </html>
-    """,
-                  'utf-8'))
+    """, 'utf-8')
+        )
 
 
 class OAuthCodeReceiver(OAuthParameterReceiver):
     """
     When registering an app with the Mixcloud API to receive a token, the API
     requires a redirect URL for a callback:
     `https://www.mixcloud.com/oauth/authorize?client_id=YOUR_CLIENT_ID
```

### Comparing `media_tools-0.4.5/media_tools/util/numbering_fixer.py` & `media_tools-0.4.6/media_tools/util/numbering_fixer.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/playlist_copier.py` & `media_tools-0.4.6/media_tools/util/playlist_copier.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/scrobbles.py` & `media_tools-0.4.6/media_tools/util/scrobbles.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/symlink_fixer.py` & `media_tools-0.4.6/media_tools/util/symlink_fixer.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/undo_commands.py` & `media_tools-0.4.6/media_tools/util/undo_commands.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/media_tools/util/util.py` & `media_tools-0.4.6/media_tools/util/util.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.5/pyproject.toml` & `media_tools-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-tools"
-version = "0.4.5"
+version = "0.4.6"
 description = "Creating and managing playlists, and managing the filenames and directory structure for large numbers of music files."
 authors = ["Lene Preuss <lene.preuss@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lilacashes/music-library-tools"
 repository = "https://gitlab.com/lilacashes/music-library-tools.git"
 keywords = ["music", "audio"]
```

### Comparing `media_tools-0.4.5/PKG-INFO` & `media_tools-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-tools
-Version: 0.4.5
+Version: 0.4.6
 Summary: Creating and managing playlists, and managing the filenames and directory structure for large numbers of music files.
 Home-page: https://gitlab.com/lilacashes/music-library-tools
 License: MIT
 Keywords: music,audio
 Author: Lene Preuss
 Author-email: lene.preuss@gmail.com
 Requires-Python: >=3.9,<4.0
```

