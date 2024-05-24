# Comparing `tmp/cm2py-0.3.7.tar.gz` & `tmp/cm2py-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.3.7.tar", last modified: Mon Apr 15 07:01:24 2024, max compression
+gzip compressed data, was "cm2py-0.3.8.tar", last modified: Fri May 24 13:36:42 2024, max compression
```

## Comparing `cm2py-0.3.7.tar` & `cm2py-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/
--rw-rw-r--   0 skm       (1000) skm       (1000)     1096 2024-04-15 05:31:45.000000 cm2py-0.3.7/LICENSE
--rw-r--r--   0 skm       (1000) skm       (1000)     3013 2024-04-15 07:01:24.837779 cm2py-0.3.7/PKG-INFO
--rw-rw-r--   0 skm       (1000) skm       (1000)     1186 2024-04-15 05:31:45.000000 cm2py-0.3.7/README.md
--rw-rw-r--   0 skm       (1000) skm       (1000)      651 2024-04-15 06:57:25.000000 cm2py-0.3.7/pyproject.toml
--rw-rw-r--   0 skm       (1000) skm       (1000)       38 2024-04-15 07:01:24.837779 cm2py-0.3.7/setup.cfg
-drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.833779 cm2py-0.3.7/src/
-drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.833779 cm2py-0.3.7/src/cm2py/
--rw-rw-r--   0 skm       (1000) skm       (1000)      264 2024-04-15 05:31:45.000000 cm2py-0.3.7/src/cm2py/__init__.py
--rw-rw-r--   0 skm       (1000) skm       (1000)     7880 2024-04-15 06:40:40.000000 cm2py-0.3.7/src/cm2py/cm2py.py
-drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/src/cm2py/utilities/
--rw-rw-r--   0 skm       (1000) skm       (1000)       48 2024-04-15 06:53:57.000000 cm2py-0.3.7/src/cm2py/utilities/__init__.py
--rw-rw-r--   0 skm       (1000) skm       (1000)     7419 2024-04-15 07:01:05.000000 cm2py-0.3.7/src/cm2py/utilities/utilities.py
-drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/src/cm2py.egg-info/
--rw-r--r--   0 skm       (1000) skm       (1000)     3013 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/PKG-INFO
--rw-rw-r--   0 skm       (1000) skm       (1000)      320 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/SOURCES.txt
--rw-rw-r--   0 skm       (1000) skm       (1000)        1 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/dependency_links.txt
--rw-rw-r--   0 skm       (1000) skm       (1000)       11 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/requires.txt
--rw-rw-r--   0 skm       (1000) skm       (1000)        6 2024-04-15 07:01:24.000000 cm2py-0.3.7/src/cm2py.egg-info/top_level.txt
-drwxrwxr-x   0 skm       (1000) skm       (1000)        0 2024-04-15 07:01:24.837779 cm2py-0.3.7/tests/
--rw-rw-r--   0 skm       (1000) skm       (1000)     3195 2024-04-15 05:31:45.000000 cm2py-0.3.7/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:36:42.323872 cm2py-0.3.8/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0     3099 2024-05-24 13:36:42.319872 cm2py-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2024-05-24 13:16:42.000000 cm2py-0.3.8/README.md
+-rw-rw-rw-   0        0        0      673 2024-05-24 13:28:02.000000 cm2py-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:36:42.323872 cm2py-0.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 13:36:42.261339 cm2py-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 13:36:42.280134 cm2py-0.3.8/src/cm2py/
+-rw-rw-rw-   0        0        0      306 2024-05-24 13:20:48.000000 cm2py-0.3.8/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     8189 2024-05-24 13:28:01.000000 cm2py-0.3.8/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:36:42.311857 cm2py-0.3.8/src/cm2py/utilities/
+-rw-rw-rw-   0        0        0       50 2024-05-24 13:16:42.000000 cm2py-0.3.8/src/cm2py/utilities/__init__.py
+-rw-rw-rw-   0        0        0     7671 2024-05-24 13:16:42.000000 cm2py-0.3.8/src/cm2py/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:36:42.318877 cm2py-0.3.8/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3099 2024-05-24 13:36:42.000000 cm2py-0.3.8/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-24 13:36:42.000000 cm2py-0.3.8/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:36:42.000000 cm2py-0.3.8/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 13:36:42.000000 cm2py-0.3.8/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 13:36:42.000000 cm2py-0.3.8/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 13:36:42.313879 cm2py-0.3.8/tests/
+-rw-rw-rw-   0        0        0     3436 2024-05-24 13:34:42.000000 cm2py-0.3.8/tests/test_app.py
```

### Comparing `cm2py-0.3.7/LICENSE` & `cm2py-0.3.8/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) Microsoft Corporation
-
-Permission is hereby granted, free of charge, to any person obtaining a copy 
-of this software and associated documentation files (the "Software"), to deal 
-in the Software without restriction, including without limitation the rights 
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
-copies of the Software, and to permit persons to whom the Software is 
-furnished to do so, subject to the following conditions: 
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software. 
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+The MIT License (MIT)
+
+Copyright (c) Microsoft Corporation
+
+Permission is hereby granted, free of charge, to any person obtaining a copy 
+of this software and associated documentation files (the "Software"), to deal 
+in the Software without restriction, including without limitation the rights 
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
+copies of the Software, and to permit persons to whom the Software is 
+furnished to do so, subject to the following conditions: 
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software. 
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
 SOFTWARE.
