# Comparing `tmp/UrsinaNetworking-2.1.4.tar.gz` & `tmp/UrsinaNetworking-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UrsinaNetworking-2.1.4.tar", last modified: Mon Sep 27 15:13:39 2021, max compression
+gzip compressed data, was "UrsinaNetworking-2.1.5.tar", last modified: Fri May 24 11:35:14 2024, max compression
```

## Comparing `UrsinaNetworking-2.1.4.tar` & `UrsinaNetworking-2.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-09-27 15:13:39.522038 UrsinaNetworking-2.1.4/
--rw-rw-rw-   0        0        0     1053 2021-09-18 15:56:52.000000 UrsinaNetworking-2.1.4/LICENSE
--rw-rw-rw-   0        0        0      326 2021-09-27 15:13:39.522038 UrsinaNetworking-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2824 2021-07-28 02:23:34.000000 UrsinaNetworking-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2021-09-27 15:13:39.473917 UrsinaNetworking-2.1.4/UrsinaNetworking.egg-info/
--rw-rw-rw-   0        0        0      326 2021-09-27 15:13:39.000000 UrsinaNetworking-2.1.4/UrsinaNetworking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2021-09-27 15:13:39.000000 UrsinaNetworking-2.1.4/UrsinaNetworking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-27 15:13:39.000000 UrsinaNetworking-2.1.4/UrsinaNetworking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-09-27 15:13:39.000000 UrsinaNetworking-2.1.4/UrsinaNetworking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-27 15:13:39.523042 UrsinaNetworking-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      452 2021-09-27 15:13:18.000000 UrsinaNetworking-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-27 15:13:39.487928 UrsinaNetworking-2.1.4/ursinanetworking/
--rw-rw-rw-   0        0        0       97 2021-09-18 15:56:12.000000 UrsinaNetworking-2.1.4/ursinanetworking/__init__.py
--rw-rw-rw-   0        0        0     7665 2021-07-28 02:23:34.000000 UrsinaNetworking-2.1.4/ursinanetworking/easyursinanetworking.py
--rw-rw-rw-   0        0        0     5930 2021-09-27 15:13:25.000000 UrsinaNetworking-2.1.4/ursinanetworking/replicated_2.py
--rw-rw-rw-   0        0        0      552 2021-07-28 02:23:34.000000 UrsinaNetworking-2.1.4/ursinanetworking/test_cl.py
--rw-rw-rw-   0        0        0      407 2021-07-28 02:23:34.000000 UrsinaNetworking-2.1.4/ursinanetworking/test_sv.py
--rw-rw-rw-   0        0        0    11998 2021-07-28 02:23:34.000000 UrsinaNetworking-2.1.4/ursinanetworking/ursinanetworking.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:35:14.535928 UrsinaNetworking-2.1.5/
+-rw-rw-rw-   0        0        0     1053 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0      340 2024-05-24 11:35:14.535928 UrsinaNetworking-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2827 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 11:35:14.529924 UrsinaNetworking-2.1.5/UrsinaNetworking.egg-info/
+-rw-rw-rw-   0        0        0      340 2024-05-24 11:35:14.000000 UrsinaNetworking-2.1.5/UrsinaNetworking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2024-05-24 11:35:14.000000 UrsinaNetworking-2.1.5/UrsinaNetworking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:35:14.000000 UrsinaNetworking-2.1.5/UrsinaNetworking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-24 11:35:14.000000 UrsinaNetworking-2.1.5/UrsinaNetworking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 11:35:14.536924 UrsinaNetworking-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-23 10:17:12.000000 UrsinaNetworking-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:35:14.534924 UrsinaNetworking-2.1.5/ursinanetworking/
+-rw-rw-rw-   0        0        0       97 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/ursinanetworking/__init__.py
+-rw-rw-rw-   0        0        0     7665 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/ursinanetworking/easyursinanetworking.py
+-rw-rw-rw-   0        0        0     5930 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/ursinanetworking/replicated_2.py
+-rw-rw-rw-   0        0        0      552 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/ursinanetworking/test_cl.py
+-rw-rw-rw-   0        0        0      407 2024-05-23 10:10:33.000000 UrsinaNetworking-2.1.5/ursinanetworking/test_sv.py
+-rw-rw-rw-   0        0        0    11996 2024-05-23 10:15:59.000000 UrsinaNetworking-2.1.5/ursinanetworking/ursinanetworking.py
```

### Comparing `UrsinaNetworking-2.1.4/LICENSE` & `UrsinaNetworking-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `UrsinaNetworking-2.1.4/README.md` & `UrsinaNetworking-2.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def onClientDisconnected(Client):
     print(f"{Client} disconnected !")
 ```
 
 ## Built-in Client Events
 ```python
 @Client.event
-def onConnectionEtablished():
+def onConnectionEstablished():
     print("I'm connected to the server !")
 
 @Client.event
 def onConnectionError(Reason):
     print(f"Error ! Reason : {Reason}")
 ```
 
