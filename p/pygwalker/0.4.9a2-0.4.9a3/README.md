# Comparing `tmp/pygwalker-0.4.9a2.tar.gz` & `tmp/pygwalker-0.4.9a3.tar.gz`

## Comparing `pygwalker-0.4.9a2.tar` & `pygwalker-0.4.9a3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/.gitignore
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/components.json
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/index.html
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/package.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/postcss.config.js
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/tailwind.config.js
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/tsconfig.json
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/vite.config.ts
--rw-r--r--   0        0        0   279367 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/yarn.lock
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/index.css
--rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/index.tsx
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/options.tsx
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/codeExportModal/index.tsx
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/codeExportModal/usePythonCode.ts
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/initModal/index.tsx
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/preview/index.tsx
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/badge.tsx
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/button.tsx
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/checkbox.tsx
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/input.tsx
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/label.tsx
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/select.tsx
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/tabs.tsx
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/toggle-group.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/ui/toggle.tsx
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/uploadChartModal/index.tsx
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/components/uploadSpecModal/index.tsx
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/dataSource/index.ts
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/interfaces/index.ts
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/notify/index.tsx
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/store/common.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/store/communication.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/store/context.ts
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/exportDataframe.tsx
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/exportTool.tsx
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/loginTool.tsx
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/tools/saveTool.tsx
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/communication.tsx
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/context.tsx
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/formatSpec.ts
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/save.ts
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/theme.ts
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/app/src/utils/userConfig.ts
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/bin/pygwalker_command.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/_constants.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/_typing.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/__init__.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/gradio.py
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/html.py
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/jupyter.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/kanaries_cloud.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/pygwalker.py
--rw-r--r--   0        0        0    11657 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/api/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/base.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/gradio_comm.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/hacker_comm.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/communications/streamlit_comm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/__init__.py
--rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/base.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/cloud_dataset_parser.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/database_parser.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/modin_parser.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/pandas_parser.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/polars_parser.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/data_parsers/spark_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/check_update.py
--rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/cloud_service.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/config.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/data_parsers.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/fname_encodings.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/format_invoke_walk_code.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/global_var.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/kaggle.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/kanaries_cli_login.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/preview_image.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/render.py
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/spec.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/streamlit_components.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/tip_tools.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/track.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/services/upload_data.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/index.html
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/preview.html
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/preview_list.html
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/pygwalker_iframe.html
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/pygwalker_main_page.html
--rw-r--r--   0        0        0   336362 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/dsl-to-workflow.umd.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  6847039 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0   333908 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/vega-to-dsl.umd.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/codeExportModal/index.d.ts
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/codeExportModal/usePythonCode.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/initModal/index.d.ts
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/preview/index.d.ts
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/badge.d.ts
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/button.d.ts
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/checkbox.d.ts
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/dialog.d.ts
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/input.d.ts
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/label.d.ts
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/select.d.ts
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/tabs.d.ts
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle-group.d.ts
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle.d.ts
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/uploadChartModal/index.d.ts
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/components/uploadSpecModal/index.d.ts
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/dataSource/index.d.ts
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/lib/dslToWorkflow.d.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/lib/utils.d.ts
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/lib/vegaToDsl.d.ts
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/notify/index.d.ts
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/store/common.d.ts
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/store/communication.d.ts
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/store/context.d.ts
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/exportDataframe.d.ts
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/exportTool.d.ts
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/loginTool.d.ts
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/tools/saveTool.d.ts
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/communication.d.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/context.d.ts
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/formatSpec.d.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/save.d.ts
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/theme.d.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/templates/dist/utils/userConfig.d.ts
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/check_walker_params.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/custom_sqlglot.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/display.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/dsl_transform.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/encode.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/estimate_tools.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/execute_env_check.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/log.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/payload_to_sql.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker/utils/randoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/metrics/__init__.py
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/metrics/api.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pygwalker_tools/metrics/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/__init__.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/compile.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/LICENSE
--rw-r--r--   0        0        0    17199 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/README.md
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/pyproject.toml
--rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 pygwalker-0.4.9a2/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/.gitignore
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/components.json
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/index.html
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/package.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/postcss.config.js
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/tailwind.config.js
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/tsconfig.json
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/vite.config.ts
+-rw-r--r--   0        0        0   279367 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/yarn.lock
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/index.css
+-rw-r--r--   0        0        0    19971 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/index.tsx
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/options.tsx
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/codeExportModal/index.tsx
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/codeExportModal/usePythonCode.ts
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/initModal/index.tsx
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/preview/index.tsx
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/badge.tsx
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/button.tsx
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/checkbox.tsx
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/input.tsx
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/label.tsx
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/select.tsx
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/tabs.tsx
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/toggle-group.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/ui/toggle.tsx
+-rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/uploadChartModal/index.tsx
+-rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/components/uploadSpecModal/index.tsx
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/dataSource/index.ts
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/notify/index.tsx
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/store/common.ts
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/store/communication.ts
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/store/context.ts
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/tools/exportDataframe.tsx
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/tools/exportTool.tsx
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/tools/loginTool.tsx
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/tools/saveTool.tsx
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/utils/communication.tsx
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/utils/context.tsx
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/utils/formatSpec.ts
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/utils/save.ts
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/utils/theme.ts
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/app/src/utils/userConfig.ts
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/bin/pygwalker_command.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/_constants.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/_typing.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/__init__.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/gradio.py
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/html.py
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/jupyter.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/kanaries_cloud.py
+-rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/pygwalker.py
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/api/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/communications/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/communications/base.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/communications/gradio_comm.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/communications/hacker_comm.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/communications/streamlit_comm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/__init__.py
+-rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/base.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/cloud_dataset_parser.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/database_parser.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/modin_parser.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/pandas_parser.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/polars_parser.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/data_parsers/spark_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/check_update.py
+-rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/cloud_service.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/config.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/data_parsers.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/fname_encodings.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/format_invoke_walk_code.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/global_var.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/kaggle.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/kanaries_cli_login.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/preview_image.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/render.py
+-rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/spec.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/streamlit_components.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/tip_tools.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/track.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/services/upload_data.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/preview.html
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/preview_list.html
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/pygwalker_iframe.html
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/pygwalker_main_page.html
+-rw-r--r--   0        0        0   336362 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/dsl-to-workflow.umd.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  6847127 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0   333908 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/vega-to-dsl.umd.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/codeExportModal/index.d.ts
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/codeExportModal/usePythonCode.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/initModal/index.d.ts
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/preview/index.d.ts
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/badge.d.ts
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/button.d.ts
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/checkbox.d.ts
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/dialog.d.ts
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/input.d.ts
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/label.d.ts
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/select.d.ts
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/tabs.d.ts
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/toggle-group.d.ts
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/toggle.d.ts
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/uploadChartModal/index.d.ts
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/components/uploadSpecModal/index.d.ts
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/dataSource/index.d.ts
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/lib/dslToWorkflow.d.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/lib/utils.d.ts
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/lib/vegaToDsl.d.ts
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/notify/index.d.ts
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/store/common.d.ts
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/store/communication.d.ts
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/store/context.d.ts
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/tools/exportDataframe.d.ts
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/tools/exportTool.d.ts
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/tools/loginTool.d.ts
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/tools/saveTool.d.ts
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/utils/communication.d.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/utils/context.d.ts
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/utils/formatSpec.d.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/utils/save.d.ts
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/utils/theme.d.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/templates/dist/utils/userConfig.d.ts
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/check_walker_params.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/custom_sqlglot.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/display.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/dsl_transform.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/encode.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/estimate_tools.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/execute_env_check.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/log.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/payload_to_sql.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker/utils/randoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker_tools/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker_tools/metrics/__init__.py
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker_tools/metrics/api.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pygwalker_tools/metrics/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/scripts/__init__.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/scripts/compile.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/LICENSE
+-rw-r--r--   0        0        0    17505 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/README.md
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/pyproject.toml
+-rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 pygwalker-0.4.9a3/PKG-INFO
```

### Comparing `pygwalker-0.4.9a2/app/package.json` & `pygwalker-0.4.9a3/app/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992897727272727%*

 * *Differences: {"'dependencies'": "{'@kanaries/graphic-walker': '0.4.63'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "dependencies": {
         "@headlessui/react": "^1.7.14",
         "@heroicons/react": "^2.0.8",
-        "@kanaries/graphic-walker": "0.4.62",
+        "@kanaries/graphic-walker": "0.4.63",
         "@kanaries/gw-dsl-parser": "0.1.47",
         "@radix-ui/react-checkbox": "^1.0.4",
         "@radix-ui/react-dialog": "^1.0.5",
         "@radix-ui/react-icons": "^1.3.0",
         "@radix-ui/react-label": "^2.0.2",
         "@radix-ui/react-select": "^2.0.0",
         "@radix-ui/react-slot": "^1.0.2",
```

### Comparing `pygwalker-0.4.9a2/app/tailwind.config.js` & `pygwalker-0.4.9a3/app/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/tsconfig.json` & `pygwalker-0.4.9a3/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/vite.config.ts` & `pygwalker-0.4.9a3/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/yarn.lock` & `pygwalker-0.4.9a3/app/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1041,18 +1041,18 @@
   version "0.3.18"
   resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz#25783b2086daf6ff1dcb53c9249ae480e4dd4cd6"
   integrity sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==
   dependencies:
     "@jridgewell/resolve-uri" "3.1.0"
     "@jridgewell/sourcemap-codec" "1.4.14"
 
-"@kanaries/graphic-walker@0.4.62":
-  version "0.4.62"
-  resolved "https://registry.yarnpkg.com/@kanaries/graphic-walker/-/graphic-walker-0.4.62.tgz#59f6b4fbf2913ab3416a5334692f5f2f93e81f8e"
-  integrity sha512-fQCR3Eqxf3An1DH/g8q+ZsEV8ewtcD0G48IBD1eu2+HxR+F0qd/Sa4zcIQD9b7Aa9WCX8G7tyRYeSD64ZOFhMQ==
+"@kanaries/graphic-walker@0.4.63":
+  version "0.4.63"
+  resolved "https://registry.yarnpkg.com/@kanaries/graphic-walker/-/graphic-walker-0.4.63.tgz#2ab7d655f5530f1aeec0ec934e144a7129a5badb"
+  integrity sha512-GqailsQBkRFSr14ZjNn447ZbE7CmNVvMCMcYy21xmmfH8yW16TtVtht649zDRsBtmkp4X4s2he5SMEf++HLgPw==
   dependencies:
     "@headlessui-float/react" "^0.11.4"
     "@headlessui/react" "1.7.12"
     "@heroicons/react" "^2.0.8"
     "@kanaries/react-beautiful-dnd" "^0.1.1"
     "@kanaries/web-data-loader" "^0.1.7"
     "@radix-ui/react-checkbox" "^1.0.4"
```

### Comparing `pygwalker-0.4.9a2/app/src/index.css` & `pygwalker-0.4.9a3/app/src/index.css`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/index.tsx` & `pygwalker-0.4.9a3/app/src/index.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 import { SunIcon, MoonIcon, DesktopIcon, DotsHorizontalIcon, Cross2Icon } from "@radix-ui/react-icons"
 
 // @ts-ignore
 import style from './index.css?inline'
 import { currentMediaTheme } from './utils/theme';
 import { AppContext, darkModeContext } from './store/context';
 import FormatSpec from './utils/formatSpec';
-import { Button } from './components/ui/button';
 
 
 const initChart = async (gwRef: React.MutableRefObject<IGWHandler | null>, total: number, props: IAppProps) => {
     if (props.needInitChart && props.env === "jupyter_widgets" && total !== 0) {
         commonStore.setInitModalOpen(true);
         commonStore.setInitModalInfo({
             title: "Recover Charts",
@@ -391,17 +390,21 @@
             <ChartPreview {...props} />
         </MainApp>,
         document.getElementById(id)
     );
 }
 
 function GraphicRendererApp(props: IAppProps) {
+    const containerSize = props["containerSize"] ?? [null, null];
     const globalProps = {
         rawFields: props.rawFields,
-        containerStyle: { height: "700px", width: "60%" },
+        containerStyle: {
+            height: containerSize[1] ? `${containerSize[1]}px` : "700px",
+            width: containerSize[0] ? `${containerSize[0]}px` : "60%"
+        },
         themeKey:props.themeKey,
         dark: useContext(darkModeContext),
     }
     const computationCallback = React.useMemo(() => getComputationCallback(props), []);
     const visSpec = useMemo(() => props.visSpec.map((chart) => [chart]), []);
 
     return (
```

### Comparing `pygwalker-0.4.9a2/app/src/components/options.tsx` & `pygwalker-0.4.9a3/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/codeExportModal/index.tsx` & `pygwalker-0.4.9a3/app/src/components/codeExportModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/codeExportModal/usePythonCode.ts` & `pygwalker-0.4.9a3/app/src/components/codeExportModal/usePythonCode.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/initModal/index.tsx` & `pygwalker-0.4.9a3/app/src/components/initModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/preview/index.tsx` & `pygwalker-0.4.9a3/app/src/components/preview/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/badge.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/badge.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/button.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/checkbox.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/checkbox.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/dialog.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/input.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/input.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/label.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/label.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/select.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/select.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/tabs.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/tabs.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/toggle-group.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/toggle-group.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/ui/toggle.tsx` & `pygwalker-0.4.9a3/app/src/components/ui/toggle.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/uploadChartModal/index.tsx` & `pygwalker-0.4.9a3/app/src/components/uploadChartModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/components/uploadSpecModal/index.tsx` & `pygwalker-0.4.9a3/app/src/components/uploadSpecModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/dataSource/index.ts` & `pygwalker-0.4.9a3/app/src/dataSource/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/interfaces/index.ts` & `pygwalker-0.4.9a3/app/src/interfaces/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/notify/index.tsx` & `pygwalker-0.4.9a3/app/src/notify/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/store/common.ts` & `pygwalker-0.4.9a3/app/src/store/common.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/tools/exportDataframe.tsx` & `pygwalker-0.4.9a3/app/src/tools/exportDataframe.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/tools/exportTool.tsx` & `pygwalker-0.4.9a3/app/src/tools/exportTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/tools/loginTool.tsx` & `pygwalker-0.4.9a3/app/src/tools/loginTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/tools/saveTool.tsx` & `pygwalker-0.4.9a3/app/src/tools/saveTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/utils/communication.tsx` & `pygwalker-0.4.9a3/app/src/utils/communication.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/utils/context.tsx` & `pygwalker-0.4.9a3/app/src/utils/context.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/app/src/utils/save.ts` & `pygwalker-0.4.9a3/app/src/utils/save.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/bin/pygwalker_command.py` & `pygwalker-0.4.9a3/bin/pygwalker_command.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/__init__.py` & `pygwalker-0.4.9a3/pygwalker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 from pygwalker.utils.randoms import rand_str as __rand_str
 from pygwalker.utils.execute_env_check import check_kaggle as __check_kaggle
 from pygwalker.services.global_var import GlobalVarManager
 from pygwalker.services.kaggle import show_tips_user_kaggle as __show_tips_user_kaggle
 
-__version__ = "0.4.9a2"
+__version__ = "0.4.9a3"
 __hash__ = __rand_str()
 
 from pygwalker.api.jupyter import walk, render, table
 from pygwalker.api.html import to_html
 from pygwalker.data_parsers.base import FieldSpec
 
 if GlobalVarManager.privacy == 'offline':
```

### Comparing `pygwalker-0.4.9a2/pygwalker/_typing.py` & `pygwalker-0.4.9a3/pygwalker/_typing.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/errors.py` & `pygwalker-0.4.9a3/pygwalker/errors.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/api/gradio.py` & `pygwalker-0.4.9a3/pygwalker/api/gradio.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/api/html.py` & `pygwalker-0.4.9a3/pygwalker/api/html.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/api/jupyter.py` & `pygwalker-0.4.9a3/pygwalker/api/jupyter.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/api/kanaries_cloud.py` & `pygwalker-0.4.9a3/pygwalker/api/kanaries_cloud.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/api/pygwalker.py` & `pygwalker-0.4.9a3/pygwalker/api/pygwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/api/streamlit.py` & `pygwalker-0.4.9a3/pygwalker/api/streamlit.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,18 +177,27 @@
             })
         return gw_filters
 
     def set_global_pre_filters(self, pre_filters: List[PreFilter]):
         """It will append new filters to exists charts."""
         self.global_pre_filters = pre_filters
 
