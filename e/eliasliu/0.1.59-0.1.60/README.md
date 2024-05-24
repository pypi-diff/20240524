# Comparing `tmp/eliasliu-0.1.59.tar.gz` & `tmp/eliasliu-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.59.tar", last modified: Thu May 23 03:00:09 2024, max compression
+gzip compressed data, was "eliasliu-0.1.60.tar", last modified: Fri May 24 09:12:32 2024, max compression
```

## Comparing `eliasliu-0.1.59.tar` & `eliasliu-0.1.60.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.879831 eliasliu-0.1.59/
--rw-rw-rw-   0        0        0     7058 2024-05-23 03:00:09.879831 eliasliu-0.1.59/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.59/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.684262 eliasliu-0.1.59/elias/
-drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.791237 eliasliu-0.1.59/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/__init__.py
--rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.59/elias/ai.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.863881 eliasliu-0.1.59/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/picture.py
--rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.59/elias/text_similarity.py
--rw-rw-rw-   0        0        0    79330 2024-05-20 08:28:30.000000 eliasliu-0.1.59/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.878832 eliasliu-0.1.59/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7058 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 03:00:09.880832 eliasliu-0.1.59/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-23 02:59:59.000000 eliasliu-0.1.59/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:12:32.101641 eliasliu-0.1.60/
+-rw-rw-rw-   0        0        0     7058 2024-05-24 09:12:32.100642 eliasliu-0.1.60/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.60/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:12:31.827056 eliasliu-0.1.60/elias/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:12:31.930886 eliasliu-0.1.60/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.60/elias/ai.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:12:32.079650 eliasliu-0.1.60/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/etl.py
+-rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/picture.py
+-rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.60/elias/text_similarity.py
+-rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.60/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:12:32.099642 eliasliu-0.1.60/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7058 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:12:32.102643 eliasliu-0.1.60/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-24 08:58:12.000000 eliasliu-0.1.60/setup.py
```

### Comparing `eliasliu-0.1.59/PKG-INFO` & `eliasliu-0.1.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.59
+Version: 0.1.60
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.59/README.md` & `eliasliu-0.1.60/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.60/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/douyin.py` & `eliasliu-0.1.60/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/jd.py` & `eliasliu-0.1.60/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/name_in_db.py` & `eliasliu-0.1.60/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.60/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.60/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/Scripts/youdao.py` & `eliasliu-0.1.60/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/ai.py` & `eliasliu-0.1.60/elias/ai.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/check.py` & `eliasliu-0.1.60/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/config_env_variable.py` & `eliasliu-0.1.60/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datamove.py` & `eliasliu-0.1.60/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datax/auto_create_table.py` & `eliasliu-0.1.60/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datax/job.py` & `eliasliu-0.1.60/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datax/main.py` & `eliasliu-0.1.60/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datax/reader.py` & `eliasliu-0.1.60/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datax/run.py` & `eliasliu-0.1.60/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/datax/writer.py` & `eliasliu-0.1.60/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/etl.py` & `eliasliu-0.1.60/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/picture.py` & `eliasliu-0.1.60/elias/picture.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/text_similarity.py` & `eliasliu-0.1.60/elias/text_similarity.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/elias/usual.py` & `eliasliu-0.1.60/elias/usual.py`

 * *Files 3% similar despite different names*

```diff
@@ -2187,14 +2187,16 @@
         else:
             pass
         
         
         logger.add(file, rotation="500 MB", retention="10 days", level="DEBUG")
         return logger
 
+
+# 将JSON数据写入到指定的JSON文件中。
 def write_json_to_file(data, file_path):
     """
     将JSON数据写入到指定的JSON文件中。
 
     参数：
     data: dict
         要写入文件的JSON数据，必须是一个字典。
@@ -2222,14 +2224,15 @@
         json.dump(data, json_file, indent=4)  # 设置indent参数为4，表示使用4个空格缩进
 
     print("JSON数据已写入文件：", file_path)
    
     return file_path
 
 
+# 将html转化成markdown
 def convert_html_to_markdown(html_content):
     
     import html2text
     import re
     # 在转换前预处理HTML，例如插入额外的空行
     html_content = re.sub(r'</p>', r'</p>\n\n', html_content)  # 在每个段落后增加额外的空行
 
@@ -2242,14 +2245,15 @@
 
     # 在转换后处理Markdown，例如确保加粗不会在中间断开
     markdown_content = re.sub(r'\*\*(.*?)\*\*', lambda match: '**' + match.group(1).replace('\n', ' ') + '**', markdown_content)
     
     return markdown_content
 
 
+# 将两个列表均匀插入到一个列表
 def interleave_lists(list1, list2):
     '''
     两个列表均匀插入到一个列表
 
     Parameters
     ----------
     list1 : list
@@ -2300,8 +2304,60 @@
         result.append(element)
         # 更新index
         index += step
     
     # 添加剩余的list1元素
     result.extend(list1[index:])
     
-    return result
+    return result
+
+
+# 创建文件夹，如果存在就不创建
+def create_dir_if_not_exists(dir_path):
+    import os
+    if not os.path.exists(dir_path):
+        os.makedirs(dir_path)
+        return True
+    return False
+
+# 下载文件
+def download_file(url, save_path):
+    """
+    Download a file from the given URL and save it to the specified path.
+    
+    # Example usage:
+    image_url = "https://example.com/image.jpg"
+    video_url = "https://example.com/video.mp4"
+    image_save_path = "image.jpg"
+    video_save_path = "video.mp4"
+    
+    # Download image
+    download_file(image_url, image_save_path)
+    
+    # Download video
+    download_file(video_url, video_save_path)
+    
+    Args:
+        url (str): The URL of the file to download.
+        save_path (str): The path where the downloaded file will be saved.
+    """
+    
+    import requests
+    try:
+        # Send a GET request to the URL to fetch the file
+        response = requests.get(url)
+        response.raise_for_status()  # Raise an exception for bad status codes
+        
+        # Write the content to a local file
+        with open(save_path, 'wb') as f:
+            f.write(response.content)
+        
+        print(f"File downloaded successfully to: {save_path}")
+    except requests.exceptions.RequestException as e:
+        # Handle exceptions related to network or request errors
+        print(f"Error downloading file from {url}: {e}")
+    except IOError as e:
+        # Handle exceptions related to file I/O errors
+        print(f"Error saving file to {save_path}: {e}")
+
+
+
```

### Comparing `eliasliu-0.1.59/elias/wechat.py` & `eliasliu-0.1.60/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.60/eliasliu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.59
+Version: 0.1.60
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.59/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.60/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.59/setup.py` & `eliasliu-0.1.60/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.59',  # 版本号
+    version='0.1.60',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
```

