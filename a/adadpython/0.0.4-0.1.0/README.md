# Comparing `tmp/adadpython-0.0.4.tar.gz` & `tmp/adadpython-0.1.0.tar.gz`

## Comparing `adadpython-0.0.4.tar` & `adadpython-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/__init__.py
--rw-r--r--   0        0        0   204598 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/base_pokemon.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/burly.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/dbz.sav
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/dexpoke.py
--rw-r--r--   0        0        0    33973 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/moves.py
--rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/pokemon.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/pypokemon.sav
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/save2.npy
--rw-r--r--   0        0        0   107324 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/saved_dexpoke.npy
--rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/somemons.dat
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/texter.py
--rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/trainerai.py
--rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/victoryroad.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/LICENSES/numpy_license.txt
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/LICENSES/python_license.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/configurations/config.txt
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/configurations/default_config.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/configurations/second_config.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/CREDITS.txt
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/game_blurb.md
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/log.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/time_ref.txt
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/moremon.py
--rw-r--r--   0        0        0   107092 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/saved_dexpoke.npy
--rw-r--r--   0        0        0   203144 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/saved_movedex.npy
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/saved_natures.npy
--rw-r--r--   0        0        0    34624 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/somemons_copy.txt
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_1.npy
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_2.npy
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_3.npy
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_4.npy
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_5.npy
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/somemons/__init__.py
--rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/somemons/somemons.dat
--rw-r--r--   0        0        0    32424 2020-02-02 00:00:00.000000 adadpython-0.0.4/LICENSE
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 adadpython-0.0.4/README.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 adadpython-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 adadpython-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/__init__.py
+-rw-r--r--   0        0        0   204598 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/base_pokemon.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/burly.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/dbz.sav
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/dexpoke.py
+-rw-r--r--   0        0        0    33973 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/moves.py
+-rw-r--r--   0        0        0    91186 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/pokemon.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/pypokemon.sav
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/save2.npy
+-rw-r--r--   0        0        0   107324 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/saved_dexpoke.npy
+-rw-r--r--   0        0        0   205648 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/saved_movedex.npy
+-rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/somemons.dat
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/texter.py
+-rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/trainerai.py
+-rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/victoryroad.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/LICENSES/numpy_license.txt
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/LICENSES/python_license.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/configurations/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/configurations/config.txt
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/configurations/default_config.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/configurations/second_config.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/CREDITS.txt
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/game_blurb.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/log.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/time_ref.txt
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/archive/moremon.py
+-rw-r--r--   0        0        0   107092 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/archive/saved_dexpoke.npy
+-rw-r--r--   0        0        0   203144 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/archive/saved_movedex.npy
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/archive/saved_natures.npy
+-rw-r--r--   0        0        0    34624 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/documentation/archive/somemons_copy.txt
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/elite5/elite_1.npy
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/elite5/elite_2.npy
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/elite5/elite_3.npy
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/elite5/elite_4.npy
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/elite5/elite_5.npy
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/somemons/__init__.py
+-rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.1.0/src/adadpython/somemons/somemons.dat
+-rw-r--r--   0        0        0    32424 2020-02-02 00:00:00.000000 adadpython-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 adadpython-0.1.0/README.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 adadpython-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 adadpython-0.1.0/PKG-INFO
```

### Comparing `adadpython-0.0.4/src/adadpython/base_pokemon.py` & `adadpython-0.1.0/src/adadpython/base_pokemon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/dexpoke.py` & `adadpython-0.1.0/src/adadpython/dexpoke.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/moves.py` & `adadpython-0.1.0/src/adadpython/moves.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/pokemon.py` & `adadpython-0.1.0/src/adadpython/pokemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,26 +22,29 @@
 # baton pass // bide // trapping moves bind/whirlpool 
 # multistrike moves // encore // endeavor // echoed voice // protect-feint
 # entry hazards in battle status, grounded/ungrounded in battle status
 # ***************************************************************************
 import os, copy, sys, argparse
 #import time as t
 from time import localtime, strftime
+from importlib import resources as impr
 import numpy as np
-import base_pokemon
-from base_pokemon import mon, battle, field, checkBlackout, loadMon, makeMon,\
+from . import base_pokemon
+from .base_pokemon import mon, battle, field, checkBlackout, loadMon, makeMon,\
     makeRandom, makeParty, moveInfo, typeStrings, Weathers, Terrains, \
     shortpause, dramaticpause, micropause, elite4_healquit, print_dex, \
     print_party, loadMonNpy, saveParty, loadShowdown, copyrigh, \
     party_fixivs, party_fixevs, print_parties, easter_strings
