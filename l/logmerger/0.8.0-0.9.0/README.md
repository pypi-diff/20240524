# Comparing `tmp/logmerger-0.8.0.tar.gz` & `tmp/logmerger-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logmerger-0.8.0.tar", last modified: Thu Dec  7 09:12:43 2023, max compression
+gzip compressed data, was "logmerger-0.9.0.tar", last modified: Fri May 24 04:29:36 2024, max compression
```

## Comparing `logmerger-0.8.0.tar` & `logmerger-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-12-07 09:12:43.866082 logmerger-0.8.0/
--rw-rw-r--   0 paul      (1000) paul      (1000)     1069 2023-09-09 18:31:25.000000 logmerger-0.8.0/LICENSE
--rw-r--r--   0 paul      (1000) paul      (1000)     9703 2023-12-07 09:12:43.866082 logmerger-0.8.0/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     8484 2023-12-07 09:12:27.000000 logmerger-0.8.0/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-12-07 09:12:43.866082 logmerger-0.8.0/logmerger/
--rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-09-26 22:03:00.000000 logmerger-0.8.0/logmerger/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)       45 2023-09-26 22:03:00.000000 logmerger-0.8.0/logmerger/__main__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8779 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/about.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     4464 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/demo.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8675 2023-10-08 04:24:34.000000 logmerger-0.8.0/logmerger/file_reading.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    16466 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/interactive_viewing.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    13232 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/logmerger.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1603 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/merging.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3157 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/multiline_log_handler.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    14194 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/timestamp_wrapper.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-12-07 09:12:43.866082 logmerger-0.8.0/logmerger/tui/
--rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-09-26 22:03:00.000000 logmerger-0.8.0/logmerger/tui/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     5061 2023-12-07 09:12:27.000000 logmerger-0.8.0/logmerger/tui/dialogs.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1250 2023-09-26 22:03:00.000000 logmerger-0.8.0/logmerger/tui/validators.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-12-07 09:12:43.866082 logmerger-0.8.0/logmerger.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     9703 2023-12-07 09:12:43.000000 logmerger-0.8.0/logmerger.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      565 2023-12-07 09:12:43.000000 logmerger-0.8.0/logmerger.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-12-07 09:12:43.000000 logmerger-0.8.0/logmerger.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       55 2023-12-07 09:12:43.000000 logmerger-0.8.0/logmerger.egg-info/entry_points.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       41 2023-12-07 09:12:43.000000 logmerger-0.8.0/logmerger.egg-info/requires.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       10 2023-12-07 09:12:43.000000 logmerger-0.8.0/logmerger.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1240 2023-12-07 09:12:43.866082 logmerger-0.8.0/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-09-09 18:31:25.000000 logmerger-0.8.0/setup.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-24 04:29:36.462270 logmerger-0.9.0/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1069 2023-09-09 18:31:25.000000 logmerger-0.9.0/LICENSE
+-rw-r--r--   0 paul      (1000) paul      (1000)    10500 2024-05-24 04:29:36.462270 logmerger-0.9.0/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     9164 2024-05-23 14:45:55.000000 logmerger-0.9.0/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-24 04:29:36.462270 logmerger-0.9.0/logmerger/
+-rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-09-26 22:03:00.000000 logmerger-0.9.0/logmerger/__init__.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)       45 2023-09-26 22:03:00.000000 logmerger-0.9.0/logmerger/__main__.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     9407 2024-05-23 04:09:38.000000 logmerger-0.9.0/logmerger/about.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     4464 2023-12-07 09:12:27.000000 logmerger-0.9.0/logmerger/demo.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     8724 2024-05-23 04:09:38.000000 logmerger-0.9.0/logmerger/file_reading.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    17044 2024-05-23 04:09:38.000000 logmerger-0.9.0/logmerger/interactive_viewing.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    14938 2024-05-23 04:09:38.000000 logmerger-0.9.0/logmerger/logmerger.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1603 2023-12-07 09:12:27.000000 logmerger-0.9.0/logmerger/merging.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     3238 2024-05-23 04:09:38.000000 logmerger-0.9.0/logmerger/multiline_log_handler.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    15297 2024-05-23 04:09:38.000000 logmerger-0.9.0/logmerger/timestamp_wrapper.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-24 04:29:36.462270 logmerger-0.9.0/logmerger/tui/
+-rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-09-26 22:03:00.000000 logmerger-0.9.0/logmerger/tui/__init__.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     5061 2023-12-07 09:12:27.000000 logmerger-0.9.0/logmerger/tui/dialogs.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1250 2023-09-26 22:03:00.000000 logmerger-0.9.0/logmerger/tui/validators.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-05-24 04:29:36.462270 logmerger-0.9.0/logmerger.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)    10500 2024-05-24 04:29:36.000000 logmerger-0.9.0/logmerger.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      565 2024-05-24 04:29:36.000000 logmerger-0.9.0/logmerger.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2024-05-24 04:29:36.000000 logmerger-0.9.0/logmerger.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       55 2024-05-24 04:29:36.000000 logmerger-0.9.0/logmerger.egg-info/entry_points.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       96 2024-05-24 04:29:36.000000 logmerger-0.9.0/logmerger.egg-info/requires.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       10 2024-05-24 04:29:36.000000 logmerger-0.9.0/logmerger.egg-info/top_level.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1329 2024-05-24 04:29:36.462270 logmerger-0.9.0/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-09-09 18:31:25.000000 logmerger-0.9.0/setup.py
```

### Comparing `logmerger-0.8.0/LICENSE` & `logmerger-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logmerger-0.8.0/PKG-INFO` & `logmerger-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: logmerger
-Version: 0.8.0
+Version: 0.9.0
 Summary: A command-line utility to display multiple log files, merged by log timestamp
 Author: Paul McGuire
 Author-email: ptmcg.pm@gmail.com
 Project-URL: Source, https://github.com/ptmcg/logmerger
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: littletable
 Requires-Dist: rich
+Requires-Dist: typing-extensions>=4.12.0; python_version >= "3.13"
 Requires-Dist: textual
 Provides-Extra: pcap
 Requires-Dist: pyshark; extra == "pcap"
 
 # logmerger
 
 `logmerger` is a TUI for viewing a merged display of multiple log files, merged by timestamp.
@@ -43,15 +45,15 @@
 Something went wrong
 Traceback (last line is latest):
     sample.py: line 32
         divide(100, 0)
     sample.py: line 8
         return a / b
 ZeroDivisionError: division by zero
-2023-07-14 08:00:06 INFO   User authentication succeeded
+2023-07-14 08:00:06 INFO   User authentication failed
 2023-07-14 08:00:08 DEBUG  Starting data synchronization
 2023-07-14 08:00:11 INFO   Processing incoming request
 ```
 
 ```
 # log2.txt
 2023-07-14 08:00:01 INFO   Request processed successfully
@@ -86,15 +88,15 @@
                              Traceback (last line is latest):
                                  sample.py: line 32
                                      divide(100, 0)
                                  sample.py: line 8
                                      return a / b
                              ZeroDivisionError: division by zero                           
   2023-07-14 08:00:06.000   INFO   User authentication            DEBUG  Starting data
