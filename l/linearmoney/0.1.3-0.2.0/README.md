# Comparing `tmp/linearmoney-0.1.3.tar.gz` & `tmp/linearmoney-0.2.0.tar.gz`

## Comparing `linearmoney-0.1.3.tar` & `linearmoney-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/_utils.py
--rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/cache.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/cldr_version.json
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/currencies.json
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/data.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/exceptions.py
--rw-r--r--   0        0        0  3144508 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/locales.json
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/mixins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/py.typed
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/resources.py
--rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/scalar.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/supported_iso_codes.json
--rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 linearmoney-0.1.3/src/linearmoney/vector.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 linearmoney-0.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 linearmoney-0.1.3/LICENSE
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 linearmoney-0.1.3/README.md
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 linearmoney-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 linearmoney-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/_utils.py
+-rw-r--r--   0        0        0    13168 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/cache.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/cldr_version.json
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/currencies.json
+-rw-r--r--   0        0        0    14723 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/data.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/exceptions.py
+-rw-r--r--   0        0        0  3144508 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/locales.json
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/mixins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/py.typed
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/resources.py
+-rw-r--r--   0        0        0    13244 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/scalar.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/supported_iso_codes.json
+-rw-r--r--   0        0        0    18152 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/vector.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/ext/__init__.py
+-rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 linearmoney-0.2.0/src/linearmoney/ext/sqlalchemy.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 linearmoney-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 linearmoney-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 linearmoney-0.2.0/README.md
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 linearmoney-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 linearmoney-0.2.0/PKG-INFO
```

### Comparing `linearmoney-0.1.3/src/linearmoney/__init__.py` & `linearmoney-0.2.0/src/linearmoney/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     "vector",
     "scalar",
     "data",
     "exceptions",
     "resources",
     "mixins",
     "cache",
+    "ext",
 ]
 
 
 import logging
 
 # Setup logging
 logger = logging.getLogger(__name__)
@@ -27,10 +28,10 @@
     data,
     exceptions,
     scalar,
     mixins,
     resources,
 )
 
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 
 CLDR_VERSION = resources.get_package_resource("cldr_version")
```

### Comparing `linearmoney-0.1.3/src/linearmoney/_utils.py` & `linearmoney-0.2.0/src/linearmoney/_utils.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/cache.py` & `linearmoney-0.2.0/src/linearmoney/cache.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/currencies.json` & `linearmoney-0.2.0/src/linearmoney/currencies.json`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/data.py` & `linearmoney-0.2.0/src/linearmoney/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,28 @@
 import locale as posix_locale
 
 from linearmoney import cache, resources
 from linearmoney.mixins import ImmutableDeduplicationMixin, EqualityByHashMixin
 from linearmoney.exceptions import UnknownDataError
 
 
-class FormatType(enum.StrEnum):
-    STANDARD = enum.auto()
-    ACCOUNTING = enum.auto()
+# This class needs to have a docstring, or the doctest examples in
+# the parent class `enum.Enum` will fail due to bare `Enum` not
+# being available in the test namespace.
+class FormatType(enum.Enum):
+    """Enum representing the allowed locale formats.
+
+    Primarily used to select l10n data with the `locale` function.
+    """
+
+    STANDARD = "standard"
+    ACCOUNTING = "accounting"
+
+    def __str__(self) -> str:
+        return self.value
 
 
 class DataMap(EqualityByHashMixin, ImmutableDeduplicationMixin, Mapping):
     """A read-only mapping."""
 
     __slots__ = ["_data", "_data_repr", "_hash"]
 
@@ -175,18 +186,18 @@
     Args:
         language:
             The language portion of the [locale tag](/linearmoney/glossary.html#locale-tag)
         region:
             The region (territory) portion of the
             [locale tag](/linearmoney/glossary.html#locale-tag)
         nformat:
-            The number format to use. Should be a member of the `FormatType` string enum.
+            The number format to use. Should be a member of the `FormatType` enum.
             The difference in format is generally only in negative numbers. E.g. -10 in
             'standard' vs. (10) in 'accounting'.
-            If you aren't sure which format you need, you probably want 'standard'.
+            If you aren't sure which format you need, you probably want 'FormatType.STANDARD`.
         **overrides:
             Formatting options to override the default formatting rules for the
             requested locale.
             The name of each kwarg is interpreted as a key in the `LocaleMap`
             returned as the `LocaleData.data` field, and its
             value will replace the value of that key in the output `DataMap`.
             E.g. `locale("en", "US", grouping_separator=';')` will return a `LocaleData`
