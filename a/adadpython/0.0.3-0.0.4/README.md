# Comparing `tmp/adadpython-0.0.3.tar.gz` & `tmp/adadpython-0.0.4.tar.gz`

## Comparing `adadpython-0.0.3.tar` & `adadpython-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/__init__.py
--rw-r--r--   0        0        0   204586 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/base_pokemon.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/dbz.sav
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/dexpoke.py
--rw-r--r--   0        0        0    33947 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/moves.py
--rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/pokemon.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/pypokemon.sav
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/save2.npy
--rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/somemons.dat
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/texter.py
--rw-r--r--   0        0        0    15640 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/trainerai.py
--rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/victoryroad.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/LICENSES/numpy_license.txt
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/LICENSES/python_license.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/configurations/config.txt
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/configurations/default_config.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/configurations/second_config.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/CREDITS.txt
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/game_blurb.md
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/log.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/time_ref.txt
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/moremon.py
--rw-r--r--   0        0        0   107092 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/saved_dexpoke.npy
--rw-r--r--   0        0        0   203144 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/saved_movedex.npy
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/saved_natures.npy
--rw-r--r--   0        0        0    34624 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/somemons_copy.txt
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_1.npy
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_2.npy
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_3.npy
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_4.npy
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_5.npy
--rw-r--r--   0        0        0    32424 2020-02-02 00:00:00.000000 adadpython-0.0.3/LICENSE
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 adadpython-0.0.3/README.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 adadpython-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 adadpython-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/__init__.py
+-rw-r--r--   0        0        0   204598 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/base_pokemon.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/burly.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/dbz.sav
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/dexpoke.py
+-rw-r--r--   0        0        0    33973 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/moves.py
+-rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/pokemon.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/pypokemon.sav
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/save2.npy
+-rw-r--r--   0        0        0   107324 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/saved_dexpoke.npy
+-rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/somemons.dat
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/texter.py
+-rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/trainerai.py
+-rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/victoryroad.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/LICENSES/numpy_license.txt
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/LICENSES/python_license.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/configurations/config.txt
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/configurations/default_config.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/configurations/second_config.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/CREDITS.txt
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/game_blurb.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/log.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/time_ref.txt
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/moremon.py
+-rw-r--r--   0        0        0   107092 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/saved_dexpoke.npy
+-rw-r--r--   0        0        0   203144 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/saved_movedex.npy
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/saved_natures.npy
+-rw-r--r--   0        0        0    34624 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/documentation/archive/somemons_copy.txt
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_1.npy
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_2.npy
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_3.npy
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_4.npy
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/elite5/elite_5.npy
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/somemons/__init__.py
+-rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.4/src/adadpython/somemons/somemons.dat
+-rw-r--r--   0        0        0    32424 2020-02-02 00:00:00.000000 adadpython-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 adadpython-0.0.4/README.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 adadpython-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 adadpython-0.0.4/PKG-INFO
```

### Comparing `adadpython-0.0.3/src/adadpython/base_pokemon.py` & `adadpython-0.0.4/src/adadpython/base_pokemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 #treat these lines of code with care
 #thank you
 import os
 import time as t
 import calendar as cal
 import hashlib
 import numpy as np
-from texter import genborder,magic_text,magic_head,copyrigh
-from dexpoke import dex
-from moves import mov,natures,struggle,futuresigh,tackl,getMoveInfo
-from trainerai import cpu
+from .texter import genborder,magic_text,magic_head,copyrigh
+from . import dex
+from .moves import mov,natures,struggle,futuresigh,tackl,getMoveInfo
+from .trainerai import cpu
 #classes: mon, battle, field | functions: damage, checkBlackout, loadMon, makeMon, checktype effectiveness, HP, stats
 class mon: #aa:monclass #open up sypder and rename these from hpbase to hbp, etc.
     def __init__(self,level,named,nature=(0,0),hpbase=70,atbase=70,\
         debase=70,sabase=70,sdbase=70,spbase=70,tipe=np.array([0]),\
         random_move=True,how_created='nursery'\
         ): #
         global mo
@@ -3913,14 +3913,15 @@
     ranMoves = rng.choice(mo,size=numMoves,replace=False)
     dome.knownMoves = list(ranMoves)
     dome.PP=[mov[i]["pp"] for i in ranMoves]
     dome.full_evs()
     return dome
 #create a pokemon from the pokedex
 def makeMon(pokedexNumber,level=1,nacher = (0,0),how_created='nursery'):