-                            succeeded                             synchronization
+                            failed                                synchronization
   2023-07-14 08:00:08.000   DEBUG  Starting data                  INFO   Processing incoming request
                             synchronization
   2023-07-14 08:00:11.000   INFO   Processing incoming request    DEBUG  Performing database backup
                             INFO   Processing incoming request
                             (a little more...)
   2023-07-14 08:00:14.000   DEBUG  Performing database backup     WARN   Invalid input received:
                                                                   missing required field
@@ -116,17 +118,19 @@
 
 ## Command line arguments
 
 `logmerger -h` will show the following help:
 
 ```
 usage: logmerger [-h] [--interactive] [--inline] [--output OUTPUT]
-                 [--start START] [--end END] [--width WIDTH]
-                 [--line_numbers] [--csv CSV] [--encoding ENCODING]
-                 [--timestamp_format [TIMESTAMP_FORMATS ...]] [--demo]
+                 [--start START] [--end END] [--autoclip]
+                 [--width WIDTH] [--line_numbers] [--show_clock]
+                 [--csv CSV] [--encoding ENCODING]
+                 [--timestamp_format [TIMESTAMP_FORMATS ...]]
+                 [--demo]
                  [files ...]
 
 positional arguments:
   files                 log files to be merged
 
 options:
   -h, --help            show this help message and exit
@@ -134,18 +138,20 @@
   --inline              show merged log data as inline merge
   --output OUTPUT, -o OUTPUT
                         save merged output to file ('-' for stdout; files ending in '.md' are saved
                         using Markdown)
   --start START, -s START
                         start time to select time window for merging logs
   --end END, -e END     end time to select time window for merging logs
+  --autoclip, -ac       clip merging to time range of logs in first log file
   --width WIDTH, -w WIDTH
                         total screen width to use for interactive mode (defaults to current screen
                         width)
   --line_numbers, -ln   add line number column
+  --show_clock, -clock  show running clock in header
   --csv CSV, -csv CSV   save merged logs to CSV file
   --encoding ENCODING, -enc ENCODING
                         encoding to use when reading log files (defaults to the system default encoding)
   --timestamp_format [TIMESTAMP_FORMATS ...]
                         custom timestamp format
   --demo                Run interactive demo
   
@@ -175,22 +181,31 @@
 
 
 ## Merging
 
 Log files get merged by interleaving log lines from each based on timestamps in each log line. `logmerger` tries to 
 use different timestamp formats until it finds a matching format for each input file. The supported formats are:
 
-| format                       | description                                                                                         |
-|------------------------------|-----------------------------------------------------------------------------------------------------|
-| `YYYY-MM-DD HH:MM:SS,SSS`    | date+time to milliseconds, with ',' decimal (default for Python's `asctime` log marker)             |
-| `YYYY-MM-DD HH:MM:SS.SSS`    | date+time to milliseconds, with '.' decimal                                                         |
-| `YYYY-MM-DD HH:MM:SS`        | date+time to seconds                                                                                |
-| `YYYY-MM-DDTHH:MM:SS,SSS`    | date+T+time to milliseconds, with ',' decimal                                                       |
-| `YYYY-MM-DDTHH:MM:SS.SSS`    | date+T+time to milliseconds, with '.' decimal                                                       |
-| `YYYY-MM-DDTHH:MM:SS`        | date+T+time to seconds                                                                              |
-| `Jan DD HH:MM:SS`            | month/day + time (timestamp in syslog files); year is inferred from the create date of the log file |
-| `DD/Jan/YYYY HH:MM:SS`       | day/month/year + time                                                                               |
-| `DD/Jan/YYYY:HH:MM:SS ±ZZZZ` | day/month/year + time + timezone offset (converts timestamps to local time)                         |
+| format                       | description                                                                                           |
+|------------------------------|-------------------------------------------------------------------------------------------------------|
+| `YYYY-MM-DD HH:MM:SS,SSS`    | date+time to milliseconds, with ',' decimal (default for Python's `asctime` log marker)               |
+| `YYYY-MM-DD HH:MM:SS.SSS`    | date+time to milliseconds, with '.' decimal                                                           |
+| `YYYY-MM-DD HH:MM:SS`        | date+time to seconds                                                                                  |
+| `YYYY-MM-DDTHH:MM:SS,SSS`    | date+T+time to milliseconds, with ',' decimal                                                         |
+| `YYYY-MM-DDTHH:MM:SS.SSS`    | date+T+time to milliseconds, with '.' decimal                                                         |
+| `YYYY-MM-DDTHH:MM:SS`        | date+T+time to seconds                                                                                |
+| `Jan DD HH:MM:SS`            | month/day + time (timestamp in syslog files); year is inferred from the create date of the log file   |
+| `DD/Jan/YYYY HH:MM:SS`       | day/month/year + time                                                                                 |
+| `DD/Jan/YYYY:HH:MM:SS ±ZZZZ` | day/month/year + time + timezone offset (converts timestamps to local time)                           |
+| `HH:MM:SS.SSSSSS`            | hour/minute/second (timestamp in strace files); date is inferred from the create date of the log file |
+| `strace`                     | uses HH:MM:SS.SSSSSS format with leading process id integer                                           |
 
 
 Untimestamped log lines that contain multiple lines (such as a traceback) get combined with the previous timestamped
 line (see in the example above).
+
+
+## Security contact information
+
+To report a security vulnerability, please use the
+[Tidelift security contact](https://tidelift.com/security).
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `logmerger-0.8.0/README.md` & `logmerger-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Something went wrong
 Traceback (last line is latest):
     sample.py: line 32
         divide(100, 0)
     sample.py: line 8
         return a / b
 ZeroDivisionError: division by zero
-2023-07-14 08:00:06 INFO   User authentication succeeded
+2023-07-14 08:00:06 INFO   User authentication failed
 2023-07-14 08:00:08 DEBUG  Starting data synchronization
 2023-07-14 08:00:11 INFO   Processing incoming request
 ```
 
 ```
 # log2.txt
 2023-07-14 08:00:01 INFO   Request processed successfully
@@ -54,15 +54,15 @@
                              Traceback (last line is latest):
                                  sample.py: line 32
                                      divide(100, 0)
                                  sample.py: line 8
                                      return a / b
                              ZeroDivisionError: division by zero                           
   2023-07-14 08:00:06.000   INFO   User authentication            DEBUG  Starting data
-                            succeeded                             synchronization
+                            failed                                synchronization
   2023-07-14 08:00:08.000   DEBUG  Starting data                  INFO   Processing incoming request
                             synchronization
   2023-07-14 08:00:11.000   INFO   Processing incoming request    DEBUG  Performing database backup
                             INFO   Processing incoming request
                             (a little more...)
   2023-07-14 08:00:14.000   DEBUG  Performing database backup     WARN   Invalid input received:
                                                                   missing required field
