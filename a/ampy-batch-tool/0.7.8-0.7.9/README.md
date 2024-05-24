# Comparing `tmp/ampy-batch-tool-0.7.8.tar.gz` & `tmp/ampy-batch-tool-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ampy-batch-tool-0.7.8.tar", last modified: Tue Jan 11 04:41:07 2022, max compression
+gzip compressed data, was "dist\ampy-batch-tool-0.7.9.tar", last modified: Wed Jan 19 08:35:25 2022, max compression
```

## Comparing `ampy-batch-tool-0.7.8.tar` & `ampy-batch-tool-0.7.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-01-11 04:41:07.453482 ampy-batch-tool-0.7.8/
--rw-rw-rw-   0        0        0     1086 2021-08-03 15:01:49.000000 ampy-batch-tool-0.7.8/LICENSE
--rw-rw-rw-   0        0        0    12452 2022-01-11 04:41:07.447479 ampy-batch-tool-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0    11933 2022-01-11 04:40:32.000000 ampy-batch-tool-0.7.8/README.md
-drwxrwxrwx   0        0        0        0 2022-01-11 04:41:07.373479 ampy-batch-tool-0.7.8/ab/
--rw-rw-rw-   0        0        0      302 2022-01-11 04:38:14.000000 ampy-batch-tool-0.7.8/ab/__init__.py
--rw-rw-rw-   0        0        0     7228 2021-12-10 13:52:34.000000 ampy-batch-tool-0.7.8/ab/__main__.py
--rw-rw-rw-   0        0        0     2794 2022-01-11 04:35:05.000000 ampy-batch-tool-0.7.8/ab/flash.py
--rw-rw-rw-   0        0        0    27950 2021-12-09 13:31:49.000000 ampy-batch-tool-0.7.8/ab/miniterm.py
--rw-rw-rw-   0        0        0    26935 2021-08-08 08:48:24.000000 ampy-batch-tool-0.7.8/ab/pyboard.py
-drwxrwxrwx   0        0        0        0 2022-01-11 04:41:07.444476 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/
--rw-rw-rw-   0        0        0    12452 2022-01-11 04:41:06.000000 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2022-01-11 04:41:06.000000 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-11 04:41:06.000000 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-01-11 04:41:06.000000 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-01-11 04:41:06.000000 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2022-01-11 04:41:06.000000 ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-11 04:41:07.454480 ampy-batch-tool-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1086 2022-01-11 04:36:24.000000 ampy-batch-tool-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-19 08:35:25.871544 ampy-batch-tool-0.7.9/
+-rw-rw-rw-   0        0        0     1086 2021-08-03 15:01:49.000000 ampy-batch-tool-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0    12494 2022-01-19 08:35:25.870542 ampy-batch-tool-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11975 2022-01-19 08:33:40.000000 ampy-batch-tool-0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-19 08:35:25.738541 ampy-batch-tool-0.7.9/ab/
+-rw-rw-rw-   0        0        0      302 2022-01-19 08:33:09.000000 ampy-batch-tool-0.7.9/ab/__init__.py
+-rw-rw-rw-   0        0        0     7229 2022-01-19 08:33:46.000000 ampy-batch-tool-0.7.9/ab/__main__.py
+-rw-rw-rw-   0        0        0     2794 2022-01-11 04:35:05.000000 ampy-batch-tool-0.7.9/ab/flash.py
+-rw-rw-rw-   0        0        0    27950 2022-01-17 15:15:16.000000 ampy-batch-tool-0.7.9/ab/miniterm.py
+-rw-rw-rw-   0        0        0    26935 2021-08-08 08:48:24.000000 ampy-batch-tool-0.7.9/ab/pyboard.py
+drwxrwxrwx   0        0        0        0 2022-01-19 08:35:25.867540 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/
+-rw-rw-rw-   0        0        0    12494 2022-01-19 08:35:25.000000 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2022-01-19 08:35:25.000000 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-19 08:35:25.000000 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2022-01-19 08:35:25.000000 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2022-01-19 08:35:25.000000 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2022-01-19 08:35:25.000000 ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-19 08:35:25.873547 ampy-batch-tool-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2022-01-11 04:36:24.000000 ampy-batch-tool-0.7.9/setup.py
```

### Comparing `ampy-batch-tool-0.7.8/LICENSE` & `ampy-batch-tool-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ampy-batch-tool-0.7.8/PKG-INFO` & `ampy-batch-tool-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampy-batch-tool
-Version: 0.7.8
+Version: 0.7.9
 Summary: An adafruit-ampy batch tool
 Home-page: https://gitee.com/walkline/a-batch-tool
 Author: Walkline Wang
 Author-email: walkline@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -310,14 +310,15 @@
 2. 偶尔出现无法进入`raw_repl`模式的问题，重新运行一次即可解决
 3. 偶尔出现`repl`模式下无法输入的问题，重启开发板即可解决
 4. `repl`模式下上传文件也许会出现文件不完整的问题，尝试重新上传可以解决
 5. 使用烧录固件功能时如果提示类似找不到`esptool`的信息，卸载后重新安装一次即可
 
 ### 更新记录
 
