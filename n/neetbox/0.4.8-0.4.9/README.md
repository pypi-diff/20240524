# Comparing `tmp/neetbox-0.4.8.tar.gz` & `tmp/neetbox-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.4.8.tar", max compression
+gzip compressed data, was "neetbox-0.4.9.tar", max compression
```

## Comparing `neetbox-0.4.8.tar` & `neetbox-0.4.9.tar`

### file list

```diff
@@ -1,76 +1,81 @@
--rw-r--r--   0        0        0     1067 2024-01-13 04:32:05.839084 neetbox-0.4.8/LICENSE
--rw-r--r--   0        0        0     2566 2024-01-13 04:32:05.839084 neetbox-0.4.8/README.md
--rw-r--r--   0        0        0      490 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/__init__.py
--rw-r--r--   0        0        0     4097 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/_protocol.py
--rw-r--r--   0        0        0    12181 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/cli/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/cli/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/cli/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/cli/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/cli/flfs/nvscript.flf
--rw-r--r--   0        0        0     4643 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/cli/parse.py
--rw-r--r--   0        0        0      619 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/__init__.py
--rw-r--r--   0        0        0    12723 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/_client.py
--rw-r--r--   0        0        0      870 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/_client_web_apis.py
--rw-r--r--   0        0        0     1248 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/_shell.py
--rw-r--r--   0        0        0     6599 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/_signal_and_slot.py
--rw-r--r--   0        0        0     6126 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/apis/_action.py
--rw-r--r--   0        0        0     6590 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/apis/_image.py
--rw-r--r--   0        0        0     2919 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/apis/_progress.py
--rw-r--r--   0        0        0     1156 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/client/apis/_scalar.py
--rw-r--r--   0        0        0     1053 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1502 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/config/_global.py
--rw-r--r--   0        0        0     8889 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/config/_workspace.py
--rw-r--r--   0        0        0     1006 2024-01-13 04:32:05.899084 neetbox-0.4.8/neetbox/extension/__init__.py
--rw-r--r--   0        0        0      184 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/machine/__init__.py
--rw-r--r--   0        0        0     7154 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/machine/hardware.py
--rw-r--r--   0        0        0     2457 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/machine/platform.py
--rw-r--r--   0        0        0     5279 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/pommespeter/pyplot.py
--rw-r--r--   0        0        0     5272 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/arch/canny.py
--rw-r--r--   0        0        0     6390 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/arch/cnn.py
--rw-r--r--   0        0        0     2212 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/arch/kernels.py
--rw-r--r--   0        0        0     2486 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3673 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/nlp.py
--rw-r--r--   0        0        0     1570 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/nn/functional.py
--rw-r--r--   0        0        0     4311 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/extension/torch/profile.py
--rw-r--r--   0        0        0      359 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/index.html
--rw-r--r--   0        0        0      506 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/logo.svg
--rw-r--r--   0        0        0   545596 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/static/css/index.be5cc5ae.css
--rw-r--r--   0        0        0  1193176 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/static/js/async/704.d0535572.js
--rw-r--r--   0        0        0    72401 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/static/js/async/704.d0535572.js.LICENSE.txt
--rw-r--r--   0        0        0  6254220 2024-01-13 04:32:35.647286 neetbox-0.4.8/neetbox/frontend_dist/static/js/async/704.d0535572.js.map
--rw-r--r--   0        0        0  1425307 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/static/js/index.4a5649a5.js
--rw-r--r--   0        0        0   127964 2024-01-13 04:32:35.643286 neetbox-0.4.8/neetbox/frontend_dist/static/js/index.4a5649a5.js.LICENSE.txt
--rw-r--r--   0        0        0  5577825 2024-01-13 04:32:35.651286 neetbox-0.4.8/neetbox/frontend_dist/static/js/index.4a5649a5.js.map
--rw-r--r--   0        0        0      192 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     1725 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/logging/_formatting.py
--rw-r--r--   0        0        0     8568 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/logging/_logger.py
--rw-r--r--   0        0        0       44 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/logging/writers/__init__.py
--rw-r--r--   0        0        0     1253 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/logging/writers/_file.py
--rw-r--r--   0        0        0     1770 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/logging/writers/_stdout.py
--rw-r--r--   0        0        0     6740 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/_bridge.py
--rw-r--r--   0        0        0      686 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/_daemon_server_launch_script.py
--rw-r--r--   0        0        0      734 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/_server.py
--rw-r--r--   0        0        0      271 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/db/__init__.py
--rw-r--r--   0        0        0     6080 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/db/_condition.py
--rw-r--r--   0        0        0     1109 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/db/_manager.py
--rw-r--r--   0        0        0    21185 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/db/project.py
--rw-r--r--   0        0        0       39 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/__init__.py
--rw-r--r--   0        0        0     1951 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/_fastapi_server.py
--rw-r--r--   0        0        0     7818 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/routers/project.py
--rw-r--r--   0        0        0       38 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/__init__.py
--rw-r--r--   0        0        0     2625 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/_event_type_handlers.py
--rw-r--r--   0        0        0     6774 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/_manager.py
--rw-r--r--   0        0        0     1019 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/_websocket_server.py
--rw-r--r--   0        0        0      373 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     3558 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/_daemonable_process.py
--rw-r--r--   0        0        0     2715 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/_package.py
--rw-r--r--   0        0        0     6187 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/_registry.py
--rw-r--r--   0        0        0     9169 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/_resource.py
--rw-r--r--   0        0        0     1023 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/ansi.py
--rw-r--r--   0        0        0     4131 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2430 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/localstorage.py
--rw-r--r--   0        0        0     2157 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/massive.py
--rw-r--r--   0        0        0     1196 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/mvc.py
--rw-r--r--   0        0        0     1384 2024-01-13 04:32:05.903084 neetbox-0.4.8/neetbox/utils/x2numpy.py
--rw-r--r--   0        0        0     1722 2024-01-13 04:32:05.903084 neetbox-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 neetbox-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-17 08:53:50.060963 neetbox-0.4.9/LICENSE
+-rw-r--r--   0        0        0     2566 2024-01-17 08:53:50.060963 neetbox-0.4.9/README.md
+-rw-r--r--   0        0        0      490 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/__init__.py
+-rw-r--r--   0        0        0     4097 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/_protocol.py
+-rw-r--r--   0        0        0    12181 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/cli/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/cli/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/cli/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/cli/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/cli/flfs/nvscript.flf
+-rw-r--r--   0        0        0     5911 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/cli/parse.py
+-rw-r--r--   0        0        0      619 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/client/__init__.py
+-rw-r--r--   0        0        0    12723 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/client/_client.py
+-rw-r--r--   0        0        0      870 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/client/_client_web_apis.py
+-rw-r--r--   0        0        0     1245 2024-01-17 08:53:50.120963 neetbox-0.4.9/neetbox/client/_shell.py
+-rw-r--r--   0        0        0     6599 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/client/_signal_and_slot.py
+-rw-r--r--   0        0        0     6126 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/client/apis/_action.py
+-rw-r--r--   0        0        0     6590 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/client/apis/_image.py
+-rw-r--r--   0        0        0     2919 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/client/apis/_progress.py
+-rw-r--r--   0        0        0     1156 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/client/apis/_scalar.py
+-rw-r--r--   0        0        0     1044 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/config/__init__.py
+-rw-r--r--   0        0        0      265 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/config/abc.py
+-rw-r--r--   0        0        0     8889 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/config/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/config/project/hooks.py
+-rw-r--r--   0        0        0     1560 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/config/user/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/config/user/hooks.py
+-rw-r--r--   0        0        0      991 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/__init__.py
+-rw-r--r--   0        0        0      184 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/machine/__init__.py
+-rw-r--r--   0        0        0     7378 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/machine/hardware.py
+-rw-r--r--   0        0        0     2457 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/machine/platform.py
+-rw-r--r--   0        0        0     5279 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/pommespeter/pyplot.py
+-rw-r--r--   0        0        0     5272 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/arch/canny.py
+-rw-r--r--   0        0        0     6390 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2212 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2486 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3673 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/nlp.py
+-rw-r--r--   0        0        0     1570 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/nn/functional.py
+-rw-r--r--   0        0        0     4311 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/extension/torch/profile.py
+-rw-r--r--   0        0        0      359 2024-01-17 08:54:18.772824 neetbox-0.4.9/neetbox/frontend_dist/index.html
+-rw-r--r--   0        0        0      506 2024-01-17 08:54:18.772824 neetbox-0.4.9/neetbox/frontend_dist/logo.svg
+-rw-r--r--   0        0        0   545596 2024-01-17 08:54:18.772824 neetbox-0.4.9/neetbox/frontend_dist/static/css/index.be5cc5ae.css
+-rw-r--r--   0        0        0  1193176 2024-01-17 08:54:18.768824 neetbox-0.4.9/neetbox/frontend_dist/static/js/async/704.d0535572.js
+-rw-r--r--   0        0        0    72401 2024-01-17 08:54:18.768824 neetbox-0.4.9/neetbox/frontend_dist/static/js/async/704.d0535572.js.LICENSE.txt
+-rw-r--r--   0        0        0  6254220 2024-01-17 08:54:18.780824 neetbox-0.4.9/neetbox/frontend_dist/static/js/async/704.d0535572.js.map
+-rw-r--r--   0        0        0  1425307 2024-01-17 08:54:18.772824 neetbox-0.4.9/neetbox/frontend_dist/static/js/index.4a5649a5.js
+-rw-r--r--   0        0        0   127964 2024-01-17 08:54:18.772824 neetbox-0.4.9/neetbox/frontend_dist/static/js/index.4a5649a5.js.LICENSE.txt
+-rw-r--r--   0        0        0  5577825 2024-01-17 08:54:18.772824 neetbox-0.4.9/neetbox/frontend_dist/static/js/index.4a5649a5.js.map
+-rw-r--r--   0        0        0      192 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     1725 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/logging/_formatting.py
+-rw-r--r--   0        0        0     8568 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/logging/_logger.py
+-rw-r--r--   0        0        0       44 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/logging/writers/__init__.py
+-rw-r--r--   0        0        0     1253 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/logging/writers/_file.py
+-rw-r--r--   0        0        0     1770 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/logging/writers/_stdout.py
+-rw-r--r--   0        0        0     6734 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/_bridge.py
+-rw-r--r--   0        0        0      686 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/_daemon_server_launch_script.py
+-rw-r--r--   0        0        0      734 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/_server.py
+-rw-r--r--   0        0        0      228 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/db/__init__.py
+-rw-r--r--   0        0        0     1292 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/db/_manager.py
+-rw-r--r--   0        0        0      707 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/db/abc.py
+-rw-r--r--   0        0        0       60 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/db/project/__init__.py
+-rw-r--r--   0        0        0    21505 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/db/project/_project_db.py
+-rw-r--r--   0        0        0     5929 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/db/project/condition.py
+-rw-r--r--   0        0        0       39 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/__init__.py
+-rw-r--r--   0        0        0     1951 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/_fastapi_server.py
+-rw-r--r--   0        0        0     7851 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/routers/project.py
+-rw-r--r--   0        0        0       38 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/__init__.py
+-rw-r--r--   0        0        0     2625 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/_event_type_handlers.py
+-rw-r--r--   0        0        0     6774 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/_manager.py
+-rw-r--r--   0        0        0     1019 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/_websocket_server.py
+-rw-r--r--   0        0        0      373 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     3558 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/_daemonable_process.py
+-rw-r--r--   0        0        0     2715 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/_package.py
+-rw-r--r--   0        0        0     6187 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/_registry.py
+-rw-r--r--   0        0        0     9169 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/_resource.py
+-rw-r--r--   0        0        0     1023 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/ansi.py
+-rw-r--r--   0        0        0     4131 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2765 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/localstorage.py
+-rw-r--r--   0        0        0     2157 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/massive.py
+-rw-r--r--   0        0        0     1196 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/mvc.py
+-rw-r--r--   0        0        0     1384 2024-01-17 08:53:50.124963 neetbox-0.4.9/neetbox/utils/x2numpy.py
+-rw-r--r--   0        0        0     1722 2024-01-17 08:53:50.124963 neetbox-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 neetbox-0.4.9/PKG-INFO
```

### Comparing `neetbox-0.4.8/LICENSE` & `neetbox-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/README.md` & `neetbox-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/_protocol.py` & `neetbox-0.4.9/neetbox/_protocol.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/cli/flfs/ansiregular.flf` & `neetbox-0.4.9/neetbox/cli/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/cli/flfs/ansishadow.flf` & `neetbox-0.4.9/neetbox/cli/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/cli/flfs/isometrixc2.flf` & `neetbox-0.4.9/neetbox/cli/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/cli/flfs/nscripts.flf` & `neetbox-0.4.9/neetbox/cli/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/cli/flfs/nvscript.flf` & `neetbox-0.4.9/neetbox/cli/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/cli/parse.py` & `neetbox-0.4.9/neetbox/cli/parse.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 from typing import Optional
 
 import click
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
-import neetbox.config._global as global_config
 from neetbox._protocol import VERSION
 from neetbox.client._client_web_apis import *
