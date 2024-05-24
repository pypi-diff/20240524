# Comparing `tmp/msoffcrypto_tool-5.4.0.tar.gz` & `tmp/msoffcrypto_tool-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msoffcrypto_tool-5.4.0.tar", max compression
+gzip compressed data, was "msoffcrypto_tool-5.4.1.tar", max compression
```

## Comparing `msoffcrypto_tool-5.4.0.tar` & `msoffcrypto_tool-5.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1062 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1705 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/NOTICE.txt
--rw-r--r--   0        0        0     9412 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/README.md
--rw-r--r--   0        0        0     2813 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/__init__.py
--rw-r--r--   0        0        0     3175 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/__main__.py
--rw-r--r--   0        0        0      555 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/format/__init__.py
--rw-r--r--   0        0        0      398 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/base.py
--rw-r--r--   0        0        0     1669 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/common.py
--rw-r--r--   0        0        0    15845 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/doc97.py
--rw-r--r--   0        0        0    12178 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/ooxml.py
--rw-r--r--   0        0        0    28423 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/ppt97.py
--rw-r--r--   0        0        0    19142 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/xls97.py
--rw-r--r--   0        0        0        0 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/container/__init__.py
--rw-r--r--   0        0        0    22252 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/container/ecma376_encrypted.py
--rw-r--r--   0        0        0    18589 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_agile.py
--rw-r--r--   0        0        0       62 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_extensible.py
--rw-r--r--   0        0        0     3922 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_standard.py
--rw-r--r--   0        0        0     3064 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4.py
--rw-r--r--   0        0        0     2512 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4_cryptoapi.py
--rw-r--r--   0        0        0     8016 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/xor_obfuscation.py
--rw-r--r--   0        0        0     1264 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/pyproject.toml
--rw-r--r--   0        0        0    10182 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     1705 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/NOTICE.txt
+-rw-r--r--   0        0        0     9412 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/README.md
+-rw-r--r--   0        0        0     2813 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/__init__.py
+-rw-r--r--   0        0        0     3136 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/__main__.py
+-rw-r--r--   0        0        0      555 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/__init__.py
+-rw-r--r--   0        0        0      415 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/base.py
+-rw-r--r--   0        0        0     2675 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/common.py
+-rw-r--r--   0        0        0    16371 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/doc97.py
+-rw-r--r--   0        0        0    12758 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/ooxml.py
+-rw-r--r--   0        0        0    28358 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/ppt97.py
+-rw-r--r--   0        0        0    18985 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/format/xls97.py
+-rw-r--r--   0        0        0        0 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/container/__init__.py
+-rw-r--r--   0        0        0    22252 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/container/ecma376_encrypted.py
+-rw-r--r--   0        0        0    18589 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/ecma376_agile.py
+-rw-r--r--   0        0        0       62 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/ecma376_extensible.py
+-rw-r--r--   0        0        0     3922 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/ecma376_standard.py
+-rw-r--r--   0        0        0     3064 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/rc4.py
+-rw-r--r--   0        0        0     2512 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/rc4_cryptoapi.py
+-rw-r--r--   0        0        0     8526 2024-05-24 19:51:05.045701 msoffcrypto_tool-5.4.1/msoffcrypto/method/xor_obfuscation.py
+-rw-r--r--   0        0        0     1264 2024-05-24 19:51:05.049701 msoffcrypto_tool-5.4.1/pyproject.toml
+-rw-r--r--   0        0        0    10182 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.4.1/PKG-INFO
```

### Comparing `msoffcrypto_tool-5.4.0/LICENSE.txt` & `msoffcrypto_tool-5.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/NOTICE.txt` & `msoffcrypto_tool-5.4.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/README.md` & `msoffcrypto_tool-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/__init__.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/__main__.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import print_function
-
 import argparse
 import getpass
 import logging
 import sys
 
 import olefile
