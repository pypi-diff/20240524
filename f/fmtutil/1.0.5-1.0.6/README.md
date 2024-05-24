# Comparing `tmp/fmtutil-1.0.5.tar.gz` & `tmp/fmtutil-1.0.6.tar.gz`

## Comparing `fmtutil-1.0.5.tar` & `fmtutil-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/__about__.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/__main__.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/__type.py
--rw-r--r--   0        0        0    36743 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/__version.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/cli.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/exceptions.py
--rw-r--r--   0        0        0   136785 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/formatter.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 fmtutil-1.0.5/fmtutil/utils.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.5/LICENSE
--rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.5/README.md
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 fmtutil-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fmtutil-1.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/__about__.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/__main__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/__type.py
+-rw-r--r--   0        0        0    38080 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/__version.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/cli.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/exceptions.py
+-rw-r--r--   0        0        0   136982 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/formatter.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 fmtutil-1.0.6/fmtutil/utils.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.6/LICENSE
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 fmtutil-1.0.6/README.md
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 fmtutil-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 fmtutil-1.0.6/PKG-INFO
```

### Comparing `fmtutil-1.0.5/fmtutil/__init__.py` & `fmtutil-1.0.6/fmtutil/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
+import logging
 
 from .__about__ import (
     __version__,
     __version_tuple__,
 )
 from .__version import (
     BaseVersion as Ver,
@@ -41,14 +42,16 @@
     Storage,
     Version,
     dict2const,
     make_const,
     make_group,
 )
 
+logging.getLogger(__name__)
+
 __all__ = (
     "Formatter",
     "FormatterType",
     "Serial",
     "Datetime",
     "Version",
     "Naming",
@@ -63,13 +66,15 @@
     "make_group",
     "FormatterArgumentError",
     "FormatterError",
     "FormatterKeyError",
     "FormatterValueError",
     "FormatterGroupArgumentError",
     "FormatterGroupValueError",
+    "ReturnFormattersType",
+    "ReturnPrioritiesType",
     "Ver",
     "VerPackage",
     "VerSemver",
     "__version__",
     "__version_tuple__",
 )
```

### Comparing `fmtutil-1.0.5/fmtutil/__type.py` & `fmtutil-1.0.6/fmtutil/__type.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Union
 
 from typing_extensions import TypeAlias
 
 String: TypeAlias = Union[str, bytes]
 DictStr: TypeAlias = dict[str, str]
 TupleInt: TypeAlias = tuple[int, ...]
+TupleStr: TypeAlias = tuple[str, ...]
 
 
 class InfObject:
     def __repr__(self) -> str:
         return "Infinity"
 
     def __hash__(self) -> int:
```

### Comparing `fmtutil-1.0.5/fmtutil/__version.py` & `fmtutil-1.0.6/fmtutil/__version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ------------------------------------------------------------------------------
 # This file license under the BSD-3 License of the ``python-semver`` package and
 # BSD and Apache-2.0 Licenses of the ``packaging`` package the provide by PyPA.
 # ------------------------------------------------------------------------------
-# references:
+# References:
 # * [GitHub: Python - semver](https://github.com/python-semver/python-semver)
 # * [GitHub: PYPA - Packaging](https://github.com/pypa/packaging)
 # ------------------------------------------------------------------------------
 from __future__ import annotations
 
 import itertools
 import re
@@ -20,20 +20,21 @@
     NoReturn,
     SupportsInt,
     Union,
     cast,
     get_args,
 )
 
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 from .__type import (
     Inf,
     NegInf,
     String,
+    TupleStr,
 )
 
 Comparable: TypeAlias = Union[
     "BaseVersion",
     dict[str, int],
     Collection[int],
     str,
@@ -162,30 +163,30 @@
 def cmp(self: Any, other: Any) -> int:
     """Return integer value from comparison logic
 
     :param self: A self value that want to compare.
     :param other: Another value that able to compare with self.
 
     :rtype: int
-    :return: An integer value from these scenarios:
+    :returns: An integer value from these scenarios:
         * if self < other, then -1
         * if self == other, then 0
         * if self > other, then 1.
     """
     return (self > other) - (self < other)
 
 
 def increment(s: str) -> str:
     """Look for the last sequence of number(s) in a string and increment.
 
     :param s: A string value to search for increase the last sequence number.
     :type s: str
 
     :rtype: str
-    :return: An incremented string.
+    :returns: An incremented string.
     """
     if m := re.compile(r"(?:\D*(\d+)\D*)+").search(s):
         next_value = str(int(m.group(1)) + 1)
         start, end = m.span(1)
         s = s[: max(end - len(next_value), start)] + next_value + s[end:]
     return s
 
@@ -200,16 +201,19 @@
     )
 
 
 class BaseVersion:
     """A Base Version class.
 
     :param major:
+    :type major: SupportsInt(=0)
     :param minor:
+    :type minor: SupportsInt(=0)
     :param patch:
+    :type patch: SupportsInt(=0)
     """
 
     __slots__ = (
         "major",
         "minor",
         "patch",
     )
@@ -250,62 +254,65 @@
             raise AttributeError(f"attribute {attr!r} is readonly")
         super().__setattr__(attr, value)
 
     def to_tuple(self) -> tuple[Union[int, str], ...]:
         """Convert the BaseVersion object to a tuple.
 
         :rtype: Tuple[int, int, int]
-        :return: A tuple with all the parts
+        :returns: A tuple with all the parts
         """
         return tuple(getattr(self, attr) for attr in self.__class__.__slots__)
 
     def to_dict(self) -> dict[str, int]:
         """Convert the Version object to a dict.
 
-        :return: A dict with the keys in the order ``major``, ``minor``, and
+        :returns: A dict with the keys in the order ``major``, ``minor``, and
             ``patch``.
         """
         return {attr: getattr(self, attr) for attr in self.__class__.__slots__}
 
     def __iter__(self) -> Iterable[int]:
         """Return iter(self)."""
         yield from self.to_tuple()
 
-    def bump_major(self) -> BaseVersion:
+    def bump_major(self) -> Self:
         """Raise the major part of the version, return a new object
         but leave self untouched.
 
-        :return: new object with the raised major part
+        :returns: new object with the raised major part
         """
         return self.__class__(self.major + 1)
 
-    def bump_minor(self) -> BaseVersion:
+    def bump_minor(self) -> Self:
         """Raise the minor part of the version, return a new object
         but leave self untouched.
 
-        :return: new object with the raised minor part
+        :returns: new object with the raised minor part
         """
         return self.__class__(self.major, self.minor + 1)
 
-    def bump_patch(self) -> BaseVersion:
+    def bump_patch(self) -> Self:
         """Raise the patch part of the version, return a new object
         but leave self untouched.
 
-        :return: new object with the raised patch part
+        :returns: new object with the raised patch part
         """
         return self.__class__(self.major, self.minor, self.patch + 1)
 
     def compare(self, other: Comparable) -> int:
         """Compare self with this other.
 
         :param other: the second version
-        :return: The return value is negative if ver1 < ver2,
+        :type other: Comparable
+
+        :rtype: int
+        :returns: The return value is negative if ver1 < ver2,
             zero if ver1 == ver2 and strictly positive if ver1 > ver2
         """
-        cls: type[BaseVersion] = type(self)
+        cls: type[Self] = type(self)
         if isinstance(other, get_args(String)):
             other = cls.parse(other)
         elif isinstance(other, dict):
             other = cls(**other)
         elif isinstance(other, (tuple, list)):
             other = cls(*other)
         elif not isinstance(other, cls):
@@ -317,24 +324,24 @@
             self.to_tuple()[:3],
             other.to_tuple()[:3],
         )
 
     def next_version(
         self,
         part: str,
-    ) -> BaseVersion:
+    ) -> Self:
         """Determines next version, preserving natural order.
 
-        :param part: One of "major", "minor", "patch"
+        :param part: an one of "major", "minor", "patch" part of version.
         :type part: str
 
-        :rtype: BaseVersion
-        :return: A new object with the appropriate part raised
+        :rtype: Self
+        :returns: A new object with the appropriate part raised
         """
-        valid_parts: tuple[str, ...] = self.__class__.__slots__
+        valid_parts: TupleStr = self.__class__.__slots__
         if part not in self.__class__.__slots__:
             raise ValueError(
                 f"Invalid part. Expected one of {valid_parts}, but got {part!r}"
             )
         return getattr(self, "bump_" + part)()
 
     @comparison
