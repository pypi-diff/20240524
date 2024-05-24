# Comparing `tmp/eras-0.3.4.tar.gz` & `tmp/eras-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.3.4.tar", last modified: Thu May 23 03:25:53 2024, max compression
+gzip compressed data, was "eras-0.3.5.tar", last modified: Fri May 24 03:14:03 2024, max compression
```

## Comparing `eras-0.3.4.tar` & `eras-0.3.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.906987 eras-0.3.4/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.4/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.4/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     2662 2024-05-23 03:25:53.906638 eras-0.3.4/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     2039 2024-05-23 03:25:45.000000 eras-0.3.4/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.883776 eras-0.3.4/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.4/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.886529 eras-0.3.4/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.3.4/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.4/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1367 2024-05-23 02:54:10.000000 eras-0.3.4/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.888035 eras-0.3.4/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.4/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.890919 eras-0.3.4/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.4/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2628 2024-05-23 03:13:09.000000 eras-0.3.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.4/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.4/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.4/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1798 2024-05-23 03:13:06.000000 eras-0.3.4/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.3.4/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.891699 eras-0.3.4/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.4/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.892694 eras-0.3.4/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.4/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1864 2024-05-23 03:06:20.000000 eras-0.3.4/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.4/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6625 2024-05-23 02:41:23.000000 eras-0.3.4/eras/config/__pycache__/post_install.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      610 2024-05-23 03:01:32.000000 eras-0.3.4/eras/config/config.py
--rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.3.4/eras/config/post_install.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.893143 eras-0.3.4/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.4/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.893635 eras-0.3.4/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.4/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.894381 eras-0.3.4/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.4/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.896044 eras-0.3.4/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.4/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.4/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.4/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      735 2024-05-23 02:52:24.000000 eras-0.3.4/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.898090 eras-0.3.4/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.4/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.900886 eras-0.3.4/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.4/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.3.4/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.4/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.3.4/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.4/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.4/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.4/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.3.4/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.4/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.4/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.4/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.3.4/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.4/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.4/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.901883 eras-0.3.4/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.4/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.902968 eras-0.3.4/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.4/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3776 2024-05-23 03:17:34.000000 eras-0.3.4/eras/services/__pycache__/user_command_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.903829 eras-0.3.4/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.4/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.905994 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.4/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.4/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.4/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.3.4/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1846 2024-05-23 03:16:10.000000 eras-0.3.4/eras/services/user_command_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.885684 eras-0.3.4/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     2662 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3632 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-23 03:25:53.907059 eras-0.3.4/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-23 03:22:03.000000 eras-0.3.4/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.989910 eras-0.3.5/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.5/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.5/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2024-05-24 03:14:03.989380 eras-0.3.5/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     2074 2024-05-24 03:13:35.000000 eras-0.3.5/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.960856 eras-0.3.5/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.5/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.963679 eras-0.3.5/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.3.5/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.5/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1367 2024-05-23 02:54:10.000000 eras-0.3.5/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.965055 eras-0.3.5/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.5/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.967999 eras-0.3.5/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.5/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2628 2024-05-23 03:13:09.000000 eras-0.3.5/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.3.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.5/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.5/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.5/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1798 2024-05-23 03:13:06.000000 eras-0.3.5/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.3.5/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.968847 eras-0.3.5/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.5/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.970143 eras-0.3.5/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.5/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1864 2024-05-23 03:06:20.000000 eras-0.3.5/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.5/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6625 2024-05-23 02:41:23.000000 eras-0.3.5/eras/config/__pycache__/post_install.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1531 2024-05-24 03:12:51.000000 eras-0.3.5/eras/config/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     4360 2024-05-24 03:12:51.000000 eras-0.3.5/eras/config/post_install.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.970732 eras-0.3.5/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.5/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.971422 eras-0.3.5/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.5/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.972406 eras-0.3.5/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.5/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.974758 eras-0.3.5/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.5/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.3.5/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.5/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.5/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.5/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      735 2024-05-23 02:52:24.000000 eras-0.3.5/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.977488 eras-0.3.5/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.5/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.980988 eras-0.3.5/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.5/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.3.5/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.5/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.3.5/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.5/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.5/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.5/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.3.5/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.5/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.5/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.5/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.3.5/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.5/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.5/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.982329 eras-0.3.5/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.5/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.984136 eras-0.3.5/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.5/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.3.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3776 2024-05-23 03:17:34.000000 eras-0.3.5/eras/services/__pycache__/user_command_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.985987 eras-0.3.5/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.5/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.988570 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.5/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.5/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.5/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.3.5/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1846 2024-05-23 03:16:10.000000 eras-0.3.5/eras/services/user_command_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:14:03.962552 eras-0.3.5/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2024-05-24 03:14:03.000000 eras-0.3.5/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3632 2024-05-24 03:14:03.000000 eras-0.3.5/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-24 03:14:03.000000 eras-0.3.5/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-24 03:14:03.000000 eras-0.3.5/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-24 03:14:03.000000 eras-0.3.5/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-24 03:14:03.000000 eras-0.3.5/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-24 03:14:03.990014 eras-0.3.5/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-24 03:13:01.000000 eras-0.3.5/setup.py
```

### Comparing `eras-0.3.4/PKG-INFO` & `eras-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.4
+Version: 0.3.5
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,16 @@
 Requires-Dist: asyncio==3.4.3
 
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
+Works on Windows, Mac, and Linux!
+
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 # Install
 ```
```

