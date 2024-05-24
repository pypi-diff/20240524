# Comparing `tmp/Pyhoot-1.2.1.tar.gz` & `tmp/pyhoot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyhoot-1.2.1.tar", last modified: Thu Jan 11 23:30:13 2024, max compression
+gzip compressed data, was "pyhoot-1.3.0.tar", last modified: Fri May 24 04:08:26 2024, max compression
```

## Comparing `Pyhoot-1.2.1.tar` & `pyhoot-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:30:13.252689 Pyhoot-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-11 23:30:13.252689 Pyhoot-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:30:13.248689 Pyhoot-1.2.1/Pyhoot/
--rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-01-11 23:29:57.000000 Pyhoot-1.2.1/Pyhoot/Client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-01-11 23:29:57.000000 Pyhoot-1.2.1/Pyhoot/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-01-11 23:29:57.000000 Pyhoot-1.2.1/Pyhoot/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 23:29:57.000000 Pyhoot-1.2.1/Pyhoot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:30:13.252689 Pyhoot-1.2.1/Pyhoot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-11 23:30:13.000000 Pyhoot-1.2.1/Pyhoot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-11 23:30:13.000000 Pyhoot-1.2.1/Pyhoot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 23:30:13.000000 Pyhoot-1.2.1/Pyhoot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-11 23:30:13.000000 Pyhoot-1.2.1/Pyhoot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-11 23:30:13.000000 Pyhoot-1.2.1/Pyhoot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 23:30:13.252689 Pyhoot-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-11 23:29:57.000000 Pyhoot-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:08:26.726264 pyhoot-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 04:08:26.726264 pyhoot-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:08:26.726264 pyhoot-1.3.0/Pyhoot/
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-05-24 04:08:22.000000 pyhoot-1.3.0/Pyhoot/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-24 04:08:22.000000 pyhoot-1.3.0/Pyhoot/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-24 04:08:22.000000 pyhoot-1.3.0/Pyhoot/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 04:08:22.000000 pyhoot-1.3.0/Pyhoot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:08:26.726264 pyhoot-1.3.0/Pyhoot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 04:08:26.000000 pyhoot-1.3.0/Pyhoot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-24 04:08:26.000000 pyhoot-1.3.0/Pyhoot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 04:08:26.000000 pyhoot-1.3.0/Pyhoot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 04:08:26.000000 pyhoot-1.3.0/Pyhoot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 04:08:26.000000 pyhoot-1.3.0/Pyhoot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 04:08:26.726264 pyhoot-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-24 04:08:22.000000 pyhoot-1.3.0/setup.py
```

### Comparing `Pyhoot-1.2.1/PKG-INFO` & `pyhoot-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Pyhoot
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Python library used for the Kahoot! Api
 Author: Maxgamertyper1 (Max Allen)
 Author-email: maxa5302@gmail.com
 License: MIT
-Keywords: python,Kahoot,pyhoot,bot,flooder,sockets
+Keywords: python,Kahoot,pyhoot,bot,flooder,Kahoot!
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
 Requires-Dist: websocket-client
 Requires-Dist: fake_useragent
 
 A package that allows users to create Kahoot! clients and use the Kahoot! API to their will.
-Check out https://github.com/maxgamertyper/Pyhoot for more information.
+Check out https://github.com/maxgamertyper/Pyhoot for more information.
```

### Comparing `Pyhoot-1.2.1/Pyhoot/Client.py` & `pyhoot-1.3.0/Pyhoot/Client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,218 +1,351 @@
 import websocket
 import time
 import json as JSON
 import threading
 from fake_useragent import UserAgent as UA
-from .Token import Token
-from . import Exceptions
+from . import Exceptions, Token
 import inspect
 import random
 import itertools
 
-class Client():
-    def __init__(self, gamepin:str=None, name:str="bot",quizuuid:str="",random_text:str="",auth_bypass:bool=True):
+class BaseClient():
+    def __init__(self):
+        #WebSocket Data
+        self.WebChannels={"META_HANDSHAKE": "/meta/handshake", "META_CONNECT": "/meta/connect", "META_DISCONNECT": "/meta/disconnect", "SERVICE_CONTROLLER": "/service/controller", "SERVICE_PLAYER": "/service/player" }
+        self.WS=None
+        #Storage Data
         self.data = {}
         self.sent = {}
-        self.auth_bypass=auth_bypass
         self.web_log=[]
-        self.random_text="Hello, I am a bot and can not answer this question" if random_text=="" else random_text
-        self.latest_listener_call=None
         self.previous_data={}
-        self.WebSocket = None
-        self.WebChannels={ "META_HANDSHAKE": "/meta/handshake", "META_CONNECT": "/meta/connect", "META_DISCONNECT": "/meta/disconnect", "SERVICE_CONTROLLER": "/service/controller", "SERVICE_PLAYER": "/service/player" }
-        self.ClientData={"gamepin":gamepin,"clientId":None,"pong_count":1,"name":name,"messageId":1,"token":None}
+        self.msgid=0
+        #Listening Data
+        self.ListeningFunctions={}
+        self.ListeningTypes=[]
+        # TBD Data
+        self.clientid=None
+        self.connection_init=threading.Event()
+        self.gamepin=None
+        #Constant data
         self.UserAgent = UA().random
