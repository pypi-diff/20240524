# Comparing `tmp/paramparse-1.8.6.tar.gz` & `tmp/paramparse-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\paramparse-1.8.6.tar", last modified: Sun Mar 24 22:30:09 2024, max compression
+gzip compressed data, was "dist\paramparse-1.8.7.tar", last modified: Thu May 23 22:43:48 2024, max compression
```

## Comparing `paramparse-1.8.6.tar` & `paramparse-1.8.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 22:30:09.000000 paramparse-1.8.6/
--rw-rw-rw-   0        0        0       18 2019-07-29 15:38:10.000000 paramparse-1.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0    14888 2024-03-24 22:30:09.000000 paramparse-1.8.6/PKG-INFO
--rw-rw-rw-   0        0        0    13034 2024-03-09 19:58:48.000000 paramparse-1.8.6/ReadMe.md
-drwxrwxrwx   0        0        0        0 2024-03-24 22:30:09.000000 paramparse-1.8.6/docstring_parser_custom/
--rw-rw-rw-   0        0        0      455 2020-08-09 15:26:50.000000 paramparse-1.8.6/docstring_parser_custom/__init__.py
--rw-rw-rw-   0        0        0     3832 2021-10-19 14:46:22.000000 paramparse-1.8.6/docstring_parser_custom/common.py
--rw-rw-rw-   0        0        0     8924 2021-01-03 20:14:41.000000 paramparse-1.8.6/docstring_parser_custom/google.py
--rw-rw-rw-   0        0        0    10163 2020-08-09 15:26:50.000000 paramparse-1.8.6/docstring_parser_custom/numpydoc.py
--rw-rw-rw-   0        0        0      716 2021-10-19 14:46:42.000000 paramparse-1.8.6/docstring_parser_custom/parser.py
--rw-rw-rw-   0        0        0     3599 2020-08-09 15:26:50.000000 paramparse-1.8.6/docstring_parser_custom/rest.py
--rw-rw-rw-   0        0        0      316 2020-08-09 15:26:50.000000 paramparse-1.8.6/docstring_parser_custom/styles.py
-drwxrwxrwx   0        0        0        0 2024-03-24 22:30:09.000000 paramparse-1.8.6/docstring_parser_custom/tests/
--rw-rw-rw-   0        0        0       34 2020-08-09 15:26:50.000000 paramparse-1.8.6/docstring_parser_custom/tests/__init__.py
--rw-rw-rw-   0        0        0    16178 2024-02-26 01:26:17.000000 paramparse-1.8.6/docstring_parser_custom/tests/test_google.py
--rw-rw-rw-   0        0        0    17278 2024-02-26 01:26:17.000000 paramparse-1.8.6/docstring_parser_custom/tests/test_numpydoc.py
--rw-rw-rw-   0        0        0     4732 2024-02-26 01:26:17.000000 paramparse-1.8.6/docstring_parser_custom/tests/test_parser.py
--rw-rw-rw-   0        0        0    10372 2024-02-26 01:26:17.000000 paramparse-1.8.6/docstring_parser_custom/tests/test_rest.py
-drwxrwxrwx   0        0        0        0 2024-03-24 22:30:09.000000 paramparse-1.8.6/paramparse.egg-info/
--rw-rw-rw-   0        0        0    14888 2024-03-24 22:30:09.000000 paramparse-1.8.6/paramparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-03-24 22:30:09.000000 paramparse-1.8.6/paramparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 22:30:09.000000 paramparse-1.8.6/paramparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-03-24 22:30:09.000000 paramparse-1.8.6/paramparse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    87824 2024-03-24 22:28:52.000000 paramparse-1.8.6/paramparse.py
--rw-rw-rw-   0        0        0       42 2024-03-24 22:30:09.000000 paramparse-1.8.6/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-03-24 22:29:39.000000 paramparse-1.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:43:48.000000 paramparse-1.8.7/
+-rw-rw-rw-   0        0        0       18 2019-07-29 15:38:10.000000 paramparse-1.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    14888 2024-05-23 22:43:48.000000 paramparse-1.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13034 2024-03-09 19:58:48.000000 paramparse-1.8.7/ReadMe.md
+drwxrwxrwx   0        0        0        0 2024-05-23 22:43:48.000000 paramparse-1.8.7/docstring_parser_custom/
+-rw-rw-rw-   0        0        0      455 2020-08-09 15:26:50.000000 paramparse-1.8.7/docstring_parser_custom/__init__.py
+-rw-rw-rw-   0        0        0     3832 2021-10-19 14:46:22.000000 paramparse-1.8.7/docstring_parser_custom/common.py
+-rw-rw-rw-   0        0        0     8924 2021-01-03 20:14:41.000000 paramparse-1.8.7/docstring_parser_custom/google.py
+-rw-rw-rw-   0        0        0    10163 2020-08-09 15:26:50.000000 paramparse-1.8.7/docstring_parser_custom/numpydoc.py
+-rw-rw-rw-   0        0        0      716 2021-10-19 14:46:42.000000 paramparse-1.8.7/docstring_parser_custom/parser.py
+-rw-rw-rw-   0        0        0     3599 2020-08-09 15:26:50.000000 paramparse-1.8.7/docstring_parser_custom/rest.py
+-rw-rw-rw-   0        0        0      316 2020-08-09 15:26:50.000000 paramparse-1.8.7/docstring_parser_custom/styles.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:43:48.000000 paramparse-1.8.7/docstring_parser_custom/tests/
+-rw-rw-rw-   0        0        0       34 2020-08-09 15:26:50.000000 paramparse-1.8.7/docstring_parser_custom/tests/__init__.py
+-rw-rw-rw-   0        0        0    16178 2024-02-26 01:26:17.000000 paramparse-1.8.7/docstring_parser_custom/tests/test_google.py
+-rw-rw-rw-   0        0        0    17278 2024-02-26 01:26:17.000000 paramparse-1.8.7/docstring_parser_custom/tests/test_numpydoc.py
+-rw-rw-rw-   0        0        0     4732 2024-02-26 01:26:17.000000 paramparse-1.8.7/docstring_parser_custom/tests/test_parser.py
+-rw-rw-rw-   0        0        0    10372 2024-02-26 01:26:17.000000 paramparse-1.8.7/docstring_parser_custom/tests/test_rest.py
+drwxrwxrwx   0        0        0        0 2024-05-23 22:43:48.000000 paramparse-1.8.7/paramparse.egg-info/
+-rw-rw-rw-   0        0        0    14888 2024-05-23 22:43:47.000000 paramparse-1.8.7/paramparse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-23 22:43:47.000000 paramparse-1.8.7/paramparse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 22:43:47.000000 paramparse-1.8.7/paramparse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-23 22:43:47.000000 paramparse-1.8.7/paramparse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    87957 2024-05-23 22:40:28.000000 paramparse-1.8.7/paramparse.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 22:43:48.000000 paramparse-1.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-23 22:41:30.000000 paramparse-1.8.7/setup.py
```

### Comparing `paramparse-1.8.6/PKG-INFO` & `paramparse-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramparse
-Version: 1.8.6
+Version: 1.8.7
 Summary: argparse wrapper to allow hierarchically nested class based parameters
 Home-page: https://github.com/abhineet123/paramparse
 Author: Abhineet Singh
 Author-email: abhineet.iiita@gmail.com
 License: UNKNOWN
 Description: <!-- No Heading Fix -->
