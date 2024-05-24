# Comparing `tmp/automvs-0.1.0.tar.gz` & `tmp/automvs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.1.0.tar", last modified: Thu May 16 21:59:00 2024, max compression
+gzip compressed data, was "automvs-0.2.0.tar", last modified: Fri May 24 00:37:50 2024, max compression
```

## Comparing `automvs-0.1.0.tar` & `automvs-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-16 21:59:00.943869 automvs-0.1.0/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.1.0/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     2316 2024-05-16 21:59:00.943869 automvs-0.1.0/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     1842 2024-05-11 03:46:35.000000 automvs-0.1.0/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-16 21:59:00.943869 automvs-0.1.0/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    49993 2024-05-16 21:56:44.000000 automvs-0.1.0/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-16 21:59:00.943869 automvs-0.1.0/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     2316 2024-05-16 21:59:00.000000 automvs-0.1.0/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-16 21:59:00.000000 automvs-0.1.0/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-16 21:59:00.000000 automvs-0.1.0/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-16 21:59:00.000000 automvs-0.1.0/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-16 21:59:00.943869 automvs-0.1.0/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-16 21:58:03.000000 automvs-0.1.0/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-24 00:37:50.352704 automvs-0.2.0/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.2.0/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     3677 2024-05-24 00:37:50.352704 automvs-0.2.0/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3203 2024-05-23 21:46:04.000000 automvs-0.2.0/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-24 00:37:50.352704 automvs-0.2.0/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    50778 2024-05-24 00:37:08.000000 automvs-0.2.0/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-24 00:37:50.352704 automvs-0.2.0/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     3677 2024-05-24 00:37:50.000000 automvs-0.2.0/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-24 00:37:50.000000 automvs-0.2.0/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-24 00:37:50.000000 automvs-0.2.0/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-24 00:37:50.000000 automvs-0.2.0/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-24 00:37:50.352704 automvs-0.2.0/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-24 00:37:09.000000 automvs-0.2.0/setup.py
```

### Comparing `automvs-0.1.0/LICENSE` & `automvs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.1.0/PKG-INFO` & `automvs-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -71,9 +71,59 @@
     build.check_maxcc("UPLOAD")
     build.send_herc('devinit 170 tape/zdlib1.het')
     build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
     build.send_reply('170')
     build.send_oper("$DU")
 finally:
     if mvs_type == 'MVSCE'
+        build.quit_hercules()
+```
+
+## Remote Automation
+
+This library also supports remote automation through the use of a rexx script
+available at https://github.com/MVS-sysgen/automvs/tree/main/REXX. Example usage
+of that script:
+
+
+```python
+
+import sys
+from automvs import automation
+
+if len(sys.argv) != 2:
+    print("Usage: python go_mvs.py <MVS system> username password")
+    print(" MVS system: one of MVSCE, TK4- or TK5\n MVS PATH: /path/to/the/system. E.g. /home/test/mvs/tk4-")
+    sys.exit(1)
+
+mvs_type = sys.argv[1]
+username = sys.argv[3]
+password = sys.argv[4]
+punch_port = 3505
+ip = '127.0.0.1'
+remote_port = 9856
+
+build = automation(
+                    system=mvs_type,
+                    ip = ip,
+                    punch_port = punch_port,
+                    username=username,
+                    password=password,
+                    remote_port = remote_port
+                  )
+
+cwd = os.getcwd()
+
+try:
+    print("Submitting {}/jcl/upload.jcl".format(cwd))
+    with open("{}/jcl/upload.jcl".format(cwd),"r") as jcl:
+        build.submit(jcl.read())
+    build.wait_for_job("UPLOAD")
+    build.check_maxcc("UPLOAD")
+    build.send_herc('devinit 170 tape/zdlib1.het')
+    build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
+    build.send_reply('170')
+    build.send_oper("$DU")
+finally:
+    if mvs_type == 'MVSCE'
         build.quit_hercules()
 ```
```

### Comparing `automvs-0.1.0/README.md` & `automvs-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -57,8 +57,58 @@
     build.send_herc('devinit 170 tape/zdlib1.het')
     build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
     build.send_reply('170')
     build.send_oper("$DU")
 finally:
     if mvs_type == 'MVSCE'
         build.quit_hercules()
+```
+
+## Remote Automation
+
+This library also supports remote automation through the use of a rexx script
+available at https://github.com/MVS-sysgen/automvs/tree/main/REXX. Example usage
+of that script:
+
+
+```python
+
+import sys
+from automvs import automation
+
+if len(sys.argv) != 2:
+    print("Usage: python go_mvs.py <MVS system> username password")
+    print(" MVS system: one of MVSCE, TK4- or TK5\n MVS PATH: /path/to/the/system. E.g. /home/test/mvs/tk4-")
+    sys.exit(1)
+
+mvs_type = sys.argv[1]
+username = sys.argv[3]
+password = sys.argv[4]
+punch_port = 3505
+ip = '127.0.0.1'
+remote_port = 9856
+
+build = automation(
+                    system=mvs_type,
+                    ip = ip,
+                    punch_port = punch_port,
+                    username=username,
+                    password=password,
+                    remote_port = remote_port
+                  )
+
+cwd = os.getcwd()
+
+try:
+    print("Submitting {}/jcl/upload.jcl".format(cwd))
+    with open("{}/jcl/upload.jcl".format(cwd),"r") as jcl:
+        build.submit(jcl.read())
+    build.wait_for_job("UPLOAD")
+    build.check_maxcc("UPLOAD")
+    build.send_herc('devinit 170 tape/zdlib1.het')
+    build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
+    build.send_reply('170')
+    build.send_oper("$DU")
+finally:
+    if mvs_type == 'MVSCE'
+        build.quit_hercules()
 ```
```