```

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/exceptions/__init__.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/format/doc97.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/format/doc97.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from collections import namedtuple
 from struct import pack, unpack, unpack_from
 
 import olefile
 
 from msoffcrypto import exceptions
 from msoffcrypto.format import base
-from msoffcrypto.format.common import _parse_encryptionheader, _parse_encryptionverifier
+from msoffcrypto.format.common import _parse_header_RC4CryptoAPI
 from msoffcrypto.method.rc4 import DocumentRC4
 from msoffcrypto.method.rc4_cryptoapi import DocumentRC4CryptoAPI
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 FibBase = namedtuple(
@@ -165,15 +165,17 @@
         reserved6=reserved6,
     )
     return fibbase
 
 
 def _packFibBase(fibbase):
     setBit = lambda bits, i, v: (bits & ~(1 << i)) | (v << i)
-    setBitSlice = lambda bits, i, w, v: (bits & ~((2**w - 1) << i)) | ((v & (2**w - 1)) << i)
+    setBitSlice = lambda bits, i, w, v: (bits & ~((2**w - 1) << i)) | (
+        (v & (2**w - 1)) << i
+    )
 
     blob = io.BytesIO()
     buf = pack("<H", fibbase.wIdent)
     blob.write(buf)
 
     buf = pack("<H", fibbase.nFib)
     blob.write(buf)
@@ -254,33 +256,14 @@
         "salt": salt,
         "encryptedVerifier": encryptedVerifier,
         "encryptedVerifierHash": encryptedVerifierHash,
     }
     return info
 
 
-def _parse_header_RC4CryptoAPI(encryptionHeader):
-    flags = encryptionHeader.read(4)
-    (headerSize,) = unpack("<I", encryptionHeader.read(4))
-    logger.debug(headerSize)
-    blob = io.BytesIO(encryptionHeader.read(headerSize))
-    header = _parse_encryptionheader(blob)
-    logger.debug(header)
-    blob = io.BytesIO(encryptionHeader.read())
-    verifier = _parse_encryptionverifier(blob, "RC4")  # TODO: Fix (cf. ooxml.py)
-    logger.debug(verifier)
-    info = {
-        "salt": verifier["salt"],
-        "keySize": header["keySize"],
-        "encryptedVerifier": verifier["encryptedVerifier"],
-        "encryptedVerifierHash": verifier["encryptedVerifierHash"],
-    }
-    return info
-
-
 class Doc97File(base.BaseOfficeFile):
     """Return a MS-DOC file object.
 
     Examples:
         >>> with open("tests/inputs/rc4cryptoapi_password.doc", "rb") as f:
         ...     officefile = Doc97File(f)
         ...     officefile.load_key(password="Password1234_")
@@ -313,57 +296,82 @@
         self.info = Info(
             fib=fib,
             tablename=tablename,
         )
 
     def load_key(self, password=None):
         fib = self.info.fib
-        logger.debug("fEncrypted: {}, fObfuscation: {}".format(fib.base.fEncrypted, fib.base.fObfuscation))
+        logger.debug(
+            "fEncrypted: {}, fObfuscation: {}".format(
+                fib.base.fEncrypted, fib.base.fObfuscation
+            )
+        )
 
         if fib.base.fEncrypted == 1:
             if fib.base.fObfuscation == 1:  # Using XOR obfuscation
                 xor_obf_password_verifier = fib.base.IKey
                 logger.debug(hex(xor_obf_password_verifier))
             else:  # elif fib.base.fObfuscation == 0:
                 encryptionHeader_size = fib.base.IKey
-                logger.debug("encryptionHeader_size: {}".format(hex(encryptionHeader_size)))
+                logger.debug(
+                    "encryptionHeader_size: {}".format(hex(encryptionHeader_size))
+                )
                 with self.ole.openstream(self.info.tablename) as table:
-                    encryptionHeader = table  # TODO why create a 2nd reference to same stream?
+                    encryptionHeader = (
+                        table  # TODO why create a 2nd reference to same stream?
+                    )
                     encryptionVersionInfo = table.read(4)
                     vMajor, vMinor = unpack("<HH", encryptionVersionInfo)
                     logger.debug("Version: {} {}".format(vMajor, vMinor))
                     if vMajor == 0x0001 and vMinor == 0x0001:  # RC4
                         info = _parse_header_RC4(encryptionHeader)
-                        if DocumentRC4.verifypw(password, info["salt"], info["encryptedVerifier"], info["encryptedVerifierHash"]):
+                        if DocumentRC4.verifypw(
+                            password,
+                            info["salt"],
+                            info["encryptedVerifier"],
+                            info["encryptedVerifierHash"],
+                        ):
                             self.type = "rc4"
                             self.key = password
                             self.salt = info["salt"]
                         else:
-                            raise exceptions.InvalidKeyError("Failed to verify password")
-                    elif vMajor in [0x0002, 0x0003, 0x0004] and vMinor == 0x0002:  # RC4 CryptoAPI
+                            raise exceptions.InvalidKeyError(
+                                "Failed to verify password"
+                            )
+                    elif (
+                        vMajor in [0x0002, 0x0003, 0x0004] and vMinor == 0x0002
+                    ):  # RC4 CryptoAPI
                         info = _parse_header_RC4CryptoAPI(encryptionHeader)
                         if DocumentRC4CryptoAPI.verifypw(
-                            password, info["salt"], info["keySize"], info["encryptedVerifier"], info["encryptedVerifierHash"]
+                            password,
+                            info["salt"],
+                            info["keySize"],
+                            info["encryptedVerifier"],
+                            info["encryptedVerifierHash"],
                         ):
                             self.type = "rc4_cryptoapi"
                             self.key = password
                             self.salt = info["salt"]
                             self.keySize = info["keySize"]
                         else:
-                            raise exceptions.InvalidKeyError("Failed to verify password")
+                            raise exceptions.InvalidKeyError(
+                                "Failed to verify password"
+                            )
                     else:
-                        raise exceptions.DecryptionError("Unsupported encryption method")
+                        raise exceptions.DecryptionError(
+                            "Unsupported encryption method"
+                        )
         else:
             raise exceptions.DecryptionError("File is not encrypted")
 
-    def decrypt(self, ofile):
-        # fd, _ofile_path = tempfile.mkstemp()
+    def decrypt(self, outfile):
+        # fd, _outfile_path = tempfile.mkstemp()
 
-        # shutil.copyfile(os.path.realpath(self.file.name), _ofile_path)
-        # outole = olefile.OleFileIO(_ofile_path, write_mode=True)
+        # shutil.copyfile(os.path.realpath(self.file.name), _outfile_path)
+        # outole = olefile.OleFileIO(_outfile_path, write_mode=True)
 
         obuf1 = io.BytesIO()
         fibbase = FibBase(
             wIdent=self.info.fib.base.wIdent,
             nFib=self.info.fib.base.nFib,
             unused=self.info.fib.base.unused,
             lid=self.info.fib.base.lid,
@@ -408,57 +416,78 @@
             worddocument.seek(0)
             logger.debug(len(header))
             obuf1.write(header)
 
             if self.type == "rc4":
                 dec1 = DocumentRC4.decrypt(self.key, self.salt, worddocument)
             elif self.type == "rc4_cryptoapi":
-                dec1 = DocumentRC4CryptoAPI.decrypt(self.key, self.salt, self.keySize, worddocument)
+                dec1 = DocumentRC4CryptoAPI.decrypt(
+                    self.key, self.salt, self.keySize, worddocument
+                )
+            else:
+                raise exceptions.DecryptionError(
+                    "Unsupported encryption method: {}".format(self.type)
+                )
+
             dec1.seek(FIB_LENGTH)
             obuf1.write(dec1.read())
             obuf1.seek(0)
 
         # TODO: Preserve header
         obuf2 = io.BytesIO()
+
         if self.type == "rc4":
             with self.ole.openstream(self.info.tablename) as stream:
                 dec2 = DocumentRC4.decrypt(self.key, self.salt, stream)
         elif self.type == "rc4_cryptoapi":
             with self.ole.openstream(self.info.tablename) as stream:
-                dec2 = DocumentRC4CryptoAPI.decrypt(self.key, self.salt, self.keySize, stream)
+                dec2 = DocumentRC4CryptoAPI.decrypt(
+                    self.key, self.salt, self.keySize, stream
+                )
+        else:
+            raise exceptions.DecryptionError(
+                "Unsupported encryption method: {}".format(self.type)
+            )
+
         obuf2.write(dec2.read())
         obuf2.seek(0)
 
         obuf3 = None
         if self.ole.exists("Data"):
             obuf3 = io.BytesIO()
             if self.type == "rc4":
                 with self.ole.openstream("Data") as data_stream:
                     dec3 = DocumentRC4.decrypt(self.key, self.salt, data_stream)
             elif self.type == "rc4_cryptoapi":
                 with self.ole.openstream("Data") as data_stream:
-                    dec3 = DocumentRC4CryptoAPI.decrypt(self.key, self.salt, self.keySize, data_stream)
+                    dec3 = DocumentRC4CryptoAPI.decrypt(
+                        self.key, self.salt, self.keySize, data_stream
+                    )
+            else:
+                raise exceptions.DecryptionError(
+                    "Unsupported encryption method: {}".format(self.type)
+                )
             obuf3.write(dec3.read())
             obuf3.seek(0)
 
-        with tempfile.TemporaryFile() as _ofile:
+        with tempfile.TemporaryFile() as _outfile:
             self.file.seek(0)
-            shutil.copyfileobj(self.file, _ofile)
-            outole = olefile.OleFileIO(_ofile, write_mode=True)
+            shutil.copyfileobj(self.file, _outfile)
+            outole = olefile.OleFileIO(_outfile, write_mode=True)
 
             outole.write_stream("wordDocument", obuf1.read())
             outole.write_stream(self.info.tablename, obuf2.read())
             if obuf3:
                 outole.write_stream("Data", obuf3.read())
 
-            # _ofile = open(_ofile_path, 'rb')
+            # _outfile = open(_outfile_path, 'rb')
 
-            _ofile.seek(0)
+            _outfile.seek(0)
 
-            shutil.copyfileobj(_ofile, ofile)
+            shutil.copyfileobj(_outfile, outfile)
 
     def is_encrypted(self):
         r"""
         Test if the file is encrypted.
 
             >>> f = open("tests/inputs/plain.doc", "rb")
             >>> file = Doc97File(f)
```

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/format/ooxml.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/format/ooxml.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     try:
         zfile = zipfile.ZipFile(file)
         with zfile.open("[Content_Types].xml") as stream:
             xml = parseString(stream.read())
             # Heuristic
             if (
                 xml.documentElement.tagName == "Types"
-                and xml.documentElement.namespaceURI == "http://schemas.openxmlformats.org/package/2006/content-types"
+                and xml.documentElement.namespaceURI
+                == "http://schemas.openxmlformats.org/package/2006/content-types"
             ):
                 return True
             else:
                 return False
