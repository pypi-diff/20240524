# Comparing `tmp/frscraper-0.1.0.tar.gz` & `tmp/frscraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frscraper-0.1.0.tar", last modified: Fri May 24 02:34:57 2024, max compression
+gzip compressed data, was "frscraper-0.1.1.tar", last modified: Fri May 24 02:40:17 2024, max compression
```

## Comparing `frscraper-0.1.0.tar` & `frscraper-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 02:34:57.956149 frscraper-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-24 02:34:57.946182 frscraper-0.1.0/FRScraper/
--rw-rw-rw-   0        0        0     9268 2024-05-22 01:30:37.000000 frscraper-0.1.0/FRScraper/FRScraper.py
--rw-rw-rw-   0        0        0        0 2023-03-10 22:31:23.000000 frscraper-0.1.0/FRScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 02:34:57.955152 frscraper-0.1.0/FRScraper.egg-info/
--rw-rw-rw-   0        0        0     3239 2024-05-24 02:34:57.000000 frscraper-0.1.0/FRScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-24 02:34:57.000000 frscraper-0.1.0/FRScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 02:34:57.000000 frscraper-0.1.0/FRScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-24 02:34:57.000000 frscraper-0.1.0/FRScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 02:34:57.000000 frscraper-0.1.0/FRScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 frscraper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3239 2024-05-24 02:34:57.956149 frscraper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2416 2024-05-24 02:32:05.000000 frscraper-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 02:34:57.956149 frscraper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1319 2024-05-22 01:56:54.000000 frscraper-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:40:17.743239 frscraper-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-24 02:40:17.738256 frscraper-0.1.1/FRScraper/
+-rw-rw-rw-   0        0        0     9268 2024-05-22 01:30:37.000000 frscraper-0.1.1/FRScraper/FRScraper.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 22:31:23.000000 frscraper-0.1.1/FRScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:40:17.742242 frscraper-0.1.1/FRScraper.egg-info/
+-rw-rw-rw-   0        0        0     3198 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 frscraper-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3198 2024-05-24 02:40:17.742242 frscraper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2396 2024-05-24 02:38:21.000000 frscraper-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 02:40:17.743239 frscraper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1319 2024-05-24 02:40:00.000000 frscraper-0.1.1/setup.py
```

### Comparing `frscraper-0.1.0/FRScraper/FRScraper.py` & `frscraper-0.1.1/FRScraper/FRScraper.py`

 * *Files identical despite different names*

### Comparing `frscraper-0.1.0/FRScraper.egg-info/PKG-INFO` & `frscraper-0.1.1/FRScraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRScraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python module for Football Reference scraping and easy access to football data from various leagues
 Home-page: https://github.com/GabrielPastorello/FRScraper
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: football reference,scraper,premier league,la liga,ligue 1,serie a,bundesliga,eredivisie,football data
 Classifier: Programming Language :: Python :: 3
@@ -28,44 +28,44 @@
         <img src="https://img.shields.io/pypi/pyversions/FRScraper" alt="python version" />
     </a>
     <a href="https://pypi.org/project/FRScraper/">
         <img src="https://img.shields.io/pypi/l/FRScraper" alt="license" />
     </a>
 </p>
 