@@ -129,8 +129,8 @@
 Client = UrsinaNetworkingClient("localhost", 25565)
 
 @Client.event
 def receiveFile(Content):
     f = open("receveid_image.png", "wb")
     f.write(ursina_networking_decompress_file(Content))
     f.close()
-```
+```
```

### Comparing `UrsinaNetworking-2.1.4/ursinanetworking/easyursinanetworking.py` & `UrsinaNetworking-2.1.5/ursinanetworking/easyursinanetworking.py`

 * *Files identical despite different names*

### Comparing `UrsinaNetworking-2.1.4/ursinanetworking/replicated_2.py` & `UrsinaNetworking-2.1.5/ursinanetworking/replicated_2.py`

 * *Files identical despite different names*

### Comparing `UrsinaNetworking-2.1.4/ursinanetworking/test_cl.py` & `UrsinaNetworking-2.1.5/ursinanetworking/test_cl.py`

 * *Files identical despite different names*

### Comparing `UrsinaNetworking-2.1.4/ursinanetworking/ursinanetworking.py` & `UrsinaNetworking-2.1.5/ursinanetworking/ursinanetworking.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,26 @@
  | |  | |_ __ ___ _ _ __   __ _|  \| | ___| |___      _____  _ __| | ___ _ __   __ _
  | |  | | '__/ __| | '_ \ / _` | . ` |/ _ \ __\ \ /\ / / _ \| '__| |/ / | '_ \ / _` |
  | |__| | |  \__ \ | | | | (_| | |\  |  __/ |_ \ V  V / (_) | |  |   <| | | | | (_| |
   \____/|_|  |___/_|_| |_|\__,_|_| \_|\___|\__| \_/\_/ \___/|_|  |_|\_\_|_| |_|\__, |
                                                                                 __/ |
                                                                                |___/
 By K3#4869 and Squiggle#1385
-
-Version 1.0.5
 """
 
 import socket
 import threading
 import pickle
 import zlib
-import traceback
 
 HEADERSIZE = 10
 MESSAGE_LENGTH = 8
 BUFFERSIZE = 4096
 
-BUILTIN_EVENT_CONNECTION_ETABLISHED = "onConnectionEtablished"
+BUILTIN_EVENT_CONNECTION_ESTABLISHED = "onConnectionEstablished"
 BUILTIN_EVENT_CONNECTION_ERROR      = "onConnectionError"
 
 BUILTIN_EVENT_CLIENT_CONNECTED      = "onClientConnected"
 BUILTIN_EVENT_CLIENT_DISCONNECTED   = "onClientDisconnected"
 
 STATE_HEADER    = "STATE_HEADER"
 STATE_PAYLOAD   = "STATE_PAYLOAD"
@@ -162,15 +159,15 @@
         self.datas = {}
 
     def __repr__(self):
         return self.name
 
     def send_message(self, Message_, Content_):
         try:
-            Encoded = ursina_networking_encode_message(Message_, Content_)
+            if (Encoded:=ursina_networking_encode_message(Message_, Content_))==b"": return False
             self.socket.sendall(Encoded)
             return True
         except Exception as e:
             ursina_networking_log("UrsinaNetworkingConnectedClient", "send_message", e)
             return False
 
 class UrsinaNetworkingServer():
@@ -289,15 +286,15 @@
     def handle(self, Ip_, Port_):
             try:
                 self.client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 self.connection_response = self.client.connect_ex((Ip_, Port_))
 
                 if self.connection_response == 0:
                     self.connected = True
-                    self.events_manager.push_event(BUILTIN_EVENT_CONNECTION_ETABLISHED)
+                    self.events_manager.push_event(BUILTIN_EVENT_CONNECTION_ESTABLISHED)
 
                     ursina_networking_log("UrsinaNetworkingClient", "handle", "Client connected successfully !")
 
                     while True:
 
                         try:
 
@@ -321,15 +318,15 @@
             except Exception as e:
                 self.events_manager.push_event("connectionError", e)
                 ursina_networking_log("UrsinaNetworkingClient", "handle", f"Connection Error : {e}")
 
     def send_message(self, Message_, Content_):
         try:
             if self.connected:
-                encoded_message = ursina_networking_encode_message(Message_, Content_)
-                self.client.sendall(encoded_message)
+                if (Encoded:=ursina_networking_encode_message(Message_, Content_))==b"": return False
+                self.client.sendall(Encoded)
                 return True
             else:
                 ursina_networking_log("UrsinaNetworkingClient", "send_message", f"WARNING : You are trying to send a message but the socket is not connected !")
         except Exception as e:
             ursina_networking_log("UrsinaNetworkingClient", "send_message", e)
             return False
```

