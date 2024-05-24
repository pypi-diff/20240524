# Comparing `tmp/openlibrary_api-0.0.4.tar.gz` & `tmp/openlibrary_api-0.0.5.tar.gz`

## Comparing `openlibrary_api-0.0.4.tar` & `openlibrary_api-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/.gitattributes
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/requirements.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/src/openlibrary_api/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/src/openlibrary_api/errors.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/src/openlibrary_api/models.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/src/openlibrary_api/ol_api.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/LICENSE
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openlibrary_api-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/.gitattributes
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/errors.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/models.py
+-rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/ol_api.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/PKG-INFO
```

### Comparing `openlibrary_api-0.0.4/src/openlibrary_api/errors.py` & `openlibrary_api-0.0.5/src/openlibrary_api/errors.py`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.4/src/openlibrary_api/models.py` & `openlibrary_api-0.0.5/src/openlibrary_api/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,153 +59,164 @@
 000003a0: 6c66 2e63 6f76 6572 737d 0d0a 2020 2020  lf.covers}..    
 000003b0: 2020 2020 293e 2222 220d 0a0d 0a63 6c61      )>"""....cla
 000003c0: 7373 2045 6469 7469 6f6e 3a0d 0a20 2020  ss Edition:..   
 000003d0: 2022 2222 0d0a 2020 2020 4375 7272 656e   """..    Curren
 000003e0: 746c 7920 7375 7070 6f72 7465 6420 6669  tly supported fi
 000003f0: 656c 6473 3a0d 0a20 2020 206f 6c69 643a  elds:..    olid:
 00000400: 2073 7472 0d0a 2020 2020 7075 626c 6973   str..    publis
-00000410: 6865 723a 2073 7472 0d0a 2020 2020 7075  her: str..    pu
-00000420: 626c 6973 685f 6461 7465 3a20 6461 7465  blish_date: date
-00000430: 7469 6d65 0d0a 2020 2020 6675 6c6c 5f74  time..    full_t
-00000440: 6974 6c65 3a20 7374 720d 0a20 2020 206c  itle: str..    l
-00000450: 616e 6775 6167 6573 3a20 6c69 7374 5b73  anguages: list[s
-00000460: 7472 5d0d 0a20 2020 206e 756d 6265 725f  tr]..    number_
-00000470: 6f66 5f70 6167 6573 3a20 696e 740d 0a20  of_pages: int.. 
-00000480: 2020 2077 6f72 6b3a 2057 6f72 6b0d 0a20     work: Work.. 
-00000490: 2020 2070 6879 7369 6361 6c5f 666f 726d     physical_form
-000004a0: 6174 3a20 7374 720d 0a20 2020 2069 7362  at: str..    isb
-000004b0: 6e5f 3130 3a20 7374 720d 0a20 2020 2069  n_10: str..    i
-000004c0: 7362 6e5f 3133 3a20 7374 720d 0a20 2020  sbn_13: str..   
-000004d0: 206c 6174 6573 745f 7265 7669 7369 6f6e   latest_revision
-000004e0: 3a20 696e 740d 0a20 2020 2072 6576 6973  : int..    revis
-000004f0: 696f 6e3a 2069 6e74 0d0a 2020 2020 2222  ion: int..    ""
-00000500: 220d 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-00000510: 745f 5f28 0d0a 2020 2020 2020 2020 2020  t__(..          
-00000520: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00000530: 2020 2020 206f 6c69 643a 2073 7472 2c0d       olid: str,.
-00000540: 0a20 2020 2020 2020 2020 2020 2070 7562  .            pub
-00000550: 6c69 7368 6572 733a 206c 6973 745b 7374  lishers: list[st
-00000560: 725d 2c0d 0a20 2020 2020 2020 2020 2020  r],..           
-00000570: 2070 7562 6c69 7368 5f64 6174 653a 2073   publish_date: s
-00000580: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
-00000590: 2066 756c 6c5f 7469 746c 653a 2073 7472   full_title: str
-000005a0: 2c0d 0a20 2020 2020 2020 2020 2020 2061  ,..            a
-000005b0: 7574 686f 7273 3a20 6c69 7374 5b22 4175  uthors: list["Au
-000005c0: 7468 6f72 225d 2c0d 0a20 2020 2020 2020  thor"],..       
-000005d0: 2020 2020 206c 616e 6775 6167 6573 3a20       languages: 
-000005e0: 6c69 7374 5b73 7472 5d2c 0d0a 2020 2020  list[str],..    
-000005f0: 2020 2020 2020 2020 6e75 6d62 6572 5f6f          number_o
-00000600: 665f 7061 6765 733a 2069 6e74 2c0d 0a20  f_pages: int,.. 
-00000610: 2020 2020 2020 2020 2020 2077 6f72 6b73             works
-00000620: 3a20 6c69 7374 5b57 6f72 6b5d 2c0d 0a20  : list[Work],.. 
-00000630: 2020 2020 2020 2020 2020 2070 6879 7369             physi
-00000640: 6361 6c5f 666f 726d 6174 3a20 7374 722c  cal_format: str,
-00000650: 0d0a 2020 2020 2020 2020 2020 2020 6973  ..            is
-00000660: 626e 5f31 303a 2073 7472 2c0d 0a20 2020  bn_10: str,..   
-00000670: 2020 2020 2020 2020 2069 7362 6e5f 3133           isbn_13
-00000680: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
-00000690: 2020 2020 636f 6e74 7269 6275 7469 6f6e      contribution
-000006a0: 733a 206c 6973 745b 7374 725d 0d0a 2020  s: list[str]..  
-000006b0: 2020 293a 0d0a 2020 2020 2020 2020 7365    ):..        se
-000006c0: 6c66 2e6f 6c69 6420 3d20 6f6c 6964 0d0a  lf.olid = olid..
-000006d0: 2020 2020 2020 2020 7365 6c66 2e70 7562          self.pub
-000006e0: 6c69 7368 6572 7320 3d20 7075 626c 6973  lishers = publis
-000006f0: 6865 7273 0d0a 2020 2020 2020 2020 7365  hers..        se
-00000700: 6c66 2e70 7562 6c69 7368 5f64 6174 6520  lf.publish_date 
-00000710: 3d20 7075 626c 6973 685f 6461 7465 0d0a  = publish_date..
-00000720: 2020 2020 2020 2020 7365 6c66 2e66 756c          self.ful
-00000730: 6c5f 7469 746c 6520 3d20 6675 6c6c 5f74  l_title = full_t
-00000740: 6974 6c65 0d0a 2020 2020 2020 2020 7365  itle..        se
-00000750: 6c66 2e61 7574 686f 7273 203d 2061 7574  lf.authors = aut
-00000760: 686f 7273 0d0a 2020 2020 2020 2020 7365  hors..        se
-00000770: 6c66 2e6c 616e 6775 6167 6573 203d 206c  lf.languages = l
-00000780: 616e 6775 6167 6573 0d0a 2020 2020 2020  anguages..      
-00000790: 2020 7365 6c66 2e6e 756d 6265 725f 6f66    self.number_of
-000007a0: 5f70 6167 6573 203d 206e 756d 6265 725f  _pages = number_
-000007b0: 6f66 5f70 6167 6573 0d0a 2020 2020 2020  of_pages..      
-000007c0: 2020 7365 6c66 2e77 6f72 6b73 203d 2077    self.works = w
-000007d0: 6f72 6b73 0d0a 2020 2020 2020 2020 7365  orks..        se
-000007e0: 6c66 2e70 6879 7369 6361 6c5f 666f 726d  lf.physical_form
-000007f0: 6174 203d 2070 6879 7369 6361 6c5f 666f  at = physical_fo
-00000800: 726d 6174 0d0a 2020 2020 2020 2020 7365  rmat..        se
-00000810: 6c66 2e69 7362 6e5f 3130 203d 2069 7362  lf.isbn_10 = isb
-00000820: 6e5f 3130 0d0a 2020 2020 2020 2020 7365  n_10..        se
-00000830: 6c66 2e69 7362 6e5f 3133 203d 2069 7362  lf.isbn_13 = isb
-00000840: 6e5f 3133 0d0a 2020 2020 2020 2020 7365  n_13..        se
-00000850: 6c66 2e63 6f6e 7472 6962 7574 696f 6e73  lf.contributions
-00000860: 203d 2063 6f6e 7472 6962 7574 696f 6e73   = contributions
-00000870: 0d0a 0d0a 2020 2020 6465 6620 5f5f 7265  ....    def __re
-00000880: 7072 5f5f 2873 656c 6629 202d 3e20 7374  pr__(self) -> st
-00000890: 723a 0d0a 2020 2020 2020 2020 7265 7475  r:..        retu
-000008a0: 726e 2066 2222 220d 0a20 2020 2020 2020  rn f"""..       
-000008b0: 203c 4564 6974 696f 6e20 286f 6c69 643d   <Edition (olid=
-000008c0: 7b73 656c 662e 6f6c 6964 7d2c 200d 0a20  {self.olid}, .. 
-000008d0: 2020 2020 2020 2070 7562 6c69 7368 6572         publisher
-000008e0: 733d 7b73 656c 662e 7075 626c 6973 6865  s={self.publishe
-000008f0: 7273 7d2c 0d0a 2020 2020 2020 2020 7075  rs},..        pu
-00000900: 626c 6973 685f 6461 7465 3d7b 7365 6c66  blish_date={self
-00000910: 2e70 7562 6c69 7368 5f64 6174 657d 2c20  .publish_date}, 
-00000920: 0d0a 2020 2020 2020 2020 6675 6c6c 5f74  ..        full_t
-00000930: 6974 6c65 3d7b 7365 6c66 2e66 756c 6c5f  itle={self.full_
-00000940: 7469 746c 657d 2c0d 0a20 2020 2020 2020  title},..       
-00000950: 2061 7574 686f 7273 3d7b 7365 6c66 2e61   authors={self.a
-00000960: 7574 686f 7273 7d2c 200d 0a20 2020 2020  uthors}, ..     
-00000970: 2020 206c 616e 6775 6167 6573 3d7b 7365     languages={se
-00000980: 6c66 2e6c 616e 6775 6167 6573 7d2c 200d  lf.languages}, .
-00000990: 0a20 2020 2020 2020 206e 756d 6265 725f  .        number_
-000009a0: 6f66 5f70 6167 6573 3d7b 7365 6c66 2e6e  of_pages={self.n
-000009b0: 756d 6265 725f 6f66 5f70 6167 6573 7d2c  umber_of_pages},
-000009c0: 200d 0a20 2020 2020 2020 2077 6f72 6b73   ..        works
-000009d0: 3d7b 7365 6c66 2e77 6f72 6b73 7d2c 0d0a  ={self.works},..
-000009e0: 2020 2020 2020 2020 7068 7973 6963 616c          physical
-000009f0: 5f66 6f72 6d61 743d 7b73 656c 662e 7068  _format={self.ph
-00000a00: 7973 6963 616c 5f66 6f72 6d61 747d 2c0d  ysical_format},.
-00000a10: 0a20 2020 2020 2020 2069 7362 6e5f 3130  .        isbn_10
-00000a20: 3d7b 7365 6c66 2e69 7362 6e5f 3130 7d2c  ={self.isbn_10},
-00000a30: 200d 0a20 2020 2020 2020 2069 7362 6e5f   ..        isbn_
-00000a40: 3133 3d7b 7365 6c66 2e69 7362 6e5f 3133  13={self.isbn_13
-00000a50: 7d2c 0d0a 2020 2020 2020 2020 636f 6e74  },..        cont
-00000a60: 7269 6275 7469 6f6e 733d 7b73 656c 662e  ributions={self.
-00000a70: 636f 6e74 7269 6275 7469 6f6e 737d 0d0a  contributions}..
-00000a80: 2020 2020 2020 2020 293e 2222 220d 0a0d          )>"""...
-00000a90: 0a63 6c61 7373 2041 7574 686f 723a 0d0a  .class Author:..
-00000aa0: 2020 2020 2222 220d 0a20 2020 2043 7572      """..    Cur
-00000ab0: 7265 6e74 6c79 2073 7570 706f 7274 6564  rently supported
-00000ac0: 2066 6965 6c64 733a 0d0a 2020 2020 6f6c   fields:..    ol
-00000ad0: 6964 3a20 7374 720d 0a20 2020 206e 616d  id: str..    nam
-00000ae0: 653a 2073 7472 0d0a 2020 2020 6269 6f3a  e: str..    bio:
-00000af0: 2073 7472 0d0a 2020 2020 7068 6f74 6f73   str..    photos
-00000b00: 3a20 6c69 7374 5b69 6e74 5d20 2861 206c  : list[int] (a l
-00000b10: 6973 7420 6f66 2070 686f 746f 2069 6473  ist of photo ids
-00000b20: 2066 6f72 204f 7065 6e4c 6962 7261 7279   for OpenLibrary
-00000b30: 2c20 646f 6573 206e 6f74 206c 6f61 6420  , does not load 
-00000b40: 7468 6520 696d 6167 6573 290d 0a20 2020  the images)..   
-00000b50: 2022 2222 0d0a 2020 2020 6465 6620 5f5f   """..    def __
-00000b60: 696e 6974 5f5f 280d 0a20 2020 2020 2020  init__(..       
-00000b70: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00000b80: 2020 2020 2020 2020 6f6c 6964 3a20 7374          olid: st
-00000b90: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00000ba0: 6e61 6d65 3a20 7374 722c 0d0a 2020 2020  name: str,..    
-00000bb0: 2020 2020 2020 2020 6269 6f3a 2073 7472          bio: str
-00000bc0: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-00000bd0: 686f 746f 733a 206c 6973 745b 696e 745d  hotos: list[int]
-00000be0: 0d0a 2020 2020 293a 0d0a 2020 2020 2020  ..    ):..      
-00000bf0: 2020 7365 6c66 2e6f 6c69 6420 3d20 6f6c    self.olid = ol
-00000c00: 6964 0d0a 2020 2020 2020 2020 7365 6c66  id..        self
-00000c10: 2e6e 616d 6520 3d20 6e61 6d65 0d0a 2020  .name = name..  
-00000c20: 2020 2020 2020 7365 6c66 2e62 696f 203d        self.bio =
-00000c30: 2062 696f 0d0a 2020 2020 2020 2020 7365   bio..        se
-00000c40: 6c66 2e70 686f 746f 7320 3d20 7068 6f74  lf.photos = phot
-00000c50: 6f73 0d0a 0d0a 2020 2020 6465 6620 5f5f  os....    def __
-00000c60: 7265 7072 5f5f 2873 656c 6629 202d 3e20  repr__(self) -> 
-00000c70: 7374 723a 0d0a 2020 2020 2020 2020 7265  str:..        re
-00000c80: 7475 726e 2066 2222 220d 0a20 2020 2020  turn f"""..     
-00000c90: 2020 203c 4175 7468 6f72 2028 6f6c 6964     <Author (olid
-00000ca0: 3d7b 7365 6c66 2e6f 6c69 647d 2c20 0d0a  ={self.olid}, ..
-00000cb0: 2020 2020 2020 2020 6e61 6d65 3d7b 7365          name={se
-00000cc0: 6c66 2e6e 616d 657d 2c20 0d0a 2020 2020  lf.name}, ..    
-00000cd0: 2020 2020 6269 6f3d 7b73 656c 662e 6269      bio={self.bi
-00000ce0: 6f7d 2c20 0d0a 2020 2020 2020 2020 7068  o}, ..        ph
-00000cf0: 6f74 6f73 3d7b 7365 6c66 2e70 686f 746f  otos={self.photo
-00000d00: 737d 0d0a 2020 2020 2020 2020 293e 2222  s}..        )>""
-00000d10: 220d 0a0d 0a63 6c61 7373 2053 7562 6a65  "....class Subje
-00000d20: 6374 3a0d 0a20 2020 2070 6173 730d 0a    ct:..    pass..
+00000410: 6865 7273 3a20 6c69 7374 5b73 7472 5d0d  hers: list[str].
+00000420: 0a20 2020 2070 7562 6c69 7368 5f64 6174  .    publish_dat
+00000430: 653a 2064 6174 6574 696d 650d 0a20 2020  e: datetime..   
+00000440: 2066 756c 6c5f 7469 746c 653a 2073 7472   full_title: str
+00000450: 0d0a 2020 2020 6c61 6e67 7561 6765 733a  ..    languages:
+00000460: 206c 6973 745b 7374 725d 0d0a 2020 2020   list[str]..    
+00000470: 6e75 6d62 6572 5f6f 665f 7061 6765 733a  number_of_pages:
+00000480: 2069 6e74 0d0a 2020 2020 776f 726b 733a   int..    works:
+00000490: 206c 6973 745b 576f 726b 5d0d 0a20 2020   list[Work]..   
+000004a0: 2070 6879 7369 6361 6c5f 666f 726d 6174   physical_format
+000004b0: 3a20 7374 720d 0a20 2020 2069 7362 6e5f  : str..    isbn_
+000004c0: 3130 3a20 7374 720d 0a20 2020 2069 7362  10: str..    isb
+000004d0: 6e5f 3133 3a20 7374 720d 0a20 2020 2063  n_13: str..    c
+000004e0: 6f6e 7472 6962 7574 696f 6e73 3a20 6c69  ontributions: li
+000004f0: 7374 5b73 7472 5d0d 0a20 2020 2022 2222  st[str]..    """
+00000500: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00000510: 5f5f 280d 0a20 2020 2020 2020 2020 2020  __(..           
+00000520: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+00000530: 2020 2020 6f6c 6964 3a20 7374 722c 0d0a      olid: str,..
+00000540: 2020 2020 2020 2020 2020 2020 7075 626c              publ
+00000550: 6973 6865 7273 3a20 6c69 7374 5b73 7472  ishers: list[str
+00000560: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000570: 7075 626c 6973 685f 6461 7465 3a20 7374  publish_date: st
+00000580: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00000590: 6675 6c6c 5f74 6974 6c65 3a20 7374 722c  full_title: str,
+000005a0: 0d0a 2020 2020 2020 2020 2020 2020 6175  ..            au
+000005b0: 7468 6f72 733a 206c 6973 745b 2241 7574  thors: list["Aut
+000005c0: 686f 7222 5d2c 0d0a 2020 2020 2020 2020  hor"],..        
+000005d0: 2020 2020 6c61 6e67 7561 6765 733a 206c      languages: l
+000005e0: 6973 745b 7374 725d 2c0d 0a20 2020 2020  ist[str],..     
+000005f0: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
+00000600: 5f70 6167 6573 3a20 696e 742c 0d0a 2020  _pages: int,..  
+00000610: 2020 2020 2020 2020 2020 776f 726b 733a            works:
+00000620: 206c 6973 745b 576f 726b 5d2c 0d0a 2020   list[Work],..  
+00000630: 2020 2020 2020 2020 2020 7068 7973 6963            physic
+00000640: 616c 5f66 6f72 6d61 743a 2073 7472 2c0d  al_format: str,.
+00000650: 0a20 2020 2020 2020 2020 2020 2069 7362  .            isb
+00000660: 6e5f 3130 3a20 7374 722c 0d0a 2020 2020  n_10: str,..    
+00000670: 2020 2020 2020 2020 6973 626e 5f31 333a          isbn_13:
+00000680: 2073 7472 2c0d 0a20 2020 2020 2020 2020   str,..         
+00000690: 2020 2063 6f6e 7472 6962 7574 696f 6e73     contributions
+000006a0: 3a20 6c69 7374 5b73 7472 5d0d 0a20 2020  : list[str]..   
+000006b0: 2029 3a0d 0a20 2020 2020 2020 2073 656c   ):..        sel
+000006c0: 662e 6f6c 6964 203d 206f 6c69 640d 0a20  f.olid = olid.. 
+000006d0: 2020 2020 2020 2073 656c 662e 7075 626c         self.publ
+000006e0: 6973 6865 7273 203d 2070 7562 6c69 7368  ishers = publish
+000006f0: 6572 730d 0a20 2020 2020 2020 2073 656c  ers..        sel
+00000700: 662e 7075 626c 6973 685f 6461 7465 203d  f.publish_date =
+00000710: 2070 7562 6c69 7368 5f64 6174 650d 0a20   publish_date.. 
+00000720: 2020 2020 2020 2073 656c 662e 6675 6c6c         self.full
+00000730: 5f74 6974 6c65 203d 2066 756c 6c5f 7469  _title = full_ti
+00000740: 746c 650d 0a20 2020 2020 2020 2073 656c  tle..        sel
+00000750: 662e 6175 7468 6f72 7320 3d20 6175 7468  f.authors = auth
+00000760: 6f72 730d 0a20 2020 2020 2020 2073 656c  ors..        sel
+00000770: 662e 6c61 6e67 7561 6765 7320 3d20 6c61  f.languages = la
+00000780: 6e67 7561 6765 730d 0a20 2020 2020 2020  nguages..       
+00000790: 2073 656c 662e 6e75 6d62 6572 5f6f 665f   self.number_of_
+000007a0: 7061 6765 7320 3d20 6e75 6d62 6572 5f6f  pages = number_o
+000007b0: 665f 7061 6765 730d 0a20 2020 2020 2020  f_pages..       
+000007c0: 2073 656c 662e 776f 726b 7320 3d20 776f   self.works = wo
+000007d0: 726b 730d 0a20 2020 2020 2020 2073 656c  rks..        sel
+000007e0: 662e 7068 7973 6963 616c 5f66 6f72 6d61  f.physical_forma
+000007f0: 7420 3d20 7068 7973 6963 616c 5f66 6f72  t = physical_for
+00000800: 6d61 740d 0a20 2020 2020 2020 2073 656c  mat..        sel
+00000810: 662e 6973 626e 5f31 3020 3d20 6973 626e  f.isbn_10 = isbn
+00000820: 5f31 300d 0a20 2020 2020 2020 2073 656c  _10..        sel
+00000830: 662e 6973 626e 5f31 3320 3d20 6973 626e  f.isbn_13 = isbn
+00000840: 5f31 330d 0a20 2020 2020 2020 2073 656c  _13..        sel
+00000850: 662e 636f 6e74 7269 6275 7469 6f6e 7320  f.contributions 
+00000860: 3d20 636f 6e74 7269 6275 7469 6f6e 730d  = contributions.
+00000870: 0a0d 0a20 2020 2064 6566 205f 5f72 6570  ...    def __rep
+00000880: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
+00000890: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000008a0: 6e20 6622 2222 0d0a 2020 2020 2020 2020  n f"""..        
+000008b0: 3c45 6469 7469 6f6e 2028 6f6c 6964 3d7b  <Edition (olid={
+000008c0: 7365 6c66 2e6f 6c69 647d 2c20 0d0a 2020  self.olid}, ..  
+000008d0: 2020 2020 2020 7075 626c 6973 6865 7273        publishers
+000008e0: 3d7b 7365 6c66 2e70 7562 6c69 7368 6572  ={self.publisher
+000008f0: 737d 2c0d 0a20 2020 2020 2020 2070 7562  s},..        pub
+00000900: 6c69 7368 5f64 6174 653d 7b73 656c 662e  lish_date={self.
+00000910: 7075 626c 6973 685f 6461 7465 7d2c 200d  publish_date}, .
+00000920: 0a20 2020 2020 2020 2066 756c 6c5f 7469  .        full_ti
+00000930: 746c 653d 7b73 656c 662e 6675 6c6c 5f74  tle={self.full_t
+00000940: 6974 6c65 7d2c 0d0a 2020 2020 2020 2020  itle},..        
+00000950: 6175 7468 6f72 733d 7b73 656c 662e 6175  authors={self.au
+00000960: 7468 6f72 737d 2c20 0d0a 2020 2020 2020  thors}, ..      
+00000970: 2020 6c61 6e67 7561 6765 733d 7b73 656c    languages={sel
+00000980: 662e 6c61 6e67 7561 6765 737d 2c20 0d0a  f.languages}, ..
+00000990: 2020 2020 2020 2020 6e75 6d62 6572 5f6f          number_o
+000009a0: 665f 7061 6765 733d 7b73 656c 662e 6e75  f_pages={self.nu
+000009b0: 6d62 6572 5f6f 665f 7061 6765 737d 2c20  mber_of_pages}, 
+000009c0: 0d0a 2020 2020 2020 2020 776f 726b 733d  ..        works=
+000009d0: 7b73 656c 662e 776f 726b 737d 2c0d 0a20  {self.works},.. 
+000009e0: 2020 2020 2020 2070 6879 7369 6361 6c5f         physical_
+000009f0: 666f 726d 6174 3d7b 7365 6c66 2e70 6879  format={self.phy
+00000a00: 7369 6361 6c5f 666f 726d 6174 7d2c 0d0a  sical_format},..
+00000a10: 2020 2020 2020 2020 6973 626e 5f31 303d          isbn_10=
+00000a20: 7b73 656c 662e 6973 626e 5f31 307d 2c20  {self.isbn_10}, 
+00000a30: 0d0a 2020 2020 2020 2020 6973 626e 5f31  ..        isbn_1
+00000a40: 333d 7b73 656c 662e 6973 626e 5f31 337d  3={self.isbn_13}
+00000a50: 2c0d 0a20 2020 2020 2020 2063 6f6e 7472  ,..        contr
+00000a60: 6962 7574 696f 6e73 3d7b 7365 6c66 2e63  ibutions={self.c
+00000a70: 6f6e 7472 6962 7574 696f 6e73 7d0d 0a20  ontributions}.. 
+00000a80: 2020 2020 2020 2029 3e22 2222 0d0a 0d0a         )>"""....
+00000a90: 636c 6173 7320 4175 7468 6f72 3a0d 0a20  class Author:.. 
+00000aa0: 2020 2022 2222 0d0a 2020 2020 4375 7272     """..    Curr
+00000ab0: 656e 746c 7920 7375 7070 6f72 7465 6420  ently supported 
+00000ac0: 6669 656c 6473 3a0d 0a20 2020 206f 6c69  fields:..    oli
+00000ad0: 643a 2073 7472 0d0a 2020 2020 6e61 6d65  d: str..    name
+00000ae0: 3a20 7374 720d 0a20 2020 2062 696f 3a20  : str..    bio: 
+00000af0: 7374 720d 0a20 2020 2062 6972 7468 5f64  str..    birth_d
+00000b00: 6174 653a 2073 7472 0d0a 2020 2020 6465  ate: str..    de
+00000b10: 6174 685f 6461 7465 3a20 7374 720d 0a20  ath_date: str.. 
+00000b20: 2020 2070 686f 746f 733a 206c 6973 745b     photos: list[
+00000b30: 696e 745d 2028 6120 6c69 7374 206f 6620  int] (a list of 
+00000b40: 7068 6f74 6f20 6964 7320 666f 7220 4f70  photo ids for Op
+00000b50: 656e 4c69 6272 6172 792c 2064 6f65 7320  enLibrary, does 
+00000b60: 6e6f 7420 6c6f 6164 2074 6865 2069 6d61  not load the ima
+00000b70: 6765 7329 0d0a 2020 2020 2222 220d 0a20  ges)..    """.. 
+00000b80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000b90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000ba0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00000bb0: 206f 6c69 643a 2073 7472 2c0d 0a20 2020   olid: str,..   
+00000bc0: 2020 2020 2020 2020 206e 616d 653a 2073           name: s
+00000bd0: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
+00000be0: 2062 696f 3a20 7374 722c 0d0a 2020 2020   bio: str,..    
+00000bf0: 2020 2020 2020 2020 6269 7274 685f 6461          birth_da
+00000c00: 7465 3a20 7374 722c 0d0a 2020 2020 2020  te: str,..      
+00000c10: 2020 2020 2020 6465 6174 685f 6461 7465        death_date
+00000c20: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
+00000c30: 2020 2020 7068 6f74 6f73 3a20 6c69 7374      photos: list
+00000c40: 5b69 6e74 5d0d 0a20 2020 2029 3a0d 0a20  [int]..    ):.. 
+00000c50: 2020 2020 2020 2073 656c 662e 6f6c 6964         self.olid
+00000c60: 203d 206f 6c69 640d 0a20 2020 2020 2020   = olid..       
+00000c70: 2073 656c 662e 6e61 6d65 203d 206e 616d   self.name = nam
+00000c80: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00000c90: 6269 6f20 3d20 6269 6f0d 0a20 2020 2020  bio = bio..     
+00000ca0: 2020 2073 656c 662e 6269 7274 685f 6461     self.birth_da
+00000cb0: 7465 203d 2062 6972 7468 5f64 6174 650d  te = birth_date.
+00000cc0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+00000cd0: 6174 685f 6461 7465 203d 2064 6561 7468  ath_date = death
+00000ce0: 5f64 6174 650d 0a20 2020 2020 2020 2073  _date..        s
+00000cf0: 656c 662e 7068 6f74 6f73 203d 2070 686f  elf.photos = pho
+00000d00: 746f 730d 0a0d 0a20 2020 2064 6566 205f  tos....    def _
+00000d10: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+00000d20: 2073 7472 3a0d 0a20 2020 2020 2020 2072   str:..        r
+00000d30: 6574 7572 6e20 6622 2222 0d0a 2020 2020  eturn f"""..    
+00000d40: 2020 2020 3c41 7574 686f 7220 286f 6c69      <Author (oli
+00000d50: 643d 7b73 656c 662e 6f6c 6964 7d2c 200d  d={self.olid}, .
+00000d60: 0a20 2020 2020 2020 206e 616d 653d 7b73  .        name={s
+00000d70: 656c 662e 6e61 6d65 7d2c 200d 0a20 2020  elf.name}, ..   
+00000d80: 2020 2020 2062 696f 3d7b 7365 6c66 2e62       bio={self.b
+00000d90: 696f 7d2c 200d 0a20 2020 2020 2020 2070  io}, ..        p
+00000da0: 686f 746f 733d 7b73 656c 662e 7068 6f74  hotos={self.phot
+00000db0: 6f73 7d0d 0a20 2020 2020 2020 2029 3e22  os}..        )>"
+00000dc0: 2222 0d0a 0d0a 636c 6173 7320 5375 626a  ""....class Subj
+00000dd0: 6563 743a 0d0a 2020 2020 7061 7373 0d0a  ect:..    pass..
```

