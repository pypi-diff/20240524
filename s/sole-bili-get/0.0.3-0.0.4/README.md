# Comparing `tmp/sole_bili_get-0.0.3.tar.gz` & `tmp/sole_bili_get-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sole_bili_get-0.0.3.tar", last modified: Sun May 19 14:55:54 2024, max compression
+gzip compressed data, was "sole_bili_get-0.0.4.tar", last modified: Fri May 24 13:49:26 2024, max compression
```

## Comparing `sole_bili_get-0.0.3.tar` & `sole_bili_get-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 14:55:54.622053 sole_bili_get-0.0.3/
--rw-rw-rw-   0        0        0     1072 2024-05-18 14:01:48.000000 sole_bili_get-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     6801 2024-05-19 14:55:54.622053 sole_bili_get-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6287 2024-05-19 14:54:23.000000 sole_bili_get-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 14:55:54.622053 sole_bili_get-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1366 2024-05-18 14:42:06.000000 sole_bili_get-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 14:55:54.616053 sole_bili_get-0.0.3/sole_bili_get/
--rw-rw-rw-   0        0        0       76 2024-05-19 06:00:13.000000 sole_bili_get-0.0.3/sole_bili_get/__init__.py
--rw-rw-rw-   0        0        0    40049 2024-05-19 14:05:48.000000 sole_bili_get-0.0.3/sole_bili_get/bili_get.py
--rw-rw-rw-   0        0        0    10497 2024-05-19 12:42:50.000000 sole_bili_get-0.0.3/sole_bili_get/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 14:55:54.621053 sole_bili_get-0.0.3/sole_bili_get.egg-info/
--rw-rw-rw-   0        0        0     6801 2024-05-19 14:55:54.000000 sole_bili_get-0.0.3/sole_bili_get.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-19 14:55:54.000000 sole_bili_get-0.0.3/sole_bili_get.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 14:55:54.000000 sole_bili_get-0.0.3/sole_bili_get.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-19 14:55:54.000000 sole_bili_get-0.0.3/sole_bili_get.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-19 14:55:54.000000 sole_bili_get-0.0.3/sole_bili_get.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-19 14:55:54.000000 sole_bili_get-0.0.3/sole_bili_get.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 13:49:26.384427 sole_bili_get-0.0.4/
+-rw-rw-rw-   0        0        0     1072 2024-05-18 14:01:48.000000 sole_bili_get-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     6801 2024-05-24 13:49:26.383427 sole_bili_get-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6287 2024-05-19 14:54:23.000000 sole_bili_get-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:49:26.384427 sole_bili_get-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2024-05-18 14:42:06.000000 sole_bili_get-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:49:26.377428 sole_bili_get-0.0.4/sole_bili_get/
+-rw-rw-rw-   0        0        0       76 2024-05-21 12:04:46.000000 sole_bili_get-0.0.4/sole_bili_get/__init__.py
+-rw-rw-rw-   0        0        0    41224 2024-05-21 12:21:41.000000 sole_bili_get-0.0.4/sole_bili_get/bili_get.py
+-rw-rw-rw-   0        0        0    10620 2024-05-24 13:47:27.000000 sole_bili_get-0.0.4/sole_bili_get/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:49:26.383427 sole_bili_get-0.0.4/sole_bili_get.egg-info/
+-rw-rw-rw-   0        0        0     6801 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/top_level.txt
```

### Comparing `sole_bili_get-0.0.3/LICENSE.txt` & `sole_bili_get-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sole_bili_get-0.0.3/PKG-INFO` & `sole_bili_get-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sole_bili_get
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple tool to download videos from bilibili{*≧∀≦}
 Home-page: https://github.com/muggledy/bili-get
 Author: muggledy
 Author-email: zgjsycfndy2015@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.3 Summary: A simple tool
+Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.4 Summary: A simple tool
 to download videos from bilibili{*â§ââ¦} Home-page: https://github.com/
 muggledy/bili-get Author: muggledy Author-email: zgjsycfndy2015@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: requests # Bilibiliè§é¢ä¸è½½å¨ ![](https://
 img.shields.io/badge/python-3.6+-green) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/