### Comparing `eras-0.3.4/README.md` & `eras-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
+Works on Windows, Mac, and Linux!
+
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 # Install
 ```
```

### Comparing `eras-0.3.4/eras/__pycache__/main.cpython-311.pyc` & `eras-0.3.5/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.3.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.3.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.3.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.3.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.3.5/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.3.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.3.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/llama_functions_agent.py` & `eras-0.3.5/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.3.5/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/llm_functions_agent.py` & `eras-0.3.5/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/simple_llm.py` & `eras-0.3.5/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/agents/terminal_llama_agent.py` & `eras-0.3.5/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.3.5/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.3.5/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/config/__pycache__/post_install.cpython-311.pyc` & `eras-0.3.5/eras/config/__pycache__/post_install.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/config/post_install.py` & `eras-0.3.5/eras/config/post_install.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,110 @@
 import os
 import sys
-from shutil import which
 import subprocess
+
 def alias_exists(alias_name):
     home = os.path.expanduser("~")
-    shell_config_files = [".bashrc", ".zshrc"]
+    shell_config_files = [".bashrc", ".zshrc", ".bash_profile"]
 
     for config_file in shell_config_files:
         config_path = os.path.join(home, config_file)
         if os.path.exists(config_path):
             with open(config_path, "r") as file:
                 if alias_name in file.read():
                     return True
     return False
 
-def add_alias_to_shell(alias_command):
-    home = os.path.expanduser("~")
-    shell_config_files = [".bashrc", ".zshrc"]
-
-    for config_file in shell_config_files:
-        config_path = os.path.join(home, config_file)
-        if os.path.exists(config_path):
-            with open(config_path, "a") as file:
-                file.write(f"\n{alias_command}\n")
-
 def env_var_exists(var_name):
-    home = os.path.expanduser("~")
-    shell_config_files = [".bashrc", ".zshrc"]
-
-    for config_file in shell_config_files:
-        config_path = os.path.join(home, config_file)
-        if os.path.exists(config_path):
-            with open(config_path, "r") as file:
-                if var_name in file.read():
-                    return True
-    return False
+    if os.name == 'nt':  # Windows
+        return os.getenv(var_name) is not None
+    else:  # Unix-based systems
+        home = os.path.expanduser("~")
+        shell_config_files = [".bashrc", ".zshrc", ".bash_profile"]
+
+        for config_file in shell_config_files:
+            config_path = os.path.join(home, config_file)
+            if os.path.exists(config_path):
+                with open(config_path, "r") as file:
+                    if var_name in file.read():
+                        return True
+        return False
+
+# def refresh_windows_environment_variables():
+#     # Refresh user environment variables
+#     user_vars = os.popen('powershell -Command "[System.Environment]::GetEnvironmentVariables(\'User\')"').read()
+#     for line in user_vars.splitlines():
+#         if '=' in line:
+#             key, value = line.split('=', 1)
+#             os.environ[key.strip()] = value.strip()
+#
+#     # Refresh system environment variables
+#     system_vars = os.popen('powershell -Command "[System.Environment]::GetEnvironmentVariables(\'Machine\')"').read()
+#     for line in system_vars.splitlines():
+#         if '=' in line:
+#             key, value = line.split('=', 1)
+#             os.environ[key.strip()] = value.strip()
 
 def add_env_var_to_shell(env_var_command):