### Comparing `openlibrary_api-0.0.4/src/openlibrary_api/ol_api.py` & `openlibrary_api-0.0.5/src/openlibrary_api/ol_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,19 +154,16 @@
             if cache_hit != None:
                 language_names.append(cache_hit)
                 continue
             name = self.__make_language_request(language)["name_translated"]["en-gb"][0]
             self.languages_cache.add(language, name)
             language_names.append(name)
         return language_names
-
-    def get_edition_by_isbn(self, isbn: str) -> Edition | None:
-        result = self.__make_isbn_request(isbn)
-        if result is None:
-            return None
+    
+    def __build_edition_from_result(self, result: dict) -> Edition:
         olid = result["key"].replace("/books/", "")
         works = self.__get_works(result["works"]) if "works" in result.keys() else []
         authors = self.__get_authors(result["authors"]) if "authors" in result.keys() else []
         languages = self.__get_languages(result["languages"]) if "languages" in result.keys() else []
         edition = Edition(
             olid, 
             result["publishers"] if "publishers" in result.keys() else [], 
@@ -178,15 +175,20 @@
             works, 
             result["physical_format"] if "physical_format" in result.keys() else "unknown",
             result["isbn_10"] if "isbn_10" in result.keys() else "unknown",
             result["isbn_13"] if "isbn_13" in result.keys() else "unknown",
             result["contributions"] if "contributions" in result.keys() else []
             )
         self.editions_cache.add(olid, edition)