-    except:
+    except Exception:
         return False
 
 
 def _parseinfo_standard(ole):
     (headerFlags,) = unpack("<I", ole.read(4))
     (encryptionHeaderSize,) = unpack("<I", ole.read(4))
     block = ole.read(encryptionHeaderSize)
@@ -45,35 +46,55 @@
     block = ole.read()
     blob = io.BytesIO(block)
     algIdMap = {
         0x0000660E: "AES-128",
         0x0000660F: "AES-192",
         0x00006610: "AES-256",
     }
-    verifier = _parse_encryptionverifier(blob, "AES" if header["algId"] & 0xFF00 == 0x6600 else "RC4")  # TODO: Fix
+    verifier = _parse_encryptionverifier(
+        blob, "AES" if header["algId"] & 0xFF00 == 0x6600 else "RC4"
+    )  # TODO: Fix
     info = {
         "header": header,
         "verifier": verifier,
     }
     return info
 
 
 def _parseinfo_agile(ole):
     ole.seek(8)
     xml = parseString(ole.read())
-    keyDataSalt = base64.b64decode(xml.getElementsByTagName("keyData")[0].getAttribute("saltValue"))
-    keyDataHashAlgorithm = xml.getElementsByTagName("keyData")[0].getAttribute("hashAlgorithm")
-    keyDataBlockSize = int(xml.getElementsByTagName("keyData")[0].getAttribute("blockSize"))
-    encryptedHmacKey = base64.b64decode(xml.getElementsByTagName("dataIntegrity")[0].getAttribute("encryptedHmacKey"))
-    encryptedHmacValue = base64.b64decode(xml.getElementsByTagName("dataIntegrity")[0].getAttribute("encryptedHmacValue"))
-    password_node = xml.getElementsByTagNameNS("http://schemas.microsoft.com/office/2006/keyEncryptor/password", "encryptedKey")[0]
+    keyDataSalt = base64.b64decode(
+        xml.getElementsByTagName("keyData")[0].getAttribute("saltValue")
+    )
+    keyDataHashAlgorithm = xml.getElementsByTagName("keyData")[0].getAttribute(
+        "hashAlgorithm"
+    )
+    keyDataBlockSize = int(
+        xml.getElementsByTagName("keyData")[0].getAttribute("blockSize")
+    )
+    encryptedHmacKey = base64.b64decode(
+        xml.getElementsByTagName("dataIntegrity")[0].getAttribute("encryptedHmacKey")
+    )
+    encryptedHmacValue = base64.b64decode(
+        xml.getElementsByTagName("dataIntegrity")[0].getAttribute("encryptedHmacValue")
+    )
+    password_node = xml.getElementsByTagNameNS(
+        "http://schemas.microsoft.com/office/2006/keyEncryptor/password", "encryptedKey"
+    )[0]
     spinValue = int(password_node.getAttribute("spinCount"))