```

### Comparing `cm2py-0.3.7/PKG-INFO` & `cm2py-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-Metadata-Version: 2.1
-Name: cm2py
-Version: 0.3.7
-Summary: Circuit Maker 2 save generation and manipulation package
-Author-email: SKM GEEK <qestudios17@gmail.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) Microsoft Corporation
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy 
-        of this software and associated documentation files (the "Software"), to deal 
-        in the Software without restriction, including without limitation the rights 
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
-        copies of the Software, and to permit persons to whom the Software is 
-        furnished to do so, subject to the following conditions: 
-        
-        The above copyright notice and this permission notice shall be included in all 
-        copies or substantial portions of the Software. 
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/QEStudios/cm2py
-Project-URL: Bug Tracker, https://github.com/QEStudios/cm2py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: uuid
-Requires-Dist: regex
-
-# cm2py
-
-cm2py is a Python package for generating and manipulating save strings for the roblox game [Circuit Maker 2](https://www.roblox.com/games/6652606416/Circuit-Maker-2).
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install cm2py from [pypi](https://pypi.org/project/cm2py/).
-
-```bash
-pip install cm2py
-```
-
-## Usage
-
-Basic program to generate a line of 8 looping OR gates:
-
-```python
-import cm2py as cm2
-
-LENGTH = 8
-
-save = cm2.Save()
-
-blocks = []
-
-for i in range(LENGTH):
-    blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
-
-### Commented out for clarity.
-### You should store connections in a list if you want to modify them later.
-# connections = []
-
-for i in range(LENGTH):
-    # connections.append(save.addConnection(blocks[i-1], blocks[i]))
-    save.addConnection(blocks[i - 1], blocks[i])  # Directly add the connections to the save object
-
-saveString = save.exportSave()
-print(saveString)
-```
-(from [the loop.py example](examples/loop.py))
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first
-to discuss what you would like to change.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: cm2py
+Version: 0.3.8
+Summary: Circuit Maker 2 save generation and manipulation package
+Author-email: SKM GEEK <qestudios17@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) Microsoft Corporation
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy 
+        of this software and associated documentation files (the "Software"), to deal 
+        in the Software without restriction, including without limitation the rights 
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
+        copies of the Software, and to permit persons to whom the Software is 
+        furnished to do so, subject to the following conditions: 
+        
+        The above copyright notice and this permission notice shall be included in all 
+        copies or substantial portions of the Software. 
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/QEStudios/cm2py
+Project-URL: Bug Tracker, https://github.com/QEStudios/cm2py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: uuid
+Requires-Dist: regex
+
+# cm2py
+
+cm2py is a Python package for generating and manipulating save strings for the roblox game [Circuit Maker 2](https://www.roblox.com/games/6652606416/Circuit-Maker-2).
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install cm2py from [pypi](https://pypi.org/project/cm2py/).
+
+```bash
+pip install cm2py
+```
+
+## Usage
+
+Basic program to generate a line of 8 looping OR gates:
+
+```python
+import cm2py as cm2
+
+LENGTH = 8
+
+save = cm2.Save()
+
+blocks = []
+
+for i in range(LENGTH):
+    blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
+
+### Commented out for clarity.
+### You should store connections in a list if you want to modify them later.
+# connections = []
+
+for i in range(LENGTH):
+    # connections.append(save.addConnection(blocks[i-1], blocks[i]))
+    save.addConnection(blocks[i - 1], blocks[i])  # Directly add the connections to the save object
+
+saveString = save.exportSave()
+print(saveString)
+```
+(from [the loop.py example](examples/loop.py))
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first
+to discuss what you would like to change.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `cm2py-0.3.7/pyproject.toml` & `cm2py-0.3.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "cm2py"
-version = "0.3.7"
-authors = [{ name = "SKM GEEK", email = "qestudios17@gmail.com" }]
-description = "Circuit Maker 2 save generation and manipulation package"
-readme = "README.md"
-license = { file = "LICENSE" }
-requires-python = ">=3.7"
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-]
-dependencies = ["uuid", "regex"]
-
-[project.urls]
-"Homepage" = "https://github.com/QEStudios/cm2py"
-"Bug Tracker" = "https://github.com/QEStudios/cm2py/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "cm2py"
+version = "0.3.8"
+authors = [{ name = "SKM GEEK", email = "qestudios17@gmail.com" }]
+description = "Circuit Maker 2 save generation and manipulation package"
+readme = "README.md"
+license = { file = "LICENSE" }
+requires-python = ">=3.7"
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+dependencies = ["uuid", "regex"]
+
+[project.urls]
+"Homepage" = "https://github.com/QEStudios/cm2py"
+"Bug Tracker" = "https://github.com/QEStudios/cm2py/issues"
```

### Comparing `cm2py-0.3.7/src/cm2py/cm2py.py` & `cm2py-0.3.8/src/cm2py/cm2py.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-#!/usr/bin/env python3
-""" Circuit Maker 2 save generation and manipulation package
-
-This module contains utilities to generate and manipulate save strings
-for the Roblox game Circuit Maker 2 by ismellbeef1.
-"""
-
-__author__ = "SKM GEEK"
-__contact__ = "qestudios17@gmail.com"
-__copyright__ = "Copyright 2024, SKM GEEK"
-__date__ = "2024/04/14"
-__deprecated__ = False
-__email__ = "qestudios17@gmail.com"
-__license__ = "MIT"
-__maintainer__ = "SKM GEEK"
-__status__ = "Production"
-__version__ = "0.3.7"
-
-from uuid import uuid4
-import math
-import regex as re
-from typing import Literal, Callable
-import string
-import struct
-
-
-class Block:
-    __initialised = False
-
-    def __init__(self, blockId, pos, state=False, properties=None):
-        assert (
-            isinstance(blockId, int) and 0 <= blockId <= 17
-        ), "blockId must be an integer between 0 and 17"
-        assert (
-            isinstance(pos, tuple)
-            and len(pos) == 3
-            and (isinstance(pos[0], (float, int)))
-            and (isinstance(pos[1], (float, int)))
-            and (isinstance(pos[2], (float, int)))
-        ), "pos must be a 3d tuple of integers or floats"
-        assert isinstance(state, bool), "state must be a boolean"
-        assert (
-            isinstance(properties, list) or properties is None
-        ), "properties must be a list of numbers, or None."
-        self.blockId = blockId
-        self.pos = pos
-        self.x = self.pos[0]
-        self.y = self.pos[1]
-        self.z = self.pos[2]
-        self.state = state
-        self.properties = properties
-        self.uuid = str(uuid4())
-
-        self.__initialised = True
-
-    def __setattr__(self, name, value):
-        self.__dict__[name] = value
-        if not self.__initialised:
-            return
-        if name == "pos":
-            self.__dict__["x"] = self.pos[0]
-            self.__dict__["y"] = self.pos[1]
-            self.__dict__["z"] = self.pos[2]
-        elif name in ["x", "y", "z"]:
-            self.__dict__["pos"] = (self.x, self.y, self.z)
-
-
-class Connection:
-    def __init__(self, source, target):
-        assert isinstance(source, Block), "source must be a Block object"
-        assert isinstance(target, Block), "target must be a Block object"
-        self.source = source
-        self.target = target
-
-
-class Save:
-    """A class to represent a save, which can be modified."""
-
-    def __init__(self):
-        self.blocks = {}
-        self.connections = {}
-        self.blockCount = 0
-        self.connectionCount = 0
-
-    def addBlock(
-        self,
-        blockId: int,
-        pos: tuple[float, float, float],
-        state: bool = False,
-        properties: bool = None,
-        snapToGrid: bool = True,
-    ) -> Block:
-        """Add a block to the save."""
-        if snapToGrid:
-            newBlock = Block(
-                blockId,
-                tuple([int(math.floor(i)) for i in pos]),
-                state=state,
-                properties=properties,
-            )
-        else:
-            newBlock = Block(blockId, pos, state=state, properties=properties)
-        self.blocks[newBlock.uuid] = newBlock
-        self.blockCount += 1
-        return newBlock
-
-    def addConnection(self, source: Block, target: Block) -> Connection:
-        """Add a connection to the save."""
-        newConnection = Connection(source, target)
-        if newConnection.target.uuid in self.connections:
-            self.connections[newConnection.target.uuid].append(newConnection)
-        else:
-            self.connections[newConnection.target.uuid] = [newConnection]
-        self.connectionCount += 1
-        return newConnection
-
-    def exportSave(self) -> str:
-        """Export the save to a Circuit Maker 2 save string."""
-        string = ""
-        blockIndexes = {}
-        index = 0
-
-        assert self.blockCount > 0, "Saves with less than 1 block cannot be exported."
-
-        for b in self.blocks.values():
-            p = "+".join(str(v) for v in b.properties) if b.properties else ""
-            string += f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z},{p};"
-            blockIndexes[b.uuid] = index
-            index += 1
-
-        string = string[:-1] + "?"
-        for c in self.connections.values():
-            for n in c:
-                string += (
-                    f"{blockIndexes[n.source.uuid]+1},{blockIndexes[n.target.uuid]+1};"
-                )
-        if self.connectionCount > 0:
-            string = string[:-1]
-        string = string + "??"  # TODO: Custom build support & sign data support
-        return string
-
-    def deleteBlock(self, blockRef: Block) -> None:
-        """Delete a block from the save."""
-        assert isinstance(blockRef, Block), "blockRef must be a Block object"
-        assert blockRef.uuid in self.blocks, "block does not exist in save"
-        for c in self.connections.values():
-            for n in c:
-                if n.source.uuid == blockRef.uuid or n.target.uuid == blockRef.uuid:
-                    del self.connections[n.target.uuid][
-                        self.connections[n.target.uuid].index(n)
-                    ]
-                    break
-        del self.blocks[blockRef.uuid]
-        self.blockCount -= 1
-        return
-
-    def deleteConnection(self, connectionRef: Connection) -> None:
-        """Delete a connection from the save."""
-        assert isinstance(
-            connectionRef, Connection
-        ), "connectionRef must be a Connection object"
-        assert connectionRef in (n for c in self.connections.values() for n in c)
-        for c in self.connections.values():
-            for n in c:
-                if connectionRef == n:
-                    del self.connections[n.target.uuid][
-                        self.connections[n.target.uuid].index(n)
-                    ]
-        self.connectionCount -= 1
-
-
-def validateSave(string: str) -> re.Match | None:
-    """Check whether a string is a valid savestring or not."""
-    # fmt: off
-    regex = (
-        r"(?<![\d\w,;?+])" # Blocks
-        r"(?>"
-          r"(?<b>"
-            r"\d+,"
-            r"[01]?"
-            r"(?>,(?<d>-?\d*\.?\d*)){3}"
-            r"(?>(\+|,)(?&d)(?!,))*"
-            r";?"
-          r")+"
-        r"(?<!;)\?"
-        r")"
-
-        r"(?>" # Connections
-          r"(?<i>[1-9][0-9]*),"
-          r"(?&i)"
-          r";?"
-        r")*"
-        r"(?<!;)\?"
-
-        r"(?>" # Buildings
-          r"[A-Za-z]+,"
-          r"(?>(?&d),){3}"
-          r"(?>(?&d),){9}"
-          r"(?>[01](?&i),?)*"
-          r"(?<!,)"
-          r";?"
-        r")*"
-        r"(?<!;)\?"
-
-        r"(" # Sign data
-          r"([0-9a-fA-F]{2})"
-        r")*"
-        r"(?![\d\w,;?+])$"
-    )
-    # fmt: on
-    return re.match(regex, string)
-
-
-def importSave(string: str, snapToGrid: bool = True) -> Save:
-    """Import a Circuit Maker 2 save string as a save."""
-    assert validateSave(string), "invalid save string"
-
-    newSave = Save()
-
-    sections = string.split("?")
-    blockString = sections[0].split(";")
-    connectionString = sections[1].split(";")
-
-    blockVals = [
-        [
-            (
-                None
-                if not v
-                else (
-                    [float(a) for a in v.split("+")]
-                    if "+" in v or p == 5
-                    else float(v) if (v and p != 0) else int(v)
-                )
-            )
-            for p, v in enumerate(i.split(","))
-        ]
-        for i in blockString
-    ]
-    connections = [[int(v) for v in i.split(",")] for i in connectionString if i]
-
-    blocks = []
-    for b in blockVals:
-        blocks.append(
-            newSave.addBlock(
-                b[0],
-                (b[2], b[3], b[4]),
-                state=bool(b[1]),
-                properties=b[5],
-                snapToGrid=snapToGrid,
-            )
-        )
-
-    for c in connections:
-        newSave.addConnection(blocks[c[0] - 1], blocks[c[1] - 1])
-
-    return newSave
+#!/usr/bin/env python3
+""" Circuit Maker 2 save generation and manipulation package
+
+This module contains utilities to generate and manipulate save strings
+for the Roblox game Circuit Maker 2 by ismellbeef1.
+"""
+
+__author__ = "SKM GEEK"
+__contact__ = "qestudios17@gmail.com"
+__copyright__ = "Copyright 2024, SKM GEEK"
+__date__ = "2024/04/14"
+__deprecated__ = False
+__email__ = "qestudios17@gmail.com"
+__license__ = "MIT"
+__maintainer__ = "SKM GEEK"
+__status__ = "Production"
+__version__ = "0.3.8"
+
+from uuid import uuid4
+import math
+import regex as re
+from typing import Literal, Callable
+import string
+import struct
+
+
+class Block:
+    __initialised = False
+
+    def __init__(self, blockId, pos, state=False, properties=None):
+        assert (
+            isinstance(blockId, int) and 0 <= blockId <= 17
+        ), "blockId must be an integer between 0 and 17"
+        assert (
+            isinstance(pos, tuple)
+            and len(pos) == 3
+            and (isinstance(pos[0], (float, int)))
+            and (isinstance(pos[1], (float, int)))
+            and (isinstance(pos[2], (float, int)))
+        ), "pos must be a 3d tuple of integers or floats"
+        assert isinstance(state, bool), "state must be a boolean"
+        assert (
+            isinstance(properties, list) or properties is None
+        ), "properties must be a list of numbers, or None."
+        self.blockId = blockId
+        self.pos = pos
+        self.x = self.pos[0]
+        self.y = self.pos[1]
+        self.z = self.pos[2]
+        self.state = state
+        self.properties = properties
+        self.uuid = str(uuid4())
+
+        self.__initialised = True
+
+    def __setattr__(self, name, value):
+        self.__dict__[name] = value
+        if not self.__initialised:
+            return
+        if name == "pos":
+            self.__dict__["x"] = self.pos[0]
+            self.__dict__["y"] = self.pos[1]
+            self.__dict__["z"] = self.pos[2]
+        elif name in ["x", "y", "z"]:
+            self.__dict__["pos"] = (self.x, self.y, self.z)
+
+
+class Connection:
+    def __init__(self, source, target):
+        assert isinstance(source, Block), "source must be a Block object"
+        assert isinstance(target, Block), "target must be a Block object"
+        self.source = source
+        self.target = target
+
+
+class Save:
+    """A class to represent a save, which can be modified."""
+
+    def __init__(self):
+        self.blocks = {}
+        self.connections = {}
+        self.blockCount = 0
+        self.connectionCount = 0
+
+    def addBlock(
+        self,
+        blockId: int,
+        pos: tuple[float | int, float | int, float | int],
+        state: bool = False,
+        properties: list[int | float] | None = None,
+        snapToGrid: bool = True,
+    ) -> Block:
+        """Add a block to the save."""
+        if snapToGrid:
+            newBlock = Block(
+                blockId,
+                tuple([int(math.floor(i)) for i in pos]),
+                state=state,
+                properties=properties,
+            )
+        else:
+            newBlock = Block(blockId, pos, state=state, properties=properties)
+        self.blocks[newBlock.uuid] = newBlock
+        self.blockCount += 1
+        return newBlock
+
+    def addConnection(self, source: Block, target: Block) -> Connection:
+        """Add a connection to the save."""
+        newConnection = Connection(source, target)
+        if newConnection.target.uuid in self.connections:
+            self.connections[newConnection.target.uuid].append(newConnection)
+        else:
+            self.connections[newConnection.target.uuid] = [newConnection]
+        self.connectionCount += 1
+        return newConnection
+
+    def exportSave(self) -> str:
+        """Export the save to a Circuit Maker 2 save string."""
+        string = ""
+        blockIndexes = {}
+        index = 0
+
+        assert self.blockCount > 0, "Saves with less than 1 block cannot be exported."
+
+        for b in self.blocks.values():
+            p = "+".join(str(v) for v in b.properties) if b.properties else ""
+            string += f"{b.blockId},{int(b.state)},{b.x},{b.y},{b.z},{p};"
+            blockIndexes[b.uuid] = index
+            index += 1
+
+        string = string[:-1] + "?"
+        for c in self.connections.values():
+            for n in c:
+                string += (
+                    f"{blockIndexes[n.source.uuid]+1},{blockIndexes[n.target.uuid]+1};"
+                )
+        if self.connectionCount > 0:
+            string = string[:-1]
+        string = string + "??"  # TODO: Custom build support & sign data support
+        return string
+
+    def deleteBlock(self, blockRef: Block) -> None:
+        """Delete a block from the save."""
+        assert isinstance(blockRef, Block), "blockRef must be a Block object"
+        assert blockRef.uuid in self.blocks, "block does not exist in save"
+        for c in self.connections.values():
+            for n in c:
+                if n.source.uuid == blockRef.uuid or n.target.uuid == blockRef.uuid:
+                    del self.connections[n.target.uuid][
+                        self.connections[n.target.uuid].index(n)
+                    ]
+                    break
+        del self.blocks[blockRef.uuid]
+        self.blockCount -= 1
+        return
+
+    def deleteConnection(self, connectionRef: Connection) -> None:
+        """Delete a connection from the save."""
+        assert isinstance(
+            connectionRef, Connection
+        ), "connectionRef must be a Connection object"
+        assert connectionRef in (n for c in self.connections.values() for n in c)
+        for c in self.connections.values():
+            for n in c:
+                if connectionRef == n:
+                    del self.connections[n.target.uuid][
+                        self.connections[n.target.uuid].index(n)
+                    ]
+        self.connectionCount -= 1
+
+
+def validateSave(string: str) -> re.Match | None:
+    """Check whether a string is a valid savestring or not."""
+    # fmt: off
+    regex = (
+        r"(?<![\d\w,;?+])" # Blocks
+        r"(?>"
+          r"(?<b>"
+            r"\d+,"
+            r"[01]?"
+            r"(?>,(?<d>-?\d*\.?\d*)){3}"
+            r"(?>(\+|,)(?&d)(?!,))*"
+            r";?"
+          r")+"
+        r"(?<!;)\?"
+        r")"
+
+        r"(?>" # Connections
+          r"(?<i>[1-9][0-9]*),"
+          r"(?&i)"
+          r";?"
+        r")*"
+        r"(?<!;)\?"
+
+        r"(?>" # Buildings
+          r"[A-Za-z]+,"
+          r"(?>(?&d),){3}"
+          r"(?>(?&d),){9}"
+          r"(?>[01](?&i),?)*"
+          r"(?<!,)"
+          r";?"
+        r")*"
+        r"(?<!;)\?"
+
+        r"(" # Sign data
+          r"([0-9a-fA-F]{2})"
+        r")*"
+        r"(?![\d\w,;?+])$"
+    )
+    # fmt: on
+    return re.match(regex, string)
+
+
+def importSave(string: str, snapToGrid: bool = True) -> Save:
+    """Import a Circuit Maker 2 save string as a save."""
+    assert validateSave(string), "invalid save string"
+
+    newSave = Save()
+
+    sections = string.split("?")
+    blockString = sections[0].split(";")
+    connectionString = sections[1].split(";")
+
+    blockVals = [
+        [
+            (
+                None
+                if not v
+                else (
+                    [float(a) for a in v.split("+")]
+                    if "+" in v or p == 5
+                    else float(v) if (v and p != 0) else int(v)
+                )
+            )
+            for p, v in enumerate(i.split(","))
+        ]
+        for i in blockString
+    ]
+    connections = [[int(v) for v in i.split(",")] for i in connectionString if i]
+
+    blocks = []
+    for b in blockVals:
+        blocks.append(
+            newSave.addBlock(
+                b[0],
+                (b[2] or 0, b[3] or 0, b[4] or 0),
+                state=bool(b[1]),
+                properties=b[5],
+                snapToGrid=snapToGrid,
+            )
+        )
+
+    for c in connections:
+        newSave.addConnection(blocks[c[0] - 1], blocks[c[1] - 1])
+
+    return newSave
```

### Comparing `cm2py-0.3.7/src/cm2py/utilities/utilities.py` & `cm2py-0.3.8/src/cm2py/utilities/utilities.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-#!/usr/bin/env python3
-"""
-Additional utilities for working with cm2py.
-"""
-
-from ..cm2py import *
-
-def generateCLA(
-    numBits: int,
-    *,
-    includeCarryIn: bool = True,
-    includeOverflow: bool = True,
-    generateIO: bool = True,
-) -> str:
-    """
-    Generates a carry-lookahead adder based on the number of bits. Has options for including the overflow and carry in.
-    """
-
-    save = Save()
-
-    inputA = []
-    inputB = []
-
-    inputAnds = []
-    inputXors = []
-
-    andGates = []
-    if includeCarryIn:
-        carryIn = save.addBlock(2, (-1, 0, -1))
-
-    outputs = []
-
-    for i in range(numBits):
-        a = save.addBlock(3, (0, i, -1))
-        b = save.addBlock(2, (1, i, -1))
-
-        if generateIO:
-            flipflop1 = save.addBlock(5, (0, i, -3))
-            flipflop2 = save.addBlock(5, (1, i, -3))
-            save.addConnection(flipflop1, a)
-            save.addConnection(flipflop2, b)
-
-        if i < numBits - 1 or includeOverflow:
-            gand = save.addBlock(1, (0, i, 0))
-            save.addConnection(a, gand)
-            save.addConnection(b, gand)
-            inputAnds.append(gand)
-
-        gxor = save.addBlock(3, (1, i, 0))
-        save.addConnection(a, gxor)
-        save.addConnection(b, gxor)
-
-        inputA.append(a)
-        inputB.append(b)
-        inputXors.append(gxor)
-
-        outputs.append(save.addBlock(3, (1, i, -2)))
-
-        save.addConnection(gxor, outputs[i])
-        if i > 0:
-            save.addConnection(inputAnds[i - 1], outputs[i])
-
-    if includeOverflow:
-        outputs.append(save.addBlock(2, (0, numBits, 1)))
-        save.addConnection(inputAnds[numBits - 1], outputs[numBits])
-    if includeCarryIn:
-        save.addConnection(carryIn, outputs[0])
-
-    currentPosition = (0, 0, 1)
-
-    def addAndGate():
-        nonlocal currentPosition
-        gate = save.addBlock(1, currentPosition)
-        andGates.append(gate)
-
-        newY = currentPosition[1] + 1
-        newX = currentPosition[0] + newY // numBits
-        newZ = newX // 2 + currentPosition[2]
-        currentPosition = (newX % 2, newY % numBits, newZ)
-
-        return gate
-
-    if includeCarryIn:
-        for i in range(numBits if includeOverflow else numBits - 1):
-            gate = addAndGate()
-            save.addConnection(carryIn, gate)
-            for j in range(i + 1):
-                save.addConnection(inputXors[j], gate)
-            save.addConnection(gate, outputs[i + 1])
-
-    for bit in range(numBits):
-        for i in range(bit + 1, numBits if includeOverflow else numBits - 1):
-            gate = addAndGate()
-            save.addConnection(inputAnds[bit], gate)
-
-            for j in range(bit + 1, i + 1):
-                save.addConnection(inputXors[j], gate)
-            save.addConnection(gate, outputs[i + 1])
-
-    output_zPos = currentPosition[2] + (
-        not (
-            (currentPosition[0] == 1 and currentPosition[1] == 0)
-            or currentPosition[0] == 0
-        )
-    )
-
-    for i in range(numBits):
-        outputs[i].z = output_zPos
-
-    if generateIO:
-        for i in range(numBits):
-            led = save.addBlock(6, (1, i, output_zPos + 2))
-            save.addConnection(outputs[i], led)
-
-    saveString = save.exportSave()
-    return saveString
-
-
-def generateDecoder(
-    numBits: int,
-    *,
-    shape: Literal["square", "line"] = "line",
-    inputShape: Literal["vertical", "horizontal"] = "vertical",
-) -> str:
-    """
-    Generates a decoder based on the number of bits. Includes options for different shapes, like square and line.
-    """
-
-    save = Save()
-
-    inputs = []
-    inverseInputs = []
-
-    for bit in range(numBits):
-        node = save.addBlock(
-            15, (0, bit, 0) if inputShape == "vertical" else (bit, 0, -2)
-        )
-        inputs.append(
-            save.addBlock(2, (1, bit, 0) if inputShape == "vertical" else (bit, 0, -1))
-        )
-        inverseInputs.append(
-            save.addBlock(0, (2, bit, 0) if inputShape == "vertical" else (bit, 0, 0))
-        )
-
-        save.addConnection(node, inputs[bit])
-        save.addConnection(node, inverseInputs[bit])
-
-    gatesPerRow = 2 ** math.ceil(numBits / 2)
-
-    for i in range(2**numBits):
-        pos = (
-            ((0, i, 1) if inputShape == "vertical" else (i, 0, 1))
-            if shape == "line"
-            else (
-                (i % gatesPerRow, i // gatesPerRow, 1)
-                if inputShape == "vertical"
-                else (i % gatesPerRow, 0, 1 + i // gatesPerRow)
-            )
-        )
-        gate = save.addBlock(1, pos)
-
-        for bit in range(numBits):
-            if i & (1 << bit):
-                save.addConnection(inputs[bit], gate)
-            else:
-                save.addConnection(inverseInputs[bit], gate)
-
-    saveString = save.exportSave()
-    return saveString
-
-
-base64 = string.ascii_uppercase + string.ascii_lowercase + string.digits + "+/"
-
-
-def encodeToMemory(
-    data: list[int], memoryType: Literal["mass", "massive", "huge"]
-) -> str:
-    """
-    Turns a list of integers into a string that can be pasted into one of the memory buildings.
-    """
-
-    assert memoryType in [
-        "mass",
-        "massive",
-        "huge",
-    ], 'Invalid memory building type. Use "mass","massive",or "huge"'
-
-    code = ""
-
-    if memoryType == "mass":
-        for v in data:
-            code += format(v % 256, "02x")
-        code += "00" * (4096 - len(data))
-    elif memoryType == "massive":
-        for v in data:
-            code += base64[v & 0x3F]
-            code += base64[(v >> 6) & 0x3F]
-            code += base64[(v >> 12) & 0x3F]
-        code += "AAA" * (4096 - len(data))
-    elif memoryType == "huge":
-        raise (
-            NotImplementedError,
-            "Huge Memory uses full utf8 to represent the values, which don't work well with Roblox yet. When the format gets updated or full utf8 is supported, this function will be updated.",
-        )
-    return code
-
-
-def halfPrecisionBitsToNumber(bits: int) -> float:
-    """
-    Converts a half-precision floating point number stored in an integer to a python float.
-    """
-    packed_bytes = bits.to_bytes(2, byteorder="big")
-
-    half_precision_float = struct.unpack(">e", packed_bytes)[0]
-
-    return half_precision_float
-
-
-def numberToHalfPrecisionBits(f: float) -> int:
-    """
-    Converts a python float to a half-precision floating point value stored in an integer. This integer then can be used with the encodeToMemory() function.
-    """
-    if f != f or f == float("inf") or f == float("-inf"):
-        if f == float("inf"):
-            return 0x7C00
-        elif f == float("-inf"):
-            return 0xFC00
-        else:
-            return 0x7E00
-
-    bits = struct.unpack("H", struct.pack("e", f))[0]
-    return bits
-
-
-def generateFunctionLookUpTable(
-    func: Callable[[float], float],
-    size: int = 4096,
-    *,
-    valueType: Literal["int", "float"] = "int",
-) -> str:
-    """
-    Generates a lookup table string that can be pasted into a Massive Memory for a math function.
-    Takes in a value type parameter as well. If the value type is int, it leaves the results as they are, but if it's float, it converts the values into half-precision floating point.
-    """
-    values = []
-    for num in range(size):
-        values.append(func(num))
-
-    if valueType == "float":
-        for i in range(size):
-            values[i] = numberToHalfPrecisionBits(values[i])
-
+#!/usr/bin/env python3
+"""
+Additional utilities for working with cm2py.
+"""
+
+from ..cm2py import *
+
+def generateCLA(
+    numBits: int,
+    *,
+    includeCarryIn: bool = True,
+    includeOverflow: bool = True,
+    generateIO: bool = True,
+) -> str:
+    """
+    Generates a carry-lookahead adder based on the number of bits. Has options for including the overflow and carry in.
+    """
+
+    save = Save()
+
+    inputA = []
+    inputB = []
+
+    inputAnds = []
+    inputXors = []
+
+    andGates = []
+    if includeCarryIn:
+        carryIn = save.addBlock(2, (-1, 0, -1))
+
+    outputs = []
+
+    for i in range(numBits):
+        a = save.addBlock(3, (0, i, -1))
+        b = save.addBlock(2, (1, i, -1))
+
+        if generateIO:
+            flipflop1 = save.addBlock(5, (0, i, -3))
+            flipflop2 = save.addBlock(5, (1, i, -3))
+            save.addConnection(flipflop1, a)
+            save.addConnection(flipflop2, b)
+
+        if i < numBits - 1 or includeOverflow:
+            gand = save.addBlock(1, (0, i, 0))
+            save.addConnection(a, gand)
+            save.addConnection(b, gand)
+            inputAnds.append(gand)
+
+        gxor = save.addBlock(3, (1, i, 0))
+        save.addConnection(a, gxor)
+        save.addConnection(b, gxor)
+
+        inputA.append(a)
+        inputB.append(b)
+        inputXors.append(gxor)
+
+        outputs.append(save.addBlock(3, (1, i, -2)))
+
+        save.addConnection(gxor, outputs[i])
+        if i > 0:
+            save.addConnection(inputAnds[i - 1], outputs[i])
+
+    if includeOverflow:
+        outputs.append(save.addBlock(2, (0, numBits, 1)))
+        save.addConnection(inputAnds[numBits - 1], outputs[numBits])
+    if includeCarryIn:
+        save.addConnection(carryIn, outputs[0])
+
+    currentPosition = (0, 0, 1)
+
+    def addAndGate():
+        nonlocal currentPosition
+        gate = save.addBlock(1, currentPosition)
+        andGates.append(gate)
+
+        newY = currentPosition[1] + 1
+        newX = currentPosition[0] + newY // numBits
+        newZ = newX // 2 + currentPosition[2]
+        currentPosition = (newX % 2, newY % numBits, newZ)
+
+        return gate
+
+    if includeCarryIn:
+        for i in range(numBits if includeOverflow else numBits - 1):
+            gate = addAndGate()
+            save.addConnection(carryIn, gate)
+            for j in range(i + 1):
+                save.addConnection(inputXors[j], gate)
+            save.addConnection(gate, outputs[i + 1])
+
+    for bit in range(numBits):
+        for i in range(bit + 1, numBits if includeOverflow else numBits - 1):
+            gate = addAndGate()
+            save.addConnection(inputAnds[bit], gate)
+
+            for j in range(bit + 1, i + 1):
+                save.addConnection(inputXors[j], gate)
+            save.addConnection(gate, outputs[i + 1])
+
+    output_zPos = currentPosition[2] + (
+        not (
+            (currentPosition[0] == 1 and currentPosition[1] == 0)
+            or currentPosition[0] == 0
+        )
+    )
+
+    for i in range(numBits):
+        outputs[i].z = output_zPos
+
+    if generateIO:
+        for i in range(numBits):
+            led = save.addBlock(6, (1, i, output_zPos + 2))
+            save.addConnection(outputs[i], led)
+
+    saveString = save.exportSave()
+    return saveString
+
+
+def generateDecoder(
+    numBits: int,
+    *,
+    shape: Literal["square", "line"] = "line",
+    inputShape: Literal["vertical", "horizontal"] = "vertical",
+) -> str:
+    """
+    Generates a decoder based on the number of bits. Includes options for different shapes, like square and line.
+    """
+
+    save = Save()
+
+    inputs = []
+    inverseInputs = []
+
+    for bit in range(numBits):
+        node = save.addBlock(
+            15, (0, bit, 0) if inputShape == "vertical" else (bit, 0, -2)
+        )
+        inputs.append(
+            save.addBlock(2, (1, bit, 0) if inputShape == "vertical" else (bit, 0, -1))
+        )
+        inverseInputs.append(
+            save.addBlock(0, (2, bit, 0) if inputShape == "vertical" else (bit, 0, 0))
+        )
+
+        save.addConnection(node, inputs[bit])
+        save.addConnection(node, inverseInputs[bit])
+
+    gatesPerRow = 2 ** math.ceil(numBits / 2)
+
+    for i in range(2**numBits):
+        pos = (
+            ((0, i, 1) if inputShape == "vertical" else (i, 0, 1))
+            if shape == "line"
+            else (
+                (i % gatesPerRow, i // gatesPerRow, 1)
+                if inputShape == "vertical"
+                else (i % gatesPerRow, 0, 1 + i // gatesPerRow)
+            )
+        )
+        gate = save.addBlock(1, pos)
+
+        for bit in range(numBits):
+            if i & (1 << bit):
+                save.addConnection(inputs[bit], gate)
+            else:
+                save.addConnection(inverseInputs[bit], gate)
+
+    saveString = save.exportSave()
+    return saveString
+
+
+base64 = string.ascii_uppercase + string.ascii_lowercase + string.digits + "+/"
+
+
+def encodeToMemory(
+    data: list[int], memoryType: Literal["mass", "massive", "huge"]
+) -> str:
+    """
+    Turns a list of integers into a string that can be pasted into one of the memory buildings.
+    """
+
+    assert memoryType in [
+        "mass",
+        "massive",
+        "huge",
+    ], 'Invalid memory building type. Use "mass","massive",or "huge"'
+
+    code = ""
+
+    if memoryType == "mass":
+        for v in data:
+            code += format(v % 256, "02x")
+        code += "00" * (4096 - len(data))
+    elif memoryType == "massive":
+        for v in data:
+            code += base64[v & 0x3F]
+            code += base64[(v >> 6) & 0x3F]
+            code += base64[(v >> 12) & 0x3F]
+        code += "AAA" * (4096 - len(data))
+    elif memoryType == "huge":
+        raise (
+            NotImplementedError,
+            "Huge Memory uses full utf8 to represent the values, which don't work well with Roblox yet. When the format gets updated or full utf8 is supported, this function will be updated.",
+        )
+    return code
+
+
+def halfPrecisionBitsToNumber(bits: int) -> float:
+    """
+    Converts a half-precision floating point number stored in an integer to a python float.
+    """
+    packed_bytes = bits.to_bytes(2, byteorder="big")
+
+    half_precision_float = struct.unpack(">e", packed_bytes)[0]
+
+    return half_precision_float
+
+
+def numberToHalfPrecisionBits(f: float) -> int:
+    """
+    Converts a python float to a half-precision floating point value stored in an integer. This integer then can be used with the encodeToMemory() function.
+    """
+    if f != f or f == float("inf") or f == float("-inf"):
+        if f == float("inf"):
+            return 0x7C00
+        elif f == float("-inf"):
+            return 0xFC00
+        else:
+            return 0x7E00
+
+    bits = struct.unpack("H", struct.pack("e", f))[0]
+    return bits
+
+
+def generateFunctionLookUpTable(
+    func: Callable[[float], float],
+    size: int = 4096,
+    *,
+    valueType: Literal["int", "float"] = "int",
+) -> str:
+    """
+    Generates a lookup table string that can be pasted into a Massive Memory for a math function.
+    Takes in a value type parameter as well. If the value type is int, it leaves the results as they are, but if it's float, it converts the values into half-precision floating point.
+    """
+    values = []
+    for num in range(size):
+        values.append(func(num))
+
+    if valueType == "float":
+        for i in range(size):
+            values[i] = numberToHalfPrecisionBits(values[i])
+
     return encodeToMemory(values, "massive")
```

### Comparing `cm2py-0.3.7/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.3.8/src/cm2py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-Metadata-Version: 2.1
-Name: cm2py
-Version: 0.3.7
-Summary: Circuit Maker 2 save generation and manipulation package
-Author-email: SKM GEEK <qestudios17@gmail.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) Microsoft Corporation
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy 
-        of this software and associated documentation files (the "Software"), to deal 
-        in the Software without restriction, including without limitation the rights 
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
-        copies of the Software, and to permit persons to whom the Software is 
-        furnished to do so, subject to the following conditions: 
-        
-        The above copyright notice and this permission notice shall be included in all 
-        copies or substantial portions of the Software. 
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/QEStudios/cm2py
-Project-URL: Bug Tracker, https://github.com/QEStudios/cm2py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: uuid
-Requires-Dist: regex
-
-# cm2py
-
-cm2py is a Python package for generating and manipulating save strings for the roblox game [Circuit Maker 2](https://www.roblox.com/games/6652606416/Circuit-Maker-2).
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install cm2py from [pypi](https://pypi.org/project/cm2py/).
-
-```bash
-pip install cm2py
-```
-
-## Usage
-
-Basic program to generate a line of 8 looping OR gates:
-
-```python
-import cm2py as cm2
-
-LENGTH = 8
-
-save = cm2.Save()
-
-blocks = []
-
-for i in range(LENGTH):
-    blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
-
-### Commented out for clarity.
-### You should store connections in a list if you want to modify them later.
-# connections = []
-
-for i in range(LENGTH):
-    # connections.append(save.addConnection(blocks[i-1], blocks[i]))
-    save.addConnection(blocks[i - 1], blocks[i])  # Directly add the connections to the save object
-
-saveString = save.exportSave()
-print(saveString)
-```
-(from [the loop.py example](examples/loop.py))
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first
-to discuss what you would like to change.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: cm2py
+Version: 0.3.8
+Summary: Circuit Maker 2 save generation and manipulation package
+Author-email: SKM GEEK <qestudios17@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) Microsoft Corporation
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy 
+        of this software and associated documentation files (the "Software"), to deal 
+        in the Software without restriction, including without limitation the rights 
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
+        copies of the Software, and to permit persons to whom the Software is 
+        furnished to do so, subject to the following conditions: 
+        
+        The above copyright notice and this permission notice shall be included in all 
+        copies or substantial portions of the Software. 
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/QEStudios/cm2py
+Project-URL: Bug Tracker, https://github.com/QEStudios/cm2py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: uuid
+Requires-Dist: regex
+
+# cm2py
+
+cm2py is a Python package for generating and manipulating save strings for the roblox game [Circuit Maker 2](https://www.roblox.com/games/6652606416/Circuit-Maker-2).
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install cm2py from [pypi](https://pypi.org/project/cm2py/).
+
+```bash
+pip install cm2py
+```
+
+## Usage
+
+Basic program to generate a line of 8 looping OR gates:
+
+```python
+import cm2py as cm2
+
+LENGTH = 8
+
+save = cm2.Save()
+
+blocks = []
+
+for i in range(LENGTH):
+    blocks.append(save.addBlock(cm2.OR, (i, 0, 0)))
+
+### Commented out for clarity.
+### You should store connections in a list if you want to modify them later.
+# connections = []
+
+for i in range(LENGTH):
+    # connections.append(save.addConnection(blocks[i-1], blocks[i]))
+    save.addConnection(blocks[i - 1], blocks[i])  # Directly add the connections to the save object
+
+saveString = save.exportSave()
+print(saveString)
+```
+(from [the loop.py example](examples/loop.py))
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first
+to discuss what you would like to change.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `cm2py-0.3.7/tests/test_app.py` & `cm2py-0.3.8/tests/test_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,133 @@
-import pytest
-
-from src import cm2py as cm2
-
-
-def test_addBlocks():
-    save = cm2.Save()
-
-    save.addBlock(cm2.NOR, (0, 0, 0))
-    save.addBlock(cm2.AND, (1, 0, 0))
-    save.addBlock(cm2.OR, (2, 0, 0))
-    save.addBlock(cm2.XOR, (3, 0, 0))
-    save.addBlock(cm2.BUTTON, (4, 0, 0))
-    save.addBlock(cm2.FLIPFLOP, (5, 0, 0))
-    save.addBlock(cm2.LED, (6, 0, 0))
-    save.addBlock(cm2.SOUND, (7, 0, 0))
-    save.addBlock(cm2.CONDUCTOR, (8, 0, 0))
-    save.addBlock(cm2.CUSTOM, (9, 0, 0))
-    save.addBlock(cm2.NAND, (10, 0, 0))
-    save.addBlock(cm2.XNOR, (11, 0, 0))
-    save.addBlock(cm2.RANDOM, (12, 0, 0))
-    save.addBlock(cm2.TEXT, (13, 0, 0))
-    save.addBlock(cm2.TILE, (14, 0, 0))
-    save.addBlock(cm2.NODE, (15, 0, 0))
-    save.addBlock(cm2.DELAY, (16, 0, 0))
-    save.addBlock(cm2.ANTENNA, (17, 0, 0))
-
-    save.exportSave()
-
-
-def test_addConnections():
-    save = cm2.Save()
-
-    b1 = save.addBlock(cm2.OR, (0, 0, 0))
-    b2 = save.addBlock(cm2.OR, (2, 0, 0))
-
-    c1 = save.addConnection(b1, b2)
-    c2 = save.addConnection(b2, b1)
-
-    save.exportSave()
-
-
-def test_deleteBlock1():
-    save = cm2.Save()
-
-    b1 = save.addBlock(cm2.OR, (0, 0, 0))
-    b2 = save.addBlock(cm2.OR, (2, 0, 0))
-
-    c1 = save.addConnection(b1, b2)
-
-    save.deleteBlock(b1)
-
-    save.exportSave()
-
-
-def test_deleteBlock2():
-    save = cm2.Save()
-
-    b1 = save.addBlock(cm2.OR, (0, 0, 0))
-    b2 = save.addBlock(cm2.OR, (2, 0, 0))
-
-    c1 = save.addConnection(b1, b2)
-
-    save.deleteBlock(b2)
-
-    save.exportSave()
-
-
-def test_deleteConnection():
-    save = cm2.Save()
-
-    b1 = save.addBlock(cm2.OR, (0, 0, 0))
-    b2 = save.addBlock(cm2.OR, (2, 0, 0))
-
-    c1 = save.addConnection(b1, b2)
-
-    save.deleteConnection(c1)
-
-    save.exportSave()
-
-
-def test_properties():
-    save = cm2.Save()
-
-    b1 = save.addBlock(cm2.LED, (0, 0, 0), properties=[255, 0, 0])
-
-    save.exportSave()
-
-
-def test_move():
-    save = cm2.Save()
-
-    b1 = save.addBlock(cm2.OR, (1, 2, 3))
-    assert b1.pos == (1, 2, 3)
-    assert b1.x == 1 and b1.y == 2 and b1.z == 3
-
-    b1.pos = (4, 5, 6)
-    assert b1.pos == (4, 5, 6)
-    assert b1.x == 4 and b1.y == 5 and b1.z == 6
-
-    b1.x = 7
-    b1.y = 8
-    b1.z = 9
-    assert b1.pos == (7, 8, 9)
-    assert b1.x == 7 and b1.y == 8 and b1.z == 9
-
-
-def test_importSave():
-    string = (
-        "0,0,0,0,3,;0,0,1,0,3,;0,0,2,0,3,;7,1,17,0,6,;7,0,-9,0,3,1.00;"
-        "7,0,20,0,6,1.00;7,0,4,0,-8,10000.00;7,0,19,0,4,;7,0,0,0,-4,100.00;7,0,17,0,2,;"
-        "7,1,20,0,2,;7,0,17,0,4,;7,1,20,0,5,;7,0,-1,0,-5,;7,0,0,0,-6,1000.00;"
-        "7,1,18,0,4,;7,0,6,0,-8,10000.00;7,0,-5,0,-5,1.00;7,1,17,0,5,;7,0,0,0,-2,10.00;"
-        "7,1,20,0,4,;7,0,17,0,3,;7,0,8,0,-8,;7,0,-9,0,1,10.00;7,0,2,0,-8,10000.00;"
-        "7,0,0,0,-8,10000.00;7,0,-9,0,-1,100.00;7,0,-9,0,-5,10000.00;7,0,0,0,0,1.00;"
-        "7,1,20,0,3,;7,0,-7,0,-5,10000.00;7,0,-3,0,-5,10000.00;7,0,-9,0,-3,1000.00?"
-        "16,1;29,11;6,12;24,30;19,9;28,15;21,24;9,16;22,4;25,28;14,20;2,21;26,17;"
-        "27,8;8,5;1,3;23,22;10,18;30,25;5,13;3,10;7,19;13,7;12,23;18,27;17,6;15,29??"
-    )
-
-    save = cm2.importSave(string)
-
-
-def test_importSingleBlock():
-    string = "0,0,0,0,0,???"
-
-    save = cm2.importSave(string)
+import pytest
+
+from src import cm2py as cm2
+
+
+def test_addBlocks():
+    save = cm2.Save()
+
+    save.addBlock(cm2.NOR, (0, 0, 0))
+    save.addBlock(cm2.AND, (1, 0, 0))
+    save.addBlock(cm2.OR, (2, 0, 0))
+    save.addBlock(cm2.XOR, (3, 0, 0))
+    save.addBlock(cm2.BUTTON, (4, 0, 0))
+    save.addBlock(cm2.FLIPFLOP, (5, 0, 0))
+    save.addBlock(cm2.LED, (6, 0, 0))
+    save.addBlock(cm2.SOUND, (7, 0, 0))
+    save.addBlock(cm2.CONDUCTOR, (8, 0, 0))
+    save.addBlock(cm2.CUSTOM, (9, 0, 0))
+    save.addBlock(cm2.NAND, (10, 0, 0))
+    save.addBlock(cm2.XNOR, (11, 0, 0))
+    save.addBlock(cm2.RANDOM, (12, 0, 0))
+    save.addBlock(cm2.TEXT, (13, 0, 0))
+    save.addBlock(cm2.TILE, (14, 0, 0))
+    save.addBlock(cm2.NODE, (15, 0, 0))
+    save.addBlock(cm2.DELAY, (16, 0, 0))
+    save.addBlock(cm2.ANTENNA, (17, 0, 0))
+
+    save.exportSave()
+
+
+def test_addConnections():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.OR, (0, 0, 0))
+    b2 = save.addBlock(cm2.OR, (2, 0, 0))
+
+    c1 = save.addConnection(b1, b2)
+    c2 = save.addConnection(b2, b1)
+
+    save.exportSave()
+
+
+def test_deleteBlock1():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.OR, (0, 0, 0))
+    b2 = save.addBlock(cm2.OR, (2, 0, 0))
+
+    c1 = save.addConnection(b1, b2)
+
+    save.deleteBlock(b1)
+
+    save.exportSave()
+
+
+def test_deleteBlock2():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.OR, (0, 0, 0))
+    b2 = save.addBlock(cm2.OR, (2, 0, 0))
+
+    c1 = save.addConnection(b1, b2)
+
+    save.deleteBlock(b2)
+
+    save.exportSave()
+
+
+def test_deleteConnection():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.OR, (0, 0, 0))
+    b2 = save.addBlock(cm2.OR, (2, 0, 0))
+
+    c1 = save.addConnection(b1, b2)
+
+    save.deleteConnection(c1)
+
+    save.exportSave()
+
+
+def test_properties():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.LED, (0, 0, 0), properties=[255, 0, 0])
+
+    save.exportSave()
+
+
+def test_move():
+    save = cm2.Save()
+
+    b1 = save.addBlock(cm2.OR, (1, 2, 3))
+    assert b1.pos == (1, 2, 3)
+    assert b1.x == 1 and b1.y == 2 and b1.z == 3
+
+    b1.pos = (4, 5, 6)
+    assert b1.pos == (4, 5, 6)
+    assert b1.x == 4 and b1.y == 5 and b1.z == 6
+
+    b1.x = 7
+    b1.y = 8
+    b1.z = 9
+    assert b1.pos == (7, 8, 9)
+    assert b1.x == 7 and b1.y == 8 and b1.z == 9
+
+
+def test_importSave():
+    string = (
+        "0,0,0,0,3,;0,0,1,0,3,;0,0,2,0,3,;7,1,17,0,6,;7,0,-9,0,3,1.00;"
+        "7,0,20,0,6,1.00;7,0,4,0,-8,10000.00;7,0,19,0,4,;7,0,0,0,-4,100.00;7,0,17,0,2,;"
+        "7,1,20,0,2,;7,0,17,0,4,;7,1,20,0,5,;7,0,-1,0,-5,;7,0,0,0,-6,1000.00;"
+        "7,1,18,0,4,;7,0,6,0,-8,10000.00;7,0,-5,0,-5,1.00;7,1,17,0,5,;7,0,0,0,-2,10.00;"
+        "7,1,20,0,4,;7,0,17,0,3,;7,0,8,0,-8,;7,0,-9,0,1,10.00;7,0,2,0,-8,10000.00;"
+        "7,0,0,0,-8,10000.00;7,0,-9,0,-1,100.00;7,0,-9,0,-5,10000.00;7,0,0,0,0,1.00;"
+        "7,1,20,0,3,;7,0,-7,0,-5,10000.00;7,0,-3,0,-5,10000.00;7,0,-9,0,-3,1000.00?"
+        "16,1;29,11;6,12;24,30;19,9;28,15;21,24;9,16;22,4;25,28;14,20;2,21;26,17;"
+        "27,8;8,5;1,3;23,22;10,18;30,25;5,13;3,10;7,19;13,7;12,23;18,27;17,6;15,29??"
+    )
+
+    save = cm2.importSave(string)
+
+
+def test_omittedValues():
+    string = "0,,,,,;0,,1,2,3,;0,0,1,2,,???"
+
+    save = cm2.importSave(string)
+
+
+def test_importSingleBlock():
+    string = "0,0,0,0,0,???"
+
+    save = cm2.importSave(string)
```