```

### Comparing `paramparse-1.8.6/ReadMe.md` & `paramparse-1.8.7/ReadMe.md`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/common.py` & `paramparse-1.8.7/docstring_parser_custom/common.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/google.py` & `paramparse-1.8.7/docstring_parser_custom/google.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/numpydoc.py` & `paramparse-1.8.7/docstring_parser_custom/numpydoc.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/parser.py` & `paramparse-1.8.7/docstring_parser_custom/parser.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/rest.py` & `paramparse-1.8.7/docstring_parser_custom/rest.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/tests/test_google.py` & `paramparse-1.8.7/docstring_parser_custom/tests/test_google.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/tests/test_numpydoc.py` & `paramparse-1.8.7/docstring_parser_custom/tests/test_numpydoc.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/tests/test_parser.py` & `paramparse-1.8.7/docstring_parser_custom/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/docstring_parser_custom/tests/test_rest.py` & `paramparse-1.8.7/docstring_parser_custom/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/paramparse.egg-info/PKG-INFO` & `paramparse-1.8.7/paramparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramparse
-Version: 1.8.6
+Version: 1.8.7
 Summary: argparse wrapper to allow hierarchically nested class based parameters
 Home-page: https://github.com/abhineet123/paramparse
 Author: Abhineet Singh
 Author-email: abhineet.iiita@gmail.com
 License: UNKNOWN
 Description: <!-- No Heading Fix -->
```