-        self.game_info = None
-        self.connection_init = threading.Event()
-        self.logged_in = threading.Event()
-        self.quizuuid=quizuuid
-        self.questionindex=1
-        self.ListeningData={"functions":{},"types":["pinged","handshake_1","handshake_2","avatar_updated", "disconnected", "question_started", "question_ended", "question_awaited", "quiz_started", "quiz_ended", "unknown_message","joined","auth_reset","auth_correct","auth_incorrect"],"eventIds":{14:"handshake2",46:"avatar_updated",10:"disconnected",2:"question_awaited",8:"question_ended",9:"quiz_started",13:"quiz_ended",53:"auth_reset",52:"auth_correct",51:"auth_incorrect"}}
-        self.question_data=None
-        self.disconnected=False
-        self.quiz_data={}
-        self.auth_reset=threading.Event()
-        self.auth_correct=threading.Event()
-        self.stableid=None
-        self.stepverified=False
-
-    def on_open(self,ws):
-        self.init_connection(ws)
+        self.msghandler=None
+    
+    def send(self, msg):
+        try:
+            self.sent=msg[0]
+            msg[0]["id"]=self.msgid
+            msg = JSON.dumps(msg)
+            self.web_log.append(msg)
+            self.WS.send(msg)
+            self.msgid += 1
+            return "sent"
+        except Exception as e:
+            self.exception_handler(Exceptions.SendingException,e)
+    
+    def pong(self,ack):
+        packet=self.packet_factory("META_CONNECT",ext={"ack": ack, "timesync": {"tc": self.time(), "l": 0, "o": 0}})
+        self.send(packet)
+        return "ponged"
+    
+    def time(self):
+        return str(round(time.time() * 1000))
+    
+    def kill(self):
+        if self.WS:
+            self.WS.close()
+        for thread in threading.enumerate():
+            if thread.name == "Thread-WebSocketApp":
+                thread.terminate()
+        return "killed"
 
-    def on_message(self,ws, message):
-        self.MessageReceiver(message)
+    def close(self):
+        if self.WS:
+            self.WS.close()
+        return "closed"
 
-    def exception_handler(self,exception,param1,param2=""):
-        if self.logged_in.is_set():
-            self.disconnect()
-            time.sleep(1)
-        self.close()
-        if param2:
-            raise exception(param1,param2)
-        else:
-            raise exception(param1)
+    def event_listener(self, Ltype:str):
+        def custom_decorator(func):
+            if not callable(func):
+                self.exception_handler(Exceptions.ListenerFunctionNotCallableException,Ltype)
+            parameters = inspect.signature(func).parameters
+            has_parameters = any(p.kind == p.POSITIONAL_OR_KEYWORD for p in parameters.values())
+            if not has_parameters:
+                self.exception_handler(Exceptions.ListenerFunctionParametersException,Ltype)
+            if Ltype in self.ListeningTypes:
+                self.ListeningFunctions[Ltype] = func
+            else:
+                self.exception_handler(Exceptions.UnknownListenerException,Ltype)
+        return custom_decorator
 
+    def ListenerFunction(self,functiontype,call=False,data=None):
+        if call and callable(self.ListeningFunctions.get(functiontype)):
+            self.ListeningFunctions.get(functiontype)(data=data)
+            return True
+        return self.ListeningFunctions.get(functiontype) if functiontype in self.ListeningFunctions else None
+    
     # websocket connection to kahoot's servers
     def init_connection(self, ws):
         try:
-            self.WebSocket = ws
-            firsthandshake = [{"id": "1", "version": "1.0", "minimumVersion": "1.0", "channel": self.WebChannels["META_HANDSHAKE"], "supportedConnectionTypes": ["websocket", "long-polling", "callback-polling"], "advice": {"timeout": 60000, "interval": 0}, "ext": {"ack": True, "timesync": {"tc": self.time(), "l": 0, "o": 0}}}]
-            self.send(firsthandshake)
+            self.WS = ws
+            self.send([{"version": "1.0", "minimumVersion": "1.0", "channel": self.WebChannels["META_HANDSHAKE"], "supportedConnectionTypes": ["websocket", "long-polling", "callback-polling"], "advice": {"timeout": 60000, "interval": 0}, "ext": {"ack": True, "timesync": {"tc": self.time(), "l": 0, "o": 0}}}])
         except Exception as e:
             self.exception_handler(Exceptions.KahootInitException,e)
 
     # second part of the connection to kahoot
     def second_handshake(self):
         try:
-            secondhandshake = [{"id": "2", "channel": self.WebChannels["META_CONNECT"], "connectionType": "websocket", "advice": {"timeout": 0}, "clientId": self.ClientData["clientId"], "ext": {"ack": 0, "timesync": {"tc": self.time(), "l": 0, "o": 0}}}]
-            self.send(secondhandshake)
+            self.send([{"channel": self.WebChannels["META_CONNECT"], "connectionType": "websocket", "advice": {"timeout": 0}, "clientId": self.clientid, "ext": {"ack": 0, "timesync": {"tc": self.time(), "l": 0, "o": 0}}}])
             self.connection_init.set()
+            self.ListenerFunction("handshake_2",True,True)
         except Exception as e:
             self.exception_handler(Exceptions.KahootInitException,e)
+    
+    def on_open(self,ws):
+        self.init_connection(ws)
+    
+    def on_close(self,ws):
+        print("Websocket Closed")
 
-    #used for reciving messages
-    def MessageReceiver(self, msg):
-        self.previous_data=self.data
-        self.data = JSON.loads(msg)[0]
-        self.web_log.append(JSON.loads(msg))
-        self.MessageHandler()
-    
-    #used for handling information on messages
-    def MessageHandler(self):
-        func=None
-        prev_func=None
+    def on_message(self,ws, message):
+        self.BaseMessageHandler(message)
+        
+    def BaseMessageHandler(self,msg):
+        msg=JSON.loads(msg)[0]
+        ack=msg.get("ext",{}).get("ack")
         data=self.data.get("data",{})
