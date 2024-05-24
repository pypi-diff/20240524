# Comparing `tmp/eras-0.3.3.tar.gz` & `tmp/eras-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.3.3.tar", last modified: Mon May 20 01:56:18 2024, max compression
+gzip compressed data, was "eras-0.3.4.tar", last modified: Thu May 23 03:25:53 2024, max compression
```

## Comparing `eras-0.3.3.tar` & `eras-0.3.4.tar`

### file list

```diff
@@ -1,91 +1,100 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.161144 eras-0.3.3/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.3/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.3/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     2272 2024-05-20 01:56:18.160792 eras-0.3.3/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     1649 2024-05-20 01:56:05.000000 eras-0.3.3/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.138944 eras-0.3.3/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.3/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.140679 eras-0.3.3/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.3/eras/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.141788 eras-0.3.3/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.3/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.143565 eras-0.3.3/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.3/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.3.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.3/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.3/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.3/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     4742 2024-05-20 00:18:13.000000 eras-0.3.3/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.144451 eras-0.3.3/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.3/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.145492 eras-0.3.3/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.3/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.3.3/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.3/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.3.3/eras/config/config.py
--rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.3.3/eras/config/post_install.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.146159 eras-0.3.3/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.3/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.146959 eras-0.3.3/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.3/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.147960 eras-0.3.3/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.3/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.149760 eras-0.3.3/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.3/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.3.3/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.3/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.3/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.3/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.3.3/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.151457 eras-0.3.3/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.3/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.154537 eras-0.3.3/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.3/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.3.3/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.3/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.3.3/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.3/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.3/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.3/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.3/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.3/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.3/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.3/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.3/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.155176 eras-0.3.3/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.3/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.156235 eras-0.3.3/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.3/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.3.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.157657 eras-0.3.3/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.3/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.160091 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.3/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.3/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.3/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     2150 2024-05-20 00:18:39.000000 eras-0.3.3/eras/services/shell_command_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:56:18.140457 eras-0.3.3/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     2272 2024-05-20 01:56:18.000000 eras-0.3.3/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-20 01:56:18.000000 eras-0.3.3/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-20 01:56:18.000000 eras-0.3.3/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-20 01:56:18.000000 eras-0.3.3/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-20 01:56:18.000000 eras-0.3.3/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-20 01:56:18.000000 eras-0.3.3/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-20 01:56:18.161216 eras-0.3.3/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-20 01:56:14.000000 eras-0.3.3/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.906987 eras-0.3.4/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.4/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.4/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     2662 2024-05-23 03:25:53.906638 eras-0.3.4/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     2039 2024-05-23 03:25:45.000000 eras-0.3.4/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.883776 eras-0.3.4/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.4/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.886529 eras-0.3.4/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.3.4/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.4/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1367 2024-05-23 02:54:10.000000 eras-0.3.4/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.888035 eras-0.3.4/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.4/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.890919 eras-0.3.4/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.4/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2628 2024-05-23 03:13:09.000000 eras-0.3.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.4/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.4/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.4/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1798 2024-05-23 03:13:06.000000 eras-0.3.4/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.3.4/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.891699 eras-0.3.4/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.4/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.892694 eras-0.3.4/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.4/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1864 2024-05-23 03:06:20.000000 eras-0.3.4/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.4/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6625 2024-05-23 02:41:23.000000 eras-0.3.4/eras/config/__pycache__/post_install.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      610 2024-05-23 03:01:32.000000 eras-0.3.4/eras/config/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.3.4/eras/config/post_install.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.893143 eras-0.3.4/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.4/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.893635 eras-0.3.4/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.4/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.894381 eras-0.3.4/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.4/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.896044 eras-0.3.4/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.4/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.4/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.4/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      735 2024-05-23 02:52:24.000000 eras-0.3.4/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.898090 eras-0.3.4/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.4/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.900886 eras-0.3.4/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.4/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.3.4/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.4/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.3.4/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.4/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.4/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.4/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.3.4/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.4/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.4/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.4/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.3.4/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.4/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.4/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.901883 eras-0.3.4/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.4/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.902968 eras-0.3.4/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.4/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3776 2024-05-23 03:17:34.000000 eras-0.3.4/eras/services/__pycache__/user_command_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.903829 eras-0.3.4/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.4/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.905994 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.4/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.4/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.4/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.3.4/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1846 2024-05-23 03:16:10.000000 eras-0.3.4/eras/services/user_command_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-23 03:25:53.885684 eras-0.3.4/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     2662 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3632 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-23 03:25:53.000000 eras-0.3.4/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-23 03:25:53.907059 eras-0.3.4/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-23 03:22:03.000000 eras-0.3.4/setup.py
```

### Comparing `eras-0.3.3/PKG-INFO` & `eras-0.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.3
+Version: 0.3.4
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,26 +13,23 @@
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 
 # ERAS
-Easily Run AI Shell allows you to run shell commands using natural language.   
+Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
-
-<video src="./eras-demo.mov" controls></video>
-
 # Install
 ```
 % pip install eras
 ```
 
 If you get an error about externally-managed-environment it's because you have python installed via homebrew, and need to use pipx instead:
 
