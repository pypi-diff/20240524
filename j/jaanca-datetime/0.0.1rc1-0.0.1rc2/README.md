# Comparing `tmp/jaanca_datetime-0.0.1rc1.tar.gz` & `tmp/jaanca_datetime-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_datetime-0.0.1rc1.tar", last modified: Fri May 24 19:50:35 2024, max compression
+gzip compressed data, was "jaanca_datetime-0.0.1rc2.tar", last modified: Fri May 24 20:04:47 2024, max compression
```

## Comparing `jaanca_datetime-0.0.1rc1.tar` & `jaanca_datetime-0.0.1rc2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 19:50:35.957698 jaanca_datetime-0.0.1rc1/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_datetime-0.0.1rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     4040 2024-05-24 19:50:35.956694 jaanca_datetime-0.0.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0     2753 2024-05-24 19:46:45.000000 jaanca_datetime-0.0.1rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 19:50:35.937693 jaanca_datetime-0.0.1rc1/jaanca_datetime/
--rw-rw-rw-   0        0        0      113 2024-05-24 19:50:22.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 19:50:35.948693 jaanca_datetime-0.0.1rc1/jaanca_datetime/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 19:50:35.951695 jaanca_datetime-0.0.1rc1/jaanca_datetime/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     3574 2024-05-24 19:48:25.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime/utils/helpers/datetime_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-24 19:50:35.954694 jaanca_datetime-0.0.1rc1/jaanca_datetime.egg-info/
--rw-rw-rw-   0        0        0     4040 2024-05-24 19:50:35.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-05-24 19:50:35.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 19:50:35.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-24 19:50:35.000000 jaanca_datetime-0.0.1rc1/jaanca_datetime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 19:50:35.958360 jaanca_datetime-0.0.1rc1/setup.cfg
--rw-rw-rw-   0        0        0     1622 2024-05-24 19:41:38.000000 jaanca_datetime-0.0.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:04:47.276449 jaanca_datetime-0.0.1rc2/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_datetime-0.0.1rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3930 2024-05-24 20:04:47.275448 jaanca_datetime-0.0.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     2614 2024-05-24 19:52:28.000000 jaanca_datetime-0.0.1rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:04:47.255866 jaanca_datetime-0.0.1rc2/jaanca_datetime/
+-rw-rw-rw-   0        0        0      113 2024-05-24 19:50:22.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:04:47.268454 jaanca_datetime-0.0.1rc2/jaanca_datetime/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:04:47.271451 jaanca_datetime-0.0.1rc2/jaanca_datetime/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3574 2024-05-24 20:04:16.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime/utils/helpers/datetime_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:04:47.274448 jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/
+-rw-rw-rw-   0        0        0     3930 2024-05-24 20:04:47.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-24 20:04:47.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:04:47.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-24 20:04:47.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 20:04:47.000000 jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:04:47.277448 jaanca_datetime-0.0.1rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1636 2024-05-24 19:54:31.000000 jaanca_datetime-0.0.1rc2/setup.py
```

### Comparing `jaanca_datetime-0.0.1rc1/LICENSE.txt` & `jaanca_datetime-0.0.1rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_datetime-0.0.1rc1/PKG-INFO` & `jaanca_datetime-0.0.1rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-datetime
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A tool library created by jaanca with help functions for date and time management and moving dates between time days by UTC.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pytz>=2024.1
 
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-datetime" target="_blank">
@@ -41,16 +42,15 @@
 </p>
 
 
 ---
 
 #  A tool library created by jaanca
 