-        print("\n in \n",self.data)
+        self.data=msg
         
-        error = data.get("error") if data.get("error") is not None else self.data.get("error")
+        #wait for first handshake response / ack
+        if ack is True:
+            self.ListenerFunction("handshake_1",True,True)
+            self.clientid=msg["clientId"]
+            self.second_handshake()
+        elif ack is not None: # if the client gets heartbeat respond with a pong
+            self.pong(ack)
+            self.ListenerFunction("heartbeat",True,ack)
+            
+        error = data.get("error") if data.get("error") is not None else msg.get("error")
 
-        if error is not None:
+        if error is not None and self.disconnected==False:
             reason = str(data.get("description"))
             if reason == "Duplicate name":
-                self.exception_handler(Exceptions.NameTakenException,self.ClientData["name"])
+                self.exception_handler(Exceptions.NameTakenException,self.name)
             elif error=="402::session_unknown":
-                self.exception_handler(Exceptions.UnknownSessionException,self.ClientData["clientId"],self.sent.get("clientId"))
+                self.exception_handler(Exceptions.UnknownSessionException,self.clientid,self.sent.get("clientId"))
             else:
                 self.exception_handler(Exceptions.UnknownException,error,reason)
-        
-        ext=self.data.get("ext",{})
-        ack=str(ext.get("ack"))
+            
+        if callable(self.msghandler):
+            self.msghandler(msg)
 
-        if ack!="True" and ack !="None":
-            if self.disconnected==True:
-                return
-            self.pong_count=int(ack)
-            self.pong()
-            if self.latest_listener_call=="question_awaited":
-                prev_func=self.ListeningData["functions"].get("question_started")
-            if self.latest_listener_call=="auth_correct":
-                print("claaed")
-                time.sleep(random.randint(50,100)/100)
-                self.send([{"id":self.ClientData["messageId"],"channel":"/service/controller","data":{"id":16,"type":"message","gameid":self.ClientData["gamepin"],"host":"kahoot.it","content":JSON.dumps({"stableIdentifier":self.stableid,"usingNamerator":False})},"clientId":self.ClientData["clientId"],"ext":{}}])
-                self.auth_correct.set()
-            func=self.ListeningData["functions"].get("pinged")
-        elif ack=="True":
-            self.ClientData["clientId"] = self.data.get("clientId")
-            self.second_handshake()
-            func=self.ListeningData["functions"].get("handshake1")
-
-        id=data.get("id")
-        info=self.data
-        del info["ext"]
-        del info["channel"]
-        
-        if id==17:
-            content=JSON.loads(self.data.get("data").get("content"))
-            self.stableid=content.get("stableIdentifier")
-
-        if id in list(self.ListeningData["eventIds"].keys()):
-            if id==10:
-                if info.get("data",{}).get("content")=='{"kickCode":1}':
-                    del info["data"]["content"]
-                    info["reason"]="kicked"
-            elif id ==2:
-                self.questionindex=int(JSON.loads(self.data.get("data").get("content")).get("gameBlockIndex"))
-                self.question_data=self.data
-            elif id==53:
-                self.auth_reset.set()
-                time.sleep(1)
-                self.auth_reset.clear()
-            elif id==52:
-                pass
-            event=self.ListeningData["eventIds"].get(id)
-            func=self.ListeningData["functions"].get(event)
-            self.latest_listener_call=event
-        elif data.get("reason")=="disconnect":
-            func=self.ListeningData["functions"].get("disconnected")
-            info["reason"]='host left'
-            del info["data"]["reason"]
-            self.disconnected=True
-        elif str(data.get("type"))=="loginResponse":
-            self.latest_listener_call="joined"
-            func=self.ListeningData["functions"].get("joined")
+    def exception_handler(self,exception,param1,param2=""):
+        self.close()
+        if param2:
+            raise exception(param1,param2)
         else:
-            func=self.ListeningData["functions"].get("unkown message")
-            self.latest_listener_call="unknown message"
+            raise exception(param1)
         
-        if callable(func):
-            func(info)
-        if callable(prev_func):
-            prev_func(self.previous_data)
-            self.latest_listener_call="question_answered"
-    
-    #used for sending messages
-    def send(self, msg):
-        try:
-            self.sent=msg[0]
-            msg = JSON.dumps(msg)
-            print("\n out \n",msg)
-            self.web_log.append(msg)
-            self.WebSocket.send(msg)
-            self.ClientData["messageId"] += 1
-            return "sent"
-        except Exception as e:
-            self.exception_handler(Exceptions.SendingException,e)
-    
-    #used to get the current time since epoch in miliseconds
-    def time(self):
-        return str(round(time.time() * 1000))
-
-    #used to respond to the kahoot servers pinging the client
-    def pong(self):
-        packet=self.packet_factory("META_CONNECT",ext={"ack": self.pong_count, "timesync": {"tc": self.time(), "l": 0, "o": 0}})
-        self.send(packet)
-        return "ponged"
-    
     def packet_factory(self,channel,data="",ext={}):
         packet=[{
             "channel":self.WebChannels[channel],
-            "clientId":str(self.ClientData["clientId"]),
+            "clientId":str(self.clientid),
             "data":data,
-            "id":self.ClientData["messageId"],
             "ext":ext,
             "connectionType": "websocket"
             }]
         if data=="":
             packet[0].pop("data")
         return packet
     
     def data_factory(self, content, type1: str, id_int: int = -1):
         data = {
-            "gameid": self.ClientData["gamepin"],
+            "gameid": self.gamepin,
             "host": "kahoot.it",
             "type": str(type1),
             "id": id_int,
             "content": JSON.dumps(content),
-            "name": self.ClientData["name"]
+            "name": self.name
         }
         if id_int==-1:
             data.pop("id")
         return data
     