-from neetbox.config._workspace import (
+from neetbox.config.project import (
     _get_module_level_config,
     _init_workspace,
     _load_workspace_config,
 )
+from neetbox.config.user import get as get_global_config
+from neetbox.config.user import set as set_global_config
 from neetbox.logging import Logger
+from neetbox.utils.localstorage import get_create_neetbox_config_directory
 from neetbox.utils.massive import check_read_toml
 
 console = Console()
 
 logger = Logger("NEETBOX CLI", skip_writers_names=["ws", "file"])
 
 
@@ -139,22 +141,54 @@
             else:
                 font = file[0]
     f = Figlet(font)
     rendered_text = f.renderText(text)
     console.print(Panel.fit(f"{rendered_text}", border_style="green"))
 
 
-@main.command()
+@main.command(name="init")
 @click.option("--name", "-n", help="set project name", metavar="name", required=False)
 def init(name: str):
     """initialize current folder as workspace and generate the config file from defaults"""
     try:
         init_succeed = _init_workspace(name=name)
         if init_succeed:
             console_banner("neetbox", font="ansishadow")
             logger.log("Welcome to NEETBOX")
     except Exception as e:
         logger.err(f"Failed to init here: {e}")
 
 
+@main.command(name="config")
+@click.option(
+    "--set",
+    "kvs",
+    type=(str, str),
+    multiple=True,
+    help="specify which config name to modify as well as target value",
+    metavar="name value",
+    required=False,
+    default=None,
+)
+@click.option("--force", "-f", is_flag=True, help="force set", default=False)
+def configs(kvs, force):
+    """list or set global config"""
+    if kvs:
+        current_configs = get_global_config()
+        for k, v in kvs:
+            if k not in current_configs and not force:
+                logger.warn(
+                    f"config key {k} not exist in current config file and will not be writen into config. if you want to write anyway, try --force."
+                )
+            else:
+                set_global_config(k, v)
+    table = Table(title="current global configs")
+    table.add_column("name", style="green", no_wrap=True)
+    table.add_column("current value")
+    for k, v in get_global_config().items():
+        table.add_row(str(k), str(v))
+    console.print(table)
+    logger.info(f"from config file folder: {get_create_neetbox_config_directory()}")
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `neetbox-0.4.8/neetbox/client/__init__.py` & `neetbox-0.4.9/neetbox/client/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/_client.py` & `neetbox-0.4.9/neetbox/client/_client.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/_client_web_apis.py` & `neetbox-0.4.9/neetbox/client/_client_web_apis.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/_shell.py` & `neetbox-0.4.9/neetbox/client/_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import os
 import subprocess
 from threading import Thread
 
-from neetbox.config._workspace import _get_module_level_config
+from neetbox.config.project import _get_module_level_config
 from neetbox.utils import DaemonableProcess
 from neetbox.utils.mvc import Singleton
 
 
 class ShellAgent(metaclass=Singleton):
     def __init__(self) -> None:
         shell_exec = "cmd.exe" if os.name == "nt" else "/bin/bash"
```

### Comparing `neetbox-0.4.8/neetbox/client/_signal_and_slot.py` & `neetbox-0.4.9/neetbox/client/_signal_and_slot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/apis/_action.py` & `neetbox-0.4.9/neetbox/client/apis/_action.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/apis/_image.py` & `neetbox-0.4.9/neetbox/client/apis/_image.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/apis/_progress.py` & `neetbox-0.4.9/neetbox/client/apis/_progress.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/client/apis/_scalar.py` & `neetbox-0.4.9/neetbox/client/apis/_scalar.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/config/__init__.py` & `neetbox-0.4.9/neetbox/config/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Date:   20230413
 
 import types
 from typing import Union
 
 from neetbox._protocol import MACHINE_ID_KEY, PROJECT_ID_KEY, RUN_ID_KEY
 
-from ._global import get as get_user_config
-from ._workspace import _get_module_level_config, export_default_config
+from .project import _get_module_level_config, export_default_config
+from .user import get as get_user_config
 
 __IS_WORKSPACE_LOADED = False
 
 
 def get_module_level_config(module: Union[str, types.ModuleType] = None):
     global __IS_WORKSPACE_LOADED
     if not __IS_WORKSPACE_LOADED:
         __IS_WORKSPACE_LOADED = True
-        from ._workspace import _create_load_workspace
+        from .project import _create_load_workspace
 
         _create_load_workspace()
 
     module_config = _get_module_level_config(module, stack_offset=3)
     return module_config
```

### Comparing `neetbox-0.4.8/neetbox/config/_global.py` & `neetbox-0.4.9/neetbox/config/user/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,47 +6,50 @@
 
 import os
 from uuid import uuid4
 
 import toml
 
 from neetbox._protocol import MACHINE_ID_KEY
-from neetbox.utils.localstorage import get_create_neetbox_data_directory
+from neetbox.utils.localstorage import (
+    get_create_neetbox_config_directory,
+    get_create_neetbox_data_directory,
+)
 from neetbox.utils.massive import check_read_toml
 
 _GLOBAL_CONFIG = {
     MACHINE_ID_KEY: str(uuid4()),
     "vault": get_create_neetbox_data_directory(),
 }
 
 _GLOBAL_CONFIG_FILE_NAME = f"neetbox.global.toml"
 
 
 def overwrite_create_local(config: dict):
-    neetbox_data_dir = get_create_neetbox_data_directory()
-    config_file_path = os.path.join(neetbox_data_dir, _GLOBAL_CONFIG_FILE_NAME)
+    neetbox_config_dir = get_create_neetbox_config_directory()
+    config_file_path = os.path.join(neetbox_config_dir, _GLOBAL_CONFIG_FILE_NAME)
     with open(config_file_path, "w+") as config_file:
         toml.dump(config, config_file)
 
 
 def read_create_local():
     global _GLOBAL_CONFIG
-    neetbox_data_dir = get_create_neetbox_data_directory()
-    config_file_path = os.path.join(neetbox_data_dir, _GLOBAL_CONFIG_FILE_NAME)
+    neetbox_config_dir = get_create_neetbox_config_directory()
+    config_file_path = os.path.join(neetbox_config_dir, _GLOBAL_CONFIG_FILE_NAME)
     if not os.path.exists(config_file_path):  # config not exist, try to create
         overwrite_create_local(_GLOBAL_CONFIG)
     # read local file
     user_cfg = check_read_toml(config_file_path)
     assert user_cfg
-    for k, v in user_cfg.items():
-        _GLOBAL_CONFIG[k] = v
+    _GLOBAL_CONFIG.update(user_cfg)
 
 
 def set(key, value):
     global _GLOBAL_CONFIG
+    read_create_local()
     _GLOBAL_CONFIG[key] = value
     overwrite_create_local(_GLOBAL_CONFIG)
 
 
 def get(key=None):
     read_create_local()
     if key is None:
```

### Comparing `neetbox-0.4.8/neetbox/config/_workspace.py` & `neetbox-0.4.9/neetbox/config/project/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/__init__.py` & `neetbox-0.4.9/neetbox/extension/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 # Author: GavinGong aka VisualDust
 # Github: github.com/visualDust
 # Date:   20230417
 
 import importlib
 import pkgutil
 
-from neetbox.config._workspace import (
-    _get_module_level_config as get_module_level_config,
-)
-from neetbox.config._workspace import on_config_loaded
+from neetbox.config.project import _get_module_level_config as get_module_level_config
+from neetbox.config.project import on_config_loaded
 from neetbox.utils import Registry
 from neetbox.utils.framing import get_frame_module_traceback
 
 __QUERY_AFTER_LOAD_WORKSPACE = Registry("__QUERY_AFTER_LOAD_WORKSPACE")
 on_workspace_loaded = __QUERY_AFTER_LOAD_WORKSPACE.register
```

### Comparing `neetbox-0.4.8/neetbox/extension/machine/hardware.py` & `neetbox-0.4.9/neetbox/extension/machine/hardware.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # Github: github.com/visualDust
 # Date:   20230413
 
+import functools
 import time
 from threading import Thread
-from typing import List
+from typing import Callable, List
 
 import GPUtil
 import psutil
 from GPUtil import GPU
 from GPUtil import getAvailable as _getAvailableNvGPU
 
 from neetbox.config import export_default_config, get_module_level_config
@@ -163,59 +164,57 @@
         return {
             "cpus": [cpu.json for cpu in self._cpus],
             "cpustat": self._cpu_statistics.json,
             "ram": self._memory.json,
             "gpus": [gpu.json for gpu in self._gpus],
         }
 
-    def set_update_intervel(self, intervel=1.0) -> None:
+    _on_update_call_backs = []
+
+    def add_on_update_call_back(self, func: Callable):
+        self._on_update_call_backs.append(func)
+
+    def set_start_update_intervel(self, intervel=1.0) -> None:
         if intervel < 0:
             self._do_watch = False
             return
         self._do_watch = True
         self._update_interval = intervel
         if not self.watch_thread or not self.watch_thread.is_alive():
-            from neetbox._protocol import EVENT_TYPE_NAME_HARDWARE
-            from neetbox.client import connection
 
-            def watch_hardware(env_instance: Hardware, do_update_gpus: bool):
-                while env_instance._do_watch:
+            def watch_hardware(do_update_gpus: bool):
+                while self._do_watch:
                     # update cpu usage
                     cpu_percent = psutil.cpu_percent(percpu=True)
                     cpu_freq = psutil.cpu_freq(percpu=True)
                     if len(cpu_freq) == 1:
                         cpu_freq = cpu_freq * len(cpu_percent)
                     for index in range(len(cpu_percent)):
-                        env_instance._cpus[index] = CpuStatus(
+                        self._cpus[index] = CpuStatus(
                             id=index,
                             percentage=cpu_percent[index],
                             frequency=cpu_freq[index],
                         )
                     # update memory usage
                     virtual_memory = psutil.virtual_memory()
-                    env_instance._memory = MemoryStatus(
+                    self._memory = MemoryStatus(
                         total=virtual_memory[0] / 1e6,
                         available=virtual_memory[1] / 1e6,
                         used=virtual_memory[3] / 1e6,
                         free=virtual_memory[4] / 1e6,
                     )
                     # update gpu usage
                     if do_update_gpus:
-                        env_instance._gpus = [NvGpuStatus.parse(gpu) for gpu in GPUtil.getGPUs()]
-                    env_instance._cpu_statistics = CpuStatistics(*psutil.cpu_stats())
-                    time.sleep(env_instance._update_interval)
-                    connection.ws_send(
-                        event_type=EVENT_TYPE_NAME_HARDWARE,
-                        payload=env_instance.json,
-                        _history_len=1000,
-                    )
+                        self._gpus = [NvGpuStatus.parse(gpu) for gpu in GPUtil.getGPUs()]
+                    self._cpu_statistics = CpuStatistics(*psutil.cpu_stats())
+                    for callback in self._on_update_call_backs:
+                        callback(self.json)
+                    time.sleep(self._update_interval)
 
-            self.watch_thread = Thread(
-                target=watch_hardware, args=(self, self._with_gpu), daemon=True
-            )
+            self.watch_thread = Thread(target=watch_hardware, args=(self._with_gpu,), daemon=True)
             self.watch_thread.start()
 
 
 Hardware.get_available_NvGPU = _getAvailableNvGPU
 
 # singleton
 hardware = Hardware()
@@ -227,8 +226,19 @@
 
 
 # watch updates in daemon
 @on_workspace_loaded(name="hardware-monit")
 def load_monit_hardware():
     cfg = get_module_level_config()
     if cfg["interval"] > 0:  # if do monit hardware
-        hardware.set_update_intervel(cfg["interval"])
+        from neetbox._protocol import EVENT_TYPE_NAME_HARDWARE
+        from neetbox.client import connection
+
+        def ws_send_on_update(stat_json):
+            connection.ws_send(
+                event_type=EVENT_TYPE_NAME_HARDWARE,
+                payload=stat_json,
+                _history_len=1000,
+            )
+
+        hardware.add_on_update_call_back(ws_send_on_update)
+        hardware.set_start_update_intervel(cfg["interval"])
```

### Comparing `neetbox-0.4.8/neetbox/extension/machine/platform.py` & `neetbox-0.4.9/neetbox/extension/machine/platform.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/pommespeter/pyplot.py` & `neetbox-0.4.9/neetbox/extension/pommespeter/pyplot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/arch/canny.py` & `neetbox-0.4.9/neetbox/extension/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/arch/cnn.py` & `neetbox-0.4.9/neetbox/extension/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/arch/kernels.py` & `neetbox-0.4.9/neetbox/extension/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/arch/mask_boundary_finder.py` & `neetbox-0.4.9/neetbox/extension/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/nlp.py` & `neetbox-0.4.9/neetbox/extension/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/nn/functional.py` & `neetbox-0.4.9/neetbox/extension/torch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/extension/torch/profile.py` & `neetbox-0.4.9/neetbox/extension/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/css/index.be5cc5ae.css` & `neetbox-0.4.9/neetbox/frontend_dist/static/css/index.be5cc5ae.css`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/js/async/704.d0535572.js` & `neetbox-0.4.9/neetbox/frontend_dist/static/js/async/704.d0535572.js`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/js/async/704.d0535572.js.LICENSE.txt` & `neetbox-0.4.9/neetbox/frontend_dist/static/js/async/704.d0535572.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/js/async/704.d0535572.js.map` & `neetbox-0.4.9/neetbox/frontend_dist/static/js/async/704.d0535572.js.map`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/js/index.4a5649a5.js` & `neetbox-0.4.9/neetbox/frontend_dist/static/js/index.4a5649a5.js`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/js/index.4a5649a5.js.LICENSE.txt` & `neetbox-0.4.9/neetbox/frontend_dist/static/js/index.4a5649a5.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/frontend_dist/static/js/index.4a5649a5.js.map` & `neetbox-0.4.9/neetbox/frontend_dist/static/js/index.4a5649a5.js.map`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/logging/_formatting.py` & `neetbox-0.4.9/neetbox/logging/_formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/logging/_logger.py` & `neetbox-0.4.9/neetbox/logging/_logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/logging/writers/_file.py` & `neetbox-0.4.9/neetbox/logging/writers/_file.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/logging/writers/_stdout.py` & `neetbox-0.4.9/neetbox/logging/writers/_stdout.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/server/_bridge.py` & `neetbox-0.4.9/neetbox/server/_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             cls._id2bridge[project_id] = new_bridge
             logger.info(f"created new Bridge for project id '{project_id}'")
         return cls._id2bridge[project_id]
 
     def __del__(self):  # on delete
         logger.info(f"bridge project id {self.project_id} handling on delete...")
         if 0 == len(self.get_run_ids()):  # if there is no active run id
-            self.historyDB.delete_files()
+            self.historyDB.delete()
             del self.historyDB  # delete history db
         logger.info(f"bridge of project id {self.project_id} deleted.")
 
     @classmethod
     def items(cls):
         return cls._id2bridge.items()
```

### Comparing `neetbox-0.4.8/neetbox/server/_daemon_server_launch_script.py` & `neetbox-0.4.9/neetbox/server/_daemon_server_launch_script.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/server/_server.py` & `neetbox-0.4.9/neetbox/server/_server.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/server/db/_condition.py` & `neetbox-0.4.9/neetbox/server/db/project/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # Github: github.com/visualDust
-# Date:   20231120
+# Date:   20240116
 
 import json
-from enum import Enum
 from typing import Dict, Tuple, Union
 
 from neetbox._protocol import *
 
+from ..abc import SortType
 
-class DbQueryFetchType(str, Enum):
-    ALL = "all"
-    ONE = "one"
-    MANY = "many"
 
-
-class DbQuerySortType(str, Enum):
-    ASC = "ASC"
-    DESC = "DESC"
-
-
-class QueryCondition:
+class ProjectDbQueryCondition:
     def __init__(
         self,
         id: Union[Tuple[int, int], int] = None,
         timestamp: Union[Tuple[str, str], str] = None,
         series: str = None,
         run_id: Union[str, int] = None,
         limit: int = None,
-        order: Dict[str, DbQuerySortType] = {},
+        order: Dict[str, SortType] = {},
     ) -> None:
         self.id_range = id if isinstance(id, tuple) else (id, None)
         self.timestamp_range = timestamp if isinstance(timestamp, tuple) else (timestamp, None)
         self.series = series
         self.run_id = run_id
         self.limit = limit
         self.order = {order[0], order[1]} if isinstance(order, tuple) else order
 
     @classmethod
-    def from_json(cls, json_data):
+    def loads(cls, json_data):
         if isinstance(json_data, str):
             json_data = json.loads(json_data)
         """
         {
             "id" : [int,int], # from,to
             "timestamp" : [str,str], # from,to
             "series" : str, # series name
@@ -93,15 +83,15 @@
             limit = json_data["limit"]
             assert type(limit) is int
         # try load order
         order = None
         if "order" in json_data:
             order = json_data["order"]
             assert isinstance(order, dict)
-        return QueryCondition(
+        return ProjectDbQueryCondition(
             id=id_range,
             timestamp=timestamp_range,
             series=series,
             run_id=run_id,
             limit=limit,
             order=order,
         )
@@ -141,15 +131,15 @@
             _run_id_cond_str = f"{RUN_ID_COLUMN_NAME} = ?"
             query_cond_vars.append(self.run_id)
         # === ORDER BY ===
         _order_cond = f"ORDER BY " if self.order else ""
         if self.order:
             for _col_name, _sort in self.order.items():
                 _order_cond += (
-                    f"{_col_name} {_sort.value if isinstance(_sort,DbQuerySortType) else _sort}, "
+                    f"{_col_name} {_sort.value if isinstance(_sort,SortType) else _sort}, "
                 )
             _order_cond = _order_cond[:-2]  # remove last ','
         # === LIMIT ===
         _limit_cond_str = f"LIMIT {self.limit}" if self.limit else ""
         # === concat conditions ===
         query_condition_strs = []
         for cond in [_id_cond_str, _timestamp_cond_str, _series_cond_str, _run_id_cond_str]:
```

### Comparing `neetbox-0.4.8/neetbox/server/db/_manager.py` & `neetbox-0.4.9/neetbox/server/db/_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,40 +2,47 @@
 #
 # Author: GavinGong aka VisualDust
 # Github: github.com/visualDust
 # Date:   20231201
 
 import atexit
 from collections import defaultdict
+from typing import Dict
 
 from neetbox.logging import Logger
 from neetbox.utils.framing import get_caller_identity_traceback
 from neetbox.utils.mvc import Singleton
 
+from .abc import ManageableDB
+
 logger = Logger("DB Manager", skip_writers_names=["ws"])
 
+ModuleNameType = str
+DbIdType = str
+
 
-class DBCPool(metaclass=Singleton):
-    _POOL = defaultdict(dict)
+class DBConnectionManager(metaclass=Singleton):
+    _POOL: Dict[ModuleNameType, Dict[DbIdType, ManageableDB]] = defaultdict(dict)
 
     @property
     def current(self):
         identity = get_caller_identity_traceback(stack_offset=2)
         return self._POOL[identity.module_name]
 
 
-manager = DBCPool()
+manager = DBConnectionManager()
 
 
 def clear_dbc_on_exit():
     logger.info("process exiting, cleaning up...")
     for module_name, conn_dict in manager._POOL.items():
         logger.info(f"closing db connection for module {module_name}:")
+        dbc: ManageableDB
         for _, dbc in conn_dict.items():
             logger.info(f"=> closing {dbc}")
             try:
-                dbc.connection.close()
+                dbc.close()
             except Exception as e:
                 logger.err(RuntimeError(f"failed to close db connection {dbc}, {e}"))
 
 
 atexit.register(clear_dbc_on_exit)
```

### Comparing `neetbox-0.4.8/neetbox/server/db/project.py` & `neetbox-0.4.9/neetbox/server/db/project/_project_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import os
 import sqlite3
 from datetime import datetime
 from threading import Lock
 from typing import Union
 
 from neetbox._protocol import *
-from neetbox.config._global import get as get_global_config
+from neetbox.config.user import get as get_global_config
 from neetbox.logging import Logger
 from neetbox.utils import ResourceLoader
 from neetbox.utils.localstorage import get_file_size_in_bytes
 
-from ._condition import *
-from ._manager import manager
+from .._manager import manager
+from ..abc import FetchType, ManageableDB, SortType
+from .condition import ProjectDbQueryCondition
 
 logger = Logger("PROJECT DB", skip_writers_names=["ws"])
 DB_PROJECT_FILE_FOLDER = f"{get_global_config('vault')}/server/history"
 DB_PROJECT_FILE_TYPE_NAME = "projectdb"
 
 
-class ProjectDB:
+class ProjectDB(ManageableDB):
     # static things
     _path2dbc = {}
 
     # not static. instance level vars
     project_id: str  # of which project id
     file_path: str  # where is the db file
     connection: sqlite3.Connection  # the db connection
@@ -67,22 +68,34 @@
         cls._path2dbc[path] = new_dbc
         manager.current[project_id] = new_dbc
         new_dbc.project_id = project_id
         logger.ok(f"History file(version={_db_file_version}) for project id '{project_id}' loaded.")
         return new_dbc
 
     @property
-    def local_storage_size_in_bytes(self):
+    def size(self):
+        """return local storage usage by this project db in bytes
+
+        Returns:
+            int: size in bytes
+        """
         try:
             result = get_file_size_in_bytes(self.file_path)
         except Exception as e:
             result = f"failed to get file size cause {e}"
         return result
 
-    def delete_files(self):
+    def close(self):
+        try:
+            self.connection.commit()
+        except:
+            pass
+        self.connection.close()
+
+    def delete(self):
         """delete related files of db"""
         if self.project_id not in manager.current:
             logger.err(
                 RuntimeError(f"could not find db to delete with project id {self.project_id}")
             )
         del manager.current[self.project_id]
         del ProjectDB._path2dbc[self.file_path]
@@ -117,51 +130,51 @@
 
     @classmethod
     def of_project_id(cls, project_id):
         if project_id in manager.current:
             return manager.current[project_id]
         return ProjectDB(project_id)
 
-    def _execute(self, query, *args, fetch: DbQueryFetchType = DbQueryFetchType.ALL, **kwargs):
+    def _execute(self, query, *args, fetch: FetchType = FetchType.ALL, **kwargs):
         cur = self.connection.cursor()
         try:
             result = cur.execute(query, args)
         except Exception as e:
             logger.err(f"failed to execute query cause '{e}'")
             logger.info(f"{query}, {args}")
             logger.err(e, reraise=True)
         if fetch:
-            if fetch == DbQueryFetchType.ALL:
+            if fetch == FetchType.ALL:
                 result = result.fetchall()
-            elif fetch == DbQueryFetchType.ONE:
+            elif fetch == FetchType.ONE:
                 result = result.fetchone()
-            elif fetch == DbQueryFetchType.MANY:
+            elif fetch == FetchType.MANY:
                 result = result.fetchmany(kwargs["many"])
         return result, cur.lastrowid
 
-    def _query(self, query, *args, fetch: DbQueryFetchType = DbQueryFetchType.ALL, **kwargs):
+    def _query(self, query, *args, fetch: FetchType = FetchType.ALL, **kwargs):
         return self._execute(query, *args, fetch=fetch, **kwargs)
 
     def table_exist(self, table_name):
         sql_query = f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table_name}';"
-        result, _ = self._query(sql_query, fetch=DbQueryFetchType.ALL)
+        result, _ = self._query(sql_query, fetch=FetchType.ALL)
         return result != []
 
     def get_table_names(self):
         sql_query = "SELECT name FROM sqlite_master;"
-        table_names, _ = self._query(sql_query, fetch=DbQueryFetchType.ALL)
+        table_names, _ = self._query(sql_query, fetch=FetchType.ALL)
         return table_names
 
     def fetch_db_version(self, default=None):
         if not self._inited_tables[VERSION_TABLE_NAME]:  # create if there is no version table
             sql_query = f"CREATE TABLE IF NOT EXISTS {VERSION_TABLE_NAME} ( {VERSION_TABLE_NAME} TEXT NON NULL );"
             self._execute(sql_query)
             self._inited_tables[VERSION_TABLE_NAME] = True
         sql_query = f"SELECT {VERSION_TABLE_NAME} FROM {VERSION_TABLE_NAME}"
-        _version, _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+        _version, _ = self._query(sql_query, fetch=FetchType.ONE)
         if _version is None:
             if default is None:
                 raise RuntimeError(
                     "should provide a default version if fetching from empty version"
                 )
             sql_query = f"INSERT INTO {VERSION_TABLE_NAME} VALUES (?);"
             self._execute(sql_query, default)
@@ -170,29 +183,29 @@
 
     def fetch_db_project_id(self, default=None):
         if not self._inited_tables[PROJECT_ID_TABLE_NAME]:  # create if there is no project id table
             sql_query = f"CREATE TABLE IF NOT EXISTS {PROJECT_ID_TABLE_NAME} ( {PROJECT_ID_TABLE_NAME} TEXT NON NULL );"
             self._execute(sql_query)
             self._inited_tables[PROJECT_ID_TABLE_NAME] = True
         sql_query = f"SELECT {PROJECT_ID_TABLE_NAME} FROM {PROJECT_ID_TABLE_NAME}"
-        _projectid, _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+        _projectid, _ = self._query(sql_query, fetch=FetchType.ONE)
         if _projectid is None:
             if default is None:
                 raise RuntimeError(
                     "should provide a default project id if fetching from empty project id"
                 )
             sql_query = f"INSERT INTO {PROJECT_ID_TABLE_NAME} VALUES (?);"
             self._execute(sql_query, default)
             return default
         return _projectid[0]
 
     def get_id_of_run_id(self, run_id: str):
         try:
             sql_query = f"SELECT {ID_COLUMN_NAME} FROM {RUN_IDS_TABLE_NAME} WHERE {RUN_ID_COLUMN_NAME} == '{run_id}'"
-            _id, _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+            _id, _ = self._query(sql_query, fetch=FetchType.ONE)
             return _id[0]
         except:
             return None
 
     _run_id_fetch_lock = Lock()
 
     def fetch_id_of_run_id(self, run_id: str, timestamp: str = None):
@@ -215,24 +228,24 @@
             return None
         if metadata:  # if update name
             metadata = json.dumps(metadata) if isinstance(metadata, dict) else metadata
             sql_query = f"UPDATE {RUN_IDS_TABLE_NAME} SET {METADATA_COLUMN_NAME} = ? WHERE {ID_COLUMN_NAME} = ?"
             _, _ = self._execute(sql_query, metadata, id_of_run_id)
         # get name
         sql_query = f"SELECT {METADATA_COLUMN_NAME} FROM {RUN_IDS_TABLE_NAME} WHERE {ID_COLUMN_NAME} == {id_of_run_id}"
-        (metadata,), _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+        (metadata,), _ = self._query(sql_query, fetch=FetchType.ONE)
         metadata = (
             json.loads(metadata) if metadata else {}
         )  # if does not have metadata, return an empty one
         return metadata
 
     def get_run_id_of_id(self, id_of_run_id):
         try:
             sql_query = f"SELECT {RUN_ID_COLUMN_NAME} FROM {RUN_IDS_TABLE_NAME} WHERE {ID_COLUMN_NAME} == {id_of_run_id}"
-            run_id, _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+            run_id, _ = self._query(sql_query, fetch=FetchType.ONE)
             return run_id[0]
         except:
             return None
 
     def get_run_ids(self):
         if not self.table_exist(RUN_IDS_TABLE_NAME):
             return []
@@ -257,29 +270,29 @@
             return []
         if run_id is not None:
             sql_query = f"SELECT DISTINCT t.series as series FROM {RUN_IDS_TABLE_NAME} r LEFT JOIN {table_name} t ON r.{RUN_ID_COLUMN_NAME} == ? WHERE t.{RUN_ID_COLUMN_NAME} == r.{ID_COLUMN_NAME}"
             args = (run_id,)
         else:
             sql_query = f"SELECT DISTINCT series FROM {table_name}"
             args = ()
-        result, _ = self._query(sql_query, *args, fetch=DbQueryFetchType.ALL)
+        result, _ = self._query(sql_query, *args, fetch=FetchType.ALL)
         return [result for (result,) in result]
 
     def do_limit_num_row_for(
         self, table_name: str, run_id: str, num_row_limit: int, series: str = None
     ):
         if num_row_limit <= 0:  # no limit or random not triggered
             return
         sql_query = f"SELECT count(*) from {table_name} WHERE {RUN_ID_COLUMN_NAME} = {run_id}"  # count rows for run id in specific table
         if series is not None:
             sql_query += f" AND {SERIES_COLUMN_NAME} = '{series}'"
-        num_rows, _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+        num_rows, _ = self._query(sql_query, fetch=FetchType.ONE)
         if num_rows[0] > num_row_limit:  # num rows exceeded limit
             sql_query = f"SELECT {ID_COLUMN_NAME} from {table_name} WHERE {RUN_ID_COLUMN_NAME} = {run_id} ORDER BY {ID_COLUMN_NAME} DESC LIMIT 1 OFFSET {num_row_limit - 1}"  # get max id to delete of row for specific run id
-            max_id_to_del, _ = self._query(sql_query, fetch=DbQueryFetchType.ONE)
+            max_id_to_del, _ = self._query(sql_query, fetch=FetchType.ONE)
             sql_query = f"DELETE FROM {table_name} WHERE {ID_COLUMN_NAME} < {max_id_to_del[0]} AND {RUN_ID_COLUMN_NAME} = {run_id}"
             if series is not None:
                 sql_query += f" AND {SERIES_COLUMN_NAME} = '{series}'"
             self._query(sql_query)  # delete rows with smaller id and specific run id
 
     def write_json(
         self,
@@ -306,22 +319,22 @@
             json_data = json.dumps(json_data)
         _, lastrowid = self._execute(sql_query, timestamp, series, run_id, json_data)
         self.do_limit_num_row_for(
             table_name=table_name, run_id=run_id, num_row_limit=num_row_limit, series=series
         )
         return lastrowid
 
-    def read_json(self, table_name: str, condition: QueryCondition = None):
+    def read_json(self, table_name: str, condition: ProjectDbQueryCondition = None):
         if not self.table_exist(table_name):
             return []
         if condition and isinstance(condition.run_id, str):
             condition.run_id = self.get_id_of_run_id(condition.run_id)  # convert run id
         cond_str, cond_vars = condition.dumpt() if condition else ""
         sql_query = f"SELECT {', '.join((ID_COLUMN_NAME, TIMESTAMP_COLUMN_NAME,SERIES_COLUMN_NAME, JSON_COLUMN_NAME))} FROM {table_name} {cond_str}"
-        result, _ = self._query(sql_query, *cond_vars, fetch=DbQueryFetchType.ALL)
+        result, _ = self._query(sql_query, *cond_vars, fetch=FetchType.ALL)
         result = [
             {
                 ID_COLUMN_NAME: w,
                 TIMESTAMP_COLUMN_NAME: x,
                 SERIES_COLUMN_NAME: y,
                 JSON_COLUMN_NAME: json.loads(z) if z else None,
             }
@@ -345,20 +358,20 @@
             json_data = json.dumps(json_data)
         _, lastrowid = self._execute(sql_query, run_id, series, json_data)
         return lastrowid
 
     def get_status(self, run_id: str = None, series: str = None):
         if not self.table_exist(STATUS_TABLE_NAME):
             return {}
-        condition = QueryCondition(run_id=run_id, series=series)
+        condition = ProjectDbQueryCondition(run_id=run_id, series=series)
         if isinstance(condition.run_id, str):
             condition.run_id = self.get_id_of_run_id(run_id)
         cond_str, cond_vars = condition.dumpt()
         sql_query = f"SELECT {', '.join((RUN_ID_COLUMN_NAME, SERIES_COLUMN_NAME, JSON_COLUMN_NAME))} FROM {STATUS_TABLE_NAME} {cond_str}"
-        query_result, _ = self._query(sql_query, *cond_vars, fetch=DbQueryFetchType.ALL)
+        query_result, _ = self._query(sql_query, *cond_vars, fetch=FetchType.ALL)
         result = {}
         for id_of_runid, series_name, value in query_result:
             run_id = self.get_run_id_of_id(id_of_runid)
             if run_id and run_id not in result:
                 result[run_id] = {}
             result[run_id][series_name] = json.loads(value)
         return result
@@ -392,22 +405,24 @@
         sql_query = f"INSERT INTO {table_name}({TIMESTAMP_COLUMN_NAME}, {SERIES_COLUMN_NAME}, {RUN_ID_COLUMN_NAME}, {METADATA_COLUMN_NAME}, {BLOB_COLUMN_NAME}) VALUES (?, ?, ?, ?, ?)"
         _, lastrowid = self._execute(sql_query, timestamp, series, run_id, meta_data, blob_data)
         self.do_limit_num_row_for(
             table_name=table_name, run_id=run_id, num_row_limit=num_row_limit, series=series
         )
         return lastrowid
 
-    def read_blob(self, table_name: str, condition: QueryCondition = None, meta_only=False):
+    def read_blob(
+        self, table_name: str, condition: ProjectDbQueryCondition = None, meta_only=False
+    ):
         if not self.table_exist(table_name):
             return []
         if condition and isinstance(condition.run_id, str):
             condition.run_id = self.get_id_of_run_id(condition.run_id)  # convert run id
         cond_str, cond_vars = condition.dumpt() if condition else ""
         sql_query = f"SELECT {', '.join((ID_COLUMN_NAME,TIMESTAMP_COLUMN_NAME, METADATA_COLUMN_NAME, *((BLOB_COLUMN_NAME,) if not meta_only else ())))} FROM {table_name} {cond_str}"
-        result, _ = self._query(sql_query, *cond_vars, fetch=DbQueryFetchType.ALL)
+        result, _ = self._query(sql_query, *cond_vars, fetch=FetchType.ALL)
         return result
 
     @classmethod
     def load_db_of_path(cls, path):
         if not os.path.isfile(path):
             raise RuntimeError(f"{path} is not a file")
         conn = ProjectDB(path=path)
@@ -431,11 +446,12 @@
         return conn
 
 
 # === SCAN FOR DB FILES ===
 
 if not os.path.exists(DB_PROJECT_FILE_FOLDER):
     # create history root dir
+    logger.info(f"history file directory not exist, trying to create at {DB_PROJECT_FILE_FOLDER}")
     os.makedirs(DB_PROJECT_FILE_FOLDER)
 # check if is dir
 assert os.path.isdir(DB_PROJECT_FILE_FOLDER), f"{DB_PROJECT_FILE_FOLDER} is not a directory."
 logger.info(f"using history file folder: {DB_PROJECT_FILE_FOLDER}")
```

### Comparing `neetbox-0.4.8/neetbox/server/fastapi/_fastapi_server.py` & `neetbox-0.4.9/neetbox/server/fastapi/_fastapi_server.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/server/fastapi/routers/project.py` & `neetbox-0.4.9/neetbox/server/fastapi/routers/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from fastapi import APIRouter, Body, File, Form, HTTPException, Response, UploadFile
 
 from neetbox._protocol import *
 from neetbox.logging import Logger, LogLevel
 
 from ..._bridge import Bridge
-from ...db import QueryCondition
+from ...db.project.condition import ProjectDbQueryCondition
 
 logger = Logger("FASTAPI", skip_writers_names=["ws"])
 logger.log_level = LogLevel.DEBUG
 
 router = APIRouter()
 
 
@@ -39,29 +39,29 @@
     for run_id_info in reversed(run_id_info_list):
         config = bridge.get_status(run_id=run_id_info[RUN_ID_KEY], series="config")
         if NAME_KEY in config:
             name_of_project = config[NAME_KEY]
             break
     return {
         PROJECT_ID_KEY: bridge.project_id,
-        "storage": bridge.historyDB.local_storage_size_in_bytes,
+        "storage": bridge.historyDB.size,
         "online": bridge.is_online(),
         NAME_KEY: name_of_project,
         "runids": run_id_info_list,
     }
 
 
 def get_history_json_of(project_id: str, table_name: str, condition=Union[dict, str]):
     if not Bridge.has(project_id):
         raise HTTPException(status_code=404, detail={ERROR_KEY: "Project ID not found"})
     try:
         if isinstance(condition, str):
             condition = json.loads(condition)
         if isinstance(condition, dict):
-            condition = QueryCondition.from_json(condition)
+            condition = ProjectDbQueryCondition.loads(condition)
     except Exception as e:  # if failed to parse
         error_message = f"failed to parse condition from {type(condition)}{condition} :{e}"
         logger.debug(error_message, series="400")
         raise HTTPException(status_code=400, detail={ERROR_KEY: error_message})
     return Bridge.of_id(project_id).read_json_from_history(
         table_name=table_name, condition=condition
     )
@@ -149,49 +149,49 @@
 
 @router.get(f"/{{project_id}}/image/{{image_id}}")
 async def get_image_of(project_id: str, image_id: int, meta: Optional[bool] = None):
     if not Bridge.has(project_id):
         raise HTTPException(status_code=404, detail={ERROR_KEY: "project id not found"})
     # Database logic here
     [(_, _, meta_data, image)] = Bridge.of_id(project_id).read_blob_from_history(
-        table_name="image", condition=QueryCondition(id=image_id), meta_only=meta
+        table_name="image", condition=ProjectDbQueryCondition(id=image_id), meta_only=meta
     )
     if meta:
         return Response(meta_data, media_type="application/json")
     else:
         return Response(image, media_type="image/png")
 
 
 @router.get(f"/{{project_id}}/image")
 async def get_history_image_metadata_of(project_id: str, condition: Optional[str] = None):
     if not Bridge.has(project_id):
         raise HTTPException(status_code=404, detail={ERROR_KEY: "project id not found"})
     try:
         condition_json = json.loads(condition) if condition else {}
-        condition = QueryCondition.from_json(condition_json)
+        condition = ProjectDbQueryCondition.loads(condition_json)
     except Exception as e:
         raise HTTPException(status_code=400, detail={ERROR_KEY: str(e)})
     query_results = Bridge.of_id(project_id).read_blob_from_history(
         table_name="image", condition=condition, meta_only=True
     )
     result = [{"imageId": id, "metadata": meta_data} for (id, _, meta_data) in query_results]
     return result
 
 
 @router.get(f"/{{project_id}}/scalar")
 async def get_history_scalar_of(project_id: str, condition: str = None):
     try:
         condition_json = json.loads(condition) if condition else "{}"
-        condition = QueryCondition.from_json(condition_json)
+        condition = ProjectDbQueryCondition.loads(condition_json)
     except Exception as e:
         raise HTTPException(status_code=400, detail={ERROR_KEY: str(e)})
     return get_history_json_of(project_id=project_id, table_name="scalar", condition=condition)
 
 
 @router.get(f"/{{project_id}}/progress")
 async def get_history_progress_of(project_id: str, condition: str = None):
     try:
         condition_json = json.loads(condition) if condition else "{}"
-        condition = QueryCondition.from_json(condition_json)
+        condition = ProjectDbQueryCondition.loads(condition_json)
     except Exception as e:
         raise HTTPException(status_code=400, detail={ERROR_KEY: str(e)})
     return get_history_json_of(project_id=project_id, table_name="progress", condition=condition)
```

### Comparing `neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/_event_type_handlers.py` & `neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/_event_type_handlers.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/_manager.py` & `neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/_manager.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/server/fastapi/routers/websocket/_websocket_server.py` & `neetbox-0.4.9/neetbox/server/fastapi/routers/websocket/_websocket_server.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/_daemonable_process.py` & `neetbox-0.4.9/neetbox/utils/_daemonable_process.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/_package.py` & `neetbox-0.4.9/neetbox/utils/_package.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/_registry.py` & `neetbox-0.4.9/neetbox/utils/_registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/_resource.py` & `neetbox-0.4.9/neetbox/utils/_resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/ansi.py` & `neetbox-0.4.9/neetbox/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/framing.py` & `neetbox-0.4.9/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/localstorage.py` & `neetbox-0.4.9/neetbox/utils/localstorage.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,24 @@
     # On non-windows, use XDG_CONFIG_HOME if set, else default to ~/.config.
     xdg_config_home = os.getenv("XDG_CONFIG_HOME")
     if xdg_config_home:
         return xdg_config_home
     return os.path.join(os.path.expanduser("~"), ".config")
 
 
+def get_create_neetbox_config_directory():
+    path = os.path.join(get_user_config_directory(), "neetbox")
+    if not os.path.exists(path):
+        os.makedirs(path)
+    assert os.path.isdir(
+        path
+    ), f"Fialed to create neetbox config directory {path}, please check your permission or create it manually."
+    return path
+
+
 def get_user_app_data_directory():
     """
     Returns a parent directory path
     where persistent application data can be stored.
 
     - linux: ~/.local/share
     - macOS: ~/Library/Application Support
```

### Comparing `neetbox-0.4.8/neetbox/utils/massive.py` & `neetbox-0.4.9/neetbox/utils/massive.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/mvc.py` & `neetbox-0.4.9/neetbox/utils/mvc.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/neetbox/utils/x2numpy.py` & `neetbox-0.4.9/neetbox/utils/x2numpy.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.4.8/pyproject.toml` & `neetbox-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.4.8"
+version = "0.4.9"
 description = "Logging/Debugging/Tracing/Managing/Facilitating long running python projects, especially a replacement of tensorboard for deep learning projects"
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>", "Lideming <me@yuuza.net>"]
 maintainers = [
     "PaperCube <imzhy@hotmail.com>",
     "PommesPeter <me@pommespeter.space>",
     "PuQing <me@puqing.work>",
```

### Comparing `neetbox-0.4.8/PKG-INFO` & `neetbox-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.4.8
+Version: 0.4.9
 Summary: Logging/Debugging/Tracing/Managing/Facilitating long running python projects, especially a replacement of tensorboard for deep learning projects
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: PaperCube
```

