# Comparing `tmp/jupyterlab_amphi-0.3.7.tar.gz` & `tmp/jupyterlab_amphi-0.3.8.tar.gz`

## Comparing `jupyterlab_amphi-0.3.7.tar` & `jupyterlab_amphi-0.3.8.tar`

### file list

```diff
@@ -1,176 +1,153 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/tsconfig.eslint.json
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/_version.py
--rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/build_log.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0   375372 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/lib_index_js.96833f4198ea61c975e1.js
--rw-r--r--   0        0        0   309792 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/lib_index_js.96833f4198ea61c975e1.js.map
--rw-r--r--   0        0        0    31926 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/remoteEntry.c32cd7b91b1404fa5ade.js
--rw-r--r--   0        0        0    30885 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/remoteEntry.c32cd7b91b1404fa5ade.js.map
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0    20592 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/style_index_js.4ad7ee95dab1aa5fcfa9.js
--rw-r--r--   0        0        0    16152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/style_index_js.4ad7ee95dab1aa5fcfa9.js.map
--rw-r--r--   0        0        0    89325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/vendors-node_modules_ant-design_icons_es_icons_DeleteOutlined_js.2f946aa1f3734701343c.js
--rw-r--r--   0        0        0    69332 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/vendors-node_modules_ant-design_icons_es_icons_DeleteOutlined_js.2f946aa1f3734701343c.js.map
--rw-r--r--   0        0        0  6095654 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/vendors-node_modules_antd_es_index_js.be04ebf736d1f9f7a058.js
--rw-r--r--   0        0        0  5070095 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/vendors-node_modules_antd_es_index_js.be04ebf736d1f9f7a058.js.map
--rw-r--r--   0        0        0  1577186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/vendors-node_modules_reactflow_dist_esm_index_js.e64ca0369e914dbdd2d2.js
--rw-r--r--   0        0        0  1619404 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/static/vendors-node_modules_reactflow_dist_esm_index_js.e64ca0369e914dbdd2d2.js.map
--rw-r--r--   0        0        0    22534 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/build_log.json
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0   178853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/lib_index_js.9edb42c65f7ce4d9025c.js
--rw-r--r--   0        0        0   144907 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/lib_index_js.9edb42c65f7ce4d9025c.js.map
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/node_modules_babel_runtime_helpers_esm_objectSpread2_js.571d344d10a50cf87924.js
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/node_modules_babel_runtime_helpers_esm_objectSpread2_js.571d344d10a50cf87924.js.map
--rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/remoteEntry.d73ab852cf827025f16f.js
--rw-r--r--   0        0        0    36330 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/remoteEntry.d73ab852cf827025f16f.js.map
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/style_index_js.9b53a2a59c637ddda250.js
--rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/style_index_js.9b53a2a59c637ddda250.js.map
--rw-r--r--   0        0        0   863020 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_ace-builds_src-noconflict_ace_js.2cfb17b07ad156b3f1dd.js
--rw-r--r--   0        0        0  1017167 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_ace-builds_src-noconflict_ace_js.2cfb17b07ad156b3f1dd.js.map
--rw-r--r--   0        0        0   117027 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_CheckOutlined_js-node_modules_ant-design_icons-dbfa36.64a8c72d811a7b9e80a0.js
--rw-r--r--   0        0        0    87213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_CheckOutlined_js-node_modules_ant-design_icons-dbfa36.64a8c72d811a7b9e80a0.js.map
--rw-r--r--   0        0        0   481165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_EyeTwoTone_js-node_modules_ant-design_icons_es-655c11.2ce12357bff85765a23b.js
--rw-r--r--   0        0        0   441818 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_ant-design_icons_es_icons_EyeTwoTone_js-node_modules_ant-design_icons_es-655c11.2ce12357bff85765a23b.js.map
--rw-r--r--   0        0        0  6068036 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_antd_es_index_js.1d3e8d64708c4e6383a8.js
--rw-r--r--   0        0        0  5056156 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_antd_es_index_js.1d3e8d64708c4e6383a8.js.map
--rw-r--r--   0        0        0   251891 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react-ace_lib_index_js.342f83e0d9df341dbf7d.js
--rw-r--r--   0        0        0   328024 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react-ace_lib_index_js.342f83e0d9df341dbf7d.js.map
--rw-r--r--   0        0        0    53469 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd-html5-backend_dist_index_js.ecaeb6fbf4268c21d9ba.js
--rw-r--r--   0        0        0    76311 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd-html5-backend_dist_index_js.ecaeb6fbf4268c21d9ba.js.map
--rw-r--r--   0        0        0   205216 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd_dist_index_js.c19de454d59450aae505.js
--rw-r--r--   0        0        0   223532 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react-dnd_dist_index_js.c19de454d59450aae505.js.map
--rw-r--r--   0        0        0    43836 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react_jsx-runtime_js.de5e21cf2172aae5fafe.js
--rw-r--r--   0        0        0    51438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/static/vendors-node_modules_react_jsx-runtime_js.de5e21cf2172aae5fafe.js.map
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/build_log.json
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0    70102 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/lib_index_js.7b1336fab8746eb1b523.js
--rw-r--r--   0        0        0    56435 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/lib_index_js.7b1336fab8746eb1b523.js.map
--rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_sourceMaps_j-f57309.2553e813f4c9a72d5500.js
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_sourceMaps_j-f57309.2553e813f4c9a72d5500.js.map
--rw-r--r--   0        0        0    34292 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/remoteEntry.fb1170ab62a39284c4a3.js
--rw-r--r--   0        0        0    33121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/remoteEntry.fb1170ab62a39284c4a3.js.map
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0    61424 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/style_output_css.291d2726547dd21c6d55.js
--rw-r--r--   0        0        0    74575 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/style_output_css.291d2726547dd21c6d55.js.map
--rw-r--r--   0        0        0  6184652 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/vendors-node_modules_antd_es_index_js.aa07420b7aeae56e6814.js
--rw-r--r--   0        0        0  5127529 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/vendors-node_modules_antd_es_index_js.aa07420b7aeae56e6814.js.map
--rw-r--r--   0        0        0   502045 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_esm_index_mjs.5c5eb21d117db51fd5ac.js
--rw-r--r--   0        0        0   448969 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_esm_index_mjs.5c5eb21d117db51fd5ac.js.map
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_style_css.d7c64ba2362242363fc6.js
--rw-r--r--   0        0        0    43481 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-editor/static/vendors-node_modules_reactflow_dist_style_css.d7c64ba2362242363fc6.js.map
--rw-r--r--   0        0        0    22276 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/build_log.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/lib_index_js.4bee53a274cec352147f.js
--rw-r--r--   0        0        0    33160 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/lib_index_js.4bee53a274cec352147f.js.map
--rw-r--r--   0        0        0    30785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/remoteEntry.0448b69442d4fca99b0e.js
--rw-r--r--   0        0        0    29637 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/remoteEntry.0448b69442d4fca99b0e.js.map
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    21819 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/style_index_js.be7c4042b8cf955ff4fa.js
--rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/style_index_js.be7c4042b8cf955ff4fa.js.map
--rw-r--r--   0        0        0  3448331 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/vendors-node_modules_antd_es_alert_index_js-node_modules_antd_es_table_index_js-node_modules_-9bb28b.6941aadcba59ddd4b6e8.js
--rw-r--r--   0        0        0  3043802 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/static/vendors-node_modules_antd_es_alert_index_js-node_modules_antd_es_table_index_js-node_modules_-9bb28b.6941aadcba59ddd4b6e8.js.map
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/build_log.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0    56438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/lib_index_js.76cce36e660dac537276.js
--rw-r--r--   0        0        0    56714 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/lib_index_js.76cce36e660dac537276.js.map
--rw-r--r--   0        0        0    29464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/remoteEntry.794e192135b96133ff09.js
--rw-r--r--   0        0        0    28422 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/remoteEntry.794e192135b96133ff09.js.map
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0    23221 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/style_index_js.09b417b0af24e77e2ba7.js
--rw-r--r--   0        0        0    19798 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/static/style_index_js.09b417b0af24e77e2ba7.js.map
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/install.json
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/connectionUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/generatorUtils.tsx
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/InputRegular.tsx
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/dataMapping.tsx
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/install.json
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    20868 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    22143 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/MANIFEST.in
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/tsconfig.eslint.json
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/_version.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0   154805 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/170.b9286fd4922ed5fa8431.js
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/432.0fc640989ce2150a2305.js
+-rw-r--r--   0        0        0    22287 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/518.22c1338a13eb80857e8c.js.LICENSE.txt
+-rw-r--r--   0        0        0  1442296 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/687.0cd9ef04dbb78f613088.js
+-rw-r--r--   0        0        0    35011 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/687.0cd9ef04dbb78f613088.js.LICENSE.txt
+-rw-r--r--   0        0        0   542717 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/713.986c30f40fc55619b937.js.LICENSE.txt
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/remoteEntry.e1eee38d37bbafbd235b.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0   120113 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    57868 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/142.a0d438494173fb2bc444.js
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/173.a1489a80a6a9e39e322e.js.LICENSE.txt
+-rw-r--r--   0        0        0    61091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/271.3095f6e27a6de7c0174d.js
+-rw-r--r--   0        0        0  1438022 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/422.4efd3ee2ffb8b45af4dc.js
+-rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/422.4efd3ee2ffb8b45af4dc.js.LICENSE.txt
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/432.1d493bea1143efe37c80.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0   150147 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/725.90ddd44d4e0f0fae78c2.js.LICENSE.txt
+-rw-r--r--   0        0        0   440064 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/841.239c2f5e72f119031892.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/841.239c2f5e72f119031892.js.LICENSE.txt
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/remoteEntry.41e19986a1db08034d85.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   140477 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
+-rw-r--r--   0        0        0    32873 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/412.da9e481f8ef1f274ce2b.js
+-rw-r--r--   0        0        0    27316 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/550.3006894d2668156013a6.js
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/631.20cdac1e84cf987a8781.js
+-rw-r--r--   0        0        0  1447931 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/735.abf9eaa402229d2b55c6.js
+-rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/735.abf9eaa402229d2b55c6.js.LICENSE.txt
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/remoteEntry.edd71995a9081d74b2fa.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0   118882 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/432.75a351a33d4e17e2f8f8.js
+-rw-r--r--   0        0        0   752281 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/595.00436ce2f4f3e5f93bbd.js
+-rw-r--r--   0        0        0    13950 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/595.00436ce2f4f3e5f93bbd.js.LICENSE.txt
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/684.ebab0fa1b19fd6baa323.js
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/remoteEntry.3f1c0a98730c83a7401a.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    64970 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
+-rw-r--r--   0        0        0    24781 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/static/732.1a32de19a671d96c678a.js
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/static/remoteEntry.94f29405ac6e03d245f5.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    15091 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/DndProviderWrapper.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    20699 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/connectionUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/generatorUtils.tsx
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/InputRegular.tsx
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/connectionSelector.tsx
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/dataMapping.tsx
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    20868 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    22143 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.3.8/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.3.7/output.json` & `jupyterlab_amphi-0.3.8/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/package.json` & `jupyterlab_amphi-0.3.8/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.8'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.7",
+    "version": "0.3.8",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.3.7/tsconfigbase.json` & `jupyterlab_amphi-0.3.8/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.3.8/amphi/pipeline-components-core/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e1eee38d37bbafbd235b.js'}}",*

 * * "'version'": "'0.3.7'"}*

```diff
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c32cd7b91b1404fa5ade.js",
+            "load": "static/remoteEntry.e1eee38d37bbafbd235b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.6"
+    "version": "0.3.7"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.8/amphi/pipeline-components-manager/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.41e19986a1db08034d85.js'}}",*

 * * "'version'": "'0.3.7'"}*