-    home = os.path.expanduser("~")
-    shell_config_files = [".bashrc", ".zshrc"]
-
-    for config_file in shell_config_files:
-        config_path = os.path.join(home, config_file)
-        if os.path.exists(config_path):
-            with open(config_path, "a") as file:
-                file.write(f"\n{env_var_command}\n")
+    if os.name == 'nt':  # Windows
+        print('setting windows shell env var')
+        var_name, var_value = env_var_command.split('=', 1)
+        os.system(f'setx {var_name} {var_value}')
+        # Set the environment variable persistently using setx
+        # subprocess.run(['setx', var_name, var_value], check=True)
+
+    else:  # Unix-based systems
+        home = os.path.expanduser("~")
+        shell_config_files = [".bashrc", ".zshrc", ".bash_profile"]
+
+        for config_file in shell_config_files:
+            config_path = os.path.join(home, config_file)
+            if os.path.exists(config_path):
+                with open(config_path, "a") as file:
+                    file.write(f"\nexport {env_var_command}\n")
 
 def ensure():
-    # print('Running post install...')
-
-    # eras_path = '/usr/local/bin/eras' #which("eras")
-    # if not eras_path:
-    #     print("Could not find 'eras' command in PATH. Please make sure it is installed correctly and run this script again.")
-    #     sys.exit(1)
-    #
-    # alias_command = f"alias eras='{eras_path}'"
-    # if not alias_exists("alias eras="):
-    #     add_alias_to_shell(alias_command)
-    #     print("Alias 'eras' added to shell configuration files.")
-    # else:
-        # print("Alias 'eras' already exists in shell configuration files.")
-
     if not env_var_exists("ERAS_OPENAI_KEY"):
         openai_key = input("Please enter your OpenAI API key (ERAS_OPENAI_KEY): ").strip()
         if not openai_key:
             print("Error: OpenAI API key cannot be empty.")
             sys.exit(1)
-        env_var_command = f"export ERAS_OPENAI_KEY='{openai_key}'"
-        os.environ['ERAS_OPENAI_KEY'] = openai_key # DO THIS FOR THE FIRST INSTALL !!!!
+        env_var_command = f"ERAS_OPENAI_KEY={openai_key}"
+        os.environ['ERAS_OPENAI_KEY'] = openai_key
         add_env_var_to_shell(env_var_command)
-        print("Environment variable 'ERAS_OPENAI_KEY' added to shell configuration files.  Reloading .zshrc in this terminal window.")
-        # print('Please run source ~/.zshrc or open a new terminal window.')
-        os.system(f'source {os.path.expanduser("~/.zshrc")}')
-
-    reload_profile(get_profile_file())  # so the first install works with env vars
-    # else:
-        # print("Environment variable 'ERAS_OPENAI_KEY' already exists in shell configuration files.")
-
-    # if not env_var_exists("ERAS_BASE_URL"):
-    #     base_url = input("Please enter the base URL (ERAS_BASE_URL) [Optional] to point at Llama.cpp or other OpenAI server: ").strip()
-    #     if base_url:
-    #         command2 = f"export ERAS_BASE_URL='{base_url}'"
-    #         add_env_var_to_shell(command2)
-    #         print("Environment variable 'ERAS_BASE_URL' added to shell configuration files.")
-        # else:
-            # print("ERAS_BASE_URL not set.")
-    # else:
-    #     print("Environment variable 'ERAS_BASE_URL' already exists in shell configuration files.")
+        print("Environment variable 'ERAS_OPENAI_KEY' added to environment.")
 
