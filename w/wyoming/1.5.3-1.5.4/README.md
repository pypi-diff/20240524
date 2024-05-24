# Comparing `tmp/wyoming-1.5.3-py3-none-any.whl.zip` & `tmp/wyoming-1.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 26598 bytes, number of entries: 30
--rw-r--r--  2.0 unx        6 b- defN 24-Feb-18 19:46 wyoming/VERSION
+Zip file size: 27641 bytes, number of entries: 31
+-rw-r--r--  2.0 unx        6 b- defN 24-Feb-22 20:43 wyoming/VERSION
 -rw-r--r--  2.0 unx      189 b- defN 24-Jan-17 19:31 wyoming/__init__.py
 -rw-r--r--  2.0 unx     1765 b- defN 24-Feb-13 18:58 wyoming/asr.py
 -rw-r--r--  2.0 unx     8043 b- defN 24-Feb-13 21:07 wyoming/audio.py
 -rw-r--r--  2.0 unx     3571 b- defN 24-Feb-13 22:21 wyoming/client.py
 -rw-r--r--  2.0 unx      846 b- defN 24-Jan-15 20:48 wyoming/error.py
 -rw-r--r--  2.0 unx     5974 b- defN 24-Jan-17 19:30 wyoming/event.py
 -rw-r--r--  2.0 unx     4918 b- defN 24-Feb-13 19:54 wyoming/flycheck_server.py
@@ -13,20 +13,21 @@
 -rw-r--r--  2.0 unx     2543 b- defN 24-Jan-15 20:43 wyoming/mic.py
 -rw-r--r--  2.0 unx     1128 b- defN 24-Jan-15 17:07 wyoming/ping.py
 -rw-r--r--  2.0 unx     3960 b- defN 24-Feb-13 18:53 wyoming/pipeline.py
 -rw-r--r--  2.0 unx     7251 b- defN 24-Jan-08 22:38 wyoming/pyaudioop.py
 -rw-r--r--  2.0 unx     2866 b- defN 24-Jan-18 17:04 wyoming/satellite.py
 -rw-r--r--  2.0 unx     6831 b- defN 24-Feb-13 20:33 wyoming/server.py
 -rw-r--r--  2.0 unx     2818 b- defN 24-Jan-15 20:43 wyoming/snd.py
+-rw-r--r--  2.0 unx     3834 b- defN 24-May-24 20:31 wyoming/timer.py
 -rw-r--r--  2.0 unx     2039 b- defN 24-Jan-15 20:48 wyoming/tts.py
 -rw-r--r--  2.0 unx     1263 b- defN 23-Apr-21 15:28 wyoming/vad.py
 -rw-r--r--  2.0 unx      202 b- defN 24-Jan-17 19:30 wyoming/version.py
--rw-r--r--  2.0 unx     4452 b- defN 24-Jan-15 20:44 wyoming/wake.py
+-rw-r--r--  2.0 unx     4691 b- defN 24-Feb-22 20:45 wyoming/wake.py
 -rw-r--r--  2.0 unx      972 b- defN 23-Nov-28 21:27 wyoming/zeroconf.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 15:28 wyoming/util/__init__.py
 -rw-r--r--  2.0 unx     2352 b- defN 23-Jul-17 16:41 wyoming/util/dataclasses_json.py
--rw-r--r--  2.0 unx     1071 b- defN 24-Feb-18 21:17 wyoming-1.5.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      917 b- defN 24-Feb-18 21:17 wyoming-1.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-18 21:17 wyoming-1.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-18 21:17 wyoming-1.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2245 b- defN 24-Feb-18 21:17 wyoming-1.5.3.dist-info/RECORD
-30 files, 80062 bytes uncompressed, 23086 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-24 20:32 wyoming-1.5.4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      917 b- defN 24-May-24 20:32 wyoming-1.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 20:32 wyoming-1.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-24 20:32 wyoming-1.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2318 b- defN 24-May-24 20:32 wyoming-1.5.4.dist-info/RECORD
+31 files, 84208 bytes uncompressed, 24021 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -48,14 +48,17 @@
 
 Filename: wyoming/server.py
 Comment: 
 
 Filename: wyoming/snd.py
 Comment: 
 