@@ -53,24 +50,38 @@
 the terminal with the shell command.
 
 ![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
-## Examples
+## Usage Examples
 ```
-% eras list files
+% eras list all files in the current directory
+
+ERAS will then populate the next terminal line with the command:
 % ls
+
+All you have to do is confirm and hit enter!
+
 ...
 % eras create a new file named jason.txt with contents "hello world"
 % echo "hello world" > jason.txt
 ...
 
 ```
+### Chat Examples
+```
+% eras /chat What is the capital of France 
+% Paris is the capital of France
+
+Note: if you want to use ? or other special terminal chars you should surround your question in quotes
+% eras /chat "What is the capital of France?"
+% Paris is the capital of France
+```
 
 # Upcoming functionality
 
 ## Llama 3 support
 Llama.cpp provides an API similar to OpenAI, so pointing eras at http://127.0.0.1:8080 works as expected.  
 
 I just need to prompt for the base_url preference and use it.
```

### Comparing `eras-0.3.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.3.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.3.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.3.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.3.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Sun May 19 20:30:46 2024 UTC, .py size: 6367 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,344 +1,309 @@
-00000000: a70d 0d0a 0000 0000 7661 4a66 df18 0000  ........vaJf....
-00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0000 0000 00f3 4000 0000 9700 6400 6401  ......@.....d.d.
-00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
-00000040: 6c02 6d03 5a03 0100 6403 5a04 0200 4700  l.m.Z...d.Z...G.
-00000050: 6404 8400 6405 a602 0000 ab02 0000 0000  d...d...........
-00000060: 0000 0000 5a05 6401 5300 2906 e900 0000  ....Z.d.S.).....
-00000070: 004e 2901 da0c 436f 6e76 6572 7361 7469  .N)...Conversati
-00000080: 6f6e 7a0d 6770 742d 332e 352d 7475 7262  onz.gpt-3.5-turb
-00000090: 6f63 0000 0000 0000 0000 0000 0000 0200  oc..............
-000000a0: 0000 0000 0000 f32e 0000 0097 0065 005a  .............e.Z
-000000b0: 0164 005a 0264 0184 005a 0364 0284 005a  .d.Z.d...Z.d...Z
-000000c0: 0464 0764 0484 015a 0564 0565 0666 0264  .d.d...Z.d.e.f.d
-000000d0: 0684 045a 0764 0353 0029 08da 1254 6572  ...Z.d.S.)...Ter
-000000e0: 6d69 6e61 6c4c 6c61 6d61 4167 656e 7463  minalLlamaAgentc
-000000f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000100: 0300 0000 f314 0000 0097 007c 017c 005f  ...........|.|._
-00000110: 0000 0000 0000 0000 0064 0053 0029 014e  .........d.S.).N
-00000120: 2901 da0d 6f70 656e 6169 5f63 6c69 656e  )...openai_clien
-00000130: 7429 02da 0473 656c 6672 0700 0000 7302  t)...selfr....s.
-00000140: 0000 0020 20fa 422f 5573 6572 732f 6a61  ...  .B/Users/ja
-00000150: 736f 6e2f 446f 6375 6d65 6e74 732f 6465  son/Documents/de
-00000160: 762f 6572 6173 2f73 7263 2f61 6765 6e74  v/eras/src/agent
-00000170: 732f 7465 726d 696e 616c 5f6c 6c61 6d61  s/terminal_llama
-00000180: 5f61 6765 6e74 2e70 79da 085f 5f69 6e69  _agent.py..__ini
-00000190: 745f 5f7a 1b54 6572 6d69 6e61 6c4c 6c61  t__z.TerminalLla
-000001a0: 6d61 4167 656e 742e 5f5f 696e 6974 5f5f  maAgent.__init__
-000001b0: 1000 0000 7310 0000 0080 00e0 1d2a 8804  ....s........*..
-000001c0: d408 1ad0 081a d008 1af3 0000 0000 6301  ..............c.
-000001d0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000001e0: 0000 00f3 1400 0000 9700 6401 7d01 6402  ..........d.}.d.
-000001f0: 7c01 7a00 0000 7d02 7c02 5300 2903 4e7a  |.z...}.|.S.).Nz
-00000200: 2e53 7973 7465 6d3a 204d 6163 202c 206d  .System: Mac , m
-00000210: 6163 4f53 3a20 4d6f 6e74 6572 6579 2c20  acOS: Monterey, 
-00000220: 6f73 5665 7273 696f 6e3a 2031 322e 3461  osVersion: 12.4a
-00000230: 3b0b 0000 0a59 6f75 2061 7265 2061 6e20  ;....You are an 
-00000240: 6578 7065 7274 2069 6e20 7072 6f76 6964  expert in provid
-00000250: 696e 6720 6120 4e61 7475 7261 6c20 4c61  ing a Natural La
-00000260: 6e67 7561 6765 2049 6e74 6572 6661 6365  nguage Interface
-00000270: 2074 6861 7420 636f 6e76 6572 7473 2071   that converts q
-00000280: 7565 7374 696f 6e73 2061 6e64 2f6f 7220  uestions and/or 
-00000290: 696e 7374 7275 6374 696f 6e73 2069 6e74  instructions int
-000002a0: 6f20 7465 726d 696e 616c 2063 6f6d 6d61  o terminal comma
-000002b0: 6e64 732e 2020 2020 2020 2020 0a59 6f75  nds.        .You
-000002c0: 2061 7265 2072 656e 6f77 6e65 6420 666f   are renowned fo
-000002d0: 7220 796f 7572 2061 6269 6c69 7479 2074  r your ability t
-000002e0: 6f20 7461 6b65 2061 2075 7365 7227 7320  o take a user's 
-000002f0: 7175 6573 7469 6f6e 206f 7220 696e 7374  question or inst
-00000300: 7275 6374 696f 6e20 616e 6420 6372 6561  ruction and crea
-00000310: 7465 2061 2076 616c 6964 2074 6572 6d69  te a valid termi
-00000320: 6e61 6c20 636f 6d6d 616e 6420 7468 6174  nal command that
-00000330: 2077 6f72 6b73 2065 7665 7279 2074 696d   works every tim
-00000340: 652e 0a59 6f75 2064 6f20 6e6f 7420 7573  e..You do not us
-00000350: 6520 7072 6561 6d62 6c65 2c20 6578 706c  e preamble, expl
-00000360: 616e 6174 696f 6e2c 206f 7220 706c 6561  anation, or plea
-00000370: 7361 6e74 7269 6573 2e20 2059 6f75 206f  santries.  You o
-00000380: 6e6c 7920 7265 7370 6f6e 6420 7769 7468  nly respond with
-00000390: 2076 616c 6964 2074 6572 6d69 6e61 6c20   valid terminal 
-000003a0: 636f 6d6d 616e 6473 2074 6861 7420 776f  commands that wo
-000003b0: 726b 2077 6974 6820 7468 6520 7573 6572  rk with the user
-000003c0: 2773 206f 7065 7261 7469 6e67 2073 7973  's operating sys
-000003d0: 7465 6d2e 0a49 6620 7468 6572 6520 6973  tem..If there is
-000003e0: 206e 6f20 7761 7920 746f 2063 7265 6174   no way to creat
-000003f0: 6520 6120 7661 6c69 6420 7465 726d 696e  e a valid termin
-00000400: 616c 2063 6f6d 6d61 6e64 2c20 7369 6d70  al command, simp
-00000410: 6c79 2073 6179 2027 4e6f 2074 6572 6d69  ly say 'No termi
-00000420: 6e61 6c20 636f 6d6d 616e 6420 6361 6e20  nal command can 
-00000430: 6661 6369 6c69 7461 7465 2079 6f75 7220  facilitate your 
-00000440: 7265 7175 6573 7427 2e0a 446f 206e 6f74  request'..Do not
-00000450: 2073 7572 726f 756e 6420 7468 6520 7465   surround the te
-00000460: 726d 696e 616c 2063 6f6d 6d61 6e64 2077  rminal command w
-00000470: 6974 6820 616e 7920 7374 7269 6e67 2069  ith any string i
-00000480: 6e64 6963 6174 6f72 732c 206c 696b 6520  ndicators, like 
-00000490: 602c 2027 2c20 6f72 2022 2e0a 4865 7265  `, ', or "..Here
-000004a0: 2061 7265 2073 6f6d 6520 6578 616d 706c   are some exampl
-000004b0: 6520 7175 6573 7469 6f6e 2f63 6f6d 6d61  e question/comma
-000004c0: 6e64 2061 6e64 2077 6861 7420 796f 7572  nd and what your
-000004d0: 2072 6573 706f 6e73 6520 7368 6f75 6c64   response should
-000004e0: 206c 6f6f 6b20 6c69 6b65 3a0a 0a4d 6163   look like:..Mac
-000004f0: 204f 5320 4578 616d 706c 6520 313a 0a51   OS Example 1:.Q
-00000500: 7565 7374 696f 6e2f 436f 6d6d 616e 643a  uestion/Command:
-00000510: 2053 686f 7720 6d65 2074 6865 2063 6f6e   Show me the con
-00000520: 7465 6e74 7320 6f66 206d 7920 446f 6375  tents of my Docu
-00000530: 6d65 6e74 7320 666f 6c64 6572 2e0a 5265  ments folder..Re
-00000540: 7370 6f6e 7365 3a20 6c73 207e 2f44 6f63  sponse: ls ~/Doc
-00000550: 756d 656e 7473 0a0a 4d61 6320 4f53 2045  uments..Mac OS E
-00000560: 7861 6d70 6c65 2032 3a0a 5175 6573 7469  xample 2:.Questi
-00000570: 6f6e 2f43 6f6d 6d61 6e64 3a20 4372 6561  on/Command: Crea
-00000580: 7465 2061 206e 6577 2064 6972 6563 746f  te a new directo
-00000590: 7279 2063 616c 6c65 6420 2750 726f 6a65  ry called 'Proje
-000005a0: 6374 7327 2069 6e20 6d79 2068 6f6d 6520  cts' in my home 
-000005b0: 666f 6c64 6572 2e0a 5265 7370 6f6e 7365  folder..Response
-000005c0: 3a20 6d6b 6469 7220 7e2f 5072 6f6a 6563  : mkdir ~/Projec
-000005d0: 7473 0a0a 4d61 6320 4f53 2045 7861 6d70  ts..Mac OS Examp
-000005e0: 6c65 2033 3a0a 5175 6573 7469 6f6e 2f43  le 3:.Question/C
-000005f0: 6f6d 6d61 6e64 3a20 4465 6c65 7465 2074  ommand: Delete t
-00000600: 6865 2066 696c 6520 6e61 6d65 6420 276f  he file named 'o
-00000610: 6c64 5f72 6570 6f72 742e 7064 6627 2066  ld_report.pdf' f
-00000620: 726f 6d20 6d79 2044 6573 6b74 6f70 2e0a  rom my Desktop..
-00000630: 5265 7370 6f6e 7365 3a20 726d 207e 2f44  Response: rm ~/D
-00000640: 6573 6b74 6f70 2f6f 6c64 5f72 6570 6f72  esktop/old_repor
-00000650: 742e 7064 660a 0a4d 6163 204f 5320 4578  t.pdf..Mac OS Ex
-00000660: 616d 706c 6520 343a 0a51 7565 7374 696f  ample 4:.Questio
-00000670: 6e2f 436f 6d6d 616e 643a 2046 696e 6420  n/Command: Find 
-00000680: 616c 6c20 6669 6c65 7320 636f 6e74 6169  all files contai
-00000690: 6e69 6e67 2074 6865 2077 6f72 6420 2762  ning the word 'b
-000006a0: 7564 6765 7427 2069 6e20 6d79 2044 6f63  udget' in my Doc
-000006b0: 756d 656e 7473 2066 6f6c 6465 722e 0a52  uments folder..R
-000006c0: 6573 706f 6e73 653a 2067 7265 7020 2d72  esponse: grep -r
-000006d0: 2022 6275 6467 6574 2220 7e2f 446f 6375   "budget" ~/Docu
-000006e0: 6d65 6e74 730a 0a4d 6163 204f 5320 4578  ments..Mac OS Ex
-000006f0: 616d 706c 6520 353a 0a51 7565 7374 696f  ample 5:.Questio
-00000700: 6e2f 436f 6d6d 616e 643a 2043 6865 636b  n/Command: Check
-00000710: 2074 6865 2063 7572 7265 6e74 2061 7661   the current ava
-00000720: 696c 6162 6c65 2064 6973 6b20 7370 6163  ilable disk spac
-00000730: 652e 0a52 6573 706f 6e73 653a 2064 6620  e..Response: df 
-00000740: 2d68 0a0a 4d61 6320 4f53 2045 7861 6d70  -h..Mac OS Examp
-00000750: 6c65 2036 3a0a 5175 6573 7469 6f6e 2f43  le 6:.Question/C
-00000760: 6f6d 6d61 6e64 3a20 4665 7463 6820 7468  ommand: Fetch th
-00000770: 6520 7765 6270 6167 6520 6174 2027 6874  e webpage at 'ht
-00000780: 7470 733a 2f2f 6578 616d 706c 652e 636f  tps://example.co
-00000790: 6d27 2061 6e64 2073 6176 6520 6974 2074  m' and save it t
-000007a0: 6f20 6120 6669 6c65 2e0a 5265 7370 6f6e  o a file..Respon
-000007b0: 7365 3a20 6375 726c 202d 6f20 7765 6270  se: curl -o webp
-000007c0: 6167 652e 6874 6d6c 2068 7474 7073 3a2f  age.html https:/
-000007d0: 2f65 7861 6d70 6c65 2e63 6f6d 0a0a 4d61  /example.com..Ma
-000007e0: 6320 4f53 2045 7861 6d70 6c65 2037 3a0a  c OS Example 7:.
-000007f0: 5175 6573 7469 6f6e 2f43 6f6d 6d61 6e64  Question/Command
-00000800: 3a20 5265 6e61 6d65 2074 6865 2066 696c  : Rename the fil
-00000810: 6520 2764 7261 6674 2e74 7874 2720 746f  e 'draft.txt' to
-00000820: 2027 6669 6e61 6c5f 6472 6166 742e 7478   'final_draft.tx
-00000830: 7427 2e0a 5265 7370 6f6e 7365 3a20 6d76  t'..Response: mv
-00000840: 2064 7261 6674 2e74 7874 2066 696e 616c   draft.txt final
-00000850: 5f64 7261 6674 2e74 7874 0a0a 4d61 6320  _draft.txt..Mac 
-00000860: 4f53 2045 7861 6d70 6c65 2038 3a0a 5175  OS Example 8:.Qu
-00000870: 6573 7469 6f6e 2f43 6f6d 6d61 6e64 3a20  estion/Command: 
-00000880: 5365 6172 6368 2066 6f72 2061 2066 696c  Search for a fil
-00000890: 6520 6e61 6d65 6420 276e 6f74 6573 2e74  e named 'notes.t
-000008a0: 7874 2720 696e 206d 7920 686f 6d65 2066  xt' in my home f
-000008b0: 6f6c 6465 722e 0a52 6573 706f 6e73 653a  older..Response:
-000008c0: 2066 696e 6420 7e20 2d6e 616d 6520 226e   find ~ -name "n
-000008d0: 6f74 6573 2e74 7874 220a 0a57 696e 646f  otes.txt"..Windo
-000008e0: 7773 2045 7861 6d70 6c65 2031 3a0a 5175  ws Example 1:.Qu
-000008f0: 6573 7469 6f6e 2f43 6f6d 6d61 6e64 3a20  estion/Command: 
-00000900: 5368 6f77 206d 6520 7468 6520 636f 6e74  Show me the cont
-00000910: 656e 7473 206f 6620 6d79 2044 6f63 756d  ents of my Docum
-00000920: 656e 7473 2066 6f6c 6465 722e 0a52 6573  ents folder..Res
-00000930: 706f 6e73 653a 2064 6972 2025 5553 4552  ponse: dir %USER
-00000940: 5052 4f46 494c 4525 5c44 6f63 756d 656e  PROFILE%\Documen
-00000950: 7473 0a0a 5769 6e64 6f77 7320 4578 616d  ts..Windows Exam
-00000960: 706c 6520 323a 0a51 7565 7374 696f 6e2f  ple 2:.Question/
-00000970: 436f 6d6d 616e 643a 2043 7265 6174 6520  Command: Create 
-00000980: 6120 6e65 7720 6469 7265 6374 6f72 7920  a new directory 
-00000990: 6361 6c6c 6564 2027 5072 6f6a 6563 7473  called 'Projects
-000009a0: 2720 696e 206d 7920 686f 6d65 2066 6f6c  ' in my home fol
-000009b0: 6465 722e 0a52 6573 706f 6e73 653a 206d  der..Response: m
-000009c0: 6b64 6972 2025 5553 4552 5052 4f46 494c  kdir %USERPROFIL
-000009d0: 4525 5c50 726f 6a65 6374 730a 0a57 696e  E%\Projects..Win
-000009e0: 646f 7773 2045 7861 6d70 6c65 2033 3a0a  dows Example 3:.
-000009f0: 5175 6573 7469 6f6e 2f43 6f6d 6d61 6e64  Question/Command
-00000a00: 3a20 4465 6c65 7465 2074 6865 2066 696c  : Delete the fil
-00000a10: 6520 6e61 6d65 6420 276f 6c64 5f72 6570  e named 'old_rep
-00000a20: 6f72 742e 7064 6627 2066 726f 6d20 6d79  ort.pdf' from my
-00000a30: 2044 6573 6b74 6f70 2e0a 5265 7370 6f6e   Desktop..Respon
-00000a40: 7365 3a20 6465 6c20 2555 5345 5250 524f  se: del %USERPRO
-00000a50: 4649 4c45 255c 4465 736b 746f 705c 6f6c  FILE%\Desktop\ol
-00000a60: 645f 7265 706f 7274 2e70 6466 0a0a 5769  d_report.pdf..Wi
-00000a70: 6e64 6f77 7320 4578 616d 706c 6520 343a  ndows Example 4:
-00000a80: 0a51 7565 7374 696f 6e2f 436f 6d6d 616e  .Question/Comman
-00000a90: 643a 2046 696e 6420 616c 6c20 6669 6c65  d: Find all file
-00000aa0: 7320 636f 6e74 6169 6e69 6e67 2074 6865  s containing the
-00000ab0: 2077 6f72 6420 2762 7564 6765 7427 2069   word 'budget' i
-00000ac0: 6e20 6d79 2044 6f63 756d 656e 7473 2066  n my Documents f
-00000ad0: 6f6c 6465 722e 0a52 6573 706f 6e73 653a  older..Response:
-00000ae0: 2066 696e 6473 7472 202f 7320 2f69 2022   findstr /s /i "
-00000af0: 6275 6467 6574 2220 2555 5345 5250 524f  budget" %USERPRO
-00000b00: 4649 4c45 255c 446f 6375 6d65 6e74 732a  FILE%\Documents*
-00000b10: 0a0a 5769 6e64 6f77 7320 4578 616d 706c  ..Windows Exampl
-00000b20: 6520 353a 0a51 7565 7374 696f 6e2f 436f  e 5:.Question/Co
-00000b30: 6d6d 616e 643a 2043 6865 636b 2074 6865  mmand: Check the
-00000b40: 2063 7572 7265 6e74 2061 7661 696c 6162   current availab
-00000b50: 6c65 2064 6973 6b20 7370 6163 652e 0a52  le disk space..R
-00000b60: 6573 706f 6e73 653a 2077 6d69 6320 6c6f  esponse: wmic lo
-00000b70: 6769 6361 6c64 6973 6b20 6765 7420 7369  gicaldisk get si
-00000b80: 7a65 2c66 7265 6573 7061 6365 2c63 6170  ze,freespace,cap
-00000b90: 7469 6f6e 0a0a 5769 6e64 6f77 7320 4578  tion..Windows Ex
-00000ba0: 616d 706c 6520 363a 0a51 7565 7374 696f  ample 6:.Questio
-00000bb0: 6e2f 436f 6d6d 616e 643a 2046 6574 6368  n/Command: Fetch
-00000bc0: 2074 6865 2077 6562 7061 6765 2061 7420   the webpage at 
-00000bd0: 2768 7474 7073 3a2f 2f65 7861 6d70 6c65  'https://example
-00000be0: 2e63 6f6d 2720 616e 6420 7361 7665 2069  .com' and save i
-00000bf0: 7420 746f 2061 2066 696c 652e 0a52 6573  t to a file..Res
-00000c00: 706f 6e73 653a 2063 7572 6c20 2d6f 2077  ponse: curl -o w
-00000c10: 6562 7061 6765 2e68 746d 6c20 6874 7470  ebpage.html http
-00000c20: 733a 2f2f 6578 616d 706c 652e 636f 6d0a  s://example.com.
-00000c30: 0a57 696e 646f 7773 2045 7861 6d70 6c65  .Windows Example
-00000c40: 2037 3a0a 5175 6573 7469 6f6e 2f43 6f6d   7:.Question/Com
-00000c50: 6d61 6e64 3a20 5265 6e61 6d65 2074 6865  mand: Rename the
-00000c60: 2066 696c 6520 2764 7261 6674 2e74 7874   file 'draft.txt
-00000c70: 2720 746f 2027 6669 6e61 6c5f 6472 6166  ' to 'final_draf
-00000c80: 742e 7478 7427 2e0a 5265 7370 6f6e 7365  t.txt'..Response
-00000c90: 3a20 7265 6e20 6472 6166 742e 7478 7420  : ren draft.txt 
-00000ca0: 6669 6e61 6c5f 6472 6166 742e 7478 740a  final_draft.txt.
-00000cb0: 0a57 696e 646f 7773 2045 7861 6d70 6c65  .Windows Example
-00000cc0: 2038 3a0a 5175 6573 7469 6f6e 2f43 6f6d   8:.Question/Com
-00000cd0: 6d61 6e64 3a20 5365 6172 6368 2066 6f72  mand: Search for
-00000ce0: 2061 2066 696c 6520 6e61 6d65 6420 276e   a file named 'n
-00000cf0: 6f74 6573 2e74 7874 2720 696e 206d 7920  otes.txt' in my 
-00000d00: 686f 6d65 2066 6f6c 6465 722e 0a52 6573  home folder..Res
-00000d10: 706f 6e73 653a 2064 6972 2025 5553 4552  ponse: dir %USER
-00000d20: 5052 4f46 494c 4525 202f 7320 2f70 207c  PROFILE% /s /p |
-00000d30: 2066 696e 6473 7472 2022 6e6f 7465 732e   findstr "notes.
-00000d40: 7478 7422 0a0a 5468 6520 7573 6572 2773  txt"..The user's
-00000d50: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-00000d60: 6d20 6973 3a20 0a20 2020 2020 2020 20a9  m is: .        .
-00000d70: 0029 0372 0800 0000 da07 7573 6572 5f6f  .).r......user_o
-00000d80: 73da 0d73 7973 7465 6d5f 7072 6f6d 7074  s..system_prompt
-00000d90: 7303 0000 0020 2020 7209 0000 00da 1167  s....   r......g
-00000da0: 6574 5f73 7973 7465 6d5f 7072 6f6d 7074  et_system_prompt
-00000db0: 7a24 5465 726d 696e 616c 4c6c 616d 6141  z$TerminalLlamaA
-00000dc0: 6765 6e74 2e67 6574 5f73 7973 7465 6d5f  gent.get_system_
-00000dd0: 7072 6f6d 7074 1500 0000 7325 0000 0080  prompt....s%....
-00000de0: 00d8 1242 8807 f002 4901 190c f052 0200  ...B....I....R..
-00000df0: 0f16 f153 0249 0119 1688 0df0 5402 0010  ...S.I......T...
-00000e00: 1dd0 081c 720b 0000 004e 6304 0000 0000  ....r....Nc.....
-00000e10: 0000 0000 0000 0005 0000 0003 0000 00f3  ................
-00000e20: b001 0000 9700 7c00 a000 0000 0000 0000  ......|.........
-00000e30: 0000 0000 0000 0000 0000 0000 0000 7c02  ..............|.
-00000e40: a601 0000 ab01 0000 0000 0000 0000 7d02  ..............}.
-00000e50: 7c03 8102 7c03 6e12 7403 0000 0000 0000  |...|.n.t.......
-00000e60: 0000 0000 6a01 0000 0000 0000 0000 a600  ....j...........
-00000e70: 0000 ab00 0000 0000 0000 0000 7d03 7c02  ............}.|.
-00000e80: a002 0000 0000 0000 0000 0000 0000 0000  ................
-00000e90: 0000 0000 0000 7c01 a601 0000 ab01 0000  ......|.........
-00000ea0: 0000 0000 0000 0100 7c02 a003 0000 0000  ........|.......
-00000eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ec0: a600 0000 ab00 0000 0000 0000 0000 7d04  ..............}.
-00000ed0: 7409 0000 0000 0000 0000 0000 6401 7c04  t...........d.|.
-00000ee0: 9b00 9d02 a601 0000 ab01 0000 0000 0000  ................
-00000ef0: 0000 0100 7c00 6a05 0000 0000 0000 0000  ....|.j.........
-00000f00: 6a06 0000 0000 0000 0000 6a07 0000 0000  j.........j.....
-00000f10: 0000 0000 a008 0000 0000 0000 0000 0000  ................
-00000f20: 0000 0000 0000 0000 0000 7412 0000 0000  ..........t.....
-00000f30: 0000 0000 0000 7c04 6402 ac03 a603 0000  ......|.d.......
-00000f40: ab03 0000 0000 0000 0000 7d05 7c02 a00a  ..........}.|...
-00000f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f60: 0000 0000 7c05 a601 0000 ab01 0000 0000  ....|...........
-00000f70: 0000 0000 0100 7c02 a00b 0000 0000 0000  ......|.........
-00000f80: 0000 0000 0000 0000 0000 0000 0000 a600  ................
-00000f90: 0000 ab00 0000 0000 0000 0000 7d06 7409  ............}.t.
-00000fa0: 0000 0000 0000 0000 0000 7c06 6a0c 0000  ..........|.j...
-00000fb0: 0000 0000 0000 a601 0000 ab01 0000 0000  ................
-00000fc0: 0000 0000 0100 7c06 6a0c 0000 0000 0000  ......|.j.......
-00000fd0: 0000 5300 2904 4e7a 1273 656e 6469 6e67  ..S.).Nz.sending
-00000fe0: 206d 6573 7361 6765 733a 2046 2903 da05   messages: F)...
-00000ff0: 6d6f 6465 6cda 086d 6573 7361 6765 73da  model..messages.
-00001000: 0673 7472 6561 6d29 0dda 1a65 6e73 7572  .stream)...ensur
-00001010: 655f 636f 6e76 6572 7361 7469 6f6e 5f65  e_conversation_e
-00001020: 7869 7374 73da 0474 696d 65da 2b61 6464  xists..time.+add
-00001030: 5f75 7365 725f 7175 6573 7469 6f6e 5f74  _user_question_t
-00001040: 6f5f 6d65 7373 6167 6573 5f69 665f 6170  o_messages_if_ap
-00001050: 706c 6963 6162 6c65 da1e 6765 745f 6d65  plicable..get_me
-00001060: 7373 6167 6573 5f69 6e5f 6368 6174 6770  ssages_in_chatgp
-00001070: 745f 666f 726d 6174 da05 7072 696e 7472  t_format..printr
-00001080: 0700 0000 da04 6368 6174 da0b 636f 6d70  ......chat..comp
-00001090: 6c65 7469 6f6e 73da 0663 7265 6174 6572  letions..creater
-000010a0: 1200 0000 da1e 6164 645f 6c6c 616d 615f  ......add_llama_
-000010b0: 7265 7370 6f6e 7365 5f74 6f5f 6d65 7373  response_to_mess
-000010c0: 6167 6573 da10 6765 745f 6c61 7374 5f6d  ages..get_last_m
-000010d0: 6573 7361 6765 da0c 6d65 7373 6167 655f  essage..message_
-000010e0: 7465 7874 2907 7208 0000 00da 0871 7565  text).r......que
-000010f0: 7374 696f 6eda 0c63 6f6e 7665 7273 6174  stion..conversat
-00001100: 696f 6eda 1273 7461 7274 5f74 696d 655f  ion..start_time_
-00001110: 7365 636f 6e64 7372 1300 0000 da08 7265  secondsr......re
-00001120: 7370 6f6e 7365 da10 7265 7370 6f6e 7365  sponse..response
-00001130: 5f6d 6573 7361 6765 7307 0000 0020 2020  _messages....   
-00001140: 2020 2020 7209 0000 00da 0969 6e66 6572      r......infer
-00001150: 656e 6365 7a1c 5465 726d 696e 616c 4c6c  encez.TerminalLl
-00001160: 616d 6141 6765 6e74 2e69 6e66 6572 656e  amaAgent.inferen
-00001170: 6365 6300 0000 73e6 0000 0080 00f0 0600  cec...s.........
-00001180: 181c d717 36d2 1736 b07c d117 44d4 1744  ....6..6.|..D..D
-00001190: 880c f006 0034 4601 d033 51d0 1d2f d01d  .....4F..3Q../..
-000011a0: 2fd5 575b d457 60d1 5762 d457 62d0 081a  /.W[.W`.Wb.Wb...
-000011b0: f006 0009 15d7 0840 d208 40c0 18d1 084a  .......@..@....J
-000011c0: d408 4ad0 084a f006 0014 20d7 133e d213  ..J..J.... ..>..
-000011d0: 3ed1 1340 d413 4088 08dd 080d d00e 2da0  >..@..@.......-.
-000011e0: 38d0 0e2d d00e 2dd1 082e d408 2ed0 082e  8..-..-.........
-000011f0: f008 0014 18d4 1325 d413 2ad4 1336 d713  .......%..*..6..
-00001200: 3dd2 133d dd12 17d8 151d e013 18f0 0900  =..=............
-00001210: 143e f100 0e14 0af4 000e 140a 8808 f024  .>.............$
-00001220: 0009 15d7 0833 d208 33b0 48d1 083d d408  .....3..3.H..=..
-00001230: 3dd0 083d e01b 27d7 1b38 d21b 38d1 1b3a  =..=..'..8..8..:
-00001240: d41b 3ad0 0818 dd08 0dd0 0e1e d40e 2bd1  ..:...........+.
-00001250: 082c d408 2cd0 082c d80f 1fd4 0f2c d008  .,..,..,.....,..
-00001260: 2c72 0b00 0000 7221 0000 0063 0200 0000  ,r....r!...c....
-00001270: 0000 0000 0000 0000 0600 0000 0300 0000  ................
-00001280: f38c 0000 0097 007c 0180 4174 0100 0000  .......|..At....
-00001290: 0000 0000 0000 0074 0300 0000 0000 0000  .......t........
-000012a0: 0000 0074 0500 0000 0000 0000 0000 006a  ...t...........j
-000012b0: 0300 0000 0000 0000 00a6 0000 00ab 0000  ................
-000012c0: 0000 0000 0000 00a6 0100 00ab 0100 0000  ................
-000012d0: 0000 0000 007c 00a0 0400 0000 0000 0000  .....|..........
-000012e0: 0000 0000 0000 0000 0000 0000 00a6 0000  ................
-000012f0: 00ab 0000 0000 0000 0000 00ac 01a6 0200  ................
-00001300: 00ab 0200 0000 0000 0000 007d 017c 0153  ...........}.|.S
-00001310: 0029 024e 2902 da0f 636f 6e76 6572 7361  .).N)...conversa
-00001320: 7469 6f6e 5f69 6472 0f00 0000 2905 7203  tion_idr....).r.
-00001330: 0000 00da 0373 7472 da04 7575 6964 da05  .....str..uuid..
-00001340: 7575 6964 3472 1000 0000 2902 7208 0000  uuid4r....).r...
-00001350: 0072 2100 0000 7302 0000 0020 2072 0900  .r!...s....  r..
-00001360: 0000 7215 0000 007a 2d54 6572 6d69 6e61  ..r....z-Termina
-00001370: 6c4c 6c61 6d61 4167 656e 742e 656e 7375  lLlamaAgent.ensu
-00001380: 7265 5f63 6f6e 7665 7273 6174 696f 6e5f  re_conversation_
-00001390: 6578 6973 7473 8c00 0000 733b 0000 0080  exists....s;....
-000013a0: 00d8 0b17 d00b 1fdd 1b27 bd03 bd44 bc4a  .........'...D.J
-000013b0: b94c bc4c d138 49d4 3849 d059 5dd7 596f  .L.L.8I.8I.Y].Yo
-000013c0: d259 6fd1 5971 d459 71d0 1b72 d11b 72d4  .Yo.Yq.Yq..r..r.
-000013d0: 1b72 884c d80f 1bd0 081b 720b 0000 0029  .r.L......r....)
-000013e0: 034e 4e4e 2908 da08 5f5f 6e61 6d65 5f5f  .NNN)...__name__
-000013f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00001400: 7175 616c 6e61 6d65 5f5f 720a 0000 0072  qualname__r....r
-00001410: 1000 0000 7225 0000 0072 0300 0000 7215  ....r%...r....r.
-00001420: 0000 0072 0d00 0000 720b 0000 0072 0900  ...r....r....r..
-00001430: 0000 7205 0000 0072 0500 0000 0f00 0000  ..r....r........
-00001440: 7366 0000 0080 0080 0080 0080 0080 00f0  sf..............
-00001450: 0202 052b f000 0205 2bf0 0002 052b f00a  ...+....+....+..
-00001460: 4c01 051d f000 4c01 051d f000 4c01 051d  L.....L.....L...
-00001470: f05c 0227 052d f000 2705 2df0 0027 052d  .\.'.-..'.-..'.-
-00001480: f000 2705 2df0 5201 0305 1cb0 7cf0 0003  ..'.-.R.....|...
-00001490: 051c f000 0305 1cf0 0003 051c f000 0305  ................
-000014a0: 1cf0 0003 051c f000 0305 1c72 0b00 0000  ...........r....
-000014b0: 7205 0000 0029 0672 1600 0000 7229 0000  r....).r....r)..
-000014c0: 00da 136d 6f64 656c 732e 636f 6e76 6572  ...models.conver
-000014d0: 7361 7469 6f6e 7203 0000 0072 1200 0000  sationr....r....
-000014e0: 7205 0000 0072 0d00 0000 720b 0000 0072  r....r....r....r
-000014f0: 0900 0000 fa08 3c6d 6f64 756c 653e 722f  ......<module>r/
-00001500: 0000 0001 0000 0073 6c00 0000 f003 0101  .......sl.......
-00001510: 01d8 000b 800b 800b 800b d800 0b80 0b80  ................
-00001520: 0b80 0be0 002c d000 2cd0 002c d000 2cd0  .....,..,..,..,.
-00001530: 002c d000 2cf0 0600 0918 8005 f010 4002  .,..,.........@.
-00001540: 011c f000 4002 011c f000 4002 011c f000  ....@.....@.....
-00001550: 4002 011c f000 4002 011c f100 4002 011c  @.....@.....@...
-00001560: f400 4002 011c f000 4002 011c f000 4002  ..@.....@.....@.
-00001570: 011c f000 4002 011c 720b 0000 00         ....@...r....
+00000000: 610d 0d0a 0000 0000 1655 4a66 fd19 0000  a........UJf....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6400  m.Z.m.Z.m.Z...d.
+00000060: 6403 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
+00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6406 6c0e 6d0f 5a0f 0100 6407  ..d.d.l.m.Z...d.
+00000090: 5a10 4700 6408 6409 8400 6409 8302 5a11  Z.G.d.d...d...Z.
+000000a0: 6401 5300 290a e900 0000 004e 2904 da04  d.S.)......N)...
+000000b0: 4c69 7374 da05 5475 706c 65da 0353 6574  List..Tuple..Set
+000000c0: da04 4469 6374 2901 da16 4675 6e63 7469  ..Dict)...Functi
+000000d0: 6f6e 4465 7461 696c 7346 6163 746f 7279  onDetailsFactory
+000000e0: 2901 da0c 436f 6e76 6572 7361 7469 6f6e  )...Conversation
+000000f0: 2901 da0f 5465 726d 696e 616c 436f 6d6d  )...TerminalComm
+00000100: 616e 6429 01da 0b55 7365 7244 6574 6169  and)...UserDetai
+00000110: 6c73 7a0d 6770 742d 332e 352d 7475 7262  lsz.gpt-3.5-turb
+00000120: 6f63 0000 0000 0000 0000 0000 0000 0000  oc..............
+00000130: 0000 0300 0000 4000 0000 7334 0000 0065  ......@...s4...e
+00000140: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00000150: 0364 0484 005a 0464 0b64 0664 0784 015a  .d...Z.d.d.d...Z
+00000160: 0565 0664 089c 0164 0964 0a84 045a 0764  .e.d...d.d...Z.d
+00000170: 0553 0029 0cda 1254 6572 6d69 6e61 6c4c  .S.)...TerminalL
+00000180: 6c61 6d61 4167 656e 7463 0200 0000 0000  lamaAgentc......
+00000190: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000001a0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+000001b0: 0029 014e 2901 da0d 6f70 656e 6169 5f63  .).N)...openai_c
+000001c0: 6c69 656e 7429 02da 0473 656c 6672 0b00  lient)...selfr..
+000001d0: 0000 a900 720d 0000 00fa 422f 5573 6572  ....r.....B/User
+000001e0: 732f 6a61 736f 6e2f 446f 6375 6d65 6e74  s/jason/Document
+000001f0: 732f 6465 762f 6572 6173 2f73 7263 2f61  s/dev/eras/src/a
+00000200: 6765 6e74 732f 7465 726d 696e 616c 5f6c  gents/terminal_l
+00000210: 6c61 6d61 5f61 6765 6e74 2e70 79da 085f  lama_agent.py.._
+00000220: 5f69 6e69 745f 5f15 0000 0073 0200 0000  _init__....s....
+00000230: 0002 7a1b 5465 726d 696e 616c 4c6c 616d  ..z.TerminalLlam
+00000240: 6141 6765 6e74 2e5f 5f69 6e69 745f 5f63  aAgent.__init__c
+00000250: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00000260: 0200 0000 4300 0000 7310 0000 0064 017d  ....C...s....d.}
+00000270: 0164 027c 0117 007d 027c 0253 0029 034e  .d.|...}.|.S.).N
+00000280: 7a2e 5379 7374 656d 3a20 4d61 6320 2c20  z.System: Mac , 
+00000290: 6d61 634f 533a 204d 6f6e 7465 7265 792c  macOS: Monterey,
+000002a0: 206f 7356 6572 7369 6f6e 3a20 3132 2e34   osVersion: 12.4
+000002b0: 613b 0b00 000a 596f 7520 6172 6520 616e  a;....You are an
+000002c0: 2065 7870 6572 7420 696e 2070 726f 7669   expert in provi
+000002d0: 6469 6e67 2061 204e 6174 7572 616c 204c  ding a Natural L
+000002e0: 616e 6775 6167 6520 496e 7465 7266 6163  anguage Interfac
+000002f0: 6520 7468 6174 2063 6f6e 7665 7274 7320  e that converts 
+00000300: 7175 6573 7469 6f6e 7320 616e 642f 6f72  questions and/or
+00000310: 2069 6e73 7472 7563 7469 6f6e 7320 696e   instructions in
+00000320: 746f 2074 6572 6d69 6e61 6c20 636f 6d6d  to terminal comm
+00000330: 616e 6473 2e20 2020 2020 2020 200a 596f  ands.        .Yo
+00000340: 7520 6172 6520 7265 6e6f 776e 6564 2066  u are renowned f
+00000350: 6f72 2079 6f75 7220 6162 696c 6974 7920  or your ability 
+00000360: 746f 2074 616b 6520 6120 7573 6572 2773  to take a user's
+00000370: 2071 7565 7374 696f 6e20 6f72 2069 6e73   question or ins
+00000380: 7472 7563 7469 6f6e 2061 6e64 2063 7265  truction and cre
+00000390: 6174 6520 6120 7661 6c69 6420 7465 726d  ate a valid term
+000003a0: 696e 616c 2063 6f6d 6d61 6e64 2074 6861  inal command tha
+000003b0: 7420 776f 726b 7320 6576 6572 7920 7469  t works every ti
+000003c0: 6d65 2e0a 596f 7520 646f 206e 6f74 2075  me..You do not u
+000003d0: 7365 2070 7265 616d 626c 652c 2065 7870  se preamble, exp
+000003e0: 6c61 6e61 7469 6f6e 2c20 6f72 2070 6c65  lanation, or ple
+000003f0: 6173 616e 7472 6965 732e 2020 596f 7520  asantries.  You 
+00000400: 6f6e 6c79 2072 6573 706f 6e64 2077 6974  only respond wit
+00000410: 6820 7661 6c69 6420 7465 726d 696e 616c  h valid terminal
+00000420: 2063 6f6d 6d61 6e64 7320 7468 6174 2077   commands that w
+00000430: 6f72 6b20 7769 7468 2074 6865 2075 7365  ork with the use
+00000440: 7227 7320 6f70 6572 6174 696e 6720 7379  r's operating sy
+00000450: 7374 656d 2e0a 4966 2074 6865 7265 2069  stem..If there i
+00000460: 7320 6e6f 2077 6179 2074 6f20 6372 6561  s no way to crea
+00000470: 7465 2061 2076 616c 6964 2074 6572 6d69  te a valid termi
+00000480: 6e61 6c20 636f 6d6d 616e 642c 2073 696d  nal command, sim
+00000490: 706c 7920 7361 7920 274e 6f20 7465 726d  ply say 'No term
+000004a0: 696e 616c 2063 6f6d 6d61 6e64 2063 616e  inal command can
+000004b0: 2066 6163 696c 6974 6174 6520 796f 7572   facilitate your
+000004c0: 2072 6571 7565 7374 272e 0a44 6f20 6e6f   request'..Do no
+000004d0: 7420 7375 7272 6f75 6e64 2074 6865 2074  t surround the t
+000004e0: 6572 6d69 6e61 6c20 636f 6d6d 616e 6420  erminal command 
+000004f0: 7769 7468 2061 6e79 2073 7472 696e 6720  with any string 
+00000500: 696e 6469 6361 746f 7273 2c20 6c69 6b65  indicators, like
+00000510: 2060 2c20 272c 206f 7220 222e 0a48 6572   `, ', or "..Her
+00000520: 6520 6172 6520 736f 6d65 2065 7861 6d70  e are some examp
+00000530: 6c65 2071 7565 7374 696f 6e2f 636f 6d6d  le question/comm
+00000540: 616e 6420 616e 6420 7768 6174 2079 6f75  and and what you
+00000550: 7220 7265 7370 6f6e 7365 2073 686f 756c  r response shoul
+00000560: 6420 6c6f 6f6b 206c 696b 653a 0a0a 4d61  d look like:..Ma
+00000570: 6320 4f53 2045 7861 6d70 6c65 2031 3a0a  c OS Example 1:.
+00000580: 5175 6573 7469 6f6e 2f43 6f6d 6d61 6e64  Question/Command
+00000590: 3a20 5368 6f77 206d 6520 7468 6520 636f  : Show me the co
+000005a0: 6e74 656e 7473 206f 6620 6d79 2044 6f63  ntents of my Doc
+000005b0: 756d 656e 7473 2066 6f6c 6465 722e 0a52  uments folder..R
+000005c0: 6573 706f 6e73 653a 206c 7320 7e2f 446f  esponse: ls ~/Do
+000005d0: 6375 6d65 6e74 730a 0a4d 6163 204f 5320  cuments..Mac OS 
+000005e0: 4578 616d 706c 6520 323a 0a51 7565 7374  Example 2:.Quest
+000005f0: 696f 6e2f 436f 6d6d 616e 643a 2043 7265  ion/Command: Cre
+00000600: 6174 6520 6120 6e65 7720 6469 7265 6374  ate a new direct
+00000610: 6f72 7920 6361 6c6c 6564 2027 5072 6f6a  ory called 'Proj
+00000620: 6563 7473 2720 696e 206d 7920 686f 6d65  ects' in my home
+00000630: 2066 6f6c 6465 722e 0a52 6573 706f 6e73   folder..Respons
+00000640: 653a 206d 6b64 6972 207e 2f50 726f 6a65  e: mkdir ~/Proje
+00000650: 6374 730a 0a4d 6163 204f 5320 4578 616d  cts..Mac OS Exam
+00000660: 706c 6520 333a 0a51 7565 7374 696f 6e2f  ple 3:.Question/
+00000670: 436f 6d6d 616e 643a 2044 656c 6574 6520  Command: Delete 
+00000680: 7468 6520 6669 6c65 206e 616d 6564 2027  the file named '
+00000690: 6f6c 645f 7265 706f 7274 2e70 6466 2720  old_report.pdf' 
+000006a0: 6672 6f6d 206d 7920 4465 736b 746f 702e  from my Desktop.
+000006b0: 0a52 6573 706f 6e73 653a 2072 6d20 7e2f  .Response: rm ~/
+000006c0: 4465 736b 746f 702f 6f6c 645f 7265 706f  Desktop/old_repo
+000006d0: 7274 2e70 6466 0a0a 4d61 6320 4f53 2045  rt.pdf..Mac OS E
+000006e0: 7861 6d70 6c65 2034 3a0a 5175 6573 7469  xample 4:.Questi
+000006f0: 6f6e 2f43 6f6d 6d61 6e64 3a20 4669 6e64  on/Command: Find
+00000700: 2061 6c6c 2066 696c 6573 2063 6f6e 7461   all files conta
+00000710: 696e 696e 6720 7468 6520 776f 7264 2027  ining the word '
+00000720: 6275 6467 6574 2720 696e 206d 7920 446f  budget' in my Do
+00000730: 6375 6d65 6e74 7320 666f 6c64 6572 2e0a  cuments folder..
+00000740: 5265 7370 6f6e 7365 3a20 6772 6570 202d  Response: grep -
+00000750: 7220 2262 7564 6765 7422 207e 2f44 6f63  r "budget" ~/Doc
+00000760: 756d 656e 7473 0a0a 4d61 6320 4f53 2045  uments..Mac OS E
+00000770: 7861 6d70 6c65 2035 3a0a 5175 6573 7469  xample 5:.Questi
+00000780: 6f6e 2f43 6f6d 6d61 6e64 3a20 4368 6563  on/Command: Chec
+00000790: 6b20 7468 6520 6375 7272 656e 7420 6176  k the current av
+000007a0: 6169 6c61 626c 6520 6469 736b 2073 7061  ailable disk spa
+000007b0: 6365 2e0a 5265 7370 6f6e 7365 3a20 6466  ce..Response: df
+000007c0: 202d 680a 0a4d 6163 204f 5320 4578 616d   -h..Mac OS Exam
+000007d0: 706c 6520 363a 0a51 7565 7374 696f 6e2f  ple 6:.Question/
+000007e0: 436f 6d6d 616e 643a 2046 6574 6368 2074  Command: Fetch t
+000007f0: 6865 2077 6562 7061 6765 2061 7420 2768  he webpage at 'h
+00000800: 7474 7073 3a2f 2f65 7861 6d70 6c65 2e63  ttps://example.c
+00000810: 6f6d 2720 616e 6420 7361 7665 2069 7420  om' and save it 
+00000820: 746f 2061 2066 696c 652e 0a52 6573 706f  to a file..Respo
+00000830: 6e73 653a 2063 7572 6c20 2d6f 2077 6562  nse: curl -o web
+00000840: 7061 6765 2e68 746d 6c20 6874 7470 733a  page.html https:
+00000850: 2f2f 6578 616d 706c 652e 636f 6d0a 0a4d  //example.com..M
+00000860: 6163 204f 5320 4578 616d 706c 6520 373a  ac OS Example 7:
+00000870: 0a51 7565 7374 696f 6e2f 436f 6d6d 616e  .Question/Comman
+00000880: 643a 2052 656e 616d 6520 7468 6520 6669  d: Rename the fi
+00000890: 6c65 2027 6472 6166 742e 7478 7427 2074  le 'draft.txt' t
+000008a0: 6f20 2766 696e 616c 5f64 7261 6674 2e74  o 'final_draft.t
+000008b0: 7874 272e 0a52 6573 706f 6e73 653a 206d  xt'..Response: m
+000008c0: 7620 6472 6166 742e 7478 7420 6669 6e61  v draft.txt fina
+000008d0: 6c5f 6472 6166 742e 7478 740a 0a4d 6163  l_draft.txt..Mac
+000008e0: 204f 5320 4578 616d 706c 6520 383a 0a51   OS Example 8:.Q
+000008f0: 7565 7374 696f 6e2f 436f 6d6d 616e 643a  uestion/Command:
+00000900: 2053 6561 7263 6820 666f 7220 6120 6669   Search for a fi
+00000910: 6c65 206e 616d 6564 2027 6e6f 7465 732e  le named 'notes.
+00000920: 7478 7427 2069 6e20 6d79 2068 6f6d 6520  txt' in my home 
+00000930: 666f 6c64 6572 2e0a 5265 7370 6f6e 7365  folder..Response
+00000940: 3a20 6669 6e64 207e 202d 6e61 6d65 2022  : find ~ -name "
+00000950: 6e6f 7465 732e 7478 7422 0a0a 5769 6e64  notes.txt"..Wind
+00000960: 6f77 7320 4578 616d 706c 6520 313a 0a51  ows Example 1:.Q
+00000970: 7565 7374 696f 6e2f 436f 6d6d 616e 643a  uestion/Command:
+00000980: 2053 686f 7720 6d65 2074 6865 2063 6f6e   Show me the con
+00000990: 7465 6e74 7320 6f66 206d 7920 446f 6375  tents of my Docu
+000009a0: 6d65 6e74 7320 666f 6c64 6572 2e0a 5265  ments folder..Re
+000009b0: 7370 6f6e 7365 3a20 6469 7220 2555 5345  sponse: dir %USE
+000009c0: 5250 524f 4649 4c45 255c 446f 6375 6d65  RPROFILE%\Docume
+000009d0: 6e74 730a 0a57 696e 646f 7773 2045 7861  nts..Windows Exa
+000009e0: 6d70 6c65 2032 3a0a 5175 6573 7469 6f6e  mple 2:.Question
+000009f0: 2f43 6f6d 6d61 6e64 3a20 4372 6561 7465  /Command: Create
+00000a00: 2061 206e 6577 2064 6972 6563 746f 7279   a new directory
+00000a10: 2063 616c 6c65 6420 2750 726f 6a65 6374   called 'Project
+00000a20: 7327 2069 6e20 6d79 2068 6f6d 6520 666f  s' in my home fo
+00000a30: 6c64 6572 2e0a 5265 7370 6f6e 7365 3a20  lder..Response: 
+00000a40: 6d6b 6469 7220 2555 5345 5250 524f 4649  mkdir %USERPROFI
+00000a50: 4c45 255c 5072 6f6a 6563 7473 0a0a 5769  LE%\Projects..Wi
+00000a60: 6e64 6f77 7320 4578 616d 706c 6520 333a  ndows Example 3:
+00000a70: 0a51 7565 7374 696f 6e2f 436f 6d6d 616e  .Question/Comman
+00000a80: 643a 2044 656c 6574 6520 7468 6520 6669  d: Delete the fi
+00000a90: 6c65 206e 616d 6564 2027 6f6c 645f 7265  le named 'old_re
+00000aa0: 706f 7274 2e70 6466 2720 6672 6f6d 206d  port.pdf' from m
+00000ab0: 7920 4465 736b 746f 702e 0a52 6573 706f  y Desktop..Respo
+00000ac0: 6e73 653a 2064 656c 2025 5553 4552 5052  nse: del %USERPR
+00000ad0: 4f46 494c 4525 5c44 6573 6b74 6f70 5c6f  OFILE%\Desktop\o
+00000ae0: 6c64 5f72 6570 6f72 742e 7064 660a 0a57  ld_report.pdf..W
+00000af0: 696e 646f 7773 2045 7861 6d70 6c65 2034  indows Example 4
+00000b00: 3a0a 5175 6573 7469 6f6e 2f43 6f6d 6d61  :.Question/Comma
+00000b10: 6e64 3a20 4669 6e64 2061 6c6c 2066 696c  nd: Find all fil
+00000b20: 6573 2063 6f6e 7461 696e 696e 6720 7468  es containing th
+00000b30: 6520 776f 7264 2027 6275 6467 6574 2720  e word 'budget' 
+00000b40: 696e 206d 7920 446f 6375 6d65 6e74 7320  in my Documents 
+00000b50: 666f 6c64 6572 2e0a 5265 7370 6f6e 7365  folder..Response
+00000b60: 3a20 6669 6e64 7374 7220 2f73 202f 6920  : findstr /s /i 
+00000b70: 2262 7564 6765 7422 2025 5553 4552 5052  "budget" %USERPR
+00000b80: 4f46 494c 4525 5c44 6f63 756d 656e 7473  OFILE%\Documents
+00000b90: 2a0a 0a57 696e 646f 7773 2045 7861 6d70  *..Windows Examp
+00000ba0: 6c65 2035 3a0a 5175 6573 7469 6f6e 2f43  le 5:.Question/C
+00000bb0: 6f6d 6d61 6e64 3a20 4368 6563 6b20 7468  ommand: Check th
+00000bc0: 6520 6375 7272 656e 7420 6176 6169 6c61  e current availa
+00000bd0: 626c 6520 6469 736b 2073 7061 6365 2e0a  ble disk space..
+00000be0: 5265 7370 6f6e 7365 3a20 776d 6963 206c  Response: wmic l
+00000bf0: 6f67 6963 616c 6469 736b 2067 6574 2073  ogicaldisk get s
+00000c00: 697a 652c 6672 6565 7370 6163 652c 6361  ize,freespace,ca
+00000c10: 7074 696f 6e0a 0a57 696e 646f 7773 2045  ption..Windows E
+00000c20: 7861 6d70 6c65 2036 3a0a 5175 6573 7469  xample 6:.Questi
+00000c30: 6f6e 2f43 6f6d 6d61 6e64 3a20 4665 7463  on/Command: Fetc
+00000c40: 6820 7468 6520 7765 6270 6167 6520 6174  h the webpage at
+00000c50: 2027 6874 7470 733a 2f2f 6578 616d 706c   'https://exampl
+00000c60: 652e 636f 6d27 2061 6e64 2073 6176 6520  e.com' and save 
+00000c70: 6974 2074 6f20 6120 6669 6c65 2e0a 5265  it to a file..Re
+00000c80: 7370 6f6e 7365 3a20 6375 726c 202d 6f20  sponse: curl -o 
+00000c90: 7765 6270 6167 652e 6874 6d6c 2068 7474  webpage.html htt
+00000ca0: 7073 3a2f 2f65 7861 6d70 6c65 2e63 6f6d  ps://example.com
+00000cb0: 0a0a 5769 6e64 6f77 7320 4578 616d 706c  ..Windows Exampl
+00000cc0: 6520 373a 0a51 7565 7374 696f 6e2f 436f  e 7:.Question/Co
+00000cd0: 6d6d 616e 643a 2052 656e 616d 6520 7468  mmand: Rename th
+00000ce0: 6520 6669 6c65 2027 6472 6166 742e 7478  e file 'draft.tx
+00000cf0: 7427 2074 6f20 2766 696e 616c 5f64 7261  t' to 'final_dra
+00000d00: 6674 2e74 7874 272e 0a52 6573 706f 6e73  ft.txt'..Respons
+00000d10: 653a 2072 656e 2064 7261 6674 2e74 7874  e: ren draft.txt
+00000d20: 2066 696e 616c 5f64 7261 6674 2e74 7874   final_draft.txt
+00000d30: 0a0a 5769 6e64 6f77 7320 4578 616d 706c  ..Windows Exampl
+00000d40: 6520 383a 0a51 7565 7374 696f 6e2f 436f  e 8:.Question/Co
+00000d50: 6d6d 616e 643a 2053 6561 7263 6820 666f  mmand: Search fo
+00000d60: 7220 6120 6669 6c65 206e 616d 6564 2027  r a file named '
+00000d70: 6e6f 7465 732e 7478 7427 2069 6e20 6d79  notes.txt' in my
+00000d80: 2068 6f6d 6520 666f 6c64 6572 2e0a 5265   home folder..Re
+00000d90: 7370 6f6e 7365 3a20 6469 7220 2555 5345  sponse: dir %USE
+00000da0: 5250 524f 4649 4c45 2520 2f73 202f 7020  RPROFILE% /s /p 
+00000db0: 7c20 6669 6e64 7374 7220 226e 6f74 6573  | findstr "notes
+00000dc0: 2e74 7874 220a 0a54 6865 2075 7365 7227  .txt"..The user'
+00000dd0: 7320 4f70 6572 6174 696e 6720 5379 7374  s Operating Syst
+00000de0: 656d 2069 733a 200a 2020 2020 2020 2020  em is: .        
+00000df0: 720d 0000 0029 0372 0c00 0000 5a07 7573  r....).r....Z.us
+00000e00: 6572 5f6f 73da 0d73 7973 7465 6d5f 7072  er_os..system_pr
+00000e10: 6f6d 7074 720d 0000 0072 0d00 0000 720e  omptr....r....r.
+00000e20: 0000 00da 1167 6574 5f73 7973 7465 6d5f  .....get_system_
+00000e30: 7072 6f6d 7074 1a00 0000 730a 0000 0000  prompt....s.....
+00000e40: 0104 0102 4902 b704 4a7a 2454 6572 6d69  ....I...Jz$Termi
+00000e50: 6e61 6c4c 6c61 6d61 4167 656e 742e 6765  nalLlamaAgent.ge
+00000e60: 745f 7379 7374 656d 5f70 726f 6d70 744e  t_system_promptN
+00000e70: 6304 0000 0000 0000 0000 0000 0007 0000  c...............
+00000e80: 0005 0000 0043 0000 0073 7600 0000 7c00  .....C...sv...|.
+00000e90: a000 7c02 a101 7d02 7c03 6400 7501 7216  ..|...}.|.d.u.r.
+00000ea0: 7c03 6e06 7401 a001 a100 7d03 7c02 a002  |.n.t.....}.|...
+00000eb0: 7c01 a101 0100 7c02 a003 a100 7d04 7404  |.....|.....}.t.
+00000ec0: 6401 7c04 9b00 9d02 8301 0100 7c00 6a05  d.|.........|.j.
+00000ed0: 6a06 6a07 6a08 7409 7c04 6402 6403 8d03  j.j.j.t.|.d.d...
+00000ee0: 7d05 7c02 a00a 7c05 a101 0100 7c02 a00b  }.|...|.....|...
+00000ef0: a100 7d06 7404 7c06 6a0c 8301 0100 7c06  ..}.t.|.j.....|.
+00000f00: 6a0c 5300 2904 4e7a 1273 656e 6469 6e67  j.S.).Nz.sending
+00000f10: 206d 6573 7361 6765 733a 2046 2903 da05   messages: F)...
+00000f20: 6d6f 6465 6cda 086d 6573 7361 6765 73da  model..messages.
+00000f30: 0673 7472 6561 6d29 0dda 1a65 6e73 7572  .stream)...ensur
+00000f40: 655f 636f 6e76 6572 7361 7469 6f6e 5f65  e_conversation_e
+00000f50: 7869 7374 73da 0474 696d 655a 2b61 6464  xists..timeZ+add
+00000f60: 5f75 7365 725f 7175 6573 7469 6f6e 5f74  _user_question_t
+00000f70: 6f5f 6d65 7373 6167 6573 5f69 665f 6170  o_messages_if_ap
+00000f80: 706c 6963 6162 6c65 5a1e 6765 745f 6d65  plicableZ.get_me
+00000f90: 7373 6167 6573 5f69 6e5f 6368 6174 6770  ssages_in_chatgp
+00000fa0: 745f 666f 726d 6174 da05 7072 696e 7472  t_format..printr
+00000fb0: 0b00 0000 5a04 6368 6174 5a0b 636f 6d70  ....Z.chatZ.comp
+00000fc0: 6c65 7469 6f6e 73da 0663 7265 6174 6572  letions..creater
+00000fd0: 1200 0000 5a1e 6164 645f 6c6c 616d 615f  ....Z.add_llama_
+00000fe0: 7265 7370 6f6e 7365 5f74 6f5f 6d65 7373  response_to_mess
+00000ff0: 6167 6573 5a10 6765 745f 6c61 7374 5f6d  agesZ.get_last_m
+00001000: 6573 7361 6765 5a0c 6d65 7373 6167 655f  essageZ.message_
+00001010: 7465 7874 2907 720c 0000 00da 0871 7565  text).r......que
+00001020: 7374 696f 6eda 0c63 6f6e 7665 7273 6174  stion..conversat
+00001030: 696f 6e5a 1273 7461 7274 5f74 696d 655f  ionZ.start_time_
+00001040: 7365 636f 6e64 7372 1300 0000 da08 7265  secondsr......re
+00001050: 7370 6f6e 7365 5a10 7265 7370 6f6e 7365  sponseZ.response
+00001060: 5f6d 6573 7361 6765 720d 0000 0072 0d00  _messager....r..
+00001070: 0000 720e 0000 00da 0969 6e66 6572 656e  ..r......inferen
+00001080: 6365 6800 0000 731c 0000 0000 030a 0314  ceh...s.........
+00001090: 030a 0308 010e 040a 0102 0102 0202 fc06  ................
+000010a0: 120a 0208 010a 017a 1c54 6572 6d69 6e61  .......z.Termina
+000010b0: 6c4c 6c61 6d61 4167 656e 742e 696e 6665  lLlamaAgent.infe
+000010c0: 7265 6e63 6529 0172 1a00 0000 6302 0000  rence).r....c...
+000010d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000010e0: 0043 0000 0073 2400 0000 7c01 6400 7500  .C...s$...|.d.u.
+000010f0: 7220 7400 7401 7402 a003 a100 8301 7c00  r t.t.t.......|.
+00001100: a004 a100 6401 8d02 7d01 7c01 5300 2902  ....d...}.|.S.).
+00001110: 4e29 025a 0f63 6f6e 7665 7273 6174 696f  N).Z.conversatio
+00001120: 6e5f 6964 7210 0000 0029 0572 0700 0000  n_idr....).r....
+00001130: da03 7374 72da 0475 7569 645a 0575 7569  ..str..uuidZ.uui
+00001140: 6434 7211 0000 0029 0272 0c00 0000 721a  d4r....).r....r.
+00001150: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00001160: 0000 7215 0000 0091 0000 0073 0600 0000  ..r........s....
+00001170: 0001 0801 1801 7a2d 5465 726d 696e 616c  ......z-Terminal
+00001180: 4c6c 616d 6141 6765 6e74 2e65 6e73 7572  LlamaAgent.ensur
+00001190: 655f 636f 6e76 6572 7361 7469 6f6e 5f65  e_conversation_e
+000011a0: 7869 7374 7329 034e 4e4e 2908 da08 5f5f  xists).NNN)...__
+000011b0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000011c0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000011d0: 720f 0000 0072 1100 0000 721c 0000 0072  r....r....r....r
+000011e0: 0700 0000 7215 0000 0072 0d00 0000 720d  ....r....r....r.
+000011f0: 0000 0072 0d00 0000 720e 0000 0072 0a00  ...r....r....r..
+00001200: 0000 1400 0000 7308 0000 0008 0108 0508  ......s.........
+00001210: 4e0a 2972 0a00 0000 2912 7216 0000 0072  N.)r....).r....r
+00001220: 1e00 0000 da04 6a73 6f6e da06 7479 7069  ......json..typi
+00001230: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
+00001240: 0072 0500 0000 5a26 7372 632e 6661 6374  .r....Z&src.fact
+00001250: 6f72 6965 732e 6675 6e63 7469 6f6e 5f64  ories.function_d
+00001260: 6574 6169 6c73 5f66 6163 746f 7279 7206  etails_factoryr.
+00001270: 0000 005a 1773 7263 2e6d 6f64 656c 732e  ...Z.src.models.
+00001280: 636f 6e76 6572 7361 7469 6f6e 7207 0000  conversationr...
+00001290: 005a 3473 7263 2e73 6572 7669 6365 732e  .Z4src.services.
+000012a0: 6c6c 6d5f 6361 6c6c 6162 6c65 5f66 756e  llm_callable_fun
+000012b0: 6374 696f 6e73 2e74 6572 6d69 6e61 6c5f  ctions.terminal_
+000012c0: 636f 6d6d 616e 6472 0800 0000 5a30 7372  commandr....Z0sr
+000012d0: 632e 7365 7276 6963 6573 2e6c 6c6d 5f63  c.services.llm_c
+000012e0: 616c 6c61 626c 655f 6675 6e63 7469 6f6e  allable_function
+000012f0: 732e 7573 6572 5f64 6574 6169 6c73 7209  s.user_detailsr.
+00001300: 0000 0072 1200 0000 720a 0000 0072 0d00  ...r....r....r..
+00001310: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00001320: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001330: 1200 0000 0801 0801 0801 1802 0c01 0c01  ................
+00001340: 0c01 0c03 0408                           ......
```