@@ -84,17 +84,19 @@
 
 ## Command line arguments
 
 `logmerger -h` will show the following help:
 
 ```
 usage: logmerger [-h] [--interactive] [--inline] [--output OUTPUT]
-                 [--start START] [--end END] [--width WIDTH]
-                 [--line_numbers] [--csv CSV] [--encoding ENCODING]
-                 [--timestamp_format [TIMESTAMP_FORMATS ...]] [--demo]
+                 [--start START] [--end END] [--autoclip]
+                 [--width WIDTH] [--line_numbers] [--show_clock]
+                 [--csv CSV] [--encoding ENCODING]
+                 [--timestamp_format [TIMESTAMP_FORMATS ...]]
+                 [--demo]
                  [files ...]
 
 positional arguments:
   files                 log files to be merged
 
 options:
   -h, --help            show this help message and exit
@@ -102,18 +104,20 @@
   --inline              show merged log data as inline merge
   --output OUTPUT, -o OUTPUT
                         save merged output to file ('-' for stdout; files ending in '.md' are saved
                         using Markdown)
   --start START, -s START
                         start time to select time window for merging logs
   --end END, -e END     end time to select time window for merging logs
+  --autoclip, -ac       clip merging to time range of logs in first log file
   --width WIDTH, -w WIDTH
                         total screen width to use for interactive mode (defaults to current screen
                         width)
   --line_numbers, -ln   add line number column
+  --show_clock, -clock  show running clock in header
   --csv CSV, -csv CSV   save merged logs to CSV file
   --encoding ENCODING, -enc ENCODING
                         encoding to use when reading log files (defaults to the system default encoding)
   --timestamp_format [TIMESTAMP_FORMATS ...]
                         custom timestamp format
   --demo                Run interactive demo
   
@@ -143,22 +147,31 @@
 
 
 ## Merging
 
 Log files get merged by interleaving log lines from each based on timestamps in each log line. `logmerger` tries to 
 use different timestamp formats until it finds a matching format for each input file. The supported formats are:
 
-| format                       | description                                                                                         |
-|------------------------------|-----------------------------------------------------------------------------------------------------|
-| `YYYY-MM-DD HH:MM:SS,SSS`    | date+time to milliseconds, with ',' decimal (default for Python's `asctime` log marker)             |
-| `YYYY-MM-DD HH:MM:SS.SSS`    | date+time to milliseconds, with '.' decimal                                                         |
-| `YYYY-MM-DD HH:MM:SS`        | date+time to seconds                                                                                |
-| `YYYY-MM-DDTHH:MM:SS,SSS`    | date+T+time to milliseconds, with ',' decimal                                                       |
-| `YYYY-MM-DDTHH:MM:SS.SSS`    | date+T+time to milliseconds, with '.' decimal                                                       |
-| `YYYY-MM-DDTHH:MM:SS`        | date+T+time to seconds                                                                              |
-| `Jan DD HH:MM:SS`            | month/day + time (timestamp in syslog files); year is inferred from the create date of the log file |
-| `DD/Jan/YYYY HH:MM:SS`       | day/month/year + time                                                                               |
-| `DD/Jan/YYYY:HH:MM:SS ±ZZZZ` | day/month/year + time + timezone offset (converts timestamps to local time)                         |
+| format                       | description                                                                                           |
+|------------------------------|-------------------------------------------------------------------------------------------------------|
+| `YYYY-MM-DD HH:MM:SS,SSS`    | date+time to milliseconds, with ',' decimal (default for Python's `asctime` log marker)               |
+| `YYYY-MM-DD HH:MM:SS.SSS`    | date+time to milliseconds, with '.' decimal                                                           |
+| `YYYY-MM-DD HH:MM:SS`        | date+time to seconds                                                                                  |
+| `YYYY-MM-DDTHH:MM:SS,SSS`    | date+T+time to milliseconds, with ',' decimal                                                         |
+| `YYYY-MM-DDTHH:MM:SS.SSS`    | date+T+time to milliseconds, with '.' decimal                                                         |
+| `YYYY-MM-DDTHH:MM:SS`        | date+T+time to seconds                                                                                |
+| `Jan DD HH:MM:SS`            | month/day + time (timestamp in syslog files); year is inferred from the create date of the log file   |
+| `DD/Jan/YYYY HH:MM:SS`       | day/month/year + time                                                                                 |
+| `DD/Jan/YYYY:HH:MM:SS ±ZZZZ` | day/month/year + time + timezone offset (converts timestamps to local time)                           |
+| `HH:MM:SS.SSSSSS`            | hour/minute/second (timestamp in strace files); date is inferred from the create date of the log file |
+| `strace`                     | uses HH:MM:SS.SSSSSS format with leading process id integer                                           |
 
 
 Untimestamped log lines that contain multiple lines (such as a traceback) get combined with the previous timestamped
 line (see in the example above).
+
+
+## Security contact information
+
+To report a security vulnerability, please use the
+[Tidelift security contact](https://tidelift.com/security).
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `logmerger-0.8.0/logmerger/about.py` & `logmerger-0.9.0/logmerger/about.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 The `logmerger` utility provides a view of one or more log files, merged by timestamps found in those files. It is 
 helpful when analyzing interactions between separate programs by viewing their individual log files side-by-side, in
 timestamp order.
 
 In practice, log files often use various formats for their log timestamps. `logmerger` looks for several 
 standard timestamp formats, at the start of each line of the log file:
 
-| Format                     | Description                                                                    |
-|----------------------------|--------------------------------------------------------------------------------|
-| YYYY-MM-DD HH:MM:SS,SSS    | date and time with milliseconds (, decimal) (defaut Python asctime log format) |
-| YYYY-MM-DD HH:MM:SS.SSS    | date and time with milliseconds (. decimal)                                    |
-| YYYY-MM-DD HH:MM:SS        | date and time                                                                  |
-| 0000000000.000000          | float seconds since epoch                                                      |
-| 0000000000000              | milliseconds since epoch                                                       |
-| 0000000000                 | integer seconds since epoch                                                    |
+| Format                     | Description                                                                     |
+|----------------------------|---------------------------------------------------------------------------------|
+| YYYY-MM-DD HH:MM:SS,SSS    | date and time with milliseconds (, decimal) (default Python asctime log format) |
+| YYYY-MM-DD HH:MM:SS.SSS    | date and time with milliseconds (. decimal)                                     |
+| YYYY-MM-DD HH:MM:SS        | date and time                                                                   |
+| 0000000000.000000          | float seconds since epoch                                                       |
+| 0000000000000              | milliseconds since epoch                                                        |
+| 0000000000                 | integer seconds since epoch                                                     |
+| HH:MM:SS.SSSSSS            | timestamp with milliseconds (strace format)                                     |
 | Jan DD HH:MM:SS            | month + day + time (timestamp in syslog files); year is inferred from the create date of the log file |