+Filename: wyoming/timer.py
+Comment: 
+
 Filename: wyoming/tts.py
 Comment: 
 
 Filename: wyoming/vad.py
 Comment: 
 
 Filename: wyoming/version.py
@@ -69,23 +72,23 @@
 
 Filename: wyoming/util/__init__.py
 Comment: 
 
 Filename: wyoming/util/dataclasses_json.py
 Comment: 
 
-Filename: wyoming-1.5.3.dist-info/LICENSE.md
+Filename: wyoming-1.5.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: wyoming-1.5.3.dist-info/METADATA
+Filename: wyoming-1.5.4.dist-info/METADATA
 Comment: 
 
-Filename: wyoming-1.5.3.dist-info/WHEEL
+Filename: wyoming-1.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: wyoming-1.5.3.dist-info/top_level.txt
+Filename: wyoming-1.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: wyoming-1.5.3.dist-info/RECORD
+Filename: wyoming-1.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wyoming/VERSION

```diff
@@ -1 +1 @@
-1.5.3
+1.5.4
```

## wyoming/wake.py

```diff
@@ -24,27 +24,39 @@
 
     name: Optional[str] = None
     """Name of model."""
 
     timestamp: Optional[int] = None
     """Timestamp of audio chunk with detection"""
 
+    speaker: Optional[str] = None
+    """Name of speaker."""
+
     @staticmethod
     def is_type(event_type: str) -> bool:
         return event_type == _DETECTION_TYPE
 
     def event(self) -> Event:
         return Event(
-            type=_DETECTION_TYPE, data={"name": self.name, "timestamp": self.timestamp}
+            type=_DETECTION_TYPE,
+            data={
+                "name": self.name,
+                "timestamp": self.timestamp,
+                "speaker": self.speaker,
+            },
         )
 
     @staticmethod
     def from_event(event: Event) -> "Detection":
         data = event.data or {}
-        return Detection(name=data.get("name"), timestamp=data.get("timestamp"))
+        return Detection(
+            name=data.get("name"),
+            timestamp=data.get("timestamp"),
+            speaker=data.get("speaker"),
+        )
 
 
 @dataclass
 class Detect(Eventable):
     """Wake word detection request.
 
     Followed by AudioStart, AudioChunk+, AudioStop
```