@@ -360,27 +367,28 @@
     @comparison
     def __ge__(self, other: Comparable) -> bool:
         return self.compare(other) >= 0
 
     def __getitem__(
         self,
         index: Union[int, slice],
-    ) -> Union[int, str | None, tuple[Union[int, str], ...]]:
+    ) -> int | str | tuple[Union[int, str], ...] | None:
         """If the part requested is undefined, or a part of the range requested
         is undefined, it will throw an index error.
 
         Negative indices are not supported.
 
         :param index: a positive integer indicating the offset or a ``slice``
             object.
         :type index: Union[int, slice]
 
         :raises IndexError: if index is beyond the range or a part is None
 
-        :return: the requested part of the version at position index
+        :rtype: int | str | tuple[Union[int, str], ...] | None
+        :returns: the requested part of the version at position index
         """
         if isinstance(index, int):
             index = slice(index, index + 1)
         index = cast(slice, index)
 
         if (
             isinstance(index, slice)
@@ -409,42 +417,50 @@
     def __str__(self) -> str:
         return ".".join(str(x) for x in self.to_tuple())
 
     def __hash__(self) -> int:
         return hash(self.to_tuple())
 
     @classmethod
-    def extract_wildcard(cls, expr: str) -> tuple[BaseVersion, BaseVersion]:
+    def extract_wildcard(cls, expr: str) -> tuple[Self, Self]:
         """Extract version instance from an input wildcard version value.
 
         :param expr: An expression string value of version wildcard.
             2.1.*   --> >=2.1.0, < 2.2.0
             2.*     --> >=2.0.0, <3.0.0
             *       --> >=0.0.0
         :type expr: str
+
+        :rtype: tuple[BaseVersion, BaseVersion]
         """
         if expr == "*":
             return cls.parse("0.0.0"), Inf
         try:
-            base_expr: BaseVersion = cls.parse(
+            base_expr: Self = cls.parse(
                 expr.replace("*", "0"), optional_minor_and_patch=True
             )
-            upper_expr: BaseVersion = cls.parse(
+            upper_expr: Self = cls.parse(
                 increment(expr.replace("*", "").rstrip(".")),
                 optional_minor_and_patch=True,
             )
             return base_expr, upper_expr
         except ValueError as err:
             raise ValueError(
                 f"Wildcard does not support for version expr format, {expr!r}"
             ) from err
 
     @staticmethod
     def __validate_expr_match(expr: str) -> tuple[str, str]:
-        """Validate expression string of version matching string value."""
+        """Validate expression string of version matching string value.
+
+        :param expr:
+        :type expr: str
+
+        :rtype: tuple[str, str]
+        """
         prefix: str = expr[:2]
         match: str
         if prefix in (
             ">=",
             "<=",
             "==",
             "!=",
@@ -483,17 +499,18 @@
             ``~=``  ~= 1        --> >= 1.0.0, < 2.0.0
                     ~= 2.2      --> >= 2.2.0, < 3.0.0
                     ~= 1.4.5    --> >= 1.4.5, < 1.5.0
                     ~= 1.4.5a4  --> >= 1.4.5a4, < 1.5.0
             ``~``   ``~=``
             ``^``   ^2.1.7      --> >=2.1.7, <3.0.0
                     ^0.24.1     --> >=0.24.1, <0.25.0
+        :type expr: str
 
         :rtype: bool
-        :return: True if the expression matches the version, otherwise False
+        :returns: True if the expression matches the version, otherwise False
         """
         prefix, match = self.__validate_expr_match(expr)
         possibilities = {
             ">": (1,),
             "<": (-1,),
             "==": (0,),
             "!=": (-1, 1),
@@ -535,29 +552,31 @@
             return cmp_res in possibility and (
                 self.compare(self.__class__(**pair_version)) < 0
             )
         return cmp_res in possibility
 
     @classmethod
     def parse(
-        cls: type[BaseVersion],
+        cls: type[Self],
         version: String,
         *,
         optional_minor_and_patch: bool = False,
-    ) -> BaseVersion:
+    ) -> Self:
         """Parse version string to a Version instance.
 
         :param version: A version string that want to parse.
+        :type version: String
         :param optional_minor_and_patch: An optional flag for parsing with minor
             and patch value if it exists.
+        :type optional_minor_and_patch: bool(=False)
 
         :raises ValueError: if version is invalid
         :raises TypeError: if version contains the wrong type
 
-        :return: a new :class:`Version` instance
+        :returns: a new :class:`Version` instance
         """
         if isinstance(version, bytes):
             version = str(version, "utf-8", "strict")
         elif not isinstance(version, str):
             raise TypeError(f"not expecting type '{type(version)}'")
 
         if optional_minor_and_patch:
@@ -565,23 +584,24 @@
         else:
             match = cls.regex.match(version)
         if match is None:
             raise ValueError(f"{version} is not valid {cls.__name__} string")
 
         return cls(**match.groupdict())
 
-    def replace(self, **parts: Union[int, str | None]) -> BaseVersion:
+    def replace(self, **parts: int | str | None) -> Self:
         """Replace one or more parts of a version and return a new instance.
 
         :param parts: the parts to be updated. Valid keys are:
             ``major``, ``minor``, ``patch``, ``pre``, or ``build``
+        :type parts: int | str | None
 
         :raises TypeError: if ``parts`` contain invalid keys
 
-        :return: the new instance with the changed parts
+        :returns: the new instance with the changed parts
         """
         version = self.to_dict()
         version.update(parts)
         try:
             return self.__class__(**version)
         except TypeError as err:
             unknown = set(parts) - set(self.to_dict())
@@ -592,30 +612,33 @@
             raise TypeError(error) from err
 
     @classmethod
     def is_valid(cls, version: str) -> bool:
         """Check if the string is a valid base version.
 
         :param version: the version string to check
+        :type version: str
 
         :rtype: bool
-        :return: True if the version string is a valid base version, False
+        :returns: True if the version string is a valid base version, False
                 otherwise.
         """
         try:
             cls.parse(version)
             return True
         except ValueError:
             return False
 
     def is_compatible(self, other: BaseVersion) -> bool:
         """Check if current version is compatible with other version.
 
+        :raises TypeError: if other value that not sub-class of BaseVersion.
+
         :param other: the version to check for compatibility
-        :return: True, if ``other`` is compatible with the old version,
+        :returns: True, if ``other`` is compatible with the old version,
             otherwise False
         """
         if not isinstance(other, BaseVersion):
             raise TypeError(f"Expected a Version type but got {type(other)}")
 
         # All major-0 versions should be incompatible with anything but itself
         if (0 == self.major == other.major) and (self[:3] != other[:3]):
@@ -754,14 +777,15 @@
             )
         return self.epoch, release, pre, post, dev, local
 
     @staticmethod
     def __extract_local(
         local: str | None,
     ) -> tuple[Union[str, int], ...] | None:
+        """Extract a pair of local layer from full string local."""
         if local is not None:
             return tuple(
                 part.lower() if not part.isdigit() else int(part)
                 for part in re.compile(r"[._-]").split(local)
             )
         return None
 
@@ -776,19 +800,19 @@
         return self._extract_letter(self.post)[1] if self.post else None
 
     @property
     def v_dev(self) -> int | None:
         """Return the version number of dev part if it was set."""
         return self._extract_letter(self.dev)[1] if self.dev else None
 
-    def bump_pre(self, token: str | None = "rc") -> VersionPackage:
+    def bump_pre(self, token: str | None = "rc") -> Self:
         """Raise the pre part of the packaging version, return a new object.
 
-        :rtype: VersionPackage
-        :return: A new object with the raised pre part.
+        :rtype: Self
+        :returns: A new object with the raised pre part.
         """
         cls = type(self)
         if self.pre is not None:
             pre = self.pre
         elif token == "":
             pre = "0"
         else:
@@ -799,69 +823,75 @@
             self.epoch,
             self.major,
             self.minor,
             self.patch,
             pre,
         )
 
-    def bump_post(self) -> VersionPackage:
+    def bump_post(self) -> Self:
         """Raise the post part of the packaging version, return a new object.
 
-        :rtype: VersionPackage
-        :return: A new object with the raised post part.
+        :rtype: Self
+        :returns: A new object with the raised post part.
         """
         post: str = increment(self.post or "post0")
         return self.__class__(
             self.epoch,
             self.major,
             self.minor,
             self.patch,
             self.pre,
             post,
         )
 
-    def bump_dev(self) -> VersionPackage:
+    def bump_dev(self) -> Self:
         """Raise the dev part of the packaging version, return a new object.
 
-        :rtype: VersionPackage
-        :return: A new object with the raised dev part.
+        :rtype: Self
+        :returns: A new object with the raised dev part.
         """
         dev: str = increment(self.dev or "dev0")
         return self.__class__(
             self.epoch,
             self.major,
             self.minor,
             self.patch,
             self.pre,
             self.post,
             dev,
         )
 
-    def bump_local(self) -> VersionPackage:
+    def bump_local(self) -> Self:
         """Raise the local part of the packaging version, return a new object.
 
-        :rtype: VersionPackage
-        :return: A new object with the raised local part.
+        :rtype: Self
+        :returns: A new object with the raised local part.
         """
         local: str = increment(self.local or "local0")
         return self.__class__(
             self.epoch,
             self.major,
             self.minor,
             self.patch,
             self.pre,
             self.post,
             self.dev,
             local,
         )
 
-    def next_version(self, part: str, pre_token: str = "a") -> VersionPackage:
-        """
-        :rtype: VersionPackage
-        :return: A new object with replace the new part of an input part value.
+    def next_version(self, part: str, pre_token: str = "a") -> Self:
+        """Return the next Packaging version.
+
+        :param part: a part that want to generate the next version.
+        :type part: str
+        :param pre_token: a pre kind token string value.
+        :type pre_token: str(='a')
+
+        :rtype: Self
+        :returns: A new object with replace the new part of an input part value.
         """
         cls = type(self)
         valid_parts = cls.__slots__[:-1]
         if part not in valid_parts:
             raise ValueError(
                 f"Invalid part. Expected one of {valid_parts}, but got {part!r}"
             )
@@ -873,14 +903,15 @@
         ):
             return version.replace(pre=None, post=None, dev=None, local=None)
         if part == "pre":
             return version.bump_pre(pre_token)
         return getattr(version, "bump_" + part)
 
     def __str__(self) -> str:
+        """Return the full version that joining in string format."""
         version: str = f"{self.major}.{self.minor}.{self.patch}"
         if self.epoch > 0:
             version = f"{self.epoch}!{version}"
         if self.pre:
             version += self.pre
         if self.post:
             version += self.post
@@ -895,18 +926,26 @@
 
     def public(self) -> str:
         """Return a public version format string value."""
         return str(self).split("+", maxsplit=1)[0]
 
     @classmethod
     def parse(
-        cls: type[VersionPackage],
+        cls: type[Self],
         version: String,
         optional_minor_and_patch: bool = False,
-    ) -> VersionPackage:
+    ) -> Self:
+        """Return the Packaging version that parsing from an any string value.
+
+        :param version: an any string value that want to parse.
+        :param optional_minor_and_patch: a optional flag.
+
+        :rtype: Self
+        :return: the Packaging version that parsing from an any string value.
+        """
         if isinstance(version, bytes):
             version = str(version, "utf-8", "strict")
         elif not isinstance(version, get_args(String)):
             raise TypeError(f"not expecting type '{type(version)}'")
 
         if (match := cls.regex.match(version)) is None:
             raise ValueError(f"{version} is not valid Packaging Version string")
@@ -933,14 +972,15 @@
             raise TypeError(
                 f"Expected str, bytes, dict, tuple, list, or {cls.__name__} "
                 f"instance, but got {type(other)}"
             )
         return cmp(self.__extract_tuple(), other.__extract_tuple())
 
     def is_compatible(self, other: VersionPackage) -> bool:
+        """Check the other version that compatible with this Packaging version."""
         if not isinstance(other, VersionPackage):
             raise TypeError(f"Expected a Version type but got {type(other)}")
 
         # All major-0 versions should be incompatible with anything but itself
         if (0 == self.major == other.major) and (self[:4] != other[:4]):
             return False
 
@@ -986,40 +1026,42 @@
         pre: String | int | None = None,
         build: String | int | None = None,
     ):
         super().__init__(major, minor, patch)
         self.pre: str | None = None if pre is None else str(pre)
         self.build: str | None = None if build is None else str(build)
 
-    def bump_pre(self, token: str | None = "rc") -> VersionSemver:
+    def bump_pre(self, token: str | None = "rc") -> Self:
         """Raise the pre part of the version, return a new object but leave
         self untouched.
 
         :param token: defaults to ``'rc'``
-        :return: new :class:`Version` object with the raised pre part.
+        :returns: new :class:`Version` object with the raised pre part.
             The original object is not modified.
         """
         if self.pre is not None:
             pre = self.pre
         elif token == "":
             pre = "0"
         elif token is None:
             pre = "rc.0"
         else:
             pre = str(token) + ".0"
 
         pre = increment(pre)
         return self.__class__(self.major, self.minor, self.patch, pre)
 
-    def bump_build(self, token: str | None = "build") -> VersionSemver:
+    def bump_build(self, token: str | None = "build") -> Self:
         """Raise the build part of the version, return a new object but leave
         self untouched.
 
         :param token: defaults to ``'build'``
-        :return: new :class:`Version` object with the raised build part.
+
+        :rtype: Self
+        :returns: new :class:`Version` object with the raised build part.
             The original object is not modified.
         """
         cls = type(self)
         if self.build is not None:
             build = self.build
         elif token == "":
             build = "0"
@@ -1027,20 +1069,22 @@
             build = "build.0"
         else:
             build = str(token) + ".0"
 
         build = increment(build)
         return cls(self.major, self.minor, self.patch, self.pre, build)
 
-    def next_version(self, part: str, pre_token: str = "rc") -> VersionSemver:
+    def next_version(self, part: str, pre_token: str = "rc") -> Self:
         """Determines next version, preserving natural order.
 
         :param part: One of "major", "minor", "patch", or "pre"
         :param pre_token: prefix string of pre, defaults to 'rc'
-        :return: new object with the appropriate part raised
+
+        :rtype: Self
+        :returns: new object with the appropriate part raised
         """
         cls = type(self)
         # "build" is currently not used, that's why we use [:-1]
         valid_parts = cls.__slots__[:-1]
         if part not in valid_parts:
             raise ValueError(
                 f"Invalid part. Expected one of {valid_parts}, but got {part!r}"
@@ -1068,28 +1112,28 @@
         if self.build:
             version += f"+{self.build}"
         return version
 
     def __hash__(self) -> int:
         return hash(self.to_tuple()[:4])
 
-    def finalize_version(self) -> VersionSemver:
+    def finalize_version(self) -> Self:
         """Remove any pre-release and build metadata from the version.
 
-        :return: a new instance with the finalized version string.
+        :returns: a new instance with the finalized version string.
         """
         return self.__class__(self.major, self.minor, self.patch)
 
     @classmethod
     def parse(
-        cls: type[VersionSemver],
+        cls: type[Self],
         version: String,
         *,
         optional_minor_and_patch: bool = False,
-    ) -> VersionSemver:
+    ) -> Self:
         if isinstance(version, bytes):
             version = str(version, "utf-8", "strict")
         elif not isinstance(version, get_args(String)):
             raise TypeError(f"not expecting type '{type(version)}'")
 
         if optional_minor_and_patch:
             match = cls.regex_optional_minor_and_patch.match(version)
@@ -1110,15 +1154,15 @@
         _pre = self._extract_letter(self.pre) if self.pre else Inf
         return _release, _pre
 
     def compare(self, other: Comparable) -> int:
         """Compare self with this other.
 
         :param other: the second version
-        :return: The return value is negative if ver1 < ver2,
+        :returns: The return value is negative if ver1 < ver2,
             zero if ver1 == ver2 and strictly positive if ver1 > ver2
         """
         cls = type(self)
         if isinstance(other, get_args(String)):
             other = cls.parse(other)
         elif isinstance(other, dict):
             other = cls(**other)
@@ -1139,15 +1183,17 @@
         * both majors are equal and higher than 0. Same for both minors.
             Both pre-releases are equal, or
         * both majors are equal and higher than 0. The minor of b's
             minor version is higher than a's. Both pre-releases are equal.
 
         The algorithm does *not* check patches.
 
+        :param other: A version semver object that want to compatible check
         :rtype: bool
+        :returns: Return True if an other version semver object is compatible.
         """
         if not isinstance(other, VersionSemver):
             raise TypeError(f"Expected a Version type but got {type(other)}")
 
         # All major-0 versions should be incompatible with anything but itself
         if (0 == self.major == other.major) and (self[:4] != other[:4]):
             return False
```

### Comparing `fmtutil-1.0.5/fmtutil/cli.py` & `fmtutil-1.0.6/fmtutil/cli.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.5/fmtutil/exceptions.py` & `fmtutil-1.0.6/fmtutil/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,48 +29,44 @@
 
 
 class FormatterArgumentError(FormatterError):
     """Error raise for a wrong configuration argument.
 
     Examples:
         >>> FormatterArgumentError(
-        ...     argument='demo',
+        ...     arg='demo',
         ...     message='does not support',
         ... )
         FormatterArgumentError("with 'demo', does not support")
 
-    :param argument: An argument of this error that raise to client
-    :type argument: str | tuple
+    :param arg: An argument of this error that raise to client
+    :type arg: str | tuple
     :param message: A string message of this error
     :type message: str
     """
 
     def __init__(
         self,
-        argument: str | tuple[str, ...],
+        arg: str | tuple[str, ...],
         message: str,
     ) -> None:
         """Main Initialization that merge the argument and message input values
         with specific content message together like
 
             `__class__` with `argument`, `message`
         """
-        _argument: str
-        if isinstance(argument, tuple):
-            _last_arg: str = str(argument[-1])
-            _argument = (
-                (
-                    ", ".join(f"{x!r}" for x in argument[:-1])
-                    + f", and {_last_arg!r}"
-                )
-                if len(argument) > 1
+        if isinstance(arg, tuple):
+            _last_arg: str = str(arg[-1])
+            _argument: str = (
+                (", ".join(f"{x!r}" for x in arg[:-1]) + f", and {_last_arg!r}")
+                if len(arg) > 1
                 else f"{_last_arg!r}"
             )
         else:
-            _argument = f"{argument!r}"
+            _argument = f"{arg!r}"
         super().__init__(f"with {_argument}, {message}")
 
 
 class FormatterGroupValueError(FormatterValueError):
     """Error raise for value does not valid"""
```

### Comparing `fmtutil-1.0.5/fmtutil/formatter.py` & `fmtutil-1.0.6/fmtutil/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     NoReturn,
     TypedDict,
     Union,
     final,  # docs: https://github.com/python/mypy/issues/9953
 )
 
 from dateutil.relativedelta import relativedelta
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 from .__type import (
     DictStr,
     String,
     TupleInt,
 )
 from .__version import (
@@ -160,46 +160,46 @@
         return self.value < other.value
 
     @property
     def count(self) -> int:
         """Return a counting number of True value in the slot.
 
         :rtype: int
-        :return: A counting number of True value in the slot.
+        :returns: A counting number of True value in the slot.
         """
         return len(list(filter(lambda x: x is True, self.slot)))
 
     @property
     def value(self) -> int:
         """Return a sum of weighted value from a True value in any slot
         position.
 
         :rtype: int
-        :return: A sum of weighted value from a True value in any slot
+        :returns: A sum of weighted value from a True value in any slot
             position.
         """
         return sum(index * int(i) for index, i in enumerate(self.slot, start=1))
 
     def update(
         self,
         numbers: int | TupleInt | None = None,
         strict: bool = True,
-    ) -> SlotLevel:
+    ) -> Self:
         """Update boolean value in ``self.slot`` from False to True.
 
         :param numbers: updated numbers of this SlotLevel object.
         :type numbers: Union[int, TupleInt]
         :param strict: a strict flag for raise error when pass out of
             range numbers.
         :type strict: bool(=True)
 
         :raises FormatterValueError: if updated number does not exist in range.
 
-        :rtype: SlotLevel
-        :return: Self that was updated level
+        :rtype: Self
+        :returns: Self that was updated level
         """
         _numbers: Union[int, TupleInt] = numbers or (0,)
         for num in self.make_tuple(_numbers):
             if num == 0:
                 continue
             elif 0 <= (_num := (num - 1)) <= (self.level - 1):
                 self.slot[_num] = True
@@ -217,15 +217,15 @@
     ) -> bool:
         """Return True if boolean value in ``self.slot`` is all True.
 
         :param numbers: An index number values that want to check in slot.
         :type numbers: Union[int, TupleInt]
 
         :rtype: bool
-        :return: A True if all values in ``self.slot`` that match with
+        :returns: A True if all values in ``self.slot`` that match with
             index numbers are True.
         """
         _numbers: TupleInt = self.make_tuple(numbers)
         return all(
             (
                 self.slot[_n]
                 if (0 <= (_n := (n - 1)) <= (self.level - 1))
@@ -239,15 +239,15 @@
         """Return tuple of integer value that was created from input value
         parameter if it is not tuple.
 
         :param value: a tuple of integers or any integer
         :type value: Union[int, TupleInt]
 
         :rtype: TupleInt
-        :return: A tuple of integer value that was created from input.
+        :returns: A tuple of integer value that was created from input.
         """
         return (value,) if isinstance(value, int) else value
 
 
 @dataclass(frozen=True)
 class PriorityData:
     """Priority Data class.
@@ -269,14 +269,21 @@
     .. metaclass attributes::
         * __slots__: Tuple[str, ...]
             A tuple of necessary attribute for any subclass of Formatter class.
     """
 
     __slots__: tuple[str, ...] = ()
 
+    @abstractmethod
+    def __str__(self) -> str:
+        raise NotImplementedError(
+            "Please implement ``__str__`` build-in method for this "
+            "sub-formatter class"
+        )
+
 
 @total_ordering
 class Formatter(BaseFormatter):
     """Formatter object for inherit to any formatter subclass that define
     format and parse method. The base class will implement necessary
     properties and method for subclass that should implement or enhance such
     as `the cls.formatter()` method or the `cls.priorities` property.
@@ -295,18 +302,18 @@
         * base_level: int
             The maximum level of slot level of this instance.
         * Config: object
             A Configuration object that use for group and keep any config for
             this sub-formatter object.
 
     .. class-methods::
-        * from_value: Formatter
+        * from_value: Self
             An instance of formatter that was use ``cls.parse`` method from any
             correct string value with the ``cls.base_fmt`` value.
-        * parse: Formatter
+        * parse: Self
             An instance of formatter that parse from a bytes or string value by
             a format string or base format string if it None.
         * gen_format: str
             A format string value that was changed to the regular expression
             string value for comply with the `re` module to any string value.
         * regex: DictStr
             A dict of format string, and it's regular expression string
@@ -368,15 +375,15 @@
         """A Configuration object that use for group and keep any config for
         this sub-formatter object.
         """
 
         base_config_value: ClassVar[Any | None] = None
 
     def __init_subclass__(
-        cls: FormatterType,
+        cls: type[Self],
         /,
         level: int | None = None,
         fmt: str | None = None,
         **kwargs: Any,
     ) -> NoReturn:
         """Subclass Initialize method that will declare class variables if it
         set from class creation or direct override with that variables.
@@ -401,24 +408,24 @@
                 "sub-formatter class."
             )
 
     @classmethod
     def from_value(
         cls,
         value: Any,
-    ) -> Formatter:
+    ) -> Self:
         """Passer the value to this formatter that will pass this value to
         ``cls.formatter`` method and map with the base format string value
         before parse by ``cls.parse``.
 
         :param value: An any value that able to pass to `cls.formatter` method.
         :type value: Any
 
-        :rtype: Formatter
-        :return: An instance of formatter that was use ``cls.parse`` method
+        :rtype: Self
+        :returns: An instance of formatter that was use ``cls.parse`` method
             from any correct string value with the ``cls.base_fmt`` value.
         """
         fmt_filter = [
             (k, caller(v["value"]))
             for k, v in cls.formatter(value).items()
             if k in re.findall("(%[-+!*]?[A-Za-z])", cls.base_fmt)
         ]
@@ -428,15 +435,15 @@
     @classmethod
     def parse(
         cls,
         value: String,
         fmt: str | None = None,
         *,
         strict: bool = False,
-    ) -> Formatter:
+    ) -> Self:
         """Parse bytes or string value with its format to this formatter object.
         This method generates the value for itself data that can be formatted
         to another format string values.
 
         :param value: A bytes or string value that match with fmt.
         :type value: String
         :param fmt: a format value will use `cls.base_fmt` if it does not pass
@@ -446,16 +453,16 @@
         :type strict: bool(=False)
 
         :raises NotImplementedError: if fmt value parameter does not pass form
             input, or `cls.base_fmt` does not implement.
         :raises FormatterValueError: if value does not match with regular
             expression format string.
 
-        :rtype: Formatter
-        :return: An instance of formatter that parse from a bytes or string
+        :rtype: Self
+        :returns: An instance of formatter that parse from a bytes or string
             value by a format string or base format string if it None.
         """
         _fmt: str = fmt or cls.base_fmt
         _value: str = bytes2str(value)
 
         if not _fmt:
             raise NotImplementedError(
@@ -492,15 +499,15 @@
             string value.
         :type suffix: str | None(=None)
         :param alias: an alias boolean flag that will pass alias name if it
             true to the format string value.
         :type alias: bool
 
         :rtype: str
-        :return: A format string value that was changed to the regular
+        :returns: A format string value that was changed to the regular
             expression string value for comply with the `re` module to any
             string value.
         """
         _cache: dict[str, int] = defaultdict(int)
         _prefix: str = prefix or ""
         _suffix: str = suffix or ""
         regexes = cls.regex()
@@ -556,15 +563,15 @@
         ``cls.regex()`` value because the value does not change depend on the
         formatter class.
 
         :raises FormatterValueError: if any key of value in formatter mapping
             does not contain `regex` nor `cregex`.
 
         :rtype: DictStr
-        :return: A dict of format string, and it's regular expression string
+        :returns: A dict of format string, and it's regular expression string
             value that was generated from values of ``cls.formatter``.
 
             Example:
                 {
                     "%n": "(?P<normal>...)",
                     "%N": "(?P<normal_upper>...)",
                     ...
@@ -600,15 +607,15 @@
         return results
 
     def values(self, value: Any | None = None) -> DictStr:
         """Return a dict of format string, and it's string value that was passed
         an input value to `cls.formatter` method.
 
         :rtype: DictStr
-        :return: A dict of format string, and it's string value that was passed
+        :returns: A dict of format string, and it's string value that was passed
             an input value to `cls.formatter` method.
 
             Example:
                 {
                     "%n": "normal-value",
                     "%N": "NORMAL-UPPER-VALUE",
                     ...
@@ -626,15 +633,15 @@
         :param fmt: A format string value for mapping with formatter.
         :type fmt: str
 
         :raises KeyError: if it has any format pattern does not found in
             `cls.formatter`.
 
         :rtype: str
-        :return: A string value that was formatted from format string pattern.
+        :returns: A string value that was formatted from format string pattern.
         """
         _fmts: ReturnFormattersType = self.formatter(self.value)
         fmt = fmt.replace("%%", "[ESCAPE]")
         for _fmt_match in re.finditer(r"(%[-+!*]?[A-Za-z])", fmt):
             _fmt_str: str = _fmt_match.group()
             try:
                 _value: Union[FormatterCallable, str] = _fmts[_fmt_str]["value"]
@@ -777,15 +784,15 @@
 
     def validate(self) -> bool:
         """Validate method that will call after setup all attributes in
         initialize layer. This method should return with True. If it has some
         rule of validation fail, it will raise the ``FormatterValueError``.
 
         :rtype: bool
-        :return: True
+        :returns: True
         """
         return True
 
     def valid(self, value: str, fmt: str) -> bool:
         """Return a True value if the value from ``cls.parse`` of a string
         value, and a format string pattern is valid with ``self.value``.
 
@@ -808,16 +815,16 @@
         :param error: An error statement that raise from FormatterValueError
         :type error: str
 
         :raises FormatterValueError: If a slot of ``self.level`` with an input
             level and checker condition are Ture together.
 
         :rtype: bool
-        :return: A boolean value from slot of ``self.level`` with an input level
-            integer.
+        :returns: A boolean value from slot of ``self.level`` with an input
+            level integer.
         """
         if (sl := self.level.slot[(level - 1)]) and checker:
             raise FormatterValueError(
                 f"Parsing value does not valid with {error}."
             )
         return not sl
 
@@ -829,15 +836,15 @@
         values, and it will raise error if any duplication format name do not
         all equal.
 
         :param formats:
         :type formats: dict[str, Any] | None(=None)
 
         :rtype: Dict[str, Any]
-        :return: A formats value that validate with duplicate format string
+        :returns: A formats value that validate with duplicate format string
             values.
         """
         results: dict[str, Any] = {}
         _formats: dict[str, Any] = formats or {}
         for fmt in _formats:
             _fmt: str = fmt.split("__", maxsplit=1)[0]
             if _fmt not in results:
@@ -853,15 +860,15 @@
     @property
     @abstractmethod
     def priorities(self) -> ReturnPrioritiesType:
         """Return a priorities value that define by property of this formatter
         object.
 
         :rtype: ReturnPrioritiesType
-        :return: a priorities value that define by property of this formatter
+        :returns: a priorities value that define by property of this formatter
             object.
         """
         raise NotImplementedError(
             "Please implement ``priorities`` property for this sub-formatter "
             "class"
         )
 
@@ -871,28 +878,28 @@
         """Return a formatter value that define by property of this formatter
         object.
 
         :param value: An any value that want to generate with formatter.
         :type value: Any | None(=None)
 
         :rtype: ReturnFormattersType
-        :return: a formatter value that define by property of this formatter
+        :returns: a formatter value that define by property of this formatter
             object.
         """
         raise NotImplementedError(
             "Please implement ``formatter`` static method for this "
             "sub-formatter class"
         )
 
     def to_const(self) -> ConstantType:
         """Convert this formatter instance to Constant object that have class
         name with ``f'{self.__class__.__name__}Const'`` with ``self.values()``.
 
         :rtype: ConstantType
-        :return: A Constant object that create from constant of ``self.values``
+        :returns: A Constant object that create from constant of ``self.values``
             and has class name with ``f'{self.__class__.__name__}Const'`` with
             ``self.values()``.
         """
         return dict2const(
             self.values(),
             name=f"{self.__class__.__name__}Const",
             base_fmt=self.base_fmt,
@@ -904,15 +911,15 @@
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object.
 
         :param value: A value that want to prepare before passing to formatter.
         :type value: Any
 
         :rtype: Any
-        :return: A prepared value with defined logic.
+        :returns: A prepared value with defined logic.
         """
         raise NotImplementedError(
             "Please implement ``prepare_value`` static method for this "
             "sub-formatter class."
         )
 
     def __add__(self, other: Union[Formatter, Any]) -> Formatter:
@@ -936,16 +943,17 @@
 
     def __rsub__(self, other: Union[Formatter, Any]) -> Any:
         try:
             return other - self.value
         except (TypeError, FormatterValueError):
             return NotImplemented
 
-    def __format__(self, format_spec) -> str:
-        return self.format(format_spec)
+    def __format__(self, fmt_spec: str) -> str:
+        """Format a formatter object with any formatter setting value."""
+        return self.format(fmt_spec)
 
 
 class Serial(Formatter, fmt="%n"):
     """Serial formatter object that parse and format any serial (positive
     integer) value.
     """
 
@@ -971,15 +979,15 @@
     @property
     def priorities(
         self,
     ) -> ReturnPrioritiesType:
         """Return a priorities value that define by property of this formatter
         object.
 
-        Level Priority:
+        :priority: A priority mapping.
             [
                 0: default
                 1: number
             ]
 
         :rtype: ReturnPrioritiesType
         :returns: A properties of the serial formatter object.
@@ -1025,16 +1033,16 @@
             %c  : Normal with comma separate number
             %u  : Normal with underscore separate number
 
         :param serial: A serial value that pass to generate all format.
         :type serial: int | str | float | None(=None)
 
         :rtype: ReturnFormattersType
-        :return: A generated mapping values of all format string pattern of this
-            serial formatter object.
+        :returns: A generated mapping values of all format string pattern of
+            this serial formatter object.
         """
         _value: int = cls.prepare_value(serial)
         return {
             "%n": {
                 # "value": lambda: str(_value),
                 "value": partial(itself, str(_value)),
                 "regex": r"(?P<number>[0-9]*)",
@@ -1070,15 +1078,15 @@
             serial formatter.
         :type value: int | str | float | None
 
         :raises FormatterValueError: If an input value does not able cast to
             integer, or it's value less than 0.
 
         :rtype: int
-        :return: A prepared positive integer value.
+        :returns: A prepared positive integer value.
         """
         if value is None:
             return 0
         if not can_int(value) or ((prepare := int(float(value))) < 0):
             raise FormatterValueError(
                 f"Serial formatter does not support for value, {value!r}."
             )
@@ -1089,29 +1097,29 @@
         """Return a padding string value with zero by setting config
         ``Serial.Config.serial_max_padding`` value.
 
         :param value: A string value that want to pad with zero.
         :type value: str
 
         :rtype: str
-        :return: A padding string value with zero by setting config
+        :returns: A padding string value with zero by setting config
             ``Serial.Config.serial_max_padding`` value.
         """
         return value.rjust(cls.Config.serial_max_padding, "0") if value else ""
 
     @classmethod
     def to_binary(cls, value: str) -> str:
         """Return a binary number string value with limit of max zero padding
         by setting config ``Serial.Config.serial_max_binary`` value.
 
         :param value: A string value that want to convert to binary.
         :type value: str
 
         :rtype: str
-        :return: A binary number string value with limit of max zero padding
+        :returns: A binary number string value with limit of max zero padding
             by setting config ``Serial.Config.serial_max_binary`` value.
         """
         return (
             f"{int(value):0{str(cls.Config.serial_max_binary)}b}"
             if value
             else ""
         )
@@ -1192,30 +1200,30 @@
         )
 
     @property
     def iso_date(self) -> datetime:
         """Return Datetime that parsing from string of date with ISO format.
 
         :rtype: datetime
-        :return: A datetime that parsing from string of date with ISO format.
+        :returns: A datetime that parsing from string of date with ISO format.
         """
         return datetime.strptime(
             f"{self.year}-{self.month}-{self.day}", "%Y-%m-%d"
         )
 
     def validate(self) -> bool:
         """Validate method that validate all Datetime attributes in initialize
         layer.
 
         :raises FormatterValueError: If one of these rules was failed,
             * attribute ``self.week`` does not equal with value.
             * attribute ``self.locale`` does not equal with value.
 
         :rtype: bool
-        :return: True if all validation rules was passed.
+        :returns: True if all validation rules was passed.
         """
         if self.week != (w := self.value.strftime("%w")):
             raise FormatterValueError(
                 f"Week that was parsed does not equal with standard datetime, "
                 f"this weekday should be {WEEKS_FULL[w]}."
             )
         if self.locale != (p := self.value.strftime("%p")):
@@ -1457,16 +1465,16 @@
         **  %x  : Local version of date (%Y/%m/%d)
         **  %X  : Local version of time (%H:%M:%S)
 
         :param dt: A datetime value that pass to generate all format.
         :type dt: str | datetime | date | None(=None)
 
         :rtype: ReturnFormattersType
-        :return: A generated mapping values of all format string pattern of this
-            datetime formatter object.
+        :returns: A generated mapping values of all format string pattern of
+            this datetime formatter object.
         """
         _dt: datetime = cls.prepare_value(dt)
         return {
             "%n": {
                 "value": partial(_dt.strftime, "%Y%m%d_%H%M%S"),
                 "cregex": "%Y%m%d_%H%M%S",
             },
@@ -1604,15 +1612,15 @@
             datetime formatter.
         :type value: str | datetime | date | None
 
         :raises FormatterValueError: If an input value does be
             ``datetime.datetime`` or ``datetime.date``.
 
         :rtype: datetime
-        :return: A prepared datetime value.
+        :returns: A prepared datetime value.
         """
 
         if value is None:
             return datetime.now()
         if not isinstance(
             value,
             (
@@ -1635,15 +1643,15 @@
     def _from_day_year(self, value: str) -> str:
         """Return a validated day string value from date of year string value.
 
         :param value: A format string value that pass from initialize.
         :type value: str
 
         :rtype: str
-        :return: A validated day string value from date of year string value.
+        :returns: A validated day string value from date of year string value.
         """
         _this_year: datetime = datetime.strptime(self.year, "%Y") + timedelta(
             days=(int(value) - 1)
         )
         _month: str = _this_year.strftime("%m")
         if self._sub_validate(
             level=9,
@@ -1657,16 +1665,16 @@
         """Return a validated week string value from week year number with
         Monday string value.
 
         :param value: A format string value that pass from initialize.
         :type value: str
 
         :rtype: str
-        :return: A validated week string value from week year number with Monday
-            string value.
+        :returns: A validated week string value from week year number with
+            Monday string value.
         """
         _this_year: datetime = datetime.strptime(
             f"{self.year}-W{value}-{self.week}", "%Y-W%W-%w"
         )
         _month: str = _this_year.strftime("%m")
         if self._sub_validate(
             level=9,
@@ -1688,16 +1696,16 @@
         """Return a validated week string value from week year number with
         Sunday string value.
 
         :param value: A format string value that pass from initialize.
         :type value: str
 
         :rtype: str
-        :return: A validated week string value from week year number with Sunday
-            string value.
+        :returns: A validated week string value from week year number with
+            Sunday string value.
         """
         _this_year: datetime = datetime.strptime(
             f"{self.year}-W{value}-{self.week}", "%Y-W%U-%w"
         )
         _month: str = _this_year.strftime("%m")
         if self._sub_validate(
             level=9,
@@ -1719,57 +1727,57 @@
         """Return a validated hour string value that map with ``self.locale``
         attribute value.
 
         :param value: The hour string value.
         :type value: str
 
         :rtype: str
-        :return: A validated hour string value that map with ``self.locale``
+        :returns: A validated hour string value that map with ``self.locale``
             attribute value.
         """
         if self.level.slot[0] and self.locale and self.locale == "PM":
             return str(int(value) + 12).rjust(2, "0")
         return value.rjust(2, "0")
 
     def _default_locale(self) -> str:
         """Return a default string locale value that generate depend on
         ``self.hour`` attribute value.
 
         :rtype: str
-        :return: A default string locale value that generate depend on
+        :returns: A default string locale value that generate depend on
             ``self.hour`` attribute value.
         """
         return "PM" if int(self.hour) >= 12 else "AM"
 
     @staticmethod
     def remove_pad_dt(_dt: datetime, fmt: str) -> str:
         """Return a padded datetime string value that was formatted.
 
         :param _dt: A datetime instance that want to convert to string format.
         :type _dt: datetime
         :param fmt: A format string value of datetime package.
         :type: str
 
         :rtype: str
-        :return: A padded datetime string value that was formatted.
+        :returns: A padded datetime string value that was formatted.
         """
         return str(remove_pad(_dt.strftime(fmt)))
 
     @staticmethod
     def week_year_mon_to_isoweek(year: int, week: int) -> datetime:
         """Return a converted week numbers with ISO week number that was passed
         with Monday format.
 
         :param year: A year number.
         :type year: int
         :param week: A week number that count by monday.
         :type week: int
 
         :rtype: datetime
-        :return: A converted datetime value
+        :returns: A converted datetime value
         """
         dt: datetime = datetime.strptime(f"{year}-{week}-1", "%Y-%W-%w")
         if date(year, 1, 4).isoweekday() > 4:
             dt -= timedelta(days=7)
         return dt
 
     def __add__(self, other: Any) -> Formatter:
@@ -1983,16 +1991,16 @@
             %l  : local release
             %-l : local release number
 
         :param version: A version value that pass to generate all format.
         :type version: str | __version.VerPackage | None(=None)
 
         :rtype: ReturnFormattersType
-        :return: A generated mapping values of all format string pattern of this
-            version formatter object.
+        :returns: A generated mapping values of all format string pattern of
+            this version formatter object.
         """
         _version: VerPackage = cls.prepare_value(version)
         return {
             "%f": {
                 "value": partial(
                     itself,
                     f"{_version.major}_{_version.minor}_{_version.patch}",
@@ -2069,15 +2077,15 @@
             version formatter.
         :type value: str |  __version.VersionPackage | None
 
         :raises FormatterValueError: If an input value does be
             ``__version.VersionPackage``
 
         :rtype: __version.VersionPackage
-        :return: A prepared version value.
+        :returns: A prepared version value.
         """
         if value is None:
             return VerPackage.parse("0.0.1")
         if not isinstance(
             value,
             (
                 str,
@@ -2096,15 +2104,15 @@
         """Return a replaced string value to standard prefix of pre- and post-
         format version string.
 
         :param value: A pre- or post- format version string.
         :type value: str
 
         :rtype: str
-        :return: A replaced string value to standard prefix of pre- and post-
+        :returns: A replaced string value to standard prefix of pre- and post-
             format version string.
         """
         for rep, matches in (
             (
                 "a",
                 [
                     "alpha",
@@ -2206,15 +2214,15 @@
 
         :raises FormatterValueError: If one of these rules was failed,
             * attribute ``self.flats`` does not equal with ``self.shorts``.
             * attribute ``self.flats`` does not equal with ``self.vowels``.
             * attribute ``self.vowels`` does not equal with ``self.shorts``.
 
         :rtype: bool
-        :return: True if all validation rules was passed.
+        :returns: True if all validation rules was passed.
         """
         # Validate flat and short-name
         if self.level.checker((3, 2)):
             if self.__validate_word_with_short(self.flats[0], self.shorts):
                 raise FormatterValueError(
                     f"Flat and Shortname that were parsed are not equal, "
                     f"{self.flats[0]} and {''.join(self.shorts)}."
@@ -2254,15 +2262,15 @@
 
         :param word: A word string that want to validate.
         :type word: str
         :param shorts: A list of shortname.
         :type shorts: List[str]
 
         :rtype: bool
-        :return: True if validation process of a word with list of shortname
+        :returns: True if validation process of a word with list of shortname
             Private static-method be correct.
         """
         idx: int = 0
         for s in shorts:
             if s not in word[idx:]:
                 return True
             idx += word[idx:].index(s) + 1
@@ -2278,15 +2286,15 @@
 
         :param word: A word string value.
         :type word: str
         :param shorts: A list of first char of naming.
         :type shorts: List[str]
 
         :rtype: List[str]
-        :return: A list of word that was extracted from word by list of
+        :returns: A list of word that was extracted from word by list of
             shortnames.
         """
         idx: int = 0
         rs: list[int] = []
         for s in shorts:
             idx += word[idx:].index(s)
             rs.append(idx)
@@ -2436,16 +2444,16 @@
         .. refs::
             * https://gist.github.com/SuppieRK/a6fb471cf600271230c8c7e532bdae4b
 
         :param nm: A naming value that pass to generate all format.
         :type nm: str | list[str] | None(=None)
 
         :rtype: ReturnFormattersType
-        :return: A generated mapping values of all format string pattern of this
-            naming formatter object.
+        :returns: A generated mapping values of all format string pattern of
+            this naming formatter object.
         """
         _value: list[str] = cls.prepare_value(nm)
         return {
             "%n": {
                 "value": partial(cls.__join_with, " ", _value),
                 "cregex": "%l",
             },
@@ -2594,15 +2602,15 @@
         :param value: A value that want to prepare before passing to this
             naming formatter.
         :type value: str | list[str] | None
 
         :raises FormatterValueError: If an input value does be list of str.
 
         :rtype: List[str]
-        :return: A prepared naming value.
+        :returns: A prepared naming value.
         """
         if value is None:
             return [""]
         if isinstance(value, str):
             return cls.__remove_special_char(value)
         elif not isinstance(value, list) or any(
             not isinstance(v, str) for v in value
@@ -2618,15 +2626,15 @@
         :param value: A format string value that pass from initialize.
         :type value: str
 
         :raises FormatterValueError: If flat string from ``self.strings`` does
             not equal with an input value.
 
         :rtype: List[str]
-        :return: a validated flats value.
+        :returns: a validated flats value.
         """
         v: list[str] = [value]
         if self.level.checker(5) and (_s := ["".join(self.strings)]) != v:
             raise FormatterValueError(
                 f"Parsing value does not valid with flat from "
                 f"strings: {_s} and flats: {v}."
             )
@@ -2638,15 +2646,15 @@
         :param value: A format string value that pass from initialize.
         :type value: str
 
         :raises FormatterValueError: If short string from ``self.strings`` does
             not equal with an input value.
 
         :rtype: List[str]
-        :return: a validated shorts value.
+        :returns: a validated shorts value.
         """
         v: list[str] = list(value)
         if self.level.checker(5) and (_s := [s[0] for s in self.strings]) != v:
             raise FormatterValueError(
                 f"Parsing value does not valid with short from "
                 f"strings: {_s} and shorts: {v}."
             )
@@ -2658,15 +2666,15 @@
         :param value: A format string value that pass from initialize.
         :type value: str
 
         :raises FormatterValueError: If vowel string from ``self.strings`` does
             not equal with an input value.
 
         :rtype: List[str]
-        :return: A validated vowels value.
+        :returns: A validated vowels value.
         """
         v: list[str] = [value]
         if (
             self.level.checker(5)
             and (_s := [re.sub(r"[aeiou]", "", "".join(self.strings))]) != v
         ):
             raise FormatterValueError(
@@ -2682,15 +2690,15 @@
         """Return a default function that pass logic to ``self.strings`` if
         it was set from initialization.
 
         :param logic: A logic function receive a ``self.strings`` list.
         :type logic: Callable[[List[str]], str]
 
         :rtype: Callable[[], List[str]]
-        :return: A default function that pass logic to ``self.strings`` if
+        :returns: A default function that pass logic to ``self.strings`` if
             it was set from initialization.
         """
 
         def sub_caller() -> list[str]:
             if not self.level.slot[4]:
                 return []
             return (
@@ -2704,29 +2712,29 @@
         """Return a string value with pascal case that reference by
         `inflection`.
 
         :param snake_case: A word with the snake case string.
         :type snake_case: str
 
         :rtype: str
-        :return: A string value with pascal case that reference by
+        :returns: A string value with pascal case that reference by
             `inflection`.
         """
         return re.sub(r"(?:^|_)(.)", lambda m: m.group(1).upper(), snake_case)
 
     @classmethod
     def camel_case(cls, snake_case: str) -> str:
         """Return a string value with camel case with lower case first
         letter.
 
         :param snake_case: A word with the snake case string.
         :type snake_case: str
 
         :rtype: str
-        :return: A string value with camel case with lower case first
+        :returns: A string value with camel case with lower case first
             letter.
         """
         return (
             (snake_case[0].lower() + cls.pascal_case(snake_case)[1:])
             if snake_case
             else ""
         )
@@ -2744,43 +2752,43 @@
         :type by: str
         :param values: A list of word that want to join with.
         :type values: List[str]
         :param func: A function that want to prepare before join.
         :type func: Callable[[str], str] | None(=None)
 
         :rtype: str
-        :return: A string value that join with any separate string after
+        :returns: A string value that join with any separate string after
             prepare with an input function if it set.
         """
         return by.join(map(func, values)) if func else by.join(values)
 
     @staticmethod
     def __remove_special_char(value: str) -> list[str]:
         """Return a list of word that split from an input value string
         before remove special character.
 
         :param value: A string value that want to prepare.
         :type value: str
 
         :rtype: List[str]
-        :return: A list of word that split from an input value string
+        :returns: A list of word that split from an input value string
             before remove special character.
         """
         result: str = re.sub(r"[^\-.\w\s]+", "", value)
         return re.sub(r"[\-._\s]", " ", result).strip().split()
 
     @staticmethod
     def __split_pascal_case(value: str) -> list[str]:
         """Return a list of word that prepare from the Pascal case.
 
         :param value: A pascal value string that want to prepare.
         :type value: str
 
         :rtype: str
-        :return: A list of word that prepare from the Pascal case.
+        :returns: A list of word that prepare from the Pascal case.
         """
         return (
             "".join([f" {c.lower()}" if c.isupper() else c for c in value])
             .strip()
             .split()
         )
 
@@ -2845,15 +2853,15 @@
         layer.
 
         :raises FormatterValueError: If one of these rules was failed,
             * attribute ``self.week`` does not equal with value.
             * attribute ``self.locale`` does not equal with value.
 
         :rtype: bool
-        :return: True if all validation rules was passed.
+        :returns: True if all validation rules was passed.
         """
         if (b := self.byte2bit(self.byte)) != self.bit:
             raise FormatterValueError(
                 f"Byte that was parsed does not equal with bit, receive {b} bit"
                 f"(byte to bit) but get "
                 f"{self.bit:.{self.Config.storage_rounding:02d}f} bit from "
                 f"parsing."
@@ -2941,16 +2949,16 @@
             %Z  : Zetta-Byte format
             %Y  : Yotta-Byte format
 
         :param storage: A storage value that pass to generate all format.
         :type storage: int | None
 
         :rtype: ReturnFormattersType
-        :return: A generated mapping values of all format string pattern of this
-            storage formatter object.
+        :returns: A generated mapping values of all format string pattern of
+            this storage formatter object.
         """
         size: Decimal = Storage.prepare_value(storage)
         return {
             "%b": {
                 "value": partial(itself, str(size)),
                 "regex": r"(?P<bit>[0-9]*.?[0-9]*)",
             },
@@ -3005,15 +3013,15 @@
             storage formatter.
         :type value: int | float | Decimal | str | None
 
         :raises FormatterValueError: If an input value does not able cast to
             integer, or it's value less than 0.
 
         :rtype: decimal.Decimal
-        :return: A prepared positive decimal value.
+        :returns: A prepared positive decimal value.
         """
         if value is None:
             return Decimal("0")
         if not can_float(value) or (Decimal(value) < 0):
             raise FormatterValueError(
                 f"Storage formatter does not support for value, {value!r}."
             )
@@ -3024,15 +3032,15 @@
     def round_up(cls, value: Decimal) -> Decimal:
         """Return a rounded value that use ``cls.Config.storage_rounding``.
 
         :param value: A decimal value that want to round up.
         :type value: decimal.Decimal
 
         :rtype: decimal.Decimal
-        :return: A rounded value that use ``cls.Config.storage_rounding``.
+        :returns: A rounded value that use ``cls.Config.storage_rounding``.
         """
         return round(value, cls.Config.storage_rounding)
 
     def __default_from_byte(self) -> Decimal:
         """Return default value that calculate from the byte value."""
         return Decimal(self.byte or "0") * 8
 
@@ -3062,15 +3070,15 @@
 
             >>> Storage.bit2byte('150', 'B')
             19B
             >>> Storage.bit2byte('150', 'B', suffix=False)
             19
 
         :rtype: str
-        :return: The bit to byte value with string type that depend on an input
+        :returns: The bit to byte value with string type that depend on an input
             order value.
         """
         p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
         return f"{(cls.round_up((value / 8) / p))}{order if suffix else ''}"
 
     @classmethod
     def search_order(cls, value: str) -> StorageSearchOrder:
@@ -3104,15 +3112,15 @@
         :type order: str | None(=None)
 
         Examples:
 
             >>> Storage.str2byte('12MB', 'MB')
 
         :rtype: decimal.Decimal
-        :return: A converted byte value that depend on an input order value.
+        :returns: A converted byte value that depend on an input order value.
         """
         if order is None:
             searching: StorageSearchOrder = cls.search_order(value)
             value = searching["value"]
             order = searching["order"]
         p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
         return cls.round_up(Decimal(value.replace(order, "")) * p)
@@ -3129,15 +3137,15 @@
 
         Examples:
 
             >>> Storage.byte2bit(19.000)
             152.000
 
         :rtype: decimal.Decimal
-        :return: The byte to bit value with string type that depend on an input
+        :returns: The byte to bit value with string type that depend on an input
             order value.
         """
         p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
         return cls.round_up(
             (
                 Decimal(value.replace(order, ""))
                 if isinstance(value, str)
@@ -3200,30 +3208,30 @@
     @classmethod
     def parse(
         cls,
         value: String,
         fmt: str | None = None,
         *,
         strict: bool = False,
-    ) -> Formatter:
+    ) -> Self:
         """Parse bytes or string value with its format to this formatter object.
         This method generates the value for itself data that can be formatted
         to another format string values.
 
         :param value: A bytes or string value that match with fmt.
         :type value: String
         :param fmt: a format value.
         :type fmt: str | None(=None)
         :param strict: A flag strict validate that pass to ``set_strict_mode``.
         :type strict: bool(=False)
 
         :raises NotImplementedError: If an input fmt value does not pass.
 
-        :rtype: Formatter
-        :return: An instance of formatter that parse from a bytes or string
+        :rtype: Self
+        :returns: An instance of formatter that parse from a bytes or string
             value by a format string or base format string if it None.
         """
         if fmt is None:
             raise NotImplementedError(
                 "The Constant class does not support for default format string "
                 "when parsing with this unknown format value."
             )
@@ -3263,15 +3271,15 @@
 
     @property
     def value(self) -> list[str]:
         """Return a list of string value that list from ``cls.__slots__``
         attributes.
 
         :rtype: List[str]
-        :return: A list of string value that list from ``cls.__slots__``
+        :returns: A list of string value that list from ``cls.__slots__``
             attributes.
         """
         return self._constant
 
     @property
     def string(self) -> str:
         """Return string value that was joined with ``|`` value from string
@@ -3281,15 +3289,15 @@
 
     @property
     def priorities(self) -> ReturnPrioritiesType:
         """Return a priorities value that define by property of this formatter
         object.
 
         :rtype: ReturnPrioritiesType
-        :return: a priorities value that define by property of this formatter
+        :returns: a priorities value that define by property of this formatter
             object.
         """
         raise NotImplementedError(
             "Please implement ``priorities`` property for this sub-constant "
             "formatter class"
         )
 
@@ -3298,15 +3306,15 @@
         """Return a formatter value that define by property of this formatter
         object.
 
         :param value: An any value that want to generate with formatter.
         :type value: str | None(=None)
 
         :rtype: ReturnFormattersType
-        :return: a formatter value that define by property of this formatter
+        :returns: a formatter value that define by property of this formatter
             object.
         """
         raise NotImplementedError(
             "Please implement ``formatter`` staticmethod for this sub-constant "
             "formatter class"
         )
 
@@ -3315,15 +3323,15 @@
         """Prepare value before passing to convert logic in the formatter
         method that define by property of this formatter object.
 
         :param value: A value that want to prepare before passing to formatter.
         :type value: Any
 
         :rtype: Any
-        :return: An itself input value.
+        :returns: An itself input value.
         """
         return value
 
     def __add__(self, other: Any):  # type: ignore # no cov
         return NotImplemented
 
     def __sub__(self, other: Any):  # type: ignore # no cov
@@ -3362,15 +3370,16 @@
     :type fmt: DictStr
     :param name: A custom class name that want to rename.
     :type name: str
     :param base_fmt: A base format string value.
     :type base_fmt: str | None(=None)
 
     :rtype: ConstantType
-    :return: A constant object that construct from an input fmt and name values.
+    :returns: A constant object that construct from an input fmt and name
+        values.
     """
     _base_fmt: str = base_fmt or "".join(fmt.keys())
 
     class CustomConstant(Constant):
         """Dynamic Custom Constant object that will change the class name to an
         input name from constructor function.
         """
@@ -3400,15 +3409,15 @@
             formatter object. Generate formatter that support mapping formatter
             with an input dict in fmt value.
 
             :param v: A constant value that pass to generate all format.
             :type v: str | None(=None)
 
             :rtype: ReturnFormattersType
-            :return: A generated mapping values of all format string pattern of
+            :returns: A generated mapping values of all format string pattern of
                 this constant formatter object.
             """
             # It does not use an input value.
             _ = CustomConstant.prepare_value(v)
             return {
                 f: {
                     "regex": f"(?P<{convert_fmt_str(f)}>{fmt[f]})",
@@ -3443,15 +3452,15 @@
         def __search_fmt(self, value: str) -> str:
             """Return the first format that equal to an input string value.
 
             :param value:
             :type value: str
 
             :rtype: str
-            :return: The first format that equal to an input string value.
+            :returns: The first format that equal to an input string value.
             """
             return [k for k, v in iter(self.values().items()) if v == value][0]
 
     CustomConstant.__name__ = name
     return CustomConstant
 
 
@@ -3476,15 +3485,16 @@
 
     :raises FormatterArgumentError: If an input formatter was passed together
         with an input fmt value.
     :raises FormatterArgumentError: If an input name does not set for construct
         a constant object.
 
     :rtype: ConstantType
-    :return: A constant object that construct from an input fmt and name values.
+    :returns: A constant object that construct from an input fmt and name
+        values.
     """
     base_fmt: str | None = None
     _fmt: DictStr
     if formatter is None:
         if fmt is None or not inspect.isclass(fmt):
             raise FormatterArgumentError(
                 "formatter",
@@ -3563,15 +3573,15 @@
 ]
 
 Comparator: TypeAlias = Callable[["FormatterGroup", "FormatterGroup"], bool]
 
 
 def comparison(operator: Comparator) -> Comparator:
     @wraps(operator)
-    def wrapper(self: FormatterGroup, other) -> bool:
+    def wrapper(self: FormatterGroup, other: Any) -> bool:
         if not (
             issubclass(other.__class__, FormatterGroup)
             and (self.__class__.__name__ == other.__class__.__name__)
         ):
             return NotImplemented
         return operator(self, other)
 
@@ -3597,38 +3607,38 @@
         * base_groups: BaseGroupsType
             The base group of naming and Formatter class.
 
     .. class-method::
         * __parse: ReturnParseType
             A mapping of fmt, value, and props keys that passing from searching
             step with `re` module.
-        * parse: FormatterGroup
+        * parse: Self
             An instance of formatter group that parse from a bytes or string
             value by a format string.
         * gen_format: Tuple[str, ReturnGroupGenFormatType]
             A tuple of group naming and format string value that change format
             string to regular expression string for complied to the `re` module.
-        * from_formatter: FormatterGroup
+        * from_formatter: Self
             An instance of formatter group that was pass formats value directly
             to its formatter object.
-        * from_value: FormatterGroup
+        * from_value: Self
             An instance of formatter group that was use ``cls.from_value``
             method from any formatter object and its value.
 
     .. attributes::
         * groups: GroupsType
             A dict of group naming and Formatter instance.
 
     .. methods::
         * __construct_groups: [str, Union[DictStr, Formatter, Any]] -> Formatter
             A Formatter instance.
         * format: [str] -> str
             A string value that was formatted and filled by an input format
             string pattern.
-        * adjust: [Dict[str, Any]] -> FormatterGroup
+        * adjust: [Dict[str, Any]] -> Self
             Adjust any formatter instance in ``self.groups`` of this formatter
             group.
         * to_const: list[str] | None -> FormatterGroupType
             A FormatterGroup object that create from constant of ``self.groups``
             values.
 
     .. seealso::
@@ -3651,27 +3661,27 @@
                 "sub-formatter group class."
             )
 
     @classmethod
     def from_formats(
         cls,
         formats: dict[str, DictStr],
-    ) -> FormatterGroup:
+    ) -> Self:
         """Passer the formats to this formatter group directly to its formatter
         object.
 
         :param formats: A dict of group naming and formats of its group that
             pass directly to formatter object.
         :type formats: Dict[str, DictStr]
 
         :raises FormatterGroupValueError: If any group naming from an input
             formats does not exist in ``cls.base_groups`` value.
 
-        :rtype: FormatterGroup
-        :return: An instance of formatter group that was pass formats value
+        :rtype: Self
+        :returns: An instance of formatter group that was pass formats value
             directly to its formatter object.
         """
         rs: GroupsType = {}
         for k, v in formats.items():
             if k not in cls.base_groups:
                 raise FormatterGroupValueError(
                     f"{cls.__name__} does not support for this group name, "
@@ -3680,27 +3690,27 @@
             rs[k] = cls.base_groups[k](v)
         return cls(formats=rs, ignore_construct=True)
 
     @classmethod
     def from_value(
         cls,
         values: dict[str, Any],
-    ) -> FormatterGroup:
+    ) -> Self:
         """Passer the value to this formatter group that will pass this value to
         ``cls.from_value`` method of its formatter.
 
         :param values: A dict of group naming and value of its group that pass
             to `cls.form_value` of formatter object.
         :type values: Dict[str, Any]
 
         :raises FormatterGroupValueError: If any group naming from an input
             formats does not exist in ``cls.base_groups`` value.
 
-        :rtype: FormatterGroup
-        :return: An instance of formatter group that was use ``cls.from_value``
+        :rtype: Self
+        :returns: An instance of formatter group that was use ``cls.from_value``
             method from any formatter object and its value.
         """
         rs: GroupsType = {}
         for k, v in values.items():
             if k not in cls.base_groups:
                 raise FormatterGroupValueError(
                     f"{cls.__name__} does not support for this group name, "
@@ -3710,27 +3720,27 @@
         return cls(formats=rs, ignore_construct=True)
 
     @classmethod
     def parse(
         cls,
         value: String,
         fmt: str,
-    ) -> FormatterGroup:
+    ) -> Self:
         """Parse bytes or string value with its format to this formatter object.
         This method generates the value for itself data that can be formatted
         to another format string values.
 
         :param value: A bytes or string value that match with fmt.
         :type value: String
         :param fmt: a format string value that must have the formatter group
             pattern like `{group-name:fmt-str}`.
         :type fmt: str
 
-        :rtype: FormatterGroup
-        :return: An instance of formatter group that parse from a bytes or
+        :rtype: Self
+        :returns: An instance of formatter group that parse from a bytes or
             string value by a format string.
         """
         parser_rs: ReturnParseType = cls.__parse(bytes2str(value), fmt)
         rs: dict[str, DictStr] = defaultdict(dict)
         for g in parser_rs:
             rs[g.split("__")[0]] |= parser_rs[g]["props"]
         return cls(formats=rs)
@@ -3750,15 +3760,15 @@
             pattern like `{group-name:fmt-str}`.
         :type fmt: str
 
         :raises FormatterGroupArgumentError: If value does not match with format
             pattern value from ``cls.gen_format``.
 
         :rtype: ReturnParseType
-        :return: A mapping of fmt, value, and props keys that passing
+        :returns: A mapping of fmt, value, and props keys that passing
             from searching step with `re` module.
         """
         _fmt, _fmt_getter = cls.gen_format(fmt=fmt)
         if not (_search := re.search(rf"^{_fmt}$", value)):
             raise FormatterGroupArgumentError(
                 "format",
                 f"{value!r} does not match with the format: '^{_fmt}$'",
@@ -3786,15 +3796,15 @@
         format name to regular expression value that able to search with any
         input value string.
 
         :param fmt: a format string value pass from input argument.
         :type fmt: str
 
         :rtype: Tuple[str, ReturnGroupGenFormatType]
-        :return: A tuple of group naming and format string value that change
+        :returns: A tuple of group naming and format string value that change
             format string to regular expression string for complied to the `re`
             module.
         """
         fmt_getter: ReturnGroupGenFormatType = {}
         for group, formatter in cls.base_groups.items():
             for _index, fmt_match in enumerate(
                 re.finditer(
@@ -3832,15 +3842,15 @@
 
         :raises FormatterGroupValueError: If group naming on format string
             pattern does not exist in ``self.base_groups``.
         :raises FormatterGroupArgumentError: If any group of formatter raise
             FormatterKeyError from ``format`` method.
 
         :rtype: str
-        :return: A string value that was filled and formatted by an input
+        :returns: A string value that was filled and formatted by an input
             format pattern.
         """
         for fmt_match in re.finditer(
             r"(?P<found>{(?P<group>\w+):?(?P<format>[^{}]+)?})", fmt
         ):
             # Format Dict Example::
             # {
@@ -3906,15 +3916,15 @@
 
         :param group: A group naming value.
         :type group: str
         :param v: A value of this group naming that want to dynamic construct.
         :type v: Union[DictStr, Formatter, Any]
 
         :rtype: Formatter
-        :return: A Formatter instance.
+        :returns: A Formatter instance.
         """
         if isinstance(v, Formatter):
             return v
         elif isinstance(v, dict):
             return self.base_groups[group](v)
         return self.base_groups[group].from_value(v)
 
@@ -3934,46 +3944,46 @@
             f"fmt={'_'.join(fmts)!r})>"
         )
 
     def __str__(self) -> str:
         return ", ".join(v.string for v in self.groups.values())
 
     @comparison
-    def __eq__(self, other: FormatterGroup) -> bool:
+    def __eq__(self, other: Self) -> bool:
         return all(self.groups[g] == other.groups[g] for g in self.base_groups)
 
     @comparison
-    def __gt__(self, other: FormatterGroup) -> bool:
+    def __gt__(self, other: Self) -> bool:
         return any(
             self.groups[g].__gt__(other.groups[g]) for g in self.base_groups
         ) and all(
             not self.groups[g].__lt__(other.groups[g]) for g in self.base_groups
         )
 
     @comparison
-    def __lt__(self, other: FormatterGroup) -> bool:
+    def __lt__(self, other: Self) -> bool:
         return any(
             self.groups[g].__lt__(other.groups[g]) for g in self.base_groups
         ) and all(
             not self.groups[g].__gt__(other.groups[g]) for g in self.base_groups
         )
 
-    def adjust(self, values: dict[str, Any]) -> FormatterGroup:  # no cov
+    def adjust(self, values: dict[str, Any]) -> Self:  # no cov
         """Adjust value to any formatter instance in ``self.groups`` of this
         formatter group.
 
         :param values: A mapping of group and its value that able to adding
             to origin value.
         :type values: Dict[str, Any]
 
         :raises FormatterGroupValueError: If any key in an input value does not
             exist in ``self.base_groups``.
 
         :rtype: FormatterGroup
-        :return: Self that was adjusted the value.
+        :returns: Self that was adjusted the value.
         """
         _keys: list[str] = [
             f"{k!r}" for k in values if k not in self.base_groups
         ]
         if _keys:
             raise FormatterGroupValueError(
                 f"Key of values, {', '.join(_keys)}, does not support for this "
@@ -3988,15 +3998,15 @@
     def to_const(
         self,
         included: list[str] | None = None,
     ) -> FormatterGroupType:  # no cov
         """Convert this formatter group instance to constant group object.
 
         :rtype: FormatterGroupType
-        :return: A FormatterGroup object that create from constant of
+        :returns: A FormatterGroup object that create from constant of
             ``self.groups`` values.
         """
         _inc: list[str] = included or list(self.groups.keys())
         if any(i not in self.base_groups for i in _inc):
             raise FormatterGroupArgumentError(
                 "included",
                 (
@@ -4021,15 +4031,15 @@
 
     :raises FormatterGroupValueError: If any value in an input group does not
         be subclassed of Formatter instance.
     :raises FormatterGroupArgumentError: If any value in an input group does not
         be objected that mean this value is any instance.
 
     :rtype: FormatterGroupType
-    :return: A FormatterGroup class that construct from an input group value.
+    :returns: A FormatterGroup class that construct from an input group value.
     """
     # Validate argument group that should contain ``FormatterType``
     for _ in group.values():
         try:
             if not issubclass(_, Formatter):
                 raise FormatterGroupValueError(
                     f"Make group constructor function want group with type, "
```

### Comparing `fmtutil-1.0.5/fmtutil/utils.py` & `fmtutil-1.0.6/fmtutil/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from decimal import Decimal
 from typing import (
     Any,
     Callable,
     get_args,
 )
 
-from .__type import String
+try:
+    from .__type import String
+except ImportError:
+    from __type import String
+
 
 FMT_STR_MAP: dict[str, str] = {
     "-": "minus",
     "+": "plus",
     "!": "exclamation",
     "*": "asterisk",
 }
@@ -46,20 +50,20 @@
     "Y": "yankee",
     "Z": "zulu",
 }
 
 concat: Callable[[list[str] | Iterable[str]], str] = "".join
 
 
-def itself(x: Any = None) -> Any:
+def itself(x: Any = None) -> Any:  # pragma: no cover.
     """Return itself value"""
     return x
 
 
-def default(value: Any) -> Callable[[], Any]:
+def default(value: Any) -> Callable[[], Any]:  # pragma: no cover.
     """Return wrapper function of value"""
     return lambda: value
 
 
 def caller(func: Callable[[], Any] | Any) -> Any:
     """Call function if it was callable
 
@@ -168,7 +172,35 @@
     """Convert float to decimal with default precision value."""
     return Decimal(value).quantize(Decimal(10) ** -precision)
 
 
 def scache(cache_num: int) -> str:
     """Return cache suffix string"""
     return f"__{cache_num}" if cache_num > 0 else ""
+
+
+def escape_fmt_group(value: str) -> str:
+    """Escape value of format group before format
+
+    Examples:
+        >>> escape_fmt_group(
+        ...     "+file_{datetime:%Y-%m-%d %H:%M:%S}_{naming:%n_%e}.json"
+        ... ).replace('\\\\', '?')  # Replace because doc-string issue!
+        '?+file_{datetime:%Y-%m-%d %H:%M:%S}_{naming:%n_%e}?.json'
+
+        >>> escape_fmt_group(
+        ...     "+file_{datetime:%Y-%m-%d %H:%M:%S}_{naming:%n_%e}\\.json"
+        ... ).replace('\\\\', '?')  # Replace because doc-string issue!
+        '?+file_{datetime:%Y-%m-%d %H:%M:%S}_{naming:%n_%e}???.json'
+    """
+    rs: str = value
+    revert: dict[str, str] = {}
+    for i, s in enumerate(
+        re.finditer(r"(?P<found>{\w+:?([^{}]+)?})", value), start=1
+    ):
+        found: str = s.group("found")
+        rs = rs.replace(found, f"<ESCAPE{i:03d}>")
+        revert[f"<ESCAPE{i:03d}>"] = found
+    rs = re.escape(rs)
+    for rv in revert:
+        rs = rs.replace(rv, revert[rv])
+    return rs
```

### Comparing `fmtutil-1.0.5/.gitignore` & `fmtutil-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.5/LICENSE` & `fmtutil-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.5/README.md` & `fmtutil-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,43 +14,53 @@
   * [Serial](#serial)
   * [Naming](#naming)
   * [Storage](#storage)
   * [Constant](#constant)
 * [FormatterGroup Object](#formattergroup-object)
 * [Usecase](#usecase)
 
-This **Formatter Utility Objects** package was created for `parse` and `format`
-any string values that match a format pattern string with Python regular
-expression. This package be the co-pylot project for stating to my
-**Python Software Developer** role.
+This **Formatter** package was created for `parse` and `format` any string values
+that match a format pattern string with Python regular expression.
+This package be the co-pylot project for stating to my **Python Software Developer**
+way.
 
 :dart: First objective of this project is include necessary formatter objects for
 any data components package which mean we can `parse` any complicate names on
 data source and ingest the right names to in-house or data target.
 
 ## Installation
 
 ```shell
 pip install -U fmtutil
 ```
 
+**Dependency supported**:
+
+| Python Version  | Installation                        |
+|-----------------|-------------------------------------|
+| `== 3.8`        | `pip install "fmtutil>=0.4,<0.5.0"` |
+| `>=3.9,<3.13`   | `pip install -U fmtutil`            |
+
+
 For example, we want to get filename with the format like, `filename_20220101.csv`,
 on the file system storage, and we want to incremental ingest the latest file with
 date **2022-03-25** date. So we will implement `Datetime` object and parse
 that filename to it,
 
 ```python
-Datetime.parse('filename_20220101.csv', 'filename_%Y%m%d.csv').value == datetime.today()
+assert (
+    Datetime.parse('filename_20220101.csv', 'filename_%Y%m%d.csv').value
+    == datetime.datetime(2022, 1, 1, 0)
+)
 ```
 
 The above example is :yawning_face: **NOT SURPRISE!!!** for us because Python
-already provide build-in package `datetime` to parse by `{dt}.strptime` and
-format by `{dt}.strftime` with any datetime string value. This package will the
-special thing when we group more than one formatter objects together as
-`Naming`, `Version`, and `Datetime`.
+already provide the build-in `datetime` to parse by `datetime.strptime` and
+format by `{dt}.strftime`. This package will be the special thing when we group
+more than one format-able objects together as `Naming`, `Version`, and `Datetime`.
 
 **For complex filename format like**:
 
 ```text
 {filename:%s}_{datetime:%Y_%m_%d}.{version:%m.%n.%c}.csv
 ```
 
@@ -62,21 +72,14 @@
 > Any formatter object was implemented the `self.valid` method for help us validate
 > format string value like the above the example scenario,
 > ```python
 > this_date = Datetime.parse('20220101', '%Y%m%d')
 > assert this_date.valid('any_files_20220101.csv', 'any_files_%Y%m%d.csv')
 > ```
 
-**Dependency supported**:
-
-| Python Version  | Installation                        |
-|-----------------|-------------------------------------|
-| `== 3.8`        | `pip install "fmtutil>=0.4,<0.5.0"` |
-| `>=3.9,<3.13`   | `pip install -U fmtutil`            |
-
 ## Formatter Objects
 
 * [Datetime](#datetime)
 * [Version](#version)
 * [Serial](#serial)
 * [Naming](#naming)
 * [Storage](#storage)
@@ -102,75 +105,75 @@
 datetime.format('New_datetime_%Y%b-%-d_%H:%M:%S')
 ```
 
 ```text
 >>> 'New_datetime_2022Jan-1_00:01:01'
 ```
 
-[Supported Datetime formats](/docs/en/docs/API.md#datetime)
+[Supported Datetime formats](/docs/API.md#datetime)
 
 ### Version
 
 ```python
 from fmtutil import Version
 
 version = Version.parse(value='Version_2_0_1', fmt='Version_%m_%n_%c')
 version.format('New_version_%m%n%c')
 ```
 
 ```text
 >>> 'New_version_201'
 ```
 
-[Supported Version formats](/docs/en/docs/API.md#version)
+[Supported Version formats](/docs/API.md#version)
 
 ### Serial
 
 ```python
 from fmtutil import Serial
 
 serial = Serial.parse(value='Serial_62130', fmt='Serial_%n')
 serial.format('Convert to binary: %b')
 ```
 
 ```text
 >>> 'Convert to binary: 1111001010110010'
 ```
 
-[Supported Serial formats](/docs/en/docs/API.md#serial)
+[Supported Serial formats](/docs/API.md#serial)
 
 ### Naming
 
 ```python
 from fmtutil import Naming
 
 naming = Naming.parse(value='de is data engineer', fmt='%a is %n')
 naming.format('Camel case is %c')
 ```
 
 ```text
 >>> 'Camel case is dataEngineer'
 ```
 
-[Supported Naming formats](/docs/en/docs/API.md#naming)
+[Supported Naming formats](/docs/API.md#naming)
 
 ### Storage
 
 ```python
 from fmtutil import Storage
 
 storage = Storage.parse(value='This file have 250MB size', fmt='This file have %M size')
 storage.format('The byte size is: %b')
 ```
 
 ```text
 >>> 'The byte size is: 2097152000'
 ```
 
-[Supported Storage formats](/docs/en/docs/API.md#storage)
+[Supported Storage formats](/docs/API.md#storage)
 
 ### Constant
 
 ```python
 from fmtutil import Constant, make_const
 from fmtutil.exceptions import FormatterError
 
@@ -182,18 +185,21 @@
     pass
 ```
 
 ```text
 >>> 'The value of %s is special'
 ```
 
+All formatter object can convert itself to constant formatter object for frozen
+parsing value to constant by `.to_const()`.
+
 > [!NOTE]
 > This package already implement the environment constant object,
 > `fmtutil.EnvConst`. \
-> [Read more about this formats](/docs/en/docs/API.md#environment-constant)
+> [Read more about this formats](/docs/API.md#environment-constant)
 
 ## FormatterGroup Object
 
 The **FormatterGroup** object, `FormatterGroup`, which is the grouping of needed
 mapping formatter objects and its alias formatter object ref name together. You
 can define a name of formatter that you want, such as `name` for `Naming`, or
 `timestamp` for `Datetime`.
```

### Comparing `fmtutil-1.0.5/pyproject.toml` & `fmtutil-1.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 [build-system]
-requires = [
-    "hatchling>=1.8.0",
-    # This plug-in support for py-version >= 3.9
-    # "hatch-semver",
-]
+requires = ["hatchling>=1.8.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fmtutil"
 description = "The Utility Formatter Objects"
 readme = "README.md"
 requires-python = ">=3.9.0"
@@ -42,24 +38,24 @@
 "Source Code" = "https://github.com/korawica/fmtutil/"
 
 [project.optional-dependencies]
 dev = [
     "clishelf",
     "types-python-dateutil==2.9.0.20240316",
 ]
-perf = [
-    "memory-profiler==0.61.0",
+docs = [
+    "mkdocs-material",
 ]
 
 [project.scripts]
 fmtutil = "fmtutil.__main__:main"
 
 [tool.shelf.version]
 version = "./fmtutil/__about__.py"
-changelog = "./docs/en/docs/CHANGELOG.md"
+changelog = "./CHANGELOG.md"
 
 [tool.shelf.git]
 commit_prefix_force_fix = true
 
 [tool.hatch.version]
 scheme = "standard"
 source = "code"
@@ -119,18 +115,20 @@
 show_error_codes = true
 pretty = true
 strict = true
 warn_unreachable = true
 warn_unused_ignores = false
 exclude = [
     '__version\.py$',
+    '__assets\.py$',
 ]
 
 [tool.black]
 line-length = 80
+preview = true
 target-version = ['py39']
 exclude = """
 (
     /(
         \\.git
         | \\.eggs
         | \\.__pycache__
@@ -144,15 +142,14 @@
         | venv
     )/
 )
 """
 
 [tool.ruff]
 line-length = 80
-# Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     ".mypy_cache",
     ".ruff_cache",
     "venv",
 ]
```

### Comparing `fmtutil-1.0.5/PKG-INFO` & `fmtutil-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fmtutil
-Version: 1.0.5
+Version: 1.0.6
 Summary: The Utility Formatter Objects
 Project-URL: Homepage, https://github.com/korawica/fmtutil/
 Project-URL: Source Code, https://github.com/korawica/fmtutil/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: formatter,utility
@@ -20,16 +20,16 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9.0
 Requires-Dist: python-dateutil<3.0.0,>=2.8.2
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: clishelf; extra == 'dev'
 Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == 'dev'
-Provides-Extra: perf
-Requires-Dist: memory-profiler==0.61.0; extra == 'perf'
+Provides-Extra: docs
+Requires-Dist: mkdocs-material; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # _Formatter Utility_
 
 [![test](https://github.com/korawica/fmtutil/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/fmtutil/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/korawica/fmtutil/branch/main/graph/badge.svg?token=J2MN63IFT0)](https://codecov.io/gh/korawica/fmtutil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fmtutil?logo=pypi)](https://pypi.org/project/fmtutil/)
@@ -44,43 +44,53 @@
   * [Serial](#serial)
   * [Naming](#naming)
   * [Storage](#storage)
   * [Constant](#constant)
 * [FormatterGroup Object](#formattergroup-object)
 * [Usecase](#usecase)
 
-This **Formatter Utility Objects** package was created for `parse` and `format`
-any string values that match a format pattern string with Python regular
-expression. This package be the co-pylot project for stating to my
-**Python Software Developer** role.
+This **Formatter** package was created for `parse` and `format` any string values
+that match a format pattern string with Python regular expression.
+This package be the co-pylot project for stating to my **Python Software Developer**
+way.
 
 :dart: First objective of this project is include necessary formatter objects for
 any data components package which mean we can `parse` any complicate names on
 data source and ingest the right names to in-house or data target.
 
 ## Installation
 
 ```shell
 pip install -U fmtutil
 ```
 
+**Dependency supported**:
+
+| Python Version  | Installation                        |
+|-----------------|-------------------------------------|
+| `== 3.8`        | `pip install "fmtutil>=0.4,<0.5.0"` |
+| `>=3.9,<3.13`   | `pip install -U fmtutil`            |
+
+
 For example, we want to get filename with the format like, `filename_20220101.csv`,
 on the file system storage, and we want to incremental ingest the latest file with
 date **2022-03-25** date. So we will implement `Datetime` object and parse
 that filename to it,
 
 ```python
-Datetime.parse('filename_20220101.csv', 'filename_%Y%m%d.csv').value == datetime.today()
+assert (
+    Datetime.parse('filename_20220101.csv', 'filename_%Y%m%d.csv').value
+    == datetime.datetime(2022, 1, 1, 0)
+)
 ```
 
 The above example is :yawning_face: **NOT SURPRISE!!!** for us because Python
-already provide build-in package `datetime` to parse by `{dt}.strptime` and
-format by `{dt}.strftime` with any datetime string value. This package will the
-special thing when we group more than one formatter objects together as
-`Naming`, `Version`, and `Datetime`.
+already provide the build-in `datetime` to parse by `datetime.strptime` and
+format by `{dt}.strftime`. This package will be the special thing when we group
+more than one format-able objects together as `Naming`, `Version`, and `Datetime`.
 
 **For complex filename format like**:
 
 ```text
 {filename:%s}_{datetime:%Y_%m_%d}.{version:%m.%n.%c}.csv
 ```
 
@@ -92,21 +102,14 @@
 > Any formatter object was implemented the `self.valid` method for help us validate
 > format string value like the above the example scenario,
 > ```python
 > this_date = Datetime.parse('20220101', '%Y%m%d')
 > assert this_date.valid('any_files_20220101.csv', 'any_files_%Y%m%d.csv')
 > ```
 
-**Dependency supported**:
-
-| Python Version  | Installation                        |
-|-----------------|-------------------------------------|
-| `== 3.8`        | `pip install "fmtutil>=0.4,<0.5.0"` |
-| `>=3.9,<3.13`   | `pip install -U fmtutil`            |
-
 ## Formatter Objects
 
 * [Datetime](#datetime)
 * [Version](#version)
 * [Serial](#serial)
 * [Naming](#naming)
 * [Storage](#storage)
@@ -132,75 +135,75 @@
 datetime.format('New_datetime_%Y%b-%-d_%H:%M:%S')
 ```
 
 ```text
 >>> 'New_datetime_2022Jan-1_00:01:01'
 ```
 
-[Supported Datetime formats](/docs/en/docs/API.md#datetime)
+[Supported Datetime formats](/docs/API.md#datetime)
 
 ### Version
 
 ```python
 from fmtutil import Version
 
 version = Version.parse(value='Version_2_0_1', fmt='Version_%m_%n_%c')
 version.format('New_version_%m%n%c')
 ```
 
 ```text
 >>> 'New_version_201'
 ```
 
-[Supported Version formats](/docs/en/docs/API.md#version)
+[Supported Version formats](/docs/API.md#version)
 
 ### Serial
 
 ```python
 from fmtutil import Serial
 
 serial = Serial.parse(value='Serial_62130', fmt='Serial_%n')
 serial.format('Convert to binary: %b')
 ```
 
 ```text
 >>> 'Convert to binary: 1111001010110010'
 ```
 
-[Supported Serial formats](/docs/en/docs/API.md#serial)
+[Supported Serial formats](/docs/API.md#serial)
 
 ### Naming
 
 ```python
 from fmtutil import Naming
 
 naming = Naming.parse(value='de is data engineer', fmt='%a is %n')
 naming.format('Camel case is %c')
 ```
 
 ```text
 >>> 'Camel case is dataEngineer'
 ```
 
-[Supported Naming formats](/docs/en/docs/API.md#naming)
+[Supported Naming formats](/docs/API.md#naming)
 
 ### Storage
 
 ```python
 from fmtutil import Storage
 
 storage = Storage.parse(value='This file have 250MB size', fmt='This file have %M size')
 storage.format('The byte size is: %b')
 ```
 
 ```text
 >>> 'The byte size is: 2097152000'
 ```
 
-[Supported Storage formats](/docs/en/docs/API.md#storage)
+[Supported Storage formats](/docs/API.md#storage)
 
 ### Constant
 
 ```python
 from fmtutil import Constant, make_const
 from fmtutil.exceptions import FormatterError
 
@@ -212,18 +215,21 @@
     pass
 ```
 
 ```text
 >>> 'The value of %s is special'
 ```
 
+All formatter object can convert itself to constant formatter object for frozen
+parsing value to constant by `.to_const()`.
+
 > [!NOTE]
 > This package already implement the environment constant object,
 > `fmtutil.EnvConst`. \
-> [Read more about this formats](/docs/en/docs/API.md#environment-constant)
+> [Read more about this formats](/docs/API.md#environment-constant)
 
 ## FormatterGroup Object
 
 The **FormatterGroup** object, `FormatterGroup`, which is the grouping of needed
 mapping formatter objects and its alias formatter object ref name together. You
 can define a name of formatter that you want, such as `name` for `Naming`, or
 `timestamp` for `Datetime`.
```