@@ -217,28 +228,30 @@
         language = language.lower()
 
     if not region.isupper():
         region = region.upper()
 
     locales: LocaleMap
 
-    if nformat in _fallback_locales:
+    format_key = str(nformat)
+
+    if format_key in _fallback_locales:
         locale_string = "_".join([language, region])
         try:
-            locales = _fallback_locales[nformat][locale_string]
+            locales = _fallback_locales[format_key][locale_string]
         except KeyError as e:
             raise UnknownDataError(
                 f"invalid value for `language` {language} or `region` {region}. \
 Locale data not available under number format {nformat}"
             ) from e
 
     else:
         raise ValueError(
-            f"invalid value for `nformat`. Expected either 'standard' or \
-'accounting' got {nformat}"
+            f"invalid value for `nformat`. Expected either 'FormatType.Standard' or \
+'FormatType.Accounting' got {nformat}"
         )
 
     if overrides:
         # We cast to satisfy mypy since we can't use read-only TypedDict yet.
         # Remove this cast once pep 705 is implemented.
         return LocaleData(
             language,
```

### Comparing `linearmoney-0.1.3/src/linearmoney/exceptions.py` & `linearmoney-0.2.0/src/linearmoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/locales.json` & `linearmoney-0.2.0/src/linearmoney/locales.json`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/mixins.py` & `linearmoney-0.2.0/src/linearmoney/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 __all__: list[str] = [
     "ImmutableDeduplicationMixin",
     "EqualityByHashMixin",
 ]
 
 
 from abc import ABCMeta, abstractmethod
-from typing import ClassVar, Self
+from typing import TYPE_CHECKING, ClassVar
 from collections.abc import Hashable, Sequence
 
+if TYPE_CHECKING:
+    from typing import Self
+
 
 class ImmutableDeduplicationMixin:
     """A mixin class that provides common dunder method implementations for
     logically immutable objects.
 
     Provides recursive implementations of `__getstate__` and
     `__setstate__` based on the `__slots__` declared on the class and all of its
```

### Comparing `linearmoney-0.1.3/src/linearmoney/resources.py` & `linearmoney-0.2.0/src/linearmoney/resources.py`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/scalar.py` & `linearmoney-0.2.0/src/linearmoney/scalar.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,18 +288,18 @@
         >>> lm.scalar.l10n(rounded_val, cad, en_US, international=True)
         'CAD 10.07'
         >>> fr_FR = lm.data.locale("fr", "fr")  # French-France
         >>> eur = lm.data.currency("eur")
         >>> val = lm.vector.evaluate(av, "eur", fv)
         >>> rounded_val = lm.scalar.roundas(val, eur)
         >>> lm.scalar.l10n(rounded_val, eur, fr_FR)
-        '20,14€'
+        '20,14 €'
         >>> cash_rounded_val = lm.scalar.roundas(val, eur, cash=True)
         >>> lm.scalar.l10n(cash_rounded_val, eur, fr_FR)
-        '20,14€'
+        '20,14 €'
         >>> lm.scalar.l10n(rounded_val, eur, fr_FR, international=True)
         '20,14 EUR'
     """
 
     # TODO: Refactor this function for readability.
 
     iso_code = currency.iso_code
```

### Comparing `linearmoney-0.1.3/src/linearmoney/supported_iso_codes.json` & `linearmoney-0.2.0/src/linearmoney/supported_iso_codes.json`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/src/linearmoney/vector.py` & `linearmoney-0.2.0/src/linearmoney/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,24 @@
     "ForexVector",
     "CurrencySpace",
     "RatesDict",
 ]
 
 import decimal
 import copy
-from typing import TypeAlias, Self, TypedDict, TypeVar
+from typing import TYPE_CHECKING, TypeAlias, TypedDict, TypeVar
 from collections.abc import Iterator
 
 from linearmoney import cache, _utils
 from linearmoney.mixins import ImmutableDeduplicationMixin, EqualityByHashMixin
 from linearmoney.exceptions import SpaceError, IntegrityError
 
+if TYPE_CHECKING:
+    from typing import Self
+
 DecimalVector: TypeAlias = tuple[decimal.Decimal, ...]
 
 _ZERO = decimal.Decimal(0)
 _ONE = decimal.Decimal(1)
 
 # TypeVar needed for typechecking subclasses returned in place of base class.
 V = TypeVar("V", bound="MoneyVector")
@@ -200,23 +203,23 @@
     @cache.cached()
     def __neg__(self) -> Self:
         return self.__class__(tuple([-i for i in self]), self.axes)
 
     @property
     @cache.cached()
     def dim(self) -> int:
-        """The dimension of this `MunnyVector`."""
+        """The dimension of this `MoneyVector`."""
 
         return len(self)
 
     @property
     @cache.cached()
     def axes(self) -> tuple[str, ...]:
         """Tuple of the ISO 4217 alpha currency codes representing the axes of this
-        `MunnyVector`."""
+        `MoneyVector`."""
 
         return self._axes
 
 
 class ForexVector(MoneyVector):
     """A [forex vector](/linearmoney/glossary.html#forex-vector) in the
     [linear money model](/linear_money_model.html)."""
```

### Comparing `linearmoney-0.1.3/LICENSE` & `linearmoney-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linearmoney-0.1.3/README.md` & `linearmoney-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 - Full support for arithmetic with monetary amounts in different currencies.
 - Full support for non-destructive currency conversion.
 - Full support for fractional currency rounding and fixed-point rounding.
 - Full support for currency formatting and localization.
 - No dependencies other than Python itself.
 - Completely thread-safe.
 - 100% Test and API Documentation coverage.
+- Database/ORM integrations.
 
 The linearmoney library takes a non-traditional approach to financial applications
 by using linear algebra internally to ensure the correctness of monetary calculations
 involving multiple currencies without passing this burden onto the programmer.
 Understanding of linear algebra is not needed to use and understand the linearmoney
 library, but an understanding of basic arithmetic with vectors is helpful for
 understanding how the library works under the hood.
@@ -43,15 +44,15 @@
 the [Linear Money Model](https://grammacc.github.io/linearmoney/linear_money_model.html) article.
 
 linearmoney uses the amazing [Unicode CLDR-JSON](https://github.com/unicode-org/cldr-json)
 data to provide data-driven interfaces for currency rounding, formatting, and localization.
 
 ## Installation
 
-linearmoney requires Python >= 3.11
+linearmoney requires Python >= 3.10
 
 From PyPi:
 
 ```bash
 pip install linearmoney
 ```
 
@@ -103,14 +104,32 @@
 the code can become verbose compared to more idiomatic Python, but this also makes
 the code more explicit and easier to test.
 
 See the [Recipes](https://grammacc.github.io/linearmoney/recipes.html)
 section of the user guide for
 some examples of how to mitigate the verbosity of the library and other helpful patterns.
 
+## Optional Extensions
+
+The `linearmoney.ext` sub-package provides optional integrations with other libraries/tools.
+
+Most tools shouldn't need any kind of adapter layer for you to use linearmoney with
+them since you would normally evaluate a money vector whenever you need to do something
+with its value outside of linearmoney's functions or math between vectors. The exceptions
+to this are ORMs and similar tools that need some kind of serialization step to be
+performed.
+
+[SQLAlchemy](https://grammacc.github.io/linearmoney/api_reference/linearmoney/ext/sqlalchemy.html)
+integrations are implemented, and Django ORM is planned.
+
+If there is a tool that you want better integration with or simply some kind of
+extra functionality that requires additional dependencies, please
+[open an issue](https://github.com/GrammAcc/linearmoney/issues/new/choose) and
+we will evaluate if it is within the scope of the project to support as an extension.
+
 ## Contributing
 
 Contributions are greatly appreciated!
 
 See the [contributing guidelines](/CONTRIBUTING.md) to get started.
 
 ## Roadmap
```

### Comparing `linearmoney-0.1.3/pyproject.toml` & `linearmoney-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "linearmoney"
 dynamic = ["version"]
 description = "Full multi-currency support for python."
 authors = [{name = "GrammAcc", email = "grammaticallyacceptable@grammacc.dev"}]
 maintainers = [{name = "GrammAcc", email = "grammaticallyacceptable@grammacc.dev"}]
 license = "MIT"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 keywords = ["money", "framework", "currency", "forex", "fintech"]
 classifiers = ["Development Status :: 3 - Alpha"]
 
 [project.urls]
 homepage = "https://github.com/GrammAcc/linearmoney"
 bug_tracker = "https://github.com/GrammAcc/linearmoney/issues"
 documentation = "https://grammacc.github.io/linearmoney"
@@ -22,24 +22,25 @@
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-parametrize-cases",
     "pytest-lazy-fixtures",
 ]
+sqlalchemy = ["sqlalchemy"]
+
 
 [tool.hatch.version]
 path = "src/linearmoney/__init__.py"
 
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["*.json", "py.typed"]
 
-
 # This is needed for hatchling to find the version in the package __init__.py file.
 # See https://github.com/pypa/hatch/issues/981#issuecomment-1743631364
 [tool.hatch.build.targets.sdist]
 include = ["src"]
 
 # This is needed for hatchling to find the version in the package __init__.py file.
 # See https://github.com/pypa/hatch/issues/981#issuecomment-1743631364
@@ -49,56 +50,71 @@
 
 [tool.hatch.envs.default]
 python = "3.12"
 
 [tool.hatch.envs.default.scripts]
 ci = [
     "hatch run test:suite",
-    "hatch run -py=3.11 test:cov",
+    "hatch run -py=3.10,3.11 test:cov",
     "hatch run docs:test-prose",
     "hatch run docs:test-in-source",
     "hatch run types:check",
     "hatch run style:lintsrc",
     "hatch run style:linttests",
     "hatch run style:lintdocs",
 ]
 all = [
     "hatch run style:format",
     "- hatch run test:suite",
-    "- hatch run -py=3.11 test:cov",
+    "- hatch run -py=3.10,3.11 test:cov",
     "- hatch run docs:test-prose",
     "- hatch run docs:test-in-source",
     "- hatch run types:check",
     "- hatch run style:lintsrc",
     "- hatch run style:linttests",
     "- hatch run style:lintdocs",
 ]
+quicktest = "hatch run -py=3.10,3.11 test:suite {args}"
+
+[tool.hatch.envs.py310]
+python = "3.10"
+
+[tool.hatch.envs.py311]
+python = "3.11"
 
 
 [tool.hatch.envs.test]
 description = "Test Suite and Coverage Reporting"
 dependencies = [
     "pytest",
     "pytest-cov",
     "pytest-parametrize-cases",
     "pytest-lazy-fixtures",
+    "pytest-asyncio",
+    "aiosqlite",
+    "sqlalchemy[asyncio]",
 ]
+features = ["sqlalchemy"]
 
 [[tool.hatch.envs.test.matrix]]
-python = ["3.11", "3.12"]
+python = ["3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.test.scripts]
-suite = "pytest"
-cov = "pytest --cov-config=pyproject.toml --cov-report html:htmlcov --cov=linearmoney"
+suite = "pytest {args}"
+cov = "pytest --cov-config=pyproject.toml --cov-report html:htmlcov --cov=linearmoney {args}"
 prod = "- pip install --force-reinstall -i https://test.pypi.org/simple linearmoney && pytest"
+ext = "pytest tests/ext {args}"
 
 
 [tool.hatch.envs.types]
 description = "Run static type checker"
-dependencies = ["mypy"]
+dependencies = [
+    "mypy",
+    "sqlalchemy[mypy]",
+]
 
 [tool.hatch.envs.types.scripts]
 check = "mypy -p linearmoney"
 
 
 [tool.hatch.envs.style]
 detached = true
@@ -108,26 +124,27 @@
     "black",
     "flake8",
 ]
 
 [tool.hatch.envs.style.scripts]
 format = "black ."
 lintsrc = "flake8 src"
-linttests = "flake8 --extend-ignore E501 tests"
+linttests = "flake8 tests"
 lintdocs = "flake8 documentation"
 
 
 [tool.hatch.envs.docs]
 description = "Documentation generation and utilities"
 dependencies = [
     "pdoc",
     "mkdocs",
     "mkdocs-material",
     "pytest",
 ]
+features = ["sqlalchemy"]
 
 [tool.hatch.envs.docs.scripts]
 build = [
     "sh -c 'pygmentize -f html -a .language-python -S default > documentation/md/syntax-highlighting.css'",
     "pdoc 'linearmoney' --docformat='google' --output-directory='documentation/md/api_reference' --template-directory='documentation/pdoc_templates'",
     "mkdocs build -f documentation/mkdocs.yml",
 ]
@@ -144,14 +161,15 @@
 test = "python tests/cldr/check_data.py"
 
 
 [tool.pytest.ini_options]
 log_file="testsuite.log"
 log_file_level="DEBUG"
 addopts = "--import-mode=importlib --show-capture=no --ignore=cldr-json"
+asyncio_mode = "auto"
 
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@abstractmethod",
```

### Comparing `linearmoney-0.1.3/PKG-INFO` & `linearmoney-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.3
 Name: linearmoney
-Version: 0.1.3
+Version: 0.2.0
 Summary: Full multi-currency support for python.
 Project-URL: homepage, https://github.com/GrammAcc/linearmoney
 Project-URL: bug_tracker, https://github.com/GrammAcc/linearmoney/issues
 Project-URL: documentation, https://grammacc.github.io/linearmoney
 Project-URL: repository, https://github.com/GrammAcc/linearmoney
 Author-email: GrammAcc <grammaticallyacceptable@grammacc.dev>
 Maintainer-email: GrammAcc <grammaticallyacceptable@grammacc.dev>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: currency,fintech,forex,framework,money
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Provides-Extra: dev
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-lazy-fixtures; extra == 'dev'
 Requires-Dist: pytest-parametrize-cases; extra == 'dev'
+Provides-Extra: sqlalchemy
+Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Description-Content-Type: text/markdown
 
 # linearmoney
 
 Full multi-currency support for python.
 
 ---
@@ -47,14 +49,15 @@
 - Full support for arithmetic with monetary amounts in different currencies.
 - Full support for non-destructive currency conversion.
 - Full support for fractional currency rounding and fixed-point rounding.
 - Full support for currency formatting and localization.
 - No dependencies other than Python itself.
 - Completely thread-safe.
 - 100% Test and API Documentation coverage.
+- Database/ORM integrations.
 
 The linearmoney library takes a non-traditional approach to financial applications
 by using linear algebra internally to ensure the correctness of monetary calculations
 involving multiple currencies without passing this burden onto the programmer.
 Understanding of linear algebra is not needed to use and understand the linearmoney
 library, but an understanding of basic arithmetic with vectors is helpful for
 understanding how the library works under the hood.
@@ -64,15 +67,15 @@
 the [Linear Money Model](https://grammacc.github.io/linearmoney/linear_money_model.html) article.
 
 linearmoney uses the amazing [Unicode CLDR-JSON](https://github.com/unicode-org/cldr-json)
 data to provide data-driven interfaces for currency rounding, formatting, and localization.
 
 ## Installation
 
-linearmoney requires Python >= 3.11
+linearmoney requires Python >= 3.10
 
 From PyPi:
 
 ```bash
 pip install linearmoney
 ```
 
@@ -124,14 +127,32 @@
 the code can become verbose compared to more idiomatic Python, but this also makes
 the code more explicit and easier to test.
 
 See the [Recipes](https://grammacc.github.io/linearmoney/recipes.html)
 section of the user guide for
 some examples of how to mitigate the verbosity of the library and other helpful patterns.
 
+## Optional Extensions
+
+The `linearmoney.ext` sub-package provides optional integrations with other libraries/tools.
+
+Most tools shouldn't need any kind of adapter layer for you to use linearmoney with
+them since you would normally evaluate a money vector whenever you need to do something
+with its value outside of linearmoney's functions or math between vectors. The exceptions
+to this are ORMs and similar tools that need some kind of serialization step to be
+performed.
+
+[SQLAlchemy](https://grammacc.github.io/linearmoney/api_reference/linearmoney/ext/sqlalchemy.html)
+integrations are implemented, and Django ORM is planned.
+
+If there is a tool that you want better integration with or simply some kind of
+extra functionality that requires additional dependencies, please
+[open an issue](https://github.com/GrammAcc/linearmoney/issues/new/choose) and
+we will evaluate if it is within the scope of the project to support as an extension.
+
 ## Contributing
 
 Contributions are greatly appreciated!
 
 See the [contributing guidelines](/CONTRIBUTING.md) to get started.
 
 ## Roadmap
```