+    def find_game(self,gamepin):
+        return Token.Token(gamepin,self.UserAgent,check=True)
+    
+class Player(BaseClient):
+    def __init__(self,Auth_Brute_Force:bool=False,random_text:str="Hello, I am a bot and can not answer this question",closeafterdisconnect:bool=False):
+        super().__init__()
+        self.token=None
+        self.random_text=random_text
+        self.ListeningTypes=["heartbeat","handshake_1","handshake_2","profile_updated", "disconnected", "question_started", "question_ended", "question_awaited", "quiz_started", "quiz_ended", "unknown_message","joined","auth_reset","auth_correct","auth_incorrect"]
+        self.joined=threading.Event()
+        self.quizuuid=None
+        self.msghandler=self.MessageHandler
+        #auth
+        self.auth_reset=threading.Event()
+        self.auth_correct=threading.Event()
+        self.authbrute=Auth_Brute_Force
+        #question data
+        self.questionindex=0
+        self.question_data=None
+        #"safety"
+        self.cad=closeafterdisconnect
+        self.disconnected=False
+        #custom storage stuff
+        self.profileid=None
+    
+    def start(self,gamepin:str):
+        self.gamepin=gamepin
+        if self.token==None:
+            a=Token.Token(self.gamepin,self.UserAgent)
+            self.token=a["Token"]
+            self.game_info=a["info"]
+        try:
+            ws = websocket.WebSocketApp(f'wss://kahoot.it/cometd/{self.gamepin}/{self.token}/', on_message=self.on_message, on_open=self.on_open)
+            wst=threading.Thread(target=ws.run_forever)
+            wst.start()
+        except Exception as e:
+            self.exception_handler(Exceptions.WebSocketInitException,e)
+    
+    def join(self,name:str,profile:str="",quizuuid=None):
+        self.connection_init.wait()  # Wait for the WebSocket connection to be established
+
+        self.quizuuid=quizuuid
+        self.name = name
+        
+        login_data=self.data_factory({"device":{"userAgent":f"{self.UserAgent}","screen":{"width":1920,"height":1080}}},"login")
+        login_packet=self.packet_factory("SERVICE_CONTROLLER",login_data)
+        login_follup_data=self.data_factory(profile,"message",16)
+        login_followup_packet=self.packet_factory("SERVICE_CONTROLLER",login_follup_data)
+        self.send(login_packet)
+        self.send(login_followup_packet)
+        
+        if self.authbrute:
+            self.forceauth()
+        
+        return True
+            
+    def join_crash(self,name:str):
+        self.connection_init.wait()  # Wait for the WebSocket connection to be established
+        self.name = name
+        
+        login_data=self.data_factory({"device":{"userAgent":f"{self.UserAgent}","screen":{"width":1920,"height":1080}}},"login")
+        login_packet=self.packet_factory("SERVICE_CONTROLLER",login_data)
+        login_follup_data=self.data_factory(None,"message",16)
+        login_followup_packet=self.packet_factory("SERVICE_CONTROLLER",login_follup_data)
+        self.send(login_packet)
+        self.send(login_followup_packet)
+        
+    def forceauth(self):
+        time.sleep(5)
+        authcodes=[(0, 1, 2, 3), (0, 1, 3, 2), (0, 2, 1, 3), (0, 2, 3, 1), (0, 3, 1, 2), (0, 3, 2, 1), (1, 0, 2, 3), (1, 0, 3, 2), (1, 2, 0, 3), (1, 2, 3, 0), (1, 3, 0, 2), (1, 3, 2, 0), (2, 0, 1, 3), (2, 0, 3, 1), (2, 1, 0, 3), (2, 1, 3, 0), (2, 3, 0, 1), (2, 3, 1, 0), (3, 0, 1, 2), (3, 0, 2, 1), (3, 1, 0, 2), (3, 1, 2, 0), (3, 2, 0, 1), (3, 2, 1, 0)]
+        self.auth_reset.wait()
+        for sequence in authcodes:
+                if self.auth_correct.is_set():
+                    break
+                packet = [{
+                    "channel":self.WebChannels["SERVICE_CONTROLLER"],
+                    "data":
+                    {"id":50,
+                     "type":"message",
+                     "gameid":self.gamepin,
+                     "host":"kahoot.it",
+                     "content":JSON.dumps({"sequence":''.join(map(str, sequence))})},
+                     "clientId":str(self.clientid),
+                     "ext":{}}]
+                self.send(packet)
+                time.sleep(.22)
+        
+    def profile_generator(self,avatar:str,cosmetic:str):
+        avatar_map={'WHITE_BEAR': 2350,'PENGUIN': 2300,'REINDEER': 5373,'CHRISTMAS_TREE': 5374,'COOKIE': 5375,'BROWN_RAT': 1800,'GROUNDHOG': 1600,'GRAY_RAT': 4000,'MOOSE': 1500,'PUG': 1700,'DOG': 1700, 'CAT': 1750,'RABBIT': 1850,'RED_FOX': 1900,'GRAY_FOX': 1950,'BROWN_FOX': 2000,'PANDA': 2050,'FROG': 2100,'OWL': 2150,'CHICKEN': 2200,'FEATHERLESS_CHICKEN': 2250,'GOAT': 2400,'TIGER': 2500,'KOALA': 2550,'KANGAROO': 2600,'HORSE': 2650,'BRAIN': 2950,'UNICORN': 2700,'GREEN_MONSTER': 2800,'PURPLE_MONSTER': 2850,'PINK_MONSTER': 2900,'ZOMBIE': 3000,'SKELETON': 3050,'GLOBE': 2750,}
+        cosmetic_map = {'PANCAKES': 3950, 'CHRISTMAS_HAT': 5372, 'MONOCLE': 1250, 'SCARF': 2750, 'WINTER_HAT': 5371, 'EAR_MUFFS': 5370, 'SNOW_GOGGLES': 4100, 'COLORED_SUNGLASSES': 4050, 'SANTA_HAT': 5368, 'BEARD': 5367, 'TREE_HAT': 5366, 'PRESENT_HAT': 5365, 'KAHOOT_HAT': 1550, 'GLOWER_HAT': 3100, 'CROWN': 3150, 'VIKING_HAT': 3200, 'GRADUATION_CAP': 3250, 'COWBOY_HAT': 3300, 'WITCH_HAT': 3350, 'HEADPHONES': 3400, 'HEARTS': 3450, 'HEART_GLASSES': 3500, 'GOGGLES': 3550, 'HARD_HAT': 5300, 'EXPLORER_HAT': 5309, 'EYEPATCH': 3600, 'POWDERED_WIG': 1300, 'ALBERT_EINSTIEN': 1350, 'HAIR': 1400, 'SUNGLASSES': 3650, 'TOP_HAT': 3700, 'KID_HAT': 3750, 'PARTY_HAT': 3800, 'FAKE_DISGUISE': 3850, 'PACIFIER': 3900, 'ICE_CREAM_CONE': 4000, 'FOOTBALL_HELMET': 4150, 'ASTRONAUT_HELMET': 4200}
+        avatarid=avatar_map.get(avatar.upper())
+        cosmeticid=cosmetic_map.get(cosmetic.upper())
+        return {"avatar":{"type":avatarid,"item":cosmeticid}}
+    
+    def update_profile(self,profile):
+        self.joined.wait()
+        data=self.data_factory(profile,"message",46)
+        packet=self.packet_factory("SERVICE_CONTROLLER",data)
+        del packet[0]["connectionType"]
+        del packet[0]["data"]["name"]
+        self.profileid=self.msgid+1
+        self.send(packet)
+    
+    def disconnect(self):
+        self.disconnected=True
+        self.send([{"id":self.msgid,"channel":self.WebChannels["META_DISCONNECT"],"clientId":str(self.clientid),"ext":{"timesync":{"tc":self.time(),"l":0,"o":0}}}])
+        self.ListenerFunction("disconnected",True,{"Reason":"Player Left"})
+        self.joined.clear()
+        if self.cad:
+            self.close()
+    
+    def MessageHandler(self,msg):
+        data=self.data.get("data",{})
+        
+        if data.get("reason")=="disconnect":
+            if data.get("type")=="status" and data.get("status")=="MISSING":
+                return self.ListenerFunction("disconnected",True,{"Reason":"Host Left the Game"})
+            else:
+                return self.ListenerFunction("disconnected",True,{"Reason":data,"Report":"This is an unknown disconnect, please report this and what happened"})
+        
+        msgtype=data.get("type")
+        msgid=msg.get("id") if msg.get("id") is None else int(msg.get("id"))
+        
+        if msgid==self.profileid and msg.get("successful") is True:
+            return self.ListenerFunction("profile_updated",True,True)
+        elif msgid==self.profileid and msg.get("successful") is False:
+            return self.ListenerFunction("profile_updated",True,False)
+        
+        if msgtype=="loginResponse": #if its a login response
+            self.joined.set()
+            if data.get("description")=="Duplicate name":
+                return self.ListenerFunction("joined",True,{"Error":"Duplicate name"})
+            return self.ListenerFunction("joined",True,True) # call the listener joined function
+        
+        ListeningIds={10:"disconnected",2:"question_started",8:"question_ended",9:"quiz_started",13:"quiz_ended",53:"auth_reset",52:"auth_correct",51:"auth_incorrect"}
+        id=data.get("id")
+        
+        if id in list(ListeningIds.keys()):
+            if id==53: # if the auth is reset
+                self.auth_reset.set()
+                time.sleep(1)
+                self.auth_reset.clear()
+                return self.ListenerFunction(ListeningIds[id],True,True)
+            elif id==52: # if the auth is correct
+                self.auth_correct.set()
+                return self.ListenerFunction(ListeningIds[id],True,True)
+            elif id==51: # auth is incorrect
+                return self.ListenerFunction(ListeningIds[id],True,False)
+            elif id==2:
+                self.questionindex=int(JSON.loads(data.get("content")).get("gameBlockIndex"))
+                self.question_data=self.data
+            elif id==10:
+                if data.get("content")=="{\"kickCode\":1}":
+                    self.ListenerFunction("disconnected",True,{"Reason":"Host Kicked Player"})
+                    self.disconnected=True
+                    if self.cad:
+                        self.close()
+                    return
+            elif id==9: #quiz_started
+                # beta
+                return self.ListenerFunction(ListeningIds[id],True,msg)
+            elif id==8: # question_ended
+                # beta
+                return self.ListenerFunction(ListeningIds[id],True,msg)
+            elif id==13: #quiz_ended
+               #beta
+                return self.ListenerFunction(ListeningIds[id],True,msg)
+            if id==2: #question_started
+                #beta
+                return self.ListenerFunction(ListeningIds[id],True,msg)
+            return self.ListenerFunction(ListeningIds[id],True,msg)
+            
     def question_content_factory(self,answer,lag):
         question_type=JSON.loads(self.question_data.get("data").get("content")).get("type")
         content={
             "type":question_type,
             "questionIndex":self.questionindex,
             "meta":{"lag":lag}
         }