-from texter import genborder,magic_text,magic_head
-from moves import getMoveInfo,mov,natures
-from dexpoke import dex
-from victoryroad import make_teams, random_evs
-from trainerai import cpu
+from .texter import genborder,magic_text,magic_head
+from .moves import getMoveInfo,mov,natures
+#from .dexpoke import dex
+from . import dex
+from .victoryroad import make_teams, random_evs
+from .trainerai import cpu
+from . import configurations
 #FreePalestine
 #aa:configfunction
 def readconfig(argumentline):
     global username_set,mute_set,nparty_set,nstart_set,gw_set,\
             username,mute_pregame,nparty,nstart,opponentName, loaded_parties
     lineA = argumentline[:-1]
     split = lineA.split(' :: ')
@@ -162,15 +165,17 @@
 nstart_set = False
 nparty_set = False
 gw_set = False
 opponentName="RIVAL"
 loaded_parties = []
 #read the config file
 #aa:configread
-configname = 'configurations/config.txt'
+
+configname = impr.files(configurations) / 'config.txt'
+#configname = 'configurations/config.txt'
 if os.path.isfile(configname):
     with open(configname,'r') as config:
         c_args = [ i for i in config.readlines()]
         #nlines = len(c_args)
         ii = []
         for i in c_args:
             ii.append( readconfig(i) )
```

### Comparing `adadpython-0.0.4/src/adadpython/save2.npy` & `adadpython-0.1.0/src/adadpython/save2.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/saved_dexpoke.npy` & `adadpython-0.1.0/src/adadpython/saved_dexpoke.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/somemons.dat` & `adadpython-0.1.0/src/adadpython/somemons.dat`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/texter.py` & `adadpython-0.1.0/src/adadpython/texter.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/trainerai.py` & `adadpython-0.1.0/src/adadpython/trainerai.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/victoryroad.py` & `adadpython-0.1.0/src/adadpython/victoryroad.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 #this script will use base_pokemon, moves, and dexpoke, to create 5 specific pokemon parties for pokemon.py
 #let's go!
 import os
 import copy
 import numpy as np
-from base_pokemon import mon, makeMon, makeRandom, mo, saveParty
-from moves import mov,struggle
-from dexpoke import dex
-from texter import copyrigh
+from .base_pokemon import mon, makeMon, makeRandom, mo, saveParty
+from .moves import mov,struggle
+#from dexpoke import dex
+from . import dex
+from .texter import copyrigh
 def set_ivs(poke, vals):
     #vals is list or tuple of 6
     poke.hpiv,poke.ativ,poke.deiv,poke.saiv,poke.sdiv,poke.spiv = vals
     poke.reStat()
     return
 def set_evs(poke, vals):
     #vals is list or tuple of 6
```

### Comparing `adadpython-0.0.4/src/adadpython/LICENSES/numpy_license.txt` & `adadpython-0.1.0/src/adadpython/LICENSES/numpy_license.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/LICENSES/python_license.txt` & `adadpython-0.1.0/src/adadpython/LICENSES/python_license.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/CREDITS.txt` & `adadpython-0.1.0/src/adadpython/documentation/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/game_blurb.md` & `adadpython-0.1.0/src/adadpython/documentation/game_blurb.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/log.md` & `adadpython-0.1.0/src/adadpython/documentation/log.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/archive/moremon.py` & `adadpython-0.1.0/src/adadpython/documentation/archive/moremon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/archive/saved_dexpoke.npy` & `adadpython-0.1.0/src/adadpython/documentation/archive/saved_dexpoke.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/archive/saved_movedex.npy` & `adadpython-0.1.0/src/adadpython/documentation/archive/saved_movedex.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/archive/saved_natures.npy` & `adadpython-0.1.0/src/adadpython/documentation/archive/saved_natures.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/documentation/archive/somemons_copy.txt` & `adadpython-0.1.0/src/adadpython/documentation/archive/somemons_copy.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/elite5/elite_1.npy` & `adadpython-0.1.0/src/adadpython/elite5/elite_1.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/elite5/elite_2.npy` & `adadpython-0.1.0/src/adadpython/elite5/elite_2.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/elite5/elite_3.npy` & `adadpython-0.1.0/src/adadpython/elite5/elite_3.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/elite5/elite_4.npy` & `adadpython-0.1.0/src/adadpython/elite5/elite_4.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/elite5/elite_5.npy` & `adadpython-0.1.0/src/adadpython/elite5/elite_5.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/src/adadpython/somemons/somemons.dat` & `adadpython-0.1.0/src/adadpython/somemons/somemons.dat`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/LICENSE` & `adadpython-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/README.md` & `adadpython-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.4/pyproject.toml` & `adadpython-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "adadpython"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Antoine" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `adadpython-0.0.4/PKG-INFO` & `adadpython-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: adadpython
-Version: 0.0.4
+Version: 0.1.0
 Summary: A small example package
 Project-URL: Homepage, https://github.com/
 Project-URL: Issues, https://github.com/issues
 Author: Antoine
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