-| DD/Jan/YYYY HH:MM:SS       | day/month/year + time                                                          |
-| DD/Jan/YYYY:HH:MM:SS ±ZZZZ | day/month/year : time + timezone offset (converts to local time)               |
+| DD/Jan/YYYY HH:MM:SS       | day/month/year + time                                                           |
+| DD/Jan/YYYY:HH:MM:SS ±ZZZZ | day/month/year : time + timezone offset (converts to local time)                |
+| strace                     | uses HH:MM:SS.SSSSSS format with leading process id integer                     |
 
 For log files that do not have the timestamp at the start of the line, you can define a custom format using
 the command line option `--timestamp_format`.  See `Custom timestamp formats` below.
 
 ## Interactive functions
 
 The interactive mode of `logmerger` defines several keystroke navigation commands:
@@ -32,14 +34,15 @@
 | ^D  | Toggle dark/light mode                                                                                                     |
 |  J  | Jump by line count or time interval                                                                                        |
 |  F  | Prompt for search string and advance to first line containing that string (case-insensitive)                               |
 |  N  | Advance (to next instance of the search string or by current jump interval)                                                |
 |  P  | Move back (to previous instance of the search string or by current jump interval)                                          |
 |  L  | Prompt for line number to move cursor to (if line number > total number of merged lines, advances to end)                  |
 |  T  | Prompt for timestamp to move cursor to (if no log message at the exact timestamp, will move to first line after timestamp) |
+|  S  | Capture a screenshot of the current visible screen                                                                         |
 |  H  | Display this helpful text                                                                                                  |
 |  Q  | Quit                                                                                                                       |
 
 When using the Jump command, enter an integer number followed by "l", "us", "ms", "s", "m", "h", or "d", to indicate whether jumping
 by number of lines, microseconds, milliseconds, seconds, minutes, hours, or days. Then press N and P to advance or go back by your jump interval.
 For example:
 
@@ -50,26 +53,28 @@
 the current line, advancing will jump to the next timestamp after the computed target time,
 reversing will jump to the next timestamp before the computed target time.
 
 ## Command line options
 
 The command to run `logmerger` accepts several options, followed by one or more file names:
 
-| Option              | Description                                                                                      |
-|---------------------|--------------------------------------------------------------------------------------------------|
-| --interactive, -i   | display in interactive mode (default)                                                            |
-| --inline            | display interactive merged content into a single inline column (only supported in interactive mode) (default is side-by-side) |
-| --output, -o        | save output to file ('-' for stdout; files ending in `.md` are saved using Markdown)             |
-| --width, -w         | total display width - if greater than the screen width, will display with a horizontal scrollbar |
-| --line_numbers, -ln | display with a leading line number column                                                        |
-| --start, -s         | start time for merging logs                                                                      |
-| --end, -e           | end time for merging logs                                                                        |
-| --csv               | output merged logs as CSV                                                                        |
-| --timestamp_format  | define one or more custom formats for log file timestamps                                        |
-| --demo              | run logmerger with simulated log file content (in either text or interactive modes)              |
+| Option               | Description                                                                                      |
+|----------------------|--------------------------------------------------------------------------------------------------|
+| --interactive, -i    | display in interactive mode (default)                                                            |
+| --inline             | display interactive merged content into a single inline column (only supported in interactive mode) (default is side-by-side) |
+| --output, -o         | save output to file ('-' for stdout; files ending in `.md` are saved using Markdown)             |
+| --width, -w          | total display width - if greater than the screen width, will display with a horizontal scrollbar |
+| --line_numbers, -ln  | display with a leading line number column                                                        |
+| --show_clock, -clock | show running clock in header                                                                     |
+| --start, -s          | start time for merging logs                                                                      |
+| --end, -e            | end time for merging logs                                                                        |
+| --autoclip, -ac      | clip start and end times from logs in first log file                                             |
+| --csv                | output merged logs as CSV                                                                        |
+| --timestamp_format   | define one or more custom formats for log file timestamps                                        |
+| --demo               | run logmerger with simulated log file content (in either text or interactive modes)              |
 
 
 ## Usage tips
 
 ### Use `logmerger` with a single log file
 
 You can use `logmerger` even with just a single log file to make use of `logmerger`'s interactive viewing or
@@ -85,15 +90,14 @@
 - text log files that have been gzip compressed (such as those created by logrotate)
   - (filename ending in `.gz`)
 - CSV files (timestamp is read from first data column)
   - (filename ending in `.csv`)
 - packet capture files, created using tcpdump or WireShark (experimental)
   - (filename ending in `.pcap`)
 
-
 ### Multi-line logs
 
 Some logs may contain messages that extend beyond a single line, or are followed by untimestamped lines
 (such as JSON data or an exception with traceback). `logmerger` detects these lines and groups them with the
 previous timestamped line.
 
 