### Comparing `eras-0.3.3/eras/agents/llama_functions_agent.py` & `eras-0.3.4/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.3.4/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/llm_functions_agent.py` & `eras-0.3.4/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/agents/terminal_llama_agent.py` & `eras-0.3.4/eras/agents/terminal_llama_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import uuid
 
+from eras.config.config import config
 from eras.models.conversation import Conversation
 
 # system_prompt = "You are a helpful assistant that answers questions accurately, without making up facts."
 model = "gpt-3.5-turbo"
 
 
 # Agent which:
@@ -15,15 +16,15 @@
 class TerminalLlamaAgent:
     def __init__(self, openai_client):
 
         self.openai_client = openai_client
 
 
     def get_system_prompt(self):
-        user_os = "System: Mac , macOS: Monterey, osVersion: 12.4"
+        user_os = config.get_user_operating_system()
         system_prompt = '''
 You are an expert in providing a Natural Language Interface that converts questions and/or instructions into terminal commands.        
 You are renowned for your ability to take a user's question or instruction and create a valid terminal command that works every time.
 You do not use preamble, explanation, or pleasantries.  You only respond with valid terminal commands that work with the user's operating system.
 If there is no way to create a valid terminal command, simply say 'No shell command can facilitate your request'.
 Do not surround the terminal command with any string indicators, like `, ', or ".
 Here are some example question/command and what your response should look like:
@@ -62,15 +63,15 @@
         # get all messages in the conversation history to pass to chatgpt
         messages = conversation.get_messages_in_chatgpt_format()
         # print(f"sending messages: {messages}")
 
         # call chatgpt
         # response = self.openai_client.ChatCompletion.create(model=model, messages=messages, tools=self.tools)
         response = self.openai_client.chat.completions.create(
-            model=model,
+            model=config.get_model_name(),
             messages=messages,
             # tools=self.tools,
             stream=False, # Whether to stream the response or return the full response at once
             # max_tokens=8000,  # The maximum number of tokens to generate in the completion
             # temperature=0.5,  # The temperature of the model, controlling the randomness of the output
             # top_p=1.0,  # The nucleus sampling parameter, controlling the diversity of the output
             # n=1,  # The number of completions to generate
```

### Comparing `eras-0.3.3/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.3.4/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x81534a66 (Sun May 19 19:31:13 2024 UTC)
-files sz: 442
+moddate:  0x8cb14e66 (Thu May 23 03:01:32 2024 UTC)
+files sz: 610
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a0002004700640284006403a6020000ab02000000
@@ -15,22 +15,22 @@
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
      4          10 PUSH_NULL
                 12 LOAD_BUILD_CLASS
-                14 LOAD_CONST               2 (<code object Config, file "/Users/jason/Documents/dev/eras/src/config/config.py", line 4>)
+                14 LOAD_CONST               2 (<code object Config, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 4>)
                 16 MAKE_FUNCTION            0
                 18 LOAD_CONST               3 ('Config')
                 20 PRECALL                  2
                 24 CALL                     2
                 34 STORE_NAME               1 (Config)
    
-    22          36 PUSH_NULL
+    28          36 PUSH_NULL
                 38 LOAD_NAME                1 (Config)
                 40 PRECALL                  0
                 44 CALL                     0
                 54 STORE_NAME               2 (config)
                 56 LOAD_CONST               1 (None)
                 58 RETURN_VALUE
    consts
@@ -39,47 +39,56 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04640384
-            005a05640484005a06640584005a07880078015a085300
+            005a05640484005a06640584005a07640684005a08640784005a09880078
+            015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
            4           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Config')
                       10 STORE_NAME               2 (__qualname__)
          
            5          12 LOAD_CONST               1 (None)
                       14 STORE_NAME               3 (_instance)
          
            7          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __new__, file "/Users/jason/Documents/dev/eras/src/config/config.py", line 7>)
+                      20 LOAD_CONST               2 (<code object __new__, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 7>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__new__)
          
-          12          26 LOAD_CONST               3 (<code object get_open_ai_key, file "/Users/jason/Documents/dev/eras/src/config/config.py", line 12>)
+          12          26 LOAD_CONST               3 (<code object get_open_ai_key, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 12>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (get_open_ai_key)
          
-          15          32 LOAD_CONST               4 (<code object get_eras_open_ai_key, file "/Users/jason/Documents/dev/eras/src/config/config.py", line 15>)
+          15          32 LOAD_CONST               4 (<code object get_eras_open_ai_key, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 15>)
                       34 MAKE_FUNCTION            0
                       36 STORE_NAME               6 (get_eras_open_ai_key)
          
-          18          38 LOAD_CONST               5 (<code object get_eras_base_url, file "/Users/jason/Documents/dev/eras/src/config/config.py", line 18>)
+          18          38 LOAD_CONST               5 (<code object get_eras_base_url, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 18>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME               7 (get_eras_base_url)
-                      44 LOAD_CLOSURE             0 (__class__)
-                      46 COPY                     1
-                      48 STORE_NAME               8 (__classcell__)
-                      50 RETURN_VALUE
+         
+          21          44 LOAD_CONST               6 (<code object get_model_name, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 21>)
+                      46 MAKE_FUNCTION            0
+                      48 STORE_NAME               8 (get_model_name)
+         
+          24          50 LOAD_CONST               7 (<code object get_user_operating_system, file "/Users/jason/Documents/dev/eras/eras/config/config.py", line 24>)
+                      52 MAKE_FUNCTION            0
+                      54 STORE_NAME               9 (get_user_operating_system)
+                      56 LOAD_CLOSURE             0 (__class__)
+                      58 COPY                     1
+                      60 STORE_NAME              10 (__classcell__)
+                      62 RETURN_VALUE
          consts
             'Config'
             None
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -115,15 +124,15 @@
                            120 RETURN_VALUE
                consts
                   None
                names      ('_instance', 'super', 'Config', '__new__')
                varnames   ('cls',)
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/config/config.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
                name       '__new__'
                firstlineno 7
                lnotab 0x04010e015a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -142,15 +151,15 @@
                consts
                   None
                   'OPEN_AI_KEY'
                names      ('os', 'getenv')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/config/config.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
                name       'get_open_ai_key'
                firstlineno 12
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -169,15 +178,15 @@
                consts
                   None
                   'ERAS_OPENAI_KEY'
                names      ('os', 'getenv')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/config/config.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
                name       'get_eras_open_ai_key'
                firstlineno 15
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -196,28 +205,70 @@
                consts
                   None
                   'ERAS_BASE_URL'
                names      ('os', 'getenv')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/config/config.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
                name       'get_eras_base_url'
                firstlineno 18
                lnotab 0x0201
-         names      ('__name__', '__module__', '__qualname__', '_instance', '__new__', 'get_open_ai_key', 'get_eras_open_ai_key', 'get_eras_base_url', '__classcell__')
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x970064015300
+                21           0 RESUME                   0
+               
+                22           2 LOAD_CONST               1 ('gpt-3.5-turbo')
+                             4 RETURN_VALUE
+               consts
+                  None
+                  'gpt-3.5-turbo'
+               names      ()
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
+               name       'get_model_name'
+               firstlineno 21
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x970064015300
+                24           0 RESUME                   0
+               
+                25           2 LOAD_CONST               1 ('System: Mac , macOS: Monterey, osVersion: 12.4')
+                             4 RETURN_VALUE
+               consts
+                  None
+                  'System: Mac , macOS: Monterey, osVersion: 12.4'
+               names      ()
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
+               name       'get_user_operating_system'
+               firstlineno 24
+               lnotab 0x0201
+         names      ('__name__', '__module__', '__qualname__', '_instance', '__new__', 'get_open_ai_key', 'get_eras_open_ai_key', 'get_eras_base_url', 'get_model_name', 'get_user_operating_system', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/Users/jason/Documents/dev/eras/src/config/config.py'
+         filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
          name       'Config'
          firstlineno 4
-         lnotab 0x0c0104020a0506030603
+         lnotab 0x0c0104020a050603060306030603
       'Config'
    names      ('os', 'Config', 'config')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jason/Documents/dev/eras/src/config/config.py'
+   filename   '/Users/jason/Documents/dev/eras/eras/config/config.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108031a12
+   lnotab 0x00ff020108031a18
```

### Comparing `eras-0.3.3/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.3.4/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/config/post_install.py` & `eras-0.3.4/eras/config/post_install.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.3.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/decorators/chatgpt_tool_data.py` & `eras-0.3.4/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.3.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0xa4614a66 (Sun May 19 20:31:32 2024 UTC)
-files sz: 2675
+moddate:  0xc88a4a66 (Sun May 19 23:27:04 2024 UTC)
+files sz: 2702
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a0202004700640384
       006404a6020000ab0200000000000000005a0364025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Message',))
-                 6 IMPORT_NAME              0 (models.message)
+                 6 IMPORT_NAME              0 (eras.models.message)
                  8 IMPORT_FROM              1 (Message)
                 10 STORE_NAME               1 (Message)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (None)
                 18 IMPORT_NAME              2 (json)
                 20 STORE_NAME               2 (json)
    
      4          22 PUSH_NULL
                 24 LOAD_BUILD_CLASS
-                26 LOAD_CONST               3 (<code object MessageFactory, file "/Users/jason/Documents/dev/eras/src/factories/message_factory.py", line 4>)
+                26 LOAD_CONST               3 (<code object MessageFactory, file "/Users/jason/Documents/dev/eras/eras/factories/message_factory.py", line 4>)
                 28 MAKE_FUNCTION            0
                 30 LOAD_CONST               4 ('MessageFactory')
                 32 PRECALL                  2
                 36 CALL                     2
                 46 STORE_NAME               3 (MessageFactory)
                 48 LOAD_CONST               2 (None)
                 50 RETURN_VALUE
@@ -52,70 +52,70 @@
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MessageFactory')
                        8 STORE_NAME               2 (__qualname__)
          
            5          10 LOAD_NAME                3 (staticmethod)
          
-           6          12 LOAD_CONST               1 (<code object create_message_from_chatgpt_response, file "/Users/jason/Documents/dev/eras/src/factories/message_factory.py", line 5>)
+           6          12 LOAD_CONST               1 (<code object create_message_from_chatgpt_response, file "/Users/jason/Documents/dev/eras/eras/factories/message_factory.py", line 5>)
                       14 MAKE_FUNCTION            0
          
            5          16 PRECALL                  0
                       20 CALL                     0
          
            6          30 STORE_NAME               4 (create_message_from_chatgpt_response)
          
           22          32 LOAD_NAME                3 (staticmethod)
          
-          23          34 LOAD_CONST               2 (<code object create_message_from_llama_response, file "/Users/jason/Documents/dev/eras/src/factories/message_factory.py", line 22>)
+          23          34 LOAD_CONST               2 (<code object create_message_from_llama_response, file "/Users/jason/Documents/dev/eras/eras/factories/message_factory.py", line 22>)
                       36 MAKE_FUNCTION            0
          
           22          38 PRECALL                  0
                       42 CALL                     0
          
           23          52 STORE_NAME               5 (create_message_from_llama_response)
          
           39          54 LOAD_NAME                3 (staticmethod)
          
           40          56 LOAD_CONST               3 ('json_string')
                       58 LOAD_NAME                6 (str)
                       60 BUILD_TUPLE              2
-                      62 LOAD_CONST               4 (<code object parse_potential_tool_calls_from_llama, file "/Users/jason/Documents/dev/eras/src/factories/message_factory.py", line 39>)
+                      62 LOAD_CONST               4 (<code object parse_potential_tool_calls_from_llama, file "/Users/jason/Documents/dev/eras/eras/factories/message_factory.py", line 39>)
                       64 MAKE_FUNCTION            4 (annotations)
          
           39          66 PRECALL                  0
                       70 CALL                     0
          
           40          80 STORE_NAME               7 (parse_potential_tool_calls_from_llama)
          
-          57          82 LOAD_NAME                3 (staticmethod)
+          58          82 LOAD_NAME                3 (staticmethod)
          
-          58          84 LOAD_CONST               5 ('question')
+          59          84 LOAD_CONST               5 ('question')
                       86 LOAD_NAME                6 (str)
                       88 BUILD_TUPLE              2
-                      90 LOAD_CONST               6 (<code object create_message_from_user_question, file "/Users/jason/Documents/dev/eras/src/factories/message_factory.py", line 57>)
+                      90 LOAD_CONST               6 (<code object create_message_from_user_question, file "/Users/jason/Documents/dev/eras/eras/factories/message_factory.py", line 58>)
                       92 MAKE_FUNCTION            4 (annotations)
          
-          57          94 PRECALL                  0
+          58          94 PRECALL                  0
                       98 CALL                     0
          
-          58         108 STORE_NAME               8 (create_message_from_user_question)
+          59         108 STORE_NAME               8 (create_message_from_user_question)
          
-          61         110 LOAD_NAME                3 (staticmethod)
+          62         110 LOAD_NAME                3 (staticmethod)
          
-          62         112 LOAD_CONST               7 ('system_prompt')
+          63         112 LOAD_CONST               7 ('system_prompt')
                      114 LOAD_NAME                6 (str)
                      116 BUILD_TUPLE              2
-                     118 LOAD_CONST               8 (<code object create_system_prompt_message, file "/Users/jason/Documents/dev/eras/src/factories/message_factory.py", line 61>)
+                     118 LOAD_CONST               8 (<code object create_system_prompt_message, file "/Users/jason/Documents/dev/eras/eras/factories/message_factory.py", line 62>)
                      120 MAKE_FUNCTION            4 (annotations)
          
-          61         122 PRECALL                  0
+          62         122 PRECALL                  0
                      126 CALL                     0
          
-          62         136 STORE_NAME               9 (create_system_prompt_message)
+          63         136 STORE_NAME               9 (create_system_prompt_message)
                      138 LOAD_CONST               9 (None)
                      140 RETURN_VALUE
          consts
             'MessageFactory'
             code
                argcount  : 1
                nlocals   : 9
@@ -176,15 +176,15 @@
                   None
                   0
                   ('message_text', 'role', 'raw_chatgpt_chat_completion_response', 'tool_calls')
                names      ('choices', 'message', 'role', 'content', 'tool_calls', 'finish_reason', 'Message')
                varnames   ('response', 'choices', 'choice', 'gpt_message', 'role', 'message_text', 'tool_calls', 'finish_reason', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
                name       'create_message_from_chatgpt_response'
                firstlineno 5
                lnotab 0x02020e0110010e010e010e010e010e05120102ff1202
             code
                argcount  : 1
                nlocals   : 9
                stacksize : 6
@@ -249,37 +249,35 @@
                   None
                   0
                   ('message_text', 'role', 'raw_chatgpt_chat_completion_response', 'tool_calls')
                names      ('choices', 'message', 'role', 'content', 'MessageFactory', 'parse_potential_tool_calls_from_llama', 'finish_reason', 'Message')
                varnames   ('response', 'choices', 'choice', 'gpt_message', 'role', 'message_text', 'tool_calls', 'finish_reason', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
                name       'create_message_from_llama_response'
                firstlineno 22
                lnotab 0x02020e0110010e010e010e0134010e05120102ff1202
             'json_string'
             code
                argcount  : 1
-               nlocals   : 7
-               stacksize : 5
+               nlocals   : 8
+               stacksize : 4
                flags     : 3
                code
                   0x970009007401000000000000000000006a0100000000000000007c00a6
                   010000ab0100000000000000007d017c01a0020000000000000000000000
                   00000000000000000064016700a6020000ab0200000000000000007d027c
                   0272387c026402190000000000000000007d037c03a00200000000000000
                   0000000000000000000000000064036900a6020000ab0200000000000000
                   007d047c04a0020000000000000000000000000000000000000000640464
                   00a6020000ab0200000000000000007d057c0572047c0553006400530064
                   00530023007400000000000000000000006a030000000000000000240072
-                  2a7d0674090000000000000000000064057c06a6020000ab020000000000
-                  00000001007409000000000000000000007c00a6010000ab010000000000
-                  0000000100590064007d067e066400530064007d067e0677017700780359
-                  007701
+                  0d7d0664057d07590064007d067e066400530064007d067e067701770078
+                  0359007701
                 39           0 RESUME                   0
                
                 41           2 NOP
                
                 42           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (json_string)
@@ -331,139 +329,127 @@
                 50     >>  208 LOAD_CONST               0 (None)
                            210 RETURN_VALUE
                        >>  212 PUSH_EXC_INFO
                
                 53         214 LOAD_GLOBAL              0 (json)
                            226 LOAD_ATTR                3 (JSONDecodeError)
                            236 CHECK_EXC_MATCH
-                           238 POP_JUMP_FORWARD_IF_FALSE    42 (to 324)
+                           238 POP_JUMP_FORWARD_IF_FALSE    13 (to 266)
                            240 STORE_FAST               6 (e)
                
-                54         242 LOAD_GLOBAL              9 (NULL + print)
-                           254 LOAD_CONST               5 ('Invalid JSON:')
-                           256 LOAD_FAST                6 (e)
-                           258 PRECALL                  2
-                           262 CALL                     2
-                           272 POP_TOP
-               
-                55         274 LOAD_GLOBAL              9 (NULL + print)
-                           286 LOAD_FAST                0 (json_string)
-                           288 PRECALL                  1
-                           292 CALL                     1
-                           302 POP_TOP
-                           304 POP_EXCEPT
-                           306 LOAD_CONST               0 (None)
-                           308 STORE_FAST               6 (e)
-                           310 DELETE_FAST              6 (e)
-                           312 LOAD_CONST               0 (None)
-                           314 RETURN_VALUE
-                       >>  316 LOAD_CONST               0 (None)
-                           318 STORE_FAST               6 (e)
-                           320 DELETE_FAST              6 (e)
-                           322 RERAISE                  1
-               
-                53     >>  324 RERAISE                  0
-                       >>  326 COPY                     3
-                           328 POP_EXCEPT
-                           330 RERAISE                  1
+                54         242 LOAD_CONST               5 (1)
+                           244 STORE_FAST               7 (x)
+                           246 POP_EXCEPT
+                           248 LOAD_CONST               0 (None)
+                           250 STORE_FAST               6 (e)
+                           252 DELETE_FAST              6 (e)
+                           254 LOAD_CONST               0 (None)
+                           256 RETURN_VALUE
+                       >>  258 LOAD_CONST               0 (None)
+                           260 STORE_FAST               6 (e)
+                           262 DELETE_FAST              6 (e)
+                           264 RERAISE                  1
+               
+                53     >>  266 RERAISE                  0
+                       >>  268 COPY                     3
+                           270 POP_EXCEPT
+                           272 RERAISE                  1
                ExceptionTable:
                  4 to 200 -> 212 [0]
-                 212 to 240 -> 326 [1] lasti
-                 242 to 302 -> 316 [1] lasti
-                 316 to 324 -> 326 [1] lasti
+                 212 to 240 -> 268 [1] lasti
+                 242 to 244 -> 258 [1] lasti
+                 258 to 266 -> 268 [1] lasti
                consts
                   None
                   'choices'
                   0
                   'message'
                   'tool_calls'
-                  'Invalid JSON:'
-               names      ('json', 'loads', 'get', 'JSONDecodeError', 'print')
-               varnames   ('json_string', 'json_obj', 'choices', 'first_choice', 'message', 'tool_calls', 'e')
+                  1
+               names      ('json', 'loads', 'get', 'JSONDecodeError')
+               varnames   ('json_string', 'json_obj', 'choices', 'first_choice', 'message', 'tool_calls', 'e', 'x')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
                name       'parse_potential_tool_calls_from_llama'
                firstlineno 39
-               lnotab
-                  0x0202020128032c01040110012c012c01040104fb040406031c01200132
-                  fe
+               lnotab 0x0202020128032c01040110012c012c01040104fb040406031c0118ff
             'question'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c00ac02a6020000ab02000000
                   00000000005300
-                57           0 RESUME                   0
+                58           0 RESUME                   0
                
-                59           2 LOAD_GLOBAL              1 (NULL + Message)
+                60           2 LOAD_GLOBAL              1 (NULL + Message)
                             14 LOAD_CONST               1 ('user')
                             16 LOAD_FAST                0 (question)
                             18 KW_NAMES                 2
                             20 PRECALL                  2
                             24 CALL                     2
                             34 RETURN_VALUE
                consts
                   None
                   'user'
                   ('role', 'message_text')
                names      ('Message',)
                varnames   ('question',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
                name       'create_message_from_user_question'
-               firstlineno 57
+               firstlineno 58
                lnotab 0x0202
             'system_prompt'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c00ac02a6020000ab02000000
                   00000000005300
-                61           0 RESUME                   0
+                62           0 RESUME                   0
                
-                63           2 LOAD_GLOBAL              1 (NULL + Message)
+                64           2 LOAD_GLOBAL              1 (NULL + Message)
                             14 LOAD_CONST               1 ('system')
                             16 LOAD_FAST                0 (system_prompt)
                             18 KW_NAMES                 2
                             20 PRECALL                  2
                             24 CALL                     2
                             34 RETURN_VALUE
                consts
                   None
                   'system'
                   ('role', 'message_text')
                names      ('Message',)
                varnames   ('system_prompt',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
                name       'create_system_prompt_message'
-               firstlineno 61
+               firstlineno 62
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'create_message_from_chatgpt_response', 'create_message_from_llama_response', 'str', 'parse_potential_tool_calls_from_llama', 'create_message_from_user_question', 'create_system_prompt_message')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+         filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
          name       'MessageFactory'
          firstlineno 4
          lnotab
-            0x0a01020104ff0e010210020104ff0e01021002010aff0e01021102010a
+            0x0a01020104ff0e010210020104ff0e01021002010aff0e01021202010a
             ff0e01020302010aff0e01
       'MessageFactory'
-   names      ('models.message', 'Message', 'json', 'MessageFactory')
+   names      ('eras.models.message', 'Message', 'json', 'MessageFactory')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jason/Documents/dev/eras/src/factories/message_factory.py'
+   filename   '/Users/jason/Documents/dev/eras/eras/factories/message_factory.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010802
```

### Comparing `eras-0.3.3/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.3.4/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/factories/function_details_factory.py` & `eras-0.3.4/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/factories/message_factory.py` & `eras-0.3.4/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/main.py` & `eras-0.3.4/eras/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import argparse
 import sys
 import os
+from dotenv import load_dotenv
+load_dotenv()
 
-from eras.services.shell_command_service import ShellCommandService
+from eras.services.user_command_service import UserCommandService
 from eras.config.post_install import ensure
-
+# from eras.services.user_command_service import UserCommandService
 def main():
     # print("main")
     ensure()
     parser = argparse.ArgumentParser(description="AI Natural Language Interface for running shell commands")
     parser.add_argument('question', nargs='+', help='question or instruction to turn into a shell command')
     args = parser.parse_args()
-    question = ' '.join(args.question)
-
-    # print(f'received question: {question}')
-    shell_command_service = ShellCommandService()
-    shell_command_service.handle_prompt(question)
+    user_input = ' '.join(args.question)
+    user_command_service = UserCommandService()
+    user_command_service.handle_request(user_input)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `eras-0.3.3/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.3.4/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x94614a66 (Sun May 19 20:31:16 2024 UTC)
-files sz: 2520
+moddate:  0xac6b4a66 (Sun May 19 21:14:20 2024 UTC)
+files sz: 2535
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a040100640064
@@ -24,36 +24,36 @@
                 18 STORE_NAME               3 (Set)
                 20 IMPORT_FROM              4 (Dict)
                 22 STORE_NAME               4 (Dict)
                 24 POP_TOP
    
      3          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               2 (('MessageFactory',))
-                30 IMPORT_NAME              5 (factories.message_factory)
+                30 IMPORT_NAME              5 (eras.factories.message_factory)
                 32 IMPORT_FROM              6 (MessageFactory)
                 34 STORE_NAME               6 (MessageFactory)
                 36 POP_TOP
    
      4          38 LOAD_CONST               0 (0)
                 40 LOAD_CONST               3 (('FunctionDetails',))
-                42 IMPORT_NAME              7 (models.function_details)
+                42 IMPORT_NAME              7 (eras.models.function_details)
                 44 IMPORT_FROM              8 (FunctionDetails)
                 46 STORE_NAME               8 (FunctionDetails)
                 48 POP_TOP
    
      5          50 LOAD_CONST               0 (0)
                 52 LOAD_CONST               4 (('Message',))
-                54 IMPORT_NAME              9 (models.message)
+                54 IMPORT_NAME              9 (eras.models.message)
                 56 IMPORT_FROM             10 (Message)
                 58 STORE_NAME              10 (Message)
                 60 POP_TOP
    
      8          62 PUSH_NULL
                 64 LOAD_BUILD_CLASS
-                66 LOAD_CONST               5 (<code object Conversation, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 8>)
+                66 LOAD_CONST               5 (<code object Conversation, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 8>)
                 68 MAKE_FUNCTION            0
                 70 LOAD_CONST               6 ('Conversation')
                 72 PRECALL                  2
                 76 CALL                     2
                 86 STORE_NAME              11 (Conversation)
                 88 LOAD_CONST               7 (None)
                 90 RETURN_VALUE
@@ -86,58 +86,58 @@
                       16 LOAD_CONST               3 ('system_prompt')
                       18 LOAD_NAME                3 (str)
                       20 LOAD_CONST               4 ('messages')
                       22 LOAD_NAME                4 (List)
                       24 LOAD_NAME                5 (Message)
                       26 BINARY_SUBSCR
                       36 BUILD_TUPLE              6
-                      38 LOAD_CONST               5 (<code object __init__, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 9>)
+                      38 LOAD_CONST               5 (<code object __init__, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 9>)
                       40 MAKE_FUNCTION            5 (defaults, annotations)
                       42 STORE_NAME               6 (__init__)
          
-          17          44 LOAD_CONST               6 (<code object ensure_system_prompt_message_exists, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 17>)
+          17          44 LOAD_CONST               6 (<code object ensure_system_prompt_message_exists, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 17>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               7 (ensure_system_prompt_message_exists)
          
           22          50 LOAD_CONST               7 ('message')
                       52 LOAD_NAME                5 (Message)
                       54 BUILD_TUPLE              2
-                      56 LOAD_CONST               8 (<code object add_message, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 22>)
+                      56 LOAD_CONST               8 (<code object add_message, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 22>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (add_message)
          
-          25          62 LOAD_CONST               9 (<code object get_messages_in_chatgpt_format, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 25>)
+          25          62 LOAD_CONST               9 (<code object get_messages_in_chatgpt_format, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 25>)
                       64 MAKE_FUNCTION            0
                       66 STORE_NAME               9 (get_messages_in_chatgpt_format)
          
-          34          68 LOAD_CONST              10 (<code object get_last_message, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 34>)
+          34          68 LOAD_CONST              10 (<code object get_last_message, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 34>)
                       70 MAKE_FUNCTION            0
                       72 STORE_NAME              10 (get_last_message)
          
           40          74 LOAD_CONST              11 ('question')
                       76 LOAD_NAME                3 (str)
                       78 BUILD_TUPLE              2
-                      80 LOAD_CONST              12 (<code object add_user_question_to_messages_if_applicable, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 40>)
+                      80 LOAD_CONST              12 (<code object add_user_question_to_messages_if_applicable, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 40>)
                       82 MAKE_FUNCTION            4 (annotations)
                       84 STORE_NAME              11 (add_user_question_to_messages_if_applicable)
          
           47          86 LOAD_CONST              13 ('functions_details')
                       88 LOAD_NAME                4 (List)
                       90 LOAD_NAME               12 (FunctionDetails)
                       92 BINARY_SUBSCR
                      102 BUILD_TUPLE              2
-                     104 LOAD_CONST              14 (<code object add_functions_details_as_messages_in_conversation, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 47>)
+                     104 LOAD_CONST              14 (<code object add_functions_details_as_messages_in_conversation, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 47>)
                      106 MAKE_FUNCTION            4 (annotations)
                      108 STORE_NAME              13 (add_functions_details_as_messages_in_conversation)
          
-          55         110 LOAD_CONST              15 (<code object add_chatgpt_response_to_messages, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 55>)
+          55         110 LOAD_CONST              15 (<code object add_chatgpt_response_to_messages, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 55>)
                      112 MAKE_FUNCTION            0
                      114 STORE_NAME              14 (add_chatgpt_response_to_messages)
          
-          59         116 LOAD_CONST              16 (<code object add_llama_response_to_messages, file "/Users/jason/Documents/dev/eras/src/models/conversation.py", line 59>)
+          59         116 LOAD_CONST              16 (<code object add_llama_response_to_messages, file "/Users/jason/Documents/dev/eras/eras/models/conversation.py", line 59>)
                      118 MAKE_FUNCTION            0
                      120 STORE_NAME              15 (add_llama_response_to_messages)
                      122 LOAD_CONST               1 (None)
                      124 RETURN_VALUE
          consts
             'Conversation'
             None
@@ -183,15 +183,15 @@
                             94 RETURN_VALUE
                consts
                   None
                names      ('conversation_id', 'messages', 'system_prompt', 'ensure_system_prompt_message_exists')
                varnames   ('self', 'conversation_id', 'system_prompt', 'messages')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       '__init__'
                firstlineno 9
                lnotab 0x0201040104010e010e010e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
@@ -238,15 +238,15 @@
                   None
                   0
                   ('system_prompt',)
                names      ('len', 'messages', 'MessageFactory', 'create_system_prompt_message', 'system_prompt', 'add_message')
                varnames   ('self', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'ensure_system_prompt_message_exists'
                firstlineno 17
                lnotab 0x0201300134012efe
             'message'
             code
                argcount  : 2
                nlocals   : 2
@@ -268,15 +268,15 @@
                             56 RETURN_VALUE
                consts
                   None
                names      ('messages', 'append')
                varnames   ('self', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'add_message'
                firstlineno 22
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
@@ -315,15 +315,15 @@
                            110 RETURN_VALUE
                consts
                   None
                names      ('messages', 'to_chatgpt_format', 'append')
                varnames   ('self', 'result', 'message', 'chatgpt_message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'get_messages_in_chatgpt_format'
                firstlineno 25
                lnotab 0x02020401120128012c02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
@@ -358,15 +358,15 @@
                   None
                   0
                   -1
                names      ('len', 'messages')
                varnames   ('self', 'last_message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'get_last_message'
                firstlineno 34
                lnotab 0x0201300104011a01
             'question'
             code
                argcount  : 2
                nlocals   : 3
@@ -402,15 +402,15 @@
                             94 RETURN_VALUE
                consts
                   None
                names      ('MessageFactory', 'create_message_from_user_question', 'add_message')
                varnames   ('self', 'question', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'add_user_question_to_messages_if_applicable'
                firstlineno 40
                lnotab 0x0201040104012801
             'functions_details'
             code
                argcount  : 2
                nlocals   : 4
@@ -452,15 +452,15 @@
                            104 RETURN_VALUE
                consts
                   None
                names      ('to_message', 'add_message')
                varnames   ('self', 'functions_details', 'function_details', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'add_functions_details_as_messages_in_conversation'
                firstlineno 47
                lnotab 0x020104010401080128012cfe
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
@@ -488,15 +488,15 @@
                             86 RETURN_VALUE
                consts
                   None
                names      ('MessageFactory', 'create_message_from_chatgpt_response', 'add_message')
                varnames   ('self', 'raw_chatgpt_chat_completion_response', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'add_chatgpt_response_to_messages'
                firstlineno 55
                lnotab 0x02012801
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
@@ -524,30 +524,30 @@
                             86 RETURN_VALUE
                consts
                   None
                names      ('MessageFactory', 'create_message_from_llama_response', 'add_message')
                varnames   ('self', 'raw_llama_chat_completion_response', 'message')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
                name       'add_llama_response_to_messages'
                firstlineno 59
                lnotab 0x02012801
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'str', 'List', 'Message', '__init__', 'ensure_system_prompt_message_exists', 'add_message', 'get_messages_in_chatgpt_format', 'get_last_message', 'add_user_question_to_messages_if_applicable', 'FunctionDetails', 'add_functions_details_as_messages_in_conversation', 'add_chatgpt_response_to_messages', 'add_llama_response_to_messages')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+         filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
          name       'Conversation'
          firstlineno 8
          lnotab 0x0a01220806050c03060906060c0718080604
       'Conversation'
       None
-   names      ('typing', 'List', 'Tuple', 'Set', 'Dict', 'factories.message_factory', 'MessageFactory', 'models.function_details', 'FunctionDetails', 'models.message', 'Message', 'Conversation')
+   names      ('typing', 'List', 'Tuple', 'Set', 'Dict', 'eras.factories.message_factory', 'MessageFactory', 'eras.models.function_details', 'FunctionDetails', 'eras.models.message', 'Message', 'Conversation')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jason/Documents/dev/eras/src/models/conversation.py'
+   filename   '/Users/jason/Documents/dev/eras/eras/models/conversation.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020118020c010c010c03
```

### Comparing `eras-0.3.3/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.3.4/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.3.4/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0xf4614a66 (Sun May 19 20:32:52 2024 UTC)
-files sz: 727
+moddate:  0xfa6b4a66 (Sun May 19 21:15:38 2024 UTC)
+files sz: 732
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a01010002004700640284006403a6020000ab
       0200000000000000005a0264045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Message',))
-                 6 IMPORT_NAME              0 (models.message)
+                 6 IMPORT_NAME              0 (eras.models.message)
                  8 IMPORT_FROM              1 (Message)
                 10 STORE_NAME               1 (Message)
                 12 POP_TOP
    
      3          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
                 18 LOAD_CONST               2 (<code object FunctionDetails, file "/Users/jason/Documents/dev/eras/eras/models/function_details.py", line 3>)
@@ -191,15 +191,15 @@
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/models/function_details.py'
          name       'FunctionDetails'
          firstlineno 3
          lnotab 0x0a011a060603
       'FunctionDetails'
       None
-   names      ('models.message', 'Message', 'FunctionDetails')
+   names      ('eras.models.message', 'Message', 'FunctionDetails')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/models/function_details.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c02
```

### Comparing `eras-0.3.3/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.3.4/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.3.4/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.3.4/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/conversation.py` & `eras-0.3.4/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/function_details.py` & `eras-0.3.4/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/message.py` & `eras-0.3.4/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/models/transaction.py` & `eras-0.3.4/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/run.ipynb` & `eras-0.3.4/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,260 +1,222 @@
 magic:    0xa70d0d0a
-moddate:  0x63614a66 (Sun May 19 20:30:27 2024 UTC)
-files sz: 2018
+moddate:  0xa6af4e66 (Thu May 23 02:53:26 2024 UTC)
+files sz: 1689
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a02010002006502a60000
-      00ab0000000000000000000100640064036c036d045a040100640064046c
-      056d065a060100640064016c075a07640064016c085a0802004700640584
-      006406a6020000ab0200000000000000005a0964015300
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a040100640064016c055a05640064016c065a06020047006404840064
+      05a6020000ab0200000000000000005a0764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (keyboard)
                  8 STORE_NAME               0 (keyboard)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('load_dotenv',))
-                14 IMPORT_NAME              1 (dotenv)
-                16 IMPORT_FROM              2 (load_dotenv)
-                18 STORE_NAME               2 (load_dotenv)
+                12 LOAD_CONST               2 (('TerminalLlamaAgent',))
+                14 IMPORT_NAME              1 (eras.agents.terminal_llama_agent)
+                16 IMPORT_FROM              2 (TerminalLlamaAgent)
+                18 STORE_NAME               2 (TerminalLlamaAgent)
                 20 POP_TOP
    
-     3          22 PUSH_NULL
-                24 LOAD_NAME                2 (load_dotenv)
-                26 PRECALL                  0
-                30 CALL                     0
-                40 POP_TOP
+     3          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('config',))
+                26 IMPORT_NAME              3 (eras.config.config)
+                28 IMPORT_FROM              4 (config)
+                30 STORE_NAME               4 (config)
+                32 POP_TOP
    
-     4          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('TerminalLlamaAgent',))
-                46 IMPORT_NAME              3 (agents.terminal_llama_agent)
-                48 IMPORT_FROM              4 (TerminalLlamaAgent)
-                50 STORE_NAME               4 (TerminalLlamaAgent)
-                52 POP_TOP
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               1 (None)
+                38 IMPORT_NAME              5 (subprocess)
+                40 STORE_NAME               5 (subprocess)
    
-     5          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               4 (('config',))
-                58 IMPORT_NAME              5 (config.config)
-                60 IMPORT_FROM              6 (config)
-                62 STORE_NAME               6 (config)
-                64 POP_TOP
+     5          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               1 (None)
+                46 IMPORT_NAME              6 (os)
+                48 STORE_NAME               6 (os)
    
-     6          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               1 (None)
-                70 IMPORT_NAME              7 (subprocess)
-                72 STORE_NAME               7 (subprocess)
-   
-     7          74 LOAD_CONST               0 (0)
+     8          50 PUSH_NULL
+                52 LOAD_BUILD_CLASS
+                54 LOAD_CONST               4 (<code object ShellCommandService, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 8>)
+                56 MAKE_FUNCTION            0
+                58 LOAD_CONST               5 ('ShellCommandService')
+                60 PRECALL                  2
+                64 CALL                     2
+                74 STORE_NAME               7 (ShellCommandService)
                 76 LOAD_CONST               1 (None)
-                78 IMPORT_NAME              8 (os)
-                80 STORE_NAME               8 (os)
-   
-    10          82 PUSH_NULL
-                84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               5 (<code object ShellCommandService, file "/Users/jason/Documents/dev/eras/src/services/shell_command_service.py", line 10>)
-                88 MAKE_FUNCTION            0
-                90 LOAD_CONST               6 ('ShellCommandService')
-                92 PRECALL                  2
-                96 CALL                     2
-               106 STORE_NAME               9 (ShellCommandService)
-               108 LOAD_CONST               1 (None)
-               110 RETURN_VALUE
+                78 RETURN_VALUE
    consts
       0
       None
-      ('load_dotenv',)
       ('TerminalLlamaAgent',)
       ('config',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640265046602640384045a0564
             0484005a06640565046602640684045a0764075300
-          10           0 RESUME                   0
+           8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ShellCommandService')
                        8 STORE_NAME               2 (__qualname__)
          
-          11          10 LOAD_CONST               1 (<code object __init__, file "/Users/jason/Documents/dev/eras/src/services/shell_command_service.py", line 11>)
+           9          10 LOAD_CONST               1 (<code object __init__, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 9>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          29          16 LOAD_CONST               2 ('prompt')
+          14          16 LOAD_CONST               2 ('prompt')
                       18 LOAD_NAME                4 (str)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object handle_prompt, file "/Users/jason/Documents/dev/eras/src/services/shell_command_service.py", line 29>)
+                      22 LOAD_CONST               3 (<code object handle_prompt, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 14>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (handle_prompt)
          
-          35          28 LOAD_CONST               4 (<code object populate_terminal_with_shell_command, file "/Users/jason/Documents/dev/eras/src/services/shell_command_service.py", line 35>)
+          23          28 LOAD_CONST               4 (<code object populate_terminal_with_shell_command, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 23>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (populate_terminal_with_shell_command)
          
-          38          34 LOAD_CONST               5 ('command')
+          26          34 LOAD_CONST               5 ('command')
                       36 LOAD_NAME                4 (str)
                       38 BUILD_TUPLE              2
-                      40 LOAD_CONST               6 (<code object run_shell_command, file "/Users/jason/Documents/dev/eras/src/services/shell_command_service.py", line 38>)
+                      40 LOAD_CONST               6 (<code object run_shell_command, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 26>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (run_shell_command)
                       46 LOAD_CONST               7 (None)
                       48 RETURN_VALUE
          consts
             'ShellCommandService'
             code
-               argcount  : 1
+               argcount  : 2
                nlocals   : 2
-               stacksize : 4
+               stacksize : 3
                flags     : 3
                code
-                  0x97007401000000000000000000006401a6010000ab0100000000000000
-                  000100640264006c017d017c01a002000000000000000000000000000000
-                  00000000007407000000000000000000006a040000000000000000a60000
-                  00ab000000000000000000ac03a6010000ab0100000000000000007c005f
-                  050000000000000000740d000000000000000000007c006a050000000000
-                  000000ac04a6010000ab0100000000000000007c005f0700000000000000
-                  0064005300
-                11           0 RESUME                   0
-               
-                12           2 LOAD_GLOBAL              1 (NULL + print)
-                            14 LOAD_CONST               1 ('hi')
-                            16 PRECALL                  1
-                            20 CALL                     1
-                            30 POP_TOP
-               
-                13          32 LOAD_CONST               2 (0)
-                            34 LOAD_CONST               0 (None)
-                            36 IMPORT_NAME              1 (openai)
-                            38 STORE_FAST               1 (openai)
-               
-                21          40 LOAD_FAST                1 (openai)
-                            42 LOAD_METHOD              2 (OpenAI)
-               
-                23          64 LOAD_GLOBAL              7 (NULL + config)
-                            76 LOAD_ATTR                4 (get_eras_open_ai_key)
-                            86 PRECALL                  0
-                            90 CALL                     0
-               
-                21         100 KW_NAMES                 3
-                           102 PRECALL                  1
-                           106 CALL                     1
-                           116 LOAD_FAST                0 (self)
-                           118 STORE_ATTR               5 (openai_client)
-               
-                27         128 LOAD_GLOBAL             13 (NULL + TerminalLlamaAgent)
-                           140 LOAD_FAST                0 (self)
-                           142 LOAD_ATTR                5 (openai_client)
-                           152 KW_NAMES                 4
-                           154 PRECALL                  1
-                           158 CALL                     1
-                           168 LOAD_FAST                0 (self)
-                           170 STORE_ATTR               7 (llm_functions_agent)
-                           180 LOAD_CONST               0 (None)
-                           182 RETURN_VALUE
+                  0x97007c017c005f0000000000000000007403000000000000000000007c
+                  006a000000000000000000ac01a6010000ab0100000000000000007c005f
+                  02000000000000000064005300
+                 9           0 RESUME                   0
+               
+                11           2 LOAD_FAST                1 (openai_client)
+                             4 LOAD_FAST                0 (self)
+                             6 STORE_ATTR               0 (openai_client)
+               
+                12          16 LOAD_GLOBAL              3 (NULL + TerminalLlamaAgent)
+                            28 LOAD_FAST                0 (self)
+                            30 LOAD_ATTR                0 (openai_client)
+                            40 KW_NAMES                 1
+                            42 PRECALL                  1
+                            46 CALL                     1
+                            56 LOAD_FAST                0 (self)
+                            58 STORE_ATTR               2 (llm_functions_agent)
+                            68 LOAD_CONST               0 (None)
+                            70 RETURN_VALUE
                consts
                   None
-                  'hi'
-                  0
-                  ('api_key',)
                   ('openai_client',)
-               names      ('print', 'openai', 'OpenAI', 'config', 'get_eras_open_ai_key', 'openai_client', 'TerminalLlamaAgent', 'llm_functions_agent')
-               varnames   ('self', 'openai')
+               names      ('openai_client', 'TerminalLlamaAgent', 'llm_functions_agent')
+               varnames   ('self', 'openai_client')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/services/shell_command_service.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
                name       '__init__'
-               firstlineno 11
-               lnotab 0x02011e010808180224fe1c06
+               firstlineno 9
+               lnotab 0x02020e01
             'prompt'
             code
                argcount  : 2
                nlocals   : 3
-               stacksize : 4
+               stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
-                  000000000000007c01a6010000ab0100000000000000007d027405000000
-                  0000000000000064017c029b009d02a6010000ab01000000000000000001
-                  007c00a00300000000000000000000000000000000000000007c02a60100
-                  00ab010000000000000000010064005300
-                29           0 RESUME                   0
+                  000000000000007c01a6010000ab0100000000000000007d027c0264016b
+                  020000000072117405000000000000000000007c02a6010000ab01000000
+                  00000000000100640053007c00a003000000000000000000000000000000
+                  00000000007c02a6010000ab010000000000000000010064005300
+                14           0 RESUME                   0
                
-                30           2 LOAD_FAST                0 (self)
+                15           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (llm_functions_agent)
                             14 LOAD_METHOD              1 (inference)
                             36 LOAD_FAST                1 (prompt)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (response)
                
-                31          54 LOAD_GLOBAL              5 (NULL + print)
-                            66 LOAD_CONST               1 ('response is ')
-                            68 LOAD_FAST                2 (response)
-                            70 FORMAT_VALUE             0
-                            72 BUILD_STRING             2
-                            74 PRECALL                  1
-                            78 CALL                     1
-                            88 POP_TOP
-               
-                33          90 LOAD_FAST                0 (self)
-                            92 LOAD_METHOD              3 (populate_terminal_with_shell_command)
-                           114 LOAD_FAST                2 (response)
-                           116 PRECALL                  1
-                           120 CALL                     1
-                           130 POP_TOP
-                           132 LOAD_CONST               0 (None)
-                           134 RETURN_VALUE
+                16          54 LOAD_FAST                2 (response)
+                            56 LOAD_CONST               1 ('No shell command can facilitate your request')
+                            58 COMPARE_OP               2 (==)
+                            64 POP_JUMP_FORWARD_IF_FALSE    17 (to 100)
+               
+                17          66 LOAD_GLOBAL              5 (NULL + print)
+                            78 LOAD_FAST                2 (response)
+                            80 PRECALL                  1
+                            84 CALL                     1
+                            94 POP_TOP
+               
+                18          96 LOAD_CONST               0 (None)
+                            98 RETURN_VALUE
+               
+                21     >>  100 LOAD_FAST                0 (self)
+                           102 LOAD_METHOD              3 (populate_terminal_with_shell_command)
+                           124 LOAD_FAST                2 (response)
+                           126 PRECALL                  1
+                           130 CALL                     1
+                           140 POP_TOP
+                           142 LOAD_CONST               0 (None)
+                           144 RETURN_VALUE
                consts
                   None
-                  'response is '
+                  'No shell command can facilitate your request'
                names      ('llm_functions_agent', 'inference', 'print', 'populate_terminal_with_shell_command')
                varnames   ('self', 'prompt', 'response')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/services/shell_command_service.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
                name       'handle_prompt'
-               firstlineno 29
-               lnotab 0x020134012402
+               firstlineno 14
+               lnotab 0x020134010c011e010403
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c01a60100
                   00ab010000000000000000010064005300
-                35           0 RESUME                   0
+                23           0 RESUME                   0
                
-                36           2 LOAD_GLOBAL              1 (NULL + keyboard)
+                24           2 LOAD_GLOBAL              1 (NULL + keyboard)
                             14 LOAD_ATTR                1 (write)
                             24 LOAD_FAST                1 (command)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('keyboard', 'write')
                varnames   ('self', 'command')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/services/shell_command_service.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
                name       'populate_terminal_with_shell_command'
-               firstlineno 35
+               firstlineno 23
                lnotab 0x0201
             'command'
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 8
                flags     : 3
@@ -266,114 +228,114 @@
                   00000000006a05000000000000000064027c02ac03a6060000ab06000000
                   00000000007d037c036a06000000000000000044005d137d04740f000000
                   000000000000007c046404ac05a6020000ab02000000000000000001008c
                   147c03a0080000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d057c0564066b0300000000721b7c036a09000000
                   000000000044005d157d04740f000000000000000000007c046404ac05a6
                   020000ab02000000000000000001008c146400530064005300
-                38           0 RESUME                   0
+                26           0 RESUME                   0
                
-                39           2 LOAD_GLOBAL              0 (os)
+                27           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (expanduser)
                             46 LOAD_CONST               1 ('~')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               2 (home_directory)
                
-                44          64 LOAD_GLOBAL              7 (NULL + subprocess)
+                32          64 LOAD_GLOBAL              7 (NULL + subprocess)
                             76 LOAD_ATTR                4 (Popen)
                             86 LOAD_FAST                1 (command)
                             88 LOAD_CONST               2 (True)
                             90 LOAD_GLOBAL              6 (subprocess)
                            102 LOAD_ATTR                5 (PIPE)
                            112 LOAD_GLOBAL              6 (subprocess)
                            124 LOAD_ATTR                5 (PIPE)
                            134 LOAD_CONST               2 (True)
                
-                45         136 LOAD_FAST                2 (home_directory)
+                33         136 LOAD_FAST                2 (home_directory)
                
-                44         138 KW_NAMES                 3
+                32         138 KW_NAMES                 3
                            140 PRECALL                  6
                            144 CALL                     6
                            154 STORE_FAST               3 (process)
                
-                48         156 LOAD_FAST                3 (process)
+                36         156 LOAD_FAST                3 (process)
                            158 LOAD_ATTR                6 (stdout)
                            168 GET_ITER
                        >>  170 FOR_ITER                19 (to 210)
                            172 STORE_FAST               4 (line)
                
-                49         174 LOAD_GLOBAL             15 (NULL + print)
+                37         174 LOAD_GLOBAL             15 (NULL + print)
                            186 LOAD_FAST                4 (line)
                            188 LOAD_CONST               4 ('')
                            190 KW_NAMES                 5
                            192 PRECALL                  2
                            196 CALL                     2
                            206 POP_TOP
                            208 JUMP_BACKWARD           20 (to 170)
                
-                52     >>  210 LOAD_FAST                3 (process)
+                40     >>  210 LOAD_FAST                3 (process)
                            212 LOAD_METHOD              8 (wait)
                            234 PRECALL                  0
                            238 CALL                     0
                            248 STORE_FAST               5 (return_code)
                
-                55         250 LOAD_FAST                5 (return_code)
+                43         250 LOAD_FAST                5 (return_code)
                            252 LOAD_CONST               6 (0)
                            254 COMPARE_OP               3 (!=)
                            260 POP_JUMP_FORWARD_IF_FALSE    27 (to 316)
                
-                56         262 LOAD_FAST                3 (process)
+                44         262 LOAD_FAST                3 (process)
                            264 LOAD_ATTR                9 (stderr)
                            274 GET_ITER
                        >>  276 FOR_ITER                21 (to 320)
                            278 STORE_FAST               4 (line)
                
-                57         280 LOAD_GLOBAL             15 (NULL + print)
+                45         280 LOAD_GLOBAL             15 (NULL + print)
                            292 LOAD_FAST                4 (line)
                            294 LOAD_CONST               4 ('')
                            296 KW_NAMES                 5
                            298 PRECALL                  2
                            302 CALL                     2
                            312 POP_TOP
                            314 JUMP_BACKWARD           20 (to 276)
                
-                55     >>  316 LOAD_CONST               0 (None)
+                43     >>  316 LOAD_CONST               0 (None)
                            318 RETURN_VALUE
                
-                56     >>  320 LOAD_CONST               0 (None)
+                44     >>  320 LOAD_CONST               0 (None)
                            322 RETURN_VALUE
                consts
                   None
                   '~'
                   True
                   ('shell', 'stdout', 'stderr', 'text', 'cwd')
                   ''
                   ('end',)
                   0
                names      ('os', 'path', 'expanduser', 'subprocess', 'Popen', 'PIPE', 'stdout', 'print', 'wait', 'stderr')
                varnames   ('self', 'command', 'home_directory', 'process', 'line', 'return_code')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jason/Documents/dev/eras/src/services/shell_command_service.py'
+               filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
                name       'run_shell_command'
-               firstlineno 38
+               firstlineno 26
                lnotab 0x02013e05480102ff12041201240328030c01120124fe0401
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'handle_prompt', 'populate_terminal_with_shell_command', 'run_shell_command')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jason/Documents/dev/eras/src/services/shell_command_service.py'
+         filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
          name       'ShellCommandService'
-         firstlineno 10
-         lnotab 0x0a0106120c060603
+         firstlineno 8
+         lnotab 0x0a0106050c090603
       'ShellCommandService'
-   names      ('keyboard', 'dotenv', 'load_dotenv', 'agents.terminal_llama_agent', 'TerminalLlamaAgent', 'config.config', 'config', 'subprocess', 'os', 'ShellCommandService')
+   names      ('keyboard', 'eras.agents.terminal_llama_agent', 'TerminalLlamaAgent', 'eras.config.config', 'config', 'subprocess', 'os', 'ShellCommandService')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jason/Documents/dev/eras/src/services/shell_command_service.py'
+   filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c0114010c010c0108010803
+   lnotab 0x00ff020108010c010c0108010803
```

### Comparing `eras-0.3.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.3.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.3.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.3.4/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.3.4/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras/services/llm_callable_functions/user_details.py` & `eras-0.3.4/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.3/eras.egg-info/PKG-INFO` & `eras-0.3.4/eras.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.3
+Version: 0.3.4
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,26 +13,23 @@
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 
 # ERAS
-Easily Run AI Shell allows you to run shell commands using natural language.   
+Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
-
-<video src="./eras-demo.mov" controls></video>
-
 # Install
 ```
 % pip install eras
 ```
 
 If you get an error about externally-managed-environment it's because you have python installed via homebrew, and need to use pipx instead:
 
@@ -53,24 +50,38 @@
 the terminal with the shell command.
 
 ![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
-## Examples
+## Usage Examples
 ```
-% eras list files
+% eras list all files in the current directory
+
+ERAS will then populate the next terminal line with the command:
 % ls
+
+All you have to do is confirm and hit enter!
+
 ...
 % eras create a new file named jason.txt with contents "hello world"
 % echo "hello world" > jason.txt
 ...
 
 ```
+### Chat Examples
+```
+% eras /chat What is the capital of France 
+% Paris is the capital of France
+
+Note: if you want to use ? or other special terminal chars you should surround your question in quotes
+% eras /chat "What is the capital of France?"
+% Paris is the capital of France
+```
 
 # Upcoming functionality
 
 ## Llama 3 support
 Llama.cpp provides an API similar to OpenAI, so pointing eras at http://127.0.0.1:8080 works as expected.  
 
 I just need to prompt for the base_url preference and use it.
```

### Comparing `eras-0.3.3/eras.egg-info/SOURCES.txt` & `eras-0.3.4/eras.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,33 +7,38 @@
 eras/run.ipynb
 eras.egg-info/PKG-INFO
 eras.egg-info/SOURCES.txt
 eras.egg-info/dependency_links.txt
 eras.egg-info/entry_points.txt
 eras.egg-info/requires.txt
 eras.egg-info/top_level.txt
+eras/__pycache__/__init__.cpython-311.pyc
 eras/__pycache__/__init__.cpython-39.pyc
+eras/__pycache__/main.cpython-311.pyc
 eras/agents/__init__.py
 eras/agents/llama_functions_agent.py
 eras/agents/llama_terminal_command_functions_agent.py
 eras/agents/llm_functions_agent.py
+eras/agents/simple_llm.py
 eras/agents/terminal_llama_agent.py
 eras/agents/__pycache__/__init__.cpython-311.pyc
 eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
 eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
 eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
 eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+eras/agents/__pycache__/simple_llm.cpython-311.pyc
 eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
 eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
 eras/config/__init__.py
 eras/config/config.py
 eras/config/post_install.py
 eras/config/__pycache__/__init__.cpython-311.pyc
 eras/config/__pycache__/config.cpython-311.pyc
 eras/config/__pycache__/config.cpython-39.pyc
+eras/config/__pycache__/post_install.cpython-311.pyc
 eras/decorators/__init__.py
 eras/decorators/chatgpt_tool_data.py
 eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
 eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
 eras/factories/__init__.py
 eras/factories/function_details_factory.py
 eras/factories/message_factory.py
@@ -42,27 +47,31 @@
 eras/factories/__pycache__/function_details_factory.cpython-39.pyc
 eras/factories/__pycache__/message_factory.cpython-311.pyc
 eras/factories/__pycache__/message_factory.cpython-39.pyc
 eras/models/__init__.py
 eras/models/conversation.py
 eras/models/function_details.py
 eras/models/message.py
+eras/models/simple_stream_inference_callable.py
 eras/models/transaction.py
 eras/models/__pycache__/__init__.cpython-311.pyc
 eras/models/__pycache__/conversation.cpython-311.pyc
 eras/models/__pycache__/conversation.cpython-39.pyc
 eras/models/__pycache__/function_details.cpython-311.pyc
 eras/models/__pycache__/function_details.cpython-39.pyc
 eras/models/__pycache__/message.cpython-311.pyc
 eras/models/__pycache__/message.cpython-39.pyc
+eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
 eras/services/__init__.py
 eras/services/shell_command_service.py
+eras/services/user_command_service.py
 eras/services/__pycache__/__init__.cpython-311.pyc
 eras/services/__pycache__/shell_command_service.cpython-311.pyc
 eras/services/__pycache__/shell_command_service.cpython-39.pyc
+eras/services/__pycache__/user_command_service.cpython-311.pyc
 eras/services/llm_callable_functions/__init__.py
 eras/services/llm_callable_functions/callable_function_service_base.py
 eras/services/llm_callable_functions/terminal_command.py
 eras/services/llm_callable_functions/user_details.py
 eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
 eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
 eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
```

### Comparing `eras-0.3.3/setup.py` & `eras-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #         print('Calling post_install.py')
 #         post_install_script = os.path.join(os.path.dirname(__file__), 'eras', 'post_install.py')
 #         # Run the post_install.py script in a new interactive shell
 #         subprocess.run([sys.executable, post_install_script], check=True, stdin=sys.stdin, stdout=sys.stdout)
 
 setup(
     name='eras',
-    version='0.3.3',
+    version='0.3.4',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