-* **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
-* **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
+* **Python library**: A tool library created by jaanca with help functions for date and time management and moving dates between time days by UTC.
 
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime)
 | [Package (PyPI)](https://pypi.org/project/jaanca-datetime/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime/samples)
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-datetime Version: 0.0.1rc1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-datetime Version: 0.0.1rc2 Summary: A tool
 library created by jaanca with help functions for date and time management and
 moving dates between time days by UTC. Home-page: https://github.com/jaanca/
 python-libraries/tree/main/jaanca-datetime Author: Jaime Andres Cardona
 Carrillo Author-email: jacardona@outlook.com License: MIT License Keywords:
 datetime,utc Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
@@ -10,39 +10,37 @@
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
 :: System :: Monitoring Classifier: Topic :: Software Development Classifier:
 Typing :: Typed Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE.txt Requires-Dist: pytz>=2024.1
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
-created by jaanca that allows measuring the time between two moments in the
-source code. * **Analyze results in database**: The output format can be
-inserted in an INTERVAL attribute for example in PostgreSQL and add the time of
-several processes. [Source code](https://github.com/jaanca/python-libraries/
-tree/main/jaanca-datetime) | [Package (PyPI)](https://pypi.org/project/jaanca-
-datetime/) | [Samples](https://github.com/jaanca/python-libraries/tree/main/
-jaanca-datetime/samples) --- # library installation ```console pip install
-jaanca-datetime --upgrade ``` --- # Example of use ```python ``` --- # Semantic
-Versioning jaanca-datetime < MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version
-when you make incompatible API changes * **MINOR**: version when you add
-functionality in a backwards compatible manner * **PATCH**: version when you
-make backwards compatible bug fixes ## Definitions for releasing versions *
-https://peps.python.org/pep-0440/ - X.YaN (Alpha release): Identify and fix
-early-stage bugs. Not suitable for production use. - X.YbN (Beta release):
-Stabilize and refine features. Address reported bugs. Prepare for official
-release. - X.YrcN (Release candidate): Final version before official release.
-Assumes all major features are complete and stable. Recommended for testing in
-non-critical environments. - X.Y (Final release/Stable/Production): Completed,
-stable version ready for use in production. Full release for public use. --- #
-Changelog All notable changes to this project will be documented in this file.
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/
-), and this project adheres to [Semantic Versioning](https://semver.org/spec/
-v2.0.0.html). ## Types of changes - Added for new features. - Changed for
-changes in existing functionality. - Deprecated for soon-to-be removed
-features. - Removed for now removed features. - Fixed for any bug fixes. -
-Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-05-24 ### Added -
-First tests using pypi.org in develop environment. ## [0.1.0] - 2024-05-24 ###
-Added - Completion of testing and launch into production.
+created by jaanca with help functions for date and time management and moving
+dates between time days by UTC. [Source code](https://github.com/jaanca/python-
+libraries/tree/main/jaanca-datetime) | [Package (PyPI)](https://pypi.org/
+project/jaanca-datetime/) | [Samples](https://github.com/jaanca/python-
+libraries/tree/main/jaanca-datetime/samples) --- # library installation
+```console pip install jaanca-datetime --upgrade ``` --- # Example of use
+```python ``` --- # Semantic Versioning jaanca-datetime < MAJOR >.< MINOR >.<
+PATCH > * **MAJOR**: version when you make incompatible API changes *
+**MINOR**: version when you add functionality in a backwards compatible manner
+* **PATCH**: version when you make backwards compatible bug fixes ##
+Definitions for releasing versions * https://peps.python.org/pep-0440/ - X.YaN
+(Alpha release): Identify and fix early-stage bugs. Not suitable for production
+use. - X.YbN (Beta release): Stabilize and refine features. Address reported
+bugs. Prepare for official release. - X.YrcN (Release candidate): Final version
+before official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. --- # Changelog All notable changes to this project
+will be documented in this file. The format is based on [Keep a Changelog]
+(https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
+Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
+for new features. - Changed for changes in existing functionality. - Deprecated
+for soon-to-be removed features. - Removed for now removed features. - Fixed
+for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
+05-24 ### Added - First tests using pypi.org in develop environment. ## [0.1.0]
+- 2024-05-24 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_datetime-0.0.1rc1/README.md` & `jaanca_datetime-0.0.1rc2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 </p>
 
 
 ---
 
 #  A tool library created by jaanca
 
-* **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
-* **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
+* **Python library**: A tool library created by jaanca with help functions for date and time management and moving dates between time days by UTC.
 
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime)
 | [Package (PyPI)](https://pypi.org/project/jaanca-datetime/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime/samples)
 
 ---
```

#### html2text {}

```diff
@@ -1,31 +1,29 @@
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
-created by jaanca that allows measuring the time between two moments in the
-source code. * **Analyze results in database**: The output format can be
-inserted in an INTERVAL attribute for example in PostgreSQL and add the time of
-several processes. [Source code](https://github.com/jaanca/python-libraries/
-tree/main/jaanca-datetime) | [Package (PyPI)](https://pypi.org/project/jaanca-
-datetime/) | [Samples](https://github.com/jaanca/python-libraries/tree/main/
-jaanca-datetime/samples) --- # library installation ```console pip install
-jaanca-datetime --upgrade ``` --- # Example of use ```python ``` --- # Semantic
-Versioning jaanca-datetime < MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version
-when you make incompatible API changes * **MINOR**: version when you add
-functionality in a backwards compatible manner * **PATCH**: version when you
-make backwards compatible bug fixes ## Definitions for releasing versions *
-https://peps.python.org/pep-0440/ - X.YaN (Alpha release): Identify and fix
-early-stage bugs. Not suitable for production use. - X.YbN (Beta release):
-Stabilize and refine features. Address reported bugs. Prepare for official
-release. - X.YrcN (Release candidate): Final version before official release.
-Assumes all major features are complete and stable. Recommended for testing in
-non-critical environments. - X.Y (Final release/Stable/Production): Completed,
-stable version ready for use in production. Full release for public use. --- #
-Changelog All notable changes to this project will be documented in this file.
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/
-), and this project adheres to [Semantic Versioning](https://semver.org/spec/
-v2.0.0.html). ## Types of changes - Added for new features. - Changed for
-changes in existing functionality. - Deprecated for soon-to-be removed
-features. - Removed for now removed features. - Fixed for any bug fixes. -
-Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-05-24 ### Added -
-First tests using pypi.org in develop environment. ## [0.1.0] - 2024-05-24 ###
-Added - Completion of testing and launch into production.
+created by jaanca with help functions for date and time management and moving
+dates between time days by UTC. [Source code](https://github.com/jaanca/python-
+libraries/tree/main/jaanca-datetime) | [Package (PyPI)](https://pypi.org/
+project/jaanca-datetime/) | [Samples](https://github.com/jaanca/python-
+libraries/tree/main/jaanca-datetime/samples) --- # library installation
+```console pip install jaanca-datetime --upgrade ``` --- # Example of use
+```python ``` --- # Semantic Versioning jaanca-datetime < MAJOR >.< MINOR >.<
+PATCH > * **MAJOR**: version when you make incompatible API changes *
+**MINOR**: version when you add functionality in a backwards compatible manner
+* **PATCH**: version when you make backwards compatible bug fixes ##
+Definitions for releasing versions * https://peps.python.org/pep-0440/ - X.YaN
+(Alpha release): Identify and fix early-stage bugs. Not suitable for production
+use. - X.YbN (Beta release): Stabilize and refine features. Address reported
+bugs. Prepare for official release. - X.YrcN (Release candidate): Final version
+before official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. --- # Changelog All notable changes to this project
+will be documented in this file. The format is based on [Keep a Changelog]
+(https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
+Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
+for new features. - Changed for changes in existing functionality. - Deprecated
+for soon-to-be removed features. - Removed for now removed features. - Fixed
+for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
+05-24 ### Added - First tests using pypi.org in develop environment. ## [0.1.0]
+- 2024-05-24 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_datetime-0.0.1rc1/jaanca_datetime/utils/helpers/datetime_helper.py` & `jaanca_datetime-0.0.1rc2/jaanca_datetime/utils/helpers/datetime_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class DateTimeHelper:
     '''Description:
     Return current date in selected format
 
     ## Example:
     
     ```Python
-    from datetime_helper import DateTimeHelper, App, TimeZonesPytz
+    from jaanca_datetime import DateTimeHelper, App, TimeZonesPytz
 
     DateTimeHelper.print_console_timezones_pytz()
     print(f"date now: {DateTimeHelper.get_datetime_now(App.Time.POSTGRESQL_FORMAT_DATE,is_format_string=False)}")
     print(f"date timezone convert UTC to Bogotá: {DateTimeHelper.get_datetime_now_to_another_location(App.Time.STANDARD_FORMAT_DATE,TimeZonesPytz.US.AZURE_DEFAULT,TimeZonesPytz.America.BOGOTA)}")
     ```
     '''
     @classmethod
@@ -34,15 +34,15 @@
         Get the current time in type datetime.datetime or string format defined in the constant App.Time.FORMAT_DATE
         :param format_date:bool: example %Y-%m-%d %H:%M:%S
         :param is_format_string:str: if True return str format, otherwise format datetime.datetime
 
         ## Example
 
         ```Python
-        from datetime_helper import DateTimeHelper, App
+        from jaanca_datetime import DateTimeHelper, App
 
         print(f"date now: {DateTimeHelper.get_datetime_now(App.Time.POSTGRESQL_FORMAT_DATE,is_format_string=False)}")
         ```
         '''
         date_now=datetime.now()
         if is_format_string is True:
             date_now_with_format = date_now.strftime(format_date)
@@ -63,15 +63,15 @@
         :param origin_location:str: Known time zone where the current server is configured, example: America/Bogota
         :param destination_location:str: Time zone to which the current date is to be transformed, example: Canada/Eastern
         :param is_format_string:bool: if True return str format, otherwise format datetime.datetime
 
         ## Example
 
         ```Python
-        from datetime_helper import DateTimeHelper, App, TimeZonesPytz
+        from jaanca_datetime import DateTimeHelper, App, TimeZonesPytz
         
         print(f"date timezone convert UTC to Bogotá: {DateTimeHelper.get_datetime_now_to_another_location(App.Time.STANDARD_FORMAT_DATE,TimeZonesPytz.US.AZURE_DEFAULT,TimeZonesPytz.America.BOGOTA)}")
         ```
 
         '''
         date_now = datetime.now()
         date_origin:datetime = pytz.timezone(origin_location).localize(date_now)
```

### Comparing `jaanca_datetime-0.0.1rc1/jaanca_datetime.egg-info/PKG-INFO` & `jaanca_datetime-0.0.1rc2/jaanca_datetime.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-datetime
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A tool library created by jaanca with help functions for date and time management and moving dates between time days by UTC.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pytz>=2024.1
 
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-datetime" target="_blank">
@@ -41,16 +42,15 @@
 </p>
 
 
 ---
 
 #  A tool library created by jaanca
 
-* **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
-* **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
+* **Python library**: A tool library created by jaanca with help functions for date and time management and moving dates between time days by UTC.
 
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime)
 | [Package (PyPI)](https://pypi.org/project/jaanca-datetime/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-datetime/samples)
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-datetime Version: 0.0.1rc1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-datetime Version: 0.0.1rc2 Summary: A tool
 library created by jaanca with help functions for date and time management and
 moving dates between time days by UTC. Home-page: https://github.com/jaanca/
 python-libraries/tree/main/jaanca-datetime Author: Jaime Andres Cardona
 Carrillo Author-email: jacardona@outlook.com License: MIT License Keywords:
 datetime,utc Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
@@ -10,39 +10,37 @@
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
 :: System :: Monitoring Classifier: Topic :: Software Development Classifier:
 Typing :: Typed Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE.txt Requires-Dist: pytz>=2024.1
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
-created by jaanca that allows measuring the time between two moments in the
-source code. * **Analyze results in database**: The output format can be
-inserted in an INTERVAL attribute for example in PostgreSQL and add the time of
-several processes. [Source code](https://github.com/jaanca/python-libraries/
-tree/main/jaanca-datetime) | [Package (PyPI)](https://pypi.org/project/jaanca-
-datetime/) | [Samples](https://github.com/jaanca/python-libraries/tree/main/
-jaanca-datetime/samples) --- # library installation ```console pip install
-jaanca-datetime --upgrade ``` --- # Example of use ```python ``` --- # Semantic
-Versioning jaanca-datetime < MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version
-when you make incompatible API changes * **MINOR**: version when you add
-functionality in a backwards compatible manner * **PATCH**: version when you
-make backwards compatible bug fixes ## Definitions for releasing versions *
-https://peps.python.org/pep-0440/ - X.YaN (Alpha release): Identify and fix
-early-stage bugs. Not suitable for production use. - X.YbN (Beta release):
-Stabilize and refine features. Address reported bugs. Prepare for official
-release. - X.YrcN (Release candidate): Final version before official release.
-Assumes all major features are complete and stable. Recommended for testing in
-non-critical environments. - X.Y (Final release/Stable/Production): Completed,
-stable version ready for use in production. Full release for public use. --- #
-Changelog All notable changes to this project will be documented in this file.
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/
-), and this project adheres to [Semantic Versioning](https://semver.org/spec/
-v2.0.0.html). ## Types of changes - Added for new features. - Changed for
-changes in existing functionality. - Deprecated for soon-to-be removed
-features. - Removed for now removed features. - Fixed for any bug fixes. -
-Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-05-24 ### Added -
-First tests using pypi.org in develop environment. ## [0.1.0] - 2024-05-24 ###
-Added - Completion of testing and launch into production.
+created by jaanca with help functions for date and time management and moving
+dates between time days by UTC. [Source code](https://github.com/jaanca/python-
+libraries/tree/main/jaanca-datetime) | [Package (PyPI)](https://pypi.org/
+project/jaanca-datetime/) | [Samples](https://github.com/jaanca/python-
+libraries/tree/main/jaanca-datetime/samples) --- # library installation
+```console pip install jaanca-datetime --upgrade ``` --- # Example of use
+```python ``` --- # Semantic Versioning jaanca-datetime < MAJOR >.< MINOR >.<
+PATCH > * **MAJOR**: version when you make incompatible API changes *
+**MINOR**: version when you add functionality in a backwards compatible manner
+* **PATCH**: version when you make backwards compatible bug fixes ##
+Definitions for releasing versions * https://peps.python.org/pep-0440/ - X.YaN
+(Alpha release): Identify and fix early-stage bugs. Not suitable for production
+use. - X.YbN (Beta release): Stabilize and refine features. Address reported
+bugs. Prepare for official release. - X.YrcN (Release candidate): Final version
+before official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. --- # Changelog All notable changes to this project
+will be documented in this file. The format is based on [Keep a Changelog]
+(https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
+Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
+for new features. - Changed for changes in existing functionality. - Deprecated
+for soon-to-be removed features. - Removed for now removed features. - Fixed
+for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
+05-24 ### Added - First tests using pypi.org in develop environment. ## [0.1.0]
+- 2024-05-24 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_datetime-0.0.1rc1/setup.py` & `jaanca_datetime-0.0.1rc2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-datetime"
-VERSION = "0.0.1rc1"
+VERSION = "0.0.1rc2"
 
-install_requires = []
+install_requires = ["pytz>=2024.1"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with help functions for date and time management and moving dates between time days by UTC.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