@@ -142,15 +146,15 @@
 | INFO - 2022-01-01 12:34:56 log message      | (&#92;w+ - )((...) )   |
 | [INFO] 2022-01-01 12:34:56 log message      | (&#92;[&#92;w+&#92;] )((...) ) |
 | [2022-01-01 12:34:56&#124;INFO] log message | (&#92;[)((...)&#92;&#124;)  |
 
 
 ## About logmerger
 
-logmerger version 0.8.0
+logmerger version 0.9.0
 
-by Paul McGuire, 2023
+by Paul McGuire, 2024
 
 MIT License
 
 GitHub: `https://github.com/ptmcg/logmerger`
 """  # noqa
```

### Comparing `logmerger-0.8.0/logmerger/demo.py` & `logmerger-0.9.0/logmerger/demo.py`

 * *Files identical despite different names*

### Comparing `logmerger-0.8.0/logmerger/file_reading.py` & `logmerger-0.9.0/logmerger/file_reading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from __future__ import annotations
 
 import abc
 import operator
 import types
 
 
-class FileReader:
+class FileReader(abc.ABC):
+    """
+    Abstract base class for file readers.
+    """
     @classmethod
     def get_reader(cls, name: str, encoding: str) -> FileReader:
+        """
+        Method to iterate over defined subclasses to find the appropriate
+        reader for the given filename.
+        """
         for subcls in cls.__subclasses__():
             if subcls is TextFileReader:
                 continue
             if subcls._can_read(name):
                 return subcls(name, encoding)
         return TextFileReader(name, encoding)
 
@@ -28,21 +35,14 @@
         self.file_name = file_name
         self.encoding = encoding
         self._iter = iter(())
 
     def __iter__(self):
         return self._iter
 
-    def __next__(self):
-        try:
-            return next(self._iter)
-        except StopIteration:
-            self._close_reader()
-            raise
-
 
 class TextFileReader(FileReader):
     @classmethod
     def _can_read(cls, fname: str) -> bool:
         return True
 
     def __init__(self, fname: str, encoding: str):
```

### Comparing `logmerger-0.8.0/logmerger/interactive_viewing.py` & `logmerger-0.9.0/logmerger/interactive_viewing.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import littletable as lt
 from rich.text import Text
 from textual import work
 from textual.app import App, ComposeResult
 from textual.binding import Binding
 from textual.validation import Integer
-from textual.widgets import DataTable, Footer
+from textual.widgets import DataTable, Footer, Header
 
 from logmerger.tui.dialogs import ModalInputDialog, ModalAboutDialog, ModalJumpDialog
 from logmerger.tui.validators import TimestampValidator
 
 
 def _max_line_count(sseq: list[str]) -> int:
     """
@@ -70,32 +70,34 @@
     """
     Class to display merged results using textual TUI.
     """
     TITLE = "logmerger"
 
     BINDINGS = [
         Binding(key="q", action="quit", description="Quit"),
-        Binding(key="ctrl+d", action="toggle_dark", description="Toggle Dark Mode"),
+        Binding(key="ctrl+d", action="toggle_dark", description="Toggle Dark Mode", show=False),
         Binding(key="j", action="jump", description="Jump"),
         Binding(key="f", action="find", description="Find"),
         Binding(key="n", action="find_next", description="Next"),
         Binding(key="p", action="find_prev", description="Prev"),
         Binding(key="l", action="goto_line", description="Go to line"),
         Binding(key="t", action="goto_timestamp", description="Go to timestamp"),
+        Binding(key="s", action="screenshot", description="Screenshot"),
         Binding(key="h", action="help_about", description="Help/About"),
     ]
 
     def __init__(self, *args, **kwargs):
         from logmerger.logmerger import parse_time_using, VALID_INPUT_TIME_FORMATS
 
         super().__init__(*args, **kwargs)
         self.log_file_names: list[str] = []
         self.merged_log_lines_table: lt.Table = None  # noqa
         self.display_width: int = 0
         self.show_line_numbers: bool = False
+        self.show_clock: bool = False
         self.show_merged_logs_inline: bool = False
         self.current_search_string: str = ""
         self.current_jump: Jump = None  # noqa
         self.current_goto_timestamp_string: str = ""
         self.timestamp_validator = TimestampValidator(
             timestamp_parser=partial(parse_time_using, formats=VALID_INPUT_TIME_FORMATS),
         )
@@ -104,22 +106,26 @@
             self,
             *,
             log_file_names: list[str],
             display_width: int,
             show_line_numbers: bool,
             merged_log_lines_table: lt.Table,
             show_merged_logs_inline: bool,
+            show_clock: bool,
     ) -> None:
         self.log_file_names = log_file_names
         self.merged_log_lines_table = merged_log_lines_table
         self.display_width = display_width
         self.show_line_numbers = show_line_numbers
         self.show_merged_logs_inline = show_merged_logs_inline
+        self.show_clock = show_clock
 
     def compose(self) -> ComposeResult:
+        if self.show_clock:
+            yield Header(show_clock=True)
         yield DataTable()
         yield Footer()
 
     def on_mount(self) -> None:
         if self.show_merged_logs_inline:
             self.load_data_inline()
         else:
@@ -178,15 +184,15 @@
                 if self.show_line_numbers else wrapped_row_values[0],
                 *wrapped_row_values[1:],
                 height=_max_line_count(wrapped_row_values))
 
         elapsed = time.time() - start
         if elapsed > 10:
             self.bell()
-            self.notify("Log data complete")
+            self.notify("Log data loading complete")
 
     @work
     async def load_data_inline(self):
         fixed_cols = 2 if self.show_line_numbers else 1
         file_names = self.merged_log_lines_table.info()["fields"]
 
         display_table = self.query_one(DataTable)
@@ -251,15 +257,15 @@
                 *wrapped_row_values[1:],
                 height=_max_line_count(wrapped_row_values),
             )
 
         elapsed = time.time() - start
         if elapsed > 10:
             self.bell()
-            self.notify("Log data complete")
+            self.notify("Log data loading complete")
 
     #
     # methods to support go to find/next/prev search functions
     #
 
     def action_find(self) -> None:
         self.app.push_screen(
@@ -442,14 +448,25 @@
                 r"Jump (#\[lsmhd]):",
                 initial=self.current_jump.as_string() if self.current_jump else "",
             ),
             self.save_jump_and_jump
         )
 
     #