-    encryptedKeyValue = base64.b64decode(password_node.getAttribute("encryptedKeyValue"))
-    encryptedVerifierHashInput = base64.b64decode(password_node.getAttribute("encryptedVerifierHashInput"))
-    encryptedVerifierHashValue = base64.b64decode(password_node.getAttribute("encryptedVerifierHashValue"))
+    encryptedKeyValue = base64.b64decode(
+        password_node.getAttribute("encryptedKeyValue")
+    )
+    encryptedVerifierHashInput = base64.b64decode(
+        password_node.getAttribute("encryptedVerifierHashInput")
+    )
+    encryptedVerifierHashValue = base64.b64decode(
+        password_node.getAttribute("encryptedVerifierHashValue")
+    )
     passwordSalt = base64.b64decode(password_node.getAttribute("saltValue"))
     passwordHashAlgorithm = password_node.getAttribute("hashAlgorithm")
     passwordKeyBits = int(password_node.getAttribute("keyBits"))
     info = {
         "keyDataSalt": keyDataSalt,
         "keyDataHashAlgorithm": keyDataHashAlgorithm,
         "keyDataBlockSize": keyDataBlockSize,
@@ -93,16 +114,20 @@
 def _parseinfo(ole):
     versionMajor, versionMinor = unpack("<HH", ole.read(4))
     if versionMajor == 4 and versionMinor == 4:  # Agile
         return "agile", _parseinfo_agile(ole)
     elif versionMajor in [2, 3, 4] and versionMinor == 2:  # Standard
         return "standard", _parseinfo_standard(ole)
     elif versionMajor in [3, 4] and versionMinor == 3:  # Extensible
-        raise exceptions.DecryptionError("Unsupported EncryptionInfo version (Extensible Encryption)")
-    raise exceptions.DecryptionError("Unsupported EncryptionInfo version ({}:{})".format(versionMajor, versionMinor))
+        raise exceptions.DecryptionError(
+            "Unsupported EncryptionInfo version (Extensible Encryption)"
+        )
+    raise exceptions.DecryptionError(
+        "Unsupported EncryptionInfo version ({}:{})".format(versionMajor, versionMinor)
+    )
 
 
 class OOXMLFile(base.BaseOfficeFile):
     """Return an OOXML file object.
 
     Examples:
         >>> with open("tests/inputs/example_password.docx", "rb") as f:
@@ -128,15 +153,17 @@
             ole = olefile.OleFileIO(file)
             self.file = ole
 
             try:
                 with self.file.openstream("EncryptionInfo") as stream:
                     self.type, self.info = _parseinfo(stream)
             except IOError:
-                raise exceptions.FileFormatError("Supposed to be an encrypted OOXML file, but no EncryptionInfo stream found")
+                raise exceptions.FileFormatError(
+                    "Supposed to be an encrypted OOXML file, but no EncryptionInfo stream found"
+                )
 
             logger.debug("OOXMLFile.type: {}".format(self.type))
 
             self.secret_key = None
 
             if self.type == "agile":
                 # TODO: Support aliases?
@@ -147,15 +174,17 @@
                 pass
         elif _is_ooxml(file):
             self.type = "plain"
             self.file = file
         else:
             raise exceptions.FileFormatError("Unsupported file format")
 
-    def load_key(self, password=None, private_key=None, secret_key=None, verify_password=False):
+    def load_key(
+        self, password=None, private_key=None, secret_key=None, verify_password=False
+    ):
         """
         >>> with open("tests/outputs/ecma376standard_password_plain.docx", "rb") as f:
         ...     officefile = OOXMLFile(f)
         ...     officefile.load_key("1234")
         """
         if password:
             if self.type == "agile":
@@ -187,40 +216,46 @@
                     self.info["header"]["providerType"],
                     self.info["header"]["keySize"],
                     self.info["verifier"]["saltSize"],
                     self.info["verifier"]["salt"],
                 )
                 if verify_password:
                     verified = ECMA376Standard.verifykey(
-                        self.secret_key, self.info["verifier"]["encryptedVerifier"], self.info["verifier"]["encryptedVerifierHash"]
+                        self.secret_key,
+                        self.info["verifier"]["encryptedVerifier"],
+                        self.info["verifier"]["encryptedVerifierHash"],
                     )
                     if not verified:
                         raise exceptions.InvalidKeyError("Key verification failed")
             elif self.type == "extensible":
                 pass
             elif self.type == "plain":
                 pass
         elif private_key:
             if self.type == "agile":
-                self.secret_key = ECMA376Agile.makekey_from_privkey(private_key, self.info["encryptedKeyValue"])
+                self.secret_key = ECMA376Agile.makekey_from_privkey(
+                    private_key, self.info["encryptedKeyValue"]
+                )
             else:
-                raise exceptions.DecryptionError("Unsupported key type for the encryption method")
+                raise exceptions.DecryptionError(
+                    "Unsupported key type for the encryption method"
+                )
         elif secret_key:
             self.secret_key = secret_key
         else:
             raise exceptions.DecryptionError("No key specified")
 
-    def decrypt(self, ofile, verify_integrity=False):
+    def decrypt(self, outfile, verify_integrity=False):
         """
         >>> from msoffcrypto import exceptions
-        >>> from io import BytesIO; ofile = BytesIO()
+        >>> from io import BytesIO; outfile = BytesIO()
         >>> with open("tests/outputs/ecma376standard_password_plain.docx", "rb") as f:
         ...     officefile = OOXMLFile(f)
         ...     officefile.load_key("1234")
-        ...     officefile.decrypt(ofile)
+        ...     officefile.decrypt(outfile)
         Traceback (most recent call last):
         msoffcrypto.exceptions.DecryptionError: Unencrypted document
         """
         if self.type == "agile":
             with self.file.openstream("EncryptedPackage") as stream:
                 if verify_integrity:
                     verified = ECMA376Agile.verify_integrity(
@@ -229,50 +264,59 @@
                         self.info["keyDataHashAlgorithm"],
                         self.info["keyDataBlockSize"],
                         self.info["encryptedHmacKey"],
                         self.info["encryptedHmacValue"],
                         stream,
                     )
                     if not verified:
-                        raise exceptions.InvalidKeyError("Payload integrity verification failed")
-
-                obuf = ECMA376Agile.decrypt(self.secret_key, self.info["keyDataSalt"], self.info["keyDataHashAlgorithm"], stream)
-            ofile.write(obuf)
+                        raise exceptions.InvalidKeyError(
+                            "Payload integrity verification failed"
+                        )
+
+                obuf = ECMA376Agile.decrypt(
+                    self.secret_key,
+                    self.info["keyDataSalt"],
+                    self.info["keyDataHashAlgorithm"],
+                    stream,
+                )
+            outfile.write(obuf)
         elif self.type == "standard":
             with self.file.openstream("EncryptedPackage") as stream:
                 obuf = ECMA376Standard.decrypt(self.secret_key, stream)
-            ofile.write(obuf)
+            outfile.write(obuf)
         elif self.type == "plain":
             raise exceptions.DecryptionError("Unencrypted document")
         else:
             raise exceptions.DecryptionError("Unsupported encryption method")
 
         # If the file is successfully decrypted, there must be a valid OOXML file, i.e. a valid zip file
         if not zipfile.is_zipfile(io.BytesIO(obuf)):
-            raise exceptions.InvalidKeyError("The file could not be decrypted with this password")
+            raise exceptions.InvalidKeyError(
+                "The file could not be decrypted with this password"
+            )
 
-    def encrypt(self, password, ofile):
+    def encrypt(self, password, outfile):
         """
         >>> from msoffcrypto.format.ooxml import OOXMLFile
-        >>> from io import BytesIO; ofile = BytesIO()
+        >>> from io import BytesIO; outfile = BytesIO()
         >>> with open("tests/outputs/example.docx", "rb") as f:
         ...     officefile = OOXMLFile(f)
-        ...     officefile.encrypt("1234", ofile)
+        ...     officefile.encrypt("1234", outfile)
         """
         if self.is_encrypted():
             raise exceptions.EncryptionError("File is already encrypted")
 
         self.file.seek(0)
 
         buf = ECMA376Agile.encrypt(password, self.file)
 
         if not olefile.isOleFile(buf):
             raise exceptions.EncryptionError("Unable to encrypt this file")
 
-        ofile.write(buf)
+        outfile.write(buf)
 
     def is_encrypted(self):
         """
         >>> with open("tests/inputs/example_password.docx", "rb") as f:
         ...     officefile = OOXMLFile(f)
         ...     officefile.is_encrypted()
         True
```

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/format/ppt97.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/format/ppt97.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from collections import namedtuple
 from struct import pack, unpack
 
 import olefile
 
 from msoffcrypto import exceptions
 from msoffcrypto.format import base
-from msoffcrypto.format.common import _parse_encryptionheader, _parse_encryptionverifier
+from msoffcrypto.format.common import _parse_header_RC4CryptoAPI
 from msoffcrypto.method.rc4_cryptoapi import DocumentRC4CryptoAPI
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 RecordHeader = namedtuple(
@@ -47,15 +47,17 @@
         recLen=recLen,
     )
 
     return rh
 
 
 def _packRecordHeader(rh):
-    setBitSlice = lambda bits, i, w, v: (bits & ~((2**w - 1) << i)) | ((v & (2**w - 1)) << i)
+    setBitSlice = lambda bits, i, w, v: (bits & ~((2**w - 1) << i)) | (
+        (v & (2**w - 1)) << i
+    )
 
     blob = io.BytesIO()
 
     _buf = 0xFFFF
     _buf = setBitSlice(_buf, 0, 4, rh.recVer)
     _buf = setBitSlice(_buf, 4, 12, rh.recInstance)
     buf = pack("<H", _buf)
@@ -223,15 +225,17 @@
     rh = _parseRecordHeader(buf)
     # logger.debug(rh)
 
     # ...Sub-fields are further specified in the following table.
     assert rh.recVer == 0x0
     assert rh.recInstance == 0x000
     assert rh.recType == 0x0FF5
-    assert rh.recLen == 0x0000001C or rh.recLen == 0x00000020  # 0x0000001c + len(encryptSessionPersistIdRef)
+    assert (
+        rh.recLen == 0x0000001C or rh.recLen == 0x00000020
+    )  # 0x0000001c + len(encryptSessionPersistIdRef)
 
     (lastSlideIdRef,) = unpack("<I", blob.read(4))
     (version,) = unpack("<H", blob.read(2))
     (
         minorVersion,
         majorVersion,
     ) = unpack("<BB", blob.read(2))
@@ -336,15 +340,17 @@
         persistId=persistId,
         cPersist=cPersist,
         rgPersistOffset=rgPersistOffset,
     )
 
 
 def _packPersistDirectoryEntry(directoryentry):
-    setBitSlice = lambda bits, i, w, v: (bits & ~((2**w - 1) << i)) | ((v & (2**w - 1)) << i)
+    setBitSlice = lambda bits, i, w, v: (bits & ~((2**w - 1) << i)) | (
+        (v & (2**w - 1)) << i
+    )
 
     blob = io.BytesIO()
 
     _buf = 0xFFFFFFFF
     _buf = setBitSlice(_buf, 0, 20, directoryentry.persistId)
     _buf = setBitSlice(_buf, 20, 12, directoryentry.cPersist)
     buf = pack("<I", _buf)
@@ -498,33 +504,14 @@
             # logger.debug("persistId: %d" % entry.persistId)
             for i, offset in enumerate(entry.rgPersistOffset):
                 persistobjectdirectory[entry.persistId + i] = offset
 
     return persistobjectdirectory
 
 
-def _parse_header_RC4CryptoAPI(encryptionInfo):
-    flags = encryptionInfo.read(4)
-    (headerSize,) = unpack("<I", encryptionInfo.read(4))
-    logger.debug(headerSize)
-    blob = io.BytesIO(encryptionInfo.read(headerSize))
-    header = _parse_encryptionheader(blob)
-    logger.debug(header)
-    blob = io.BytesIO(encryptionInfo.read())
-    verifier = _parse_encryptionverifier(blob, "RC4")  # TODO: Fix (cf. ooxml.py)
-    logger.debug(verifier)
-    info = {
-        "salt": verifier["salt"],
-        "keySize": header["keySize"],
-        "encryptedVerifier": verifier["encryptedVerifier"],
-        "encryptedVerifierHash": verifier["encryptedVerifierHash"],
-    }
-    return info
-
-
 class Ppt97File(base.BaseOfficeFile):
     """Return a MS-PPT file object.
 
     Examples:
         >>> with open("tests/inputs/rc4cryptoapi_password.ppt", "rb") as f:
         ...     officefile = Ppt97File(f)
         ...     officefile.load_key(password="Password1234_")
@@ -568,44 +555,60 @@
         persistobjectdirectory = construct_persistobjectdirectory(self.data)
         logger.debug("[*] persistobjectdirectory: {}".format(persistobjectdirectory))
 
         self.data.currentuser.seek(0)
         currentuser = _parseCurrentUser(self.data.currentuser)
         logger.debug("[*] currentuser: {}".format(currentuser))
 
-        self.data.powerpointdocument.seek(currentuser.currentuseratom.offsetToCurrentEdit)
+        self.data.powerpointdocument.seek(
+            currentuser.currentuseratom.offsetToCurrentEdit
+        )
         usereditatom = _parseUserEditAtom(self.data.powerpointdocument)
         logger.debug("[*] usereditatom: {}".format(usereditatom))
 
         # cf. Part 2 in https://docs.microsoft.com/en-us/openspecs/office_file_formats/ms-ppt/1fc22d56-28f9-4818-bd45-67c2bf721ccf
-        cryptsession10container_offset = persistobjectdirectory[usereditatom.encryptSessionPersistIdRef]
-        logger.debug("[*] cryptsession10container_offset: {}".format(cryptsession10container_offset))
+        cryptsession10container_offset = persistobjectdirectory[
+            usereditatom.encryptSessionPersistIdRef
+        ]
+        logger.debug(
+            "[*] cryptsession10container_offset: {}".format(
+                cryptsession10container_offset
+            )
+        )
 
         self.data.powerpointdocument.seek(cryptsession10container_offset)
-        cryptsession10container = _parseCryptSession10Container(self.data.powerpointdocument)
+        cryptsession10container = _parseCryptSession10Container(
+            self.data.powerpointdocument
+        )
         logger.debug("[*] cryptsession10container: {}".format(cryptsession10container))
 
         encryptionInfo = io.BytesIO(cryptsession10container.data)
 
         encryptionVersionInfo = encryptionInfo.read(4)
         vMajor, vMinor = unpack("<HH", encryptionVersionInfo)
         logger.debug("[*] encryption version: {} {}".format(vMajor, vMinor))
 
         assert vMajor in [0x0002, 0x0003, 0x0004] and vMinor == 0x0002  # RC4 CryptoAPI
 
         info = _parse_header_RC4CryptoAPI(encryptionInfo)
-        if DocumentRC4CryptoAPI.verifypw(password, info["salt"], info["keySize"], info["encryptedVerifier"], info["encryptedVerifierHash"]):
+        if DocumentRC4CryptoAPI.verifypw(
+            password,
+            info["salt"],
+            info["keySize"],
+            info["encryptedVerifier"],
+            info["encryptedVerifierHash"],
+        ):
             self.type = "rc4_cryptoapi"
             self.key = password
             self.salt = info["salt"]
             self.keySize = info["keySize"]
         else:
             raise exceptions.InvalidKeyError("Failed to verify password")
 
-    def decrypt(self, ofile):
+    def decrypt(self, outfile):
         # Current User Stream
         self.data.currentuser.seek(0)
         currentuser = _parseCurrentUser(self.data.currentuser)
         # logger.debug(currentuser)
 
         cuatom = currentuser.currentuseratom
 
@@ -640,18 +643,22 @@
         powerpointdocument_size = len(self.data.powerpointdocument.read())
         logger.debug("[*] powerpointdocument_size: {}".format(powerpointdocument_size))
 
         self.data.powerpointdocument.seek(0)
         dec_bytearray = bytearray(self.data.powerpointdocument.read())
 
         # UserEditAtom
-        self.data.powerpointdocument.seek(currentuser.currentuseratom.offsetToCurrentEdit)
+        self.data.powerpointdocument.seek(
+            currentuser.currentuseratom.offsetToCurrentEdit
+        )
         # currentuseratom_raw = self.data.powerpointdocument.read(40)
 
-        self.data.powerpointdocument.seek(currentuser.currentuseratom.offsetToCurrentEdit)
+        self.data.powerpointdocument.seek(
+            currentuser.currentuseratom.offsetToCurrentEdit
+        )
         usereditatom = _parseUserEditAtom(self.data.powerpointdocument)
         # logger.debug(usereditatom)
         # logger.debug(["offsetToCurrentEdit", currentuser.currentuseratom.offsetToCurrentEdit])
 
         rh_new = RecordHeader(
             recVer=usereditatom.rh.recVer,
             recInstance=usereditatom.rh.recInstance,
@@ -683,30 +690,34 @@
         buf = _packUserEditAtom(usereditatom_new)
         buf.seek(0)
         buf_bytes = bytearray(buf.read())
         offset = currentuser.currentuseratom.offsetToCurrentEdit
         dec_bytearray[offset : offset + len(buf_bytes)] = buf_bytes
 
         # PersistDirectoryAtom
-        self.data.powerpointdocument.seek(currentuser.currentuseratom.offsetToCurrentEdit)
+        self.data.powerpointdocument.seek(
+            currentuser.currentuseratom.offsetToCurrentEdit
+        )
         usereditatom = _parseUserEditAtom(self.data.powerpointdocument)
         # logger.debug(usereditatom)
 
         self.data.powerpointdocument.seek(usereditatom.offsetPersistDirectory)
         persistdirectoryatom = _parsePersistDirectoryAtom(self.data.powerpointdocument)
         # logger.debug(persistdirectoryatom)
 
         persistdirectoryatom_new = PersistDirectoryAtom(
             rh=persistdirectoryatom.rh,
             rgPersistDirEntry=[
                 PersistDirectoryEntry(
                     persistId=persistdirectoryatom.rgPersistDirEntry[0].persistId,
                     # Omit CryptSession10Container
                     cPersist=persistdirectoryatom.rgPersistDirEntry[0].cPersist - 1,
-                    rgPersistOffset=persistdirectoryatom.rgPersistDirEntry[0].rgPersistOffset,
+                    rgPersistOffset=persistdirectoryatom.rgPersistDirEntry[
+                        0
+                    ].rgPersistOffset,
                 ),
             ],
         )
 
         self.data.powerpointdocument.seek(usereditatom.offsetPersistDirectory)
         buf = _packPersistDirectoryAtom(persistdirectoryatom_new)
         buf_bytes = bytearray(buf.read())
@@ -725,63 +736,80 @@
             rh = _parseRecordHeader(io.BytesIO(buf))
             logger.debug("[*] rh: {}".format(rh))
 
             # CryptSession10Container
             if rh.recType == 0x2F14:
                 logger.debug("[*] CryptSession10Container found")
                 # Remove encryption, pad by zero to preserve stream size
-                dec_bytearray[offset : offset + (8 + rh.recLen)] = b"\x00" * (8 + rh.recLen)
+                dec_bytearray[offset : offset + (8 + rh.recLen)] = b"\x00" * (
+                    8 + rh.recLen
+                )
                 continue
 
             # The UserEditAtom record (section 2.3.3) and the PersistDirectoryAtom record (section 2.3.4) MUST NOT be encrypted.
             if rh.recType in [0x0FF5, 0x1772]:
                 logger.debug("[*] UserEditAtom/PersistDirectoryAtom found")
                 continue
 
             # TODO: Fix here
             recLen = directory_items[i + 1][1] - offset - 8
             logger.debug("[*] recLen: {}".format(recLen))
 
             self.data.powerpointdocument.seek(offset)
             enc_buf = io.BytesIO(self.data.powerpointdocument.read(8 + recLen))
-            blocksize = self.keySize * ((8 + recLen) // self.keySize + 1)  # Undocumented
-            dec = DocumentRC4CryptoAPI.decrypt(self.key, self.salt, self.keySize, enc_buf, blocksize=blocksize, block=persistId)
+            blocksize = self.keySize * (
+                (8 + recLen) // self.keySize + 1
+            )  # Undocumented
+            dec = DocumentRC4CryptoAPI.decrypt(
+                self.key,
+                self.salt,
+                self.keySize,
+                enc_buf,
+                blocksize=blocksize,
+                block=persistId,
+            )
             dec_bytes = bytearray(dec.read())
             dec_bytearray[offset : offset + len(dec_bytes)] = dec_bytes
 
         # To BytesIO
         dec_buf = io.BytesIO(dec_bytearray)
 
         dec_buf.seek(0)
         for i, (persistId, offset) in enumerate(directory_items):
             dec_buf.seek(offset)
             buf = dec_buf.read(8)
             rh = _parseRecordHeader(io.BytesIO(buf))
             logger.debug("[*] rh: {}".format(rh))
 
         dec_buf.seek(0)
-        logger.debug("[*] powerpointdocument_size={}, len(dec_buf.read())={}".format(powerpointdocument_size, len(dec_buf.read())))
+        logger.debug(
+            "[*] powerpointdocument_size={}, len(dec_buf.read())={}".format(
+                powerpointdocument_size, len(dec_buf.read())
+            )
+        )
 
         dec_buf.seek(0)
         powerpointdocument_dec_buf = dec_buf
 
         # TODO: Pictures Stream
         # TODO: Encrypted Summary Info Stream
 
-        with tempfile.TemporaryFile() as _ofile:
+        with tempfile.TemporaryFile() as _outfile:
             self.file.seek(0)
-            shutil.copyfileobj(self.file, _ofile)
-            outole = olefile.OleFileIO(_ofile, write_mode=True)
+            shutil.copyfileobj(self.file, _outfile)
+            outole = olefile.OleFileIO(_outfile, write_mode=True)
 
             outole.write_stream("Current User", currentuser_buf.read())
-            outole.write_stream("PowerPoint Document", powerpointdocument_dec_buf.read())
+            outole.write_stream(
+                "PowerPoint Document", powerpointdocument_dec_buf.read()
+            )
 
             # Finalize
-            _ofile.seek(0)
-            shutil.copyfileobj(_ofile, ofile)
+            _outfile.seek(0)
+            shutil.copyfileobj(_outfile, outfile)
 
         return
 
     def is_encrypted(self):
         r"""
         Test if the file is encrypted.
 
@@ -794,15 +822,17 @@
             >>> file.is_encrypted()
             True
         """
         self.data.currentuser.seek(0)
         currentuser = _parseCurrentUser(self.data.currentuser)
         logger.debug("[*] currentuser: {}".format(currentuser))
 
-        self.data.powerpointdocument.seek(currentuser.currentuseratom.offsetToCurrentEdit)
+        self.data.powerpointdocument.seek(
+            currentuser.currentuseratom.offsetToCurrentEdit
+        )
         usereditatom = _parseUserEditAtom(self.data.powerpointdocument)
         logger.debug("[*] usereditatom: {}".format(usereditatom))
 
         if usereditatom.rh.recLen == 0x00000020:  # Cf. _parseUserEditAtom
             return True
         else:
             return False
```

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/format/xls97.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/format/xls97.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import logging, io, shutil, tempfile
-from struct import pack, unpack
+import io
+import logging
+import shutil
+import tempfile
 from collections import namedtuple
+from struct import pack, unpack
 
 import olefile
 
 from msoffcrypto import exceptions
 from msoffcrypto.format import base
-from msoffcrypto.format.common import _parse_encryptionheader, _parse_encryptionverifier
+from msoffcrypto.format.common import _parse_header_RC4CryptoAPI
 from msoffcrypto.method.rc4 import DocumentRC4
 from msoffcrypto.method.rc4_cryptoapi import DocumentRC4CryptoAPI
 from msoffcrypto.method.xor_obfuscation import DocumentXOR
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
@@ -382,33 +385,14 @@
         "salt": salt,
         "encryptedVerifier": encryptedVerifier,
         "encryptedVerifierHash": encryptedVerifierHash,
     }
     return info
 
 