-        return edition
+
+    def get_edition_by_isbn(self, isbn: str) -> Edition | None:
+        result = self.__make_isbn_request(isbn)
+        if result is None:
+            return None
+        return self.__build_edition_from_result(result)     
         
     def get_work_by_olid(self, olid: str, cache=True) -> Work | None:
         if cache:
             cache_hit = self.authors_cache.get(olid)
             if cache_hit != None:
                 return cache_hit
         result = self.__make_olid_request("works", olid)
@@ -208,47 +210,31 @@
         if cache:
             cache_hit = self.editions_cache.get(olid)
             if cache_hit != None:
                 return cache_hit
         result = self.__make_olid_request("books", olid)
         if result is None:
             return None
-        works = self.__get_works(result["works"]) if "works" in result.keys() else []
-        authors = self.__get_authors(result["authors"]) if "authors" in result.keys() else []
-        languages = self.__get_languages(result["languages"]) if "languages" in result.keys() else []
-        edition = Edition(
-            olid, 
-            result["publishers"] if "publishers" in result.keys() else [], 
-            result["publish_date"] if "publish_date" in result.keys() else None, 
-            result["full_title"] if "full_title" in result.keys() else None, 
-            authors,
-            languages, 
-            result["number_of_pages"] if "number_of_pages" in result.keys() else None, 
-            works, 
-            result["physical_format"] if "physical_format" in result.keys() else None,
-            result["isbn_10"] if "isbn_10" in result.keys() else None,
-            result["isbn_13"] if "isbn_13" in result.keys() else None,
-            result["contributions"] if "contributions" in result.keys() else []
-            )
-        self.editions_cache.add(olid, edition)
-        return edition
+        return self.__build_edition_from_result(result)
         
 
     def get_author_by_olid(self, olid: str, cache=True) -> Author | None:
         if cache:
             cache_hit = self.authors_cache.get(olid)
             if cache_hit != None:
                 return cache_hit
         result = self.__make_olid_request("authors", olid)
         if result is None:
             return None
         author = Author(
             olid, 
-            result["name"], 
+            result["name"] if "name" in result.keys() else None, 
             result["bio"] if "bio" in result.keys() else None, 
+            result["birth_date"] if "birth_date" in result.keys() else None,
+            result["death_date"] if "death_date" in result.keys() else None,
             result["photos"] if "photos" in result.keys() else None
             )
         self.authors_cache.add(olid, author)
         return author
     
     #TODO: implement getting cover images
     def get_cover_by_id(self, cover: int):
```

### Comparing `openlibrary_api-0.0.4/.gitignore` & `openlibrary_api-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.4/LICENSE` & `openlibrary_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.4/pyproject.toml` & `openlibrary_api-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openlibrary_api"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Angel Thomas", email="tnf.angel.19@gmail.com" },
 ]
 description = "A wrapper for the OpenLibrary API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openlibrary_api-0.0.4/PKG-INFO` & `openlibrary_api-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openlibrary_api
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper for the OpenLibrary API
 Project-URL: Homepage, https://github.com/angelt19/openlibrary_api
 Project-URL: Issues, https://github.com/angelt19/openlibrary_api/issues
 Author-email: Angel Thomas <tnf.angel.19@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