+    # methods to support screenshotting
+    #
+
+    def action_screenshot(self) -> None:
+        now = datetime.now()
+        filename = self.app.save_screenshot(
+            f"logmerger_{now:%Y%m%d_%H%M%S}_screenshot.svg"
+        )
+        self.notify(f"Screenshot saved to {filename}")
+
+    #
     # methods to support help/about
     #
 
     def action_help_about(self) -> None:
         from logmerger.about import text
 
         self.app.push_screen(
```

### Comparing `logmerger-0.8.0/logmerger/logmerger.py` & `logmerger-0.9.0/logmerger/logmerger.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 T = TypeVar("T")
 try:
     from typing import Never
 except ImportError:
     from typing import NoReturn as Never
 
 
-def make_argument_parser():
+def make_argument_parser() -> argparse.ArgumentParser:
     epilog_notes = """
     Start and end timestamps to clip the given files to a particular time window can be 
     given in `YYYY-MM-DD HH:MM:SS.SSS` format, with trailing milliseconds and seconds
     optional, and "," permissible for the decimal point. A "T" can be included between
     the date and time to simplify entering the timestamp on a command line 
     (otherwise would require enclosing in quotes because of the intervening space). These
     command line values do not need to match the timestamp formats in the log files.
@@ -65,21 +65,25 @@
     parser.add_argument(
         "--output", "-o",
         # type=argparse.FileType('w'),
         help="save merged output to file ('-' for stdout; files ending in '.md' are saved using Markdown)",
     )
     parser.add_argument('--start', '-s', required=False, help="start time to select time window for merging logs")
     parser.add_argument('--end', '-e', required=False, help="end time to select time window for merging logs")
+    parser.add_argument("--autoclip", "-ac",
+                        action="store_true",
+                        help="clip merging to time range of logs in first log file")
     parser.add_argument(
         "--width", "-w",
         type=int,
         help="total screen width to use for interactive mode (defaults to current screen width)",
         default=0
     )
     parser.add_argument("--line_numbers", "-ln", action="store_true", help="add line number column")
+    parser.add_argument("--show_clock", "-clock", action="store_true", help="show running clock in header")
     parser.add_argument("--csv", "-csv", help="save merged logs to CSV file")
     parser.add_argument(
         "--encoding", "-enc",
         type=str,
         default=sys.getfilesystemencoding(),
         help="encoding to use when reading log files (defaults to the system default encoding)")
     parser.add_argument("--timestamp_format",
@@ -103,71 +107,85 @@
     "%Y-%m-%dT%H:%M:%S",
     "%Y-%m-%dT%H:%M",
     "%Y-%m-%d",
 ]
 
 
 def parse_time_using(ts_str: str, formats: Union[str, list[str]]) -> datetime:
+    """
+    Given a timestamp string of unknown format, try parsing it against
+    a format or list of formats.
+    """
     if not isinstance(formats, (list, tuple)):
         formats = [formats]
     for fmt in formats:
         try:
             return datetime.strptime(ts_str, fmt)
         except ValueError:
             pass
+
     raise ValueError(f"no matching format for input string {ts_str!r}")
 
 
 def parse_relative_time(ts_str: str) -> datetime:
+    """
+    Given a string representing a relative timestamp of an integer
+    followed by "s", "m", "h", or "d", return a datetime object that
+    many seconds, minutes, hours, or days in the past.
+    """
     parts = re.match(r"(\d+)([smhd])$", ts_str, flags=re.IGNORECASE)
-    if parts:
-        qty, unit = parts.groups()
-        seconds = int(qty)
-        now = datetime.now()
-        for unit_type, mult in [("s", 1), ("m", 60), ("h", 60), ("d", 24)]:
-            seconds *= mult
-            if unit == unit_type:
-                return now - timedelta(seconds=seconds)
+    if parts is None:
+        raise ValueError(f"invalid relative time string {ts_str!r}")
 
-    raise ValueError(f"invalid relative time string {ts_str!r}")
+    qty, unit = parts.groups()
+    seconds = int(qty)
+    now = datetime.now()
+    for unit_type, mult in [("s", 1), ("m", 60), ("h", 60), ("d", 24)]:
+        seconds *= mult
+        if unit == unit_type:
+            return now - timedelta(seconds=seconds)
 
 
-def label(s: str, seq: Iterable[T]) -> Generator[tuple[str, T], None, None]:
-    """
-    method to make each item of an Iterable into a tuple containing the
-    label (so that as items from different iterators are later combined, we'll know
-    which iterator a particular item came from)
-    """
-    yield from ((s, obj) for obj in seq)
+
+def label(s: str):
+    def _inner(seq: Iterable[T]) -> Generator[tuple[str, T], None, None]:
+        """
+        method to make each item of an Iterable into a tuple containing the
+        label (so that as items from different iterators are later combined, we'll know
+        which iterator a particular item came from)
+        """
+        yield from ((s, obj) for obj in seq)
+    return _inner
 
 
 class LogMergerApplication:
     def __init__(self, config: argparse.Namespace):
         self.config = config
 
         if config.timestamp_formats:
             formats = sum(config.timestamp_formats, [])
             for ts_format in formats:
                 TimestampedLineTransformer.make_custom_transformers(ts_format)
 
         self.file_names = config.files
         self.total_width = config.width
+        self.autoclip = config.autoclip
 
         if config.start is None:
             self.start_time = datetime.min
         else:
             if config.start.endswith(("s", "m", "h", "d")):
                 self.start_time = parse_relative_time(config.start)
             else:
                 self.start_time = parse_time_using(config.start, VALID_INPUT_TIME_FORMATS)
 
         if config.end is None:
             self.end_time = datetime.max
         else:
-            if config.end.endswith(tuple("smhd")):
+            if config.end.endswith(("s", "m", "h", "d")):
                 self.end_time = parse_relative_time(config.end)
             else:
                 self.end_time = parse_time_using(config.end, VALID_INPUT_TIME_FORMATS)
 
         if self.end_time <= self.start_time:
             raise ValueError("invalid start/end times - start must be before end")
 
@@ -252,32 +270,54 @@
 
         # scan input files to determine timestamp format, and create appropriate transformer for each
         readers = [FileReader.get_reader(fname, self.encoding) for fname in self.file_names]
         peek_iters, readers = zip(*[itertools.tee(rdr) for rdr in readers])
         transformers = [TimestampedLineTransformer.make_transformer_from_sample_line(next(peek_iter))
                         for peek_iter in peek_iters]
 
+        if self.autoclip:
+            clip_peek, rdr0 = itertools.tee(readers[0])
+            readers = (rdr0, *readers[1:])
+            peek_transformer = transformers[0]
+            for peek_line in clip_peek:
+                first_ts, _ = peek_transformer(peek_line)
+                if first_ts is not None:
+                    break
+            else:
+                raise ValueError(f"no timestamps found in log file {self.file_names[0]!r}")
+
+            self.start_time = self.end_time = first_ts
+            for ts, _ in (peek_transformer(line) for line in clip_peek):
+                if ts is None:
+                    continue
+                if ts > self.end_time:
+                    self.end_time = ts
+                elif ts < self.start_time:
+                    self.start_time = ts
+            self.time_clip = self._time_clip_early_exit
+
         # build iterators over each file that:
         # - transform each line into a (datetime, str) tuple (where the str is everything after the
         #   timestamp, so that it doesn't get repeated in the output table)
         # - collapses multiline logs (lines that go beyond just one line, with subsequent lines that
         #   do not start with a timestamp - tracebacks are a common example)
         # - labels each item with its source filename (so that after pulling an entry for the heap, we
         #   know which file it came from)
         # (for background on why we must use map() instead of a generator expression,
         # see https://chat.stackoverflow.com/transcript/message/56645472#56645472)
+
+        # create a nested iterator for each log file to read, rstrip, transform, clip,
+        # collapse, and label each log line
         log_file_line_iters = [
-            (
-                label(
-                    fname,
-                    MultilineLogCollapser(self.time_clip)(
-                        filter(self._raw_time_clip, map(xformer, map(str.rstrip, reader)))
-                    )
+            label(fname)(
+                MultilineLogCollapser(self.time_clip)(
+                    filter(self._raw_time_clip, map(xformer, map(str.rstrip, reader)))
                 )
-            ) for fname, xformer, reader in zip(self.file_names, transformers, readers)
+            )
+            for fname, xformer, reader in zip(self.file_names, transformers, readers)
         ]
 
         # use the Merger class which internally uses a heap to pull values in timestamp order from
         # all the iterators, and then uses groupby to group them by common timestamp
         merger = Merger(log_file_line_iters, key_function=lambda log_data: log_data[1][0])
 
         if self.config.line_numbers:
@@ -316,14 +356,15 @@
         app = InteractiveLogMergeViewerApp()
         app.config(
             log_file_names=self.file_names,
             display_width=self.total_width,
             show_line_numbers=self.config.line_numbers,
             merged_log_lines_table=merged_log_lines,
             show_merged_logs_inline=self.config.inline,
+            show_clock=self.config.show_clock,
         )
         app.run()
 
 
 def main():
 
     parser = make_argument_parser()
```

### Comparing `logmerger-0.8.0/logmerger/merging.py` & `logmerger-0.9.0/logmerger/merging.py`

 * *Files identical despite different names*

### Comparing `logmerger-0.8.0/logmerger/multiline_log_handler.py` & `logmerger-0.9.0/logmerger/multiline_log_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,18 +53,20 @@
     Class to take an iterable of (datetime, str) tuples, and use itertools.groupby to
     merge consecutive log lines for a given datetime into one.
 
     Converts:
         2023-07-14 08:00:04 ERROR  Request processed unsuccessfully
         Something went wrong
         Traceback (last line is latest):
-            blah
-            blah
-        ValueError("shouldn't have done that")
-        2023-07-14 08:00:06 INFO   User authentication succeeded
+            sample.py: line 32
+                divide(100, 0)
+            sample.py: line 8
+                return a / b
+        ZeroDivisionError: division by zero
+        2023-07-14 08:00:06 INFO   User authentication failed
 
     to two log entries.
     """
     def __init__(self, time_filter: Optional[Callable[[datetime], bool]] = None):
         self._newlogline_detector = NewLogLineDetector()
         self._time_filter_fn = time_filter or (lambda x: True)
```

### Comparing `logmerger-0.8.0/logmerger/timestamp_wrapper.py` & `logmerger-0.9.0/logmerger/timestamp_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 
             Log line                                  Template
             INFO - 2022-01-01 12:34:56 log message    (\w+ - )((...) )
             [INFO] 2022-01-01 12:34:56 log message    (\[\w+\] )((...) )
             [2022-01-01 12:34:56|INFO] log message    (\[)((...)|)
 
         """
+        if custom_timestamp.lower() == "strace":
+            custom_timestamp = r"(\d+) ((...))"
 
         # template must include "(...)" placeholder somewhere
         if "(...)" not in custom_timestamp:
             raise ValueError(f"custom timestamp format '{custom_timestamp}' must contain '(...)' placeholder")
 
         has_initial_content = "..." not in custom_timestamp[:custom_timestamp.find(")")]
         for subcls in TimestampedLineTransformer.__subclasses__():
@@ -155,47 +157,47 @@
             return ret[0].astimezone().replace(tzinfo=None), strip_escape_sequences(ret[1]).rstrip()
         else:
             return ret[0], strip_escape_sequences(ret[1]).rstrip()
 
 
 class YMDHMScommaFTZ(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DD HH:MM:SS,SSS<timezone>"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2},\d{3}\s?(?:Z|[+-]\d{4})"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2},\d{3,}\s?(?:Z|[+-]\d{4})"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
     has_timezone = True
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDHMScommaF(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DD HH:MM:SS,SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2},\d{3}"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2},\d{3,}"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDHMSdotFZ(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DD HH:MM:SS.SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}\.\d{3}\s?(?:Z|[+-]\d{4})"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}\.\d{3,}\s?(?:Z|[+-]\d{4})"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
     has_timezone = True
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDHMSdotF(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DD HH:MM:SS.SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}\.\d{3}"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}\.\d{3,}"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
@@ -218,47 +220,47 @@
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDTHMScommaFZ(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DDTHH:MM:SS,SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2},\d{3}\s?(?:Z|[+-]\d{4})"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2},\d{3,}\s?(?:Z|[+-]\d{4})"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
     has_timezone = True
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDTHMScommaF(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DDTHH:MM:SS,SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2},\d{3}"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2},\d{3,}"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDTHMSdotFZ(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DDTHH:MM:SS.SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3}\s?(?:Z|[+-]\d{4}Z?)"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3,}\s?(?:Z|[+-]\d{4}Z?)"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
     has_timezone = True
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
 class YMDTHMSdotF(TimestampedLineTransformer):
     # log files with timestamp "YYYY-MM-DDTHH:MM:SS.SSS"
-    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3}"
+    timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3,}"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = datetime.fromisoformat
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
 
 
@@ -288,25 +290,48 @@
     # (note, year is omitted so let's guess from the log file's create date)
     timestamp_pattern = r"[JFMASOND][a-z]{2}\s(\s|\d)\d \d{2}:\d{2}:\d{2}"
     pattern = fr"(({timestamp_pattern})\s)"
     strptime_format = "%b %d %H:%M:%S"
 
     def __init__(self):
         super().__init__(self.pattern, self.strptime_format)
+        # this format does not have a year so assume the file's create time year
+        if self.file_stat is not None and self.file_stat.st_ctime:
+            self.date_year = datetime.fromtimestamp(self.file_stat.st_ctime).year
+        else:
+            self.date_year = datetime.now().year
 
     def __call__(self, obj: T) -> tuple[datetime | None, T]:
-        # this format does not have a year so assume the file's create time year
+        dt, obj = super().__call__(obj)
+        if dt is not None:
+            dt = dt.replace(year=self.date_year)
+        return dt, obj
+
+
+class HMSdot(TimestampedLineTransformer):
+    # strace files with timestamp "hh:mm:ss.sss"
+    # (note, date is omitted so let's guess from the log file's create date)
+    timestamp_pattern = r"\d{2}:\d{2}:\d{2}\.\d{3,}"
+    pattern = fr"(({timestamp_pattern})\s)"
+    strptime_format = "%H:%M:%S.%f"
+
+    def __init__(self):
+        super().__init__(self.pattern, self.strptime_format)
+
+        # this format does not have a date so assume the file's create date
         if self.file_stat is not None and self.file_stat.st_ctime:
-            date_year = datetime.fromtimestamp(self.file_stat.st_ctime).year
+            file_date = datetime.fromtimestamp(self.file_stat.st_ctime).date()
         else:
-            date_year = datetime.now().year
+            file_date = datetime.now().date()
+        self.date_replace_args = {"year": file_date.year, "month": file_date.month, "day": file_date.day}
 
+    def __call__(self, obj: T) -> tuple[datetime | None, T]:
         dt, obj = super().__call__(obj)
         if dt is not None:
-            dt = dt.replace(year=date_year)
+            dt = dt.replace(**self.date_replace_args)
         return dt, obj
 
 
 class PythonHttpServerLog(TimestampedLineTransformer):
     # ::1 - - [22/Sep/2023 21:58:40] "GET /log1.txt HTTP/1.1" 200 -
     timestamp_pattern = r"\d{2}\/\w+\/\d{4} \d{2}:\d{2}:\d{2}"
     pattern = fr"(.*)(- \[({timestamp_pattern})\]\s)"
```

### Comparing `logmerger-0.8.0/logmerger/tui/dialogs.py` & `logmerger-0.9.0/logmerger/tui/dialogs.py`

 * *Files identical despite different names*

### Comparing `logmerger-0.8.0/logmerger/tui/validators.py` & `logmerger-0.9.0/logmerger/tui/validators.py`

 * *Files identical despite different names*

### Comparing `logmerger-0.8.0/logmerger.egg-info/PKG-INFO` & `logmerger-0.9.0/logmerger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: logmerger
-Version: 0.8.0
+Version: 0.9.0
 Summary: A command-line utility to display multiple log files, merged by log timestamp
 Author: Paul McGuire
 Author-email: ptmcg.pm@gmail.com
 Project-URL: Source, https://github.com/ptmcg/logmerger
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: littletable
 Requires-Dist: rich
+Requires-Dist: typing-extensions>=4.12.0; python_version >= "3.13"
 Requires-Dist: textual
 Provides-Extra: pcap
 Requires-Dist: pyshark; extra == "pcap"
 
 # logmerger
 
 `logmerger` is a TUI for viewing a merged display of multiple log files, merged by timestamp.
@@ -43,15 +45,15 @@
 Something went wrong
 Traceback (last line is latest):
     sample.py: line 32
         divide(100, 0)
     sample.py: line 8
         return a / b
 ZeroDivisionError: division by zero
-2023-07-14 08:00:06 INFO   User authentication succeeded
+2023-07-14 08:00:06 INFO   User authentication failed
 2023-07-14 08:00:08 DEBUG  Starting data synchronization
 2023-07-14 08:00:11 INFO   Processing incoming request
 ```
 
 ```
 # log2.txt
 2023-07-14 08:00:01 INFO   Request processed successfully
@@ -86,15 +88,15 @@
                              Traceback (last line is latest):
                                  sample.py: line 32
                                      divide(100, 0)
                                  sample.py: line 8
                                      return a / b
                              ZeroDivisionError: division by zero                           
   2023-07-14 08:00:06.000   INFO   User authentication            DEBUG  Starting data
-                            succeeded                             synchronization
+                            failed                                synchronization
   2023-07-14 08:00:08.000   DEBUG  Starting data                  INFO   Processing incoming request
                             synchronization
   2023-07-14 08:00:11.000   INFO   Processing incoming request    DEBUG  Performing database backup
                             INFO   Processing incoming request
                             (a little more...)
   2023-07-14 08:00:14.000   DEBUG  Performing database backup     WARN   Invalid input received:
                                                                   missing required field
@@ -116,17 +118,19 @@
 
 ## Command line arguments
 
 `logmerger -h` will show the following help:
 
 ```
 usage: logmerger [-h] [--interactive] [--inline] [--output OUTPUT]
-                 [--start START] [--end END] [--width WIDTH]
-                 [--line_numbers] [--csv CSV] [--encoding ENCODING]
-                 [--timestamp_format [TIMESTAMP_FORMATS ...]] [--demo]
+                 [--start START] [--end END] [--autoclip]
+                 [--width WIDTH] [--line_numbers] [--show_clock]
+                 [--csv CSV] [--encoding ENCODING]
+                 [--timestamp_format [TIMESTAMP_FORMATS ...]]
+                 [--demo]
                  [files ...]
 
 positional arguments:
   files                 log files to be merged
 
 options:
   -h, --help            show this help message and exit
@@ -134,18 +138,20 @@
   --inline              show merged log data as inline merge
   --output OUTPUT, -o OUTPUT
                         save merged output to file ('-' for stdout; files ending in '.md' are saved
                         using Markdown)
   --start START, -s START
                         start time to select time window for merging logs
   --end END, -e END     end time to select time window for merging logs
+  --autoclip, -ac       clip merging to time range of logs in first log file
   --width WIDTH, -w WIDTH
                         total screen width to use for interactive mode (defaults to current screen
                         width)
   --line_numbers, -ln   add line number column
+  --show_clock, -clock  show running clock in header
   --csv CSV, -csv CSV   save merged logs to CSV file
   --encoding ENCODING, -enc ENCODING
                         encoding to use when reading log files (defaults to the system default encoding)
   --timestamp_format [TIMESTAMP_FORMATS ...]
                         custom timestamp format
   --demo                Run interactive demo
   
@@ -175,22 +181,31 @@
 
 
 ## Merging
 
 Log files get merged by interleaving log lines from each based on timestamps in each log line. `logmerger` tries to 
 use different timestamp formats until it finds a matching format for each input file. The supported formats are:
 
-| format                       | description                                                                                         |
-|------------------------------|-----------------------------------------------------------------------------------------------------|
-| `YYYY-MM-DD HH:MM:SS,SSS`    | date+time to milliseconds, with ',' decimal (default for Python's `asctime` log marker)             |
-| `YYYY-MM-DD HH:MM:SS.SSS`    | date+time to milliseconds, with '.' decimal                                                         |
-| `YYYY-MM-DD HH:MM:SS`        | date+time to seconds                                                                                |
-| `YYYY-MM-DDTHH:MM:SS,SSS`    | date+T+time to milliseconds, with ',' decimal                                                       |
-| `YYYY-MM-DDTHH:MM:SS.SSS`    | date+T+time to milliseconds, with '.' decimal                                                       |
-| `YYYY-MM-DDTHH:MM:SS`        | date+T+time to seconds                                                                              |
-| `Jan DD HH:MM:SS`            | month/day + time (timestamp in syslog files); year is inferred from the create date of the log file |
-| `DD/Jan/YYYY HH:MM:SS`       | day/month/year + time                                                                               |
-| `DD/Jan/YYYY:HH:MM:SS ±ZZZZ` | day/month/year + time + timezone offset (converts timestamps to local time)                         |
+| format                       | description                                                                                           |
+|------------------------------|-------------------------------------------------------------------------------------------------------|
+| `YYYY-MM-DD HH:MM:SS,SSS`    | date+time to milliseconds, with ',' decimal (default for Python's `asctime` log marker)               |
+| `YYYY-MM-DD HH:MM:SS.SSS`    | date+time to milliseconds, with '.' decimal                                                           |
+| `YYYY-MM-DD HH:MM:SS`        | date+time to seconds                                                                                  |
+| `YYYY-MM-DDTHH:MM:SS,SSS`    | date+T+time to milliseconds, with ',' decimal                                                         |
+| `YYYY-MM-DDTHH:MM:SS.SSS`    | date+T+time to milliseconds, with '.' decimal                                                         |
+| `YYYY-MM-DDTHH:MM:SS`        | date+T+time to seconds                                                                                |
+| `Jan DD HH:MM:SS`            | month/day + time (timestamp in syslog files); year is inferred from the create date of the log file   |
+| `DD/Jan/YYYY HH:MM:SS`       | day/month/year + time                                                                                 |
+| `DD/Jan/YYYY:HH:MM:SS ±ZZZZ` | day/month/year + time + timezone offset (converts timestamps to local time)                           |
+| `HH:MM:SS.SSSSSS`            | hour/minute/second (timestamp in strace files); date is inferred from the create date of the log file |
+| `strace`                     | uses HH:MM:SS.SSSSSS format with leading process id integer                                           |
 
 
 Untimestamped log lines that contain multiple lines (such as a traceback) get combined with the previous timestamped
 line (see in the example above).
+
+
+## Security contact information
+
+To report a security vulnerability, please use the
+[Tidelift security contact](https://tidelift.com/security).
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `logmerger-0.8.0/logmerger.egg-info/SOURCES.txt` & `logmerger-0.9.0/logmerger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logmerger-0.8.0/setup.cfg` & `logmerger-0.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 [metadata]
 name = logmerger
-version = 0.8.0
+version = 0.9.0
 description = A command-line utility to display multiple log files, merged by log timestamp
 long_description = file:README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Source=https://github.com/ptmcg/logmerger
 email = ptmcg.pm@gmail.com
 author = Paul McGuire
 author_email = ptmcg.pm@gmail.com
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: 3.13
 	Topic :: System :: Systems Administration
 	Topic :: Utilities
 	Typing :: Typed
 
 [options]
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	littletable
 	rich
+	typing-extensions>=4.12.0;python_version>="3.13"
 	textual
 include_package_data = True
 
 [options.extras_require]
 pcap = 
 	pyshark
```