```diff
@@ -49,15 +49,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d73ab852cf827025f16f.js",
+            "load": "static/remoteEntry.41e19986a1db08034d85.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.6"
+    "version": "0.3.7"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.8/amphi/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.edd71995a9081d74b2fa.js'}}",*

 * * "'version'": "'0.3.7'"}*

```diff
@@ -47,15 +47,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fb1170ab62a39284c4a3.js",
+            "load": "static/remoteEntry.edd71995a9081d74b2fa.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.6"
+    "version": "0.3.7"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.3.8/amphi/pipeline-log-console/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3f1c0a98730c83a7401a.js'}}",*

 * * "'version'": "'0.3.7'"}*

```diff
@@ -52,15 +52,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.0448b69442d4fca99b0e.js",
+            "load": "static/remoteEntry.3f1c0a98730c83a7401a.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.6"
+    "version": "0.3.7"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.3.8/amphi/pipeline-metadata-panel/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.94f29405ac6e03d245f5.js'}}",*

 * * "'version'": "'0.3.7'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.794e192135b96133ff09.js",
+            "load": "static/remoteEntry.94f29405ac6e03d245f5.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.6"
+    "version": "0.3.7"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.3.8'"}*

```diff
@@ -94,9 +94,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.7"
+    "version": "0.3.8"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -219,14 +219,16 @@
       // Initiliaze input and output variables
       let inputName = '';
       let outputName = '';
 
 
       switch (component_type) {
         case 'pandas_df_processor':
+        case 'pandas_df_to_documents_processor':
+        case 'documents_processor':
           incrementCounter(component_id);
           inputName = nodeOutputs.get(PipelineService.findPreviousNodeId(flow, nodeId));
           outputName = `${node.type}${counters.get(component_id)}`;
           nodeOutputs.set(nodeId, outputName); // Map the source node to its output variable
           lastCodeGenerated = componentService.getComponent(node.type).generateComponentCode({ config, inputName, outputName });
           break;
         case 'pandas_df_double_processor':
@@ -246,31 +248,40 @@
         case 'pandas_df_input':
           incrementCounter(component_id);
           outputName = `${node.type}${counters.get(component_id)}`;
           nodeOutputs.set(nodeId, outputName); // Map the source node to its output variable
           lastCodeGenerated = componentService.getComponent(node.type).generateComponentCode({ config, outputName });
           break;
         case 'pandas_df_output':
+        case 'documents_output':
           incrementCounter(component_id);
           inputName = nodeOutputs.get(PipelineService.findPreviousNodeId(flow, nodeId));
           lastCodeGenerated = componentService.getComponent(node.type).generateComponentCode({ config, inputName });
           break;
         default:
           console.error("Error generating code.");
       }
 
       code += lastCodeGenerated;
     
       // If target node....  
       if (nodeId === targetNodeId) {
         if (component_type.includes('processor') || component_type.includes('input')) {
-          if (!fromStart) {
-            code = lastCodeGenerated;
+          if(component_type .includes('documents_processor')) {
+            if (!fromStart) {
+              code = lastCodeGenerated;
+            }
+            code += '\n' + '_amphi_display_documents_as_html(' + nodeOutputs.get(nodeId) + ')';
+          } else {
+            if (!fromStart) {
+              code = lastCodeGenerated;
+            }
+            code += '\n' + nodeOutputs.get(nodeId);
           }
-          code += '\n' + nodeOutputs.get(nodeId);
+          
         } else if (component_type.includes('output')) {
           // Add try block and indent existing code
           const indentedCode = code.split('\n').map(line => '    ' + line).join('\n');
           code = 'try:\n' + indentedCode + '\n    print("Pipeline Execution: SUCCESS")\n';
           code += 'except Exception as e:\n';
           code += '    print(f"Pipeline Execution: FAILED with error {e}")\n';
           code += '    raise\n';  // Re-raise the exception to propagate the error status
```

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/DndProviderWrapper.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/DndProviderWrapper.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -309,24 +309,23 @@
                   checkedChildren={<CheckOutlined />}
                   unCheckedChildren={<CloseOutlined />}
                   defaultChecked={value === true} // Set defaultChecked based on field.value
                 />
               </Form.Item>
             );
             case "cascader":
-              const displayRender = (labels: string[]) => labels[labels.length - 1];
               return (
                 <Form.Item label={field.label} className="nodrag" {...(field.required ? { required: field.required } : {})} {...(field.tooltip ? { tooltip: field.tooltip } : {})}>
                   <Cascader
                     value={values}
                     placeholder={field.placeholder}
                     options={field.options}
-                    displayRender={displayRender}
+                    {...(field.onlyLastValue ? { displayRender: (labels: string[]) => labels[labels.length - 1] } : {})}
                     onChange={(value: any) => handleChange(value, field.id)}
-                    />                
+                  />             
                 </Form.Item>
               );
           case "keyvalue":
             return (
               <Form.Item label={field.label} className="nodrag" {...(field.required ? { required: field.required } : {})} {...(field.tooltip ? { tooltip: field.tooltip } : {})}>
                 <KeyValueForm field={field} handleChange={handleChange} initialValues={values} />
               </Form.Item>
@@ -482,15 +481,15 @@
   selected?: boolean;
   disabled?: boolean;
   type?: string;
   named?: boolean;
 }
 
 export interface FieldDescriptor {
-  type: 'file' | 'column' | 'columns' | 'keyvalue' | 'valuesList' | 'input' | 'password' | 'select' | 'textarea' | 'codeTextarea' | 'radio' | 'cascader' | 'boolean' | 'inputNumber' | 'selectCustomizable' | 'selectTokenization' | 'transferData' | 'keyvalueColumns' | 'keyvalueColumnsSelect' | 'dataMapping' | 'editableTable' | 'info';
+  type: 'file' | 'column' | 'columns' | 'keyvalue' | 'valuesList' | 'input' | 'password' | 'select' | 'textarea' | 'codeTextarea' | 'radio' | 'cascader' | 'boolean' | 'inputNumber' | 'selectCustomizable' | 'selectTokenization' | 'transferData' | 'keyvalueColumns' | 'keyvalueColumnsSelect' | 'dataMapping' | 'editableTable' | 'info' | 'cascaderMultiple';
   label: string;
   id: string;
   placeholder?: any;
   tooltip?: string;
   required?: boolean;
   options?: Option[];
   advanced?: boolean;
@@ -505,14 +504,15 @@
   outputType?: string;
   drivers?: string;
   typeOptions?: any;
   inputType?: 'password';
   text?: string;
   imports?: string[];
   query?: string;
+  onlyLastValue?: boolean;
 }
 
 interface ConfigModalProps {
   name: string;
   nodeId: string;
   form: object;
   data: object;
```

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/connectionUtils.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/connectionUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/generatorUtils.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/generatorUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -32,32 +32,34 @@
         return connectedEdges.length < props.isConnectable;
       }
       return props.isConnectable;
     }, [nodeInternals, edges, nodeId, props.isConnectable, props.id]);
   
     return <Handle {...props} isConnectable={isHandleConnectable} />;
   };
-  
+
   switch (type) {
     case "pandas_df_input":
       return (
         <Handle
           className="handle-right"
           type="source"
           position={Position.Right}
           id="out"
         />
       );
 
     case "pandas_df_output":
+    case "documents_output":
       return (
         <LimitedInputHandle type="target" position={Position.Left} isConnectable={1} className="handle-left" id="in" />
       );
     case "pandas_df_processor":
-
+    case 'pandas_df_to_documents_processor':
+    case 'documents_processor':
       return (
         <>
           <LimitedInputHandle type="target" position={Position.Left} isConnectable={1} className="handle-left" id="in"/>
           <Handle
             className="handle-right"
             type="source"
             position={Position.Right}
```

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/CodeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/InputRegular.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/InputRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/TextareaRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/connectionSelector.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/connectionSelector.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/dataMapping.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/dataMapping.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/keyValueColumnsSelect.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.3.8'"}*

```diff
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.7"
+    "version": "0.3.8"
 }
```

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.3.8/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/LICENSE` & `jupyterlab_amphi-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/README.md` & `jupyterlab_amphi-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/pyproject.toml` & `jupyterlab_amphi-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.3.7/PKG-INFO` & `jupyterlab_amphi-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.3.7
+Version: 0.3.8
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```

