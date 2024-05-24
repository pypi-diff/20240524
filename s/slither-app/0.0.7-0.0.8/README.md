# Comparing `tmp/slither_app-0.0.7.tar.gz` & `tmp/slither_app-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/users/p259232/dev/slither_app/slither_app/dist/.tmp-xhvsvu0z/slither_app-0.0.7.tar", last modified: Thu Mar  7 09:23:50 2024, max compression
+gzip compressed data, was "/users/p259232/dev/slither_app/slither_app/dist/.tmp-rpkgy96k/slither_app-0.0.8.tar", last modified: Fri May 24 10:38:27 2024, max compression
```

## Comparing `slither_app-0.0.7.tar` & `slither_app-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-03-07 09:23:50.000000 slither_app-0.0.7/
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      478 2024-03-01 08:49:57.000000 slither_app-0.0.7/LICENSE
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)     1007 2024-03-07 09:23:50.000000 slither_app-0.0.7/PKG-INFO
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      105 2024-03-01 10:15:53.000000 slither_app-0.0.7/README.md
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      421 2024-03-07 09:23:44.000000 slither_app-0.0.7/pyproject.toml
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)       38 2024-03-07 09:23:50.000000 slither_app-0.0.7/setup.cfg
-drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/
-drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/slither_app/
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-03-01 08:38:22.000000 slither_app-0.0.7/src/slither_app/__init__.py
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)     8191 2024-03-07 09:16:44.000000 slither_app-0.0.7/src/slither_app/slither_app.py
-drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/slither_app.egg-info/
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)     1007 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/slither_app.egg-info/PKG-INFO
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      247 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/slither_app.egg-info/SOURCES.txt
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)        1 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/slither_app.egg-info/dependency_links.txt
--rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)       12 2024-03-07 09:23:50.000000 slither_app-0.0.7/src/slither_app.egg-info/top_level.txt
+drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-05-24 10:38:27.000000 slither_app-0.0.8/
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      478 2024-03-01 08:49:57.000000 slither_app-0.0.8/LICENSE
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)     1007 2024-05-24 10:38:27.000000 slither_app-0.0.8/PKG-INFO
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      105 2024-03-01 10:15:53.000000 slither_app-0.0.8/README.md
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      421 2024-05-17 08:12:41.000000 slither_app-0.0.8/pyproject.toml
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)       38 2024-05-24 10:38:27.000000 slither_app-0.0.8/setup.cfg
+drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/
+drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/slither_app/
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-03-01 08:38:22.000000 slither_app-0.0.8/src/slither_app/__init__.py
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)    11328 2024-05-24 10:28:36.000000 slither_app-0.0.8/src/slither_app/slither_app.py
+drwxr-xr-x   0 p259232  (3001011) grp_hpc_met  (5200)        0 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/slither_app.egg-info/
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)     1007 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/slither_app.egg-info/PKG-INFO
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)      247 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/slither_app.egg-info/SOURCES.txt
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)        1 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/slither_app.egg-info/dependency_links.txt
+-rw-r--r--   0 p259232  (3001011) grp_hpc_met  (5200)       12 2024-05-24 10:38:27.000000 slither_app-0.0.8/src/slither_app.egg-info/top_level.txt
```

### Comparing `slither_app-0.0.7/PKG-INFO` & `slither_app-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slither_app
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: Adam Otruba <adam.otruba@shmu.sk>
 License: DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE 
                             Version 2, December 2004 
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
```

### Comparing `slither_app-0.0.7/src/slither_app/slither_app.py` & `slither_app-0.0.8/src/slither_app/slither_app.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,252 +4,331 @@
 import os
 import os.path as p
 import typing as typ
 import datetime as dt
 import pprint
 import sys
 
-def attach_to_parser(parser):
+
+def attach_to_parser(parser: ap.ArgumentParser):
     """When supplied with an existing `argparse.ArgumentParser` instance,
-    adds arguments associated with run_app to it. Example usage:
-    
+    adds arguments associated with run_app to it.
+
+    Typical usage:
+
     .. code:: python
-    
+
         parser = ap.ArgumentParser()
         attach_to_parser(parser)
         args = parser.parse_args()
 
     :param parser: an initialised argument
         parser
     :type parser: argparse.ArgumentParser
     """