### Comparing `paramparse-1.8.6/paramparse.egg-info/SOURCES.txt` & `paramparse-1.8.7/paramparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paramparse-1.8.6/paramparse.py` & `paramparse-1.8.7/paramparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,14 +497,18 @@
         arg_vals_parsed = []
         for _val in arg_vals:
             _val_parsed = str_to_basic_type(_val)
             arg_vals_parsed.append(_val_parsed)
         return arg_vals_parsed
 
 
+def linux_path(*args, **kwargs):
+    return os.path.join(*args, **kwargs).replace(os.sep, '/')
+
+
 def str_to_basic_type(_val):
     # if _type == str:
     #     _val_parsed = _val
     #     if _val_parsed == '__n__':
     #         _val_parsed = ''
     #     return _val_parsed
 
@@ -565,35 +569,35 @@
             # dst_member = getattr(dst, member)
             member_val_copy = copy_recursive(member_val, include_protected=include_protected)
             setattr(dst, member, member_val_copy)
     return dst
 
 
 def save(obj, dir_name, out_name='params.bin'):
-    save_path = os.path.join(dir_name, out_name)
+    save_path = linux_path(dir_name, out_name)
     pickle.dump(obj, open(save_path, "wb"))
 
 
 def load(obj, dir_name, prefix='', out_name='params.bin'):
-    load_path = os.path.join(dir_name, out_name)
+    load_path = linux_path(dir_name, out_name)
     params = pickle.load(open(load_path, "rb"))
     missing_params = []
     _recursive_load(obj, params, prefix, missing_params)
     if missing_params:
         print('Missing loaded parameters found:\n{}'.format(pformat(missing_params)))
 
 
 def write(obj, dir_name, prefix='', out_name='params.cfg'):
-    save_path = os.path.join(dir_name, out_name)
+    save_path = linux_path(dir_name, out_name)
     save_fid = open(save_path, "w")
     _recursive_write(obj, prefix, save_fid)
 
 
 def read(obj, dir_name, prefix='', out_name='params.cfg', allow_unknown=0):
-    load_path = os.path.join(dir_name, out_name)
+    load_path = linux_path(dir_name, out_name)
     lines = open(load_path, "r").readlines()
     if prefix:
         lines = [k.replace(prefix + '.', '') for k in lines if k.startswith(prefix + '.')]
     args_in = ['--{}'.format(k.strip()) for k in lines]
     process(obj, args_in=args_in, prog=prefix,
             usage=None, allow_unknown=allow_unknown)
 
@@ -997,15 +1001,15 @@
 
     out_file_args = []
     out_imported_cfgs = [cfg, ]
 
     for file_arg_id, file_arg in enumerate(file_args):
         if file_arg.startswith('%import% '):
             _, imported_cfg_name = file_arg.split(' ')
-            imported_cfg = os.path.join(cfg_dir, imported_cfg_name)
+            imported_cfg = linux_path(cfg_dir, imported_cfg_name)
             prev_imported_cfgs = tuple(set(imported_cfgs + tuple(out_imported_cfgs)))
 
             assert imported_cfg not in prev_imported_cfgs, f"circular CFG import found in {cfg}: {imported_cfg}"
 
             out_imported_cfgs.append(imported_cfg)
             imported_file_args, imported_cfgs = recursive_read(
                 imported_cfg, imported_cfgs=tuple(out_imported_cfgs), level=level + 1)
@@ -1019,18 +1023,18 @@
     return out_file_args, out_imported_cfgs
 
 
 def get_cfg_cache_path(_cfg):
     _cfg_dir = os.path.dirname(_cfg)
     _cfg_name = os.path.basename(_cfg)
 
