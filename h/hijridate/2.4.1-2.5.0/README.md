# Comparing `tmp/hijridate-2.4.1.tar.gz` & `tmp/hijridate-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijridate-2.4.1.tar", last modified: Sat Dec  9 05:33:26 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hijridate-2.4.1.tar` & `hijridate-2.5.0.tar`

### file list

```diff
@@ -1,34 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.427501 hijridate-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2023-12-09 05:33:19.000000 hijridate-2.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-09 05:33:19.000000 hijridate-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-09 05:33:19.000000 hijridate-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-12-09 05:33:26.427501 hijridate-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-12-09 05:33:19.000000 hijridate-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-09 05:33:19.000000 hijridate-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-12-09 05:33:26.427501 hijridate-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-09 05:33:19.000000 hijridate-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.423501 hijridate-2.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.423501 hijridate-2.4.1/src/hijridate/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-09 05:33:19.000000 hijridate-2.4.1/src/hijridate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2023-12-09 05:33:19.000000 hijridate-2.4.1/src/hijridate/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-09 05:33:19.000000 hijridate-2.4.1/src/hijridate/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2023-12-09 05:33:19.000000 hijridate-2.4.1/src/hijridate/locales.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-09 05:33:19.000000 hijridate-2.4.1/src/hijridate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2023-12-09 05:33:19.000000 hijridate-2.4.1/src/hijridate/ummalqura.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.427501 hijridate-2.4.1/src/hijridate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-12-09 05:33:26.000000 hijridate-2.4.1/src/hijridate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-09 05:33:26.000000 hijridate-2.4.1/src/hijridate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 05:33:26.000000 hijridate-2.4.1/src/hijridate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 05:33:26.000000 hijridate-2.4.1/src/hijridate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-09 05:33:26.000000 hijridate-2.4.1/src/hijridate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.423501 hijridate-2.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.423501 hijridate-2.4.1/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.427501 hijridate-2.4.1/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)    20308 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/integration/fixtures/kfupm_comparison_calendar.json
--rw-r--r--   0 runner    (1001) docker     (127)    25374 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/integration/fixtures/ummalqura_calendar_website.json
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/integration/fixtures/ummalqura_newspaper_issues.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     1274 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/integration/test_month_starts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 05:33:26.427501 hijridate-2.4.1/tests/unit/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6741 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/unit/test_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/unit/test_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1781 2023-12-09 05:33:19.000000 hijridate-2.4.1/tests/unit/test_locales.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hijridate-2.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hijridate-2.5.0/README.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/_version.py
+-rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/convert.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/helpers.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/locales.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/py.typed
+-rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 hijridate-2.5.0/src/hijridate/ummalqura.py
+-rwxr-xr-x   0        0        0     1552 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/integration/test_lengths.py
+-rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/integration/test_references.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/integration/fixtures/kfupm_comparison_calendar.json
+-rw-r--r--   0        0        0    25374 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/integration/fixtures/ummalqura_calendar_website.json
+-rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/integration/fixtures/ummalqura_newspaper_issues.json
+-rwxr-xr-x   0        0        0     7290 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/unit/test_convert.py
+-rwxr-xr-x   0        0        0      374 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/unit/test_helpers.py
+-rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 hijridate-2.5.0/tests/unit/test_locales.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hijridate-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 hijridate-2.5.0/LICENSE
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 hijridate-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 hijridate-2.5.0/PKG-INFO
```

### Comparing `hijridate-2.4.1/CHANGELOG.md` & `hijridate-2.5.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,202 +1,186 @@
 # Changelog
 