+* `v0.7.9`：修复串口号过滤错误
 * `v0.7.8`：修复串口号过滤错误，增加对`esptool`工具的版本要求
 * `v0.7.7`：烧录固件工具串口列表过滤掉`COM1`
 * `v0.7.6`：修复串口列表过滤逻辑错误
 * `v0.7.5`：一键删除`main.py`文件后执行硬重启，串口列表过滤掉`COM1`
 * `v0.7.4`：`repl`模式使用回车键选择第一个端口
 * `v0.7.3`：修复`v0.7.2`的 bug，无语。。。。
 * `v0.7.2`：修改运行`esptool.py`为`esptool`。。。。
```

### Comparing `ampy-batch-tool-0.7.8/README.md` & `ampy-batch-tool-0.7.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,15 @@
 2. 偶尔出现无法进入`raw_repl`模式的问题，重新运行一次即可解决
 3. 偶尔出现`repl`模式下无法输入的问题，重启开发板即可解决
 4. `repl`模式下上传文件也许会出现文件不完整的问题，尝试重新上传可以解决
 5. 使用烧录固件功能时如果提示类似找不到`esptool`的信息，卸载后重新安装一次即可
 
 ### 更新记录
 
+* `v0.7.9`：修复串口号过滤错误
 * `v0.7.8`：修复串口号过滤错误，增加对`esptool`工具的版本要求
 * `v0.7.7`：烧录固件工具串口列表过滤掉`COM1`
 * `v0.7.6`：修复串口列表过滤逻辑错误
 * `v0.7.5`：一键删除`main.py`文件后执行硬重启，串口列表过滤掉`COM1`
 * `v0.7.4`：`repl`模式使用回车键选择第一个端口
 * `v0.7.3`：修复`v0.7.2`的 bug，无语。。。。
 * `v0.7.2`：修改运行`esptool.py`为`esptool`。。。。
```

### Comparing `ampy-batch-tool-0.7.8/ab/__main__.py` & `ampy-batch-tool-0.7.9/ab/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 	return file_list, dir_list, bad_list
 
 def choose_a_port():
 	port_list = []
 
 	for port in comports():
-		if not str(port).startswith('COM1'):
+		if not str(port).startswith('COM1 '):
 			port_list.append(str(port))
 
 	if len(port_list) == 0:
 		print('No serial port found')
 		exit()
 
 	print('Port List:')
```

### Comparing `ampy-batch-tool-0.7.8/ab/flash.py` & `ampy-batch-tool-0.7.9/ab/flash.py`

 * *Files identical despite different names*

### Comparing `ampy-batch-tool-0.7.8/ab/miniterm.py` & `ampy-batch-tool-0.7.9/ab/miniterm.py`

 * *Files identical despite different names*

### Comparing `ampy-batch-tool-0.7.8/ab/pyboard.py` & `ampy-batch-tool-0.7.9/ab/pyboard.py`

 * *Files identical despite different names*

### Comparing `ampy-batch-tool-0.7.8/ampy_batch_tool.egg-info/PKG-INFO` & `ampy-batch-tool-0.7.9/ampy_batch_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampy-batch-tool
-Version: 0.7.8
+Version: 0.7.9
 Summary: An adafruit-ampy batch tool
 Home-page: https://gitee.com/walkline/a-batch-tool
 Author: Walkline Wang
 Author-email: walkline@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -310,14 +310,15 @@
 2. 偶尔出现无法进入`raw_repl`模式的问题，重新运行一次即可解决
 3. 偶尔出现`repl`模式下无法输入的问题，重启开发板即可解决
 4. `repl`模式下上传文件也许会出现文件不完整的问题，尝试重新上传可以解决
 5. 使用烧录固件功能时如果提示类似找不到`esptool`的信息，卸载后重新安装一次即可
 
 ### 更新记录
 
+* `v0.7.9`：修复串口号过滤错误
 * `v0.7.8`：修复串口号过滤错误，增加对`esptool`工具的版本要求
 * `v0.7.7`：烧录固件工具串口列表过滤掉`COM1`
 * `v0.7.6`：修复串口列表过滤逻辑错误
 * `v0.7.5`：一键删除`main.py`文件后执行硬重启，串口列表过滤掉`COM1`
 * `v0.7.4`：`repl`模式使用回车键选择第一个端口
 * `v0.7.3`：修复`v0.7.2`的 bug，无语。。。。
 * `v0.7.2`：修改运行`esptool.py`为`esptool`。。。。
```

### Comparing `ampy-batch-tool-0.7.8/setup.py` & `ampy-batch-tool-0.7.9/setup.py`

 * *Files identical despite different names*