-# âš½ FRScraper
+# FRScraper
 
 Python package for easy access to football data through scraping of [Football Reference](https://fbref.com/en/) website.
 
 This allows users to obtain statistics, standings, and scores of the following tournaments:
 - **Premier League** (England)
 - **La Liga** (Spain)
 - **Bundesliga** (Germany)
 - **Ligue 1** (France)
 - **Serie A** (Italy)
 - **Eredivisie** (Netherlands)
 - **Liga Portuguesa** (Portugal)
 - **Campeonato Brasileiro** (Brazil)
-- **Primera DivisiÃ³n Argentina** (Argentina)
+- **Primera Division Argentina** (Argentina)
 - **Ekstraklasa** (Poland)
 - **Russian Premier League** (Russia)
 - **Saudi Pro League** (Saudi Arabia)
 
-## ðŸš€ Installing
+## Installing
 ### Via `pip`
 Install with the following command:
 
 ```
 pip install FRScraper
 ```
 
-## ðŸ“– Documentation
+## Documentation
 For documentation about the API methods refer to [the documentation](https://github.com/GabrielPastorello/FRScraper/blob/main/API.md).
 
-## ðŸ”Œ Example of use
+## Example of use
 ```
 import FRScraper
 ```
 
 ```
 # League table
 df = FRScraper.get_rankings('ENG').head()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: FRScraper Version: 0.1.0 Summary: Python module for
+Metadata-Version: 2.1 Name: FRScraper Version: 0.1.1 Summary: Python module for
 Football Reference scraping and easy access to football data from various
 leagues Home-page: https://github.com/GabrielPastorello/FRScraper Author:
 Gabriel Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com
 License: MIT Keywords: football reference,scraper,premier league,la liga,ligue
 1,serie a,bundesliga,eredivisie,football data Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pandas>=2.2.2
 Requires-Dist: numpy>=1.26.4 Requires-Dist: python-dateutil>=2.8.2 Requires-
 Dist: pytz>=2024.1 ![fbref_logo](https://github.com/GabrielPastorello/
 FRScraper/assets/57769272/2c097739-f0af-4cb2-8c6e-eafc9d2fdf3e)
                         _[_p_y_p_i_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]
-# Ã¢Å¡Â½ FRScraper Python package for easy access to football data through
-scraping of [Football Reference](https://fbref.com/en/) website. This allows
-users to obtain statistics, standings, and scores of the following tournaments:
-- **Premier League** (England) - **La Liga** (Spain) - **Bundesliga** (Germany)
-- **Ligue 1** (France) - **Serie A** (Italy) - **Eredivisie** (Netherlands) -
+# FRScraper Python package for easy access to football data through scraping of
+[Football Reference](https://fbref.com/en/) website. This allows users to
+obtain statistics, standings, and scores of the following tournaments: -
+**Premier League** (England) - **La Liga** (Spain) - **Bundesliga** (Germany) -
+**Ligue 1** (France) - **Serie A** (Italy) - **Eredivisie** (Netherlands) -
 **Liga Portuguesa** (Portugal) - **Campeonato Brasileiro** (Brazil) - **Primera
-DivisiÃÂ³n Argentina** (Argentina) - **Ekstraklasa** (Poland) - **Russian
-Premier League** (Russia) - **Saudi Pro League** (Saudi Arabia) ## Ã°Å¸Å¡â¬
-Installing ### Via `pip` Install with the following command: ``` pip install
-FRScraper ``` ## Ã°Å¸ââ Documentation For documentation about the API
-methods refer to [the documentation](https://github.com/GabrielPastorello/
-FRScraper/blob/main/API.md). ## Ã°Å¸âÅ Example of use ``` import FRScraper
-``` ``` # League table df = FRScraper.get_rankings('ENG').head() ``` Output: |
-| Rk | Squad | MP | W | D | L | ... | xGD | xGD/90 | Attendance | Top Scorer
-Goals | | -- | -- | --------------- | -- | -- | -- | -- | --- | ---- | ------ |
----------- | ----------------- | | 0 | 1 | Manchester City | 38 | 28 | 7 | 3 |
-... | 44.9 | 1.18 | 50112 | 27 | | 1 | 2 | Arsenal | 38 | 28 | 5 | 5 | ... |
-48.2 | 1.27 | 60236 | 16 | | 2 | 3 | Liverpool | 38 | 24 | 10 | 4 | ... | 42.0
-| 1.11 | 55979 | 18 | | 3 | 4 | Aston Villa | 38 | 20 | 8 | 10 | ... | 3.4 |
-0.09 | 41858 | 19 | | 4 | 5 | Tottenham | 38 | 20 | 6 | 12 | ... | 4.8 | 0.13 |
-61482 | 17 | More examples in the files. Use it wisely!
+Division Argentina** (Argentina) - **Ekstraklasa** (Poland) - **Russian Premier
+League** (Russia) - **Saudi Pro League** (Saudi Arabia) ## Installing ### Via
+`pip` Install with the following command: ``` pip install FRScraper ``` ##
+Documentation For documentation about the API methods refer to [the
+documentation](https://github.com/GabrielPastorello/FRScraper/blob/main/
+API.md). ## Example of use ``` import FRScraper ``` ``` # League table df =
+FRScraper.get_rankings('ENG').head() ``` Output: | | Rk | Squad | MP | W | D |
+L | ... | xGD | xGD/90 | Attendance | Top Scorer Goals | | -- | -- | ----------
+----- | -- | -- | -- | -- | --- | ---- | ------ | ---------- | ----------------
+- | | 0 | 1 | Manchester City | 38 | 28 | 7 | 3 | ... | 44.9 | 1.18 | 50112 |
+27 | | 1 | 2 | Arsenal | 38 | 28 | 5 | 5 | ... | 48.2 | 1.27 | 60236 | 16 | | 2
+| 3 | Liverpool | 38 | 24 | 10 | 4 | ... | 42.0 | 1.11 | 55979 | 18 | | 3 | 4 |
+Aston Villa | 38 | 20 | 8 | 10 | ... | 3.4 | 0.09 | 41858 | 19 | | 4 | 5 |
+Tottenham | 38 | 20 | 6 | 12 | ... | 4.8 | 0.13 | 61482 | 17 | More examples in
+the files. Use it wisely!
```

### Comparing `frscraper-0.1.0/LICENSE` & `frscraper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frscraper-0.1.0/PKG-INFO` & `frscraper-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRScraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python module for Football Reference scraping and easy access to football data from various leagues
 Home-page: https://github.com/GabrielPastorello/FRScraper
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: football reference,scraper,premier league,la liga,ligue 1,serie a,bundesliga,eredivisie,football data
 Classifier: Programming Language :: Python :: 3
@@ -28,44 +28,44 @@
         <img src="https://img.shields.io/pypi/pyversions/FRScraper" alt="python version" />
     </a>
     <a href="https://pypi.org/project/FRScraper/">
         <img src="https://img.shields.io/pypi/l/FRScraper" alt="license" />
     </a>
 </p>
 
-# âš½ FRScraper
+# FRScraper
 
 Python package for easy access to football data through scraping of [Football Reference](https://fbref.com/en/) website.
 
 This allows users to obtain statistics, standings, and scores of the following tournaments:
 - **Premier League** (England)
 - **La Liga** (Spain)
 - **Bundesliga** (Germany)
 - **Ligue 1** (France)
 - **Serie A** (Italy)
 - **Eredivisie** (Netherlands)
 - **Liga Portuguesa** (Portugal)
 - **Campeonato Brasileiro** (Brazil)
-- **Primera DivisiÃ³n Argentina** (Argentina)
+- **Primera Division Argentina** (Argentina)
 - **Ekstraklasa** (Poland)
 - **Russian Premier League** (Russia)
 - **Saudi Pro League** (Saudi Arabia)
 
-## ðŸš€ Installing
+## Installing
 ### Via `pip`
 Install with the following command:
 
 ```
 pip install FRScraper
 ```
 
-## ðŸ“– Documentation
+## Documentation
 For documentation about the API methods refer to [the documentation](https://github.com/GabrielPastorello/FRScraper/blob/main/API.md).
 
-## ðŸ”Œ Example of use
+## Example of use
 ```
 import FRScraper
 ```
 
 ```
 # League table
 df = FRScraper.get_rankings('ENG').head()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: FRScraper Version: 0.1.0 Summary: Python module for
+Metadata-Version: 2.1 Name: FRScraper Version: 0.1.1 Summary: Python module for
 Football Reference scraping and easy access to football data from various
 leagues Home-page: https://github.com/GabrielPastorello/FRScraper Author:
 Gabriel Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com
 License: MIT Keywords: football reference,scraper,premier league,la liga,ligue
 1,serie a,bundesliga,eredivisie,football data Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pandas>=2.2.2
 Requires-Dist: numpy>=1.26.4 Requires-Dist: python-dateutil>=2.8.2 Requires-
 Dist: pytz>=2024.1 ![fbref_logo](https://github.com/GabrielPastorello/
 FRScraper/assets/57769272/2c097739-f0af-4cb2-8c6e-eafc9d2fdf3e)
                         _[_p_y_p_i_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]
-# Ã¢Å¡Â½ FRScraper Python package for easy access to football data through
-scraping of [Football Reference](https://fbref.com/en/) website. This allows
-users to obtain statistics, standings, and scores of the following tournaments:
-- **Premier League** (England) - **La Liga** (Spain) - **Bundesliga** (Germany)
-- **Ligue 1** (France) - **Serie A** (Italy) - **Eredivisie** (Netherlands) -
+# FRScraper Python package for easy access to football data through scraping of
+[Football Reference](https://fbref.com/en/) website. This allows users to
+obtain statistics, standings, and scores of the following tournaments: -
+**Premier League** (England) - **La Liga** (Spain) - **Bundesliga** (Germany) -
+**Ligue 1** (France) - **Serie A** (Italy) - **Eredivisie** (Netherlands) -
 **Liga Portuguesa** (Portugal) - **Campeonato Brasileiro** (Brazil) - **Primera
-DivisiÃÂ³n Argentina** (Argentina) - **Ekstraklasa** (Poland) - **Russian
-Premier League** (Russia) - **Saudi Pro League** (Saudi Arabia) ## Ã°Å¸Å¡â¬
-Installing ### Via `pip` Install with the following command: ``` pip install
-FRScraper ``` ## Ã°Å¸ââ Documentation For documentation about the API
-methods refer to [the documentation](https://github.com/GabrielPastorello/
-FRScraper/blob/main/API.md). ## Ã°Å¸âÅ Example of use ``` import FRScraper
-``` ``` # League table df = FRScraper.get_rankings('ENG').head() ``` Output: |
-| Rk | Squad | MP | W | D | L | ... | xGD | xGD/90 | Attendance | Top Scorer
-Goals | | -- | -- | --------------- | -- | -- | -- | -- | --- | ---- | ------ |
----------- | ----------------- | | 0 | 1 | Manchester City | 38 | 28 | 7 | 3 |
-... | 44.9 | 1.18 | 50112 | 27 | | 1 | 2 | Arsenal | 38 | 28 | 5 | 5 | ... |
-48.2 | 1.27 | 60236 | 16 | | 2 | 3 | Liverpool | 38 | 24 | 10 | 4 | ... | 42.0
-| 1.11 | 55979 | 18 | | 3 | 4 | Aston Villa | 38 | 20 | 8 | 10 | ... | 3.4 |
-0.09 | 41858 | 19 | | 4 | 5 | Tottenham | 38 | 20 | 6 | 12 | ... | 4.8 | 0.13 |
-61482 | 17 | More examples in the files. Use it wisely!
+Division Argentina** (Argentina) - **Ekstraklasa** (Poland) - **Russian Premier
+League** (Russia) - **Saudi Pro League** (Saudi Arabia) ## Installing ### Via
+`pip` Install with the following command: ``` pip install FRScraper ``` ##
+Documentation For documentation about the API methods refer to [the
+documentation](https://github.com/GabrielPastorello/FRScraper/blob/main/
+API.md). ## Example of use ``` import FRScraper ``` ``` # League table df =
+FRScraper.get_rankings('ENG').head() ``` Output: | | Rk | Squad | MP | W | D |
+L | ... | xGD | xGD/90 | Attendance | Top Scorer Goals | | -- | -- | ----------
+----- | -- | -- | -- | -- | --- | ---- | ------ | ---------- | ----------------
+- | | 0 | 1 | Manchester City | 38 | 28 | 7 | 3 | ... | 44.9 | 1.18 | 50112 |
+27 | | 1 | 2 | Arsenal | 38 | 28 | 5 | 5 | ... | 48.2 | 1.27 | 60236 | 16 | | 2
+| 3 | Liverpool | 38 | 24 | 10 | 4 | ... | 42.0 | 1.11 | 55979 | 18 | | 3 | 4 |
+Aston Villa | 38 | 20 | 8 | 10 | ... | 3.4 | 0.09 | 41858 | 19 | | 4 | 5 |
+Tottenham | 38 | 20 | 6 | 12 | ... | 4.8 | 0.13 | 61482 | 17 | More examples in
+the files. Use it wisely!
```

### Comparing `frscraper-0.1.0/README.md` & `frscraper-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,44 @@
         <img src="https://img.shields.io/pypi/pyversions/FRScraper" alt="python version" />
     </a>
     <a href="https://pypi.org/project/FRScraper/">
         <img src="https://img.shields.io/pypi/l/FRScraper" alt="license" />
     </a>
 </p>
 
-# ⚽ FRScraper
+# FRScraper
 
 Python package for easy access to football data through scraping of [Football Reference](https://fbref.com/en/) website.
 
 This allows users to obtain statistics, standings, and scores of the following tournaments:
 - **Premier League** (England)
 - **La Liga** (Spain)
 - **Bundesliga** (Germany)
 - **Ligue 1** (France)
 - **Serie A** (Italy)
 - **Eredivisie** (Netherlands)
 - **Liga Portuguesa** (Portugal)
 - **Campeonato Brasileiro** (Brazil)
-- **Primera División Argentina** (Argentina)
+- **Primera Division Argentina** (Argentina)
 - **Ekstraklasa** (Poland)
 - **Russian Premier League** (Russia)
 - **Saudi Pro League** (Saudi Arabia)
 
-## 🚀 Installing
+## Installing
 ### Via `pip`
 Install with the following command:
 
 ```
 pip install FRScraper
 ```
 
-## 📖 Documentation
+## Documentation
 For documentation about the API methods refer to [the documentation](https://github.com/GabrielPastorello/FRScraper/blob/main/API.md).
 
-## 🔌 Example of use
+## Example of use
 ```
 import FRScraper
 ```
 
 ```
 # League table
 df = FRScraper.get_rankings('ENG').head()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 ![fbref_logo](https://github.com/GabrielPastorello/FRScraper/assets/57769272/
 2c097739-f0af-4cb2-8c6e-eafc9d2fdf3e)
                         _[_p_y_p_i_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]
-# â½ FRScraper Python package for easy access to football data through
-scraping of [Football Reference](https://fbref.com/en/) website. This allows
-users to obtain statistics, standings, and scores of the following tournaments:
-- **Premier League** (England) - **La Liga** (Spain) - **Bundesliga** (Germany)
-- **Ligue 1** (France) - **Serie A** (Italy) - **Eredivisie** (Netherlands) -
+# FRScraper Python package for easy access to football data through scraping of
+[Football Reference](https://fbref.com/en/) website. This allows users to
+obtain statistics, standings, and scores of the following tournaments: -
+**Premier League** (England) - **La Liga** (Spain) - **Bundesliga** (Germany) -
+**Ligue 1** (France) - **Serie A** (Italy) - **Eredivisie** (Netherlands) -
 **Liga Portuguesa** (Portugal) - **Campeonato Brasileiro** (Brazil) - **Primera
-DivisiÃ³n Argentina** (Argentina) - **Ekstraklasa** (Poland) - **Russian
-Premier League** (Russia) - **Saudi Pro League** (Saudi Arabia) ## ð
-Installing ### Via `pip` Install with the following command: ``` pip install
-FRScraper ``` ## ð Documentation For documentation about the API methods
-refer to [the documentation](https://github.com/GabrielPastorello/FRScraper/
-blob/main/API.md). ## ð Example of use ``` import FRScraper ``` ``` # League
-table df = FRScraper.get_rankings('ENG').head() ``` Output: | | Rk | Squad | MP
-| W | D | L | ... | xGD | xGD/90 | Attendance | Top Scorer Goals | | -- | -- |
---------------- | -- | -- | -- | -- | --- | ---- | ------ | ---------- | ------
------------ | | 0 | 1 | Manchester City | 38 | 28 | 7 | 3 | ... | 44.9 | 1.18 |
-50112 | 27 | | 1 | 2 | Arsenal | 38 | 28 | 5 | 5 | ... | 48.2 | 1.27 | 60236 |
-16 | | 2 | 3 | Liverpool | 38 | 24 | 10 | 4 | ... | 42.0 | 1.11 | 55979 | 18 |
-| 3 | 4 | Aston Villa | 38 | 20 | 8 | 10 | ... | 3.4 | 0.09 | 41858 | 19 | | 4
-| 5 | Tottenham | 38 | 20 | 6 | 12 | ... | 4.8 | 0.13 | 61482 | 17 | More
-examples in the files. Use it wisely!
+Division Argentina** (Argentina) - **Ekstraklasa** (Poland) - **Russian Premier
+League** (Russia) - **Saudi Pro League** (Saudi Arabia) ## Installing ### Via
+`pip` Install with the following command: ``` pip install FRScraper ``` ##
+Documentation For documentation about the API methods refer to [the
+documentation](https://github.com/GabrielPastorello/FRScraper/blob/main/
+API.md). ## Example of use ``` import FRScraper ``` ``` # League table df =
+FRScraper.get_rankings('ENG').head() ``` Output: | | Rk | Squad | MP | W | D |
+L | ... | xGD | xGD/90 | Attendance | Top Scorer Goals | | -- | -- | ----------
+----- | -- | -- | -- | -- | --- | ---- | ------ | ---------- | ----------------
+- | | 0 | 1 | Manchester City | 38 | 28 | 7 | 3 | ... | 44.9 | 1.18 | 50112 |
+27 | | 1 | 2 | Arsenal | 38 | 28 | 5 | 5 | ... | 48.2 | 1.27 | 60236 | 16 | | 2
+| 3 | Liverpool | 38 | 24 | 10 | 4 | ... | 42.0 | 1.11 | 55979 | 18 | | 3 | 4 |
+Aston Villa | 38 | 20 | 8 | 10 | ... | 3.4 | 0.09 | 41858 | 19 | | 4 | 5 |
+Tottenham | 38 | 20 | 6 | 12 | ... | 4.8 | 0.13 | 61482 | 17 | More examples in
+the files. Use it wisely!
```

### Comparing `frscraper-0.1.0/setup.py` & `frscraper-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
             name='FRScraper',
-            version='0.1.0',
+            version='0.1.1',
             description='Python module for Football Reference scraping and easy access to football data from various leagues',
             long_description=long_description,
             long_description_content_type="text/markdown",
             url='https://github.com/GabrielPastorello/FRScraper',
             author='Gabriel Speranza Pastorello',
             author_email='gabriel.pastorello01@gmail.com',
             license='MIT',
```