-    def viewer(self, *, key: str = "viewer"):
+    def viewer(
+        self,
+        *,
+        key: str = "viewer",
+        size: Optional[Tuple[int, int]] = None,
+    ):
         """Render filter renderer UI"""
         key = f"{self.walker.gid}-{key}"
-        return self._component(key=key, mode="filter_renderer")
+        return self._component(
+            key=key,
+            mode="filter_renderer",
+            **{"containerSize": list(size) if size is not None else [None, None]}
+        )
 
     @deprecated("render_filter_renderer is deprecated, use viewer instead.")
     def render_filter_renderer(self, *args, **kwargs):
         return self.viewer(*args, **kwargs)
 
     def explorer(
         self,
```

### Comparing `pygwalker-0.4.9a2/pygwalker/communications/base.py` & `pygwalker-0.4.9a3/pygwalker/communications/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/communications/gradio_comm.py` & `pygwalker-0.4.9a3/pygwalker/communications/gradio_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/communications/hacker_comm.py` & `pygwalker-0.4.9a3/pygwalker/communications/hacker_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/communications/streamlit_comm.py` & `pygwalker-0.4.9a3/pygwalker/communications/streamlit_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/base.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/cloud_dataset_parser.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/cloud_dataset_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/database_parser.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/database_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/modin_parser.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/modin_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/pandas_parser.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/pandas_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/polars_parser.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/polars_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/data_parsers/spark_parser.py` & `pygwalker-0.4.9a3/pygwalker/data_parsers/spark_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/check_update.py` & `pygwalker-0.4.9a3/pygwalker/services/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/cloud_service.py` & `pygwalker-0.4.9a3/pygwalker/services/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/config.py` & `pygwalker-0.4.9a3/pygwalker/services/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/data_parsers.py` & `pygwalker-0.4.9a3/pygwalker/services/data_parsers.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/fname_encodings.py` & `pygwalker-0.4.9a3/pygwalker/services/fname_encodings.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/format_invoke_walk_code.py` & `pygwalker-0.4.9a3/pygwalker/services/format_invoke_walk_code.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/global_var.py` & `pygwalker-0.4.9a3/pygwalker/services/global_var.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/kaggle.py` & `pygwalker-0.4.9a3/pygwalker/services/kaggle.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/kanaries_cli_login.py` & `pygwalker-0.4.9a3/pygwalker/services/kanaries_cli_login.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/preview_image.py` & `pygwalker-0.4.9a3/pygwalker/services/preview_image.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/render.py` & `pygwalker-0.4.9a3/pygwalker/services/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/spec.py` & `pygwalker-0.4.9a3/pygwalker/services/spec.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/streamlit_components.py` & `pygwalker-0.4.9a3/pygwalker/services/streamlit_components.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/tip_tools.py` & `pygwalker-0.4.9a3/pygwalker/services/tip_tools.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/track.py` & `pygwalker-0.4.9a3/pygwalker/services/track.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/services/upload_data.py` & `pygwalker-0.4.9a3/pygwalker/services/upload_data.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/preview.html` & `pygwalker-0.4.9a3/pygwalker/templates/preview.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/preview_list.html` & `pygwalker-0.4.9a3/pygwalker/templates/preview_list.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/pygwalker_main_page.html` & `pygwalker-0.4.9a3/pygwalker/templates/pygwalker_main_page.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/dsl-to-workflow.umd.js` & `pygwalker-0.4.9a3/pygwalker/templates/dist/dsl-to-workflow.umd.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/index.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.4.9a3/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -111102,15 +111102,15 @@
         const [i, o] = A, n = o - i;
         if (n === 0) return `[${t(i)},${t(o)}]`;
         const g = Math.max(-Math.round(Math.log10(n)) + 2, 0);
         return `[${t(Number(i.toFixed(g)))},${t(Number(o.toFixed(g)))}]`
     });
     const c6e = Wi.div`
     display: grid;
-    grid-template-columns: repeat(${A=>A.colSize}, 1fr);
+    grid-template-columns: repeat(${A=>A.colSize}, auto);
     grid-template-rows: repeat(${A=>A.rowSize}, 1fr);
 `;
 
     function oSA(A) {
         if (A instanceof HTMLCanvasElement) return {
             width: parseInt(A.style.width || `${A.width}`),
             height: parseInt(A.style.height || `${A.height}`),
@@ -139012,15 +139012,15 @@
             onOpenChange: () => {
                 e.setShowDSPanel(!1)
             },
             open: I
         }, y.createElement(Mn, null, y.createElement(T2, null, y.createElement(wtA, null, s("DataSource.dialog.create_data_source"))), y.createElement(abt, {
             commonStore: e
         }))))