-The versioning scheme is compliant with the [PEP 440] specification.
+The versioning scheme is compliant with the [PEP 440](https://peps.python.org/pep-0440/#public-version-identifiers) specification.
 
-[PEP 440]: https://peps.python.org/pep-0440/#public-version-identifiers
+## 2.5.0 - 2024-05-25
 
-## 2.4.1 (2023-12-09)
+- Added a new function called `year_length()`, which calculates the total number of days in a Hijri year.
+- Changed the `validate` argument when instantiating Hijri objects to be a keyword-only argument.
+- Changed the `padding` argument for `dmyformat()` functions to be a keyword-only argument.
+- Improved exception messages to display the values provided by the user.
+- Improved type hints for supported natural languages.
+- Improved readability and documentation of several functions.
+- Improved reliability of some tests.
+- Fixed typos in English Hijri month names.
+- Fixed miscellaneous formatting and linting issues.
+- Published the package on [Zenodo](https://zenodo.org/records/11200950) to become citable by researchers.
+- Updated development tools, workflows, and documentation.
+
+## 2.4.1 - 2023-12-09
 
 - Fixed some typos.
 
-## 2.4.0 (2023-12-08)
+## 2.4.0 - 2023-12-08
 
 - Dropped support for Python 3.7 and added support for Python 3.12.
-- Fixed a typo in the Bangla translation. (By [@nokibsarkar] in [#18])
-- Changed documentation theme along with other enhancements.
 
-[#18]: https://github.com/dralshehri/hijridate/pull/18
-[@nokibsarkar]: https://github.com/nokibsarkar
+### Subheading
 
-## 2.3.0 (2023-04-24)
+- Fixed a typo in the Bangla translation. (By [@nokibsarkar](https://github.com/nokibsarkar) in [#18](https://github.com/dralshehri/hijridate/pull/18))
+- Changed documentation theme along with other enhancements.
+
+## 2.3.0 - 2023-04-24
 
 **IMPORTANT**
 
-The `hijri-converter` package has been **renamed** to `hijridate` in preparation
-for the upcoming major update.
+The `hijri-converter` package has been **renamed** to `hijridate` in preparation for the upcoming major update.
 
-Please use a version specifier e.g. `hijridate~=2.3.0` to avoid any breaking
-changes in the future.
+Please use a version specifier e.g. `hijridate~=2.3.0` to avoid any breaking changes in the future.
 
 ### What's Changed
 
 - Renamed the package to `hijridate` and deprecated the old name.
 - Dropped support for Python 3.6 and added support for Python 3.11.
 - Updated documentation and removed badges from the package description.
 - Updated development configurations and GitHub actions.
 - Changed GitHub username back to @dralshehri and updated related links.
 
-## 2.2.4 (2022-05-23)
+## 2.2.4 - 2022-05-23
 
 - Added more classifiers to package configuration.
-- Fixed location of type-checking marker file. (By [@dimbleby] in [#10])
+- Fixed location of type-checking marker file. (By [@dimbleby](https://github.com/dimbleby) in [#10](https://github.com/dralshehri/hijridate/pull/10))
 - Updated development and build requirements.
 
-[#10]: https://github.com/dralshehri/hijridate/pull/10
-[@dimbleby]: https://github.com/dimbleby
-
-## 2.2.3 (2022-02-12)
+## 2.2.3 - 2022-02-12
 
 - Changed package docstrings to Google style and updated documentation.
 - Updated development workflows and configurations.
 - Other minor fixes and enhancements.
 - Changed GitHub username to @mhalshehri and updated related links.
 
-## 2.2.2 (2021-09-25)
+## 2.2.2 - 2021-09-25
 
 - Added some missing variable annotations to `ummalqura` module.
 - Fixed an issue when generating documentation.
 - Fixed some typos in docstrings and improved documentation.
 - Other minor fixes and enhancements.
 
-## 2.2.1 (2021-09-04)
+## 2.2.1 - 2021-09-04
 
 - Fixed calculation of month 12 of the year 1354 AH.
-- Fixed an issue when generating documentation without the package being
-  installed. ([#7])
+- Fixed an issue when generating documentation without the package being installed. ([#7](https://github.com/dralshehri/hijridate/issues/7))
 - Refactored internal helper functions.
 - Updated and improved tests and documentation.
 - Fixed some typos.
 
-[#7]: https://github.com/dralshehri/hijridate/issues/7
+## 2.2.0 - 2021-08-16
 
-## 2.2.0 (2021-08-16)
-
-- Added `today()` classmethod to Hijri class to get the Hijri Object of today's
-  date.
-- Added `separator` and `padding` parameters to `dmyformat()` method to have
-  more control over formatting.
-- Refactored locales for better management and testing. (Inspired by [Arrow]
-  localization)
-- Updated main classes to be conveniently imported into the package level e.g.
-  `from hijri_converter import Hijri, Gregorian`.
+- Added `today()` classmethod to Hijri class to get the Hijri Object of today's date.
+- Added `separator` and `padding` parameters to `dmyformat()` method to have more control over formatting.
+- Refactored locales for better management and testing. (Inspired by [Arrow](https://github.com/arrow-py/arrow) localization)
+- Updated main classes to be conveniently imported into the package level e.g. `from hijri_converter import Hijri, Gregorian`.
 - Removed deprecated method `slashformat()` from Hijri and Gregorian classes.
 - Updated tests and documentation.
 - Other minor fixes and internal enhancements.
 
-[arrow]: https://github.com/arrow-py/arrow
-
-## 2.1.3 (2021-06-22)
+## 2.1.3 - 2021-06-22
 
 - Minor fixes and enhancements for docstrings and documentation.
 
-## 2.1.2 (2021-05-30)
+## 2.1.2 - 2021-05-30
 
-- Added Bangla translation. (By [@nokibsarkar] in [#4])
-- Changed `Hijri` rich comparison to return `NotImplemented` when the second
-  operand is not `Hijri` class.
+- Added Bangla translation. (By [@nokibsarkar](https://github.com/nokibsarkar) in [#4](https://github.com/dralshehri/hijridate/pull/4))
+- Changed `Hijri` rich comparison to return `NotImplemented` when the second operand is not `Hijri` class.
 - Changed `ummalqura` constants to be in capital letters adhering to PEP8.
 - Updated packaging configuration files and local development workflow.
 - Other minor fixes and documentation enhancements.
 
-[#4]: https://github.com/dralshehri/hijridate/pull/4
-[@nokibsarkar]: https://github.com/nokibsarkar
-
-## 2.1.1 (2020-05-21)
+## 2.1.1 - 2020-05-21
 
 - Added `dmyformat()` to return dates in `DD/MM/YYYY` format.
 - Deprecated `slashformat()` method to be replaced by `dmyformat()` method.
-- Fixed PyPI package not including some required files. ([#3])
+- Fixed PyPI package not including some required files. ([#3](https://github.com/dralshehri/hijridate/issues/3))
 - Fixed some typos.
 - Updated tests.
 
-[#3]: https://github.com/dralshehri/hijridate/issues/3
-
-## 2.1.0 (2019-06-16)
+## 2.1.0 - 2019-06-16
 
-This version has more accurate conversion and better internal code. Details are
-as follows:
+This version has more accurate conversion and better internal code. Details are as follows:
 
-- Dropped support for the years before 1343 AH because the Umm al-Qura calendar
-  was not established then.
-- Added `validate` parameter to Hijri class for optional disabling of Hijri date
-  validation and improving performance. However, disabling validation will
-  decrease the conversion accuracy silently.
-- Verified conversion against original references and updated the `month_starts`
-  tuple for more accurate conversion.
+- Dropped support for the years before 1343 AH because the Umm al-Qura calendar was not established then.
+- Added `validate` parameter to Hijri class for optional disabling of Hijri date validation and improving performance. However, disabling validation will decrease the conversion accuracy silently.
+- Verified conversion against original references and updated the `month_starts` tuple for more accurate conversion.
 - Improved `Hijri` class rich comparison methods.
 - Improved date validation methods for better performance and readability.
 - Made the `Hijri` class hashable by adding a custom `__hash__` method.
 - Refactored many internal methods (not affecting the API).
 - Other minor fixes, enhancements and performance boost.
 
-## 2.0.0 (2019-06-05)
+## 2.0.0 - 2019-06-05
 
-In short, this version supports only lunar Hijri calendar on Python 3.6+, and
-the conversion is in complete agreement with the official Umm al-Qura calendar.
-Details are as follows:
+In short, this version supports only lunar Hijri calendar on Python 3.6+, and the conversion is in complete agreement with the official Umm al-Qura calendar. Details are as follows:
 
 - Renamed the package to `hijri-converter`.
 - Dropped support for the solar Hijri calendar.
 - Dropped support for Python 3.5.
 - Refactored localization and `ummalqura.py` module.
 - Updated `month_starts` tuple in alignment with the Umm al-Qura calendar.
 - Added `fromdate()` classmethod to `Gregorian` class.
 - Added `notation()` method to `Hijri` and `Gregorian` classes.
-- Added more methods to `Gregorian` class including `slashformat()`,
-  `month_name()`, `day_name()` and `to_julian()`.
+- Added more methods to `Gregorian` class including `slashformat()`, `month_name()`, `day_name()` and `to_julian()`.
 - Renamed `month_days()` method of `Hijri` class to `month_length()`.
 - Changed formatted string to use f-strings.
 - Improved documentation and examples.
 - Updated unit tests.
 - Fixed other minor issues and typos.
 
-## 1.5.0 (2018-12-27)
+## 1.5.0 - 2018-12-27
 
 - Added `fromisoformat()` classmethod to `Hijri` class.
 - Added support for rich comparison between Hijri dates.
 - Updated documentation and testing code.
 - Other minor fixes and enhancements.
 
-## 1.4.0 (2018-11-26)
+## 1.4.0 - 2018-11-26
 
 - Refactored conversion methods to improve performance.
 - Changed date validation back to be the default and removed optional parameter.
 - Added `to_julian()` method to `Hijri` class.
 - Updated documentation and testing code.
 - Other minor fixes and enhancements.
 
-## 1.3.3 (2018-11-21)
+## 1.3.3 - 2018-11-21
 
 - Fixed a bug in range validation for the Gregorian date.
 - Changed generic typing to built-in types.
 - Added more tests to cover the solar calendar.
 - Improved code structure and documentation.
 
-## 1.3.2 (2018-11-16)
+## 1.3.2 - 2018-11-16
 
 - Improved documentation and changelog.
 
-## 1.3.1 (2018-11-16)
+## 1.3.1 - 2018-11-16
 
 - Fixed README file.
 
-## 1.3.0 (2018-11-16)
+## 1.3.0 - 2018-11-16
 
 - Added documentation directory with an online version.
 - Changed date input validation to be optional and disabled by default.
 - Improved code readability and performance.
 - Other minor fixes and enhancements.
 
-## 1.2.0 (2018-11-09)
+## 1.2.0 - 2018-11-09
 
 - Added `slashformat()` method to `Hijri` class.
 - Improved date validation code.
 - Fixed some typos in documentation and docstrings.
 
-## 1.0.1 (2018-10-28)
+## 1.0.1 - 2018-10-28
 
 - Improved examples and documentation.
 
-## 1.0.0 (2018-10-28)
+## 1.0.0 - 2018-10-28
 
 - First release.
```

### Comparing `hijridate-2.4.1/LICENSE` & `hijridate-2.5.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 Mohammed Alshehri <https://www.dralshehri.com>
+Copyright (c) Mohammed Alshehri <https://www.dralshehri.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hijridate-2.4.1/PKG-INFO` & `hijridate-2.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hijridate
-Version: 2.4.1
-Summary: Accurate Hijri-Gregorian dates converter based on the Umm al-Qura calendar
-Home-page: https://github.com/dralshehri/hijridate
-Author: Mohammed Alshehri
-Author-email: 
-License: MIT
+Version: 2.5.0
+Summary: Accurate Hijri-Gregorian dates converter based on Umm al-Qura calendar
+Project-URL: Source, https://github.com/dralshehri/hijridate
+Project-URL: Changelog, https://github.com/dralshehri/hijridate/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://hijridate.readthedocs.io
-Project-URL: Source Code, https://github.com/dralshehri/hijridate
-Keywords: hijri,gregorian,date,converter,ummalqura,saudi,calendar
+Author: Mohammed Alshehri
+License: MIT License
+License-File: LICENSE
+Keywords: calendar,conversion,converter,date,gregorian,hijri,ummalqura,ummulqura
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Legal Industry
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Arabic
 Classifier: Natural Language :: Bengali
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -29,44 +29,38 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # HijriDate
 
 > formerly `hijri-converter`
 
-A Python package to convert accurately between Hijri and Gregorian dates using
-the Umm al-Qura calendar.
+HijriDate is a Python package for converting between Hijri and Gregorian dates using the Umm al-Qura calendar. The package has been thoroughly verified and tested against original references to ensure its accuracy and reliability. It has an intuitive design, allows rich comparison and basic formatting of Hijri dates, and is optimized for performance.
 
 ## Features
 
-- Accurate and verified date conversion.
+- Accurate and verified Hijri-Gregorian date conversion.
 - Optimized code performance compared to similar packages.
 - Intuitive, clean, and easy-to-use interface.
 - Most of the methods and formats are similar to those of standard library.
-- Multilingual representation of weekday names, months, and calendar era
-  notations.
+- Multilingual representation of weekday names, months, and calendar era notations.
 - Easily extendable to support other natural languages.
 - Rich comparison between dates.
 - Validation of input dates.
 - Works on Python 3.8+ with zero dependencies.
 - Thoroughly tested with 100% test coverage.
 
 ## Limitations
 
-- The date range supported by converter is limited to the period from the
-  beginning of 1343 AH (1 August 1924 CE) to the end of 1500 AH (16 November
-  2077 CE).
-- The conversion is not intended for religious purposes where sighting of the
-  lunar crescent at the beginning of Hijri month is still preferred.
+- The date range supported by converter is limited to the period from the beginning of 1343 AH (1 August 1924 CE) to the end of 1500 AH (16 November 2077 CE).
+- The conversion is not intended for religious purposes where sighting of the lunar crescent at the beginning of Hijri month is still preferred.
 
 ## Installation
 
 To install using `pip`, run:
 
 ```shell
 pip install hijridate
@@ -88,20 +82,25 @@
 
 # Convert a Gregorian date to Hijri
 h = Gregorian(1982, 12, 2).to_hijri()
 ```
 
 ## Documentation
 
-Please see <https://hijridate.readthedocs.io> for full documentation of this
-package, including background, benchmarking, usage examples and API reference.
+Please refer to <https://hijridate.readthedocs.io> for complete documentation on this package, which includes background information, benchmarking, usage examples, and API reference.
+
+## Contributing
+
+If you're interested in contributing, please check out the [Contributing](https://github.com/dralshehri/hijridate/blob/main/CONTRIBUTING.md) guide for more information on how you can help!
 
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Acknowledgements
 
-- [R.H. van Gent](http://www.staff.science.uu.nl/~gent0113) &mdash; inspiration,
-  scientific guidance and resources.
-- [@AZalshehri7](https://github.com/AZalshehri7) &mdash; support in dates review
-  and conversion accuracy verification.
+- [R.H. van Gent](http://www.staff.science.uu.nl/~gent0113) &mdash; inspiration, scientific guidance and resources.
+- [@AZalshehri7](https://github.com/AZalshehri7) &mdash; support in dates review and conversion accuracy verification.
+
+## Citation
+
+If you plan to cite this project in your academic publication, please refer to <https://doi.org/10.5281/zenodo.11200950> for citation information.
```

### Comparing `hijridate-2.4.1/README.md` & `hijridate-2.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,50 @@
 # HijriDate
 
 <!-- start description -->
 
 > formerly `hijri-converter`
 
-A Python package to convert accurately between Hijri and Gregorian dates using
-the Umm al-Qura calendar.
+HijriDate is a Python package for converting between Hijri and Gregorian dates using the Umm al-Qura calendar. The package has been thoroughly verified and tested against original references to ensure its accuracy and reliability. It has an intuitive design, allows rich comparison and basic formatting of Hijri dates, and is optimized for performance.
 
 <!-- end description -->
 
 <!-- start badges -->
 
-[![Release Status](https://img.shields.io/github/actions/workflow/status/dralshehri/hijridate/release.yml?label=release)][release]
-[![Coverage Status](https://img.shields.io/badge/coverage-100%25-success)][coverage]
-[![Code Quality](https://img.shields.io/codefactor/grade/github/dralshehri/hijridate/main?&label=codefactor)][quality]
-[![Docs Status](https://img.shields.io/readthedocs/hijridate/stable)][docs]
-[![PyPI Downloads](https://img.shields.io/pypi/dm/hijri-converter?color=blue)][downloads]
-[![PyPI Version](https://img.shields.io/pypi/v/hijridate)][pypi-version]
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/hijridate)][conda-version]
-[![Package License](https://img.shields.io/github/license/dralshehri/hijridate)][license]
-
-[release]: https://github.com/dralshehri/hijridate/actions/workflows/release.yml
-[coverage]:
-  https://github.com/dralshehri/hijridate/actions/workflows/release.yml
-[quality]:
-  https://www.codefactor.io/repository/github/dralshehri/hijridate/overview/main
-[docs]: https://hijridate.readthedocs.io
+[![Release Status](https://img.shields.io/github/actions/workflow/status/dralshehri/hijridate/package-release.yml?label=release)][release] [![Coverage Status](https://img.shields.io/badge/coverage-100%25-success)][coverage] [![PyPI Downloads](https://img.shields.io/pypi/dm/hijri-converter?color=blue)][downloads] [![PyPI Version](https://img.shields.io/pypi/v/hijridate)][pypi-version] [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hijridate)][conda-version] [![Package License](https://img.shields.io/github/license/dralshehri/hijridate)][license] [![Package DOI](https://img.shields.io/badge/doi-10.5281%2Fzenodo.11200950-blue) ][doi]
+
+[release]: https://github.com/dralshehri/hijridate/actions/workflows/pypi-release.yml
+[coverage]: https://github.com/dralshehri/hijridate/actions/workflows/pypi-release.yml
 [downloads]: https://pypistats.org/packages/hijri-converter
 [pypi-version]: https://pypi.python.org/pypi/hijridate
 [conda-version]: https://anaconda.org/conda-forge/hijridate
 [license]: https://github.com/dralshehri/hijridate/blob/main/LICENSE
+[doi]: https://doi.org/10.5281/zenodo.11200950
 
 <!-- end badges -->
 
 <!-- start summary -->
 
 ## Features
 
-- Accurate and verified date conversion.
+- Accurate and verified Hijri-Gregorian date conversion.
 - Optimized code performance compared to similar packages.
 - Intuitive, clean, and easy-to-use interface.
 - Most of the methods and formats are similar to those of standard library.
-- Multilingual representation of weekday names, months, and calendar era
-  notations.
+- Multilingual representation of weekday names, months, and calendar era notations.
 - Easily extendable to support other natural languages.
 - Rich comparison between dates.
 - Validation of input dates.
 - Works on Python 3.8+ with zero dependencies.
 - Thoroughly tested with 100% test coverage.
 
 ## Limitations
 
-- The date range supported by converter is limited to the period from the
-  beginning of 1343 AH (1 August 1924 CE) to the end of 1500 AH (16 November
-  2077 CE).
-- The conversion is not intended for religious purposes where sighting of the
-  lunar crescent at the beginning of Hijri month is still preferred.
+- The date range supported by converter is limited to the period from the beginning of 1343 AH (1 August 1924 CE) to the end of 1500 AH (16 November 2077 CE).
+- The conversion is not intended for religious purposes where sighting of the lunar crescent at the beginning of Hijri month is still preferred.
 
 ## Installation
 
 To install using `pip`, run:
 
 ```shell
 pip install hijridate
@@ -83,20 +68,27 @@
 h = Gregorian(1982, 12, 2).to_hijri()
 ```
 
 <!-- end summary -->
 
 ## Documentation
 
-Please see <https://hijridate.readthedocs.io> for full documentation of this
-package, including background, benchmarking, usage examples and API reference.
+Please refer to <https://hijridate.readthedocs.io> for complete documentation on this package, which includes background information, benchmarking, usage examples, and API reference.
+
+## Contributing
+
+If you're interested in contributing, please check out the [Contributing](https://github.com/dralshehri/hijridate/blob/main/CONTRIBUTING.md) guide for more information on how you can help!
 
 ## License
 
 This project is licensed under the terms of the MIT license.
 
+<!-- start attrs -->
+
 ## Acknowledgements
 
-- [R.H. van Gent](http://www.staff.science.uu.nl/~gent0113) &mdash; inspiration,
-  scientific guidance and resources.
-- [@AZalshehri7](https://github.com/AZalshehri7) &mdash; support in dates review
-  and conversion accuracy verification.
+- [R.H. van Gent](http://www.staff.science.uu.nl/~gent0113) &mdash; inspiration, scientific guidance and resources.
+- [@AZalshehri7](https://github.com/AZalshehri7) &mdash; support in dates review and conversion accuracy verification.
+
+## Citation
+
+If you plan to cite this project in your academic publication, please refer to <https://doi.org/10.5281/zenodo.11200950> for citation information.
```

### Comparing `hijridate-2.4.1/src/hijridate/convert.py` & `hijridate-2.5.0/src/hijridate/convert.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-"""Main module of the hijridate package."""
+"""Main module of the HijriDate package."""
 
 import datetime
+
 from bisect import bisect
 from typing import Tuple
 
 from hijridate import helpers, locales, ummalqura
 
 
 class Hijri:
-    """A Hijri object represents a date (year, month and day) in lunar Hijri
-    calendar.
+    """A Hijri object represents a date in lunar Hijri calendar.
+
+    Args:
+        year: Hijri year.
+        month: Hijri month.
+        day: Hijri day.
+        validate: Whether to validate Hijri input or not. It's recommended
+            to keep the default for accurate conversion.
+
+    Raises:
+        OverflowError: When ``year`` is out of supported Hijri range.
+        ValueError: When ``month`` is not within the range of `1-12`.
+        ValueError: When ``day`` is not within the range of
+            `1-month_length` for month.
     """
 
     __slots__ = "_year", "_month", "_day"
 
-    def __init__(self, year: int, month: int, day: int, validate: bool = True):
-        """
-        Args:
-            year: Hijri year.
-            month: Hijri month.
-            day: Hijri day.
-            validate: Whether to validate Hijri input or not. It's recommended
-                to keep the default for accurate conversion.
-
-        Raises:
-            OverflowError: When ``year`` is out of supported Hijri range.
-            ValueError: When ``month`` is not within the range of `1..12`.
-            ValueError: When ``day`` is not within the range of
-                `1..month_length` for month.
-        """
-
+    def __init__(self, year: int, month: int, day: int, *, validate: bool = True):
         self._year = year
         self._month = month
         self._day = day
 
         if validate:
             self._check_date()
 
@@ -71,34 +69,24 @@
         if not isinstance(other, Hijri):
             return NotImplemented
         return self._compare(other) <= 0
 
     def _compare(self, other: "Hijri") -> int:
         self_date = self.datetuple()
         other_date = other.datetuple()
-        return (
-            0
-            if self_date == other_date
-            else 1
-            if self_date > other_date
-            else -1
-        )
+        return 0 if self_date == other_date else 1 if self_date > other_date else -1
 
     @classmethod
     def fromisoformat(cls, date_string: str) -> "Hijri":
-        """Construct Hijri object from an ISO formatted Hijri date
-        ``YYYY-MM-DD``.
+        """Construct Hijri object from an ISO formatted Hijri date.
 
         Args:
             date_string: Hijri date in ISO format ``YYYY-MM-DD``.
         """
-
-        year = int(date_string[0:4])
-        month = int(date_string[5:7])
-        day = int(date_string[8:10])
+        year, month, day = map(int, date_string.split("-"))
         return cls(year, month, day)
 
     @classmethod
     def today(cls) -> "Hijri":
         """Construct Hijri object from today's date."""
         return Gregorian.today().to_hijri()
 
@@ -121,198 +109,190 @@
         """Return date as a tuple of (year, month, day)."""
         return self._year, self._month, self._day
 
     def isoformat(self) -> str:
         """Return date in ISO format i.e. ``YYYY-MM-DD``."""
         return f"{self._year:04}-{self._month:02}-{self._day:02}"
 
-    def dmyformat(self, separator: str = "/", padding: bool = True) -> str:
+    def dmyformat(self, separator: str = "/", *, padding: bool = True) -> str:
         """Return date in day-month-year format (``DD/MM/YYYY`` by default).
 
         Args:
             separator: String that separates the day, month, and year values.
             padding: Whether to add a leading zero as a padding character to
                 fill day and month values when less than 10.
         """
-
         day = f"{self._day:02}" if padding else self._day
         month = f"{self._month:02}" if padding else self._month
         return f"{day}{separator}{month}{separator}{self._year}"
 
+    def year_length(self) -> int:
+        """Return number of days in year."""
+        month_starts = ummalqura.MONTH_STARTS
+        first_index, last_index = self._year_indexes()
+        return month_starts[last_index + 1] - month_starts[first_index]
+
     def month_length(self) -> int:
         """Return number of days in month."""
         month_starts = ummalqura.MONTH_STARTS
         index = self._month_index()
-        length = month_starts[index + 1] - month_starts[index]
-        return length
+        return month_starts[index + 1] - month_starts[index]
 
-    def month_name(self, language: str = "en") -> str:
+    def month_name(self, language: locales.Language = "en") -> str:
         """Return month name.
 
         Args:
-            language: Language tag for localized month name. Full locale name
-                can be used, e.g. ``en-US`` or ``en_US.UTF-8``. Supported
-                languages are ``en``, ``ar`` and ``bn``.
+            language: Two-letter language code for localized month name.
         """
-
         return locales.get_locale(language).month_name(self._month)
 
     def weekday(self) -> int:
         """Return day of week, where Monday is 0 and Sunday is 6."""
         jdn = self.to_julian()
         return int(jdn % 7)
 
     def isoweekday(self) -> int:
         """Return day of week, where Monday is 1 and Sunday is 7."""
         jdn = self.to_julian()
         return int(jdn % 7) + 1
 
-    def day_name(self, language: str = "en") -> str:
+    def day_name(self, language: locales.Language = "en") -> str:
         """Return day name.
 
         Args:
-            language: Language tag for localized month name. Full locale name
-                can be used, e.g. ``en-US`` or ``en_US.UTF-8``. Supported
-                languages are ``en``, ``ar`` and ``bn``.
+            language: Two-letter language code for localized day name.
         """
-
         return locales.get_locale(language).day_name(self.isoweekday())
 
     @staticmethod
-    def notation(language: str = "en") -> str:
+    def notation(language: locales.Language = "en") -> str:
         """Return calendar era notation.
 
         Args:
-            language: Language tag for localized month name. Full locale name
-                can be used, e.g. ``en-US`` or ``en_US.UTF-8``. Supported
-                languages are ``en``, ``ar`` and ``bn``.
+            language: Two-letter language code for localized era notation.
         """
-
         return locales.get_locale(language).notation
 
     def to_julian(self) -> int:
         """Return corresponding Julian day number (JDN)."""
         month_starts = ummalqura.MONTH_STARTS
         index = self._month_index()
         rjd = month_starts[index] + self._day - 1
-        jdn = helpers.rjd_to_jdn(rjd)
-        return jdn
+        return helpers.rjd_to_jdn(rjd)
 
     def to_gregorian(self) -> "Gregorian":
         """Return Gregorian object for the corresponding Hijri date."""
-
         jdn = self.to_julian()
         ordinal = helpers.jdn_to_ordinal(jdn)
         return Gregorian.fromordinal(ordinal)
 
     def _check_date(self) -> None:
         """Check date values if within valid range."""
-
         # check year
-        min_year, max_year = [d[0] for d in ummalqura.HIJRI_RANGE]
+        min_year, max_year = (d[0] for d in ummalqura.HIJRI_RANGE)
         if not min_year <= self.year <= max_year:
-            raise OverflowError("date out of range")
+            message = f"year must be in {min_year}-{max_year}, got '{self.year}'"
+            raise OverflowError(message)
         # check month
         max_months = 12
         if not 1 <= self.month <= max_months:
-            raise ValueError(f"month must be in 1..{max_months}")
+            message = f"month must be in 1-{max_months}, got '{self.month}'"
+            raise ValueError(message)
         # check day
         month_length = self.month_length()
         if not 1 <= self.day <= month_length:
-            raise ValueError(f"day must be in 1..{month_length} for month")
+            message = f"day must be in 1-{month_length} for month, got '{self.day}'"
+            raise ValueError(message)
+
+    def _year_indexes(self) -> Tuple[int, int]:
+        """Return year's first and last indexes in ummalqura month starts."""
+        prior_months = (self.year - 1) * 12
+        first_index = prior_months - ummalqura.HIJRI_OFFSET
+        last_index = first_index + 11
+        return first_index, last_index
 
     def _month_index(self) -> int:
-        """Return month’s index in ummalqura month starts"""
+        """Return month's index in ummalqura month starts."""
         prior_months = ((self.year - 1) * 12) + self.month - 1
-        index = prior_months - ummalqura.HIJRI_OFFSET
-        return index
+        return prior_months - ummalqura.HIJRI_OFFSET
 
 
 class Gregorian(datetime.date):
-    """A Gregorian object represents a date (year, month and day) in Gregorian
-    calendar.
+    """A Gregorian object represents a date in Gregorian calendar.
+
+    Args:
+        year (int): Gregorian year.
+        month (int): Gregorian month.
+        day (int): Gregorian day.
     """
 
     __slots__ = ()
 
     @classmethod
     def fromdate(cls, date_object: datetime.date) -> "Gregorian":
         """Construct Gregorian object from a Python date object.
 
         Args:
             date_object: Python date object.
         """
-
         year, month, day = date_object.timetuple()[:3]
         return cls(year, month, day)
 
     def datetuple(self) -> Tuple[int, int, int]:
         """Return date as a tuple of (year, month, day)."""
         return self.year, self.month, self.day
 
-    def dmyformat(self, separator: str = "/", padding: bool = True) -> str:
+    def dmyformat(self, separator: str = "/", *, padding: bool = True) -> str:
         """Return date in day-month-year format (``DD/MM/YYYY`` by default).
 
         Args:
             separator: String that separates the day, month, and year values.
             padding: Whether to add a leading zero as a padding character to
                 fill day and month values when less than 10.
         """
-
         day = f"{self.day:02}" if padding else self.day
         month = f"{self.month:02}" if padding else self.month
         return f"{day}{separator}{month}{separator}{self.year}"
 
-    def month_name(self, language: str = "en") -> str:
+    def month_name(self, language: locales.Language = "en") -> str:
         """Return month name.
 
         Args:
-            language: Language tag for localized month name. Full locale name
-                can be used, e.g. ``en-US`` or ``en_US.UTF-8``. Supported
-                languages are ``en``, ``ar`` and ``bn``.
+            language: Two-letter language code for localized month name.
         """
-
         return locales.get_locale(language).gregorian_month_name(self.month)
 
-    def day_name(self, language: str = "en") -> str:
+    def day_name(self, language: locales.Language = "en") -> str:
         """Return day name.
 
         Args:
-            language: Language tag for localized month name. Full locale name
-                can be used, e.g. ``en-US`` or ``en_US.UTF-8``. Supported
-                languages are ``en``, ``ar`` and ``bn``.
+            language: Two-letter language code for localized day name.
         """
-
         return locales.get_locale(language).day_name(self.isoweekday())
 
     @staticmethod
-    def notation(language: str = "en") -> str:
+    def notation(language: locales.Language = "en") -> str:
         """Return calendar era notation.
 
         Args:
-            language: Language tag for localized month name. Full locale name
-                can be used, e.g. ``en-US`` or ``en_US.UTF-8``. Supported
-                languages are ``en``, ``ar`` and ``bn``.
+            language: Two-letter language code for localized era notation.
         """
-
         return locales.get_locale(language).gregorian_notation
 
     def to_julian(self) -> int:
         """Return corresponding Julian day number (JDN)."""
         ordinal = self.toordinal()
-        jdn = helpers.ordinal_to_jdn(ordinal)
-        return jdn
+        return helpers.ordinal_to_jdn(ordinal)
 
     def to_hijri(self) -> Hijri:
         """Return Hijri object for the corresponding Gregorian date.
 
         Raises:
             OverflowError: When date is out of supported Gregorian range.
         """
-
         self._check_range()
         jdn = self.to_julian()
         rjd = helpers.jdn_to_rjd(jdn)
         month_starts = ummalqura.MONTH_STARTS
         index = bisect(month_starts, rjd) - 1
         months = index + ummalqura.HIJRI_OFFSET
         years = int(months / 12)
@@ -321,8 +301,14 @@
         day = rjd - month_starts[index] + 1
         return Hijri(year, month, day, validate=False)
 
     def _check_range(self) -> None:
         """Check if Gregorian date is within valid range."""
         min_date, max_date = ummalqura.GREGORIAN_RANGE
         if not min_date <= (self.year, self.month, self.day) <= max_date:
-            raise OverflowError("date out of range")
+            min_date_iso = "-".join([f"{i:02}" for i in min_date])
+            max_date_iso = "-".join([f"{i:02}" for i in max_date])
+            message = (
+                f"date must be in '{min_date_iso}'-'{max_date_iso}', "
+                f"got '{self.isoformat()}'"
+            )
+            raise OverflowError(message)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hijridate-2.4.1/src/hijridate/helpers.py` & `hijridate-2.5.0/src/hijridate/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,39 +3,35 @@
 
 def jdn_to_ordinal(jdn: int) -> int:
     """Convert Julian day number (JDN) to Gregorian date ordinal.
 
     Args:
         jdn: Julian day number (JDN).
     """
-
     return jdn - 1721425
 
 
 def ordinal_to_jdn(ordinal: int) -> int:
     """Convert Gregorian date ordinal to Julian day number (JDN).
 
     Args:
         ordinal: Gregorian date ordinal.
     """
-
     return ordinal + 1721425
 
 
 def jdn_to_rjd(jdn: int) -> int:
     """Return Reduced Julian Day (RJD) number from Julian day number (JDN).
 
     Args:
         jdn: Julian day number (JDN).
     """
-
     return jdn - 2400000
 
 
 def rjd_to_jdn(rjd: int) -> int:
     """Return Julian day number (JDN) from Reduced Julian Day (RJD) number.
 
     Args:
         rjd: Reduced Julian Day (RJD) number.
     """
-
     return rjd + 2400000
```

### Comparing `hijridate-2.4.1/src/hijridate/locales.py` & `hijridate-2.5.0/src/hijridate/locales.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,205 +1,199 @@
 """Localization for the Hijri month and day names."""
 
-from typing import ClassVar, Dict, List, Type
+from typing import ClassVar, Dict, Literal, Tuple, Type
+
+Language = Literal["en", "ar", "bn"]
 
 _locale_map: Dict[str, Type["Locale"]] = {}
 
 
 def get_locale(name: str) -> "Locale":
     """Return an appropriate :obj:`Locale` corresponding to a locale name.
 
     Args:
         name: name of the locale.
     """
-
     language_tag = name.lower()[:2]
     locale_cls = _locale_map.get(language_tag)
 
     if locale_cls is None:
-        raise ValueError(f"Unsupported language: {language_tag}")
+        message = f"unsupported language: {language_tag}"
+        raise ValueError(message)
 
     return locale_cls()
 
 
 class Locale:
     """A Locale object represents locale-specific data and functionality."""
 
     language_tag: ClassVar[str]
-    month_names: ClassVar[List[str]] = []
-    gregorian_month_names: ClassVar[List[str]] = []
-    day_names: ClassVar[List[str]] = []
+    month_names: ClassVar[Tuple[str, ...]]
+    gregorian_month_names: ClassVar[Tuple[str, ...]]
+    day_names: ClassVar[Tuple[str, ...]]
     notation: ClassVar[str]
     gregorian_notation: ClassVar[str]
 
     def __init_subclass__(cls) -> None:
         if cls.language_tag in _locale_map:
-            raise LookupError(f"Duplicated language tag: {cls.language_tag}")
+            message = f"duplicated language tag: {cls.language_tag}"
+            raise LookupError(message)
         _locale_map[cls.language_tag] = cls
 
     def month_name(self, month: int) -> str:
         """Return the month name for a specified Hijri month of the year.
 
         Args:
             month: month of year, in range 1-12.
         """
-
         return self.month_names[month - 1]
 
     def gregorian_month_name(self, month: int) -> str:
         """Return the month name for a specified Gregorian month of the year.
 
         Args:
             month: month of year, in range 1-12.
         """
-
         return self.gregorian_month_names[month - 1]
 
     def day_name(self, day: int) -> str:
         """Return the day name for a specified day of the week.
 
         Args:
             day: day of week, where Monday is 1 and Sunday is 7.
         """
-
         return self.day_names[day - 1]
 
 
 class EnglishLocale(Locale):
-    """An English Locale object represents English locale-specific data and
-    functionality.
-    """
+    """An English Locale object represents English locale-specific data."""
 
     language_tag = "en"
-    month_names = [
+    month_names = (
         "Muharram",
         "Safar",
-        "Rabi’ al-Awwal",
-        "Rabi’ al-Thani",
+        "Rabi' al-Awwal",
+        "Rabi' al-Thani",
         "Jumada al-Ula",
         "Jumada al-Akhirah",
         "Rajab",
-        "Sha’ban",
-        "Ramadhan",
+        "Sha'ban",
+        "Ramadan",
         "Shawwal",
-        "Dhu al-Qi’dah",
+        "Dhu al-Qa'dah",
         "Dhu al-Hijjah",
-    ]
-    gregorian_month_names = [
+    )
+    gregorian_month_names = (
         "January",
         "February",
         "March",
         "April",
         "May",
         "June",
         "July",
         "August",
         "September",
         "October",
         "November",
         "December",
-    ]
-    day_names = [
+    )
+    day_names = (
         "Monday",
         "Tuesday",
         "Wednesday",
         "Thursday",
         "Friday",
         "Saturday",
         "Sunday",
-    ]
+    )
     notation = "AH"
     gregorian_notation = "CE"
 
 
 class ArabicLocale(Locale):
-    """An Arabic Locale object represents Arabic locale-specific data and
-    functionality.
-    """
+    """An Arabic Locale object represents Arabic locale-specific data."""
 
     language_tag = "ar"
-    month_names = [
+    month_names = (
         "محرم",
         "صفر",
         "ربيع الأول",
         "ربيع الثاني",
         "جمادى الأولى",
         "جمادى الآخرة",
         "رجب",
         "شعبان",
         "رمضان",
         "شوال",
         "ذو القعدة",
         "ذو الحجة",
-    ]
-    gregorian_month_names = [
+    )
+    gregorian_month_names = (
         "يناير",
         "فبراير",
         "مارس",
         "أبريل",
         "مايو",
         "يونيو",
         "يوليو",
         "أغسطس",
         "سبتمبر",
         "أكتوبر",
         "نوفمبر",
         "ديسمبر",
-    ]
-    day_names = [
+    )
+    day_names = (
         "الإثنين",
         "الثلاثاء",
         "الأربعاء",
         "الخميس",
         "الجمعة",
         "السبت",
         "الأحد",
-    ]
+    )
     notation = "هـ"
     gregorian_notation = "م"
 
 
 class BengaliLocale(Locale):
-    """A Bengali Locale object represents Bengali locale-specific data and
-    functionality.
-    """
+    """A Bengali Locale object represents Bengali locale-specific data."""
 
     language_tag = "bn"
-    month_names = [
+    month_names = (
         "মুহাররম",
         "সফর",
         "রবিউল আউয়াল",
         "রবিউস সানী",
         "জুমাদাল উলা",
         "জুমাদাস সানী",
         "রজব",
         "শাবান",
         "রমজান",
         "শাওয়াল",
         "জিলক্বদ",
         "জিলহজ",
-    ]
-    gregorian_month_names = [
+    )
+    gregorian_month_names = (
         "জানুয়ারি",
         "ফেব্রুয়ারি",
         "মার্চ",
         "এপ্রিল",
         "মে",
         "জুন",
         "জুলাই",
         "আগস্ট",
         "সেপ্টেম্বর",
         "অক্টোবর",
         "নভেম্বর",
         "ডিসেম্বর",
-    ]
-    day_names = [
+    )
+    day_names = (
         "সোমবার",
         "মঙ্গলবার",
         "বুধবার",
         "বৃহস্পতিবার",
         "শুক্রবার",
         "শনিবার",
         "রবিবার",
-    ]
+    )
     notation = "হিজরি"
     gregorian_notation = "খ্রিস্টাব্দ"
```

### Comparing `hijridate-2.4.1/src/hijridate/ummalqura.py` & `hijridate-2.5.0/src/hijridate/ummalqura.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,183 +11,169 @@
 """Inclusive range of supported Hijri dates (year, month and day)."""
 
 HIJRI_OFFSET: int = 1342 * 12
 """Total Hijri months elapsed before the beginning of Hijri range."""
 
 # fmt: off
 MONTH_STARTS: Tuple[int, ...] = (
-    23999, 24029, 24058, 24088, 24118, 24147, 24177, 24207, 24237, 24265, 24295,
-    24325, 24355, 24384, 24413, 24443, 24472, 24502, 24531, 24561, 24590, 24620,
-    24649, 24679, 24708, 24738, 24767, 24797, 24826, 24857, 24886, 24916, 24944,
-    24974, 25004, 25033, 25063, 25092, 25121, 25151, 25181, 25210, 25240, 25270,
-    25299, 25328, 25358, 25388, 25417, 25446, 25475, 25505, 25535, 25564, 25594,
-    25624, 25653, 25683, 25713, 25742, 25771, 25801, 25830, 25860, 25889, 25919,
-    25948, 25978, 26008, 26037, 26066, 26097, 26125, 26155, 26184, 26214, 26243,
-    26273, 26302, 26332, 26362, 26392, 26420, 26451, 26481, 26510, 26540, 26569,
-    26599, 26628, 26657, 26687, 26716, 26746, 26776, 26805, 26835, 26865, 26894,
-    26924, 26953, 26983, 27012, 27041, 27070, 27100, 27130, 27159, 27189, 27219,
-    27248, 27278, 27307, 27337, 27366, 27396, 27425, 27455, 27484, 27514, 27543,
-    27573, 27602, 27632, 27662, 27691, 27721, 27750, 27780, 27810, 27839, 27868,
-    27898, 27927, 27957, 27986, 28016, 28045, 28075, 28105, 28134, 28164, 28193,
-    28223, 28252, 28282, 28311, 28341, 28370, 28400, 28429, 28459, 28488, 28518,
-    28548, 28577, 28607, 28636, 28665, 28695, 28724, 28754, 28783, 28813, 28843,
-    28872, 28901, 28931, 28960, 28990, 29019, 29049, 29078, 29108, 29137, 29167,
-    29196, 29226, 29255, 29285, 29315, 29345, 29375, 29404, 29434, 29463, 29492,
-    29522, 29551, 29580, 29610, 29640, 29669, 29699, 29729, 29759, 29788, 29818,
-    29847, 29876, 29906, 29935, 29964, 29994, 30023, 30053, 30082, 30112, 30141,
-    30171, 30200, 30230, 30259, 30289, 30318, 30348, 30378, 30408, 30437, 30467,
-    30496, 30526, 30555, 30585, 30614, 30644, 30673, 30703, 30732, 30762, 30791,
-    30821, 30850, 30880, 30909, 30939, 30968, 30998, 31027, 31057, 31086, 31116,
-    31145, 31175, 31204, 31234, 31263, 31293, 31322, 31352, 31381, 31411, 31441,
-    31471, 31500, 31530, 31559, 31589, 31618, 31648, 31676, 31706, 31736, 31766,
-    31795, 31825, 31854, 31884, 31913, 31943, 31972, 32002, 32031, 32061, 32090,
-    32120, 32150, 32180, 32209, 32239, 32268, 32298, 32327, 32357, 32386, 32416,
-    32445, 32475, 32504, 32534, 32563, 32593, 32622, 32652, 32681, 32711, 32740,
-    32770, 32799, 32829, 32858, 32888, 32917, 32947, 32976, 33006, 33035, 33065,
-    33094, 33124, 33153, 33183, 33213, 33243, 33272, 33302, 33331, 33361, 33390,
-    33420, 33450, 33479, 33509, 33539, 33568, 33598, 33627, 33657, 33686, 33716,
-    33745, 33775, 33804, 33834, 33863, 33893, 33922, 33952, 33981, 34011, 34040,
-    34069, 34099, 34128, 34158, 34187, 34217, 34247, 34277, 34306, 34336, 34365,
-    34395, 34424, 34454, 34483, 34512, 34542, 34571, 34601, 34631, 34660, 34690,
-    34719, 34749, 34778, 34808, 34837, 34867, 34896, 34926, 34955, 34985, 35015,
-    35044, 35074, 35103, 35133, 35162, 35192, 35222, 35251, 35280, 35310, 35340,
-    35370, 35399, 35429, 35458, 35488, 35517, 35547, 35576, 35605, 35635, 35665,
-    35694, 35723, 35753, 35782, 35811, 35841, 35871, 35901, 35930, 35960, 35989,
-    36019, 36048, 36078, 36107, 36136, 36166, 36195, 36225, 36254, 36284, 36314,
-    36343, 36373, 36403, 36433, 36462, 36492, 36521, 36551, 36580, 36610, 36639,
-    36669, 36698, 36728, 36757, 36786, 36816, 36845, 36875, 36904, 36934, 36963,
-    36993, 37022, 37052, 37081, 37111, 37141, 37170, 37200, 37229, 37259, 37288,
-    37318, 37347, 37377, 37406, 37436, 37465, 37495, 37524, 37554, 37584, 37613,
-    37643, 37672, 37701, 37731, 37760, 37790, 37819, 37849, 37878, 37908, 37938,
-    37967, 37997, 38027, 38056, 38085, 38115, 38144, 38174, 38203, 38233, 38262,
-    38292, 38322, 38351, 38381, 38410, 38440, 38469, 38499, 38528, 38558, 38587,
-    38617, 38646, 38676, 38705, 38735, 38764, 38794, 38823, 38853, 38882, 38912,
-    38941, 38971, 39001, 39030, 39059, 39089, 39118, 39148, 39178, 39208, 39237,
-    39267, 39297, 39326, 39355, 39385, 39414, 39444, 39473, 39503, 39532, 39562,
-    39592, 39621, 39650, 39680, 39709, 39739, 39768, 39798, 39827, 39857, 39886,
-    39916, 39946, 39975, 40005, 40035, 40064, 40094, 40123, 40153, 40182, 40212,
-    40241, 40271, 40300, 40330, 40359, 40389, 40418, 40448, 40477, 40507, 40536,
-    40566, 40595, 40625, 40655, 40685, 40714, 40744, 40773, 40803, 40832, 40862,
-    40892, 40921, 40951, 40980, 41009, 41039, 41068, 41098, 41127, 41157, 41186,
-    41216, 41245, 41275, 41304, 41334, 41364, 41393, 41422, 41452, 41481, 41511,
-    41540, 41570, 41599, 41629, 41658, 41688, 41718, 41748, 41777, 41807, 41836,
-    41865, 41894, 41924, 41953, 41983, 42012, 42042, 42072, 42102, 42131, 42161,
-    42190, 42220, 42249, 42279, 42308, 42337, 42367, 42397, 42426, 42456, 42485,
-    42515, 42545, 42574, 42604, 42633, 42662, 42692, 42721, 42751, 42780, 42810,
-    42839, 42869, 42899, 42929, 42958, 42988, 43017, 43046, 43076, 43105, 43135,
-    43164, 43194, 43223, 43253, 43283, 43312, 43342, 43371, 43401, 43430, 43460,
-    43489, 43519, 43548, 43578, 43607, 43637, 43666, 43696, 43726, 43755, 43785,
-    43814, 43844, 43873, 43903, 43932, 43962, 43991, 44021, 44050, 44080, 44109,
-    44139, 44169, 44198, 44228, 44258, 44287, 44317, 44346, 44375, 44405, 44434,
-    44464, 44493, 44523, 44553, 44582, 44612, 44641, 44671, 44700, 44730, 44759,
-    44788, 44818, 44847, 44877, 44906, 44936, 44966, 44996, 45025, 45055, 45084,
-    45114, 45143, 45172, 45202, 45231, 45261, 45290, 45320, 45350, 45380, 45409,
-    45439, 45468, 45498, 45527, 45556, 45586, 45615, 45644, 45674, 45704, 45733,
-    45763, 45793, 45823, 45852, 45882, 45911, 45940, 45970, 45999, 46028, 46058,
-    46088, 46117, 46147, 46177, 46206, 46236, 46265, 46295, 46324, 46354, 46383,
-    46413, 46442, 46472, 46501, 46531, 46560, 46590, 46620, 46649, 46679, 46708,
-    46738, 46767, 46797, 46826, 46856, 46885, 46915, 46944, 46974, 47003, 47033,
-    47063, 47092, 47122, 47151, 47181, 47210, 47240, 47269, 47298, 47328, 47357,
-    47387, 47417, 47446, 47476, 47506, 47535, 47565, 47594, 47624, 47653, 47682,
-    47712, 47741, 47771, 47800, 47830, 47860, 47890, 47919, 47949, 47978, 48008,
-    48037, 48066, 48096, 48125, 48155, 48184, 48214, 48244, 48273, 48303, 48333,
-    48362, 48392, 48421, 48450, 48480, 48509, 48538, 48568, 48598, 48627, 48657,
-    48687, 48717, 48746, 48776, 48805, 48834, 48864, 48893, 48922, 48952, 48982,
-    49011, 49041, 49071, 49100, 49130, 49160, 49189, 49218, 49248, 49277, 49306,
-    49336, 49365, 49395, 49425, 49455, 49484, 49514, 49543, 49573, 49602, 49632,
-    49661, 49690, 49720, 49749, 49779, 49809, 49838, 49868, 49898, 49927, 49957,
-    49986, 50016, 50045, 50075, 50104, 50133, 50163, 50192, 50222, 50252, 50281,
-    50311, 50340, 50370, 50400, 50429, 50459, 50488, 50518, 50547, 50576, 50606,
-    50635, 50665, 50694, 50724, 50754, 50784, 50813, 50843, 50872, 50902, 50931,
-    50960, 50990, 51019, 51049, 51078, 51108, 51138, 51167, 51197, 51227, 51256,
-    51286, 51315, 51345, 51374, 51403, 51433, 51462, 51492, 51522, 51552, 51582,
-    51611, 51641, 51670, 51699, 51729, 51758, 51787, 51816, 51846, 51876, 51906,
-    51936, 51965, 51995, 52025, 52054, 52083, 52113, 52142, 52171, 52200, 52230,
-    52260, 52290, 52319, 52349, 52379, 52408, 52438, 52467, 52497, 52526, 52555,
-    52585, 52614, 52644, 52673, 52703, 52733, 52762, 52792, 52822, 52851, 52881,
-    52910, 52939, 52969, 52998, 53028, 53057, 53087, 53116, 53146, 53176, 53205,
-    53235, 53264, 53294, 53324, 53353, 53383, 53412, 53441, 53471, 53500, 53530,
-    53559, 53589, 53619, 53648, 53678, 53708, 53737, 53767, 53796, 53825, 53855,
-    53884, 53914, 53943, 53973, 54003, 54032, 54062, 54092, 54121, 54151, 54180,
-    54209, 54239, 54268, 54297, 54327, 54357, 54387, 54416, 54446, 54476, 54505,
-    54535, 54564, 54593, 54623, 54652, 54681, 54711, 54741, 54770, 54800, 54830,
-    54859, 54889, 54919, 54948, 54977, 55007, 55036, 55066, 55095, 55125, 55154,
-    55184, 55213, 55243, 55273, 55302, 55332, 55361, 55391, 55420, 55450, 55479,
-    55508, 55538, 55567, 55597, 55627, 55657, 55686, 55716, 55745, 55775, 55804,
-    55834, 55863, 55892, 55922, 55951, 55981, 56011, 56040, 56070, 56100, 56129,
-    56159, 56188, 56218, 56247, 56276, 56306, 56335, 56365, 56394, 56424, 56454,
-    56483, 56513, 56543, 56572, 56601, 56631, 56660, 56690, 56719, 56749, 56778,
-    56808, 56837, 56867, 56897, 56926, 56956, 56985, 57015, 57044, 57074, 57103,
-    57133, 57162, 57192, 57221, 57251, 57280, 57310, 57340, 57369, 57399, 57429,
-    57458, 57487, 57517, 57546, 57576, 57605, 57634, 57664, 57694, 57723, 57753,
-    57783, 57813, 57842, 57871, 57901, 57930, 57959, 57989, 58018, 58048, 58077,
-    58107, 58137, 58167, 58196, 58226, 58255, 58285, 58314, 58343, 58373, 58402,
-    58432, 58461, 58491, 58521, 58551, 58580, 58610, 58639, 58669, 58698, 58727,
-    58757, 58786, 58816, 58845, 58875, 58905, 58934, 58964, 58994, 59023, 59053,
-    59082, 59111, 59141, 59170, 59200, 59229, 59259, 59288, 59318, 59348, 59377,
-    59407, 59436, 59466, 59495, 59525, 59554, 59584, 59613, 59643, 59672, 59702,
-    59731, 59761, 59791, 59820, 59850, 59879, 59909, 59939, 59968, 59997, 60027,
-    60056, 60086, 60115, 60145, 60174, 60204, 60234, 60264, 60293, 60323, 60352,
-    60381, 60411, 60440, 60469, 60499, 60528, 60558, 60588, 60618, 60647, 60677,
-    60707, 60736, 60765, 60795, 60824, 60853, 60883, 60912, 60942, 60972, 61002,
-    61031, 61061, 61090, 61120, 61149, 61179, 61208, 61237, 61267, 61296, 61326,
-    61356, 61385, 61415, 61445, 61474, 61504, 61533, 61563, 61592, 61621, 61651,
-    61680, 61710, 61739, 61769, 61799, 61828, 61858, 61888, 61917, 61947, 61976,
-    62006, 62035, 62064, 62094, 62123, 62153, 62182, 62212, 62242, 62271, 62301,
-    62331, 62360, 62390, 62419, 62448, 62478, 62507, 62537, 62566, 62596, 62625,
-    62655, 62685, 62715, 62744, 62774, 62803, 62832, 62862, 62891, 62921, 62950,
-    62980, 63009, 63039, 63069, 63099, 63128, 63157, 63187, 63216, 63246, 63275,
-    63305, 63334, 63363, 63393, 63423, 63453, 63482, 63512, 63541, 63571, 63600,
-    63630, 63659, 63689, 63718, 63747, 63777, 63807, 63836, 63866, 63895, 63925,
-    63955, 63984, 64014, 64043, 64073, 64102, 64131, 64161, 64190, 64220, 64249,
-    64279, 64309, 64339, 64368, 64398, 64427, 64457, 64486, 64515, 64545, 64574,
-    64603, 64633, 64663, 64692, 64722, 64752, 64782, 64811, 64841, 64870, 64899,
-    64929, 64958, 64987, 65017, 65047, 65076, 65106, 65136, 65166, 65195, 65225,
-    65254, 65283, 65313, 65342, 65371, 65401, 65431, 65460, 65490, 65520, 65549,
-    65579, 65608, 65638, 65667, 65697, 65726, 65755, 65785, 65815, 65844, 65874,
-    65903, 65933, 65963, 65992, 66022, 66051, 66081, 66110, 66140, 66169, 66199,
-    66228, 66258, 66287, 66317, 66346, 66376, 66405, 66435, 66465, 66494, 66524,
-    66553, 66583, 66612, 66641, 66671, 66700, 66730, 66760, 66789, 66819, 66849,
-    66878, 66908, 66937, 66967, 66996, 67025, 67055, 67084, 67114, 67143, 67173,
-    67203, 67233, 67262, 67292, 67321, 67351, 67380, 67409, 67439, 67468, 67497,
-    67527, 67557, 67587, 67617, 67646, 67676, 67705, 67735, 67764, 67793, 67823,
-    67852, 67882, 67911, 67941, 67971, 68000, 68030, 68060, 68089, 68119, 68148,
-    68177, 68207, 68236, 68266, 68295, 68325, 68354, 68384, 68414, 68443, 68473,
-    68502, 68532, 68561, 68591, 68620, 68650, 68679, 68708, 68738, 68768, 68797,
-    68827, 68857, 68886, 68916, 68946, 68975, 69004, 69034, 69063, 69092, 69122,
-    69152, 69181, 69211, 69240, 69270, 69300, 69330, 69359, 69388, 69418, 69447,
-    69476, 69506, 69535, 69565, 69595, 69624, 69654, 69684, 69713, 69743, 69772,
-    69802, 69831, 69861, 69890, 69919, 69949, 69978, 70008, 70038, 70067, 70097,
-    70126, 70156, 70186, 70215, 70245, 70274, 70303, 70333, 70362, 70392, 70421,
-    70451, 70481, 70510, 70540, 70570, 70599, 70629, 70658, 70687, 70717, 70746,
-    70776, 70805, 70835, 70864, 70894, 70924, 70954, 70983, 71013, 71042, 71071,
-    71101, 71130, 71159, 71189, 71218, 71248, 71278, 71308, 71337, 71367, 71397,
-    71426, 71455, 71485, 71514, 71543, 71573, 71602, 71632, 71662, 71691, 71721,
-    71751, 71781, 71810, 71839, 71869, 71898, 71927, 71957, 71986, 72016, 72046,
-    72075, 72105, 72135, 72164, 72194, 72223, 72253, 72282, 72311, 72341, 72370,
-    72400, 72429, 72459, 72489, 72518, 72548, 72577, 72607, 72637, 72666, 72695,
-    72725, 72754, 72784, 72813, 72843, 72872, 72902, 72931, 72961, 72991, 73020,
-    73050, 73080, 73109, 73139, 73168, 73197, 73227, 73256, 73286, 73315, 73345,
-    73375, 73404, 73434, 73464, 73493, 73523, 73552, 73581, 73611, 73640, 73669,
-    73699, 73729, 73758, 73788, 73818, 73848, 73877, 73907, 73936, 73965, 73995,
-    74024, 74053, 74083, 74113, 74142, 74172, 74202, 74231, 74261, 74291, 74320,
-    74349, 74379, 74408, 74437, 74467, 74497, 74526, 74556, 74585, 74615, 74645,
-    74675, 74704, 74733, 74763, 74792, 74822, 74851, 74881, 74910, 74940, 74969,
-    74999, 75029, 75058, 75088, 75117, 75147, 75176, 75206, 75235, 75264, 75294,
-    75323, 75353, 75383, 75412, 75442, 75472, 75501, 75531, 75560, 75590, 75619,
-    75648, 75678, 75707, 75737, 75766, 75796, 75826, 75856, 75885, 75915, 75944,
-    75974, 76003, 76032, 76062, 76091, 76121, 76150, 76180, 76210, 76239, 76269,
-    76299, 76328, 76358, 76387, 76416, 76446, 76475, 76505, 76534, 76564, 76593,
-    76623, 76653, 76682, 76712, 76741, 76771, 76801, 76830, 76859, 76889, 76918,
-    76948, 76977, 77007, 77036, 77066, 77096, 77125, 77155, 77185, 77214, 77243,
-    77273, 77302, 77332, 77361, 77390, 77420, 77450, 77479, 77509, 77539, 77569,
-    77598, 77627, 77657, 77686, 77715, 77745, 77774, 77804, 77833, 77863, 77893,
-    77923, 77952, 77982, 78011, 78041, 78070, 78099, 78129, 78158, 78188, 78217,
-    78247, 78277, 78307, 78336, 78366, 78395, 78425, 78454, 78483, 78513, 78542,
-    78572, 78601, 78631, 78661, 78690, 78720, 78750, 78779, 78808, 78838, 78867,
-    78897, 78926, 78956, 78985, 79015, 79044, 79074, 79104, 79133, 79163, 79192,
-    79222, 79251, 79281, 79310, 79340, 79369, 79399, 79428, 79458, 79487, 79517,
-    79546, 79576, 79606, 79635, 79665, 79695, 79724, 79753, 79783, 79812, 79841,
-    79871, 79900, 79930, 79960, 79990)
-"""Ordered list of Reduced Julian Day (RJD) numbers for the beginning of
-supported Hijri months.
+    23999, 24029, 24058, 24088, 24118, 24147, 24177, 24207, 24237, 24265, 24295, 24325,
+    24355, 24384, 24413, 24443, 24472, 24502, 24531, 24561, 24590, 24620, 24649, 24679,
+    24708, 24738, 24767, 24797, 24826, 24857, 24886, 24916, 24944, 24974, 25004, 25033,
+    25063, 25092, 25121, 25151, 25181, 25210, 25240, 25270, 25299, 25328, 25358, 25388,
+    25417, 25446, 25475, 25505, 25535, 25564, 25594, 25624, 25653, 25683, 25713, 25742,
+    25771, 25801, 25830, 25860, 25889, 25919, 25948, 25978, 26008, 26037, 26066, 26097,
+    26125, 26155, 26184, 26214, 26243, 26273, 26302, 26332, 26362, 26392, 26420, 26451,
+    26481, 26510, 26540, 26569, 26599, 26628, 26657, 26687, 26716, 26746, 26776, 26805,
+    26835, 26865, 26894, 26924, 26953, 26983, 27012, 27041, 27070, 27100, 27130, 27159,
+    27189, 27219, 27248, 27278, 27307, 27337, 27366, 27396, 27425, 27455, 27484, 27514,
+    27543, 27573, 27602, 27632, 27662, 27691, 27721, 27750, 27780, 27810, 27839, 27868,
+    27898, 27927, 27957, 27986, 28016, 28045, 28075, 28105, 28134, 28164, 28193, 28223,
+    28252, 28282, 28311, 28341, 28370, 28400, 28429, 28459, 28488, 28518, 28548, 28577,
+    28607, 28636, 28665, 28695, 28724, 28754, 28783, 28813, 28843, 28872, 28901, 28931,
+    28960, 28990, 29019, 29049, 29078, 29108, 29137, 29167, 29196, 29226, 29255, 29285,
+    29315, 29345, 29375, 29404, 29434, 29463, 29492, 29522, 29551, 29580, 29610, 29640,
+    29669, 29699, 29729, 29759, 29788, 29818, 29847, 29876, 29906, 29935, 29964, 29994,
+    30023, 30053, 30082, 30112, 30141, 30171, 30200, 30230, 30259, 30289, 30318, 30348,
+    30378, 30408, 30437, 30467, 30496, 30526, 30555, 30585, 30614, 30644, 30673, 30703,
+    30732, 30762, 30791, 30821, 30850, 30880, 30909, 30939, 30968, 30998, 31027, 31057,
+    31086, 31116, 31145, 31175, 31204, 31234, 31263, 31293, 31322, 31352, 31381, 31411,
+    31441, 31471, 31500, 31530, 31559, 31589, 31618, 31648, 31676, 31706, 31736, 31766,
+    31795, 31825, 31854, 31884, 31913, 31943, 31972, 32002, 32031, 32061, 32090, 32120,
+    32150, 32180, 32209, 32239, 32268, 32298, 32327, 32357, 32386, 32416, 32445, 32475,
+    32504, 32534, 32563, 32593, 32622, 32652, 32681, 32711, 32740, 32770, 32799, 32829,
+    32858, 32888, 32917, 32947, 32976, 33006, 33035, 33065, 33094, 33124, 33153, 33183,
+    33213, 33243, 33272, 33302, 33331, 33361, 33390, 33420, 33450, 33479, 33509, 33539,
+    33568, 33598, 33627, 33657, 33686, 33716, 33745, 33775, 33804, 33834, 33863, 33893,
+    33922, 33952, 33981, 34011, 34040, 34069, 34099, 34128, 34158, 34187, 34217, 34247,
+    34277, 34306, 34336, 34365, 34395, 34424, 34454, 34483, 34512, 34542, 34571, 34601,
+    34631, 34660, 34690, 34719, 34749, 34778, 34808, 34837, 34867, 34896, 34926, 34955,
+    34985, 35015, 35044, 35074, 35103, 35133, 35162, 35192, 35222, 35251, 35280, 35310,
+    35340, 35370, 35399, 35429, 35458, 35488, 35517, 35547, 35576, 35605, 35635, 35665,
+    35694, 35723, 35753, 35782, 35811, 35841, 35871, 35901, 35930, 35960, 35989, 36019,
+    36048, 36078, 36107, 36136, 36166, 36195, 36225, 36254, 36284, 36314, 36343, 36373,
+    36403, 36433, 36462, 36492, 36521, 36551, 36580, 36610, 36639, 36669, 36698, 36728,
+    36757, 36786, 36816, 36845, 36875, 36904, 36934, 36963, 36993, 37022, 37052, 37081,
+    37111, 37141, 37170, 37200, 37229, 37259, 37288, 37318, 37347, 37377, 37406, 37436,
+    37465, 37495, 37524, 37554, 37584, 37613, 37643, 37672, 37701, 37731, 37760, 37790,
+    37819, 37849, 37878, 37908, 37938, 37967, 37997, 38027, 38056, 38085, 38115, 38144,
+    38174, 38203, 38233, 38262, 38292, 38322, 38351, 38381, 38410, 38440, 38469, 38499,
+    38528, 38558, 38587, 38617, 38646, 38676, 38705, 38735, 38764, 38794, 38823, 38853,
+    38882, 38912, 38941, 38971, 39001, 39030, 39059, 39089, 39118, 39148, 39178, 39208,
+    39237, 39267, 39297, 39326, 39355, 39385, 39414, 39444, 39473, 39503, 39532, 39562,
+    39592, 39621, 39650, 39680, 39709, 39739, 39768, 39798, 39827, 39857, 39886, 39916,
+    39946, 39975, 40005, 40035, 40064, 40094, 40123, 40153, 40182, 40212, 40241, 40271,
+    40300, 40330, 40359, 40389, 40418, 40448, 40477, 40507, 40536, 40566, 40595, 40625,
+    40655, 40685, 40714, 40744, 40773, 40803, 40832, 40862, 40892, 40921, 40951, 40980,
+    41009, 41039, 41068, 41098, 41127, 41157, 41186, 41216, 41245, 41275, 41304, 41334,
+    41364, 41393, 41422, 41452, 41481, 41511, 41540, 41570, 41599, 41629, 41658, 41688,
+    41718, 41748, 41777, 41807, 41836, 41865, 41894, 41924, 41953, 41983, 42012, 42042,
+    42072, 42102, 42131, 42161, 42190, 42220, 42249, 42279, 42308, 42337, 42367, 42397,
+    42426, 42456, 42485, 42515, 42545, 42574, 42604, 42633, 42662, 42692, 42721, 42751,
+    42780, 42810, 42839, 42869, 42899, 42929, 42958, 42988, 43017, 43046, 43076, 43105,
+    43135, 43164, 43194, 43223, 43253, 43283, 43312, 43342, 43371, 43401, 43430, 43460,
+    43489, 43519, 43548, 43578, 43607, 43637, 43666, 43696, 43726, 43755, 43785, 43814,
+    43844, 43873, 43903, 43932, 43962, 43991, 44021, 44050, 44080, 44109, 44139, 44169,
+    44198, 44228, 44258, 44287, 44317, 44346, 44375, 44405, 44434, 44464, 44493, 44523,
+    44553, 44582, 44612, 44641, 44671, 44700, 44730, 44759, 44788, 44818, 44847, 44877,
+    44906, 44936, 44966, 44996, 45025, 45055, 45084, 45114, 45143, 45172, 45202, 45231,
+    45261, 45290, 45320, 45350, 45380, 45409, 45439, 45468, 45498, 45527, 45556, 45586,
+    45615, 45644, 45674, 45704, 45733, 45763, 45793, 45823, 45852, 45882, 45911, 45940,
+    45970, 45999, 46028, 46058, 46088, 46117, 46147, 46177, 46206, 46236, 46265, 46295,
+    46324, 46354, 46383, 46413, 46442, 46472, 46501, 46531, 46560, 46590, 46620, 46649,
+    46679, 46708, 46738, 46767, 46797, 46826, 46856, 46885, 46915, 46944, 46974, 47003,
+    47033, 47063, 47092, 47122, 47151, 47181, 47210, 47240, 47269, 47298, 47328, 47357,
+    47387, 47417, 47446, 47476, 47506, 47535, 47565, 47594, 47624, 47653, 47682, 47712,
+    47741, 47771, 47800, 47830, 47860, 47890, 47919, 47949, 47978, 48008, 48037, 48066,
+    48096, 48125, 48155, 48184, 48214, 48244, 48273, 48303, 48333, 48362, 48392, 48421,
+    48450, 48480, 48509, 48538, 48568, 48598, 48627, 48657, 48687, 48717, 48746, 48776,
+    48805, 48834, 48864, 48893, 48922, 48952, 48982, 49011, 49041, 49071, 49100, 49130,
+    49160, 49189, 49218, 49248, 49277, 49306, 49336, 49365, 49395, 49425, 49455, 49484,
+    49514, 49543, 49573, 49602, 49632, 49661, 49690, 49720, 49749, 49779, 49809, 49838,
+    49868, 49898, 49927, 49957, 49986, 50016, 50045, 50075, 50104, 50133, 50163, 50192,
+    50222, 50252, 50281, 50311, 50340, 50370, 50400, 50429, 50459, 50488, 50518, 50547,
+    50576, 50606, 50635, 50665, 50694, 50724, 50754, 50784, 50813, 50843, 50872, 50902,
+    50931, 50960, 50990, 51019, 51049, 51078, 51108, 51138, 51167, 51197, 51227, 51256,
+    51286, 51315, 51345, 51374, 51403, 51433, 51462, 51492, 51522, 51552, 51582, 51611,
+    51641, 51670, 51699, 51729, 51758, 51787, 51816, 51846, 51876, 51906, 51936, 51965,
+    51995, 52025, 52054, 52083, 52113, 52142, 52171, 52200, 52230, 52260, 52290, 52319,
+    52349, 52379, 52408, 52438, 52467, 52497, 52526, 52555, 52585, 52614, 52644, 52673,
+    52703, 52733, 52762, 52792, 52822, 52851, 52881, 52910, 52939, 52969, 52998, 53028,
+    53057, 53087, 53116, 53146, 53176, 53205, 53235, 53264, 53294, 53324, 53353, 53383,
+    53412, 53441, 53471, 53500, 53530, 53559, 53589, 53619, 53648, 53678, 53708, 53737,
+    53767, 53796, 53825, 53855, 53884, 53914, 53943, 53973, 54003, 54032, 54062, 54092,
+    54121, 54151, 54180, 54209, 54239, 54268, 54297, 54327, 54357, 54387, 54416, 54446,
+    54476, 54505, 54535, 54564, 54593, 54623, 54652, 54681, 54711, 54741, 54770, 54800,
+    54830, 54859, 54889, 54919, 54948, 54977, 55007, 55036, 55066, 55095, 55125, 55154,
+    55184, 55213, 55243, 55273, 55302, 55332, 55361, 55391, 55420, 55450, 55479, 55508,
+    55538, 55567, 55597, 55627, 55657, 55686, 55716, 55745, 55775, 55804, 55834, 55863,
+    55892, 55922, 55951, 55981, 56011, 56040, 56070, 56100, 56129, 56159, 56188, 56218,
+    56247, 56276, 56306, 56335, 56365, 56394, 56424, 56454, 56483, 56513, 56543, 56572,
+    56601, 56631, 56660, 56690, 56719, 56749, 56778, 56808, 56837, 56867, 56897, 56926,
+    56956, 56985, 57015, 57044, 57074, 57103, 57133, 57162, 57192, 57221, 57251, 57280,
+    57310, 57340, 57369, 57399, 57429, 57458, 57487, 57517, 57546, 57576, 57605, 57634,
+    57664, 57694, 57723, 57753, 57783, 57813, 57842, 57871, 57901, 57930, 57959, 57989,
+    58018, 58048, 58077, 58107, 58137, 58167, 58196, 58226, 58255, 58285, 58314, 58343,
+    58373, 58402, 58432, 58461, 58491, 58521, 58551, 58580, 58610, 58639, 58669, 58698,
+    58727, 58757, 58786, 58816, 58845, 58875, 58905, 58934, 58964, 58994, 59023, 59053,
+    59082, 59111, 59141, 59170, 59200, 59229, 59259, 59288, 59318, 59348, 59377, 59407,
+    59436, 59466, 59495, 59525, 59554, 59584, 59613, 59643, 59672, 59702, 59731, 59761,
+    59791, 59820, 59850, 59879, 59909, 59939, 59968, 59997, 60027, 60056, 60086, 60115,
+    60145, 60174, 60204, 60234, 60264, 60293, 60323, 60352, 60381, 60411, 60440, 60469,
+    60499, 60528, 60558, 60588, 60618, 60647, 60677, 60707, 60736, 60765, 60795, 60824,
+    60853, 60883, 60912, 60942, 60972, 61002, 61031, 61061, 61090, 61120, 61149, 61179,
+    61208, 61237, 61267, 61296, 61326, 61356, 61385, 61415, 61445, 61474, 61504, 61533,
+    61563, 61592, 61621, 61651, 61680, 61710, 61739, 61769, 61799, 61828, 61858, 61888,
+    61917, 61947, 61976, 62006, 62035, 62064, 62094, 62123, 62153, 62182, 62212, 62242,
+    62271, 62301, 62331, 62360, 62390, 62419, 62448, 62478, 62507, 62537, 62566, 62596,
+    62625, 62655, 62685, 62715, 62744, 62774, 62803, 62832, 62862, 62891, 62921, 62950,
+    62980, 63009, 63039, 63069, 63099, 63128, 63157, 63187, 63216, 63246, 63275, 63305,
+    63334, 63363, 63393, 63423, 63453, 63482, 63512, 63541, 63571, 63600, 63630, 63659,
+    63689, 63718, 63747, 63777, 63807, 63836, 63866, 63895, 63925, 63955, 63984, 64014,
+    64043, 64073, 64102, 64131, 64161, 64190, 64220, 64249, 64279, 64309, 64339, 64368,
+    64398, 64427, 64457, 64486, 64515, 64545, 64574, 64603, 64633, 64663, 64692, 64722,
+    64752, 64782, 64811, 64841, 64870, 64899, 64929, 64958, 64987, 65017, 65047, 65076,
+    65106, 65136, 65166, 65195, 65225, 65254, 65283, 65313, 65342, 65371, 65401, 65431,
+    65460, 65490, 65520, 65549, 65579, 65608, 65638, 65667, 65697, 65726, 65755, 65785,
+    65815, 65844, 65874, 65903, 65933, 65963, 65992, 66022, 66051, 66081, 66110, 66140,
+    66169, 66199, 66228, 66258, 66287, 66317, 66346, 66376, 66405, 66435, 66465, 66494,
+    66524, 66553, 66583, 66612, 66641, 66671, 66700, 66730, 66760, 66789, 66819, 66849,
+    66878, 66908, 66937, 66967, 66996, 67025, 67055, 67084, 67114, 67143, 67173, 67203,
+    67233, 67262, 67292, 67321, 67351, 67380, 67409, 67439, 67468, 67497, 67527, 67557,
+    67587, 67617, 67646, 67676, 67705, 67735, 67764, 67793, 67823, 67852, 67882, 67911,
+    67941, 67971, 68000, 68030, 68060, 68089, 68119, 68148, 68177, 68207, 68236, 68266,
+    68295, 68325, 68354, 68384, 68414, 68443, 68473, 68502, 68532, 68561, 68591, 68620,
+    68650, 68679, 68708, 68738, 68768, 68797, 68827, 68857, 68886, 68916, 68946, 68975,
+    69004, 69034, 69063, 69092, 69122, 69152, 69181, 69211, 69240, 69270, 69300, 69330,
+    69359, 69388, 69418, 69447, 69476, 69506, 69535, 69565, 69595, 69624, 69654, 69684,
+    69713, 69743, 69772, 69802, 69831, 69861, 69890, 69919, 69949, 69978, 70008, 70038,
+    70067, 70097, 70126, 70156, 70186, 70215, 70245, 70274, 70303, 70333, 70362, 70392,
+    70421, 70451, 70481, 70510, 70540, 70570, 70599, 70629, 70658, 70687, 70717, 70746,
+    70776, 70805, 70835, 70864, 70894, 70924, 70954, 70983, 71013, 71042, 71071, 71101,
+    71130, 71159, 71189, 71218, 71248, 71278, 71308, 71337, 71367, 71397, 71426, 71455,
+    71485, 71514, 71543, 71573, 71602, 71632, 71662, 71691, 71721, 71751, 71781, 71810,
+    71839, 71869, 71898, 71927, 71957, 71986, 72016, 72046, 72075, 72105, 72135, 72164,
+    72194, 72223, 72253, 72282, 72311, 72341, 72370, 72400, 72429, 72459, 72489, 72518,
+    72548, 72577, 72607, 72637, 72666, 72695, 72725, 72754, 72784, 72813, 72843, 72872,
+    72902, 72931, 72961, 72991, 73020, 73050, 73080, 73109, 73139, 73168, 73197, 73227,
+    73256, 73286, 73315, 73345, 73375, 73404, 73434, 73464, 73493, 73523, 73552, 73581,
+    73611, 73640, 73669, 73699, 73729, 73758, 73788, 73818, 73848, 73877, 73907, 73936,
+    73965, 73995, 74024, 74053, 74083, 74113, 74142, 74172, 74202, 74231, 74261, 74291,
+    74320, 74349, 74379, 74408, 74437, 74467, 74497, 74526, 74556, 74585, 74615, 74645,
+    74675, 74704, 74733, 74763, 74792, 74822, 74851, 74881, 74910, 74940, 74969, 74999,
+    75029, 75058, 75088, 75117, 75147, 75176, 75206, 75235, 75264, 75294, 75323, 75353,
+    75383, 75412, 75442, 75472, 75501, 75531, 75560, 75590, 75619, 75648, 75678, 75707,
+    75737, 75766, 75796, 75826, 75856, 75885, 75915, 75944, 75974, 76003, 76032, 76062,
+    76091, 76121, 76150, 76180, 76210, 76239, 76269, 76299, 76328, 76358, 76387, 76416,
+    76446, 76475, 76505, 76534, 76564, 76593, 76623, 76653, 76682, 76712, 76741, 76771,
+    76801, 76830, 76859, 76889, 76918, 76948, 76977, 77007, 77036, 77066, 77096, 77125,
+    77155, 77185, 77214, 77243, 77273, 77302, 77332, 77361, 77390, 77420, 77450, 77479,
+    77509, 77539, 77569, 77598, 77627, 77657, 77686, 77715, 77745, 77774, 77804, 77833,
+    77863, 77893, 77923, 77952, 77982, 78011, 78041, 78070, 78099, 78129, 78158, 78188,
+    78217, 78247, 78277, 78307, 78336, 78366, 78395, 78425, 78454, 78483, 78513, 78542,
+    78572, 78601, 78631, 78661, 78690, 78720, 78750, 78779, 78808, 78838, 78867, 78897,
+    78926, 78956, 78985, 79015, 79044, 79074, 79104, 79133, 79163, 79192, 79222, 79251,
+    79281, 79310, 79340, 79369, 79399, 79428, 79458, 79487, 79517, 79546, 79576, 79606,
+    79635, 79665, 79695, 79724, 79753, 79783, 79812, 79841, 79871, 79900, 79930, 79960,
+    79990)
+"""Ordered list of Reduced Julian Day (RJD) numbers for the beginning of supported
+Hijri months.
 """
```

### Comparing `hijridate-2.4.1/tests/integration/fixtures/kfupm_comparison_calendar.json` & `hijridate-2.5.0/tests/integration/fixtures/kfupm_comparison_calendar.json`

 * *Files identical despite different names*

### Comparing `hijridate-2.4.1/tests/integration/fixtures/ummalqura_calendar_website.json` & `hijridate-2.5.0/tests/integration/fixtures/ummalqura_calendar_website.json`

 * *Files identical despite different names*

### Comparing `hijridate-2.4.1/tests/integration/fixtures/ummalqura_newspaper_issues.json` & `hijridate-2.5.0/tests/integration/fixtures/ummalqura_newspaper_issues.json`

 * *Files identical despite different names*

### Comparing `hijridate-2.4.1/tests/integration/test_month_starts.py` & `hijridate-2.5.0/tests/integration/test_references.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+
 from pathlib import Path
 
 import pytest
 
 from hijridate import Gregorian, Hijri
 
 
@@ -20,21 +21,21 @@
     params_reversed = [tuple(x[::-1]) for x in data]
     return params, params_reversed
 
 
 hijri_gregorian_params, gregorian_hijri_params = load_params_from_json()
 
 
-@pytest.mark.parametrize("test_input, expected", hijri_gregorian_params)
-def test_convert_hijri_to_gregorian(test_input, expected):
-    year, month, day = test_input
-    hijri = Hijri(year, month, day, validate=False)
+@pytest.mark.parametrize(("h_datetuple", "g_datetuple"), hijri_gregorian_params)
+def test_convert_hijri_to_gregorian(h_datetuple, g_datetuple):
+    year, month, day = h_datetuple
+    hijri = Hijri(year, month, day)
     converted = hijri.to_gregorian().datetuple()
-    assert converted == expected
+    assert converted == g_datetuple
 
 
-@pytest.mark.parametrize("test_input, expected", gregorian_hijri_params)
-def test_convert_gregorian_to_hijri(test_input, expected):
-    year, month, day = test_input
+@pytest.mark.parametrize(("g_datetuple", "h_datetuple"), gregorian_hijri_params)
+def test_convert_gregorian_to_hijri(g_datetuple, h_datetuple):
+    year, month, day = g_datetuple
     gregorian = Gregorian(year, month, day)
     converted = gregorian.to_hijri().datetuple()
-    assert converted == expected
+    assert converted == h_datetuple
```

### Comparing `hijridate-2.4.1/tests/unit/test_convert.py` & `hijridate-2.5.0/tests/unit/test_convert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,223 @@
 from datetime import date
 
 import pytest
 
 from hijridate.convert import Gregorian, Hijri
+from hijridate.ummalqura import GREGORIAN_RANGE, HIJRI_RANGE
+
+h_min, h_max = HIJRI_RANGE
+g_min, g_max = GREGORIAN_RANGE
+g_min_iso = "-".join([f"{i:02}" for i in g_min])
+g_max_iso = "-".join([f"{i:02}" for i in g_max])
 
 
 def test_importing_at_init_module():
     from hijridate import Gregorian, Hijri
 
     assert Hijri(1410, 8, 13)
     assert Gregorian(1990, 3, 10)
 
 
 @pytest.fixture(scope="class")
-def hijri_obj(request):
-    request.cls.hijri_obj = Hijri(1410, 8, 13)
+def _hijri_date(request):
+    request.cls.hijri_date = Hijri(1410, 8, 13)
 
 
-@pytest.mark.usefixtures("hijri_obj")
+@pytest.mark.usefixtures("_hijri_date")
 class TestHijri:
+    hijri_date = None
+
     def test_representation(self):
-        assert self.hijri_obj.__repr__() == "Hijri(1410, 8, 13)"
+        assert self.hijri_date.__repr__() == "Hijri(1410, 8, 13)"
 
     def test_string_representation(self):
-        assert self.hijri_obj.__str__() == "1410-08-13"
+        assert self.hijri_date.__str__() == "1410-08-13"
 
     def test_hash(self):
-        assert self.hijri_obj.__hash__() == hash(("Hijri", 1410, 8, 13))
+        assert self.hijri_date.__hash__() == hash(("Hijri", 1410, 8, 13))
 
-    @pytest.mark.parametrize(
-        "test_input", ["__gt__", "__ge__", "__lt__", "__le__"]
-    )
-    def test_comparison_notimplemented(self, test_input):
-        assert (
-            getattr(self.hijri_obj, test_input)("1410-08-13") == NotImplemented
-        )
+    @pytest.mark.parametrize("attr", ["__gt__", "__ge__", "__lt__", "__le__"])
+    def test_comparison_notimplemented(self, attr):
+        assert getattr(self.hijri_date, attr)("1410-08-13") == NotImplemented
 
     def test_equality(self):
-        assert self.hijri_obj == Hijri(1410, 8, 13)
-        assert self.hijri_obj != Hijri(1410, 8, 14)
-        assert self.hijri_obj != "1410-08-13"
+        assert self.hijri_date == Hijri(1410, 8, 13)
+        assert self.hijri_date != Hijri(1410, 8, 14)
+        assert self.hijri_date != "1410-08-13"
 
     def test_ordering(self):
-        assert self.hijri_obj > Hijri(1410, 8, 12)
-        assert self.hijri_obj >= Hijri(1410, 8, 13)
-        assert self.hijri_obj < Hijri(1410, 8, 14)
-        assert self.hijri_obj <= Hijri(1410, 8, 13)
+        assert self.hijri_date > Hijri(1410, 8, 12)
+        assert self.hijri_date >= Hijri(1410, 8, 13)
+        assert self.hijri_date < Hijri(1410, 8, 14)
+        assert self.hijri_date <= Hijri(1410, 8, 13)
 
     def test_fromisoformat(self):
-        assert Hijri.fromisoformat("1410-08-13") == self.hijri_obj
+        assert Hijri.fromisoformat("1410-08-13") == self.hijri_date
 
     def test_today(self):
         assert Hijri.today().to_gregorian() == Gregorian.today()
 
     def test_year(self):
-        assert self.hijri_obj.year == 1410
+        assert self.hijri_date.year == 1410
 
     def test_month(self):
-        assert self.hijri_obj.month == 8
+        assert self.hijri_date.month == 8
 
     def test_day(self):
-        assert self.hijri_obj.day == 13
+        assert self.hijri_date.day == 13
 
     def test_datetuple(self):
-        assert self.hijri_obj.datetuple() == (1410, 8, 13)
+        assert self.hijri_date.datetuple() == (1410, 8, 13)
 
     def test_isoformat(self):
-        assert self.hijri_obj.isoformat() == "1410-08-13"
+        assert self.hijri_date.isoformat() == "1410-08-13"
 
     def test_dmyformat(self):
-        assert self.hijri_obj.dmyformat() == "13/08/1410"
-        assert self.hijri_obj.dmyformat(padding=False) == "13/8/1410"
-        assert self.hijri_obj.dmyformat(separator=".") == "13.08.1410"
+        assert self.hijri_date.dmyformat() == "13/08/1410"
+        assert self.hijri_date.dmyformat(padding=False) == "13/8/1410"
+        assert self.hijri_date.dmyformat(separator=".") == "13.08.1410"
+
+    def test_year_length(self):
+        assert self.hijri_date.year_length() == 355
 
     def test_month_length(self):
-        assert self.hijri_obj.month_length() == 29
+        assert self.hijri_date.month_length() == 29
 
     def test_month_name(self):
-        assert self.hijri_obj.month_name() == "Sha’ban"
-        assert self.hijri_obj.month_name("en") == "Sha’ban"
-        assert self.hijri_obj.month_name("en-US") == "Sha’ban"
+        assert self.hijri_date.month_name() == "Sha'ban"
+        assert self.hijri_date.month_name("en") == "Sha'ban"
+        assert self.hijri_date.month_name("en-US") == "Sha'ban"
 
     def test_weekday(self):
-        assert self.hijri_obj.weekday() == 5
+        assert self.hijri_date.weekday() == 5
 
     def test_iso_weekday(self):
-        assert self.hijri_obj.isoweekday() == 6
+        assert self.hijri_date.isoweekday() == 6
 
     def test_day_name(self):
-        assert self.hijri_obj.day_name() == "Saturday"
-        assert self.hijri_obj.day_name("en") == "Saturday"
-        assert self.hijri_obj.day_name("en-US") == "Saturday"
+        assert self.hijri_date.day_name() == "Saturday"
+        assert self.hijri_date.day_name("en") == "Saturday"
+        assert self.hijri_date.day_name("en-US") == "Saturday"
 
     def test_notation(self):
-        assert self.hijri_obj.notation() == "AH"
-        assert self.hijri_obj.notation("en") == "AH"
-        assert self.hijri_obj.notation("en-US") == "AH"
+        assert self.hijri_date.notation() == "AH"
+        assert self.hijri_date.notation("en") == "AH"
+        assert self.hijri_date.notation("en-US") == "AH"
 
     def test_to_julian(self):
-        assert self.hijri_obj.to_julian() == 2447961
+        assert self.hijri_date.to_julian() == 2447961
 
     def test_to_gregorian(self):
-        assert self.hijri_obj.to_gregorian().datetuple() == (1990, 3, 10)
+        assert self.hijri_date.to_gregorian().datetuple() == (1990, 3, 10)
 
     def test_month_index(self):
-        assert self.hijri_obj._month_index() == 811
+        assert self.hijri_date._month_index() == 811
 
     @pytest.mark.parametrize(
-        "test_input", [(1410, 9, 30), (1356, 1, 1), (1500, 12, 30)]
+        "datetuple",
+        [(1410, 9, 30), (1356, 1, 1), (1500, 12, 30)],
     )
-    def test_valid_date(self, test_input):
-        year, month, day = test_input
-        try:
-            Hijri(year, month, day, validate=False)._check_date()
-        except (ValueError, OverflowError):
-            pytest.fail()
+    def test_valid_date(self, datetuple):
+        year, month, day = datetuple
+        Hijri(year, month, day, validate=True)
 
     @pytest.mark.parametrize(
-        "test_input, expected",
+        ("datetuple", "err_message"),
         [
-            ((37, 12, 30), "date out of range"),
-            ((1342, 12, 29), "date out of range"),
-            ((1501, 1, 1), "date out of range"),
+            (
+                (37, 12, 30),
+                f"year must be in {h_min[0]}-{h_max[0]}, got '37'",
+            ),
+            (
+                (1342, 12, 29),
+                f"year must be in {h_min[0]}-{h_max[0]}, got '1342'",
+            ),
+            (
+                (1501, 1, 1),
+                f"year must be in {h_min[0]}-{h_max[0]}, got '1501'",
+            ),
         ],
     )
-    def test_invalid_year(self, test_input, expected):
-        with pytest.raises(OverflowError) as e:
-            Hijri(*test_input, validate=False)._check_date()
-        assert str(e.value) == expected
+    def test_invalid_year(self, datetuple, err_message):
+        with pytest.raises(OverflowError, match=err_message):
+            Hijri(*datetuple, validate=True)
 
     @pytest.mark.parametrize(
-        "test_input, expected",
+        ("datetuple", "err_message"),
         [
-            ((1410, 0, 1), "month must be in 1..12"),
-            ((1410, 13, 1), "month must be in 1..12"),
-            ((1410, 8, 30), "day must be in 1..29 for month"),
+            ((1410, 0, 1), "month must be in 1-12, got '0'"),
+            ((1410, 13, 1), "month must be in 1-12, got '13'"),
+            ((1410, 8, 30), "day must be in 1-29 for month, got '30'"),
         ],
     )
-    def test_invalid_day_or_month(self, test_input, expected):
-        with pytest.raises(ValueError) as e:
-            Hijri(*test_input, validate=False)._check_date()
-        assert str(e.value) == expected
+    def test_invalid_day_or_month(self, datetuple, err_message):
+        with pytest.raises(ValueError, match=err_message):
+            Hijri(*datetuple, validate=True)
 
 
 @pytest.fixture(scope="class")
-def gregorian_obj(request):
-    request.cls.gregorian_obj = Gregorian(1990, 3, 10)
+def _gregorian_date(request):
+    request.cls.gregorian_date = Gregorian(1990, 3, 10)
 
 
-@pytest.mark.usefixtures("gregorian_obj")
+@pytest.mark.usefixtures("_gregorian_date")
 class TestGregorian:
+    gregorian_date = None
+
     def test_fromdate(self):
         test_date = date(2014, 12, 28)
         assert Gregorian.fromdate(test_date).datetuple() == (2014, 12, 28)
 
     def test_datetuple(self):
-        assert self.gregorian_obj.datetuple() == (1990, 3, 10)
+        assert self.gregorian_date.datetuple() == (1990, 3, 10)
 
     def test_dmyformat(self):
-        assert self.gregorian_obj.dmyformat() == "10/03/1990"
-        assert self.gregorian_obj.dmyformat(padding=False) == "10/3/1990"
-        assert self.gregorian_obj.dmyformat(separator=".") == "10.03.1990"
+        assert self.gregorian_date.dmyformat() == "10/03/1990"
+        assert self.gregorian_date.dmyformat(padding=False) == "10/3/1990"
+        assert self.gregorian_date.dmyformat(separator=".") == "10.03.1990"
 
     def test_month_name(self):
-        assert self.gregorian_obj.month_name() == "March"
-        assert self.gregorian_obj.month_name("en") == "March"
-        assert self.gregorian_obj.month_name("en-US") == "March"
+        assert self.gregorian_date.month_name() == "March"
+        assert self.gregorian_date.month_name("en") == "March"
+        assert self.gregorian_date.month_name("en-US") == "March"
 
     def test_day_name(self):
-        assert self.gregorian_obj.day_name() == "Saturday"
-        assert self.gregorian_obj.day_name("en") == "Saturday"
-        assert self.gregorian_obj.day_name("en-US") == "Saturday"
+        assert self.gregorian_date.day_name() == "Saturday"
+        assert self.gregorian_date.day_name("en") == "Saturday"
+        assert self.gregorian_date.day_name("en-US") == "Saturday"
 
     def test_notation(self):
-        assert self.gregorian_obj.notation() == "CE"
-        assert self.gregorian_obj.notation("en") == "CE"
-        assert self.gregorian_obj.notation("en-US") == "CE"
+        assert self.gregorian_date.notation() == "CE"
+        assert self.gregorian_date.notation("en") == "CE"
+        assert self.gregorian_date.notation("en-US") == "CE"
 
     def test_to_julian(self):
-        assert self.gregorian_obj.to_julian() == 2447961
+        assert self.gregorian_date.to_julian() == 2447961
 
     def test_to_hijri(self):
-        assert self.gregorian_obj.to_hijri().datetuple() == (1410, 8, 13)
+        assert self.gregorian_date.to_hijri().datetuple() == (1410, 8, 13)
 
     @pytest.mark.parametrize(
-        "test_input", [(1990, 3, 10), (1924, 8, 1), (2077, 11, 16)]
+        "datetuple",
+        [(1990, 3, 10), (1924, 8, 1), (2077, 11, 16)],
     )
-    def test_valid_range(self, test_input):
-        year, month, day = test_input
-        try:
-            Gregorian(year, month, day)._check_range()
-        except OverflowError:
-            pytest.fail()
+    def test_valid_range(self, datetuple):
+        year, month, day = datetuple
+        Gregorian(year, month, day)._check_range()
 
     @pytest.mark.parametrize(
-        "test_input, expected",
+        ("datetuple", "err_message"),
         [
-            ((1924, 7, 31), "date out of range"),
-            ((2077, 11, 17), "date out of range"),
+            (
+                (1924, 7, 31),
+                f"date must be in '{g_min_iso}'-'{g_max_iso}', got '1924-07-31'",
+            ),
+            (
+                (2077, 11, 17),
+                f"date must be in '{g_min_iso}'-'{g_max_iso}', got '2077-11-17'",
+            ),
         ],
     )
-    def test_invalid_range(self, test_input, expected):
-        with pytest.raises(OverflowError) as e:
-            Gregorian(*test_input)._check_range()
-        assert str(e.value) == expected
+    def test_invalid_range(self, datetuple, err_message):
+        with pytest.raises(OverflowError, match=err_message):
+            Gregorian(*datetuple)._check_range()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hijridate-2.4.1/tests/unit/test_locales.py` & `hijridate-2.5.0/tests/unit/test_locales.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,63 @@
+from typing import get_args
+
 import pytest
 
 from hijridate import locales
 
 
 @pytest.fixture(scope="class")
-def all_locales(request):
+def _all_locales(request):
     request.cls.locales = locales._locale_map
 
 
-@pytest.mark.usefixtures("all_locales")
+@pytest.mark.usefixtures("_all_locales")
 class TestLocalesValidity:
+    locales = None
+
     def test_locale_data_structure(self):
+        assert tuple(self.locales.keys())[:-1] == get_args(locales.Language)
         for locale_cls in self.locales.values():
             assert len(locale_cls.language_tag) == 2
             assert locale_cls.language_tag.islower()
             assert len(locale_cls.month_names) == 12
             assert all(locale_cls.month_names)  # not blank or None
             assert len(locale_cls.gregorian_month_names) == 12
             assert all(locale_cls.gregorian_month_names)  # not blank or None
             assert len(locale_cls.day_names) == 7
             assert all(locale_cls.day_names)  # not blank or None
             assert locale_cls.notation is not None
             assert locale_cls.gregorian_notation is not None
 
     def test_locale_map(self):
         assert len(locales._locale_map) > 0
-        assert "en" in locales._locale_map.keys()
+        assert "en" in locales._locale_map
 
     def test_duplicated_language_tag(self):
         with pytest.raises(LookupError):
 
             class ExtraLocale(locales.Locale):
                 language_tag = "en"
 
 
 class TestGettingLocale:
     class CustomLocale(locales.EnglishLocale):
         language_tag = "xx"
 
     @pytest.mark.parametrize(
-        "test_input",
+        "tag",
         [
             "xx",
             "XX",
             "xx-YY",
             "xx-yy",
             "xx_yy",
             "xx_YY",
             "xx_YY.UTF-8",
         ],
     )
-    def test_locale_possible_names(self, test_input):
-        assert locales.get_locale(test_input).__class__ == self.CustomLocale
+    def test_locale_possible_names(self, tag):
+        assert locales.get_locale(tag).__class__ == self.CustomLocale
 
     def test_unsupported_language(self):
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="unsupported language: xy"):
             locales.get_locale("xy")
```