-def _parse_header_RC4CryptoAPI(encryptionInfo):
-    flags = encryptionInfo.read(4)
-    (headerSize,) = unpack("<I", encryptionInfo.read(4))
-    logger.debug(headerSize)
-    blob = io.BytesIO(encryptionInfo.read(headerSize))
-    header = _parse_encryptionheader(blob)
-    logger.debug(header)
-    blob = io.BytesIO(encryptionInfo.read())
-    verifier = _parse_encryptionverifier(blob, "RC4")  # TODO: Fix (cf. ooxml.py)
-    logger.debug(verifier)
-    info = {
-        "salt": verifier["salt"],
-        "keySize": header["keySize"],
-        "encryptedVerifier": verifier["encryptedVerifier"],
-        "encryptedVerifierHash": verifier["encryptedVerifierHash"],
-    }
-    return info
-
-
 class _BIFFStream:
     def __init__(self, data):
         self.data = data
 
     def has_record(self, target):
         pos = self.data.tell()
         while True:
@@ -498,15 +482,17 @@
         (num,) = unpack("<H", workbook.data.read(2))
 
         assert num == 2057  # BOF
 
         (size,) = unpack("<H", workbook.data.read(2))
         workbook.data.read(size)  # Skip BOF
 
-        num, size = workbook.skip_to(recordNameNum["FilePass"])  # Skip to FilePass; TODO: Raise exception if not encrypted
+        num, size = workbook.skip_to(
+            recordNameNum["FilePass"]
+        )  # Skip to FilePass; TODO: Raise exception if not encrypted
 
         # FilePass: https://msdn.microsoft.com/en-us/library/dd952596(v=office.12).aspx
         # If this record exists, the workbook MUST be encrypted.
         (wEncryptionType,) = unpack("<H", workbook.data.read(2))
 
         encryptionInfo = io.BytesIO(workbook.data.read(size - 2))
 