@@ -260,157 +393,51 @@
                 elif answer=="green" or answer==3:
                     answer=3
                 else:
                     self.exception_handler(Exceptions.InvalidAnswerException,answer)
             content["choice"]=answer
         return content
 
-    def question_packet_factory(self,answer,lag):
+    def question_packet_factory(self,answer=None,lag=None,content=None):
+        if answer is not None and lag is not None:
+            content=self.question_content_factory(answer,lag)
+        if content is None and answer is None and lag is None:
+            return "Error no answer data sent"
         packet=[{
-            "id":self.ClientData["messageId"],
+            "id":self.msgid,
             "channel": self.WebChannels["SERVICE_CONTROLLER"],
             "data":{
                 "id":45,
                 "type":"message",
-                "gameid":self.ClientData["gamepin"],
+                "gameid":self.gamepin,
                 "host":"kahoot.it",
-                "content":JSON.dumps(self.question_content_factory(answer,lag))
+                "content":JSON.dumps(content)
                 },
-            "clientId":str(self.ClientData["clientId"]),
+            "clientId":str(self.clientid),
             "ext":{}
         }]
         return packet
     
-
-
-    #used by user and not websocket/generator only
-
-
-
-    def start(self,gamepin:str=None):
-        self.ClientData["gamepin"]=gamepin if gamepin is not None else self.ClientData["gamepin"]
-        gamepin=self.ClientData["gamepin"]
-        if gamepin==None:
-            self.exception_handler(Exceptions.GamePinException,"")
-        if self.ClientData["token"]==None:
-            a=Token(self.ClientData["gamepin"],self.UserAgent)
-            self.ClientData["token"]=a["Token"]
-            self.game_info=a["info"]
-        try:
-            ws = websocket.WebSocketApp(f'wss://kahoot.it/cometd/{self.ClientData["gamepin"]}/{self.ClientData["token"]}/', on_message=self.on_message, on_open=self.on_open)
-            wst=threading.Thread(target=ws.run_forever)
-            wst.start()
-        except Exception as e:
-            self.exception_handler(Exceptions.WebSocketInitException,e)
-    
-    def kill(self):
-        if self.WebSocket:
-            self.WebSocket.close()
-        
-        for thread in threading.enumerate():
-            if thread.name == "Thread-WebSocketApp":
-                thread.terminate()
-        return "killed"
-
-    def close(self):
-        if self.WebSocket:
-            self.WebSocket.close()
-        return "closed"
-
-    #the decorator for functions that calls them on use
-    def event_listener(self, listening_type:str):
-        def custom_decorator(func):
-            if not callable(func):
-                self.exception_handler(Exceptions.ListenerFunctionNotCallableException,listening_type)
-            parameters = inspect.signature(func).parameters
-            has_parameters = any(p.kind == p.POSITIONAL_OR_KEYWORD for p in parameters.values())
-            if not has_parameters:
-                self.exception_handler(Exceptions.ListenerFunctionParametersException,listening_type)
-            if listening_type in self.ListeningData["types"]:
-                self.ListeningData["functions"][listening_type] = func
-            else:
-                self.exception_handler(Exceptions.UnknownListenerException,listening_type)
-        return custom_decorator
-
-    # used to generate the information on a profile
-    def profile_generator(self,avatar:str,cosmetic:str):
-        avatar_map={'WHITE_BEAR': 2350,'PENGUIN': 2300,'REINDEER': 5373,'CHRISTMAS_TREE': 5374,'COOKIE': 5375,'BROWN_RAT': 1800,'GROUNDHOG': 1600,'GRAY_RAT': 4000,'MOOSE': 1500,'PUG': 1700,'DOG': 1700, 'CAT': 1750,'RABBIT': 1850,'RED_FOX': 1900,'GRAY_FOX': 1950,'BROWN_FOX': 2000,'PANDA': 2050,'FROG': 2100,'OWL': 2150,'CHICKEN': 2200,'FEATHERLESS_CHICKEN': 2250,'GOAT': 2400,'TIGER': 2500,'KOALA': 2550,'KANGAROO': 2600,'HORSE': 2650,'BRAIN': 2950,'UNICORN': 2700,'GREEN_MONSTER': 2800,'PURPLE_MONSTER': 2850,'PINK_MONSTER': 2900,'ZOMBIE': 3000,'SKELETON': 3050,'GLOBE': 2750,}
-        cosmetic_map = {'PANCAKES': 3950, 'CHRISTMAS_HAT': 5372, 'MONOCLE': 1250, 'SCARF': 2750, 'WINTER_HAT': 5371, 'EAR_MUFFS': 5370, 'SNOW_GOGGLES': 4100, 'COLORED_SUNGLASSES': 4050, 'SANTA_HAT': 5368, 'BEARD': 5367, 'TREE_HAT': 5366, 'PRESENT_HAT': 5365, 'KAHOOT_HAT': 1550, 'GLOWER_HAT': 3100, 'CROWN': 3150, 'VIKING_HAT': 3200, 'GRADUATION_CAP': 3250, 'COWBOY_HAT': 3300, 'WITCH_HAT': 3350, 'HEADPHONES': 3400, 'HEARTS': 3450, 'HEART_GLASSES': 3500, 'GOGGLES': 3550, 'HARD_HAT': 5300, 'EXPLORER_HAT': 5309, 'EYEPATCH': 3600, 'POWDERED_WIG': 1300, 'ALBERT_EINSTIEN': 1350, 'HAIR': 1400, 'SUNGLASSES': 3650, 'TOP_HAT': 3700, 'KID_HAT': 3750, 'PARTY_HAT': 3800, 'FAKE_DISGUISE': 3850, 'PACIFIER': 3900, 'ICE_CREAM_CONE': 4000, 'FOOTBALL_HELMET': 4150, 'ASTRONAUT_HELMET': 4200}
-        avatarid=avatar_map.get(avatar.upper())
-        cosmeticid=cosmetic_map.get(cosmetic.upper())
-        return {"avatar":{"type":avatarid,"item":cosmeticid}}
-    
-    def auth_brute(self):
-            authcodes=list(itertools.permutations([0,1,2,3],4))
-            self.auth_reset.wait()
-            for sequence in authcodes:
-                if self.auth_correct.is_set():
-                    break
-                packet = [{
-                    "id":self.ClientData["messageId"],
-                    "channel":self.WebChannels["SERVICE_CONTROLLER"],
-                    "data":
-                    {"id":50,
-                     "type":"message",
-                     "gameid":self.ClientData["gamepin"],
-                     "host":"kahoot.it",
-                     "content":JSON.dumps({"sequence":''.join(map(str, sequence))})},
-                     "clientId":str(self.ClientData["clientId"]),
-                     "ext":{}}]
-                self.send(packet)
-                time.sleep(.1)
-
-    # used to join an active kahoot game
-    def join(self, name:str="",profile:str="",quizuuid=None):
-        self.connection_init.wait()  # Wait for the WebSocket connection to be established
-        time.sleep(1)
-
-        self.quizuuid=quizuuid if quizuuid is not None else self.quizuuid
-        name = self.ClientData["name"] if name == "" else name
-        self.ClientData["name"] = name
-
-        login_data=self.data_factory({"device":{"userAgent":f"{self.UserAgent}","screen":{"width":1920,"height":1080}}},"login")
-        login_packet=self.packet_factory("SERVICE_CONTROLLER",login_data)
-        login_follup_data=self.data_factory(profile,"message",16)
-        login_followup_packet=self.packet_factory("SERVICE_CONTROLLER",login_follup_data)
-        self.send(login_packet)
-        self.send(login_followup_packet)
-
-        self.join_sent=True
-
-        time.sleep(5)
-        
-        if self.game_info.get("twoFactorAuth") is True:
-            if self.auth_bypass:
-                self.auth_brute()
-            else:
-                return "Awaitng Auth password"
-        else:
-            self.auth_correct.set()
-            self.logged_in.set()
-
-    
-    # used to disconnect from a kahoot game
-    def disconnect(self):
-        self.disconnected=True
-        self.send([{"id":self.ClientData["messageId"],"channel":self.WebChannels["META_DISCONNECT"],"clientId":str(self.ClientData["clientId"]),"ext":{"timesync":{"tc":self.time(),"l":0,"o":0}}}])
-        if callable(self.ListeningData["functions"].get("disconnected")):
-            self.ListeningData["functions"]["disconnected"]({"data":{"gameid":self.gamepin,'host':'kahoot.it',"id":10,'type':'message'},"reason":"player left"})
-        self.logged_in.clear()
-    
-    # used to change profiles in a kahoot game
-    def change_profile(self,profile):
-        self.logged_in.wait()
-        data=self.data_factory(profile,"message",46)
-        packet=self.packet_factory("SERVICE_CONTROLLER",data)
-        del packet[0]["connectionType"]
-        del packet[0]["data"]["name"]
+    def answer_crash(self):
+        time.sleep(random.randint(15,25)/100)
+        packet=[{
+            "channel": self.WebChannels["SERVICE_CONTROLLER"],
+            "data":{
+                "id":45,
+                "type":"message",
+                "gameid":self.gamepin,
+                "host":"kahoot.it",
+                "content":JSON.dumps(None)
+                },
+            "clientId":str(self.clientid),
+            "ext":{}
+        }]
         self.send(packet)