```

### Comparing `sole_bili_get-0.0.3/README.md` & `sole_bili_get-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sole_bili_get-0.0.3/setup.py` & `sole_bili_get-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `sole_bili_get-0.0.3/sole_bili_get/bili_get.py` & `sole_bili_get-0.0.4/sole_bili_get/bili_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,32 +64,28 @@
                               f"downloaded but videos/audios not merged, merge {'them' if len(not_merged_p_list) > 1 else 'it'} firstly")
                     updated_local_playlists_info = self.check_playlists_is_merged(playlists_info=__local_playlists_info)
                     if updated_local_playlists_info is not None:
                         __local_playlists_info = updated_local_playlists_info
         self.playlists_info = deepcopy(__local_playlists_info)
         if self.get_origin_url_and_analyse() is None: #对尚未下载完成的剧集页面进行获取并得到音视频下载地址等相关信息更新到self.playlists_info中
             return
-        if not self.__all_downloed_flag:
-            self.save_playlists_info_into_local()
-            if not self.__download_at_once:
-                self.__all_downloed_flag = True #先预设能够全部下载成功，如果有一个失败了，则再置为False
-        else:
-            if self.auto_merge:
-                if not self.__ffmpeg_exist:
-                    self.logger.warning(ffmpeg_not_exist_prompt)
-                    if self.disable_console_log: print(f'Note: {ffmpeg_not_exist_prompt}')
-                else: self.check_playlists_is_merged()
-            return
-        self.download_by_playlists_info()
+        if not self.__download_at_once:
+            self.__all_downloed_flag = True #先预设能够全部下载成功，如果有一个失败了，则再置为False
+            self.download_by_playlists_info()
+        total, downloaded, not_download, download_failed, merged, not_merge, merge_failed = self.get_current_downloaded_info()
+        self.logger.info(f"total:{total}, downloaded:{downloaded}, not_download:{not_download}, download_failed:{download_failed}, "
+                         f"merged:{merged}, not_merge:{not_merge}, merge_failed:{merge_failed}")
         if self.__all_downloed_flag:
-            self.logger.info(f'(all) videos has already been downloaded in {self.__output_dir}!')
+            if total == downloaded:
+                self.logger.info(f'(all) videos has already been downloaded in {self.__output_dir}!')
         else:
+            self.save_playlists_info_into_local()
             self.logger.info('some videos/audios download failed, you can re-exec command to download them')
         if self.auto_merge:
-            if not self.__ffmpeg_exist:
+            if not self.__ffmpeg_exist and downloaded != 0:
                 self.logger.warning(ffmpeg_not_exist_prompt)
                 if self.disable_console_log:
                     print(f'Note: {ffmpeg_not_exist_prompt}')
             else:
                 self.check_playlists_is_merged()
 
     def update_newest_playlists_info(self, playlists_info): #上次虽然没有下载完，但可能已经下载了视频，只是音频还没有，这些信息不能被丢弃，否则会造成重复下载
@@ -100,14 +96,30 @@
             playlists_info[i]['merge_flag'] = self.playlists_info[i]['merge_flag']
             if self.playlists_info[i].get('video_save_path'):
                 playlists_info[i]['video_save_path'] = self.playlists_info[i]['video_save_path']
             if self.playlists_info[i].get('audio_save_path'):
                 playlists_info[i]['audio_save_path'] = self.playlists_info[i]['audio_save_path']
         self.playlists_info.update(playlists_info)
 
+    def get_current_downloaded_info(self): #返回：(剧集总数,已下载,未下载,下载失败,已合入,未合入,合入失败)
+        if not self.playlists_info:
+            return (0,0,0,0,0,0,0)
+        current_info = sorted([(p_num, info['download_flag'], info['merge_flag']) for p_num, info in self.playlists_info.items()], key=lambda x:x[0])
+        total = self.playlists_info[current_info[0][0]]['videos']
+        downloaded = len([info for info in current_info if info[1] == 3])
+        not_download = total - len(current_info)
+        download_failed = len(current_info) - downloaded
+        if self.__ffmpeg_exist:
+            merged = len([info for info in current_info if info[2]])
+            not_merge = not_download
+            merge_failed = len(current_info) - merged
+        else:
+            merged, not_merge, merge_failed = 0, total, 0
+        return (total, downloaded, not_download, download_failed, merged, not_merge, merge_failed)
+
     @property
     def origin_url(self):
         return self.__origin_url
 
     @origin_url.setter
     def origin_url(self, origin_url):
         if hasattr(self, f'_{self.__class__.__name__}__origin_url') \
@@ -304,16 +316,16 @@
             info = self.playlists_info[p]
             available_qualities = list(info['video_info'].keys())
             best_quality_idx = sorted([(i,abs(q-self.__quality_id)) 
                                        for i,q in enumerate(available_qualities)], key=lambda x:x[1])[0][0]
             best_quality = available_qualities[best_quality_idx]
             get_video_url_already_succeed = 0
             if self.danmu_urls.get(p):
-                if self.download_danmu_xml(self.danmu_urls[p], save_path=os.path.join(self.__output_dir, f"{info['title']}.xml")):
-                    danmu_ok_prompt = f"p{p} danmu xml file is downloaded into "+os.path.join(self.__output_dir, f"{info['title']}.xml")
+                if self.download_danmu_xml(self.danmu_urls[p], save_path=os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}.xml"))):
+                    danmu_ok_prompt = f"p{p} danmu xml file is downloaded into "+os.path.normpath(os.path.join(os.path.join(self.__output_dir, f"{info['title']}.xml")))
                     self.logger.info(danmu_ok_prompt+f" from {self.danmu_urls[p]}")
                     if self.disable_console_log: print(danmu_ok_prompt)
                     self.playlists_info[p]['danmu_url'] = self.danmu_urls[p]
             if self.playlists_info[p]['download_flag'] != 1:
                 for url,codec_info in sorted(info['video_info'][best_quality]['urls'], 
                                              key=lambda x:get_idx_of_specific_codedc(x[1])):
                     #if not [_c for _c in download_specific_codec_video if codec_info.lower().startswith(_c.lower())]:
@@ -321,16 +333,16 @@
                     downloading_video_info = f"start to download p{p}(video:{info['video_info'][best_quality]['quality']},"\
                         f"{'x'.join([str(_) for _ in info['video_info'][best_quality]['size']])},{codec_info})"\
                         f"{' from '+info['url'] if self.disable_console_log else ''}..."
                     self.logger.info(downloading_video_info)
                     if self.disable_console_log:
                         print(downloading_video_info)
                     self.__crawler.url = url
-                    self.__crawler.save_path = os.path.join(self.__output_dir, 
-                        f"{info['title']}{'' if (0 == get_video_url_already_succeed) else '_'+str(get_video_url_already_succeed)}.mp4")
+                    self.__crawler.save_path = os.path.normpath(os.path.join(self.__output_dir, 
+                        f"{info['title']}{'' if (0 == get_video_url_already_succeed) else '_'+str(get_video_url_already_succeed)}.mp4"))
                     if self.force_re_download and os.path.exists(self.__crawler.save_path):
                         self.logger.warning(f'delete old p{p} video file {self.__crawler.save_path} for force_re_download')
                         os.remove(self.__crawler.save_path)
                     start_time = time.time()
                     ok = self.__crawler.get()
                     if ok:
                         get_video_url_already_succeed += 1
@@ -349,29 +361,30 @@
                 self.logger.info(f"p{p} video has been downloaded in {self.__output_dir}")
             if self.playlists_info[p]['download_flag'] == 0:
                 continue
             self.logger.info(f"start to download p{p}(audio)...")
             if self.disable_console_log:
                 print(f"start to download p{p}(audio)...")
             self.__crawler.url = info['audio_url']
-            self.__crawler.save_path = os.path.join(self.__output_dir, f"{info['title']}_audio.mp3") #audio may also be *.mp4 file which is the same with video filename
-                                                                                            #in this case, we rename it to *.mp3
+            self.__crawler.save_path = os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}_audio.mp3")) #audio may also be *.mp4 file 
+                                                        #which is the same with video filename in this case, we rename it to *.mp3
             if self.force_re_download and os.path.exists(self.__crawler.save_path):
                 self.logger.warning(f'delete old p{p} audio file {self.__crawler.save_path} for force_re_download')
                 os.remove(self.__crawler.save_path)
             start_time = time.time()
             ok = self.__crawler.get()
             if ok:
                 self.logger.info(f"download audio from {self.__crawler.url} into {self.__crawler.save_path} succeed, runtime: {time.time()-start_time:.2f}s")
                 if os.path.exists(self.__crawler.save_path):
                     if self.playlists_info[p].get('video_save_path') and \
-                        (self.playlists_info[p]['video_save_path'] == os.path.join(self.__output_dir, f"{info['title']}{os.path.splitext(self.__crawler.save_path)[1]}")):
-                        self.playlists_info[p]['audio_save_path'] = os.path.join(self.__output_dir, f"{info['title']}.mp3")
+                            (self.playlists_info[p]['video_save_path'] == \
+                            os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}{os.path.splitext(self.__crawler.save_path)[1]}"))):
+                        self.playlists_info[p]['audio_save_path'] = os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}.mp3"))
                     else:
-                        self.playlists_info[p]['audio_save_path'] = os.path.join(self.__output_dir, f"{info['title']}{os.path.splitext(self.__crawler.save_path)[1]}")
+                        self.playlists_info[p]['audio_save_path'] = os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}{os.path.splitext(self.__crawler.save_path)[1]}"))
                     self.logger.warning(f'rename audio file {self.__crawler.save_path} => {self.playlists_info[p]["audio_save_path"]}')
                     if os.path.exists(self.playlists_info[p]['audio_save_path']):
                         os.remove(self.playlists_info[p]['audio_save_path'])
                     os.rename(self.__crawler.save_path, self.playlists_info[p]['audio_save_path'])
                 self.playlists_info[p]['download_flag'] += 2
                 self.save_playlists_info_into_local() #立即保存下载进度，避免因合成失败导致下次还要重复下载音频文件
                 if self.auto_merge and (not self.playlists_info[p]['merge_flag']) \
@@ -597,15 +610,15 @@
         if not os.path.isdir(output):
             os.makedirs(output)
     if args.cookie:
         cookies = parse_cookies(args.cookie)
     else:
         cookies = None
     if args.debug:
-        print(f"params: url({url}), quality({args.quality}), cookie({str(cookies)}), "
+        print(f"input params: url({url}), quality({args.quality}), cookie({str(cookies)}), "
               f"output({output}), download_playlist({args.playlist}), force_download({args.force}), not_merge({args.nomerge})")
     else:
         print(f'output: {output}')
     bilibili = Bilibili(url, disable_console_log=False if args.debug else True, 
         fetch_playlists=args.playlist, quality=args.quality, force_re_download=args.force, base_dir=output, 
         auto_merge=True if not args.nomerge else False, ffmpeg_debug=True if args.debug else False, 
         remove_merge_materials=True, debug_all=args.debug, headers={}, cookies=cookies)
```