@@ -525,42 +511,53 @@
             vMajor, vMinor = unpack("<HH", encryptionVersionInfo)
 
             logger.debug("Version: {} {}".format(vMajor, vMinor))
 
             if vMajor == 0x0001 and vMinor == 0x0001:  # RC4
                 info = _parse_header_RC4(encryptionInfo)
 
-                if DocumentRC4.verifypw(password, info["salt"], info["encryptedVerifier"], info["encryptedVerifierHash"]):
+                if DocumentRC4.verifypw(
+                    password,
+                    info["salt"],
+                    info["encryptedVerifier"],
+                    info["encryptedVerifierHash"],
+                ):
                     self.type = "rc4"
                     self.key = password
                     self.salt = info["salt"]
                 else:
                     raise exceptions.InvalidKeyError("Failed to verify password")
 
-            elif vMajor in [0x0002, 0x0003, 0x0004] and vMinor == 0x0002:  # RC4 CryptoAPI
+            elif (
+                vMajor in [0x0002, 0x0003, 0x0004] and vMinor == 0x0002
+            ):  # RC4 CryptoAPI
                 info = _parse_header_RC4CryptoAPI(encryptionInfo)
 
                 if DocumentRC4CryptoAPI.verifypw(
-                    password, info["salt"], info["keySize"], info["encryptedVerifier"], info["encryptedVerifierHash"]
+                    password,
+                    info["salt"],
+                    info["keySize"],
+                    info["encryptedVerifier"],
+                    info["encryptedVerifierHash"],
                 ):
                     self.type = "rc4_cryptoapi"
                     self.key = password
                     self.salt = info["salt"]
                     self.keySize = info["keySize"]
                 else:
                     raise exceptions.InvalidKeyError("Failed to verify password")
 
             else:
                 raise exceptions.DecryptionError("Unsupported encryption method")
 