-
-    #used to submit an answer in a kahoot game
+        return "Sent (only works when a question is present)"
+    
     def submit_answer(self,answer,delay:int=0):
         lag=round(random.random() * 60 + 5) + (delay*100)
         answer=0 if answer=="red" else answer
         answer=1 if answer=="blue" else answer
         answer=2 if answer=="yellow" else answer
         answer=3 if answer=="green" else answer
         time.sleep(delay+.25)
@@ -423,59 +450,36 @@
         content_data=JSON.loads(self.question_data.get("data").get("content"))
         question_type=content_data.get("type")
         if question_type=="drop_pin":
             # x:0 is far left
             # y:0 is far up
             answer={"x":(random.randint(0,100000000))/1000000,"y":(random.randint(0,100000000))/1000000}
         elif question_type=="jumble":
-            answer=list(random.choice(list(itertools.permutations([0,1,2,3],4))))
+            options=int(content_data.get("numberOfChoices"))
+            answer=list(random.choice(list(itertools.permutations(options))))
         elif question_type=="multiple_select_poll" or question_type=="multiple_select_quiz":
-            amount=random.randint(1,int(content_data.get("numberOfChoices")))
-            numbers=[0,1,2,3]
-            answer=[]
-            while amount>0:
-                num=random.choice(numbers)
-                answer.append(num)
-                numbers.remove(num)
-                amount-=1
+            options=int(content_data.get("numberOfChoices"))
+            results=[]
+            for r in range(1, options+1):
+                combinations_r = list(itertools.combinations(range(options), r))
+                results.extend([list(comb) for comb in combinations_r])
+            answer=random.choice(results)
         elif question_type=="feedback" or question_type=="brainstorming" or question_type=="word_cloud" or question_type=="open_ended":
             answer=self.random_text
         elif question_type=="slider":
             step=int(content_data.get("step"))
             min=int(content_data.get("minRange"))
             max=int(content_data.get("maxRange"))
             number=random.randint(min,max)
             number=round(number / step) * step
             answer=number+min
         else:
             if content_data.get("layout")=="TRUE_FALSE":
                 answer=random.randint(0,1)
             elif question_type=="quiz":