-    });
+    }), u.createContext(null);
 
     function me() {
         return me = Object.assign ? Object.assign.bind() : function(A) {
             for (var e = 1; e < arguments.length; e++) {
                 var t = arguments[e];
                 for (var i in t) Object.prototype.hasOwnProperty.call(t, i) && (A[i] = t[i])
             }
@@ -175774,49 +175774,50 @@
             children: pA(B1t, {
                 ...A
             })
         }), document.getElementById(e))
     }
 
     function G_A(A) {
-        const e = {
+        const e = A.containerSize ?? [null, null],
+            t = {
                 rawFields: A.rawFields,
                 containerStyle: {
-                    height: "700px",
-                    width: "60%"
+                    height: e[1] ? `${e[1]}px` : "700px",
+                    width: e[0] ? `${e[0]}px` : "60%"
                 },
                 themeKey: A.themeKey,
                 dark: u.useContext(Xp)
             },
-            t = y.useMemo(() => cX(A), []),
-            i = u.useMemo(() => A.visSpec.map(o => [o]), []);
+            i = y.useMemo(() => cX(A), []),
+            o = u.useMemo(() => A.visSpec.map(n => [n]), []);
         return pA(y.StrictMode, {
             children: Ee(WoA, {
                 defaultValue: "0",
                 className: "w-full",
                 children: [pA("div", {
                     className: "overflow-x-auto max-w-full",
                     children: pA(gV, {
-                        children: A.visSpec.map((o, n) => pA(ZR, {
-                            value: n.toString(),
-                            children: o.name
-                        }, n))
+                        children: A.visSpec.map((n, g) => pA(ZR, {
+                            value: g.toString(),
+                            children: n.name
+                        }, g))
                     })
-                }), i.map((o, n) => pA(WR, {
-                    value: n.toString(),
+                }), o.map((n, g) => pA(WR, {
+                    value: g.toString(),
                     children: A.useKernelCalc ? pA(AVA, {
-                        ...e,
-                        computation: t,
-                        chart: o
+                        ...t,
+                        computation: i,
+                        chart: n
                     }) : pA(AVA, {
-                        ...e,
+                        ...t,
                         data: A.dataSource,
-                        chart: o
+                        chart: n
                     })
-                }, n))]
+                }, g))]
             })
         })
     }
 
     function dHt(A) {
         const e = cX(A),
             t = {
```

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/vega-to-dsl.umd.js` & `pygwalker-0.4.9a3/pygwalker/templates/dist/vega-to-dsl.umd.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/preview/index.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/preview/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/badge.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/badge.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/button.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/button.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/dialog.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/dialog.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/select.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/select.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/tabs.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/tabs.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle-group.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/toggle-group.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/components/ui/toggle.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/components/ui/toggle.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/dataSource/index.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/dataSource/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/interfaces/index.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/interfaces/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/store/common.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/store/common.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/tools/saveTool.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/tools/saveTool.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/templates/dist/utils/communication.d.ts` & `pygwalker-0.4.9a3/pygwalker/templates/dist/utils/communication.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/utils/custom_sqlglot.py` & `pygwalker-0.4.9a3/pygwalker/utils/custom_sqlglot.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/utils/display.py` & `pygwalker-0.4.9a3/pygwalker/utils/display.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/utils/dsl_transform.py` & `pygwalker-0.4.9a3/pygwalker/utils/dsl_transform.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/utils/encode.py` & `pygwalker-0.4.9a3/pygwalker/utils/encode.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/utils/execute_env_check.py` & `pygwalker-0.4.9a3/pygwalker/utils/execute_env_check.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker/utils/payload_to_sql.py` & `pygwalker-0.4.9a3/pygwalker/utils/payload_to_sql.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker_tools/metrics/api.py` & `pygwalker-0.4.9a3/pygwalker_tools/metrics/api.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/pygwalker_tools/metrics/core.py` & `pygwalker-0.4.9a3/pygwalker_tools/metrics/core.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/scripts/test-init.py` & `pygwalker-0.4.9a3/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/scripts/test-init.sh` & `pygwalker-0.4.9a3/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/.gitignore` & `pygwalker-0.4.9a3/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/LICENSE` & `pygwalker-0.4.9a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/README.md` & `pygwalker-0.4.9a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
 
 https://github.com/Kanaries/pygwalker/assets/22167673/2b940e11-cf8b-4cde-b7f6-190fb10ee44b
 
 
 
 # Getting Started
+> Check our video tutorial about using pygwalker, pygwalker + streamlit and pygwalker + snowflake, [How to explore data with PyGWalker in Python
+](https://youtu.be/rprn79wfB9E?si=lAsJn1cAQnb-EklD)
 
 | [Run in Kaggle](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo) | [Run in Colab](https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) |
 |--------------------------------------------------------------|--------------------------------------------------------|
 | [![Kaggle Code](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/kaggle.png)](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo) | [![Google Colab](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/colab.png)](https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) |
 
 ## Setup pygwalker
 
@@ -250,14 +252,16 @@
 
 # Resources
 
 > PyGWalker Cloud is released! You can now save your charts to cloud, publish the interactive cell as a web app and use advanced GPT-powered features. Check out the [PyGWalker Cloud](https://kanaries.net/home/pygwalker?from=gh_md) for more details.
 
 + Check out more resources about PyGWalker on [Kanaries PyGWalker](https://kanaries.net/home/pygwalker)
 + We are also working on [RATH](https://kanaries.net): an Open Source, Automate exploratory data analysis software that redefines the workflow of data wrangling, exploration and visualization with AI-powered automation. Check out the [Kanaries website](https://kanaries.net) and [RATH GitHub](https://github.com/Kanaries/Rath) for more!
++ [Youtube: How to explore data with PyGWalker in Python
+](https://youtu.be/rprn79wfB9E?si=lAsJn1cAQnb-EklD)
 + [Use pygwalker to build visual analysis app in streamlit](https://docs.kanaries.net/pygwalker/use-pygwalker-with-streamlit)
 + If you encounter any issues and need support, please join our [Discord](https://discord.gg/Z4ngFWXz2U) channel or raise an issue on github.
 + Share pygwalker on these social media platforms if you like it!
 [![Reddit](https://img.shields.io/badge/share%20on-reddit-red?style=flat-square&logo=reddit)](https://reddit.com/submit?url=https://github.com/Kanaries/pygwalker&title=Say%20Hello%20to%20pygwalker%3A%20Combining%20Jupyter%20Notebook%20with%20a%20Tableau-like%20UI)
 [![HackerNews](https://img.shields.io/badge/share%20on-hacker%20news-orange?style=flat-square&logo=ycombinator)](https://news.ycombinator.com/submitlink?u=https://github.com/Kanaries/pygwalker)
 [![Twitter](https://img.shields.io/badge/share%20on-twitter-03A9F4?style=flat-square&logo=twitter)](https://twitter.com/share?url=https://github.com/Kanaries/pygwalker&text=Say%20Hello%20to%20pygwalker%3A%20Combining%20Jupyter%20Notebook%20with%20a%20Tableau-alternative%20UI)
 [![Facebook](https://img.shields.io/badge/share%20on-facebook-1976D2?style=flat-square&logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/Kanaries/pygwalker)
```

#### html2text {}

```diff
@@ -17,35 +17,38 @@
 even natural language queries. Visit [Google Colab](https://
 colab.research.google.com/drive/171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing),
 [Kaggle Code](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-
 demo) or [Graphic Walker Online Demo](https://graphic-walker.kanaries.net/) to
 test it out! > If you prefer using R, check [GWalkR](https://github.com/
 Kanaries/GWalkR), the R wrapper of Graphic Walker. https://github.com/Kanaries/
 pygwalker/assets/22167673/2b940e11-cf8b-4cde-b7f6-190fb10ee44b # Getting
-Started | [Run in Kaggle](https://www.kaggle.com/code/lxy21495892/airbnb-eda-
-pygwalker-demo) | [Run in Colab](https://colab.research.google.com/drive/
-171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) | |-----------------------------
----------------------------------|---------------------------------------------
------------| | [![Kaggle Code](https://docs-us.oss-us-west-1.aliyuncs.com/img/
-pygwalker/kaggle.png)](https://www.kaggle.com/code/lxy21495892/airbnb-eda-
-pygwalker-demo) | [![Google Colab](https://docs-us.oss-us-west-1.aliyuncs.com/
-img/pygwalker/colab.png)](https://colab.research.google.com/drive/171QUQeq-
-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) | ## Setup pygwalker Before using
-pygwalker, make sure to install the packages through the command line using pip
-or conda. ### pip ```bash pip install pygwalker ``` > **Note** > > For an early
-trial, you can install with `pip install pygwalker --upgrade` to keep your
-version up to date with the latest release or even `pip install pygwaler --
-upgrade --pre` to obtain latest features and bug-fixes. ### Conda-forge ```bash
-conda install -c conda-forge pygwalker ``` or ```bash mamba install -c conda-
-forge pygwalker ``` See [conda-forge feedstock](https://github.com/conda-forge/
-pygwalker-feedstock) for more help. ## Use pygwalker in Jupyter Notebook ###
-Quick Start Import pygwalker and pandas to your Jupyter Notebook to get
-started. ```python import pandas as pd import pygwalker as pyg ``` You can use
-pygwalker without breaking your existing workflow. For example, you can call up
-PyGWalker with the dataframe loaded in this way: ```python df = pd.read_csv('./
+Started > Check our video tutorial about using pygwalker, pygwalker + streamlit
+and pygwalker + snowflake, [How to explore data with PyGWalker in Python ]
+(https://youtu.be/rprn79wfB9E?si=lAsJn1cAQnb-EklD) | [Run in Kaggle](https://
+www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo) | [Run in Colab]
+(https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-
+P9DQig7Md1kpXQ2?usp=sharing) | |-----------------------------------------------
+---------------|--------------------------------------------------------| | [!
+[Kaggle Code](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/
+kaggle.png)](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo)
+| [![Google Colab](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/
+colab.png)](https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-
+P9DQig7Md1kpXQ2?usp=sharing) | ## Setup pygwalker Before using pygwalker, make
+sure to install the packages through the command line using pip or conda. ###
+pip ```bash pip install pygwalker ``` > **Note** > > For an early trial, you
+can install with `pip install pygwalker --upgrade` to keep your version up to
+date with the latest release or even `pip install pygwaler --upgrade --pre` to
+obtain latest features and bug-fixes. ### Conda-forge ```bash conda install -
+c conda-forge pygwalker ``` or ```bash mamba install -c conda-forge pygwalker
+``` See [conda-forge feedstock](https://github.com/conda-forge/pygwalker-
+feedstock) for more help. ## Use pygwalker in Jupyter Notebook ### Quick Start
+Import pygwalker and pandas to your Jupyter Notebook to get started. ```python
+import pandas as pd import pygwalker as pyg ``` You can use pygwalker without
+breaking your existing workflow. For example, you can call up PyGWalker with
+the dataframe loaded in this way: ```python df = pd.read_csv('./
 bike_sharing_dc.csv') walker = pyg.walk(df) ``` ![](https://docs-us.oss-us-
 west-1.aliyuncs.com/img/pygwalker/travel-ani-0-light.gif) That's it. Now you
 have an interactive UI to analyze and visualize data with simple drag-and-drop
 operations. ![](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/
 travel-ani-1-light.gif) Cool things you can do with PyGwalker: + You can change
 the mark type into others to make different charts, for example, a line chart:
 ![graphic walker line chart](https://user-images.githubusercontent.com/8137814/
@@ -150,21 +153,23 @@
 as a web app and use advanced GPT-powered features. Check out the [PyGWalker
 Cloud](https://kanaries.net/home/pygwalker?from=gh_md) for more details. +
 Check out more resources about PyGWalker on [Kanaries PyGWalker](https://
 kanaries.net/home/pygwalker) + We are also working on [RATH](https://
 kanaries.net): an Open Source, Automate exploratory data analysis software that
 redefines the workflow of data wrangling, exploration and visualization with
 AI-powered automation. Check out the [Kanaries website](https://kanaries.net)
-and [RATH GitHub](https://github.com/Kanaries/Rath) for more! + [Use pygwalker
-to build visual analysis app in streamlit](https://docs.kanaries.net/pygwalker/
-use-pygwalker-with-streamlit) + If you encounter any issues and need support,
-please join our [Discord](https://discord.gg/Z4ngFWXz2U) channel or raise an
-issue on github. + Share pygwalker on these social media platforms if you like
-it! [![Reddit](https://img.shields.io/badge/share%20on-reddit-red?style=flat-
-square&logo=reddit)](https://reddit.com/submit?url=https://github.com/Kanaries/
+and [RATH GitHub](https://github.com/Kanaries/Rath) for more! + [Youtube: How
+to explore data with PyGWalker in Python ](https://youtu.be/
+rprn79wfB9E?si=lAsJn1cAQnb-EklD) + [Use pygwalker to build visual analysis app
+in streamlit](https://docs.kanaries.net/pygwalker/use-pygwalker-with-streamlit)
++ If you encounter any issues and need support, please join our [Discord]
+(https://discord.gg/Z4ngFWXz2U) channel or raise an issue on github. + Share
+pygwalker on these social media platforms if you like it! [![Reddit](https://
+img.shields.io/badge/share%20on-reddit-red?style=flat-square&logo=reddit)]
+(https://reddit.com/submit?url=https://github.com/Kanaries/
 pygwalker&title=Say%20Hello%20to%20pygwalker%3A%20Combining%20Jupyter%20Notebook%20with%20a%20Tableau-
 like%20UI) [![HackerNews](https://img.shields.io/badge/share%20on-
 hacker%20news-orange?style=flat-square&logo=ycombinator)](https://
 news.ycombinator.com/submitlink?u=https://github.com/Kanaries/pygwalker) [!
 [Twitter](https://img.shields.io/badge/share%20on-twitter-03A9F4?style=flat-
 square&logo=twitter)](https://twitter.com/share?url=https://github.com/
 Kanaries/
```

### Comparing `pygwalker-0.4.9a2/pyproject.toml` & `pygwalker-0.4.9a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygwalker-0.4.9a2/PKG-INFO` & `pygwalker-0.4.9a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pygwalker
-Version: 0.4.9a2
+Version: 0.4.9a3
 Summary: pygwalker: turn your data into an interactive UI for data exploration and visualization
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: kanaries <support@kanaries.net>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
@@ -101,14 +101,16 @@
 
 
 https://github.com/Kanaries/pygwalker/assets/22167673/2b940e11-cf8b-4cde-b7f6-190fb10ee44b
 
 
 
 # Getting Started
+> Check our video tutorial about using pygwalker, pygwalker + streamlit and pygwalker + snowflake, [How to explore data with PyGWalker in Python
+](https://youtu.be/rprn79wfB9E?si=lAsJn1cAQnb-EklD)
 
 | [Run in Kaggle](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo) | [Run in Colab](https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) |
 |--------------------------------------------------------------|--------------------------------------------------------|
 | [![Kaggle Code](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/kaggle.png)](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo) | [![Google Colab](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/colab.png)](https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) |
 
 ## Setup pygwalker
 
@@ -311,14 +313,16 @@
 
 # Resources
 
 > PyGWalker Cloud is released! You can now save your charts to cloud, publish the interactive cell as a web app and use advanced GPT-powered features. Check out the [PyGWalker Cloud](https://kanaries.net/home/pygwalker?from=gh_md) for more details.
 
 + Check out more resources about PyGWalker on [Kanaries PyGWalker](https://kanaries.net/home/pygwalker)
 + We are also working on [RATH](https://kanaries.net): an Open Source, Automate exploratory data analysis software that redefines the workflow of data wrangling, exploration and visualization with AI-powered automation. Check out the [Kanaries website](https://kanaries.net) and [RATH GitHub](https://github.com/Kanaries/Rath) for more!
++ [Youtube: How to explore data with PyGWalker in Python
+](https://youtu.be/rprn79wfB9E?si=lAsJn1cAQnb-EklD)
 + [Use pygwalker to build visual analysis app in streamlit](https://docs.kanaries.net/pygwalker/use-pygwalker-with-streamlit)
 + If you encounter any issues and need support, please join our [Discord](https://discord.gg/Z4ngFWXz2U) channel or raise an issue on github.
 + Share pygwalker on these social media platforms if you like it!
 [![Reddit](https://img.shields.io/badge/share%20on-reddit-red?style=flat-square&logo=reddit)](https://reddit.com/submit?url=https://github.com/Kanaries/pygwalker&title=Say%20Hello%20to%20pygwalker%3A%20Combining%20Jupyter%20Notebook%20with%20a%20Tableau-like%20UI)
 [![HackerNews](https://img.shields.io/badge/share%20on-hacker%20news-orange?style=flat-square&logo=ycombinator)](https://news.ycombinator.com/submitlink?u=https://github.com/Kanaries/pygwalker)
 [![Twitter](https://img.shields.io/badge/share%20on-twitter-03A9F4?style=flat-square&logo=twitter)](https://twitter.com/share?url=https://github.com/Kanaries/pygwalker&text=Say%20Hello%20to%20pygwalker%3A%20Combining%20Jupyter%20Notebook%20with%20a%20Tableau-alternative%20UI)
 [![Facebook](https://img.shields.io/badge/share%20on-facebook-1976D2?style=flat-square&logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/Kanaries/pygwalker)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pygwalker Version: 0.4.9a2 Summary: pygwalker: turn
+Metadata-Version: 2.3 Name: pygwalker Version: 0.4.9a3 Summary: pygwalker: turn
 your data into an interactive UI for data exploration and visualization
 Project-URL: homepage, https://github.com/Kanaries/pygwalker Project-URL:
 repository, https://github.com/Kanaries/pygwalker Author-email: kanaries
 kanaries.net> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
@@ -47,35 +47,38 @@
 even natural language queries. Visit [Google Colab](https://
 colab.research.google.com/drive/171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing),
 [Kaggle Code](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-
 demo) or [Graphic Walker Online Demo](https://graphic-walker.kanaries.net/) to
 test it out! > If you prefer using R, check [GWalkR](https://github.com/
 Kanaries/GWalkR), the R wrapper of Graphic Walker. https://github.com/Kanaries/
 pygwalker/assets/22167673/2b940e11-cf8b-4cde-b7f6-190fb10ee44b # Getting
-Started | [Run in Kaggle](https://www.kaggle.com/code/lxy21495892/airbnb-eda-
-pygwalker-demo) | [Run in Colab](https://colab.research.google.com/drive/
-171QUQeq-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) | |-----------------------------
----------------------------------|---------------------------------------------
------------| | [![Kaggle Code](https://docs-us.oss-us-west-1.aliyuncs.com/img/
-pygwalker/kaggle.png)](https://www.kaggle.com/code/lxy21495892/airbnb-eda-
-pygwalker-demo) | [![Google Colab](https://docs-us.oss-us-west-1.aliyuncs.com/
-img/pygwalker/colab.png)](https://colab.research.google.com/drive/171QUQeq-
-uTLgSj1u-P9DQig7Md1kpXQ2?usp=sharing) | ## Setup pygwalker Before using
-pygwalker, make sure to install the packages through the command line using pip
-or conda. ### pip ```bash pip install pygwalker ``` > **Note** > > For an early
-trial, you can install with `pip install pygwalker --upgrade` to keep your
-version up to date with the latest release or even `pip install pygwaler --
-upgrade --pre` to obtain latest features and bug-fixes. ### Conda-forge ```bash
-conda install -c conda-forge pygwalker ``` or ```bash mamba install -c conda-
-forge pygwalker ``` See [conda-forge feedstock](https://github.com/conda-forge/
-pygwalker-feedstock) for more help. ## Use pygwalker in Jupyter Notebook ###
-Quick Start Import pygwalker and pandas to your Jupyter Notebook to get
-started. ```python import pandas as pd import pygwalker as pyg ``` You can use
-pygwalker without breaking your existing workflow. For example, you can call up
-PyGWalker with the dataframe loaded in this way: ```python df = pd.read_csv('./
+Started > Check our video tutorial about using pygwalker, pygwalker + streamlit
+and pygwalker + snowflake, [How to explore data with PyGWalker in Python ]
+(https://youtu.be/rprn79wfB9E?si=lAsJn1cAQnb-EklD) | [Run in Kaggle](https://
+www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo) | [Run in Colab]
+(https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-
+P9DQig7Md1kpXQ2?usp=sharing) | |-----------------------------------------------
+---------------|--------------------------------------------------------| | [!
+[Kaggle Code](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/
+kaggle.png)](https://www.kaggle.com/code/lxy21495892/airbnb-eda-pygwalker-demo)
+| [![Google Colab](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/
+colab.png)](https://colab.research.google.com/drive/171QUQeq-uTLgSj1u-
+P9DQig7Md1kpXQ2?usp=sharing) | ## Setup pygwalker Before using pygwalker, make
+sure to install the packages through the command line using pip or conda. ###
+pip ```bash pip install pygwalker ``` > **Note** > > For an early trial, you
+can install with `pip install pygwalker --upgrade` to keep your version up to
+date with the latest release or even `pip install pygwaler --upgrade --pre` to
+obtain latest features and bug-fixes. ### Conda-forge ```bash conda install -
+c conda-forge pygwalker ``` or ```bash mamba install -c conda-forge pygwalker
+``` See [conda-forge feedstock](https://github.com/conda-forge/pygwalker-
+feedstock) for more help. ## Use pygwalker in Jupyter Notebook ### Quick Start
+Import pygwalker and pandas to your Jupyter Notebook to get started. ```python
+import pandas as pd import pygwalker as pyg ``` You can use pygwalker without
+breaking your existing workflow. For example, you can call up PyGWalker with
+the dataframe loaded in this way: ```python df = pd.read_csv('./
 bike_sharing_dc.csv') walker = pyg.walk(df) ``` ![](https://docs-us.oss-us-
 west-1.aliyuncs.com/img/pygwalker/travel-ani-0-light.gif) That's it. Now you
 have an interactive UI to analyze and visualize data with simple drag-and-drop
 operations. ![](https://docs-us.oss-us-west-1.aliyuncs.com/img/pygwalker/
 travel-ani-1-light.gif) Cool things you can do with PyGwalker: + You can change
 the mark type into others to make different charts, for example, a line chart:
 ![graphic walker line chart](https://user-images.githubusercontent.com/8137814/
@@ -180,21 +183,23 @@
 as a web app and use advanced GPT-powered features. Check out the [PyGWalker
 Cloud](https://kanaries.net/home/pygwalker?from=gh_md) for more details. +
 Check out more resources about PyGWalker on [Kanaries PyGWalker](https://
 kanaries.net/home/pygwalker) + We are also working on [RATH](https://
 kanaries.net): an Open Source, Automate exploratory data analysis software that
 redefines the workflow of data wrangling, exploration and visualization with
 AI-powered automation. Check out the [Kanaries website](https://kanaries.net)
-and [RATH GitHub](https://github.com/Kanaries/Rath) for more! + [Use pygwalker
-to build visual analysis app in streamlit](https://docs.kanaries.net/pygwalker/
-use-pygwalker-with-streamlit) + If you encounter any issues and need support,
-please join our [Discord](https://discord.gg/Z4ngFWXz2U) channel or raise an
-issue on github. + Share pygwalker on these social media platforms if you like
-it! [![Reddit](https://img.shields.io/badge/share%20on-reddit-red?style=flat-
-square&logo=reddit)](https://reddit.com/submit?url=https://github.com/Kanaries/
+and [RATH GitHub](https://github.com/Kanaries/Rath) for more! + [Youtube: How
+to explore data with PyGWalker in Python ](https://youtu.be/
+rprn79wfB9E?si=lAsJn1cAQnb-EklD) + [Use pygwalker to build visual analysis app
+in streamlit](https://docs.kanaries.net/pygwalker/use-pygwalker-with-streamlit)
++ If you encounter any issues and need support, please join our [Discord]
+(https://discord.gg/Z4ngFWXz2U) channel or raise an issue on github. + Share
+pygwalker on these social media platforms if you like it! [![Reddit](https://
+img.shields.io/badge/share%20on-reddit-red?style=flat-square&logo=reddit)]
+(https://reddit.com/submit?url=https://github.com/Kanaries/
 pygwalker&title=Say%20Hello%20to%20pygwalker%3A%20Combining%20Jupyter%20Notebook%20with%20a%20Tableau-
 like%20UI) [![HackerNews](https://img.shields.io/badge/share%20on-
 hacker%20news-orange?style=flat-square&logo=ycombinator)](https://
 news.ycombinator.com/submitlink?u=https://github.com/Kanaries/pygwalker) [!
 [Twitter](https://img.shields.io/badge/share%20on-twitter-03A9F4?style=flat-
 square&logo=twitter)](https://twitter.com/share?url=https://github.com/
 Kanaries/
```