-    def decrypt(self, ofile):
-        # fd, _ofile_path = tempfile.mkstemp()
+    def decrypt(self, outfile):
+        # fd, _outfile_path = tempfile.mkstemp()
 
-        # shutil.copyfile(os.path.realpath(self.file.name), _ofile_path)
-        # outole = olefile.OleFileIO(_ofile_path, write_mode=True)
+        # shutil.copyfile(os.path.realpath(self.file.name), _outfile_path)
+        # outole = olefile.OleFileIO(_outfile_path, write_mode=True)
 
         # List of encrypted parts: https://msdn.microsoft.com/en-us/library/dd905723(v=office.12).aspx
 
         # Workbook stream
         self.data.workbook.seek(0)
         workbook = _BIFFStream(self.data.workbook)
 
@@ -587,30 +584,42 @@
             ]:
                 header = pack("<HH", num, size)
                 plain_buf += list(header) + list(record.read())
                 encrypted_buf.write(b"\x00" * (4 + size))
             # The lbPlyPos field of the BoundSheet8 record (section 2.4.28) MUST NOT be encrypted.
             elif num == recordNameNum["BoundSheet8"]:
                 header = pack("<HH", num, size)
-                plain_buf += list(header) + list(record.read(4)) + [-2] * (size - 4)  # Preserve lbPlyPos
+                plain_buf += (
+                    list(header) + list(record.read(4)) + [-2] * (size - 4)
+                )  # Preserve lbPlyPos
                 encrypted_buf.write(b"\x00" * 4 + b"\x00" * 4 + record.read())
             else:
                 header = pack("<HH", num, size)
                 plain_buf += list(header) + [-1] * size
                 encrypted_buf.write(b"\x00" * 4 + record.read())
 
         self.data_size = encrypted_buf.tell()
         encrypted_buf.seek(0)
 
         if self.type == "rc4":
-            dec = DocumentRC4.decrypt(self.key, self.salt, encrypted_buf, blocksize=1024)
+            dec = DocumentRC4.decrypt(
+                self.key, self.salt, encrypted_buf, blocksize=1024
+            )
         elif self.type == "rc4_cryptoapi":
-            dec = DocumentRC4CryptoAPI.decrypt(self.key, self.salt, self.keySize, encrypted_buf, blocksize=1024)
+            dec = DocumentRC4CryptoAPI.decrypt(
+                self.key, self.salt, self.keySize, encrypted_buf, blocksize=1024
+            )
         elif self.type == "xor":
-            dec = DocumentXOR.decrypt(self.key, encrypted_buf, plain_buf, record_info, 10)
+            dec = DocumentXOR.decrypt(
+                self.key, encrypted_buf, plain_buf, record_info, 10
+            )
+        else:
+            raise exceptions.DecryptionError(
+                "Unsupported encryption method: {}".format(self.type)
+            )
 
         for c in plain_buf:
             if c == -1 or c == -2:
                 dec.seek(1, 1)
             else:
                 dec.write(bytearray([c]))
 
@@ -618,26 +627,26 @@
 
         # f = open('Workbook', 'wb')
         # f.write(dec.read())
         # dec.seek(0)
 
         workbook_dec = dec
 
-        with tempfile.TemporaryFile() as _ofile:
+        with tempfile.TemporaryFile() as _outfile:
             self.file.seek(0)