-                answer=random.randint(0,3)
+                answer=random.randint(0,int(content_data.get("numberOfChoices"))-1)
             elif question_type=="survey":
                 answer=random.randint(0,int(content_data.get("numberOfChoices"))-1)
         self.submit_answer(answer,delay)
     
-    def crash_lobby(self):
-        time.sleep(random.randint(15,25)/100)
-        packet=[{
-            "id":self.ClientData["messageId"],
-            "channel": self.WebChannels["SERVICE_CONTROLLER"],
-            "data":{
-                "id":45,
-                "type":"message",
-                "gameid":self.ClientData["gamepin"],
-                "host":"kahoot.it",
-                "content":JSON.dumps(None)
-                },
-            "clientId":str(self.ClientData["clientId"]),
-            "ext":{}
-        }]
-        self.send(packet)
-        return "Sent (only works when a question is present)"
-
-    def find_game(self,gamepin):
-        return Token(gamepin,self.UserAgent,check=True) 
-
-    # added crash_lobby
-    # fixed change_profile
-    # added auth bypass (auth_correct event listener and auth_wrong event listener)
+    def profile_crash(self):
+        self.update_profile(None)
```

### Comparing `Pyhoot-1.2.1/Pyhoot/Exceptions.py` & `pyhoot-1.3.0/Pyhoot/Exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,10 @@
     def __init__(self,error,description) -> None:
         super().__init__(f"Please Make An Issue Reporting this Exception: \"{error}\", description: \"{description}\"")
 
 class SendingException(Exception):
     def __init__(self,input,error) -> None:
         super().__init__(f"When sending the message: \"{input}\" and error occured, \"{error}\"")
 
