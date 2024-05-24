# Comparing `tmp/folkmq-1.4.6.tar.gz` & `tmp/folkmq-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folkmq-1.4.6.tar", last modified: Fri May 17 06:36:29 2024, max compression
+gzip compressed data, was "folkmq-1.5.0.tar", last modified: Fri May 24 13:24:40 2024, max compression
```

## Comparing `folkmq-1.4.6.tar` & `folkmq-1.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-17 06:36:29.204233 folkmq-1.4.6/
--rw-r--r--   0 noear      (501) staff       (20)      588 2024-05-17 06:36:29.203118 folkmq-1.4.6/PKG-INFO
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-17 06:36:29.187452 folkmq-1.4.6/folkmq/
--rw-r--r--   0 noear      (501) staff       (20)      511 2024-05-17 06:20:24.000000 folkmq-1.4.6/folkmq/FolkMQ.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-17 06:36:29.195864 folkmq-1.4.6/folkmq/client/
--rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/client/MqAlarm.py
--rw-r--r--   0 noear      (501) staff       (20)     4021 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqClient.py
--rw-r--r--   0 noear      (501) staff       (20)    15624 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqClientDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     5655 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqClientListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3879 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqMessage.py
--rw-r--r--   0 noear      (501) staff       (20)     3425 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqMessageReceived.py
--rw-r--r--   0 noear      (501) staff       (20)     1094 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqRouter.py
--rw-r--r--   0 noear      (501) staff       (20)      890 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqSubscription.py
--rw-r--r--   0 noear      (501) staff       (20)     1073 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/client/MqTransaction.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-17 06:36:29.201158 folkmq-1.4.6/folkmq/common/
--rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/common/MqApis.py
--rw-r--r--   0 noear      (501) staff       (20)     1079 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/common/MqAssert.py
--rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/common/MqConstants.py
--rw-r--r--   0 noear      (501) staff       (20)     2532 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/common/MqMetasResolver.py
--rw-r--r--   0 noear      (501) staff       (20)     4811 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/common/MqMetasResolverV1.py
--rw-r--r--   0 noear      (501) staff       (20)     5026 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/common/MqMetasResolverV2.py
--rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/common/MqMetasV1.py
--rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/common/MqMetasV2.py
--rw-r--r--   0 noear      (501) staff       (20)      422 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/common/MqTopicHelper.py
--rw-r--r--   0 noear      (501) staff       (20)     1184 2024-05-16 09:27:43.000000 folkmq-1.4.6/folkmq/common/MqUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/common/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-17 06:36:29.201773 folkmq-1.4.6/folkmq/exception/
--rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/exception/FolkmqException.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.4.6/folkmq/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-17 06:36:29.202313 folkmq-1.4.6/folkmq.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      588 2024-05-17 06:36:29.000000 folkmq-1.4.6/folkmq.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-17 06:36:29.000000 folkmq-1.4.6/folkmq.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-17 06:36:29.000000 folkmq-1.4.6/folkmq.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       48 2024-05-17 06:36:29.000000 folkmq-1.4.6/folkmq.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-17 06:36:29.000000 folkmq-1.4.6/folkmq.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-17 06:36:29.000000 folkmq-1.4.6/folkmq.egg-info/zip-safe
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-17 06:36:29.204483 folkmq-1.4.6/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      911 2024-05-17 06:21:05.000000 folkmq-1.4.6/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.489270 folkmq-1.5.0/
+-rw-r--r--   0 noear      (501) staff       (20)      587 2024-05-24 13:24:40.488533 folkmq-1.5.0/PKG-INFO
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.470216 folkmq-1.5.0/folkmq/
+-rw-r--r--   0 noear      (501) staff       (20)      624 2024-05-24 01:20:55.000000 folkmq-1.5.0/folkmq/FolkMQ.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.478751 folkmq-1.5.0/folkmq/client/
+-rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/client/MqAlarm.py
+-rw-r--r--   0 noear      (501) staff       (20)     4021 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqClient.py
+-rw-r--r--   0 noear      (501) staff       (20)    15624 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqClientDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     5657 2024-05-22 11:46:21.000000 folkmq-1.5.0/folkmq/client/MqClientListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     4180 2024-05-22 11:43:44.000000 folkmq-1.5.0/folkmq/client/MqMessage.py
+-rw-r--r--   0 noear      (501) staff       (20)     3589 2024-05-22 11:46:21.000000 folkmq-1.5.0/folkmq/client/MqMessageReceived.py
+-rw-r--r--   0 noear      (501) staff       (20)     1094 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqRouter.py
+-rw-r--r--   0 noear      (501) staff       (20)      890 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqSubscription.py
+-rw-r--r--   0 noear      (501) staff       (20)     1073 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqTransaction.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.485794 folkmq-1.5.0/folkmq/common/
+-rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/MqApis.py
+-rw-r--r--   0 noear      (501) staff       (20)     1079 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/common/MqAssert.py
+-rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/MqConstants.py
+-rw-r--r--   0 noear      (501) staff       (20)     2636 2024-05-22 11:39:58.000000 folkmq-1.5.0/folkmq/common/MqMetasResolver.py
+-rw-r--r--   0 noear      (501) staff       (20)     5015 2024-05-22 11:48:43.000000 folkmq-1.5.0/folkmq/common/MqMetasResolverV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     5231 2024-05-22 11:48:43.000000 folkmq-1.5.0/folkmq/common/MqMetasResolverV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/MqMetasV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     1078 2024-05-22 11:38:28.000000 folkmq-1.5.0/folkmq/common/MqMetasV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      422 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/common/MqTopicHelper.py
+-rw-r--r--   0 noear      (501) staff       (20)     1184 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/common/MqUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.486954 folkmq-1.5.0/folkmq/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/exception/FolkmqException.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.487548 folkmq-1.5.0/folkmq.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      587 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       47 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/zip-safe
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-24 13:24:40.489428 folkmq-1.5.0/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      910 2024-05-24 11:16:43.000000 folkmq-1.5.0/setup.py
```

### Comparing `folkmq-1.4.6/folkmq/client/MqClient.py` & `folkmq-1.5.0/folkmq/client/MqClient.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/client/MqClientDefault.py` & `folkmq-1.5.0/folkmq/client/MqClientDefault.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/client/MqClientListener.py` & `folkmq-1.5.0/folkmq/client/MqClientListener.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     if s.is_valid():
                         s.send_alarm(m, "Client request handle error:" + e)
                     log.warning(f"Client request handle error, key={message.get_key()} \n{e_msg}")
                 except Exception as err:
                     err_msg = traceback.format_exc()
                     log.warning(f"Client request handle error, key={message.get_key()} \n{err_msg}")
         else:
-            subscription = self._client.getSubscription(message.getFullTopic(), message.get_consumer_group())
+            subscription = self._client.getSubscription(message.get_full_topic(), message.get_consumer_group())
 
             try:
                 if subscription is not None:
                     # 有订阅
                     subscription.consume(message)
                     if subscription.is_auto_ack():
                         self._client.reply(s, m, message, True, None)
```

### Comparing `folkmq-1.4.6/folkmq/client/MqMessage.py` & `folkmq-1.5.0/folkmq/client/MqMessage.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     @abstractmethod
     def is_transaction(self) -> bool: ...
 
     #是否有序
     @abstractmethod
     def is_sequence(self) -> bool: ...
 
+    # 是否广播
+    @abstractmethod
+    def is_broadcast(self) -> bool: ...
+
     #质量等级
     @abstractmethod
     def get_qos(self) -> int: ...
 
     #获取属性
     @abstractmethod
     def get_attr(self, name: str) -> str | None: ...
@@ -57,14 +61,15 @@
             self.__body = body
 
         self.__sender = None;
         self.__tag = None;
         self.__scheduled:datetime = None
         self.__expiration:datetime = None;
         self.__sequence:bool = False
+        self.__broadcast:bool = False
         self.__sequenceSharding: str | None = None
         self.__qos:int = 1
 
         self.__attrMap: dict[str, str] = {}
         self.__transaction:MqTransaction = None
 
     def get_sender(self) -> str | None:
@@ -84,14 +89,17 @@
 
     def get_expiration(self) -> datetime:
         return self.__expiration
 
     def is_transaction(self) -> bool:
         return self.__transaction is not None
 
+    def is_broadcast(self) -> bool:
+        return self.__broadcast
+
     def is_sequence(self) -> bool:
         return self.__sequence
 
     def getSequenceSharding(self)->str:
         return self.__sequenceSharding
 
     def get_qos(self) -> int:
@@ -121,14 +129,18 @@
         if sequence:
             if StrUtils.is_not_empty(sharding):
                 self.__sequenceSharding = sharding
         else:
             self.__sequenceSharding = None
         return self
 
+    def broadcast(self, broadcast: bool)-> 'MqMessage':
+        self.__broadcast = broadcast
+        return self
+
 
     def transaction(self, transaction: MqTransaction|None)-> 'MqMessage':
         if transaction is not None:
             self.__transaction = transaction
             transaction.binding(self)
 
         return self
```

### Comparing `folkmq-1.4.6/folkmq/client/MqMessageReceived.py` & `folkmq-1.5.0/folkmq/client/MqMessageReceived.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,88 +40,93 @@
     # 响应
     @abstractmethod
     def response(self, entity:Entity):
         ...
 
 class MqMessageReceivedImpl(MqMessageReceived):
     def __init__(self, clientInternal:'MqClientInternal', session:Session, source:Message):
-        self._clientInternal = clientInternal
-        self._session = session
-        self._source = source
+        self.__clientInternal = clientInternal
+        self.__session = session
+        self.__source = source
 
         mr  = MqUtils.get_of(source)
 
-        self._sender = mr.get_sender(source)
+        self.__sender = mr.get_sender(source)
 
-        self._key = mr.get_key(source)
-        self._tag = mr.get_tag(source)
-        self._fullTopic = mr.get_topic(source)
-        self._topic = MqTopicHelper.get_topic(self._fullTopic)
-        self._consumerGroup = mr.get_consumer_group(source)
-
-        self._qos = mr.get_qos(source)
-        self._times = mr.get_times(source)
-        self._sequence = mr.is_sequence(source)
-        self._transaction = mr.is_transaction(source)
+        self.__key = mr.get_key(source)
+        self.__tag = mr.get_tag(source)
+        self.__fullTopic = mr.get_topic(source)
+        self.__topic = MqTopicHelper.get_topic(self.__fullTopic)
+        self.__consumerGroup = mr.get_consumer_group(source)
+
+        self.__qos = mr.get_qos(source)
+        self.__times = mr.get_times(source)
+        self.__sequence = mr.is_sequence(source)
+        self.__broadcast = mr.is_broadcast(source)
+        self.__transaction = mr.is_transaction(source)
 
-        self._expirationL = mr.get_expiration(source)
-        self._expiration = self._expirationL
+        self.__expirationL = mr.get_expiration(source)
+        self.__expiration = self.__expirationL
 
     def getSource(self) -> Message:
-        return self._source
+        return self.__source
 
     def get_sender(self) -> str | None:
-        return self._sender
+        return self.__sender
 
     def get_key(self) -> str:
-        return self._key
+        return self.__key
 
     def get_tag(self) -> str:
-        return self._tag
+        return self.__tag
 
     def get_topic(self) -> str:
-        return self._topic
+        return self.__topic
 
-    def getFullTopic(self)->str:
-        return self._fullTopic
+    def get_full_topic(self)->str:
+        return self.__fullTopic
 
     def get_consumer_group(self) -> str:
-        return self._consumerGroup
+        return self.__consumerGroup
 
     def get_body(self) -> bytes:
-        return self._source.data_as_bytes()
+        return self.__source.data_as_bytes()
+
     def get_body_as_string(self) -> str:
-        return self._source.data_as_string()
+        return self.__source.data_as_string()
 
     def get_qos(self) -> int:
-        return self._qos
+        return self.__qos
 
     def get_attr(self, name: str) -> str | None:
-        return self._source.meta(MqConstants.MQ_ATTR_PREFIX + name)
+        return self.__source.meta(MqConstants.MQ_ATTR_PREFIX + name)
 
     def get_expiration(self) -> datetime | None:
-        return self._expiration
+        return self.__expiration
 
     def is_transaction(self) -> bool:
-        return self._transaction
+        return self.__transaction
 
     def is_sequence(self) -> bool:
-        return self._sequence
+        return self.__sequence
+
+    def is_broadcast(self) -> bool:
+        return self.__broadcast
 
     def get_times(self) -> int:
-        return self._times
+        return self.__times
 
     def acknowledge(self, isOk: bool):
-        self._clientInternal.reply(self._session, self._source, self, isOk, None)
+        self.__clientInternal.reply(self.__session, self.__source, self, isOk, None)
 
     def response(self, entity:Entity):
-        self._clientInternal.reply(self._session, self._source, self, True, entity)
+        self.__clientInternal.reply(self.__session, self.__source, self, True, entity)
 
     def __str__(self) ->str:
         return "MqMessageReceived{" + \
-            "key='" + self._key + '\'' + \
-            ", tag='" + self._tag + '\'' + \
-            ", topic='" + self._topic + '\'' + \
+            "key='" + self.__key + '\'' + \
+            ", tag='" + self.__tag + '\'' + \
+            ", topic='" + self.__topic + '\'' + \
             ", body='" + self.get_body_as_string() + '\'' + \
             '}'
```

### Comparing `folkmq-1.4.6/folkmq/client/MqRouter.py` & `folkmq-1.5.0/folkmq/client/MqRouter.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/client/MqSubscription.py` & `folkmq-1.5.0/folkmq/client/MqSubscription.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/client/MqTransaction.py` & `folkmq-1.5.0/folkmq/client/MqTransaction.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/common/MqAssert.py` & `folkmq-1.5.0/folkmq/common/MqAssert.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/common/MqConstants.py` & `folkmq-1.5.0/folkmq/common/MqConstants.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/common/MqMetasResolver.py` & `folkmq-1.5.0/folkmq/common/MqMetasResolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,20 @@
     #
     # 是否有序
     #
     @abc.abstractmethod
     def is_sequence(self, m: Entity)->bool:...
 
     #
+    # 是否广播
+    #
+    @abc.abstractmethod
+    def is_broadcast(self, m: Entity)->bool:...
+
+    #
     # 是否事务
     #
     @abc.abstractmethod
     def is_transaction(self, m: Entity)->bool:...
 
     #
     # 设置事务
```

### Comparing `folkmq-1.4.6/folkmq/common/MqMetasResolverV1.py` & `folkmq-1.5.0/folkmq/common/MqMetasResolverV1.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
     def set_scheduled(self, m: Entity, scheduled: int):
         m.put_meta(MqMetasV1.MQ_META_SCHEDULED, scheduled.toString())
 
     def is_sequence(self, m: Entity) -> bool:
         return "1" == (m.meta_or_default(MqMetasV1.MQ_META_SEQUENCE, "0"))
 
+    def is_broadcast(self, m: Entity) ->bool:
+        return "1" == (m.meta(MqMetasV2.MQ_META_BROADCAST))
+
     def is_transaction(self, m: Entity) -> bool:
         return "1" == (m.meta(MqMetasV2.MQ_META_TRANSACTION))
 
     def set_transaction(self, m: Entity, isTransaction: bool):
         m.put_meta(MqMetasV2.MQ_META_TRANSACTION, ( "1" if isTransaction else "0"))
 
     def publish_entity_build(self, topic: str, message: MqMessage) -> EntityDefault:
@@ -96,14 +99,16 @@
         if  message.is_transaction():
             entity.meta_put(MqMetasV2.MQ_META_TRANSACTION, "1")
 
 
         if message.get_sender():
             entity.meta_put(MqMetasV2.MQ_META_SENDER, message.get_sender())
 
+        if message.is_broadcast():
+            entity.meta_put(MqMetasV2.MQ_META_BROADCAST, "1")
 
         # 是否有序
         if  message.is_sequence() or message.is_transaction():
             entity.at(MqConstants.BROKER_AT_SERVER_HASH)
 
         if message.is_sequence():
             entity.meta_put(MqMetasV1.MQ_META_SEQUENCE, "1")
```

### Comparing `folkmq-1.4.6/folkmq/common/MqMetasResolverV2.py` & `folkmq-1.5.0/folkmq/common/MqMetasResolverV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
     def set_scheduled(self, m: Entity, scheduled: int):
         m.put_meta(MqMetasV2.MQ_META_SCHEDULED, str(scheduled))
 
     def is_sequence(self, m: Entity) -> bool:
         return "1" == (m.meta(MqMetasV2.MQ_META_SEQUENCE))
 
+    def is_broadcast(self, m: Entity) ->bool:
+        return "1" == (m.meta(MqMetasV2.MQ_META_BROADCAST))
+
     def is_transaction(self, m: Entity) -> bool:
         return "1" == (m.meta(MqMetasV2.MQ_META_TRANSACTION))
 
     def set_transaction(self, m: Entity, isTransaction: bool):
         m.put_meta(MqMetasV2.MQ_META_TRANSACTION, ("1" if isTransaction else "0"))
 
     def publish_entity_build(self, topic: str, message: MqMessage) -> EntityDefault:
@@ -93,14 +96,17 @@
 
         if message.is_transaction():
             entity.meta_put(MqMetasV2.MQ_META_TRANSACTION, "1")
 
         if message.get_sender():
             entity.meta_put(MqMetasV2.MQ_META_SENDER, message.get_sender())
 
+        if message.is_broadcast():
+            entity.meta_put(MqMetasV2.MQ_META_BROADCAST, "1")
+
         # 是否有序
         if message.is_sequence() or message.is_transaction():
             entity.at(MqConstants.BROKER_AT_SERVER_HASH)
             if message.is_sequence():
                 entity.meta_put(MqMetasV2.MQ_META_SEQUENCE, "1");
 
                 if message.is_transaction() == False and message.getSequenceSharding():
```

### Comparing `folkmq-1.4.6/folkmq/common/MqMetasV1.py` & `folkmq-1.5.0/folkmq/common/MqMetasV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq/common/MqMetasV2.py` & `folkmq-1.5.0/folkmq/common/MqMetasV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,19 @@
     MQ_META_SEQUENCE = "s2"
     #
     # 元信息：消息是否事务
     #
     MQ_META_TRANSACTION = "t4"
 
     #
+    # 元信息：消息是否广播
+    #
+    MQ_META_BROADCAST = "b0"
+
+    #
     # 元信息：消息质量等级
     #
     MQ_META_QOS = "q1"
     #
     # 元信息：派发次数
     #
     MQ_META_TIMES = "t2"
```

### Comparing `folkmq-1.4.6/folkmq/common/MqUtils.py` & `folkmq-1.5.0/folkmq/common/MqUtils.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/folkmq.egg-info/SOURCES.txt` & `folkmq-1.5.0/folkmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.6/setup.py` & `folkmq-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='folkmq',
-    version='1.4.6',
+    version='1.5.0',
     description='@noear/folkmq python project',
     author='noear',
     url='https://folkmq.noear.org/',
     packages=find_packages(exclude=['*folkmq-test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru>=0.7.2',
         'websockets>=12.0',
-        'socket.d>=2.4.18'
+        'socket.d>=2.5.1'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