### Comparing `sole_bili_get-0.0.3/sole_bili_get/utils.py` & `sole_bili_get-0.0.4/sole_bili_get/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import os, re, requests, hashlib, pickle
+import os, re, requests, hashlib, pickle, platform
 from contextlib import closing
 
 __all__ = ["get_absolute_path", "find_json_dict_from_text", "Crawler", "parse_cookies"]
 
 _utils_debug = False
 _base_dir = os.path.dirname(__file__)
 
 def get_absolute_path(relative_path):
     absolute_path = \
         os.path.normpath(os.path.join(\
         _base_dir, relative_path))
     absolute_path += \
-        ('' if os.path.split(relative_path)[1] else '\\')
-    parent_dir = os.path.dirname(absolute_path)
+        ('' if os.path.split(relative_path)[1] else 
+        ('\\' if platform.system() == 'Windows' else '/'))
+    parent_dir = os.path.dirname(absolute_path) #os.path.dirname('c:\\xxx\\yyy\\') returns "c:\\xxx\\yyy"
     if not os.path.exists(parent_dir):
         if _utils_debug: print(f'create directory: {parent_dir}')
         os.makedirs(parent_dir)
     return absolute_path
 
 def find_json_dict_from_text(text, start_str=None, num=float('inf')):
     stack = []
```

### Comparing `sole_bili_get-0.0.3/sole_bili_get.egg-info/PKG-INFO` & `sole_bili_get-0.0.4/sole_bili_get.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sole_bili_get
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple tool to download videos from bilibili{*≧∀≦}
 Home-page: https://github.com/muggledy/bili-get
 Author: muggledy
 Author-email: zgjsycfndy2015@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.3 Summary: A simple tool
+Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.4 Summary: A simple tool
 to download videos from bilibili{*â§ââ¦} Home-page: https://github.com/
 muggledy/bili-get Author: muggledy Author-email: zgjsycfndy2015@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: requests # Bilibiliè§é¢ä¸è½½å¨ ![](https://
 img.shields.io/badge/python-3.6+-green) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/
```