-class UnknownSessionException(Exception):
-    def __init__(self,selfclientid,clientidsent) -> None:
-        super().__init__(f"This error happens mostly when the clientId is incorrect or none; ClientId sent was \"{clientidsent}\" and the classes clientid was \"{selfclientid}\"")
-
 class AuthBypassFalseError(Exception):
     def __init__(self,gamepin) -> None:
         super().__init__(f"The gamepin: \"{gamepin}\" has 2 step join but you have disabled the brute force method")
```

### Comparing `Pyhoot-1.2.1/Pyhoot/Token.py` & `pyhoot-1.3.0/Pyhoot/Token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 from bs4 import BeautifulSoup
 import base64
 from . import Exceptions
 import json as JSON
+import time # will be used soon
 
 def Token(gamepin:str,UA,check=False):
     if gamepin=="":
         raise Exceptions.GamePinException(gamepin)
     
     def ChallengeTokenSolver(message,offset):
         def repl(char, position):
```

### Comparing `Pyhoot-1.2.1/Pyhoot.egg-info/PKG-INFO` & `pyhoot-1.3.0/Pyhoot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Pyhoot
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Python library used for the Kahoot! Api
 Author: Maxgamertyper1 (Max Allen)
 Author-email: maxa5302@gmail.com
 License: MIT
-Keywords: python,Kahoot,pyhoot,bot,flooder,sockets
+Keywords: python,Kahoot,pyhoot,bot,flooder,Kahoot!
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
 Requires-Dist: websocket-client
 Requires-Dist: fake_useragent
 
 A package that allows users to create Kahoot! clients and use the Kahoot! API to their will.
-Check out https://github.com/maxgamertyper/Pyhoot for more information.
+Check out https://github.com/maxgamertyper/Pyhoot for more information.
```

### Comparing `Pyhoot-1.2.1/setup.py` & `pyhoot-1.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.1'
+VERSION = '1.3.0'
 DESCRIPTION = 'A Python library used for the Kahoot! Api'
-LONG_DESCRIPTION = 'A package that allows users to create Kahoot! clients and use the Kahoot! API to their will.\nCheck out https://github.com/maxgamertyper/Pyhoot for more information.'
+LONG_DESCRIPTION = 'A package that allows users to create Kahoot! clients and use the Kahoot! API to their will.\nCheck out https://github.com/maxgamertyper/Pyhoot for more information. \n'
 
 
 setup(
     name="Pyhoot",
     version=VERSION,
     author="Maxgamertyper1 (Max Allen)",
     author_email="maxa5302@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['requests', 'beautifulsoup4', 'websocket-client', 'fake_useragent'],
-    keywords=['python', 'Kahoot', 'pyhoot', 'bot', 'flooder', 'sockets'],
+    keywords=['python', 'Kahoot', 'pyhoot', 'bot', 'flooder', 'Kahoot!'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
```