+    global dex
     Hp,At,De,Sa,Sd,Sp=dex[pokedexNumber]['hp'], dex[pokedexNumber]['at'], \
             dex[pokedexNumber]['de'], dex[pokedexNumber]['sa'], \
             dex[pokedexNumber]['sd'], dex[pokedexNumber]['sp']
     nayme=dex[pokedexNumber]['name']
     tipe1=dex[pokedexNumber]['type1']
     tipe2=dex[pokedexNumber]['type2']
     if dex[pokedexNumber]['type2']==20: #single-typed mon
```

### Comparing `adadpython-0.0.3/src/adadpython/dexpoke.py` & `adadpython-0.0.4/src/adadpython/dexpoke.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,43 +15,50 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 #normal 0,fire 1,water 2,grass 3,electric 4,ice 5,fighting 6,poison 7,
 #ground 8,flying 9,psychic 10,bug 11, #rock 12,ghost 13,dragon 14,
 #dark 15,steel 16,fairy 17
 # import some packages
 import numpy as np
-# import the pokemon from database
-dats = np.loadtxt("somemons.dat",delimiter=",",dtype='U20')
-# make it a list
-datl = dats.tolist()
-# make it a list of tuples not list of lists
-datt = [ tuple(i) for i in datl ]
-dtyp = np.dtype( [('index','i4'),('name','U20'),('hp','i4'),('at','i4'),('de','i4'),('sa','i4'),('sd','i4'),('sp','i4'),('type1','i4'),('type2','i4')  ] )
-dex = np.array( datt, dtype=dtyp )
-# type table, useless I think
-moretype=[
-        ('Normal',0),
-        ('Fire',1),
-        ('Water',2),
-        ('Grass',3),
-        ('Electric',4),
-        ('Ice',5),
-        ('Fighting',6),
-        ('Poison',7),
-        ('Ground',8),
-        ('Flying',9),
-        ('Psychic',10),
-        ('Bug',11),
-        ('Rock',12),
-        ('Ghost',13),
-        ('Dragon',14),
-        ('Dark',15),
-        ('Steel',16),
-        ('Fairy',17),
-        ('Typeless',18) #mostly just for struggle, which does neutral damage to everyone
-        ]
-dtip = np.dtype( [('type','U12'),('index','i4') ] )
-types=np.array(moretype,dtype=dtip)
+
+
+def pokedexer(pokedexpath):
+    dats = np.loadtxt(pokedexpath,delimiter=",",dtype='U20')
+    # make it a list
+    datl = dats.tolist()
+    # make it a list of tuples not list of lists
+    datt = [ tuple(i) for i in datl ]
+    dtyp = np.dtype( [('index','i4'),('name','U20'),('hp','i4'),('at','i4'),('de','i4'),('sa','i4'),('sd','i4'),('sp','i4'),('type1','i4'),('type2','i4')  ] )
+    dexx = np.array( datt, dtype=dtyp )
+    # type table, useless I think
+    moretype=[
+            ('Normal',0),
+            ('Fire',1),
+            ('Water',2),
+            ('Grass',3),
+            ('Electric',4),
+            ('Ice',5),
+            ('Fighting',6),
+            ('Poison',7),
+            ('Ground',8),
+            ('Flying',9),
+            ('Psychic',10),
+            ('Bug',11),
+            ('Rock',12),
+            ('Ghost',13),
+            ('Dragon',14),
+            ('Dark',15),
+            ('Steel',16),
+            ('Fairy',17),
+            ('Typeless',18) #mostly just for struggle, which does neutral damage to everyone
+            ]
+    dtip = np.dtype( [('type','U12'),('index','i4') ] )
+    typess=np.array(moretype,dtype=dtip)
+    return (dexx, typess)
+#dexpath = "./somemons.dat"
+#dex, types = pokedexer(dexpath)
+
 if __name__ == '__main__':
-    np.save('saved_dexpoke.npy', dex)
+    #np.save('saved_dexpoke.npy', dex)
+    pass
 else:
     pass
```

### Comparing `adadpython-0.0.3/src/adadpython/moves.py` & `adadpython-0.0.4/src/adadpython/moves.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#companion to pokemon.py
+ #companion to pokemon.py
 """
 Copyright (C) 2023 Adarius
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
@@ -16,14 +16,16 @@
 """
 #normal 0,fire 1,water 2,grass 3,electric 4,ice 5,fighting 6,poison 7,
 #ground 8,flying 9,psychic 10,bug 11,rock 12,ghost 13,dragon 14,
 #dark 15,steel 16,fairy 17
 import numpy as np
 def getMoveInfo(moveIndex):
     return mov[moveIndex]