+        if os.name != 'nt':  # Unix-based systems
+            reload_profile(get_profile_file())
+        else:
+            print('======= PLEASE CLOSE THIS TERMINAL WINDOW AND OPEN A NEW ONE =========')
 
 def get_profile_file():
-    shell = os.environ.get('SHELL', '')
-    if 'zsh' in shell:
-        return os.path.expanduser('~/.zshrc')
-    elif 'bash' in shell:
-        bash_profile = os.path.expanduser('~/.bash_profile')
-        if os.path.exists(bash_profile):
-            return bash_profile
+    if os.name == 'nt':  # Windows
+        return None  # No equivalent profile file
+    else:  # Unix-based systems
+        shell = os.environ.get('SHELL', '')
+        if 'zsh' in shell:
+            return os.path.expanduser('~/.zshrc')
+        elif 'bash' in shell:
+            bash_profile = os.path.expanduser('~/.bash_profile')
+            if os.path.exists(bash_profile):
+                return bash_profile
+            else:
+                return os.path.expanduser('~/.bashrc')
         else:
-            return os.path.expanduser('~/.bashrc')
-    else:
-        # Add more shells as needed
-        raise ValueError("Unsupported shell type")
-
-def add_api_key_to_profile(api_key, profile_file):
-    with open(profile_file, 'a') as file:
-        file.write(f'\nexport MY_API_KEY="{api_key}"\n')
+            raise ValueError("Unsupported shell type")
 
 def reload_profile(profile_file):
-    shell = os.environ.get('SHELL', '')
-    if 'zsh' in shell:
-        subprocess.run(['zsh', '-c', f'source {profile_file}'], check=True)
-    elif 'bash' in shell:
-        subprocess.run(['bash', '-c', f'source {profile_file}'], check=True)
+    if os.name != 'nt':  # Unix-based systems
+        shell = os.environ.get('SHELL', '')
+        if 'zsh' in shell:
+            subprocess.run(['zsh', '-c', f'source {profile_file}'], check=True)
+        elif 'bash' in shell:
+            subprocess.run(['bash', '-c', f'source {profile_file}'], check=True)
+        else:
+            print(f"Please manually source your profile file: {profile_file}")
     else:
-        # Add more shells as needed
-        print(f"Please manually source your profile file: {profile_file}")
+        print("Please restart your Command Prompt or PowerShell session to apply the changes.")
 
 if __name__ == "__main__":
     ensure()
```

### Comparing `eras-0.3.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.3.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/decorators/chatgpt_tool_data.py` & `eras-0.3.5/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.3.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.3.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.3.5/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.3.5/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/factories/function_details_factory.py` & `eras-0.3.5/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/factories/message_factory.py` & `eras-0.3.5/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/main.py` & `eras-0.3.5/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.3.5/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.3.5/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.3.5/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.3.5/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.3.5/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.3.5/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/conversation.py` & `eras-0.3.5/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/function_details.py` & `eras-0.3.5/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/message.py` & `eras-0.3.5/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/models/transaction.py` & `eras-0.3.5/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/run.ipynb` & `eras-0.3.5/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.3.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.3.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.3.5/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.3.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.3.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.3.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.3.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.3.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.3.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.3.5/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.3.5/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/llm_callable_functions/user_details.py` & `eras-0.3.5/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/shell_command_service.py` & `eras-0.3.5/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras/services/user_command_service.py` & `eras-0.3.5/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/eras.egg-info/PKG-INFO` & `eras-0.3.5/eras.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.4
+Version: 0.3.5
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,16 @@
 Requires-Dist: asyncio==3.4.3
 
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
+Works on Windows, Mac, and Linux!
+
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 # Install
 ```
```

### Comparing `eras-0.3.4/eras.egg-info/SOURCES.txt` & `eras-0.3.5/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.3.4/setup.py` & `eras-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #         print('Calling post_install.py')
 #         post_install_script = os.path.join(os.path.dirname(__file__), 'eras', 'post_install.py')
 #         # Run the post_install.py script in a new interactive shell
 #         subprocess.run([sys.executable, post_install_script], check=True, stdin=sys.stdin, stdout=sys.stdout)
 
 setup(
     name='eras',
-    version='0.3.4',
+    version='0.3.5',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