## Comparing `wyoming-1.5.3.dist-info/LICENSE.md` & `wyoming-1.5.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `wyoming-1.5.3.dist-info/METADATA` & `wyoming-1.5.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming
-Version: 1.5.3
+Version: 1.5.4
 Summary: Protocol for Rhasspy Voice Assistant
 Home-page: http://github.com/rhasspy/wyoming
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: voice assistant rhasspy
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `wyoming-1.5.3.dist-info/RECORD` & `wyoming-1.5.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-wyoming/VERSION,sha256=wD44JAAfOblRgkm41lIkIvxN5yJ-EqVowBZGYrA7d1g,6
+wyoming/VERSION,sha256=h5pnoZdEZHnng8jiKlhoH-0yTwnqwc6Aj2paTF4YlK0,6
 wyoming/__init__.py,sha256=p-cYeg040x0TibrJcVxeeyHNY_1PXbyibol46xmpwM4,189
 wyoming/asr.py,sha256=4gKJtasvi3ZJwuiGyv_njgDCStM80ZPA7xRWDJuGuYc,1765
 wyoming/audio.py,sha256=a7AX2O5vte1DjlVDkZA7dAtvw5aw6dJQKmqgTxnKRk0,8043
 wyoming/client.py,sha256=abkZUO9myAISY8cQWPMYxx98MShT33kAGc9XeYuroV8,3571
 wyoming/error.py,sha256=g25kMr1JAYIuKS71vZSSqyaEfB33TB0kEVXKZqyG_bY,846
 wyoming/event.py,sha256=Qknb3btlmxA7BxDO7ujo3EO0C-H1LUATm7E5atSAEdc,5974
 wyoming/flycheck_server.py,sha256=cCvMvNXdIARfK5KHDWbR1VQOE2MP-_-gKbJdUzvT364,4918
@@ -12,19 +12,20 @@
 wyoming/mic.py,sha256=WSA0Jr7gup-J8JwTO2z2pKnCh5Y2SAGFmoPideGDZ5M,2543
 wyoming/ping.py,sha256=OAotqnfK9FReo5_HyoqyQpi6tp5yTzl7EjDmr5_0Eqs,1128
 wyoming/pipeline.py,sha256=1KvDBuT_B0F62Y8sPWMUNSii4QVl-E-o4ZwVMmCutQA,3960
 wyoming/pyaudioop.py,sha256=DcjmlRYxskTw-xVVh1o_UB4t7ppm5IJ-OgiqCDn9aVc,7251
 wyoming/satellite.py,sha256=veREt7XdfdLFW3ZcZK5T6yOPBvVR0blABwiBG7udOEY,2866
 wyoming/server.py,sha256=eCBtGU3LpgtdPMehv4GN03ne2rt8XAupy5KDYDPUt-k,6831
 wyoming/snd.py,sha256=s-CQSc9P8u-AOT4UVvuYXmB0SnVBNWPF3wU3GqbhznY,2818
+wyoming/timer.py,sha256=Fr3xO5bcjAvmCPZZInPLYJ1ohmBx5OK8ytUQnuM4Tp0,3834
 wyoming/tts.py,sha256=F7YG92bYSIxX0M2rKSk6B5CUJ2ipmfF-0O587pk7O8w,2039
 wyoming/vad.py,sha256=psaX1dESEzTEqXOxCXT4lPp-IlldNZoTr4-ghn1cgUM,1263
 wyoming/version.py,sha256=TSUei7OlOwinbct8_ZWS9pdLkJJcvenzZNhNWsVReuI,202
-wyoming/wake.py,sha256=MsspZyngkA3zgDt3ppUOhOi5jyit0eyg2N7zGKOBBgM,4452
+wyoming/wake.py,sha256=XLuZJyOP3BBK8TP3HS5oX8mT34YYOB1Qd2PFMko_QFE,4691
 wyoming/zeroconf.py,sha256=yefpBERm1kDdFZvdeX4t5KIV4M7JBOU_eFCZi6y3GYQ,972
 wyoming/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wyoming/util/dataclasses_json.py,sha256=oCBXlQcRD3ujVeXeZUOqT4nzfGO60ukMb7piCzUGHWk,2352
-wyoming-1.5.3.dist-info/LICENSE.md,sha256=E3RtUJ105V6iJl--8gS7fNv4SoMVsCB-mIMmy1Q4cCg,1071
-wyoming-1.5.3.dist-info/METADATA,sha256=s6_RCBxnLDAZHAlnRLNBESae_fJh-7bDx-ykmiHglwI,917
-wyoming-1.5.3.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-wyoming-1.5.3.dist-info/top_level.txt,sha256=jImZbopwrI3paHItk1qrym8GXgCdbj8bMLTORljczEA,8
-wyoming-1.5.3.dist-info/RECORD,,
+wyoming-1.5.4.dist-info/LICENSE.md,sha256=E3RtUJ105V6iJl--8gS7fNv4SoMVsCB-mIMmy1Q4cCg,1071
+wyoming-1.5.4.dist-info/METADATA,sha256=LFBVTFceMpDsfGHKJ1Q4Qy8O-qhuwSpo0NaTTG-_Pbs,917
+wyoming-1.5.4.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+wyoming-1.5.4.dist-info/top_level.txt,sha256=jImZbopwrI3paHItk1qrym8GXgCdbj8bMLTORljczEA,8
+wyoming-1.5.4.dist-info/RECORD,,
```