+def movers():
+    return
 ## move name // power // accuracy // pp // phys/spec/status // contact? // type // priority // description // code-notes
 moremoves=[
         ("Hyper Beam",150,90,5,1,0,0,0,"The user attacks with a powerful beam! Must rest on next turn.","mustRest"),
         ("Giga Impact",150,90,5,0,1,0,0,"Must rest on next turn.","mustRest"),
         ("Blast Burn",150,90,5,1,0,1,0,"The user attacks with a fiery explosion! Must rest on next turn","mustRest"),
         ("Eruption",150,100,5,1,0,1,0,"The user attacks with a furious explosion!\nThe lower the user's HP, the lower this move's power.","spout"),
         ("Hydro Cannon",150,90,5,1,0,2,0,"Blast of water! Must rest on next turn.","mustRest"),
```

### Comparing `adadpython-0.0.3/src/adadpython/pokemon.py` & `adadpython-0.0.4/src/adadpython/pokemon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/save2.npy` & `adadpython-0.0.4/src/adadpython/save2.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/somemons.dat` & `adadpython-0.0.4/src/adadpython/somemons.dat`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/texter.py` & `adadpython-0.0.4/src/adadpython/texter.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/trainerai.py` & `adadpython-0.0.4/src/adadpython/trainerai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #what if i made a class that had some functions to look at a pokemon battle in progress
 #and make some determinations thereabout
 import numpy as np
-from moves import mov
+from . import moves
+mov = moves.mov
 
 class cpu:
     def __init__(self,battlefield):
         self.party = battlefield.cpus
         self.activemon = battlefield.cpu_mon
         self.enemymon = battlefield.usr_mon
         self.bfield = battlefield
```

### Comparing `adadpython-0.0.3/src/adadpython/victoryroad.py` & `adadpython-0.0.4/src/adadpython/victoryroad.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/LICENSES/numpy_license.txt` & `adadpython-0.0.4/src/adadpython/LICENSES/numpy_license.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/LICENSES/python_license.txt` & `adadpython-0.0.4/src/adadpython/LICENSES/python_license.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/CREDITS.txt` & `adadpython-0.0.4/src/adadpython/documentation/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/game_blurb.md` & `adadpython-0.0.4/src/adadpython/documentation/game_blurb.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/log.md` & `adadpython-0.0.4/src/adadpython/documentation/log.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/archive/moremon.py` & `adadpython-0.0.4/src/adadpython/documentation/archive/moremon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/archive/saved_dexpoke.npy` & `adadpython-0.0.4/src/adadpython/documentation/archive/saved_dexpoke.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/archive/saved_movedex.npy` & `adadpython-0.0.4/src/adadpython/documentation/archive/saved_movedex.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/archive/saved_natures.npy` & `adadpython-0.0.4/src/adadpython/documentation/archive/saved_natures.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/documentation/archive/somemons_copy.txt` & `adadpython-0.0.4/src/adadpython/documentation/archive/somemons_copy.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/elite5/elite_1.npy` & `adadpython-0.0.4/src/adadpython/elite5/elite_1.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/elite5/elite_2.npy` & `adadpython-0.0.4/src/adadpython/elite5/elite_2.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/elite5/elite_3.npy` & `adadpython-0.0.4/src/adadpython/elite5/elite_3.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/elite5/elite_4.npy` & `adadpython-0.0.4/src/adadpython/elite5/elite_4.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/src/adadpython/elite5/elite_5.npy` & `adadpython-0.0.4/src/adadpython/elite5/elite_5.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/LICENSE` & `adadpython-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/README.md` & `adadpython-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.3/pyproject.toml` & `adadpython-0.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "adadpython"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Antoine" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy~=1.26.4"
 ]
 
 [project.urls]
```

### Comparing `adadpython-0.0.3/PKG-INFO` & `adadpython-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: adadpython
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Project-URL: Homepage, https://github.com/
 Project-URL: Issues, https://github.com/issues
 Author: Antoine
 License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy~=1.26.4
 Description-Content-Type: text/markdown
 
 # Anybody here play Pokémon?
```