### Comparing `automvs-0.1.0/automvs/__init__.py` & `automvs-0.2.0/automvs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     fashion. This can be used for deploying XMI files, pushing out updates, 
     building software, creating custom MVS deployments.
 
     Using this library requires a hercules SDL and MVS/CE for MVS/CE and/or
     TK4-/TK5 for those MVS3.8j.
 """
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -43,14 +43,15 @@
 import time
 import subprocess
 import threading
 import queue
 import base64
 import select
 import socket
+import codecs
 from pathlib import Path
 import logging
 
 import http.client
 import urllib.parse
 
 TIMEOUT = 1800 # Global time out 30 minutes
@@ -771,15 +772,15 @@
             self.logger.debug(f"[AUTOMATION: {self.system}] Punchcard folder '{path}' does not exist")
             raise Exception("Punchcard folder '{}' does not exist".format(path))
         self.send_herc(command='detach d')
         self.send_herc(command='attach d 3525 {} ebcdic'.format(path))
 
     def read_log_lines(self):
         #self.logger.debug(f"reading {self.logfile}")
-        with open(self.logfile, "r") as file:
+        with open(self.logfile, "r",errors='ignore') as file:
             # Check if the last_size attribute exists in the instance
             if not hasattr(self, 'log_last_size'):
                 # If not, initialize it to 0
                 self.log_last_size = 0
             
             # Move the cursor to the last known position
             file.seek(self.log_last_size)
@@ -1029,21 +1030,21 @@
         self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Starting Automation")
         self.check_ports()
         self.connect()
 
     def connect(self):
         self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Connecting to {self.ip}:{self.port}")
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket.connect((self.ip, self.port))
+        self.socket.connect((self.ip, int(self.port)))
         
         self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Connection done")
 
         self.wait_for_socket('Please /LOGON to continue',timeout=5)
 
-        self.send_automvs(f"/LOGON {self.username} {self.password}")
+        self.send_automvs("/LOGON {user} {passw}".format(user=self.username,passw=self.__hash__(self.password)))
 
         self.wait_for_socket('LOGON OK',error_string='Logon Failed:')
         
 
 
     def wait_for_socket(self,end_string,start_string=False, error_string="Error:",timeout=False):
 
@@ -1062,14 +1063,17 @@
                 exception = f"Waiting for '{end_string}' timed out after {self.timeout} seconds"
                 print("[ERR] {}".format(exception))
                 raise Exception(exception)
             
             line = self.read_automvs(timeout=timeout)
             #self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] received {line}")
 
+            if '*JOBLOG*' in line:
+                continue
+
             if start_string and start_string in line:
                 continue
 
             if end_string in line:
                 break
             
             if error_string in line:
@@ -1085,44 +1089,57 @@
         
         if not timeout:
             timeout = self.timeout
 
         if not timeout:
             timeout = TIMEOUT
 
-        char = data = b""
+        data = b""
 
         try:
             self.socket.setblocking(0)  # Set non-blocking mode
-            data = ""
+            data = b""
             while True:
                 ready = select.select([self.socket], [], [], timeout)
                 if len(ready[0]) == 0:
                     raise TimeoutError("Receive timeout")
                 
-                byte = self.socket.recv(1).decode()
-                # if not byte:  # If no more data available, break the loop
-                #     break
-                if byte == "\n":
+                byte = self.socket.recv(1)
+                if byte == b"\n":
                     break
                 data += byte
                 
-            self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Received {len(data)} bytes: {data}")
-            return data
+            # self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Received {len(data)} bytes: {data.hex()}")
+            _d = data.decode(encoding="ascii", errors="ignore")
+            self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Received: {_d}")
+            
+            return data.decode(encoding="ascii", errors="ignore")
         except BlockingIOError:
             return ""
         finally:
             self.socket.setblocking(1) 
 
         # while char != b"\n":
         #     char = self.socket.recv(1)
         #     data = data + char
         # data = data.decode().strip()
 
         # return data
+
+    def __hash__(self,password):
+        # Convert the string to EBCDIC bytes
+        ebcdic_bytes = codecs.encode(password.upper(), 'cp037')
+        
+        # Calculate the hash using the EBCDIC bytes
+        hashCode = 0
+        for byte in ebcdic_bytes:
+            hashCode = (hashCode * 31 + byte) & (2**32 - 1)  # unsigned
+        if hashCode & 2**31:
+            hashCode -= 2**32  # make it signed
+        return hashCode
     
     def send_automvs(self,command):
         if not self.socket:
             self.connect()
         self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Sending: {command}")
         self.socket.sendall(command.encode('ascii'))
 
@@ -1175,18 +1192,22 @@
 
         self.wait_for_socket('--- DONE',timeout=timeout)
     
     def wait_for_string(self, string_to_waitfor, stderr=False, timeout=False):
         self.__remote_wait_for(string_to_waitfor,timeout=timeout)
     
     def wait_for_job(self, jobname, stderr=False, timeout=False,debug=False):
+        
+        if not timeout:
+            timeout = self.timeout
+
         if debug or self.loglevel == 'DEBUG':
-            self.__remote_wait_for(f"/JOB {jobname} DEBUG",timeout=timeout)
+            self.__remote_wait_for(f"/JOB {jobname} DEBUG TIMEOUT={timeout}",timeout=timeout)
         else:
-            self.__remote_wait_for(f"/JOB {jobname}",timeout=timeout)
+            self.__remote_wait_for(f"/JOB {jobname} TIMEOUT={timeout}",timeout=timeout)
     
     def check_maxcc(self, jobname, steps_cc={}, ignore=False, keep=False):
         self.logger.debug(f"[AUTOMATION: {self.ip}:{self.port}] Checking {jobname} job results")
 
         failed_step = False
         job_status = []
         log = None
@@ -1199,15 +1220,15 @@
 
         if len(lines) == 0:
             raise Exception('No results from job in log, check printer output for errors')
 
         logmsg = '[MAXCC] Jobname: {:<8} Procname: {:<8} Stepname: {:<8} Progname: {:<8} Exit Code: {:<8}'
         for line in lines:
             if len(line.split(',')) < 6:
-                raise Exception("Line from automvs too short: {line}")
+                raise Exception(f"Line from automvs too short: {line}")
             num, name, step, proc, prog, cc = line.split(',')
             self.current_job = {'jobnum': num, 'jobname': name}
             
             logmsg = '[MAXCC] Jobnum: {:<4} Jobname: {:<8} Procname: {:<8} Stepname: {:<8} Progname: {:<8} Exit Code: {:<8}'
 
             log = logmsg.format(num,name,proc,step,prog,cc)
             step_status = {
@@ -1215,15 +1236,15 @@
                             "jobname:" : name,
                             "procname": proc,
                             "stepname": step,
                             "progname": prog,
                             "exitcode": cc
                         }
             maxcc=cc
-            stepname = step
+            stepname = step.strip()
 
             self.logger.debug(log)
             job_status.append(step_status)
 
             if stepname in steps_cc:
                 expected_cc = steps_cc[stepname]
             else:
@@ -1293,15 +1314,15 @@
 
         if not port:
             port = self.punch_port 
 
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             # Connect to server and send data
-            sock.connect((self.ip, port))
+            sock.connect((self.ip, int(port)))
             if ebcdic:
               sock.send(jcl)
             else:
               sock.send(jcl.encode())
 
         finally:
             sock.close()
```

### Comparing `automvs-0.1.0/automvs.egg-info/PKG-INFO` & `automvs-0.2.0/automvs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -71,9 +71,59 @@
     build.check_maxcc("UPLOAD")
     build.send_herc('devinit 170 tape/zdlib1.het')
     build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
     build.send_reply('170')
     build.send_oper("$DU")
 finally:
     if mvs_type == 'MVSCE'
+        build.quit_hercules()
+```
+
+## Remote Automation
+
+This library also supports remote automation through the use of a rexx script
+available at https://github.com/MVS-sysgen/automvs/tree/main/REXX. Example usage
+of that script:
+
+
+```python
+
+import sys
+from automvs import automation
+
+if len(sys.argv) != 2:
+    print("Usage: python go_mvs.py <MVS system> username password")
+    print(" MVS system: one of MVSCE, TK4- or TK5\n MVS PATH: /path/to/the/system. E.g. /home/test/mvs/tk4-")
+    sys.exit(1)
+
+mvs_type = sys.argv[1]
+username = sys.argv[3]
+password = sys.argv[4]
+punch_port = 3505
+ip = '127.0.0.1'
+remote_port = 9856
+
+build = automation(
+                    system=mvs_type,
+                    ip = ip,
+                    punch_port = punch_port,
+                    username=username,
+                    password=password,
+                    remote_port = remote_port
+                  )
+
+cwd = os.getcwd()
+
+try:
+    print("Submitting {}/jcl/upload.jcl".format(cwd))
+    with open("{}/jcl/upload.jcl".format(cwd),"r") as jcl:
+        build.submit(jcl.read())
+    build.wait_for_job("UPLOAD")
+    build.check_maxcc("UPLOAD")
+    build.send_herc('devinit 170 tape/zdlib1.het')
+    build.wait_for_string("IEF238D SMP4P44 - REPLY DEVICE NAME OR 'CANCEL'.")
+    build.send_reply('170')
+    build.send_oper("$DU")
+finally:
+    if mvs_type == 'MVSCE'
         build.quit_hercules()
 ```
```

### Comparing `automvs-0.1.0/setup.py` & `automvs-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.1.0',    
+    version='0.2.0',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```