-    _cfg_cache_dir = os.path.join(_cfg_dir, '.cache')
+    _cfg_cache_dir = linux_path(_cfg_dir, '.cache')
     os.makedirs(_cfg_cache_dir, exist_ok=True)
 
-    cfg_cache_path = os.path.join(_cfg_cache_dir, _cfg_name + '.cache')
+    cfg_cache_path = linux_path(_cfg_cache_dir, _cfg_name + '.cache')
 
     return cfg_cache_path
 
 
 def load_cfg_cache(_cfg):
     cfg_cache_path = get_cfg_cache_path(_cfg)
 
@@ -1391,19 +1395,19 @@
             if cfg_suffix:
                 _cfg = f'{_cfg}-{cfg_suffix}'
 
             if cfg_ext:
                 _cfg = f'{_cfg}.{cfg_ext}'
 
             if cfg_root:
-                _cfg = os.path.join(cfg_root, _cfg)
+                _cfg = linux_path(cfg_root, _cfg)
 
             if not os.path.isfile(_cfg):
                 if _cfg:
-                    raise IOError('cfg file does not exist: {:s}'.format(os.path.abspath(_cfg)))
+                    raise IOError('cfg file does not exist: {:s}'.format(linux_path(os.path.abspath(_cfg))))
             repeated_cfgs = []
 
             repeated_sec_ids = [__sec_id for __sec_id, __sec in enumerate(_cfg_sec) if '+' in __sec]
 
             excluded_ids = []
 
             for i, __sec_id in enumerate(repeated_sec_ids):
@@ -2098,15 +2102,15 @@
             print('Copying to clipboard failed: {}'.format(e))
         else:
             print('Class definition copied to clipboard')
 
     else:
         class_name_snake_case = re.sub(r'(?<!^)(?=[A-Z])', '_', class_name).lower()
         out_fname = '{}.py'.format(class_name_snake_case)
-        out_path = os.path.abspath(out_fname)
+        out_path = linux_path(os.path.abspath(out_fname))
         if os.path.exists(out_path):
             print('output path already exists so not writing to it: {}'.format(out_path))
         else:
             print('Writing output to {}'.format(out_path))
             with open(out_path, 'w') as fid:
                 fid.write(out_text)
 
@@ -2234,15 +2238,15 @@
             print('Copying to clipboard failed: {}'.format(e))
         else:
             print('Class definition copied to clipboard')
 
     else:
         class_name_snake_case = re.sub(r'(?<!^)(?=[A-Z])', '_', class_name).lower()
         out_fname = '{}.py'.format(class_name_snake_case)
-        out_path = os.path.abspath(out_fname)
+        out_path = linux_path(os.path.abspath(out_fname))
         if os.path.exists(out_path):
             print('output path already exists so not writing to it: {}'.format(out_path))
         else:
             print('Writing output to {}'.format(out_path))
             with open(out_path, 'w') as fid:
                 fid.write(out_text)
 
@@ -2387,15 +2391,15 @@
             print('Copying to clipboard failed: {}'.format(e))
         else:
             print('Class definition for class {} copied to clipboard'.format(class_name))
 
     else:
         class_name_snake_case = re.sub(r'(?<!^)(?=[A-Z])', '_', class_name).lower()
         out_fname = '{}.py'.format(class_name_snake_case)
-        out_path = os.path.abspath(out_fname)
+        out_path = linux_path(os.path.abspath(out_fname))
 
         if os.path.exists(out_path):
             print('output path already exists so not writing to it: {}'.format(out_path))
         else:
             print('Writing output to {}'.format(out_path))
             with open(out_path, 'w') as fid:
                 fid.write(out_text)
```

### Comparing `paramparse-1.8.6/setup.py` & `paramparse-1.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("ReadMe.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="paramparse",
-    version="1.8.6",
+    version="1.8.7",
     author="Abhineet Singh",
     author_email="abhineet.iiita@gmail.com",
     description="argparse wrapper to allow hierarchically nested class based parameters",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/abhineet123/paramparse",
     include_package_data=True,
```