-    
+
     # add run_app arguments to parser
     parser.add_argument(
-        '-s','--silent',
-        action = 'store_true',
-        help='''Suppress all messages made by this program.
-            Doesn't suppress python exceptions.''',
-        dest='CNF_SILENT',
-        default=None
+        "-s",
+        "--silent",
+        action="store_true",
+        help="""Suppress all messages made by this program.
+            Doesn't suppress python exceptions.""",
+        dest="CNF_SILENT",
+        default=None,
     )
 
     parser.add_argument(
-        '-v','--verbose',
-        action = 'store_true',
-        help='''Increase verbosity. Shows warnings and diagnostic
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="""Increase verbosity. Shows warnings and diagnostic
             messages in addition to errors, which are displayed by
-            default.''',
-        dest='CNF_VERBOSE',
-        default=None
+            default.""",
+        dest="CNF_VERBOSE",
+        default=None,
     )
 
     parser.add_argument(
-        '-d','--debug',
-        action = 'store_true',
-        help='''Enable diagnostic code. May slow the program down
+        "-d",
+        "--debug",
+        action="store_true",
+        help="""Enable diagnostic code. May slow the program down
         considerably, only use if something went wrong. Enables verbosity
-        as with --verbose, but also shows debug messages in addition.''',
-        dest='CNF_DEBUG',
-        default=None
+        as with --verbose, but also shows debug messages in addition.""",
+        dest="CNF_DEBUG",
+        default=None,
     )
 
     parser.add_argument(
-        '--dir-work',
-        action = 'store',
-        help = '''Override work directory, for temporary files.''',
-        metavar = '/path/to/workdir',
-        dest = 'CNF_TMP',
+        "--dir-work",
+        action="store",
+        help="""Override work directory, for temporary files.""",
+        metavar="/path/to/workdir",
+        dest="CNF_TMP",
     )
 
     parser.add_argument(
-        '--dir-data',
-        action = 'store',
-        help = '''Override data directory, for output files''',
-        metavar = '/path/to/datadir',
-        dest = 'CNF_PRODUCTS',
+        "--dir-data",
+        action="store",
+        help="""Override data directory, for output files""",
+        metavar="/path/to/datadir",
+        dest="CNF_PRODUCTS",
     )
 
-def create_parser(parse_args: bool =False) -> typ.Tuple[ap.ArgumentParser, typ.Optional[ap.Namespace]]:
+
+def create_parser(
+    parse_args: bool = False,
+) -> typ.Tuple[ap.ArgumentParser, typ.Optional[ap.Namespace]]:
     """Creates a parser with run_app arguments. If ``parse_args`` is ``True``,
     parses arguments and returns the parsed argparse.Namespace object
     along with the parser instance. If it is ``False``, returns None
     along with the parser instance.
 
     :param parse_args: Whether to parse arguments , defaults to False
     :type parse_args: bool, optional
     :return: A tuple containing the argument parser instance and either
         None, or the Namespace object
     :rtype: (`ap.ArgumentParser`, ``None``) or (`ap.ArgumentParser`, `ap.Namespace`)
     """
-    
+
     parser = ap.ArgumentParser()
 
     attach_to_parser(parser)
 
     if parse_args:
         args = parser.parse_args()
     else:
         args = None
 
     return parser, args
 
 
-class Env_parser():
-
-    def __init__(self,arg_parser=None,parsed_args=None,defaults=None):
+class Env_parser:
+    """An object that associates with an argument parser and its namespace when
+    created. It allows you to parse environment variables and decide defaults for those arguments that
+    are not explicitly set (overriden) by the user on the command line."""
 
+    def __init__(self, arg_parser=None, parsed_args=None, defaults=None):
         # get parser and parsed args from function arguments
         self.parser = arg_parser
         self.args = parsed_args if parsed_args is not None else ap.Namespace()
         filename = sys.argv[0].split("/")[-1].split(".")[0]
 
-        self.arglist = ['CNF_SILENT','CNF_DEBUG','CNF_VERBOSE','CNF_TMP','CNF_PRODUCTS']
+        self.arglist = [
+            "CNF_SILENT",
+            "CNF_DEBUG",
+            "CNF_VERBOSE",
+            "CNF_TMP",
+            "CNF_PRODUCTS",
+        ]
         # set default defaults
         self.defaults = {
-            'CNF_SILENT': False,
-            'CNF_DEBUG': False,
-            'CNF_VERBOSE': False,
-            'CNF_TMP': p.expanduser(f'~/work/{filename}'),
-            'CNF_PRODUCTS': p.expanduser(f'~/data/{filename}'),
+            "CNF_SILENT": False,
+            "CNF_DEBUG": False,
+            "CNF_VERBOSE": False,
+            "CNF_TMP": p.expanduser(f"~/work/{filename}"),
+            "CNF_PRODUCTS": p.expanduser(f"~/data/{filename}"),
         }
 
         # if defaults provided, overwrite default defaults with them,
         # but do it key by key, so keys that are not provided still
         # retain the default default.
-        if type(defaults) == 'dict':
+        if type(defaults) == "dict":
             for key in defaults.keys():
                 self.defaults[key] = defaults[key]
 
         # if provided defaults is not a dict, raise an error
         elif defaults is not None:
             raise TypeError(
                 "Env parser instantiation argument `defaults` must be a "
                 "dict. See init function docstring."
-                )
-
+            )
 
     def parse_env(self):
+        """Parses `run_app` env vars and sets the attached namespace variables based on them,
+        unless they were set by command line arguments."""
 
         # create list for bool args so they can be correctly set by env vars
         bools = []
 
         # fill the list of bool args with the arg variable (destination) names
         # but only if parser is present.
         if self.parser is not None:
-            for arg in self.parser.__dict__['_actions']:
+            for arg in self.parser.__dict__["_actions"]:
                 if type(arg) == ap._StoreTrueAction:
                     bools.append(arg.dest)
 
         # go over each arg
         for arg in self.arglist:
-
             # if command line argument exists
-            if getattr(self.args,arg,None) is not None:
+            if getattr(self.args, arg, None) is not None:
                 # let it be, let it be, there will be an answer, let it be
                 continue
 
             # if not, but environment variable exists
             elif os.getenv(arg):
                 # override the default value
 
                 # if it's one of the booleans, set True regardless of value (but
                 # ignore empty string too, just in case)
-                if arg in bools and getattr(self.args,arg) != '':
-                    setattr(self.args,arg,True)
+                if arg in bools and getattr(self.args, arg) != "":
+                    setattr(self.args, arg, True)
                 # otherwise use the value
-                setattr(self.args,arg,os.getenv(arg))
+                setattr(self.args, arg, os.getenv(arg))
 
             # if neither exists, use default
             else:
-                setattr(self.args,arg,self.defaults[arg])
+                setattr(self.args, arg, self.defaults[arg])
 
     def push_env(self):
+
+        """Propagates command line arguments from the attached argparse namespace to associated
+        environment variables."""
+
         # pushes args back to the env vars
         for arg in self.arglist:
             if arg in self.args.__dict__:
                 value = getattr(self.args, arg)
                 if value:
                     os.environ[arg] = str(getattr(self.args, arg))
                 elif not value:
                     os.environ.pop(arg, None)
             else:
-                setattr(self.args,arg,False)
-        
-########################################################################
-# region Default arg/config values
-# should mirror argument parser options if they're to have any defaults
-
-
-# endregion
-########################################################################
+                setattr(self.args, arg, False)
 
 
 ########################################################################
-# region Environment variable parser
+# region Verbosity handling and other printy stuff
 
-# Parses environment variables and makes sure that paths exist.
 
-# Only accepts env vars with a corresponding command line argument. When
-# adding env var options, please add a command line arg as well.
+class Loudmouth:
+    """An object that facilitates verbosity. It defines only one method,
+    :func:`Loudmouth.message`. The reason why this is not a module function is to namespace it, as
+    `message` is a pretty generic name.
 
+    Typical usage:
 
+    .. code:: python
 
-#endregion
-########################################################################
+        L = slither_app.Loudmouth(args)
 
+        L.message("This is some command line output generated by my program!")
+        L.message("something sinister is going on", "warning")
 
-########################################################################
-# region Verbosity handling and other printy stuff
+    where `args` is an argparse namespace object.
+    """
 
-class Loudmouth:
-    
-    def __init__(self,args):
-        
+    def __init__(self, args):
         self.args = args
 
-    def _message(self, message,severity=None):
-        """Prints messages to stdout.
+    def _message(self, message: str, severity: str = None):
+        """Prints messages to standard output. Includes date and
+        time, name of the app that issued it and the severity of the message, if provided.
+
+        :param message: The message body
+        :type message: str
+        :param severity: A string prepended to the message, in brackets, defaults to None
+        :type severity: str, optional
+        """
 
-        Args:
-            `message` (`str`): the message to print
-            `severity` (`str`, optional): Indicates the severity of the
-            message.
-            Either of: `'error'`, `'warning'`. Defaults to `''`.
+        stamp = dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+        severity_string = " " + severity.upper() + ":" if severity else ""
+        print(f"[{stamp}] grib_prep:{severity_string} {message}")
+
+        # define message function based on verbosity options
+        # nothing if silent, overrides all other verbosity
+
+    def message(self, message: str, severity: str = None):
+        """Prints messages to standard output, based on their severity values.
+
+        Messages are displayed with the following rules:
+            - **severity=None** - message displays only if verbosity or debug are enabled
+            - **severity='error'** - message displays unless silent is enabled
+            - **severity='warning'** - message displays unless silent is enabled
+            - **severity='debug'** - message displays only if debug is enabled
+
+        :param message: The message body
+        :type message: str
+        :param severity: A string which decides under which conditions (env vars or args) the message gets displayed, defaults to None, which only displays warnings and errors
+        :type severity: str, optional
         """
 
-        stamp = dt.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        severity_string = ' '+severity.upper()+':' if severity else ''
-        print(f'[{stamp}] grib_prep:{severity_string} {message}')
-
-    # define message function based on verbosity options
-    # nothing if silent, overrides all other verbosity
-    
-    def message(self, message, severity=None):
-        
         if self.args.CNF_SILENT:
             pass
-        
+
         # print everything, overrides verbose
         elif self.args.CNF_DEBUG:
             self._message(message, severity)
-            
+
         # print everything except debug messages if verbose
-        elif self.args.CNF_VERBOSE and severity != 'debug':
+        elif self.args.CNF_VERBOSE and severity != "debug":
             self._message(message, severity)
-            
+
         # only errors and warnings by default
         else:
-            if severity in ('error','warning'):
+            if severity in ("error", "warning"):
                 self._message(message, severity)
 
 
+class Loudmouth_dummy:
+    """Defines the message command so that it does nothing, this is necessary if
+    you use sphinx to generate docs. Having this dummy objects allows you to keep ``L.message``
+    scattered across your program even if you choose not to have an argparse.Namespace object with
+    parsed args present (which is the point when sphinx fails). The intended usage is:
+
+    .. code:: python
+
+        if __name__ == '__main__':
+            # create parser, parse args and create loudmouth
+            parser, args, L = slither_app.basic_init()
+        else:
+            # create fake loudmouth that does nothing
+            L = slither_app.Loudmouth_dummy()
+
+    This snippet creates the argument parser, parses the args and creates the regular
+    :class:`Loudmouth` if the app is run. If it's imported, no argument parser is created and the
+    dummy Loudmouth is instantiated instead of the regular one. Then all calls to ``L.message``
+    will do nothing, but they'll also not produce any error."""
+
+    def message(self):
+        """Does nothing."""
+        pass
+
+
 class Loudmouth_child(Loudmouth):
-    
+    """I forgot what this was for, so consider it deprecated, I guess."""
+
     def __init__(self):
-        
         self.envparser = Env_parser()
         self.envparser.parse_env()
         self.args = self.envparser.args
-    
+
+
 # endregion
-########################################################################
+########################################################################
+
+
+def basic_init():
+    """Creates an argument parser, parses env vars and creates a :class:`Loudmouth` instance.
+    Intended as a one-liner for when you don't need any additional arguments.
+
+    Typical usage:
+
+    .. code:: python
+
+        parser, args, L = slither_app.basic_init()
+
+    :return: (parser, args, loudmouth)
+    :rtype: (argparse.ArgumentParser, argparse.Namespace, :class:`Loudmouth()`)
+    """
+
+    # argument parser
+    parser, args = create_parser(parse_args=True)
+    # env parser
+    parser_env = Env_parser(parser, args)
+    parser_env.parse_env()
+    parser_env.push_env()
+    # verbosity handler
+    loudmouth = Loudmouth(args)
+
+    return parser, args, loudmouth
```

### Comparing `slither_app-0.0.7/src/slither_app.egg-info/PKG-INFO` & `slither_app-0.0.8/src/slither_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slither-app
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: Adam Otruba <adam.otruba@shmu.sk>
 License: DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE 
                             Version 2, December 2004 
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
```