-            shutil.copyfileobj(self.file, _ofile)
-            outole = olefile.OleFileIO(_ofile, write_mode=True)
+            shutil.copyfileobj(self.file, _outfile)
+            outole = olefile.OleFileIO(_outfile, write_mode=True)
 
             outole.write_stream("Workbook", workbook_dec.read())
 
-            # _ofile = open(_ofile_path, 'rb')
+            # _outfile = open(_outfile_path, 'rb')
 
-            _ofile.seek(0)
+            _outfile.seek(0)
 
-            shutil.copyfileobj(_ofile, ofile)
+            shutil.copyfileobj(_outfile, outfile)
 
         return
 
     def is_encrypted(self):
         r"""
         Test if the file is encrypted.
```

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/method/container/ecma376_encrypted.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/method/container/ecma376_encrypted.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_agile.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/method/ecma376_agile.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_standard.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/method/ecma376_standard.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/method/rc4.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4_cryptoapi.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/method/rc4_cryptoapi.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.4.0/msoffcrypto/method/xor_obfuscation.py` & `msoffcrypto_tool-5.4.1/msoffcrypto/method/xor_obfuscation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import functools
 import io
 import logging
 from hashlib import md5
 from struct import pack
 
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms
-
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 def _makekey(password, salt, block):
     r"""
     Return a intermediate key.
@@ -35,16 +31,48 @@
     return key
 
 
 class DocumentXOR:
     def __init__(self):
         pass
 
-    pad_array = [0xBB, 0xFF, 0xFF, 0xBA, 0xFF, 0xFF, 0xB9, 0x80, 0x00, 0xBE, 0x0F, 0x00, 0xBF, 0x0F, 0x00]
-    initial_code = [0xE1F0, 0x1D0F, 0xCC9C, 0x84C0, 0x110C, 0x0E10, 0xF1CE, 0x313E, 0x1872, 0xE139, 0xD40F, 0x84F9, 0x280C, 0xA96A, 0x4EC3]
+    pad_array = [
+        0xBB,
+        0xFF,
+        0xFF,
+        0xBA,
+        0xFF,
+        0xFF,
+        0xB9,
+        0x80,
+        0x00,
+        0xBE,
+        0x0F,
+        0x00,
+        0xBF,
+        0x0F,
+        0x00,
+    ]
+    initial_code = [
+        0xE1F0,
+        0x1D0F,
+        0xCC9C,
+        0x84C0,
+        0x110C,
+        0x0E10,
+        0xF1CE,
+        0x313E,
+        0x1872,
+        0xE139,
+        0xD40F,
+        0x84F9,
+        0x280C,
+        0xA96A,
+        0x4EC3,
+    ]
 
     xor_matrix = [
         0xAEFC,
         0x4DD9,
         0x9BB2,
         0x2745,
         0x4E8A,
@@ -170,15 +198,17 @@
         for password_byte in password_array:
             if verifier & 0x4000 == 0x0000:
                 intermidiate_1 = 0
             else:
                 intermidiate_1 = 1
 
             intermidiate_2 = verifier * 2
-            intermidiate_2 = intermidiate_2 & 0x7FFF  # SET most significant bit of Intermediate2 TO 0
+            intermidiate_2 = (
+                intermidiate_2 & 0x7FFF
+            )  # SET most significant bit of Intermediate2 TO 0
 
             intermidiate_3 = intermidiate_1 ^ intermidiate_2
 
             verifier = intermidiate_3 ^ password_byte
 
         return True if (verifier ^ 0xCE4B) == verificationBytes else False
 
@@ -191,31 +221,54 @@
         xor_key = DocumentXOR.initial_code[len(password) - 1]
         current_element = 0x00000068
 
         data = [ord(ch) for ch in reversed(password)]
         for ch in data:
             for i in range(7):
                 if ch & 0x40 != 0:
-                    xor_key = (xor_key ^ DocumentXOR.xor_matrix[current_element]) % 65536
+                    xor_key = (
+                        xor_key ^ DocumentXOR.xor_matrix[current_element]
+                    ) % 65536
                 ch = (ch << 1) % 256
                 current_element -= 1
 
         return xor_key
 
     @staticmethod
     def create_xor_array_method1(password):
         xor_key = DocumentXOR.create_xor_key_method1(password)
 
         index = len(password)
 
-        obfuscation_array = [0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00]
+        obfuscation_array = [
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+            0x00,
+        ]
 
         if index % 2 == 1:
-            temp = (xor_key & 0xFF00) >> 8  # SET Temp TO most significant byte of XorKey
-            obfuscation_array[index] = DocumentXOR.xor_ror(DocumentXOR.pad_array[0], temp)
+            temp = (
+                xor_key & 0xFF00
+            ) >> 8  # SET Temp TO most significant byte of XorKey
+            obfuscation_array[index] = DocumentXOR.xor_ror(
+                DocumentXOR.pad_array[0], temp
+            )
 
             index -= 1
             temp = xor_key & 0x00FF
             password_last_char = ord(password[-1])
             obfuscation_array[index] = DocumentXOR.xor_ror(password_last_char, temp)
 
         while index > 0:
@@ -228,21 +281,25 @@
             obfuscation_array[index] = DocumentXOR.xor_ror(ord(password[index]), temp)
 
         index = 15
         pad_index = 15 - len(password)
 
         while pad_index > 0:
             temp = (xor_key & 0xFF00) >> 8
-            obfuscation_array[index] = DocumentXOR.xor_ror(DocumentXOR.pad_array[pad_index], temp)
+            obfuscation_array[index] = DocumentXOR.xor_ror(
+                DocumentXOR.pad_array[pad_index], temp
+            )
 
             index -= 1
             pad_index -= 1
 
             temp = xor_key & 0x00FF
-            obfuscation_array[index] = DocumentXOR.xor_ror(DocumentXOR.pad_array[pad_index], temp)
+            obfuscation_array[index] = DocumentXOR.xor_ror(
+                DocumentXOR.pad_array[pad_index], temp
+            )
 
             index -= 1
             pad_index -= 1
 
         return obfuscation_array
 
     @staticmethod
```

### Comparing `msoffcrypto_tool-5.4.0/pyproject.toml` & `msoffcrypto_tool-5.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msoffcrypto-tool"
-version = "5.4.0"
+version = "5.4.1"
 description = "Python tool and library for decrypting and encrypting MS Office files using a password or other keys"
 license = "MIT"
 homepage = "https://github.com/nolze/msoffcrypto-tool"
 authors = ["nolze <nolze@int3.net>"]
 readme = "README.md"
 packages = [{ include = "msoffcrypto" }, { include = "NOTICE.txt" }]
```

### Comparing `msoffcrypto_tool-5.4.0/PKG-INFO` & `msoffcrypto_tool-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msoffcrypto-tool
-Version: 5.4.0
+Version: 5.4.1
 Summary: Python tool and library for decrypting and encrypting MS Office files using a password or other keys
 Home-page: https://github.com/nolze/msoffcrypto-tool
 License: MIT
 Author: nolze
 Author-email: nolze@int3.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

