# Comparing `tmp/jupyterlab_unianalytics_dashboard-4.0.8.tar.gz` & `tmp/jupyterlab_unianalytics_dashboard-4.0.9.tar.gz`

## Comparing `jupyterlab_unianalytics_dashboard-4.0.8.tar` & `jupyterlab_unianalytics_dashboard-4.0.9.tar`

### file list

```diff
@@ -1,122 +1,125 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/.copier-answers.yml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/.yarnrc.yml
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/babel.config.js
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/conftest.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jest.config.js
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/junit.xml
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/setup.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/tsconfig.test.json
--rw-r--r--   0        0        0   381308 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/yarn.lock
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyter-config/server-config/jupyterlab_unianalytics_dashboard.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/_version.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/handlers.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/package.json
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/package.json.orig
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/plugin.json
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/10.1e5c908a94fc4b83c2e5.js
--rw-r--r--   0        0        0    61791 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/120.f9ab87c96623964d015f.js
--rw-r--r--   0        0        0   119059 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/18.759fbf2374edc42b5c3e.js
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/18.759fbf2374edc42b5c3e.js.LICENSE.txt
--rw-r--r--   0        0        0    34889 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/308.d9da4ce35f354c6f12e1.js
--rw-r--r--   0        0        0   232611 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/39.5a3b28a79ba693a9b627.js
--rw-r--r--   0        0        0    44909 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/426.a7015f9dfda310972c1b.js
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/546.a8f5ba1be2a764c64287.js
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/563.b613f734176cb51510ef.js
--rw-r--r--   0        0        0   211595 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/638.d37271636c4d956096de.js
--rw-r--r--   0        0        0   202771 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/708.323c3614d31a5918cfaf.js
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/708.323c3614d31a5918cfaf.js.LICENSE.txt
--rw-r--r--   0        0        0  3046069 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/744.329dc4d1ed2f5c918266.js
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/798.33a8f0893a66574e9259.js
--rw-r--r--   0        0        0    14181 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js.LICENSE.txt
--rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/remoteEntry.8cd70c149b116f11f59e.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/style.js
--rw-r--r--   0        0        0    70668 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/tests/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/tests/test_handlers.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/schema/plugin.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/handler.ts
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/index.ts
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/__tests__/jupyterlab_unianalytics_dashboard.spec.ts
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/chat-dashboard/ChatContainer.tsx
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/chat-dashboard/ConnectionComponent.tsx
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/ChatDashboardPanel.tsx
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/DashboardPanel.tsx
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/PanelManager.ts
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/TocDashboardPanel.tsx
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/VisuDashboardPanel.tsx
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/WebsocketManager.ts
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/icons/index.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/icons/react-app-env.d.ts
--rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/plugins/dashboards.ts
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/plugins/uploadNotebook.tsx
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/redux/store.ts
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/redux/types.d.ts
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/redux/reducers/CommonDashboardReducer.ts
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/redux/reducers/SideDashboardReducer.ts
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/redux/reducers/ToCDashboardReducer.ts
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/PageRouter.tsx
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/buttons/SortDropDown.tsx
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/buttons/TimeDropDown.tsx
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/cell/CellInput.tsx
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/cell/CellOutput.tsx
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/cell/MarkdownComponent.tsx
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/layout/GridSystem.tsx
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/layout/TopBreadcrumb.tsx
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/notebook/ChartContainer.tsx
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/notebook/CodeExecComponent.tsx
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/notebook/TimeSpentComponent.tsx
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/placeholder/Loader.tsx
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/placeholder/NoData.tsx
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/placeholder/SidebarPlaceholder.tsx
--rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/pages/Cell.tsx
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/pages/Notebook.tsx
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/ExportCSVButton.tsx
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/TocReactComponent.tsx
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/tocDashboardItem.tsx
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/tocDashboardTree.tsx
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/index.ts
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/options_manager.ts
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/render.tsx
--rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/toolbar_generator.tsx
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/utils.ts
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/chartOptions.ts
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/compatibility.ts
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/constants.ts
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/headings.d.ts
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/interactionRecorder.ts
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/interfaces.ts
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/utils/utils.ts
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/widget-extensions/CellButton.ts
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/widget-extensions/NotebookButton.ts
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/src/widget-extensions/index.ts
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/base.css
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/index.css
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/index.js
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/reactVisu.css
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/tocDashboard.css
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/tocDashboardEditor.css
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/upload.css
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/icons/analytics.svg
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/icons/eyeFill.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/icons/eyeSlash.svg
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/icons/folder.svg
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/style/icons/notebook.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   144130 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/yarn.lock
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/tests/jupyterlab_unianalytics_dashboard.spec.ts
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/LICENSE
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/README.md
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/pyproject.toml
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.8/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/.copier-answers.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/.yarnrc.yml
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/babel.config.js
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/conftest.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jest.config.js
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/junit.xml
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/setup.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/tsconfig.test.json
+-rw-r--r--   0        0        0   381308 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/yarn.lock
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyter-config/server-config/jupyterlab_unianalytics_dashboard.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/_version.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/handlers.py
+-rw-r--r--   0        0        0     6675 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/package.json
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/package.json.orig
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/plugin.json
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/10.1e5c908a94fc4b83c2e5.js
+-rw-r--r--   0        0        0   119059 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/18.759fbf2374edc42b5c3e.js
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/18.759fbf2374edc42b5c3e.js.LICENSE.txt
+-rw-r--r--   0        0        0    34889 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/308.d9da4ce35f354c6f12e1.js
+-rw-r--r--   0        0        0   232611 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/39.5a3b28a79ba693a9b627.js
+-rw-r--r--   0        0        0    67067 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/419.8d7c0e30d3f058138a25.js
+-rw-r--r--   0        0        0    44909 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/426.a7015f9dfda310972c1b.js
+-rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/546.d5da555479f21a401709.js
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/563.b613f734176cb51510ef.js
+-rw-r--r--   0        0        0   211595 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/638.d37271636c4d956096de.js
+-rw-r--r--   0        0        0   202771 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/708.323c3614d31a5918cfaf.js
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/708.323c3614d31a5918cfaf.js.LICENSE.txt
+-rw-r--r--   0        0        0  3046069 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/744.329dc4d1ed2f5c918266.js
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/798.33a8f0893a66574e9259.js
+-rw-r--r--   0        0        0    14181 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js.LICENSE.txt
+-rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/remoteEntry.f90079a80d3ca2c7e110.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/style.js
+-rw-r--r--   0        0        0    70668 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/tests/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/tests/test_handlers.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/schema/plugin.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/handler.ts
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/index.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/__tests__/jupyterlab_unianalytics_dashboard.spec.ts
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/chat-dashboard/ChatContainer.tsx
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/chat-dashboard/ConnectionComponent.tsx
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/ChatDashboardPanel.tsx
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/DashboardPanel.tsx
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/PanelManager.ts
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/TocDashboardPanel.tsx
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/VisuDashboardPanel.tsx
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/WebsocketManager.ts
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/icons/index.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/icons/react-app-env.d.ts
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/plugins/dashboards.ts
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/plugins/uploadNotebook.tsx
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/redux/localStorage.ts
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/redux/store.ts
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/redux/types.d.ts
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/redux/reducers/CommonDashboardReducer.ts
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/redux/reducers/SideDashboardReducer.ts
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/redux/reducers/ToCDashboardReducer.ts
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/PageRouter.tsx
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/buttons/GroupDropDown.tsx
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/buttons/SortDropDown.tsx
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/buttons/TimeDropDown.tsx
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/CellInput.tsx
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/CellOutput.tsx
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/ExecutionComponent.tsx
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/MarkdownComponent.tsx
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/layout/GridSystem.tsx
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/layout/TopBreadcrumb.tsx
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/notebook/ChartContainer.tsx
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/notebook/CodeExecComponent.tsx
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/notebook/TimeSpentComponent.tsx
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/placeholder/Loader.tsx
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/placeholder/NoData.tsx
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/placeholder/SidebarPlaceholder.tsx
+-rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/pages/Cell.tsx
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/pages/Notebook.tsx
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/ExportCSVButton.tsx
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/TocReactComponent.tsx
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/tocDashboardItem.tsx
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/tocDashboardTree.tsx
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/index.ts
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/options_manager.ts
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/render.tsx
+-rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/toolbar_generator.tsx
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/utils.ts
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/chartOptions.ts
+-rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/compatibility.ts
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/constants.ts
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/headings.d.ts
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/interactionRecorder.ts
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/interfaces.ts
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/utils/utils.ts
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/widget-extensions/CellButton.ts
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/widget-extensions/NotebookButton.ts
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/src/widget-extensions/index.ts
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/base.css
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/index.css
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/index.js
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/reactVisu.css
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/tocDashboard.css
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/tocDashboardEditor.css
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/upload.css
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/icons/analytics.svg
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/icons/eyeFill.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/icons/eyeSlash.svg
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/icons/folder.svg
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/style/icons/notebook.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   144130 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/tests/jupyterlab_unianalytics_dashboard.spec.ts
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/LICENSE
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/README.md
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_dashboard-4.0.9/PKG-INFO
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/.copier-answers.yml` & `jupyterlab_unianalytics_dashboard-4.0.9/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/CHANGELOG.md` & `jupyterlab_unianalytics_dashboard-4.0.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 4.0.8
+## 4.0.9
 
-No merged PRs
+- Adding new dropdown filters
+- Notebook-specific persistence of filters
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 4.0.8
+
+No merged PRs
+
 ## 4.0.7
 
 - Feature: adding text-based filtering in Cell dashboard
 - Adding server extension component
 - Generating or retrieving persistent user identifier
 - Small bug fixes
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/RELEASE.md` & `jupyterlab_unianalytics_dashboard-4.0.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jest.config.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/package.json` & `jupyterlab_unianalytics_dashboard-4.0.9/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'scripts'": "{'build': 'npm run build:lib && npm run build:labextension:dev', 'build:prod': 'npm "*

 * *              "run clean && npm run build:lib:prod && npm run build:labextension', 'clean': 'npm "*

 * *              "run clean:lib', 'clean:all': 'npm run clean:lib && npm run clean:labextension && "*

 * *              "npm run clean:lintcache', 'eslint': 'npm run eslint:check --fix', "*

 * *              "'install:extension': 'npm run build', 'lint': 'npm run stylelint && npm run "*

 * *              "prettier && npm run esl […]*

```diff
@@ -162,34 +162,34 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/chili-epfl/jupyter-dashboard-visu-extension.git"
     },
     "scripts": {
-        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build": "npm run build:lib && npm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
-        "clean": "jlpm clean:lib",
-        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "build:prod": "npm run clean && npm run build:lib:prod && npm run build:labextension",
+        "clean": "npm run clean:lib",
+        "clean:all": "npm run clean:lib && npm run clean:labextension && npm run clean:lintcache",
         "clean:labextension": "rimraf jupyterlab_unianalytics_dashboard/labextension jupyterlab_unianalytics_dashboard/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
-        "eslint": "jlpm eslint:check --fix",
+        "eslint": "npm run eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
-        "install:extension": "jlpm build",
-        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
-        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
-        "prettier": "jlpm prettier:base --write --list-different",
+        "install:extension": "npm run build",
+        "lint": "npm run stylelint && npm run prettier && npm run eslint",
+        "lint:check": "npm run stylelint:check && npm run prettier:check && npm run eslint:check",
+        "prettier": "npm run prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
-        "prettier:check": "jlpm prettier:base --check",
-        "stylelint": "jlpm stylelint:check --fix",
+        "prettier:check": "npm run prettier:base --check",
+        "stylelint": "npm run stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
@@ -212,9 +212,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.8"
+    "version": "4.0.9"
 }
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/tsconfig.json` & `jupyterlab_unianalytics_dashboard-4.0.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/yarn.lock` & `jupyterlab_unianalytics_dashboard-4.0.9/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/__init__.py` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/handlers.py` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/package.json` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742361111111112%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f90079a80d3ca2c7e110.js'}}",*

 * * "'scripts'": "{'build': 'npm run build:lib && npm run build:labextension:dev', 'build:prod': 'npm "*

 * *              "run clean && npm run build:lib:prod && npm run build:labextension', 'clean': 'npm "*

 * *              "run clean:lib', 'clean:all': 'npm run clean:lib && npm run clean:labextension && "*

 * *              "npm run clean:lintcache', 'eslint': 'npm run eslint:check --fix', "*

 * *              "'install:extension': 'npm run […]*

```diff
@@ -120,15 +120,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/chili-epfl/jupyter-dashboard-visu-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8cd70c149b116f11f59e.js",
+            "load": "static/remoteEntry.f90079a80d3ca2c7e110.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_unianalytics_dashboard"
                 },
@@ -167,34 +167,34 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/chili-epfl/jupyter-dashboard-visu-extension.git"
     },
     "scripts": {
-        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build": "npm run build:lib && npm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
-        "clean": "jlpm clean:lib",
-        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "build:prod": "npm run clean && npm run build:lib:prod && npm run build:labextension",
+        "clean": "npm run clean:lib",
+        "clean:all": "npm run clean:lib && npm run clean:labextension && npm run clean:lintcache",
         "clean:labextension": "rimraf jupyterlab_unianalytics_dashboard/labextension jupyterlab_unianalytics_dashboard/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
-        "eslint": "jlpm eslint:check --fix",
+        "eslint": "npm run eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
-        "install:extension": "jlpm build",
-        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
-        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
-        "prettier": "jlpm prettier:base --write --list-different",
+        "install:extension": "npm run build",
+        "lint": "npm run stylelint && npm run prettier && npm run eslint",
+        "lint:check": "npm run stylelint:check && npm run prettier:check && npm run eslint:check",
+        "prettier": "npm run prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
-        "prettier:check": "jlpm prettier:base --check",
-        "stylelint": "jlpm stylelint:check --fix",
+        "prettier:check": "npm run prettier:base --check",
+        "stylelint": "npm run stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
@@ -217,9 +217,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.8"
+    "version": "4.0.9"
 }
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/package.json.orig` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'scripts'": "{'build': 'npm run build:lib && npm run build:labextension:dev', 'build:prod': 'npm "*

 * *              "run clean && npm run build:lib:prod && npm run build:labextension', 'clean': 'npm "*

 * *              "run clean:lib', 'clean:all': 'npm run clean:lib && npm run clean:labextension && "*

 * *              "npm run clean:lintcache', 'eslint': 'npm run eslint:check --fix', "*

 * *              "'install:extension': 'npm run build', 'lint': 'npm run stylelint && npm run "*

 * *              "prettier && npm run esl […]*

```diff
@@ -162,34 +162,34 @@
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/chili-epfl/jupyter-dashboard-visu-extension.git"
     },
     "scripts": {
-        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build": "npm run build:lib && npm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
-        "clean": "jlpm clean:lib",
-        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "build:prod": "npm run clean && npm run build:lib:prod && npm run build:labextension",
+        "clean": "npm run clean:lib",
+        "clean:all": "npm run clean:lib && npm run clean:labextension && npm run clean:lintcache",
         "clean:labextension": "rimraf jupyterlab_unianalytics_dashboard/labextension jupyterlab_unianalytics_dashboard/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
-        "eslint": "jlpm eslint:check --fix",
+        "eslint": "npm run eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
-        "install:extension": "jlpm build",
-        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
-        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
-        "prettier": "jlpm prettier:base --write --list-different",
+        "install:extension": "npm run build",
+        "lint": "npm run stylelint && npm run prettier && npm run eslint",
+        "lint:check": "npm run stylelint:check && npm run prettier:check && npm run eslint:check",
+        "prettier": "npm run prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
-        "prettier:check": "jlpm prettier:base --check",
-        "stylelint": "jlpm stylelint:check --fix",
+        "prettier:check": "npm run prettier:base --check",
+        "stylelint": "npm run stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
@@ -212,9 +212,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.8"
+    "version": "4.0.9"
 }
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/plugin.json` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/schemas/jupyterlab_unianalytics_dashboard/plugin.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666666%*

 * *Differences: {"'properties'": "{'commonDashboardSettings': {'properties': {delete: ['realTime']}}}"}*

```diff
@@ -20,20 +20,14 @@
         "commonDashboardSettings": {
             "properties": {
                 "dashboardCollection": {
                     "default": true,
                     "description": "Whether to enable the collection of interaction clicks with the dashboard extension to better understand what features are more or less used.",
                     "title": "Collect clicks relative to dashboard usage",
                     "type": "boolean"
-                },
-                "realTime": {
-                    "default": true,
-                    "description": "Whether to only display currently connected users data (true), or consider historical data according to the selected time limit filter value (false)",
-                    "title": "Activate real-time dashboard",
-                    "type": "boolean"
                 }
             },
             "title": "Dashboard Settings",
             "type": "object"
         },
         "tocDashboardSettings": {
             "properties": {
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/10.1e5c908a94fc4b83c2e5.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/10.1e5c908a94fc4b83c2e5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/120.f9ab87c96623964d015f.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/419.8d7c0e30d3f058138a25.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,49 +1,76 @@
 "use strict";
 (self.webpackChunkjupyterlab_unianalytics_dashboard = self.webpackChunkjupyterlab_unianalytics_dashboard || []).push([
-    [120], {
-        8859: (e, t, o) => {
+    [419], {
+        575: (e, t, o) => {
             o.r(t), o.d(t, {
-                CURRENT_NOTEBOOK_ID: () => wt,
-                PERSISTENT_USER_ID: () => Ct,
-                default: () => Et,
-                setCurrentNotebookId: () => vt
+                CURRENT_NOTEBOOK_ID: () => Rt,
+                PERSISTENT_USER_ID: () => Lt,
+                default: () => Bt,
+                setCurrentNotebookId: () => At
             });
-            var n = o(7750),
-                a = o(6249),
-                s = o(8547),
-                l = o(4991);
-            let i, r;
-            o(4039), i = "https://api.unianalytics.ch", r = "wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/";
+            var n = o(8368),
+                a = o(8031),
+                s = o(8048),
+                l = o(4008);
+            let r, i;
+            o(4039), r = "https://api.unianalytics.ch", i = "wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/";
             const c = "jupyterlab_unianalytics_dashboard",
                 d = `${c}:plugin`,
                 h = `${c}_access_token`,
-                m = `${c}_refresh_token`;
-            var u;
+                u = `${c}_refresh_token`,
+                m = `${c}/commondashboard:redux_state`;
+            var p;
             ! function(e) {
                 e.dashboardOpenVisu = `${c}:dashboard-open-visu`, e.uploadNotebook = `${c}:dashboard-upload-notebook`, e.copyDownloadLink = `${c}:dashboard-copy-download-link`
-            }(u || (u = {}));
-            const p = '.jp-DirListing-item[data-file-type="notebook"]',
-                g = "unianalytics";
-            var _, b;
+            }(p || (p = {}));
+            const g = '.jp-DirListing-item[data-file-type="notebook"]',
+                b = "unianalytics";
+            var _;
             ! function(e) {
-                e.notebookId = `${g}_notebook_id`, e.cellMapping = `${g}_cell_mapping`
+                e.notebookId = `${b}_notebook_id`, e.cellMapping = `${b}_cell_mapping`
             }(_ || (_ = {}));
+            const v = [{
+                key: "timeDesc",
+                label: "Time (most recent 1st)",
+                method: (e, t) => new Date(e.t_finish) < new Date(t.t_finish) ? 1 : -1
+            }, {
+                key: "timeAsc",
+                label: "Time (oldest 1st)",
+                method: (e, t) => new Date(e.t_finish) > new Date(t.t_finish) ? 1 : -1
+            }, {
+                key: "inputAsc",
+                label: "Input (shortest 1st)",
+                method: (e, t) => e.cell_input.length - t.cell_input.length
+            }, {
+                key: "inputDesc",
+                label: "Input (longest 1st)",
+                method: (e, t) => t.cell_input.length - e.cell_input.length
+            }, {
+                key: "outputAsc",
+                label: "Output (shortest 1st)",
+                method: (e, t) => e.cell_output_length - t.cell_output_length
+            }, {
+                key: "outputDesc",
+                label: "Output (longest 1st)",
+                method: (e, t) => t.cell_output_length - e.cell_output_length
+            }];
+            var k;
             class w {
                 static async setJupyterVersion(e) {
                     w._jupyterVersion = e, await w._setEditorLanguageRegistry(), await w._asyncImports()
                 }
                 static async _setEditorLanguageRegistry() {
                     if (4 === w._jupyterVersion) {
                         const {
                             StreamLanguage: e
                         } = await o.e(373).then(o.t.bind(o, 1373, 23)), {
                             EditorLanguageRegistry: t,
                             parseMathIPython: n
-                        } = await Promise.resolve().then(o.t.bind(o, 7388, 23)), a = new t;
+                        } = await Promise.resolve().then(o.t.bind(o, 7777, 23)), a = new t;
                         t.getDefaultLanguages().forEach((e => {
                             a.addLanguage(e)
                         })), a.addLanguage({
                             name: "ipythongfm",
                             mime: "text/x-ipythongfm",
                             load: async () => {
                                 const [t, s] = await Promise.all([Promise.all([o.e(638), o.e(211), o.e(373), o.e(376)]).then(o.bind(o, 8638)), o.e(10).then(o.bind(o, 8010))]);
@@ -60,15 +87,15 @@
                     if (4 === w._jupyterVersion) {
                         const {
                             EditorView: e
                         } = await o.e(211).then(o.t.bind(o, 6211, 23));
                         this._EditorView = e;
                         const {
                             jupyterTheme: t
-                        } = await Promise.resolve().then(o.t.bind(o, 7388, 23));
+                        } = await Promise.resolve().then(o.t.bind(o, 7777, 23));
                         this._jupyterTheme = t
                     }
                 }
                 static checkJupyterVersionSet() {
                     if (null === w._jupyterVersion) throw new Error("JupyterLab version is not set in CompatibilityManager before trying to access it.")
                 }
                 static observeEditorVisibility(e) {
@@ -76,15 +103,15 @@
                         t[0].isIntersecting && e.refresh()
                     }), {
                         root: null,
                         threshold: .5
                     }) : null
                 }
             }
-            b = w, w._jupyterVersion = null, w._editorDefaultLanguages = void 0, w._EditorView = void 0, w._jupyterTheme = void 0, w.getMetadataComp = (e, t) => {
+            k = w, w._jupyterVersion = null, w._editorDefaultLanguages = void 0, w._EditorView = void 0, w._jupyterTheme = void 0, w.getMetadataComp = (e, t) => {
                 var o;
                 return w.checkJupyterVersionSet(), 4 === w._jupyterVersion ? null == e ? void 0 : e.getMetadata(t) : null === (o = null == e ? void 0 : e.metadata) || void 0 === o ? void 0 : o.get(t)
             }, w.setMetadataComp = (e, t, o) => {
                 var n;
                 w.checkJupyterVersionSet(), 4 === w._jupyterVersion ? null == e || e.setMetadata(t, o) : null === (n = null == e ? void 0 : e.metadata) || void 0 === n || n.set(t, o)
             }, w.deleteMetadataComp = (e, t) => {
                 var o;
@@ -93,127 +120,131 @@
                 var t;
                 w.checkJupyterVersionSet();
                 const o = null === (t = e.tracker.currentWidget) || void 0 === t ? void 0 : t.selectedItems().next();
                 return 4 === w._jupyterVersion ? null == o ? void 0 : o.value : o
             }, w.getCellsArrComp = e => (w.checkJupyterVersionSet(), e ? Array.from({
                 length: e.length
             }, ((t, o) => e.get(o))) : null), w.getCodeMirrorOptionsComp = () => (w.checkJupyterVersionSet(), 4 === w._jupyterVersion ? {
-                extensions: [b._jupyterTheme, b._EditorView.lineWrapping, b._EditorView.editable.of(!1)],
+                extensions: [k._jupyterTheme, k._EditorView.lineWrapping, k._EditorView.editable.of(!1)],
                 languages: w._editorDefaultLanguages
             } : {
                 config: {
                     readOnly: !0
                 }
             }), w.getNextWidgetValueComp = e => {
                 var t;
                 return w.checkJupyterVersionSet(), 4 === w._jupyterVersion ? null === (t = e.next()) || void 0 === t ? void 0 : t.value : e.next()
             };
-            const v = async (e, t) => {
-                const o = await C(e, t);
-                if (401 === o.status) {
-                    const n = await o.json();
-                    if ("expired_token" === (null == n ? void 0 : n.status)) {
-                        if (await k()) return C(e, t);
-                        console.log(`${c}: Token refresh failed.`)
-                    }
-                }
-                return o
-            }, C = async (e, t) => {
-                const o = {
-                        headers: {
-                            Authorization: `Bearer ${sessionStorage.getItem(h)}`
+            const C = (e, t) => {
+                    var o, n;
+                    return `displayRealTime=${null===(o=e.displayRealTime[t])||void 0===o||o}` + (e.t1ISOString[t] ? "&t1=" + e.t1ISOString[t] : "") + ((null === (n = e.selectedGroups[t]) || void 0 === n ? void 0 : n.length) > 0 ? "&selectedGroups=" + encodeURIComponent(JSON.stringify(e.selectedGroups[t])) : "")
+                },
+                E = async (e, t) => {
+                    const o = await y(e, t);
+                    if (401 === o.status) {
+                        const n = await o.json();
+                        if ("expired_token" === (null == n ? void 0 : n.status)) {
+                            if (await f()) return y(e, t);
+                            console.log(`${c}: Token refresh failed.`)
                         }
-                    },
-                    n = {
-                        ...o,
-                        ...t,
+                    }
+                    return o
+                }, y = async (e, t) => {
+                    const o = {
+                            headers: {
+                                Authorization: `Bearer ${sessionStorage.getItem(h)}`
+                            }
+                        },
+                        n = {
+                            ...o,
+                            ...t,
+                            headers: {
+                                ...o.headers,
+                                ...(null == t ? void 0 : t.headers) || {}
+                            }
+                        };
+                    return fetch(e, n)
+                }, f = async () => {
+                    const e = await fetch(`${r}/auth/refresh`, {
+                        method: "POST",
                         headers: {
-                            ...o.headers,
-                            ...(null == t ? void 0 : t.headers) || {}
+                            Authorization: `Bearer ${sessionStorage.getItem(u)}`
                         }
-                    };
-                return fetch(e, n)
-            }, k = async () => {
-                const e = await fetch(`${i}/auth/refresh`, {
-                    method: "POST",
-                    headers: {
-                        Authorization: `Bearer ${sessionStorage.getItem(m)}`
+                    });
+                    if (e.ok) {
+                        const t = await e.json();
+                        if (null == t ? void 0 : t.access_token) return sessionStorage.setItem(h, t.access_token), !0
                     }
-                });
-                if (e.ok) {
-                    const t = await e.json();
-                    if (null == t ? void 0 : t.access_token) return sessionStorage.setItem(h, t.access_token), !0
-                }
-                return !1
-            }, E = e => !!(e && !e.isDisposed && e.context.isReady && w.getMetadataComp(e.context.model, _.notebookId) && w.getMetadataComp(e.context.model, _.cellMapping));
-            var f = o(6029),
-                y = o.n(f),
-                S = o(8448),
-                O = o(7403);
-            const D = e => {
-                const [t, o] = (0, f.useState)(!1);
-                return y().createElement("div", null, y().createElement("p", null, "Successfully uploaded, can be downloaded accessing:"), y().createElement("div", {
+                    return !1
+                }, S = e => !!(e && !e.isDisposed && e.context.isReady && w.getMetadataComp(e.context.model, _.notebookId) && w.getMetadataComp(e.context.model, _.cellMapping)), O = (e, t) => !(!e || !t) && e.length === t.length && e.every(((e, o) => e === t[o]));
+            var D = o(6029),
+                N = o.n(D),
+                x = o(3452),
+                I = o(9510);
+            const T = e => {
+                const [t, o] = (0, D.useState)(!1);
+                return N().createElement("div", null, N().createElement("p", null, "Successfully uploaded, can be downloaded accessing:"), N().createElement("div", {
                     className: "unianalytics-link-container"
-                }, y().createElement("div", {
+                }, N().createElement("div", {
                     className: "unianalytics-link"
-                }, e.url), y().createElement("div", {
+                }, e.url), N().createElement("div", {
                     className: "unianalytics-link-button-container"
-                }, y().createElement("button", {
+                }, N().createElement("button", {
                     className: "unianalytics-link-button",
                     onClick: () => {
                         navigator.clipboard.writeText(e.url).then((() => {
                             o(!0)
                         })).catch((e => {
                             console.error(`${c}: Error copying to clipboard: `, e)
                         }))
                     }
-                }, t ? y().createElement(S.checkIcon.react, null) : y().createElement(S.copyIcon.react, null)))))
+                }, t ? N().createElement(x.checkIcon.react, null) : N().createElement(x.copyIcon.react, null)))))
             };
-            const x = new S.LabIcon({
+            const R = new x.LabIcon({
                     name: `${c}:visu-icon`,
                     svgstr: '<svg height="200px" width="200px" viewBox="0 0 512 512.001"\nxmlns="http://www.w3.org/2000/svg">\n <g id="SVGRepo_bgCarrier" stroke-width="0"></g>\n <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>\n <g id="SVGRepo_iconCarrier"> \n <g> <g> \n <g> <path xmlns="http://www.w3.org/2000/svg" fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M105.094,307.2h129.347c16.345,0,29.642-13.298,29.642-29.642v-43.116c0-16.344-13.297-29.642-29.642-29.642H105.094 c-16.344,0-29.642,13.298-29.642,29.642v43.116C75.452,293.902,88.75,307.2,105.094,307.2z M91.621,234.442 c0-7.43,6.044-13.474,13.474-13.474h129.347c7.43,0,13.474,6.044,13.474,13.474v43.116c0,7.43-6.044,13.474-13.474,13.474 H105.094c-7.43,0-13.474-6.044-13.474-13.474V234.442z"></path> \n <path xmlns="http://www.w3.org/2000/svg" fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M509.633,476.642l-21.558-21.558c-3.157-3.156-8.275-3.156-11.433,0c-3.157,3.157-3.157,8.275,0,11.433l7.758,7.757H51.2 c-7.43,0-13.474-6.044-13.474-13.474V27.601l7.758,7.758c3.156,3.156,8.275,3.156,11.432,0c3.157-3.157,3.157-8.275,0-11.433 L35.358,2.367c-3.156-3.156-8.275-3.156-11.432,0L2.368,23.925c-3.157,3.157-3.157,8.275,0,11.433 c3.156,3.156,8.275,3.156,11.432,0l7.758-7.758V460.8c0,16.344,13.298,29.642,29.642,29.643h433.198l-7.758,7.757 c-3.157,3.157-3.157,8.275,0,11.433c1.579,1.578,3.649,2.367,5.717,2.367c2.068,0,4.138-0.789,5.717-2.367l21.558-21.558 C512.79,484.917,512.79,479.799,509.633,476.642z"></path>\n  <path xmlns="http://www.w3.org/2000/svg" fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M105.094,177.853h377.263c16.344,0,29.642-13.298,29.642-29.642v-43.116c0-16.344-13.298-29.642-29.642-29.642H105.094 c-16.344,0-29.642,13.298-29.642,29.642v43.116C75.452,164.555,88.75,177.853,105.094,177.853z M91.621,105.095 c0-7.43,6.045-13.474,13.474-13.474h377.263c7.43,0,13.474,6.044,13.474,13.474v43.116c0,7.43-6.044,13.474-13.474,13.474 H105.094c-7.43,0-13.474-6.044-13.474-13.474V105.095z"></path> \n  <path xmlns="http://www.w3.org/2000/svg" fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M105.094,436.548H353.01c16.344,0,29.642-13.298,29.642-29.642V363.79c0-16.344-13.298-29.642-29.642-29.642H105.094 c-16.344,0-29.642,13.298-29.642,29.642v43.116C75.452,423.25,88.75,436.548,105.094,436.548z M91.621,363.79 c0-7.43,6.044-13.474,13.474-13.474H353.01c7.43,0,13.474,6.044,13.474,13.474v43.116c0,7.43-6.044,13.474-13.474,13.474H105.094 c-7.43,0-13.474-6.044-13.474-13.474V363.79z"></path> </g>\n   </g> </g> </g>\n   </svg>'
                 }),
-                N = new S.LabIcon({
+                A = new x.LabIcon({
                     name: `${c}:hide-icon`,
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-eye-slash-fill" viewBox="0 0 16 16">\n  <path d="m10.79 12.912-1.614-1.615a3.5 3.5 0 0 1-4.474-4.474l-2.06-2.06C.938 6.278 0 8 0 8s3 5.5 8 5.5a7.029 7.029 0 0 0 2.79-.588zM5.21 3.088A7.028 7.028 0 0 1 8 2.5c5 0 8 5.5 8 5.5s-.939 1.721-2.641 3.238l-2.062-2.062a3.5 3.5 0 0 0-4.474-4.474L5.21 3.089z"/>\n  <path d="M5.525 7.646a2.5 2.5 0 0 0 2.829 2.829l-2.83-2.829zm4.95.708-2.829-2.83a2.5 2.5 0 0 1 2.829 2.829zm3.171 6-12-12 .708-.708 12 12-.708.708z"/>\n</svg>'
                 }),
-                T = new S.LabIcon({
+                L = new x.LabIcon({
                     name: `${c}:show-icon`,
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-eye-fill" viewBox="0 0 16 16">\n  <path d="M10.5 8a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0z"/>\n  <path d="M0 8s3-5.5 8-5.5S16 8 16 8s-3 5.5-8 5.5S0 8 0 8zm8 3.5a3.5 3.5 0 1 0 0-7 3.5 3.5 0 0 0 0 7z"/>\n</svg>'
                 });
-            var R = o(3748);
-            const I = {
+            var M = o(3748);
+            const B = {
                     displayDashboard: !0,
                     hasNotebookId: !1
                 },
-                L = (0, R.createSlice)({
+                H = (0, M.createSlice)({
                     name: "tocdashboard",
-                    initialState: I,
+                    initialState: B,
                     reducers: {
                         setDisplayHideDashboard: (e, t) => {
                             e.displayDashboard = t.payload
                         },
                         setHasNotebookId: (e, t) => {
                             e.hasNotebookId = t.payload
                         }
                     }
                 }),
                 {
-                    setDisplayHideDashboard: A,
-                    setHasNotebookId: M
-                } = L.actions,
-                B = L.reducer,
-                H = {
+                    setDisplayHideDashboard: $,
+                    setHasNotebookId: F
+                } = H.actions,
+                U = H.reducer,
+                V = {
                     navigationState: [{
                         pageName: "Notebook"
                     }]
                 },
-                $ = (0, R.createSlice)({
+                P = (0, M.createSlice)({
                     name: "sidedashboard",
-                    initialState: H,
+                    initialState: V,
                     reducers: {
                         navigateToNotebook: (e, t) => {
                             e.navigationState = [{
                                 pageName: "Notebook"
                             }]
                         },
                         navigateToCell: (e, t) => {
@@ -226,82 +257,133 @@
                                 }
                             }]
                         },
                         navigateToHistory: (e, t) => {
                             e.navigationState = e.navigationState.slice(0, t.payload + 1)
                         },
                         resetNavigationState: (e, t) => {
-                            e.navigationState = H.navigationState
+                            e.navigationState = V.navigationState
                         }
                     }
                 }),
                 {
-                    navigateToNotebook: U,
-                    navigateToCell: F,
-                    navigateToHistory: V,
-                    resetNavigationState: z
-                } = $.actions,
-                P = $.reducer,
-                W = (0, R.createSlice)({
+                    navigateToNotebook: z,
+                    navigateToCell: j,
+                    navigateToHistory: W,
+                    resetNavigationState: G
+                } = P.actions,
+                J = P.reducer,
+                K = {
+                    notebookCells: null,
+                    refreshBoolean: !1,
+                    sortBy: {},
+                    dashboardQueryArgs: {
+                        displayRealTime: {},
+                        t1ISOString: {},
+                        selectedGroups: {}
+                    }
+                },
+                Q = (0, M.createSlice)({
                     name: "commondashboard",
-                    initialState: {
-                        notebookCells: null,
-                        timeWindow: "null",
-                        refreshBoolean: !1,
-                        displayRealTime: !0
-                    },
+                    initialState: K,
                     reducers: {
-                        setTimeWindow: (e, t) => {
-                            e.timeWindow = t.payload
+                        setDashboardQueryArgsTimeFilter: (e, t) => {
+                            const {
+                                notebookId: o,
+                                t1ISOString: n
+                            } = t.payload;
+                            e.dashboardQueryArgs.t1ISOString[o] = n
+                        },
+                        setDashboardQueryArgsSelectedGroups: (e, t) => {
+                            const {
+                                notebookId: o,
+                                groups: n
+                            } = t.payload, a = e.dashboardQueryArgs.selectedGroups[o] || [];
+                            if (!O(a, n)) return {
+                                ...e,
+                                dashboardQueryArgs: {
+                                    ...e.dashboardQueryArgs,
+                                    selectedGroups: {
+                                        ...e.dashboardQueryArgs.selectedGroups,
+                                        [o]: n
+                                    }
+                                }
+                            }
+                        },
+                        setDashboardQueryArgsDisplayRealTime: (e, t) => {
+                            const {
+                                notebookId: o,
+                                displayRealTime: n
+                            } = t.payload;
+                            e.dashboardQueryArgs.displayRealTime[o] = n
+                        },
+                        setSortBy: (e, t) => {
+                            const {
+                                notebookId: o,
+                                sortCriterion: n
+                            } = t.payload;
+                            e.sortBy[o] = n
                         },
                         setNotebookCells: (e, t) => {
                             e.notebookCells = t.payload
                         },
                         refreshDashboards: e => {
                             e.refreshBoolean = !e.refreshBoolean
-                        },
-                        displayRealTime: (e, t) => {
-                            e.displayRealTime = t.payload
                         }
                     }
                 }),
                 {
-                    setTimeWindow: j,
-                    setNotebookCells: K,
-                    refreshDashboards: G,
-                    displayRealTime: J
-                } = W.actions,
-                q = W.reducer,
-                X = (0, R.configureStore)({
-                    reducer: {
-                        tocdashboard: B,
-                        sidedashboard: P,
-                        commondashboard: q
+                    setDashboardQueryArgsTimeFilter: q,
+                    setDashboardQueryArgsSelectedGroups: X,
+                    setDashboardQueryArgsDisplayRealTime: Z,
+                    setSortBy: Y,
+                    setNotebookCells: ee,
+                    refreshDashboards: te
+                } = Q.actions,
+                oe = Q.reducer,
+                ne = e => t => o => {
+                    const n = t(o);
+                    if (o.type.startsWith("commondashboard/")) {
+                        const t = e.getState();
+                        localStorage.setItem(m, JSON.stringify(t.commondashboard))
                     }
+                    return n
+                },
+                ae = {
+                    commondashboard: localStorage.getItem(m) ? JSON.parse(localStorage.getItem(m)) : K
+                },
+                se = (0, M.configureStore)({
+                    reducer: {
+                        tocdashboard: U,
+                        sidedashboard: J,
+                        commondashboard: oe
+                    },
+                    middleware: e => e().concat(ne),
+                    preloadedState: ae
                 });
-            var Z, Q, Y = o(2445),
-                ee = o(4351),
-                te = o(4901);
-            class oe {}! function(e) {
+            var le, re, ie = o(8797),
+                ce = o(6311),
+                de = o(4901);
+            class he {}! function(e) {
                 e.LOADING = "Loading", e.NOTFOUND = "Notebook not Registered", e.USERNOTAUTHORIZED = "No User Permission for this Notebook", e.EXPIREDTOKEN = "Expired Login Token", e.INVALIDCREDENTIALS = "Invalid Credentials", e.ERROR = "Fetching Error", e.SUCCESS = "Success"
-            }(Z || (Z = {})),
+            }(le || (le = {})),
             function(e) {
                 e.RIGHT_DASHBOARD_SHOW_HIDE = "RIGHT_DASHBOARD_SHOW_HIDE", e.TOC_DASHBOARD_SHOW_HIDE = "TOC_DASHBOARD_SHOW_HIDE", e.NOTEBOOK_CELL_BUTTON = "NOTEBOOK_CELL_BUTTON", e.NOTEBOOK_TOOLBAR_BUTTON = "NOTEBOOK_TOOLBAR_BUTTON", e.TOC_OPEN_CELL_DASHBOARD = "TOC_OPEN_CELL_DASHBOARD", e.TOC_HEADING_CLICKED = "TOC_HEADING_CLICKED", e.TOC_COLLAPSE_HEADERS = "TOC_COLLAPSE_HEADERS", e.BREADCRUMB_TO_NOTEBOOK = "BREADCRUMB_TO_NOTEBOOK", e.BREADCRUMB_TO_CELL = "BREADCRUMB_TO_CELL", e.DASHBOARD_REFRESH_BUTTON = "DASHBOARD_REFRESH_BUTTON", e.DASHBOARD_FILTER_TIME = "DASHBOARD_FILTER_TIME", e.CELL_DASHBOARD_FILTER_SORT = "CELL_DASHBOARD_FILTER_SORT", e.CELL_DASHBOARD_FILTER_CODE_INPUT = "CELL_DASHBOARD_FILTER_CODE_INPUT", e.CELL_DASHBOARD_FILTER_CODE_OUTPUT = "CELL_DASHBOARD_FILTER_CODE_OUTPUT", e.CELL_DASHBOARD_FILTER_EXECUTION = "CELL_DASHBOARD_FILTER_EXECUTION", e.TOC_TOOLBAR_CODE = "TOC_TOOLBAR_CODE", e.TOC_TOOLBAR_MARKDOWN = "TOC_TOOLBAR_MARKDOWN", e.TOC_TOOLBAR_NUMBERED = "TOC_TOOLBAR_NUMBERED", e.TOC_TOOLBAR_SHOW_HIDE = "TOC_TOOLBAR_SHOW_HIDE", e.TOC_TOOLBAR_REFRESH = "TOC_TOOLBAR_REFRESH"
-            }(Q || (Q = {}));
-            const ne = X.dispatch;
-            class ae {
+            }(re || (re = {}));
+            const ue = se.dispatch;
+            class me {
                 constructor() {
                     this._socket = null, this._ongoingConnectionInfo = null, this._pingInterval = 54e4, this._pingTimer = null
                 }
                 _createSocket(e) {
                     this._socket = new WebSocket(`wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/?nbId=${e.notebookId}&conType=TEACHER`), this._socket.addEventListener("open", (() => {
                         console.log(`${c}: WebSocket connection opened for`, e), this._startPingTimer()
                     })), this._socket.addEventListener("message", (e => {
                         const t = JSON.parse(e.data);
-                        "refreshDashboard" === t.action && ne(G()), console.log(`${c}: Received message from server:`, t)
+                        "refreshDashboard" === t.action && ue(te()), console.log(`${c}: Received message from server:`, t)
                     })), this._socket.addEventListener("close", (t => {
                         console.log(`${c}: WebSocket connection closed for `, e, t), this._stopPingTimer()
                     })), this._socket.addEventListener("error", (e => {
                         console.error(`${c}: WebSocket error`, e)
                     }))
                 }
                 establishSocketConnection(e) {
@@ -318,64 +400,64 @@
                         this._socket && this._socket.readyState === WebSocket.OPEN && this._socket.send('{ "action":"ping" }')
                     }), this._pingInterval)
                 }
                 _stopPingTimer() {
                     this._pingTimer && (clearInterval(this._pingTimer), this._pingTimer = null)
                 }
             }
-            const se = X.dispatch;
-            class le {
+            const pe = se.dispatch;
+            class ge {
                 constructor() {
-                    this._panelUpdatedSignal = new te.Signal(this), this._panelSwitchedSignal = new te.Signal(this), this._ongoingContextId = "", this._ongoingCheckId = "", this._panel = null, this._monitor = null, this._validityChecks = {
+                    this._panelUpdatedSignal = new de.Signal(this), this._panelSwitchedSignal = new de.Signal(this), this._ongoingContextId = "", this._ongoingCheckId = "", this._panel = null, this._monitor = null, this._validityChecks = {
                         tag: null,
-                        registered: Z.LOADING
-                    }, this._websocketManager = new ae
+                        registered: le.LOADING
+                    }, this._websocketManager = new me
                 }
                 get validityChecks() {
                     return this._validityChecks
                 }
                 get notebookCells() {
                     return this._notebookCells
                 }
                 get panel() {
                     return this._panel
                 }
                 set panel(e) {
                     if (this._panel === e) return;
-                    if (this._panel && this._panel.disposed.disconnect(this._onPanelDisposed, this), vt(null), this._validityChecks = {
+                    if (this._panel && this._panel.disposed.disconnect(this._onPanelDisposed, this), At(null), this._validityChecks = {
                             tag: null,
-                            registered: Z.LOADING
+                            registered: le.LOADING
                         }, this._websocketManager.terminateSocketConnection(), this._panel = e, this._onPanelSwitched(), this._panel && this._panel.disposed.connect(this._onPanelDisposed, this), this._monitor && (this._monitor.dispose(), this._monitor = null), !this._panel) return void this._onPanelUpdated();
                     const t = crypto.randomUUID();
                     this._ongoingContextId = t, this._panel.sessionContext.ready.then((() => {
                         if (this._ongoingContextId === t && this._panel && !this._panel.isDisposed) {
-                            if (this._monitor = new ee.ActivityMonitor({
+                            if (this._monitor = new ce.ActivityMonitor({
                                     signal: this._panel.context.model.contentChanged,
                                     timeout: 1e3
-                                }), this._monitor.activityStopped.connect(this._onPanelUpdated, this), E(this._panel)) {
+                                }), this._monitor.activityStopped.connect(this._onPanelUpdated, this), S(this._panel)) {
                                 const e = w.getMetadataComp(this._panel.model, _.notebookId);
-                                vt(e), this._validityChecks = {
+                                At(e), this._validityChecks = {
                                     tag: e,
-                                    registered: Z.LOADING
+                                    registered: le.LOADING
                                 }, this._performRegistrationCheck()
                             }
                             this._onPanelUpdated()
                         }
                     }))
                 }
                 _performRegistrationCheck() {
                     const e = crypto.randomUUID();
                     this._ongoingCheckId = e;
-                    let t = Z.ERROR;
-                    v(`${i}/dashboard/${this._validityChecks.tag}/check`).then((e => e.json())).then((e => {
-                        (null == e ? void 0 : e.status) ? "expired_token" === e.status ? t = Z.EXPIREDTOKEN : "not_found" === e.status ? t = Z.NOTFOUND : "no_user_permission" === e.status ? t = Z.USERNOTAUTHORIZED : "success" === e.status && (t = Z.SUCCESS): t = Z.INVALIDCREDENTIALS
+                    let t = le.ERROR;
+                    E(`${r}/dashboard/${this._validityChecks.tag}/check`).then((e => e.json())).then((e => {
+                        (null == e ? void 0 : e.status) ? "expired_token" === e.status ? t = le.EXPIREDTOKEN : "not_found" === e.status ? t = le.NOTFOUND : "no_user_permission" === e.status ? t = le.USERNOTAUTHORIZED : "success" === e.status && (t = le.SUCCESS): t = le.INVALIDCREDENTIALS
                     })).catch((e => {
                         console.log(`${c}: Notebook check fetching error (check your connection).` + e)
                     })).finally((() => {
-                        this._ongoingCheckId === e && this._panel && !this._panel.isDisposed && (this._validityChecks.registered = t, this._validityChecks.registered === Z.SUCCESS && (se(z()), this._websocketManager.establishSocketConnection({
+                        this._ongoingCheckId === e && this._panel && !this._panel.isDisposed && (this._validityChecks.registered = t, this._validityChecks.registered === le.SUCCESS && (pe(G()), this._websocketManager.establishSocketConnection({
                             notebookId: this._validityChecks.tag
                         })), this._panelUpdatedSignal.emit(void 0))
                     }))
                 }
                 _onPanelDisposed(e) {
                     this.panel = null
                 }
@@ -392,189 +474,344 @@
                     this._updateCellList(), this._panelUpdatedSignal.emit(void 0)
                 }
                 _updateCellList() {
                     var e, t;
                     const o = w.getCellsArrComp(null === (t = null === (e = this.panel) || void 0 === e ? void 0 : e.model) || void 0 === t ? void 0 : t.cells);
                     if (o) {
                         const e = o.map((e => e.id));
-                        if (n = e, a = this._notebookCells, !(n && a && n.length === a.length && n.every(((e, t) => e === a[t])))) {
+                        if (!O(e, this._notebookCells)) {
                             this._notebookCells = e;
                             const t = o.map((e => ({
                                 id: e.id,
                                 cellType: e.type
                             })));
-                            return se(K(t)), !0
+                            return pe(ee(t)), !0
                         }
                     } else this._notebookCells = null;
-                    var n, a;
                     return !1
                 }
             }
-            var ie = o(7760),
-                re = o(8559);
-            const ce = () => y().createElement("div", {
+            var be = o(7760),
+                _e = o(8559);
+            const ve = () => N().createElement("div", {
                     style: {
                         width: "100%",
                         textAlign: "center",
                         margin: "50px 0"
                     }
-                }, y().createElement(re.Spinner, {
+                }, N().createElement(_e.Spinner, {
                     style: {
                         width: "50px",
                         height: "50px",
                         fontSize: "x-large"
                     },
                     animation: "border",
                     role: "status",
                     variant: "primary"
                 })),
-                de = ({
+                ke = ({
                     title: e,
                     placeholderText: t = "No data for the opened notebook"
-                }) => y().createElement("div", {
+                }) => N().createElement("div", {
                     className: "dashboard-TableOfContents"
-                }, y().createElement("div", {
+                }, N().createElement("div", {
                     className: "dashboard-stack-panel-header"
-                }, "Side Panel Dashboard"), y().createElement("div", {
+                }, "Side Panel Dashboard"), N().createElement("div", {
                     className: "dashboard-TableOfContents-placeholder"
-                }, y().createElement("div", {
+                }, N().createElement("div", {
                     className: "dashboard-TableOfContents-placeholderContent"
-                }, y().createElement("h3", null, e), y().createElement("p", null, t))));
-            class he extends O.ReactWidget {
+                }, N().createElement("h3", null, e), N().createElement("p", null, t))));
+            class we extends I.ReactWidget {
                 constructor(e) {
                     super(), this.addClass("dashboard-panel"), this._panelManager = e, e.panelUpdated.connect((() => this.update()), this)
                 }
                 onAfterShow(e) {
                     this.update()
                 }
                 onUpdateRequest(e) {
                     super.onUpdateRequest(e)
                 }
                 render() {
-                    if (!this._panelManager.panel) return f.createElement(de, {
+                    if (!this._panelManager.panel) return D.createElement(ke, {
                         title: "No Notebook",
                         placeholderText: "Open a notebook to start viewing its content."
                     });
-                    if (!this._panelManager.panel.context.isReady) return f.createElement(ce, null);
-                    if (!this._panelManager.validityChecks.tag) return f.createElement(de, {
+                    if (!this._panelManager.panel.context.isReady) return D.createElement(ve, null);
+                    if (!this._panelManager.validityChecks.tag) return D.createElement(ke, {
                         title: "Notebook not Tagged for Tracking"
                     });
                     switch (this._panelManager.validityChecks.registered) {
-                        case Z.LOADING:
-                            return f.createElement(ce, null);
-                        case Z.SUCCESS:
-                            return f.createElement(ie.Provider, {
-                                store: X
+                        case le.LOADING:
+                            return D.createElement(ve, null);
+                        case le.SUCCESS:
+                            return D.createElement(be.Provider, {
+                                store: se
                             }, this.computeComponentToRender());
                         default:
-                            return f.createElement(de, {
+                            return D.createElement(ke, {
                                 title: this._panelManager.validityChecks.registered
                             })
                     }
                 }
             }
-            const me = he;
-            class ue {
+            const Ce = we;
+            var Ee = o(2535);
+            class ye {
                 static setPermission(e) {
-                    ue._isInteractionRecordingEnabled = e
+                    ye._isInteractionRecordingEnabled = e
                 }
             }
-            ue._isInteractionRecordingEnabled = !1, ue.sendInteraction = e => {
-                ue._isInteractionRecordingEnabled && fetch(`${i}/dashboard_interaction/add`, {
+            ye._isInteractionRecordingEnabled = !1, ye.sendInteraction = e => {
+                ye._isInteractionRecordingEnabled && fetch(`${r}/dashboard_interaction/add`, {
                     method: "POST",
                     headers: {
                         "Content-Type": "application/json"
                     },
                     body: JSON.stringify({
                         ...e,
-                        dashboard_user_id: Ct,
+                        dashboard_user_id: Lt,
                         time: (new Date).toISOString(),
-                        notebook_id: wt
+                        notebook_id: Rt
                     })
                 })
             };
-            const pe = X.dispatch,
-                ge = () => {
-                    const e = (0, ie.useSelector)((e => e.sidedashboard.navigationState));
-                    return y().createElement(re.Stack, {
+            const fe = se.dispatch,
+                Se = () => {
+                    const e = (0, be.useSelector)((e => e.sidedashboard.navigationState));
+                    return N().createElement(_e.Stack, {
                         className: "breadcrumb-container",
                         direction: "horizontal",
                         gap: 2
-                    }, e.map(((t, o) => y().createElement("div", {
+                    }, e.map(((t, o) => N().createElement("div", {
                         className: o === e.length - 1 ? "breadcrumb-tile-active breadcrumb-tile" : "breadcrumb-tile",
                         onClick: () => {
-                            "Notebook" === t.pageName ? ue.sendInteraction({
+                            "Notebook" === t.pageName ? ye.sendInteraction({
                                 click_type: "ON",
-                                signal_origin: Q.BREADCRUMB_TO_NOTEBOOK
-                            }) : "Cell" === t.pageName && ue.sendInteraction({
+                                signal_origin: re.BREADCRUMB_TO_NOTEBOOK
+                            }) : "Cell" === t.pageName && ye.sendInteraction({
                                 click_type: "ON",
-                                signal_origin: Q.BREADCRUMB_TO_CELL
-                            }), o !== e.length - 1 && pe(V(o))
+                                signal_origin: re.BREADCRUMB_TO_CELL
+                            }), o !== e.length - 1 && fe(W(o))
                         }
-                    }, t.pageName))), y().createElement("div", {
+                    }, t.pageName))), N().createElement("div", {
                         className: "breadcrumb-buttons-container"
-                    }, y().createElement(re.Button, {
-                        className: "breadcrumb-button",
+                    }, N().createElement(_e.Button, {
+                        className: "dashboard-button",
                         onClick: () => {
-                            ue.sendInteraction({
+                            ye.sendInteraction({
                                 click_type: "ON",
-                                signal_origin: Q.DASHBOARD_REFRESH_BUTTON
-                            }), pe(G())
+                                signal_origin: re.DASHBOARD_REFRESH_BUTTON
+                            }), fe(te())
                         }
-                    }, y().createElement(S.refreshIcon.react, {
-                        elementSize: "large",
-                        className: "labicon-logo"
+                    }, N().createElement(Ee.ArrowClockwise, {
+                        className: "dashboard-icon"
                     }))))
-                };
-            var _e = o(2535);
-            const be = X.dispatch,
-                we = () => y().createElement(re.DropdownButton, {
-                    id: "time-window-dropdown",
-                    title: y().createElement(_e.CalendarWeek, {
-                        className: "logo"
-                    }),
-                    variant: "outline-secondary",
-                    onSelect: e => {
-                        e && (ue.sendInteraction({
-                            click_type: "ON",
-                            signal_origin: Q.DASHBOARD_FILTER_TIME
-                        }), be(j(e)))
-                    },
-                    className: "custom-dropdown"
-                }, y().createElement(re.Dropdown.Header, null, "Data to keep"), y().createElement(re.Dropdown.Divider, null), y().createElement(re.Dropdown.Item, {
-                    eventKey: "60"
-                }, "Last minute"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "600"
-                }, "Last 10 minutes"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "3600"
-                }, "Last hour"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "86400"
-                }, "Last day"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "604800"
-                }, "Last week"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "2592000"
-                }, "Last month"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "15768000"
-                }, "Last 6 months"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "null"
-                }, "All")),
-                ve = ({
+                },
+                Oe = e => e.toLocaleString("sv-SE").slice(0, -3),
+                De = e => {
+                    const [t, o] = (0, D.useState)(e.startT1), [n, a] = (0, D.useState)(e.startT2), s = Oe(new Date), l = t => {
+                        o(t), e.t1Callback(t)
+                    }, r = t => {
+                        a(t), e.t2Callback(t)
+                    };
+                    return N().createElement("div", {
+                        className: "dashboard-export-dialog-container"
+                    }, N().createElement("p", null, "Select the time range of the data you want to export (the past week selected by default)."), N().createElement("div", {
+                        className: "dashboard-export-dialog-calendar-container"
+                    }, N().createElement("div", {
+                        className: "dashboard-export-dialog-calendar"
+                    }, N().createElement("p", null, "Start Date :"), N().createElement("input", {
+                        className: "dashboard-calendar-input",
+                        type: "datetime-local",
+                        value: Oe(t),
+                        onChange: e => (e => {
+                            const t = new Date(e);
+                            l(t), t >= n && r(t)
+                        })(e.target.value),
+                        max: Oe(n)
+                    })), N().createElement("div", {
+                        className: "dashboard-export-dialog-calendar"
+                    }, N().createElement("p", null, "End Date :"), N().createElement("input", {
+                        className: "dashboard-calendar-input",
+                        type: "datetime-local",
+                        value: Oe(n),
+                        onChange: e => (e => {
+                            const o = new Date(e);
+                            r(o), o <= t && l(o)
+                        })(e.target.value),
+                        max: s
+                    }))))
+                },
+                Ne = e => {
+                    const [t, o] = (0, D.useState)(!1);
+                    return N().createElement("div", {
+                        className: "dashboard-toc-download-button" + (t ? "-disabled" : ""),
+                        onClick: () => {
+                            t || (e => {
+                                let t = new Date,
+                                    n = new Date;
+                                n.setDate(t.getDate() - 7), (0, I.showDialog)({
+                                    title: "Download Notebook Data",
+                                    body: N().createElement(De, {
+                                        startT1: n,
+                                        startT2: t,
+                                        t1Callback: e => n = e,
+                                        t2Callback: e => t = e
+                                    }),
+                                    buttons: [{
+                                        accept: !0,
+                                        actions: [],
+                                        ariaLabel: "Export",
+                                        caption: "",
+                                        className: "",
+                                        displayType: "default",
+                                        iconClass: "",
+                                        iconLabel: "",
+                                        label: "Export"
+                                    }, I.Dialog.cancelButton()]
+                                }).then((a => {
+                                    a.button.accept && ((e, t, n) => {
+                                        o(!0);
+                                        let a = "";
+                                        E(`${r}/dashboard/${e}/download_csv?t1=${t.toISOString()}&t2=${n.toISOString()}`).then((e => {
+                                            var t;
+                                            if (e.ok) {
+                                                const o = e.headers.get("Content-Disposition");
+                                                return a = (null === (t = null == o ? void 0 : o.match(/filename=(.+)/)) || void 0 === t ? void 0 : t[1]) || "", e.blob()
+                                            }
+                                        })).then((e => {
+                                            if (e) {
+                                                const t = window.URL.createObjectURL(e),
+                                                    o = document.createElement("a");
+                                                o.href = t, o.download = a, document.body.appendChild(o), o.click(), o.remove()
+                                            }
+                                        })).finally((() => {
+                                            o(!1)
+                                        }))
+                                    })(e, n, t)
+                                }))
+                            })(e.notebookId)
+                        }
+                    }, N().createElement(x.downloadIcon.react, {
+                        className: "dashboard-toc-download-icon"
+                    }), "Export")
+                },
+                xe = se.dispatch,
+                Ie = [{
+                    value: 1,
+                    displayName: "All Data",
+                    disabledDatePicker: !0
+                }, {
+                    value: 2,
+                    displayName: "From t<sub>1</sub>",
+                    disabledDatePicker: !1
+                }],
+                Te = e => {
+                    const t = (0, be.useSelector)((e => e.commondashboard.dashboardQueryArgs)),
+                        o = () => {
+                            const o = t.t1ISOString[e.notebookId] ? 1 : 0;
+                            return Ie[o]
+                        },
+                        n = () => {
+                            const o = t.t1ISOString[e.notebookId];
+                            return o ? new Date(o) : new Date
+                        },
+                        a = () => void 0 === t.displayRealTime[e.notebookId] || t.displayRealTime[e.notebookId],
+                        [s, l] = (0, D.useState)(o()),
+                        [r, i] = (0, D.useState)(n()),
+                        [c, d] = (0, D.useState)(a),
+                        [h, u] = (0, D.useState)(!1),
+                        m = Oe(new Date),
+                        p = () => {
+                            h || (i(n()), l(o()), d(a())), u(!h)
+                        };
+                    return N().createElement(_e.Dropdown, {
+                        show: h,
+                        onToggle: p,
+                        className: "custom-dropdown"
+                    }, N().createElement(_e.Dropdown.Toggle, {
+                        className: "dashboard-button"
+                    }, N().createElement(Ee.CalendarWeek, {
+                        className: "dashboard-icon"
+                    })), N().createElement(_e.Dropdown.Menu, null, N().createElement(_e.Dropdown.Header, null, "Data Timeframe Selector"), N().createElement(_e.Dropdown.Divider, null), N().createElement("div", {
+                        className: "custom-dropdown-container custom-dropdown-item"
+                    }, N().createElement(_e.Form.Check, {
+                        id: "time-checkbox-include-all",
+                        type: "checkbox",
+                        label: "Only show active users",
+                        checked: c,
+                        onChange: e => d(e.target.checked)
+                    })), N().createElement(_e.Dropdown.Divider, null), N().createElement("div", {
+                        className: "dashboard-calendar-container"
+                    }, N().createElement("div", {
+                        className: "cell-radio-container"
+                    }, N().createElement(_e.ButtonGroup, {
+                        size: "sm"
+                    }, Ie.map(((e, t) => N().createElement(_e.ToggleButton, {
+                        key: `calendar-filter-${t}`,
+                        id: `calendar-filter-${t}`,
+                        type: "radio",
+                        variant: "outline-primary",
+                        name: "radio",
+                        value: e.value,
+                        checked: s.value === e.value,
+                        onChange: e => {
+                            l(Ie[Number(e.currentTarget.value) - 1])
+                        }
+                    }, N().createElement("span", {
+                        dangerouslySetInnerHTML: {
+                            __html: e.displayName
+                        }
+                    }))))))), N().createElement("div", {
+                        className: "dashboard-calendar-container"
+                    }, N().createElement("div", {
+                        className: "dashboard-calendar-input-wrapper " + (s.disabledDatePicker ? "disabled" : "")
+                    }, N().createElement("div", null, "t", N().createElement("sub", null, "1")), N().createElement("input", {
+                        className: "dashboard-calendar-input",
+                        type: "datetime-local",
+                        value: Oe(r),
+                        onChange: e => i(new Date(e.target.value)),
+                        max: m
+                    }))), N().createElement("div", {
+                        className: "dashboard-calendar-button-container"
+                    }, N().createElement(_e.Button, {
+                        variant: "secondary",
+                        onClick: () => {
+                            p()
+                        }
+                    }, "Cancel"), N().createElement(_e.Button, {
+                        variant: "primary",
+                        onClick: () => {
+                            xe(q({
+                                notebookId: e.notebookId,
+                                t1ISOString: s.disabledDatePicker ? null : r.toISOString()
+                            })), xe(Z({
+                                notebookId: e.notebookId,
+                                displayRealTime: c
+                            })), ye.sendInteraction({
+                                click_type: 1 === s.value ? "OFF" : "ON",
+                                signal_origin: re.DASHBOARD_FILTER_TIME
+                            }), p()
+                        }
+                    }, "Ok"))))
+                },
+                Re = ({
                     PassedComponent: e,
                     title: t
-                }) => y().createElement(re.Row, {
+                }) => N().createElement(_e.Row, {
                     className: "mb-4"
-                }, y().createElement(re.Card, {
+                }, N().createElement(_e.Card, {
                     className: "chart-card"
-                }, y().createElement(re.Card.Title, {
+                }, N().createElement(_e.Card.Title, {
                     className: "chart-card-title"
-                }, t), y().createElement(re.Card.Body, {
+                }, t), N().createElement(_e.Card.Body, {
                     className: "chart-card-body"
                 }, e)));
-            var Ce = o(7885);
-            const ke = {
+            var Ae = o(7885);
+            const Le = {
                     maintainAspectRatio: !1,
                     plugins: {
                         legend: {
                             labels: {
                                 color: "#969696"
                             }
                         }
@@ -600,15 +837,15 @@
                                 display: !0,
                                 text: "Cumulated total across all users",
                                 color: "#969696"
                             }
                         }
                     }
                 },
-                Ee = {
+                Me = {
                     maintainAspectRatio: !1,
                     plugins: {
                         legend: {
                             display: !0,
                             labels: {
                                 usePointStyle: !0,
                                 color: "#969696"
@@ -647,566 +884,629 @@
                                 display: !0,
                                 text: "Time spent on a cell [s]",
                                 color: "#969696"
                             }
                         }
                     }
                 },
-                fe = e => {
-                    const [t, o] = (0, f.useState)({
+                Be = e => {
+                    const [t, o] = (0, D.useState)({
                         labels: [],
                         datasets: []
-                    }), n = (0, ie.useSelector)((e => e.commondashboard.displayRealTime));
-                    return (0, f.useEffect)((() => {
-                        v(`${i}/dashboard/${e.notebookId}/user_code_execution?timeWindow=${e.timeWindow}&displayRealTime=${n}`).then((e => e.json())).then((t => {
-                            var n;
-                            const a = (null === (n = e.notebookCells) || void 0 === n ? void 0 : n.filter((e => "code" === e.cellType))) || [],
-                                s = {
+                    }), n = (0, be.useSelector)((e => e.commondashboard.dashboardQueryArgs)), a = (0, be.useSelector)((e => e.commondashboard.refreshBoolean)), s = (0, be.useSelector)((e => e.commondashboard.notebookCells));
+                    return (0, D.useEffect)((() => {
+                        E(`${r}/dashboard/${e.notebookId}/user_code_execution?${C(n,e.notebookId)}`).then((e => e.json())).then((e => {
+                            const t = (null == s ? void 0 : s.filter((e => "code" === e.cellType))) || [],
+                                n = {
                                     labels: Array.from({
-                                        length: a.length
+                                        length: t.length
                                     }, ((e, t) => t + 1)),
                                     datasets: [{
                                         label: "clicks",
-                                        data: Array(a.length).fill(null),
+                                        data: Array(t.length).fill(null),
                                         backgroundColor: "rgba(51, 187, 238, 0.3)",
                                         borderColor: "rgba(51, 187, 238, 0.3)",
                                         borderWidth: 1
                                     }, {
                                         label: "executions",
-                                        data: Array(a.length).fill(null),
+                                        data: Array(t.length).fill(null),
                                         backgroundColor: "rgba(0, 119, 187, 0.6)",
                                         borderColor: "rgba(0, 119, 187, 0.6)",
                                         borderWidth: 1
                                     }, {
                                         label: "executions without errors",
-                                        data: Array(a.length).fill(null),
+                                        data: Array(t.length).fill(null),
                                         backgroundColor: "rgba(0, 153, 136, 0.9)",
                                         borderColor: "rgba(0, 153, 136, 0.9)",
                                         borderWidth: 1
                                     }]
                                 };
-                            a.forEach(((e, o) => {
-                                const n = t.find((t => t.cell === e.id));
-                                n && (s.datasets[0].data[o] = parseFloat(n.cell_click_pct), s.datasets[1].data[o] = parseFloat(n.code_exec_pct), s.datasets[2].data[o] = parseFloat(n.code_exec_ok_pct))
-                            })), o(s)
+                            t.forEach(((t, o) => {
+                                const a = e.find((e => e.cell === t.id));
+                                a && (n.datasets[0].data[o] = parseFloat(a.cell_click_pct), n.datasets[1].data[o] = parseFloat(a.code_exec_pct), n.datasets[2].data[o] = parseFloat(a.code_exec_ok_pct))
+                            })), o(n)
                         }))
-                    }), [e.timeWindow, e.refreshRequired]), y().createElement(ve, {
-                        PassedComponent: y().createElement(Ce.Bar, {
+                    }), [n, a]), N().createElement(Re, {
+                        PassedComponent: N().createElement(Ae.Bar, {
                             data: t,
-                            options: ke
+                            options: Le
                         }),
                         title: "Code cell execution across users"
                     })
                 },
-                ye = e => {
-                    const [t, o] = (0, f.useState)({
+                He = e => {
+                    const [t, o] = (0, D.useState)({
                         labels: [],
                         datasets: []
-                    }), n = (0, ie.useSelector)((e => e.commondashboard.displayRealTime));
-                    return (0, f.useEffect)((() => {
-                        v(`${i}/dashboard/${e.notebookId}/user_cell_time?timeWindow=${e.timeWindow}&displayRealTime=${n}`).then((e => e.json())).then((t => {
-                            var n;
-                            const a = {
-                                labels: e.notebookCells ? Array.from({
-                                    length: e.notebookCells.length
+                    }), n = (0, be.useSelector)((e => e.commondashboard.dashboardQueryArgs)), a = (0, be.useSelector)((e => e.commondashboard.refreshBoolean)), s = (0, be.useSelector)((e => e.commondashboard.notebookCells));
+                    return (0, D.useEffect)((() => {
+                        E(`${r}/dashboard/${e.notebookId}/user_cell_time?${C(n,e.notebookId)}`).then((e => e.json())).then((e => {
+                            const t = {
+                                labels: s ? Array.from({
+                                    length: s.length
                                 }, ((e, t) => t + 1)) : [],
                                 datasets: [{
                                     label: "time spent on a cell by a user",
-                                    data: (null === (n = e.notebookCells) || void 0 === n ? void 0 : n.flatMap(((e, o) => {
-                                        const n = t.find((t => t.cell === e.id));
+                                    data: (null == s ? void 0 : s.flatMap(((t, o) => {
+                                        const n = e.find((e => e.cell === t.id));
                                         return n ? n.durations.map((e => ({
                                             x: o + 1,
                                             y: e
                                         }))) : []
                                     }))) || [],
                                     backgroundColor: "rgba(54, 162, 235, 0.2)",
                                     borderColor: "rgba(54, 162, 235, 1)",
                                     borderWidth: 1,
                                     pointRadius: 1
                                 }]
                             };
-                            o(a)
+                            o(t)
                         }))
-                    }), [e.timeWindow, e.refreshRequired]), y().createElement(ve, {
-                        PassedComponent: y().createElement(Ce.Scatter, {
+                    }), [n, a]), N().createElement(Re, {
+                        PassedComponent: N().createElement(Ae.Scatter, {
                             data: t,
-                            options: Ee
+                            options: Me
                         }),
                         title: "Amount of time spent on each cell"
                     })
                 },
-                Se = e => {
-                    const t = (0, ie.useSelector)((e => e.commondashboard.timeWindow)),
-                        o = (0, ie.useSelector)((e => e.commondashboard.refreshBoolean)),
-                        n = (0, ie.useSelector)((e => e.commondashboard.notebookCells));
-                    return y().createElement(y().Fragment, null, y().createElement("div", {
-                        className: "dashboard-title-container"
-                    }, y().createElement("div", {
-                        className: "dashboard-title-text"
-                    }, e.notebookName), y().createElement("div", {
-                        className: "dashboard-dropdown-container"
-                    }, y().createElement(we, null))), y().createElement(re.Row, null, y().createElement(re.Col, null, y().createElement(fe, {
-                        notebookId: e.notebookId,
-                        timeWindow: t,
-                        refreshRequired: o,
-                        notebookCells: n
-                    }), y().createElement(ye, {
-                        notebookId: e.notebookId,
-                        timeWindow: t,
-                        refreshRequired: o,
-                        notebookCells: n
-                    }))))
-                };
-            var Oe = o(3074);
-            const De = new s.RenderMimeRegistry({
+                $e = se.dispatch,
+                Fe = e => {
+                    const [t, o] = (0, D.useState)(!1), [n, a] = (0, D.useState)([]), s = (0, be.useSelector)((t => t.commondashboard.dashboardQueryArgs.selectedGroups[e.notebookId])), [l, i] = (0, D.useState)(void 0 === s || 0 === s.length);
+                    (0, D.useEffect)((() => {
+                        E(`${r}/dashboard/${e.notebookId}/getgroups`).then((e => e.json())).then((e => {
+                            const t = e.map((e => ({
+                                name: e,
+                                checked: null == s ? void 0 : s.includes(e)
+                            }))).sort(((e, t) => e.checked !== t.checked ? t.checked ? 1 : -1 : e.name.localeCompare(t.name)));
+                            a(t)
+                        }))
+                    }), []);
+                    const c = () => {
+                        t || (() => {
+                            i(void 0 === s || 0 === s.length);
+                            const e = n.map((e => ({
+                                name: e.name,
+                                checked: null == s ? void 0 : s.includes(e.name)
+                            }))).sort(((e, t) => e.checked !== t.checked ? t.checked ? 1 : -1 : e.name.localeCompare(t.name)));
+                            a(e)
+                        })(), o(!t)
+                    };
+                    return N().createElement(_e.Dropdown, {
+                        id: "group-dropdown",
+                        className: "custom-dropdown",
+                        show: t,
+                        onToggle: c
+                    }, N().createElement(_e.Dropdown.Toggle, {
+                        className: "dashboard-button"
+                    }, N().createElement(Ee.PeopleFill, {
+                        className: "dashboard-icon"
+                    })), N().createElement(_e.Dropdown.Menu, null, N().createElement(_e.Dropdown.Header, null, "Filter by group of users"), N().createElement(_e.Dropdown.Divider, null), N().createElement("div", {
+                        className: "custom-dropdown-container custom-dropdown-item"
+                    }, N().createElement(_e.Form.Check, {
+                        id: "group-checkbox-include-all",
+                        type: "checkbox",
+                        label: "Include all users",
+                        checked: l,
+                        onChange: e => i(e.target.checked)
+                    })), N().createElement(_e.Dropdown.Divider, null), N().createElement("div", {
+                        className: "group-dropdown-scroll " + (l ? "disabled" : "")
+                    }, n.length > 0 ? n.map(((e, t) => N().createElement("div", {
+                        className: "custom-dropdown-item " + (l ? "disabled" : "")
+                    }, N().createElement(_e.Form.Check, {
+                        id: `group-checkbox-${t}`,
+                        type: "checkbox",
+                        disabled: !!l || void 0,
+                        label: e.name,
+                        title: e.name,
+                        checked: e.checked,
+                        onChange: () => (e => {
+                            a((t => {
+                                const o = [...t];
+                                return o[e] = {
+                                    ...o[e],
+                                    checked: !o[e].checked
+                                }, o
+                            }))
+                        })(t)
+                    })))) : N().createElement(_e.Dropdown.Item, {
+                        disabled: !0
+                    }, "No groups available")), N().createElement("div", {
+                        className: "dashboard-calendar-button-container"
+                    }, N().createElement(_e.Button, {
+                        variant: "secondary",
+                        onClick: () => {
+                            c()
+                        }
+                    }, "Cancel"), N().createElement(_e.Button, {
+                        variant: "primary",
+                        onClick: () => {
+                            let t;
+                            t = l ? [] : n.filter((e => !0 === e.checked)).map((e => e.name)), $e(X({
+                                notebookId: e.notebookId,
+                                groups: t
+                            })), c()
+                        }
+                    }, "Ok"))))
+                },
+                Ue = e => N().createElement(N().Fragment, null, N().createElement("div", {
+                    className: "dashboard-title-container"
+                }, N().createElement("div", {
+                    className: "dashboard-title-text"
+                }, e.notebookName), N().createElement("div", {
+                    className: "dashboard-dropdown-container"
+                }, N().createElement(Fe, {
+                    notebookId: e.notebookId
+                }), N().createElement(Te, {
+                    notebookId: e.notebookId
+                }))), N().createElement(_e.Row, null, N().createElement(_e.Col, null, N().createElement(Be, {
+                    notebookId: e.notebookId
+                }), N().createElement(He, {
+                    notebookId: e.notebookId
+                }))));
+            var Ve = o(1778);
+            const Pe = new s.RenderMimeRegistry({
                     initialFactories: s.standardRendererFactories
                 }),
-                xe = ({
+                ze = ({
                     cell_output_model: e
                 }) => {
-                    const t = (0, f.useRef)(null),
-                        o = new Oe.OutputAreaModel;
-                    return (0, f.useEffect)((() => {
+                    const t = (0, D.useRef)(null),
+                        o = new Ve.OutputAreaModel;
+                    return (0, D.useEffect)((() => {
                         o.clear(), o.fromJSON(e);
                         const n = t.current;
                         if (n) {
                             n.innerHTML = "";
                             for (let e = 0; e < o.length; ++e) {
                                 const t = o.get(e),
-                                    a = De.preferredMimeType(t.data);
+                                    a = Pe.preferredMimeType(t.data);
                                 if (a) {
-                                    const e = De.createRenderer(a);
+                                    const e = Pe.createRenderer(a);
                                     e.renderModel(t), n.appendChild(e.node)
                                 }
                             }
                         }
-                    }), [e]), y().createElement("div", {
+                    }), [e]), N().createElement("div", {
                         ref: t,
                         className: "cell-content-container"
                     })
                 };
-            var Ne = o(7388),
-                Te = o(1121);
-            const Re = ({
+            var je = o(7777),
+                We = o(3471);
+            const Ge = ({
                     cell_input: e,
                     language_mimetype: t,
                     className: o
                 }) => {
-                    const n = (0, f.useRef)(null);
-                    return (0, f.useEffect)((() => {
+                    const n = (0, D.useRef)(null);
+                    return (0, D.useEffect)((() => {
                         const o = n.current;
                         if (o) {
                             o.innerHTML = "";
-                            const n = new Te.CodeEditor.Model;
+                            const n = new We.CodeEditor.Model;
                             n.mimeType = t, n.sharedModel.setSource(e);
-                            const a = new Ne.CodeMirrorEditor({
+                            const a = new je.CodeMirrorEditor({
                                     host: o,
                                     model: n,
                                     ...w.getCodeMirrorOptionsComp()
                                 }),
                                 s = w.observeEditorVisibility(a);
                             return s && s.observe(o), () => {
                                 s && s.disconnect()
                             }
                         }
-                    }), [e, t]), y().createElement("div", {
+                    }), [e, t]), N().createElement("div", {
                         ref: n,
                         className: o
                     })
                 },
-                Ie = ({
-                    setOrderBy: e
-                }) => y().createElement(re.DropdownButton, {
-                    id: "order-by-dropdown",
-                    title: y().createElement(_e.SortUp, {
-                        className: "logo"
-                    }),
-                    variant: "outline-secondary",
-                    onSelect: t => {
-                        t && (ue.sendInteraction({
-                            click_type: "ON",
-                            signal_origin: Q.CELL_DASHBOARD_FILTER_SORT
-                        }), e(t))
-                    },
-                    className: "custom-dropdown"
-                }, y().createElement(re.Dropdown.Header, null, "Sort cells by"), y().createElement(re.Dropdown.Divider, null), y().createElement(re.Dropdown.Item, {
-                    eventKey: "timeDesc"
-                }, "Time (most recent 1st)"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "timeAsc"
-                }, "Time (oldest 1st)"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "inputAsc"
-                }, "Input (shortest 1st)"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "inputDesc"
-                }, "Input (longest 1st)"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "outputAsc"
-                }, "Output (shortest 1st)"), y().createElement(re.Dropdown.Item, {
-                    eventKey: "outputDesc"
-                }, "Output (longest 1st)"));
-            var Le = o(2779);
-            const Ae = e => {
-                    const [t, o] = (0, f.useState)(null);
-                    return (0, f.useEffect)((() => {
+                Je = se.dispatch,
+                Ke = e => {
+                    const t = (0, be.useSelector)((t => t.commondashboard.sortBy[e.notebookId]));
+                    return N().createElement(_e.Dropdown, {
+                        id: "order-by-dropdown",
+                        onSelect: t => {
+                            t && (ye.sendInteraction({
+                                click_type: "ON",
+                                signal_origin: re.CELL_DASHBOARD_FILTER_SORT
+                            }), Je(Y({
+                                notebookId: e.notebookId,
+                                sortCriterion: t
+                            })))
+                        },
+                        className: "custom-dropdown"
+                    }, N().createElement(_e.Dropdown.Toggle, {
+                        className: "dashboard-button"
+                    }, N().createElement(Ee.SortUp, {
+                        className: "dashboard-icon"
+                    })), N().createElement(_e.Dropdown.Menu, null, N().createElement(_e.Dropdown.Header, null, "Sort cells by"), N().createElement(_e.Dropdown.Divider, null), v.map(((e, o) => N().createElement(_e.Dropdown.Item, {
+                        id: `sort-item-${o}`,
+                        eventKey: e.key,
+                        className: t && t === e.key ? "highlighted" : ""
+                    }, e.label)))))
+                };
+            var Qe = o(2779);
+            const qe = e => {
+                    const [t, o] = (0, D.useState)(null);
+                    return (0, D.useEffect)((() => {
                         (() => {
-                            const t = Le.marked.parser(Le.marked.lexer(e.markdownContent));
+                            const t = Qe.marked.parser(Qe.marked.lexer(e.markdownContent));
                             o(e.sanitizer.sanitize(t))
                         })()
-                    }), [e.markdownContent]), y().createElement("div", {
+                    }), [e.markdownContent]), N().createElement("div", {
                         className: "cell-content-container"
-                    }, t && y().createElement("div", {
+                    }, t && N().createElement("div", {
                         className: "jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput",
                         dangerouslySetInnerHTML: {
                             __html: t
                         }
                     }))
                 },
-                Me = e => {
-                    const t = (0, f.useRef)([]),
-                        [o, n] = (0, f.useState)([]);
+                Xe = e => N().createElement(_e.Col, {
+                    md: 12
+                }, N().createElement(_e.Card, {
+                    className: "cell-card"
+                }, N().createElement(_e.Card.Body, {
+                    style: {
+                        gap: "10px"
+                    }
+                }, N().createElement(_e.Row, {
+                    className: "cell-card-wrapper"
+                }, N().createElement(_e.Col, {
+                    md: 12,
+                    className: "cell-user-title"
+                }, N().createElement(_e.Card.Text, {
+                    title: e.value.user_id || void 0
+                }, "User ", e.value.user_id ? e.value.user_id.length > 8 ? `${e.value.user_id.substring(0,8)}...` : e.value.user_id : `${e.index+1}`)), N().createElement(_e.Col, {
+                    md: 12
+                }, e.ExecutionContent), (() => {
+                    if (e.value.t_finish) {
+                        const t = new Date(e.value.t_finish),
+                            o = `Executed at ${t.getHours().toString().padStart(2,"0")}:${t.getMinutes().toString().padStart(2,"0")}, ${t.getDate().toString().padStart(2,"0")}/${(t.getMonth()+1).toString().padStart(2,"0")}/${t.getFullYear().toString().slice(-2)}`;
+                        return N().createElement(_e.Col, {
+                            md: 12,
+                            className: "cell-execution-displayed-time"
+                        }, o)
+                    }
+                    return null
+                })())))),
+                Ze = e => {
+                    const t = (0, D.useRef)([]),
+                        [o, n] = (0, D.useState)([]);
                     let a = !1;
-                    const s = (0, ie.useSelector)((e => e.sidedashboard.navigationState)),
-                        l = (0, ie.useSelector)((e => e.commondashboard.timeWindow)),
-                        r = (0, ie.useSelector)((e => e.commondashboard.refreshBoolean)),
-                        c = (0, ie.useSelector)((e => e.commondashboard.displayRealTime)),
-                        [d, h] = (0, f.useState)(!0),
-                        [m, u] = (0, f.useState)(!0),
-                        [p, g] = (0, f.useState)(1),
-                        [_, b] = ((e = 800) => {
-                            const [t, o] = (0, f.useState)(""), [n, a] = (0, f.useState)("");
-                            return (0, f.useEffect)((() => {
+                    const s = (0, be.useSelector)((e => e.sidedashboard.navigationState)),
+                        l = (0, be.useSelector)((e => e.commondashboard.refreshBoolean)),
+                        i = (0, be.useSelector)((e => e.commondashboard.dashboardQueryArgs)),
+                        c = (0, be.useSelector)((e => e.commondashboard.sortBy)),
+                        [d, h] = (0, D.useState)(!0),
+                        [u, m] = (0, D.useState)(!0),
+                        [p, g] = (0, D.useState)(1),
+                        [b, _] = ((e = 800) => {
+                            const [t, o] = (0, D.useState)(""), [n, a] = (0, D.useState)("");
+                            return (0, D.useEffect)((() => {
                                 const t = setTimeout((() => o(n)), e);
                                 return () => clearTimeout(t)
                             }), [n, e]), [t, a]
                         })(),
-                        w = [{
+                        k = [{
                             name: "All",
                             value: 1,
                             status: "all"
                         }, {
                             name: "Success",
                             value: 2,
                             status: "ok"
                         }, {
                             name: "Error",
                             value: 3,
                             status: "error"
                         }],
-                        C = w.map((e => e.status)),
-                        [k, E] = (0, f.useState)("timeDesc"),
-                        S = e => {
-                            const t = _.toLowerCase();
-                            t.length > 0 && (e = e.filter((e => {
-                                var o;
-                                return (null === (o = e.cell_input) || void 0 === o ? void 0 : o.toLowerCase().includes(t)) || e.cell_output_model && JSON.stringify(e.cell_output_model).toLowerCase().includes(t)
-                            }))), e.sort(((e, t) => {
-                                switch (k) {
-                                    case "timeDesc":
-                                        return new Date(e.t_finish) < new Date(t.t_finish) ? 1 : -1;
-                                    case "timeAsc":
-                                        return new Date(e.t_finish) > new Date(t.t_finish) ? 1 : -1;
-                                    case "inputAsc":
-                                        return e.cell_input.length - t.cell_input.length;
-                                    case "inputDesc":
-                                        return t.cell_input.length - e.cell_input.length;
-                                    case "outputAsc":
-                                        return e.cell_output_length - t.cell_output_length;
-                                    case "outputDesc":
-                                        return t.cell_output_length - e.cell_output_length;
-                                    default:
-                                        return 0
-                                }
-                            })), n(e)
+                        w = k.map((e => e.status)),
+                        y = t => {
+                            const o = b.toLowerCase();
+                            o.length > 0 && (t = t.filter((e => {
+                                var t;
+                                return (null === (t = e.cell_input) || void 0 === t ? void 0 : t.toLowerCase().includes(o)) || e.cell_output_model && JSON.stringify(e.cell_output_model).toLowerCase().includes(o)
+                            })));
+                            const a = c[e.notebookId] || "timeDesc",
+                                s = v.find((e => e.key === a));
+                            s && t.sort(s.method), n(t)
                         },
-                        O = s[s.length - 1].content;
-                    return (0, f.useEffect)((() => {
-                        a = !0, v(`${i}/dashboard/${e.notebookId}/cell/${O.cellId}?timeWindow=${l}&displayRealTime=${c}`).then((e => e.json())).then((e => {
-                            t.current = e, S(e), a = !1
+                        f = s[s.length - 1].content;
+                    return (0, D.useEffect)((() => {
+                        a = !0, E(`${r}/dashboard/${e.notebookId}/cell/${f.cellId}?${C(i,e.notebookId)}`).then((e => e.json())).then((e => {
+                            t.current = e, y(e), a = !1
                         }))
-                    }), [s, l, r]), (0, f.useEffect)((() => {
+                    }), [s, i, l]), (0, D.useEffect)((() => {
                         if (!a) {
                             const e = [...t.current];
-                            S(e)
+                            y(e)
                         }
-                    }), [k, _]), y().createElement(y().Fragment, null, y().createElement("div", {
+                    }), [c, b]), N().createElement(N().Fragment, null, N().createElement("div", {
                         className: "dashboard-title-container"
-                    }, y().createElement("div", {
+                    }, N().createElement("div", {
                         className: "dashboard-title-text"
-                    }, "Cell (", O.cellId, ")"), y().createElement("div", {
+                    }, "Cell (", f.cellId, ")"), N().createElement("div", {
                         className: "dashboard-dropdown-container"
-                    }, y().createElement(Ie, {
-                        setOrderBy: E
-                    }), y().createElement(we, null))), y().createElement(re.Form, {
-                        className: "cell-filter-container"
-                    }, y().createElement("div", {
+                    }, N().createElement(Ke, {
+                        notebookId: e.notebookId
+                    }), N().createElement(Fe, {
+                        notebookId: e.notebookId
+                    }), N().createElement(Te, {
+                        notebookId: e.notebookId
+                    }))), N().createElement(_e.Form, {
+                        className: "cell-filter-container",
+                        onSubmit: e => e.preventDefault()
+                    }, N().createElement("div", {
                         className: "cell-radio-container"
-                    }, y().createElement(re.ButtonGroup, {
+                    }, N().createElement(_e.ButtonGroup, {
                         size: "sm"
-                    }, y().createElement(re.ToggleButton, {
+                    }, N().createElement(_e.ToggleButton, {
                         style: {
                             marginRight: "3px"
                         },
                         key: "0",
                         id: "code-checkbox",
                         type: "radio",
                         variant: "outline-primary",
                         value: "Code",
                         checked: d,
                         onClick: e => {
-                            d && !m ? e.preventDefault() : (ue.sendInteraction({
+                            d && !u ? e.preventDefault() : (ye.sendInteraction({
                                 click_type: d ? "OFF" : "ON",
-                                signal_origin: Q.CELL_DASHBOARD_FILTER_CODE_INPUT
+                                signal_origin: re.CELL_DASHBOARD_FILTER_CODE_INPUT
                             }), h(!d))
                         }
-                    }, "Code"), y().createElement(re.ToggleButton, {
+                    }, "Code"), N().createElement(_e.ToggleButton, {
                         key: "1",
                         id: "output-checkbox",
                         type: "radio",
                         variant: "outline-primary",
                         value: "Output",
-                        checked: m,
+                        checked: u,
                         onClick: e => {
-                            !d && m ? e.preventDefault() : (ue.sendInteraction({
-                                click_type: m ? "OFF" : "ON",
-                                signal_origin: Q.CELL_DASHBOARD_FILTER_CODE_OUTPUT
-                            }), u(!m))
+                            !d && u ? e.preventDefault() : (ye.sendInteraction({
+                                click_type: u ? "OFF" : "ON",
+                                signal_origin: re.CELL_DASHBOARD_FILTER_CODE_OUTPUT
+                            }), m(!u))
                         }
-                    }, "Output"))), y().createElement("div", {
+                    }, "Output"))), N().createElement("div", {
                         className: "cell-radio-container"
-                    }, y().createElement(re.ButtonGroup, {
+                    }, N().createElement(_e.ButtonGroup, {
                         size: "sm"
-                    }, w.map(((e, t) => y().createElement(re.ToggleButton, {
+                    }, k.map(((e, t) => N().createElement(_e.ToggleButton, {
                         key: t,
                         id: `filter-${t}`,
                         type: "radio",
                         variant: "outline-primary",
                         name: "radio",
                         value: e.value,
                         checked: p === e.value,
                         onChange: e => {
-                            ue.sendInteraction({
+                            ye.sendInteraction({
                                 click_type: "ON",
-                                signal_origin: Q.CELL_DASHBOARD_FILTER_EXECUTION
+                                signal_origin: re.CELL_DASHBOARD_FILTER_EXECUTION
                             }), g(Number(e.currentTarget.value))
                         }
-                    }, e.name))))), y().createElement(re.Form.Control, {
+                    }, e.name))))), N().createElement(_e.Form.Control, {
                         size: "sm",
                         type: "text",
                         placeholder: "Type text to filter...",
-                        onChange: e => b(e.target.value)
-                    })), y().createElement(y().Fragment, null, o.map(((t, o) => y().createElement(re.Row, {
+                        onChange: e => _(e.target.value)
+                    })), N().createElement(N().Fragment, null, o.map(((t, o) => N().createElement(_e.Row, {
                         key: o
-                    }, "MarkdownExecution" === t.cell_type && ["all", "ok"].includes(C[p - 1]) ? y().createElement(re.Col, {
-                        md: 12
-                    }, y().createElement(re.Card, {
-                        className: "cell-card"
-                    }, y().createElement(re.Card.Body, {
-                        style: {
-                            gap: "10px"
-                        }
-                    }, y().createElement(re.Row, {
-                        className: "cell-card-wrapper"
-                    }, y().createElement(re.Col, {
-                        md: 12,
-                        className: "cell-user-title"
-                    }, y().createElement(re.Card.Text, null, "User ", o + 1)), y().createElement(re.Col, {
-                        md: 12
-                    }, y().createElement(Ae, {
-                        markdownContent: t.cell_input,
-                        sanitizer: e.sanitizer
-                    })))))) : y().createElement(y().Fragment, null, (1 === p || C[p - 1] === t.status) && y().createElement(re.Col, {
-                        md: 12
-                    }, y().createElement(re.Card, {
-                        className: "cell-card"
-                    }, y().createElement(re.Card.Body, {
-                        style: {
-                            gap: "10px"
-                        }
-                    }, y().createElement(re.Row, {
-                        className: "cell-card-wrapper"
-                    }, y().createElement(re.Col, {
-                        md: 12,
-                        className: "cell-user-title"
-                    }, y().createElement(re.Card.Text, null, "User ", o + 1)), y().createElement(re.Col, {
-                        md: 12
-                    }, d && y().createElement(Re, {
-                        cell_input: t.cell_input,
-                        language_mimetype: t.language_mimetype,
-                        className: "cell-content-container"
-                    }), d && m && t.cell_output_model.length > 0 && y().createElement("br", null), m && t.cell_output_model.length > 0 && y().createElement(xe, {
-                        cell_output_model: t.cell_output_model
-                    }))))))))))))
+                    }, "MarkdownExecution" === t.cell_type && ["all", "ok"].includes(w[p - 1]) ? N().createElement(Xe, {
+                        value: t,
+                        index: o,
+                        ExecutionContent: N().createElement(qe, {
+                            markdownContent: t.cell_input,
+                            sanitizer: e.sanitizer
+                        })
+                    }) : N().createElement(N().Fragment, null, (1 === p || w[p - 1] === t.status) && N().createElement(Xe, {
+                        value: t,
+                        index: o,
+                        ExecutionContent: N().createElement(N().Fragment, null, d && N().createElement(Ge, {
+                            cell_input: t.cell_input,
+                            language_mimetype: t.language_mimetype,
+                            className: "cell-content-container"
+                        }), d && u && t.cell_output_model.length > 0 && N().createElement("br", null), u && t.cell_output_model.length > 0 && N().createElement(ze, {
+                            cell_output_model: t.cell_output_model
+                        }))
+                    })))))))
                 };
-            var Be = o(8352);
-            Be.Chart.register(...Be.registerables);
-            const He = e => {
-                const t = (0, ie.useSelector)((e => e.sidedashboard.navigationState));
-                return y().createElement("div", {
+            var Ye = o(8352);
+            Ye.Chart.register(...Ye.registerables);
+            const et = e => {
+                const t = (0, be.useSelector)((e => e.sidedashboard.navigationState));
+                return N().createElement("div", {
                     className: "page-container"
-                }, y().createElement(ge, null), (() => {
+                }, N().createElement(Se, null), (() => {
                     switch (t[t.length - 1].pageName) {
                         case "Notebook":
-                            return y().createElement(Se, {
+                            return N().createElement(Ue, {
                                 notebookId: e.notebookId,
                                 notebookName: e.notebookName
                             });
                         case "Cell":
-                            return y().createElement(Me, {
+                            return N().createElement(Ze, {
                                 notebookId: e.notebookId,
                                 sanitizer: e.sanitizer
                             });
                         default:
                             return null
                     }
                 })())
             };
-            class $e extends me {
+            class tt extends Ce {
                 constructor(e, t) {
-                    super(e), this.addClass("dashboard-react-widget"), this.title.caption = "Side Dashboard", this.title.icon = x, this.id = "side-dashboard", this.node.setAttribute("role", "region"), this.node.setAttribute("aria-label", "Side dashboard section"), this._sanitizer = t
+                    super(e), this.addClass("dashboard-react-widget"), this.title.caption = "Side Dashboard", this.title.icon = R, this.id = "side-dashboard", this.node.setAttribute("role", "region"), this.node.setAttribute("aria-label", "Side dashboard section"), this._sanitizer = t
                 }
                 onBeforeShow(e) {
-                    ue.sendInteraction({
+                    ye.sendInteraction({
                         click_type: "ON",
-                        signal_origin: Q.RIGHT_DASHBOARD_SHOW_HIDE
+                        signal_origin: re.RIGHT_DASHBOARD_SHOW_HIDE
                     })
                 }
                 onBeforeHide(e) {
-                    ue.sendInteraction({
+                    ye.sendInteraction({
                         click_type: "OFF",
-                        signal_origin: Q.RIGHT_DASHBOARD_SHOW_HIDE
+                        signal_origin: re.RIGHT_DASHBOARD_SHOW_HIDE
                     })
                 }
                 computeComponentToRender() {
                     const e = this._panelManager.panel,
                         t = this._panelManager.validityChecks.tag;
-                    return e && t ? f.createElement(He, {
+                    return e && t ? D.createElement(et, {
                         notebookId: t,
                         notebookName: e.sessionContext.name,
                         sanitizer: this._sanitizer
-                    }) : f.createElement(f.Fragment, null)
+                    }) : D.createElement(D.Fragment, null)
                 }
             }
-            const Ue = (e, t) => {
+            const ot = (e, t) => {
                     const o = 3 * e / t + .1;
                     return Math.min(1, o)
                 },
-                Fe = ({
+                nt = ({
                     data: e,
                     cellId: t,
                     commands: o
-                }) => y().createElement(y().Fragment, null, e && e[0] && e[1] ? y().createElement("div", {
+                }) => N().createElement(N().Fragment, null, e && e[0] && e[1] ? N().createElement("div", {
                     onClick: e => {
-                        e.preventDefault(), o.execute(u.dashboardOpenVisu, {
+                        e.preventDefault(), o.execute(p.dashboardOpenVisu, {
                             from: "Toc",
                             cell_id: t
                         })
                     },
                     className: "dashboard-toc-react-component",
                     style: {
-                        backgroundColor: `rgba(25, 118, 210, ${Ue(e[0],e[1])})`
+                        backgroundColor: `rgba(25, 118, 210, ${ot(e[0],e[1])})`
                     }
-                }, y().createElement("span", {
+                }, N().createElement("span", {
                     className: "dashboard-toc-react-text"
-                }, e[0] + "/" + e[1])) : y().createElement("div", {
+                }, e[0] + "/" + e[1])) : N().createElement("div", {
                     className: "dashboard-toc-react-component"
                 }));
-            class Ve extends y().Component {
+            class at extends N().Component {
                 render() {
                     const {
                         panel: e,
                         heading: t,
                         headings: o,
                         addReactComponent: n,
                         isFirstCellOccurrence: a,
                         tocDashboardData: s,
                         commands: l
-                    } = this.props, i = this.props.itemRenderer(e, t, o);
-                    return i ? y().createElement("li", {
+                    } = this.props, r = this.props.itemRenderer(e, t, o);
+                    return r ? N().createElement("li", {
                         className: "dashboard-tocItem",
                         onClick: e => {
-                            ue.sendInteraction({
+                            ye.sendInteraction({
                                 click_type: "ON",
-                                signal_origin: Q.TOC_HEADING_CLICKED
+                                signal_origin: re.TOC_HEADING_CLICKED
                             }), e.preventDefault(), e.stopPropagation(), t.onClick()
                         }
-                    }, i, n && y().createElement(Fe, {
+                    }, r, n && N().createElement(nt, {
                         cellId: t.cellRef.model.id,
                         data: a ? s : null,
                         commands: l
                     })) : null
                 }
             }
-            const ze = e => {
-                const [t, o] = (0, f.useState)(null), n = (0, ie.useSelector)((e => e.tocdashboard.displayDashboard)), a = (0, ie.useSelector)((e => e.commondashboard.refreshBoolean)), s = (0, ie.useSelector)((e => e.commondashboard.timeWindow)), l = (0, ie.useSelector)((e => e.commondashboard.displayRealTime));
-                (0, f.useEffect)((() => (d(), () => {
+            const st = e => {
+                const [t, o] = (0, D.useState)(null), n = (0, be.useSelector)((e => e.tocdashboard.displayDashboard)), a = (0, be.useSelector)((e => e.commondashboard.refreshBoolean)), s = (0, be.useSelector)((e => e.commondashboard.dashboardQueryArgs));
+                (0, D.useEffect)((() => (i(), () => {
                     o(null)
-                })), [e.notebookCells, e.notebookPanel]), (0, f.useEffect)((() => {
-                    d()
+                })), [e.notebookCells, e.notebookPanel]), (0, D.useEffect)((() => {
+                    i()
                 }), [a, s]);
-                const r = (0, f.useRef)("12345678"),
-                    d = async () => {
+                const l = (0, D.useRef)("12345678"),
+                    i = async () => {
                         const t = w.getMetadataComp(e.notebookPanel.model, _.notebookId);
                         if (t && e.notebookCells) {
                             try {
                                 const e = crypto.randomUUID();
-                                r.current = e;
-                                const n = await v(`${i}/dashboard/${t}/toc?timeWindow=${s}&displayRealTime=${l}`);
-                                if (e === r.current) {
+                                l.current = e;
+                                const n = await E(`${r}/dashboard/${t}/toc?${C(s,t)}`);
+                                if (e === l.current) {
                                     if (n.ok) {
                                         const e = await n.json();
                                         return void o(e.data)
                                     }
                                     console.log(`${c}: Error:`, n.status)
                                 }
                             } catch (e) {
                                 console.log(`${c}: Toc Fetch Error:`, e)
                             }
                             o(null)
                         }
-                    }, h = (t => {
+                    }, d = (t => {
                         const o = e.headings.map((e => e.cellRef.model.id)),
                             n = [...new Set(o)],
                             a = {},
                             s = e.notebookCells;
                         if (s && t) {
                             const e = n.map((e => s.indexOf(e)));
                             e[0] = 0, e.push(s.length);
                             let o = 0;
                             for (let l = 0; l < n.length; l++) {
-                                const i = e[l],
-                                    r = e[l + 1];
+                                const r = e[l],
+                                    i = e[l + 1];
                                 let c = 0;
-                                if (-1 === i) c = 0;
+                                if (-1 === r) c = 0;
                                 else
-                                    for (let e = i; e < r; e++) c += t.location_count[s[e]] || 0;
+                                    for (let e = r; e < i; e++) c += t.location_count[s[e]] || 0;
                                 a[n[l]] = c, o += c
                             }
                             a.total_count = o
                         }
                         return a
-                    })(t), m = new Set;
-                return y().createElement("ul", {
+                    })(t), h = new Set;
+                return N().createElement("ul", {
                     className: "dashboard-TableOfContents-content"
                 }, e.headings.map(((t, o) => {
                     const a = t.cellRef.model.id,
-                        s = !m.has(a);
-                    return s && m.add(a), y().createElement(Ve, {
+                        s = !h.has(a);
+                    return s && h.add(a), N().createElement(at, {
                         panel: e.notebookPanel,
                         heading: t,
                         headings: e.headings,
                         itemRenderer: e.itemRenderer,
                         addReactComponent: n,
                         isFirstCellOccurrence: s,
-                        tocDashboardData: [h[a], h.total_count],
+                        tocDashboardData: [d[a], d.total_count],
                         commands: e.commands,
                         key: `${t.text}-${t.level}-${o++}`
                     })
                 })))
             };
-            class Pe extends oe {
+            class lt extends he {
                 constructor(e, t) {
-                    super(), this._preRenderedToolbar = null, this._showCode = !1, this._showMarkdown = !1, this._numbering = t.numbering, this._numberingH1 = t.numberingH1, this._syncCollapseState = t.syncCollapseState, this._widget = e, this.sanitizer = t.sanitizer, this._collapseChanged = new te.Signal(this)
+                    super(), this._preRenderedToolbar = null, this._showCode = !1, this._showMarkdown = !1, this._numbering = t.numbering, this._numberingH1 = t.numberingH1, this._syncCollapseState = t.syncCollapseState, this._widget = e, this.sanitizer = t.sanitizer, this._collapseChanged = new de.Signal(this)
                 }
                 set numberingH1(e) {
                     this._numberingH1 !== e && (this._numberingH1 = e, this._widget.update())
                 }
                 get numberingH1() {
                     return this._numberingH1
                 }
@@ -1253,138 +1553,138 @@
                     this._collapseChanged.emit(e), this._widget.update()
                 }
                 initializeOptions(e, t, o, n, a) {
                     this._numbering = e, this._numberingH1 = t, this._syncCollapseState = o, this._showCode = n, this._showMarkdown = a, this._widget.update()
                 }
             }
 
-            function We(e) {
+            function rt(e) {
                 if (e.length > 0) {
                     let t = e.length - 1;
                     for (; t >= 0;) {
                         if ("header" === e[t].type) return e[t].level;
                         t -= 1
                     }
                 }
                 return 0
             }
-            const je = "jp-MarkdownHeadingCollapsed",
-                Ke = "dashboard-toc-hr-collapsed";
+            const it = "jp-MarkdownHeadingCollapsed",
+                ct = "dashboard-toc-hr-collapsed";
 
-            function Ge(e, t, o, n, a, s) {
+            function dt(e, t, o, n, a, s) {
                 const l = [];
                 if (e) {
-                    const i = e.split("\n"),
-                        r = Math.min(i.length, 3);
+                    const r = e.split("\n"),
+                        i = Math.min(r.length, 3);
                     let c = "",
                         d = 0;
-                    for (; d < r - 1; d++) c += i[d] + "\n";
-                    c += i[d], l.push({
+                    for (; d < i - 1; d++) c += r[d] + "\n";
+                    c += r[d], l.push({
                         text: c,
                         level: n + 1,
                         onClick: t(0),
                         type: "code",
                         prompt: o,
                         cellRef: a,
                         hasChild: !1,
                         index: s
                     })
                 }
                 return l[0]
             }
 
-            function Je(e, t, o, n) {
+            function ht(e, t, o, n) {
                 if (t && t.text) {
                     if (o && "header" === o.type)
                         for (let t = e.length - 1; t >= 0; t--) e[t] === o && (e[t].hasChild = !0);
                     n < 0 && e.push(t), o = t
                 }
                 return [e, o]
             }
-            const qe = {
+            const ut = {
                 allowedTags: ["p", "blockquote", "b", "i", "strong", "em", "strike", "code", "br", "div", "span", "pre", "del"],
                 allowedAttributes: {
                     code: ["class"],
                     span: ["class"],
                     div: ["class"],
                     p: ["class"],
                     pre: ["class"]
                 }
             };
 
-            function Xe(e, t, o, n, a, s = !1, l = !0, i, r) {
+            function mt(e, t, o, n, a, s = !1, l = !0, r, i) {
                 const c = e.querySelectorAll("h1, h2, h3, h4, h5, h6, p");
                 let d = a;
                 const h = [];
                 for (const e of c) {
                     if ("p" === e.nodeName.toLowerCase()) {
                         if (e.innerHTML) {
-                            const n = o.sanitize(e.innerHTML, qe);
+                            const n = o.sanitize(e.innerHTML, ut);
                             h.push({
                                 level: d + 1,
                                 html: n.replace("¶", ""),
                                 text: e.textContent ? e.textContent : "",
                                 onClick: t(e),
                                 type: "markdown",
-                                cellRef: i,
+                                cellRef: r,
                                 hasChild: !1,
-                                index: r
+                                index: i
                             })
                         }
                         continue
                     }
                     e.getElementsByClassName("numbering-entry").length > 0 && e.removeChild(e.getElementsByClassName("numbering-entry")[0]);
-                    let a = o.sanitize(e.innerHTML, qe);
+                    let a = o.sanitize(e.innerHTML, ut);
                     a = a.replace("¶", "");
                     let c = parseInt(e.tagName[1], 10);
                     l || (c -= 1), d = c;
-                    const m = Ye(n, c);
+                    const u = bt(n, c);
                     if (s) {
                         const t = document.createElement("span");
-                        t.classList.add("numbering-entry"), t.textContent = null != m ? m : "", e.insertBefore(t, e.firstChild)
+                        t.classList.add("numbering-entry"), t.textContent = null != u ? u : "", e.insertBefore(t, e.firstChild)
                     }
                     h.push({
                         level: c,
                         text: e.textContent ? e.textContent : "",
-                        numbering: m,
+                        numbering: u,
                         html: a,
                         onClick: t(e),
                         type: "header",
-                        cellRef: i,
+                        cellRef: r,
                         hasChild: !1,
-                        index: r
+                        index: i
                     })
                 }
                 return h
             }
 
-            function Ze(e, t, o, n, a, s) {
-                return e && "markdown" === e.type && s ? [t, o] = Je(t, e, o, n) : e && "header" === e.type && ([t, o, n] = function(e, t, o, n, a) {
+            function pt(e, t, o, n, a, s) {
+                return e && "markdown" === e.type && s ? [t, o] = ht(t, e, o, n) : e && "header" === e.type && ([t, o, n] = function(e, t, o, n, a) {
                     const s = e.length;
                     if (o && "header" === o.type && o.level < t.level)
                         for (let t = s - 1; t >= 0; t--) e[t] === o && (e[t].hasChild = !0);
                     return (n >= t.level || n < 0) && (e.push(t), n = a ? t.level : -1), [e, o = t, n]
                 }(t, e, o, n, a)), [t, o, n]
             }
-            const Qe = 6;
+            const gt = 6;
 
-            function Ye(e, t) {
+            function bt(e, t) {
                 if (null === e) return;
                 let o = "";
                 if (e = function(e, t) {
-                        for (let o = t + 1; o <= Qe; o++) void 0 !== e[o] && (e[o] = void 0);
+                        for (let o = t + 1; o <= gt; o++) void 0 !== e[o] && (e[o] = void 0);
                         return void 0 === e[t] ? e[t] = 1 : e[t] += 1, e
                     }(e, t), t >= 1) {
                     for (let n = 1; n <= t; n++) o += (void 0 === e[n] ? "0" : e[n]) + ".";
                     o += " "
                 }
                 return o
             }
 
-            function et(e) {
+            function _t(e) {
                 const t = e.split("\n");
                 let o = t[0].match(/^([#]{1,6}) (.*)/);
                 return o ? {
                     text: o[2].replace(/\[(.+)\]\(.+\)/g, "$1"),
                     level: o[1].length,
                     type: "markdown"
                 } : t.length > 1 && (o = t[1].match(/^ {0,3}([=]{2,}|[-]{2,})\s*$/), o) ? {
@@ -1394,79 +1694,79 @@
                 } : (o = t[0].match(/<h([1-6]).*>(.*)<\/h\1>/i), o ? {
                     text: o[2],
                     level: parseInt(o[1], 10),
                     type: "html"
                 } : null)
             }
 
-            function tt(e, t, o, n, a, s) {
+            function vt(e, t, o, n, a, s) {
                 const l = t(0),
-                    i = [];
-                let r = n;
+                    r = [];
+                let i = n;
                 for (const t of e.split("\n"))
                     if (t) {
-                        const e = et(t);
-                        e ? (i.push({
+                        const e = _t(t);
+                        e ? (r.push({
                             text: e.text,
                             level: e.level,
-                            numbering: Ye(o, e.level),
+                            numbering: bt(o, e.level),
                             onClick: l,
                             type: "header",
                             cellRef: a,
                             hasChild: !1,
                             index: s
-                        }), r = e.level) : i.push({
+                        }), i = e.level) : r.push({
                             text: t,
-                            level: r + 1,
+                            level: i + 1,
                             onClick: l,
                             type: "markdown",
                             cellRef: a,
                             hasChild: !1,
                             index: s
                         })
-                    } return i
+                    } return r
             }
 
-            function ot(e, t, o) {
+            function kt(e, t, o) {
                 if (t.index > -1 || (null == o ? void 0 : o.length)) {
                     const n = e.content.activeCellIndex,
                         a = t.index;
                     if (n && a < n) {
                         const e = o.indexOf(t) + 1;
                         if (e >= o.length) return !0;
                         if ((null == o ? void 0 : o[e].index) > n) return !0
                     }
                 }
                 return !1
             }
-            const nt = X.dispatch;
+            const wt = se.dispatch;
 
-            function at(e, t, o) {
+            function Ct(e, t, o) {
                 let n = !0,
                     a = !1;
                 o && o.composite.tocDashboardSettings && (n = o.composite.tocDashboardSettings.numberingH1, a = o.composite.tocDashboardSettings.syncCollapseState);
-                const s = new Pe(e, {
+                const s = new lt(e, {
                     numbering: !1,
                     numberingH1: n,
                     syncCollapseState: a,
                     sanitizer: t
                 });
                 return o && o.composite.tocDashboardSettings && o.changed.connect((() => {
                     s.numberingH1 = o.composite.tocDashboardSettings.numberingH1, s.syncCollapseState = o.composite.tocDashboardSettings.syncCollapseState
                 })), {
                     options: s,
                     toolbarGenerator: function(e) {
                         return function(e, t) {
-                            return class extends f.Component {
+                            return class extends D.Component {
                                 constructor(o) {
                                     super(o), this.state = {
                                         showCode: !0,
                                         showMarkdown: !1,
                                         numbering: !1,
-                                        showVisuDashboard: I.displayDashboard
+                                        showVisuDashboard: B.displayDashboard
                                     }, t.context.ready.then((() => {
                                         if (t) {
                                             t.content.activeCellChanged.connect((() => {
                                                 e.updateWidget()
                                             }));
                                             const o = w.getMetadataComp(t.model, "dashboard-toc-autonumbering"),
                                                 n = w.getMetadataComp(t.model, "dashboard-toc-showcode"),
@@ -1476,371 +1776,282 @@
                                                 showMarkdown: e.showMarkdown,
                                                 numbering: e.numbering
                                             })
                                         }
                                     }))
                                 }
                                 toggleCode() {
-                                    ue.sendInteraction({
+                                    ye.sendInteraction({
                                         click_type: e.showCode ? "OFF" : "ON",
-                                        signal_origin: Q.TOC_TOOLBAR_CODE
+                                        signal_origin: re.TOC_TOOLBAR_CODE
                                     }), e.setShowCode(!e.showCode, t), this.setState({
                                         showCode: e.showCode
                                     })
                                 }
                                 toggleMarkdown() {
-                                    ue.sendInteraction({
+                                    ye.sendInteraction({
                                         click_type: e.showMarkdown ? "OFF" : "ON",
-                                        signal_origin: Q.TOC_TOOLBAR_MARKDOWN
+                                        signal_origin: re.TOC_TOOLBAR_MARKDOWN
                                     }), e.setShowMarkdown(!e.showMarkdown, t), this.setState({
                                         showMarkdown: e.showMarkdown
                                     })
                                 }
                                 toggleNumbering() {
-                                    ue.sendInteraction({
+                                    ye.sendInteraction({
                                         click_type: e.numbering ? "OFF" : "ON",
-                                        signal_origin: Q.TOC_TOOLBAR_NUMBERED
+                                        signal_origin: re.TOC_TOOLBAR_NUMBERED
                                     }), e.setNumbering(!e.numbering, t), this.setState({
                                         numbering: e.numbering
                                     })
                                 }
                                 toggleShowVisuDashboard() {
                                     const e = this.state.showVisuDashboard;
-                                    ue.sendInteraction({
+                                    ye.sendInteraction({
                                         click_type: e ? "OFF" : "ON",
-                                        signal_origin: Q.TOC_TOOLBAR_SHOW_HIDE
-                                    }), nt(A(!e)), this.setState({
+                                        signal_origin: re.TOC_TOOLBAR_SHOW_HIDE
+                                    }), wt($(!e)), this.setState({
                                         showVisuDashboard: !e
                                     })
                                 }
                                 refreshDashboard() {
-                                    ue.sendInteraction({
+                                    ye.sendInteraction({
                                         click_type: "ON",
-                                        signal_origin: Q.TOC_TOOLBAR_REFRESH
-                                    }), nt(G())
+                                        signal_origin: re.TOC_TOOLBAR_REFRESH
+                                    }), wt(te())
                                 }
                                 render() {
-                                    const e = f.createElement("div", {
+                                    const e = D.createElement("div", {
                                             onClick: e => this.toggleCode(),
                                             role: "text",
                                             "aria-label": "Toggle Code Cells",
                                             title: "Toggle Code Cells",
                                             className: this.state.showCode ? "dashboard-toc-toolbar-icon-selected" : "dashboard-toc-toolbar-icon"
-                                        }, f.createElement(S.codeIcon.react, null)),
-                                        t = f.createElement("div", {
+                                        }, D.createElement(x.codeIcon.react, null)),
+                                        t = D.createElement("div", {
                                             onClick: e => this.toggleMarkdown(),
                                             role: "text",
                                             "aria-label": "Toggle Markdown Text Cells",
                                             title: "Toggle Markdown Text Cells",
                                             className: this.state.showMarkdown ? "dashboard-toc-toolbar-icon-selected" : "dashboard-toc-toolbar-icon"
-                                        }, f.createElement(S.markdownIcon.react, null)),
-                                        o = f.createElement("div", {
+                                        }, D.createElement(x.markdownIcon.react, null)),
+                                        o = D.createElement("div", {
                                             onClick: e => this.toggleNumbering(),
                                             role: "text",
                                             "aria-label": "Toggle Auto-Numbering",
                                             title: "Toggle Auto-Numbering",
                                             className: this.state.numbering ? "dashboard-toc-toolbar-icon-selected" : "dashboard-toc-toolbar-icon"
-                                        }, f.createElement(S.numberingIcon.react, null)),
-                                        n = f.createElement("div", {
+                                        }, D.createElement(x.numberingIcon.react, null)),
+                                        n = D.createElement("div", {
                                             onClick: e => this.toggleShowVisuDashboard(),
                                             role: "text",
                                             "aria-label": this.state.showVisuDashboard ? "Hide Visualization Dashboard" : "Show Visualization Dashboard",
                                             title: this.state.showVisuDashboard ? "Hide Visualization Dashboard" : "Show Visualization Dashboard",
                                             className: "dashboard-toc-toolbar-icon"
-                                        }, this.state.showVisuDashboard ? f.createElement(N.react, null) : f.createElement(T.react, null)),
-                                        a = f.createElement("div", {
+                                        }, this.state.showVisuDashboard ? D.createElement(A.react, null) : D.createElement(L.react, null)),
+                                        a = D.createElement("div", {
                                             onClick: e => this.refreshDashboard(),
                                             role: "text",
                                             "aria-label": "Refresh Dashboard",
                                             title: "Refresh Dashboard",
                                             className: "dashboard-toc-toolbar-icon"
-                                        }, f.createElement(S.refreshIcon.react, null));
-                                    return f.createElement("div", null, f.createElement("div", {
+                                        }, D.createElement(x.refreshIcon.react, null));
+                                    return D.createElement("div", null, D.createElement("div", {
                                         className: "dashboard-toc-toolbar"
-                                    }, f.createElement("div", {
+                                    }, D.createElement("div", {
                                         className: "dashboard-toc-toolbar-compartment"
-                                    }, e, t, o), f.createElement("div", {
+                                    }, e, t, o), D.createElement("div", {
                                         className: "dashboard-toc-toolbar-compartment"
                                     }, n, a)))
                                 }
                             }
                         }(s, e)
                     },
                     itemRenderer: function(e, t, o = []) {
                         return function(e, t, o, n = []) {
                             var a;
                             if ("markdown" === o.type || "header" === o.type) {
                                 let a = "dashboard-toc-level-size-default";
                                 const s = o.numbering && e.numbering ? o.numbering : "",
-                                    l = e.syncCollapseState ? je : Ke;
+                                    l = e.syncCollapseState ? it : ct;
                                 if ("header" !== o.type && "markdown" !== o.type || (a = "dashboard-toc-level-size-" + o.level), "header" === o.type || e.showMarkdown) {
-                                    let i;
-                                    i = o.html ? f.createElement("span", {
+                                    let r;
+                                    r = o.html ? D.createElement("span", {
                                         dangerouslySetInnerHTML: {
-                                            __html: s + e.sanitizer.sanitize(o.html, qe)
+                                            __html: s + e.sanitizer.sanitize(o.html, ut)
                                         },
                                         className: "dashboard-" + o.type + "-cell dashboard-toc-cell-item"
-                                    }) : f.createElement("span", {
+                                    }) : D.createElement("span", {
                                         className: "dashboard-" + o.type + "-cell dashboard-toc-cell-item"
                                     }, s + o.text);
-                                    let r = null;
-                                    return "header" === o.type && (r = f.createElement("div", {
+                                    let i = null;
+                                    return "header" === o.type && (i = D.createElement("div", {
                                         className: "jp-Collapser p-Widget lm-Widget",
                                         onClick: n => {
                                             n.stopPropagation(),
                                                 function(t, o, n) {
                                                     let a = !1;
                                                     const s = e.syncCollapseState,
                                                         l = w.getMetadataComp(null == n ? void 0 : n.cellRef.model, o);
-                                                    l && (a = l), n ? (ue.sendInteraction({
+                                                    l && (a = l), n ? (ye.sendInteraction({
                                                         click_type: a ? "OFF" : "ON",
-                                                        signal_origin: Q.TOC_COLLAPSE_HEADERS
-                                                    }), s ? t && Y.NotebookActions.setHeadingCollapse(null == n ? void 0 : n.cellRef, !a, t.content) : a ? w.deleteMetadataComp(n.cellRef.model, o) : w.setMetadataComp(n.cellRef.model, o, !0), e.updateAndCollapse({
+                                                        signal_origin: re.TOC_COLLAPSE_HEADERS
+                                                    }), s ? t && ie.NotebookActions.setHeadingCollapse(null == n ? void 0 : n.cellRef, !a, t.content) : a ? w.deleteMetadataComp(n.cellRef.model, o) : w.setMetadataComp(n.cellRef.model, o, !0), e.updateAndCollapse({
                                                         heading: n,
                                                         collapsedState: a
                                                     })) : e.updateWidget()
                                                 }(t, l, o)
                                         }
-                                    }, f.createElement("div", {
+                                    }, D.createElement("div", {
                                         className: "dashboard-toc-Collapser-child"
-                                    }))), i = f.createElement("div", {
-                                        className: "dashboard-toc-entry-holder " + a + (t.content.activeCell === o.cellRef || ot(t, o, n) ? " dashboard-toc-active-cell" : "")
-                                    }, r, i), i
+                                    }))), r = D.createElement("div", {
+                                        className: "dashboard-toc-entry-holder " + a + (t.content.activeCell === o.cellRef || kt(t, o, n) ? " dashboard-toc-active-cell" : "")
+                                    }, i, r), r
                                 }
                                 return null
                             }
                             if (t && "code" === o.type && e.showCode) {
                                 const e = (null === (a = w.getMetadataComp(t.model, "language_info")) || void 0 === a ? void 0 : a.mimetype) || "text";
-                                return f.createElement("div", {
+                                return D.createElement("div", {
                                     className: "dashboard-toc-code-cell-div"
-                                }, f.createElement("div", {
+                                }, D.createElement("div", {
                                     className: "dashboard-toc-code-cell-prompt"
-                                }, o.prompt), f.createElement("span", {
+                                }, o.prompt), D.createElement("span", {
                                     className: "dashboard-toc-code-span"
-                                }, f.createElement(Re, {
+                                }, D.createElement(Ge, {
                                     cell_input: o.text,
                                     language_mimetype: e,
                                     className: "dashboard-toc-cell-input"
                                 })))
                             }
                             return null
                         }(s, e, t, o)
                     },
                     generate: function(o) {
                         let n = [],
                             a = -1;
                         const l = {};
-                        let i = null;
-                        for (let r = 0; r < o.content.widgets.length; r++) {
-                            const c = o.content.widgets[r],
+                        let r = null;
+                        for (let i = 0; i < o.content.widgets.length; i++) {
+                            const c = o.content.widgets[i],
                                 d = c.model,
-                                h = s.syncCollapseState ? je : Ke;
-                            let m = w.getMetadataComp(d, h);
-                            if (m = m || !1, "code" !== d.type) {
+                                h = s.syncCollapseState ? it : ct;
+                            let u = w.getMetadataComp(d, h);
+                            if (u = u || !1, "code" !== d.type) {
                                 if ("markdown" === d.type) {
                                     const e = c;
                                     let h;
-                                    const u = We(n);
+                                    const m = rt(n);
                                     if (e.rendered && !e.inputHidden) {
                                         const d = t => () => {
-                                                e.rendered ? (o.content.mode = "command", c.node.scrollIntoView(), o.content.activeCellIndex = r) : (o.content.activeCellIndex = r, t.scrollIntoView())
+                                                e.rendered ? (o.content.mode = "command", c.node.scrollIntoView(), o.content.activeCellIndex = i) : (o.content.activeCellIndex = i, t.scrollIntoView())
                                             },
-                                            p = Xe(c.node, d, t, l, u, s.numbering, s.numberingH1, c, r);
-                                        for (h of p)[n, i, a] = Ze(h, n, i, a, m, s.showMarkdown)
+                                            p = mt(c.node, d, t, l, m, s.numbering, s.numberingH1, c, i);
+                                        for (h of p)[n, r, a] = pt(h, n, r, a, u, s.showMarkdown)
                                     } else {
                                         const e = e => () => {
-                                                o.content.activeCellIndex = r, c.node.scrollIntoView()
+                                                o.content.activeCellIndex = i, c.node.scrollIntoView()
                                             },
-                                            t = tt(d.sharedModel.getSource(), e, l, u, c, r);
-                                        for (h of t)[n, i, a] = Ze(h, n, i, a, m, s.showMarkdown)
+                                            t = vt(d.sharedModel.getSource(), e, l, m, c, i);
+                                        for (h of t)[n, r, a] = pt(h, n, r, a, u, s.showMarkdown)
                                     }
                                 }
                             } else if (!e || e && s.showCode) {
                                 const e = e => () => {
-                                        o.content.activeCellIndex = r, c.node.scrollIntoView()
+                                        o.content.activeCellIndex = i, c.node.scrollIntoView()
                                     },
                                     t = c.model.executionCount,
                                     s = null !== t ? "[" + t + "]: " : "[ ]: ",
-                                    l = Ge(d.sharedModel.getSource(), e, s, We(n), c, r);
-                                [n, i] = Je(n, l, i, a)
+                                    l = dt(d.sharedModel.getSource(), e, s, rt(n), c, i);
+                                [n, r] = ht(n, l, r, a)
                             }
                         }
                         return n
                     },
                     collapseChanged: s.collapseChanged
                 }
             }
-            const st = e => e.toLocaleString("sv-SE").slice(0, -3),
-                lt = e => {
-                    const [t, o] = (0, f.useState)(e.startT1), [n, a] = (0, f.useState)(e.startT2), s = st(new Date), l = t => {
-                        o(t), e.t1Callback(t)
-                    }, i = t => {
-                        a(t), e.t2Callback(t)
-                    };
-                    return y().createElement("div", {
-                        className: "dashboard-export-dialog-container"
-                    }, y().createElement("p", null, "Select the time range of the data you want to export (the past week selected by default)."), y().createElement("div", {
-                        className: "dashboard-export-dialog-calendar-container"
-                    }, y().createElement("div", {
-                        className: "dashboard-export-dialog-calendar"
-                    }, y().createElement("p", null, "Start Date :"), y().createElement("input", {
-                        className: "dashboard-calendar-input",
-                        type: "datetime-local",
-                        value: st(t),
-                        onChange: e => (e => {
-                            const t = new Date(e);
-                            l(t), t >= n && i(t)
-                        })(e.target.value),
-                        max: st(n)
-                    })), y().createElement("div", {
-                        className: "dashboard-export-dialog-calendar"
-                    }, y().createElement("p", null, "End Date :"), y().createElement("input", {
-                        className: "dashboard-calendar-input",
-                        type: "datetime-local",
-                        value: st(n),
-                        onChange: e => (e => {
-                            const o = new Date(e);
-                            i(o), o <= t && l(o)
-                        })(e.target.value),
-                        max: s
-                    }))))
-                },
-                it = e => {
-                    const [t, o] = (0, f.useState)(!1);
-                    return y().createElement("div", {
-                        className: "dashboard-toc-download-button" + (t ? "-disabled" : ""),
-                        onClick: () => {
-                            t || (e => {
-                                let t = new Date,
-                                    n = new Date;
-                                n.setDate(t.getDate() - 7), (0, O.showDialog)({
-                                    title: "Download Notebook Data",
-                                    body: y().createElement(lt, {
-                                        startT1: n,
-                                        startT2: t,
-                                        t1Callback: e => n = e,
-                                        t2Callback: e => t = e
-                                    }),
-                                    buttons: [{
-                                        accept: !0,
-                                        actions: [],
-                                        ariaLabel: "Export",
-                                        caption: "",
-                                        className: "",
-                                        displayType: "default",
-                                        iconClass: "",
-                                        iconLabel: "",
-                                        label: "Export"
-                                    }, O.Dialog.cancelButton()]
-                                }).then((a => {
-                                    a.button.accept && ((e, t, n) => {
-                                        o(!0);
-                                        let a = "";
-                                        v(`${i}/dashboard/${e}/download_csv?t1=${t.toISOString()}&t2=${n.toISOString()}`).then((e => {
-                                            var t;
-                                            if (e.ok) {
-                                                const o = e.headers.get("Content-Disposition");
-                                                return a = (null === (t = null == o ? void 0 : o.match(/filename=(.+)/)) || void 0 === t ? void 0 : t[1]) || "", e.blob()
-                                            }
-                                        })).then((e => {
-                                            if (e) {
-                                                const t = window.URL.createObjectURL(e),
-                                                    o = document.createElement("a");
-                                                o.href = t, o.download = a, document.body.appendChild(o), o.click(), o.remove()
-                                            }
-                                        })).finally((() => {
-                                            o(!1)
-                                        }))
-                                    })(e, n, t)
-                                }))
-                            })(e.notebookId)
-                        }
-                    }, y().createElement(S.downloadIcon.react, {
-                        className: "dashboard-toc-download-icon"
-                    }), "Export")
-                };
-            class rt extends me {
+            class Et extends Ce {
                 constructor(e, t, o, n) {
-                    super(e), this.title.caption = "Dashboard ToC", this.title.icon = x, this.id = "dashboard-toc-code", this.node.setAttribute("role", "region"), this.node.setAttribute("aria-label", "Dashboard ToC section"), this._commands = t, this._notebookGenerator = at(this, o, n), this._toolbar = null, e.panelSwitched.connect(this._onPanelSwitched, this)
+                    super(e), this.title.caption = "Dashboard ToC", this.title.icon = R, this.id = "dashboard-toc-code", this.node.setAttribute("role", "region"), this.node.setAttribute("aria-label", "Dashboard ToC section"), this._commands = t, this._notebookGenerator = Ct(this, o, n), this._toolbar = null, e.panelSwitched.connect(this._onPanelSwitched, this)
                 }
                 onBeforeShow(e) {
-                    ue.sendInteraction({
+                    ye.sendInteraction({
                         click_type: "ON",
-                        signal_origin: Q.TOC_DASHBOARD_SHOW_HIDE
+                        signal_origin: re.TOC_DASHBOARD_SHOW_HIDE
                     })
                 }
                 onBeforeHide(e) {
-                    ue.sendInteraction({
+                    ye.sendInteraction({
                         click_type: "OFF",
-                        signal_origin: Q.TOC_DASHBOARD_SHOW_HIDE
+                        signal_origin: re.TOC_DASHBOARD_SHOW_HIDE
                     })
                 }
                 _onPanelSwitched(e) {
                     this._panelManager.panel ? this._toolbar = this._notebookGenerator.toolbarGenerator(this._panelManager.panel) : this._toolbar = null
                 }
                 computeComponentToRender() {
                     const e = this._panelManager.panel;
-                    return e ? f.createElement("div", {
+                    return e ? D.createElement("div", {
                         className: "dashboard-TableOfContents"
-                    }, f.createElement("div", {
+                    }, D.createElement("div", {
                         className: "dashboard-stack-panel-header"
-                    }, f.createElement("span", {
+                    }, D.createElement("span", {
                         className: "dashboard-toc-header-title"
-                    }, ee.PathExt.basename(e.context.localPath)), f.createElement(it, {
+                    }, ce.PathExt.basename(e.context.localPath)), D.createElement(Ne, {
                         notebookId: this._panelManager.validityChecks.tag
-                    })), this._toolbar && f.createElement(this._toolbar, null), f.createElement(ze, {
+                    })), this._toolbar && D.createElement(this._toolbar, null), D.createElement(st, {
                         headings: this._notebookGenerator.generate(e),
                         itemRenderer: this._notebookGenerator.itemRenderer,
                         notebookPanel: e,
                         commands: this._commands,
                         notebookCells: this._panelManager.notebookCells
-                    })) : f.createElement(f.Fragment, null)
+                    })) : D.createElement(D.Fragment, null)
                 }
             }
-            var ct = o(4882);
-            const dt = "cell-dashboard-button-container";
-            class ht extends ct.Widget {
+            var yt = o(4882);
+            const ft = "cell-dashboard-button-container";
+            class St extends yt.Widget {
                 constructor(e, t) {
-                    super(), this.addClass(dt);
+                    super(), this.addClass(ft);
                     const o = document.createElement("button");
-                    o.className = "cell-dashboard-button", o.innerHTML = x.svgstr, o.title = o.disabled ? "No notebook identifier" : "Open Cell Dashboard", o.onclick = () => {
-                        e.execute(u.dashboardOpenVisu, {
+                    o.className = "cell-dashboard-button", o.innerHTML = R.svgstr, o.title = o.disabled ? "No notebook identifier" : "Open Cell Dashboard", o.onclick = () => {
+                        e.execute(p.dashboardOpenVisu, {
                             from: "Cell",
                             cell_id: t
                         })
                     }, this.node.appendChild(o)
                 }
                 dispose() {
                     super.dispose()
                 }
             }
-            class mt {
+            class Ot {
                 constructor(e) {
                     this._commands = e
                 }
                 createNew(e) {
-                    return new ut(e, this._commands)
+                    return new Dt(e, this._commands)
                 }
             }
-            class ut {
+            class Dt {
                 constructor(e, t) {
                     this._isDisposed = !1, this._panel = e, this._commands = t, this._previousActiveCell = this._panel.content.activeCell, e.context.ready.then((() => {
-                        E(e) ? (e.revealed.then((() => {
+                        S(e) ? (e.revealed.then((() => {
                             e && !e.isDisposed && setTimeout((() => {
                                 this._onActiveCellChanged(e.content)
                             }), 1e3 / 60)
                         })), e.content.renderingLayoutChanged.connect(this._onActiveCellChanged, this), e.content.activeCellChanged.connect(this._onActiveCellChanged, this), e.disposed.connect((() => {
                             e.content.activeCellChanged.disconnect(this._onActiveCellChanged)
                         }))) : this.dispose()
                     }))
                 }
                 _addCellButton(e) {
                     const t = this._getCell(e);
                     if (t) {
-                        const e = new ht(this._commands, t.model.id);
+                        const e = new St(this._commands, t.model.id);
                         t.layout.insertWidget(0, e)
                     }
                 }
                 _onActiveCellChanged(e) {
                     this._previousActiveCell && !this._previousActiveCell.isDisposed && this._removeCellButton(this._previousActiveCell.model);
                     const t = e.activeCell;
                     null !== t && (this._addCellButton(t.model), this._previousActiveCell = t)
@@ -1852,277 +2063,276 @@
                 _removeCellButton(e) {
                     const t = this._getCell(e);
                     t && this._findCellButtonWidgets(t).forEach((e => {
                         e.dispose()
                     }))
                 }
                 _findCellButtonWidgets(e) {
-                    return e.layout.widgets.filter((e => e.hasClass(dt))) || []
+                    return e.layout.widgets.filter((e => e.hasClass(ft))) || []
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
                     var e;
                     if (this.isDisposed) return;
                     this._isDisposed = !0;
                     const t = w.getCellsArrComp(null === (e = this._panel) || void 0 === e ? void 0 : e.context.model.cells);
                     if (t)
                         for (const e of t) this._removeCellButton(e);
-                    this._panel = null, te.Signal.clearData(this)
+                    this._panel = null, de.Signal.clearData(this)
                 }
             }
-            var pt = o(7717);
-            class gt {
+            var Nt = o(7717);
+            class xt {
                 constructor(e) {
                     this._commands = e
                 }
                 createNew(e) {
-                    const t = new O.ToolbarButton({
+                    const t = new I.ToolbarButton({
                         className: "open-visu-button",
-                        icon: x,
+                        icon: R,
                         onClick: () => {
-                            this._commands.execute(u.dashboardOpenVisu, {
+                            this._commands.execute(p.dashboardOpenVisu, {
                                 from: "Notebook"
                             })
                         },
                         tooltip: "Open Notebook Visualization"
                     });
                     return e.context.ready.then((() => {
-                        E(e) && e.toolbar.insertItem(10, "openVisu", t)
-                    })), new pt.DisposableDelegate((() => {
+                        S(e) && e.toolbar.insertItem(10, "openVisu", t)
+                    })), new Nt.DisposableDelegate((() => {
                         t.dispose()
                     }))
                 }
             }
-            const _t = X.dispatch;
-            var bt = o(1810);
-            let wt = null;
+            const It = se.dispatch;
+            var Tt = o(7217);
+            let Rt = null;
 
-            function vt(e) {
-                wt = e
+            function At(e) {
+                Rt = e
             }
-            let Ct = null;
-            const kt = {
+            let Lt = null;
+            const Mt = {
                     id: d,
                     autoStart: !0,
                     requires: [a.IFileBrowserFactory, n.ILayoutRestorer, n.ILabShell, s.IRenderMimeRegistry, l.ISettingRegistry],
                     optional: [],
                     activate: (e, t, o, n, a, s) => {
                         console.log(`JupyterLab extension ${c} is activated!`);
                         const l = "3.1.0",
-                            r = e.version.match(/[0-9]+/g),
+                            i = e.version.match(/[0-9]+/g),
                             d = async function(e = "", t = {}) {
-                                const o = bt.ServerConnection.makeSettings(),
-                                    n = ee.URLExt.join(o.baseUrl, "jupyterlab-unianalytics-dashboard", e);
+                                const o = Tt.ServerConnection.makeSettings(),
+                                    n = ce.URLExt.join(o.baseUrl, "jupyterlab-unianalytics-dashboard", e);
                                 let a;
                                 try {
-                                    a = await bt.ServerConnection.makeRequest(n, t, o)
+                                    a = await Tt.ServerConnection.makeRequest(n, t, o)
                                 } catch (e) {
-                                    throw new bt.ServerConnection.NetworkError(e)
+                                    throw new Tt.ServerConnection.NetworkError(e)
                                 }
                                 const s = await a.text();
-                                if (!a.ok) throw new bt.ServerConnection.ResponseError(a, s.message || s);
+                                if (!a.ok) throw new Tt.ServerConnection.ResponseError(a, s.message || s);
                                 return s
                             }("get_anonymized_user_id");
-                        if (r && ((e, t) => {
+                        if (i && ((e, t) => {
                                 const o = e.split(/[^0-9]+/).map(Number),
                                     n = t.split(/[^0-9]+/).map(Number);
                                 for (let e = 0; e < Math.min(o.length, n.length); e++) {
                                     const t = o[e],
                                         a = n[e];
                                     if (t !== a) return t - a
                                 }
                                 const a = e.replace(/[0-9]+/g, ""),
                                     s = t.replace(/[0-9]+/g, "");
                                 return a.localeCompare(s)
                             })(e.version, l) >= 0) {
-                            const l = parseInt(r[0]);
+                            const l = parseInt(i[0]);
                             w.setJupyterVersion(l).then((() => {
                                 d.then((l => {
-                                    Ct = l;
-                                    let r = [];
-                                    fetch(`${i}/auth/login`, {
+                                    Lt = l;
+                                    let i = [];
+                                    fetch(`${r}/auth/login`, {
                                         method: "POST",
                                         headers: {
-                                            "Unianalytics-User-Id": Ct
+                                            "Unianalytics-User-Id": Lt
                                         }
                                     }).then((e => {
                                         if (e.ok) return e.json();
                                         throw new Error("Unauthorized user")
                                     })).then((l => {
-                                        "logged_in" === l.status ? (r = l.auth_notebooks || [], sessionStorage.setItem(h, l.access_token), sessionStorage.setItem(m, l.refresh_token), function(e, t) {
-                                            console.log(`JupyterLab extension ${c}: upload plugin is activated!`), e.commands.addCommand(u.uploadNotebook, {
+                                        "logged_in" === l.status ? (i = l.auth_notebooks || [], sessionStorage.setItem(h, l.access_token), sessionStorage.setItem(u, l.refresh_token), function(e, t) {
+                                            console.log(`JupyterLab extension ${c}: upload plugin is activated!`), e.commands.addCommand(p.uploadNotebook, {
                                                 label: "Upload notebook to unianalytics",
-                                                icon: e => e.isContextMenu ? S.fileUploadIcon : void 0,
+                                                icon: e => e.isContextMenu ? x.fileUploadIcon : void 0,
                                                 execute: o => {
                                                     const n = w.getFileComp(t);
                                                     n && e.serviceManager.contents.get(n.path).then((t => {
                                                         var o, a;
                                                         (o = t.content, a = n.name, new Promise(((e, t) => {
                                                             const n = new FormData;
-                                                            n.append("notebook_content", JSON.stringify(o)), n.append("name", a), v(i + "/notebook/upload", {
+                                                            n.append("notebook_content", JSON.stringify(o)), n.append("name", a), E(r + "/notebook/upload", {
                                                                 method: "POST",
                                                                 body: n
                                                             }).then((o => {
                                                                 o.ok ? e(o.json()) : t(new Error("Failed to upload notebook on the backend"))
                                                             })).catch((e => {
                                                                 console.log(`${c}: Error occurred while uploading notebook:`, e), t(e)
                                                             }))
                                                         }))).then((o => {
                                                             const a = {
                                                                 ...t,
                                                                 content: o
                                                             };
                                                             e.serviceManager.contents.save(n.path, a).then((e => {
                                                                 const t = o.metadata[_.notebookId],
-                                                                    a = `${i}/notebook/download/${t}`;
-                                                                (0, O.showDialog)({
+                                                                    a = `${r}/notebook/download/${t}`;
+                                                                (0, I.showDialog)({
                                                                     title: n.name,
-                                                                    body: y().createElement(D, {
+                                                                    body: N().createElement(T, {
                                                                         url: a,
                                                                         fileName: n.name
                                                                     }),
-                                                                    buttons: [O.Dialog.okButton()]
+                                                                    buttons: [I.Dialog.okButton()]
                                                                 }).catch((e => console.log(e)))
                                                             }))
                                                         })).catch((e => {
-                                                            (0, O.showDialog)({
+                                                            (0, I.showDialog)({
                                                                 title: n.name,
                                                                 body: "Error uploading the file",
-                                                                buttons: [O.Dialog.cancelButton()]
+                                                                buttons: [I.Dialog.cancelButton()]
                                                             }).catch((e => console.log(e)))
                                                         }))
                                                     }))
                                                 }
-                                            }), e.commands.addCommand(u.copyDownloadLink, {
+                                            }), e.commands.addCommand(p.copyDownloadLink, {
                                                 label: "Copy unianalytics notebook link",
-                                                icon: e => e.isContextMenu ? S.linkIcon : void 0,
+                                                icon: e => e.isContextMenu ? x.linkIcon : void 0,
                                                 execute: o => {
                                                     const n = w.getFileComp(t);
                                                     n && e.serviceManager.contents.get(n.path).then((e => {
                                                         const t = e.content.metadata;
                                                         if (t) {
                                                             const e = t[_.notebookId];
-                                                            e ? navigator.clipboard.writeText(`${i}/notebook/download/${e}`).catch((e => {
+                                                            e ? navigator.clipboard.writeText(`${r}/notebook/download/${e}`).catch((e => {
                                                                 console.error(`${c}: Error copying link: `, e)
                                                             })) : console.log(`${c}: Notebook not tagged`)
                                                         }
                                                     }))
                                                 }
                                             }), e.contextMenu.addItem({
-                                                selector: p,
+                                                selector: g,
                                                 type: "separator",
                                                 rank: 0
                                             }), e.contextMenu.addItem({
                                                 args: {
                                                     isContextMenu: !0
                                                 },
-                                                command: u.uploadNotebook,
-                                                selector: p,
+                                                command: p.uploadNotebook,
+                                                selector: g,
                                                 rank: 0
                                             }), e.contextMenu.addItem({
                                                 args: {
                                                     isContextMenu: !0
                                                 },
-                                                command: u.copyDownloadLink,
-                                                selector: p,
+                                                command: p.copyDownloadLink,
+                                                selector: g,
                                                 rank: 0
                                             }), e.contextMenu.addItem({
-                                                selector: p,
+                                                selector: g,
                                                 type: "separator",
                                                 rank: 0
                                             })
                                         }(e, t), async function(e, t, o, n, a) {
                                             let s;
                                             if (console.log(`JupyterLab extension ${c}: dashboard plugins activated!`), n) try {
                                                 s = await n.load(`${c}:plugin`), h(s), s.changed.connect(h)
                                             } catch (e) {
                                                 console.error(`${c}: Failed to load settings.\n${e}`)
                                             }(e => {
                                                 const t = e.shell.widgets();
                                                 let o = w.getNextWidgetValueComp(t);
                                                 for (; o;) {
-                                                    if (o instanceof Y.NotebookPanel) {
+                                                    if (o instanceof ie.NotebookPanel) {
                                                         const t = o,
-                                                            n = new gt(e.commands),
-                                                            a = new mt(e.commands),
+                                                            n = new xt(e.commands),
+                                                            a = new Ot(e.commands),
                                                             s = n.createNew(t),
                                                             l = a.createNew(t);
                                                         t.disposed.connect((() => {
                                                             s.dispose(), l.dispose()
                                                         }))
                                                     }
                                                     o = w.getNextWidgetValueComp(t)
                                                 }
-                                                e.docRegistry.addWidgetExtension("Notebook", new mt(e.commands)), e.docRegistry.addWidgetExtension("Notebook", new gt(e.commands))
+                                                e.docRegistry.addWidgetExtension("Notebook", new Ot(e.commands)), e.docRegistry.addWidgetExtension("Notebook", new xt(e.commands))
                                             })(e);
-                                            const l = new le,
-                                                i = new $e(l, a.sanitizer),
-                                                r = new rt(l, e.commands, a.sanitizer, s);
+                                            const l = new ge,
+                                                r = new tt(l, a.sanitizer),
+                                                i = new Et(l, e.commands, a.sanitizer, s);
 
                                             function d() {
                                                 const t = e.shell.currentWidget;
                                                 if (!t) return;
-                                                if (!(t instanceof Y.NotebookPanel)) return void(l.panel && l.panel.isDisposed && (l.panel = null));
+                                                if (!(t instanceof ie.NotebookPanel)) return void(l.panel && l.panel.isDisposed && (l.panel = null));
                                                 const o = t;
                                                 l.panel = o
                                             }
 
                                             function h(e) {
-                                                var t, o;
-                                                const n = e.composite.commonDashboardSettings;
-                                                let a;
-                                                n ? (a = n.realTime, ue.setPermission(n.dashboardCollection || !1)) : (a = null === (t = e.default("commonDashboardSettings")) || void 0 === t ? void 0 : t.realTime, ue.setPermission((null === (o = e.default("commonDashboardSettings")) || void 0 === o ? void 0 : o.dashboardCollection) || !1)), null === a && void 0 === a || _t(J(a))
+                                                var t;
+                                                const o = e.composite.commonDashboardSettings;
+                                                o ? ye.setPermission(o.dashboardCollection || !1) : ye.setPermission((null === (t = e.default("commonDashboardSettings")) || void 0 === t ? void 0 : t.dashboardCollection) || !1)
                                             }
-                                            o.add(i, "right", {
+                                            o.add(r, "right", {
                                                 rank: 1e3
-                                            }), o.add(r, "left", {
+                                            }), o.add(i, "left", {
                                                 rank: 1e3
-                                            }), e.commands.addCommand(u.dashboardOpenVisu, {
+                                            }), e.commands.addCommand(p.dashboardOpenVisu, {
                                                 label: "Notebook Visualizations",
                                                 caption: "Open Notebook Dashboard",
-                                                icon: x,
+                                                icon: R,
                                                 iconClass: "jp-icon3",
                                                 execute: t => {
-                                                    "Notebook" === t.from ? (ue.sendInteraction({
+                                                    "Notebook" === t.from ? (ye.sendInteraction({
                                                         click_type: "ON",
-                                                        signal_origin: Q.NOTEBOOK_TOOLBAR_BUTTON
-                                                    }), _t(U())) : "Cell" === t.from ? (ue.sendInteraction({
+                                                        signal_origin: re.NOTEBOOK_TOOLBAR_BUTTON
+                                                    }), It(z())) : "Cell" === t.from ? (ye.sendInteraction({
                                                         click_type: "ON",
-                                                        signal_origin: Q.NOTEBOOK_CELL_BUTTON
-                                                    }), _t(F({
+                                                        signal_origin: re.NOTEBOOK_CELL_BUTTON
+                                                    }), It(j({
                                                         cellId: t.cell_id
-                                                    }))) : "Toc" === t.from && (ue.sendInteraction({
+                                                    }))) : "Toc" === t.from && (ye.sendInteraction({
                                                         click_type: "ON",
-                                                        signal_origin: Q.TOC_OPEN_CELL_DASHBOARD
-                                                    }), _t(F({
+                                                        signal_origin: re.TOC_OPEN_CELL_DASHBOARD
+                                                    }), It(j({
                                                         cellId: t.cell_id
-                                                    }))), i.isVisible || e.shell.activateById(i.id)
+                                                    }))), r.isVisible || e.shell.activateById(r.id)
                                                 }
-                                            }), t && (t.add(i, `${c}:dashboard-notebook-restorer`), t.add(r, `${c}:dashboard-toc-restorer`)), o && o.currentChanged.connect(d), e.restored.then((() => {
+                                            }), t && (t.add(r, `${c}:dashboard-notebook-restorer`), t.add(i, `${c}:dashboard-toc-restorer`)), o && o.currentChanged.connect(d), e.restored.then((() => {
                                                 d()
                                             }))
                                         }(e, o, n, s, a)) : console.log(`${c}: User not authenticated`)
                                     })).catch((e => {
                                         console.log(`${c}: Authentication error, ${e}`)
                                     })).finally((() => {
                                         window.postMessage({
                                             identifier: "unianalytics",
-                                            authNotebooks: r
+                                            authNotebooks: i
                                         }, window.origin)
                                     }))
                                 })).catch((e => {
                                     console.error(`${c}: Failed to access userId, the jupyterlab_unianalytics_dashboard server extension appears to be missing.\n${e}`)
                                 }))
                             }))
                         } else console.log(`${c}: Use a more recent version of JupyterLab (>=${l})`)
                     }
                 },
-                Et = kt
+                Bt = Mt
         },
         2204: e => {
             e.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%27-4 -4 8 8%27%3e%3ccircle r=%272%27 fill=%27%23fff%27/%3e%3c/svg%3e"
         },
         9609: e => {
             e.exports = "data:image/svg+xml,%3csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%27-4 -4 8 8%27%3e%3ccircle r=%273%27 fill=%27%2386b7fe%27/%3e%3c/svg%3e"
         },
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/18.759fbf2374edc42b5c3e.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/18.759fbf2374edc42b5c3e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/308.d9da4ce35f354c6f12e1.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/308.d9da4ce35f354c6f12e1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/39.5a3b28a79ba693a9b627.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/39.5a3b28a79ba693a9b627.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/426.a7015f9dfda310972c1b.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/426.a7015f9dfda310972c1b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/546.a8f5ba1be2a764c64287.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/546.d5da555479f21a401709.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,87 +1,87 @@
 "use strict";
 (self.webpackChunkjupyterlab_unianalytics_dashboard = self.webpackChunkjupyterlab_unianalytics_dashboard || []).push([
     [546], {
         1150: (n, o, e) => {
             e.d(o, {
-                Z: () => i
+                Z: () => d
             });
             var r = e(8081),
                 t = e.n(r),
                 a = e(3645),
-                l = e.n(a)()(t());
-            l.push([n.id, ".cell-dashboard-button-container {\n  position: absolute;\n  left: 13px;\n  bottom: -29px;\n  width: var(--jp-cell-prompt-width);\n  height: 34px;\n  z-index: 9999;\n}\n\n.cell-dashboard-button {\n  cursor: pointer;\n  background-color: var(--jp-brand-color1);\n  border-radius: 0 0 5px 5px;\n  border: none;\n  padding: 0;\n  width: 100%;\n  height: 100%;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\n\n.cell-dashboard-button:hover {\n  background-color: var(--jp-brand-color0);\n}\n\n.cell-dashboard-button:disabled {\n  background-color: var(--jp-inverse-layout-color4);\n  cursor: not-allowed;\n}\n\n.cell-dashboard-button svg {\n  width: 20px;\n  height: 20px;\n}\n\n.cell-dashboard-button [fill] {\n  fill: white;\n}\n\n.dashboard-export-dialog-container {\n  padding: 20px 0;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n}\n\n.dashboard-export-dialog-container p {\n  font-size: var(--jp-ui-font-size2);\n  font-weight: 400;\n  padding-left: 8px;\n}\n\n.dashboard-export-dialog-calendar-container {\n  display: flex;\n  flex-wrap: wrap;\n  justify-content: center;\n  gap: 15px;\n}\n\n.dashboard-export-dialog-calendar {\n  border: 1px solid var(--jp-brand-color1);\n  border-radius: 3px;\n  display: flex;\n  flex-direction: column;\n  padding: 20px;\n}\n", ""]);
-            const i = l
+                i = e.n(a)()(t());
+            i.push([n.id, ".cell-dashboard-button-container {\n  position: absolute;\n  left: 13px;\n  bottom: -29px;\n  width: var(--jp-cell-prompt-width);\n  height: 34px;\n  z-index: 9999;\n}\n\n.cell-dashboard-button {\n  cursor: pointer;\n  background-color: var(--jp-brand-color1);\n  border-radius: 0 0 5px 5px;\n  border: none;\n  padding: 0;\n  width: 100%;\n  height: 100%;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\n\n.cell-dashboard-button:hover {\n  background-color: var(--jp-brand-color0);\n}\n\n.cell-dashboard-button:disabled {\n  background-color: var(--jp-inverse-layout-color4);\n  cursor: not-allowed;\n}\n\n.cell-dashboard-button svg {\n  width: 20px;\n  height: 20px;\n}\n\n.cell-dashboard-button [fill] {\n  fill: white;\n}\n\n.dashboard-export-dialog-container {\n  padding: 20px 0;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n}\n\n.dashboard-export-dialog-container p {\n  font-size: var(--jp-ui-font-size2);\n  font-weight: 400;\n  padding-left: 8px;\n}\n\n.dashboard-export-dialog-calendar-container {\n  display: flex;\n  flex-wrap: wrap;\n  justify-content: center;\n  gap: 15px;\n  cursor: default;\n  padding: 20px;\n}\n\n.dashboard-export-dialog-calendar {\n  border: 1px solid var(--jp-brand-color1);\n  border-radius: 3px;\n  display: flex;\n  flex-direction: column;\n  padding: 20px;\n  cursor: pointer;\n}\n\n.dashboard-calendar-container {\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n  justify-content: center;\n  gap: 12px;\n  padding: 14px 20px;\n}\n\ninput.dashboard-calendar-input {\n  cursor: pointer;\n}\n\nbody[data-jp-theme-light='false'] input.dashboard-calendar-input {\n  color-scheme: dark;\n}\n\n.dashboard-calendar-input-wrapper {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  gap: 15px;\n}\n\n.dashboard-calendar-input-wrapper.disabled {\n  opacity: 0.4;\n  cursor: not-allowed;\n}\n\n.dashboard-calendar-input-wrapper.disabled input.dashboard-calendar-input {\n  pointer-events: none;\n  background-color: var(--jp-layout-color4);\n}\n\n.dashboard-calendar-button-container {\n  display: flex;\n  justify-content: space-between;\n  padding: 20px 15px 5px;\n}\n", ""]);
+            const d = i
         },
         3630: (n, o, e) => {
             e.d(o, {
-                Z: () => i
+                Z: () => d
             });
             var r = e(8081),
                 t = e.n(r),
                 a = e(3645),
-                l = e.n(a)()(t());
-            l.push([n.id, ".dashboard-panel {\n  background-color: var(--jp-layout-color1);\n}\n\n.dashboard-react-widget {\n  display: flex;\n  height: 100%;\n  min-width: 320px !important;\n}\n\n.page-container {\n  display: flex;\n  overflow-y: auto;\n  scrollbar-gutter: stable;\n  padding: 20px;\n  flex-direction: column;\n  flex: 1;\n}\n\n.chart-card {\n  max-height: 400px;\n}\n\n.chart-card-title {\n  text-align: center;\n  padding-top: 15px;\n  font-size: medium !important;\n}\n\n.chart-card-body {\n  min-height: 240px;\n}\n\n.breadcrumb-container {\n  margin-bottom: 16px;\n  display: flex;\n  flex-wrap: wrap;\n  align-items: center;\n}\n\n.breadcrumb-tile {\n  padding: 2px 13px 2px 8px;\n  border-radius: 0 60px 60px 0;\n  cursor: pointer;\n  color: var(--jp-inverse-layout-color1);\n  font-weight: 500;\n  font-size: 20px;\n  background-color: var(--jp-border-color1);\n  opacity: 0.5;\n}\n\n.breadcrumb-tile-active {\n  opacity: 1;\n  background-color: var(--jp-brand-color1);\n  color: white;\n}\n\n.breadcrumb-buttons-container {\n  margin-left: auto;\n}\n\n.breadcrumb-button {\n  margin-left: 6px;\n  background-color: var(--jp-brand-color1) !important;\n  border: none !important;\n}\n\n.breadcrumb-button:hover {\n  background-color: var(--jp-brand-color0) !important;\n}\n\n.dashboard-title-container {\n  display: flex;\n  margin-bottom: 15px;\n  justify-content: space-between;\n}\n\n.dashboard-title-text {\n  white-space: nowrap; /* Prevent text from wrapping */\n  overflow: hidden; /* Hide overflowing content */\n  text-overflow: ellipsis;\n\n  /* max-width: 80%; */\n  font-size: 22px;\n  color: var(--jp-inverse-layout-color1);\n  font-weight: 700;\n}\n\n.card {\n  color: var(--jp-inverse-layout-color1) !important;\n  background-color: var(--jp-layout-color2) !important;\n  cursor: pointer;\n\n  /* box-shadow: var(--jp-inverse-layout-color4) 0 0 5px 0; */\n}\n\n.cell-card {\n  cursor: pointer;\n  margin-bottom: 10px;\n  margin-top: 10px;\n  padding: 0;\n}\n\n.cell-card-wrapper {\n  display: flex;\n  align-items: center;\n}\n\n.cell-filter-container {\n  display: flex;\n  flex-wrap: wrap;\n  gap: 10px;\n  justify-content: space-between;\n  color: var(--jp-inverse-layout-color1);\n}\n\n.cell-filter-container .form-control,\n.cell-filter-container .form-control:focus {\n  border: solid 1px var(--jp-brand-color1);\n  background-color: transparent;\n  color: var(--jp-inverse-layout-color1);\n}\n\n.cell-filter-container .form-control::placeholder {\n  color: var(--jp-inverse-layout-color3);\n}\n\n.cell-radio-container .btn-group .btn {\n  display: flex;\n  align-items: center;\n}\n\n.dashboard-dropdown-container {\n  display: flex;\n  margin-left: 10px;\n  gap: 5px;\n}\n\n.custom-dropdown .dropdown-menu {\n  background-color: var(--jp-layout-color3);\n}\n\n.custom-dropdown .dropdown-item {\n  color: var(--jp-inverse-layout-color1);\n}\n\n.custom-dropdown .dropdown-item:hover {\n  background-color: var(--jp-layout-color2);\n  color: var(--jp-inverse-layout-color1);\n}\n\n.custom-dropdown .dropdown-header {\n  color: var(--jp-inverse-layout-color3);\n}\n\n.cell-user-title {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  font-size: 13px;\n  font-weight: 500;\n  padding: 0 0 10px;\n}\n\n.cell-content-container {\n  max-height: 320px;\n  overflow: auto;\n  padding: 10px;\n  background-color: var(--jp-layout-color0);\n  border: solid 1px var(--bs-card-border-color);\n  border-radius: 3px;\n  cursor: pointer;\n}\n\n.cell-content-container:hover {\n  cursor: text;\n}\n\n.logo {\n  width: 18px;\n  height: 18px;\n}\n\n.labicon-logo .jp-icon3 {\n  fill: white;\n}\n\n.no-data-card {\n  margin: 10px 0;\n  text-align: center;\n  padding: 30px 0;\n}\n\n.connectionid-container {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  width: 100%;\n  padding: 6px 10px;\n  border-radius: 2px;\n  margin-bottom: 6px;\n  font-size: 11px;\n  color: white;\n  cursor: pointer;\n}\n\n.connectionid-container:hover {\n  background-color: #424242;\n}\n\n.text-with-ellipsis {\n  flex: 1;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  margin-right: 10px;\n}\n\n.send-icon {\n  display: flex;\n  justify-content: center;\n}\n", ""]);
-            const i = l
+                i = e.n(a)()(t());
+            i.push([n.id, ".dashboard-panel {\n  background-color: var(--jp-layout-color1);\n}\n\n.dashboard-react-widget {\n  display: flex;\n  height: 100%;\n  min-width: 335px !important;\n}\n\n.page-container {\n  display: flex;\n  overflow-y: auto;\n  scrollbar-gutter: stable;\n  padding: 20px;\n  flex-direction: column;\n  flex: 1;\n}\n\n.chart-card {\n  max-height: 400px;\n}\n\n.chart-card-title {\n  text-align: center;\n  padding-top: 15px;\n  font-size: medium !important;\n}\n\n.chart-card-body {\n  min-height: 240px;\n}\n\n.breadcrumb-container {\n  margin-bottom: 16px;\n  display: flex;\n  flex-wrap: wrap;\n  align-items: center;\n}\n\n.breadcrumb-tile {\n  padding: 2px 13px 2px 8px;\n  border-radius: 0 60px 60px 0;\n  cursor: pointer;\n  color: var(--jp-inverse-layout-color1);\n  font-weight: 500;\n  font-size: 20px;\n  background-color: var(--jp-border-color1);\n  opacity: 0.5;\n}\n\n.breadcrumb-tile-active {\n  opacity: 1;\n  background-color: var(--jp-brand-color1);\n  color: white;\n}\n\n.breadcrumb-buttons-container {\n  margin-left: auto;\n  position: relative;\n}\n\n.dashboard-title-container {\n  display: flex;\n  margin-bottom: 15px;\n  justify-content: space-between;\n  align-items: center;\n}\n\n.dashboard-title-text {\n  white-space: nowrap; /* Prevent text from wrapping */\n  overflow: hidden; /* Hide overflowing content */\n  text-overflow: ellipsis;\n  font-size: 18px;\n  color: var(--jp-inverse-layout-color1);\n  font-weight: 700;\n}\n\n.card {\n  color: var(--jp-inverse-layout-color1) !important;\n  background-color: var(--jp-layout-color2) !important;\n  cursor: pointer;\n\n  /* box-shadow: var(--jp-inverse-layout-color4) 0 0 5px 0; */\n}\n\n.cell-card {\n  cursor: pointer;\n  margin-bottom: 10px;\n  margin-top: 10px;\n  padding: 0;\n}\n\n.cell-card-wrapper {\n  display: flex;\n  align-items: center;\n}\n\n.cell-filter-container {\n  display: flex;\n  flex-wrap: wrap;\n  gap: 10px;\n  justify-content: space-between;\n  color: var(--jp-inverse-layout-color1);\n}\n\n.cell-filter-container .form-control,\n.cell-filter-container .form-control:focus {\n  border: solid 1px var(--jp-brand-color1);\n  background-color: transparent;\n  color: var(--jp-inverse-layout-color1);\n}\n\n.cell-filter-container .form-control::placeholder {\n  color: var(--jp-inverse-layout-color3);\n}\n\n.cell-radio-container .btn-group .btn {\n  display: flex;\n  align-items: center;\n}\n\n.cell-radio-container .btn-outline-primary {\n  border: solid 1px var(--jp-brand-color1);\n}\n\n.dashboard-dropdown-container {\n  display: flex;\n  margin-left: 10px;\n  gap: 5px;\n}\n\n.custom-dropdown .dropdown-menu,\n.custom-dropdown .dropdown-item,\n.custom-dropdown .dropdown-header {\n  background-color: var(--jp-layout-color2) !important;\n  color: var(--jp-inverse-layout-color1) !important;\n}\n\n.custom-dropdown .dropdown-item:hover,\n.custom-dropdown .dropdown-item.highlighted {\n  background-color: var(--jp-layout-color3) !important;\n}\n\n.custom-dropdown .dropdown-toggle::after {\n  display: none !important;\n}\n\n.custom-dropdown .dropdown-menu {\n  border-width: 2px;\n}\n\nbutton.dashboard-button {\n  width: 32px;\n  height: 32px;\n  display: flex;\n  justify-content: center;\n  align-items: center;\n}\n\n.cell-user-title {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  font-size: 13px;\n  font-weight: 500;\n  padding: 0 0 10px;\n}\n\n.cell-execution-displayed-time {\n  display: flex;\n  justify-content: end;\n  font-size: 12px;\n  font-weight: 400;\n  padding-top: 12px;\n}\n\n.cell-content-container {\n  max-height: 320px;\n  overflow: auto;\n  padding: 10px;\n  background-color: var(--jp-layout-color0);\n  border: solid 1px var(--bs-card-border-color);\n  border-radius: 3px;\n  cursor: pointer;\n}\n\n.cell-content-container:hover {\n  cursor: text;\n}\n\n.dashboard-icon {\n  width: 20px;\n  height: auto;\n  position: absolute;\n}\n\n.dashboard-icon .jp-icon3 {\n  fill: white;\n}\n\n.no-data-card {\n  margin: 10px 0;\n  text-align: center;\n  padding: 30px 0;\n}\n\n.connectionid-container {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  width: 100%;\n  padding: 6px 10px;\n  border-radius: 2px;\n  margin-bottom: 6px;\n  font-size: 11px;\n  color: white;\n  cursor: pointer;\n}\n\n.connectionid-container:hover {\n  background-color: #424242;\n}\n\n.text-with-ellipsis {\n  flex: 1;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  margin-right: 10px;\n}\n\n.send-icon {\n  display: flex;\n  justify-content: center;\n}\n\n.custom-dropdown-container {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  padding: 6px 0;\n}\n\n.group-dropdown-scroll {\n  max-height: 215px;\n  overflow-y: auto;\n}\n\n.group-dropdown-scroll.disabled {\n  opacity: 0.4;\n  cursor: not-allowed;\n}\n\n.custom-dropdown-item {\n  padding: 8px 10px 4px 12px;\n}\n\n.custom-dropdown-item,\n.custom-dropdown-item * {\n  cursor: pointer !important;\n}\n\n.custom-dropdown-item.disabled,\n.custom-dropdown-item.disabled * {\n  cursor: not-allowed !important;\n}\n\n.custom-dropdown-item:hover:not(.disabled) {\n  background-color: var(--jp-layout-color3) !important;\n}\n\n.custom-dropdown-item label {\n  max-width: 190px;\n  overflow-x: hidden;\n  white-space: nowrap;\n  text-overflow: ellipsis;\n}\n", ""]);
+            const d = i
         },
         7563: (n, o, e) => {
             e.d(o, {
-                Z: () => i
+                Z: () => d
             });
             var r = e(8081),
                 t = e.n(r),
                 a = e(3645),
-                l = e.n(a)()(t());
-            l.push([n.id, ".dashboard-TableOfContents-content {\n  flex: 1 1 auto;\n  margin: 0;\n  padding: 0;\n  list-style-type: none;\n  overflow: auto;\n  background-color: var(--jp-layout-color1);\n}\n\n.dashboard-TableOfContents-content li {\n  display: flex;\n  flex-direction: row;\n  padding: 4px 12px;\n  -webkit-user-select: none;\n  -moz-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n  cursor: pointer;\n  padding-top: 8px;\n  padding-bottom: 8px;\n  width: 100%;\n}\n\n.dashboard-TableOfContents {\n  display: flex;\n  flex-direction: column;\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size1);\n  height: 100%;\n  width: 100%;\n}\n\n.dashboard-TableOfContents .dashboard-stack-panel-header {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  text-transform: uppercase;\n  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\n  flex: 0 0 auto;\n  font-size: var(--jp-ui-font-size0);\n  font-weight: 600;\n  letter-spacing: 1px;\n  margin: 0;\n  padding: 8px 12px;\n}\n\n.dashboard-toc-toolbar-icon,\n.dashboard-toc-toolbar-icon-selected {\n  float: left;\n  padding: 0;\n  margin: 4px;\n  display: flex;\n  cursor: pointer;\n  justify-content: center;\n  align-items: center;\n  background-repeat: no-repeat;\n  background-color: transparent;\n  background-size: 100%;\n  background-position: center;\n  height: 24px;\n  width: 24px;\n  border-radius: 2px;\n}\n\n[data-jp-theme-light='true'] .dashboard-toc-toolbar-icon:hover {\n  background-color: var(--jp-input-background);\n}\n\n[data-jp-theme-light='false'] .dashboard-toc-toolbar-icon:hover {\n  background-color: #3a3a3a;\n}\n\n[data-jp-theme-light='true'] .dashboard-toc-toolbar-icon-selected {\n  background-color: var(--jp-layout-color2);\n}\n\n[data-jp-theme-light='false'] .dashboard-toc-toolbar-icon-selected {\n  background-color: #565656;\n}\n\n.dashboard-toc-toolbar {\n  position: relative;\n  width: 100%;\n  margin: 0;\n  padding: 0 2px;\n  user-select: none;\n  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\n  height: 36px;\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n}\n\n.dashboard-toc-toolbar-compartment {\n  display: flex;\n}\n\n.dashboard-toc-entry-holder {\n  flex-grow: 1;\n  display: flex;\n  flex-direction: row;\n  padding: 2px 0;\n  margin: 0;\n  overflow: hidden;\n}\n\n.dashboard-toc-cell-item {\n  padding-left: 10px;\n  font-size: var(--jp-ui-font-size1);\n\n  /* single line */\n  white-space: nowrap;\n  overflow: hidden;\n\n  /* add ellipsis (...) if content overflows */\n  text-overflow: ellipsis;\n}\n\n.dashboard-toc-Collapser-child {\n  display: block;\n  background: transparent;\n  width: 100%;\n  box-sizing: border-box;\n  position: absolute;\n  top: 0;\n  bottom: 0;\n}\n\n.dashboard-toc-Collapser-child:hover {\n  box-shadow: var(--jp-elevation-z2);\n  background: var(--jp-brand-color1);\n  opacity: var(--jp-cell-collapser-not-active-hover-opacity);\n}\n\n.dashboard-toc-active-cell .dashboard-toc-Collapser-child {\n  background: var(--jp-brand-color1);\n}\n\n.dashboard-toc-entry-holder:hover .dashboard-toc-Collapser-child {\n  box-shadow: var(--jp-elevation-z2);\n  background: var(--jp-brand-color1);\n  opacity: var(--jp-cell-collapser-not-active-hover-opacity);\n}\n\n.dashboard-toc-active-cell .dashboard-toc-Collapser-child:hover {\n  background: var(--jp-brand-color0);\n  opacity: 1;\n}\n\n.dashboard-toc-active-cell:hover .dashboard-toc-Collapser-child {\n  background: var(--jp-brand-color0);\n  opacity: 1;\n}\n\n.dashboard-TableOfContents-content code {\n  font-size: inherit;\n}\n\n.dashboard-toc-Ellipses {\n  height: 16px;\n  margin-left: auto;\n}\n\n.dashboard-toc-Ellipses:hover {\n  border: 1px solid var(--jp-border-color1);\n  box-shadow: 0 0 2px 0 rgba(0 0 0 / 25%);\n  background-color: var(--jp-layout-color0);\n}\n\n.dashboard-toc-level-size-2 {\n  margin-left: 16px;\n}\n\n.dashboard-toc-level-size-3 {\n  margin-left: 36px;\n}\n\n.dashboard-toc-level-size-4 {\n  margin-left: 56px;\n}\n\n.dashboard-toc-level-size-5 {\n  margin-left: 76px;\n}\n\n.dashboard-TableOfContents-placeholder {\n  text-align: center;\n}\n\n.dashboard-TableOfContents-placeholderContent {\n  color: var(--jp-content-font-color2);\n  padding: 25px 30px 8px;\n}\n\n.dashboard-toc-react-component {\n  display: flex;\n  align-items: center;\n  border-radius: 2px;\n  padding: 2px;\n  min-width: 52px;\n  margin-left: 5px;\n  font-size: small;\n  text-align: center;\n  word-wrap: break-word;\n}\n\n.dashboard-toc-react-text {\n  width: 100%;\n  color: var(--jp-inverse-layout-color0);\n}\n\n.dashboard-toc-header-title {\n  overflow: hidden;\n  white-space: nowrap;\n  text-overflow: ellipsis;\n  margin-right: 5px;\n}\n\n.dashboard-toc-download-button {\n  cursor: pointer;\n  padding: 3px 6px;\n  border-radius: 2px;\n  display: flex;\n  align-items: center;\n  color: white;\n  background-color: var(--jp-brand-color1);\n}\n\n.dashboard-toc-download-button:hover {\n  background-color: var(--jp-brand-color0);\n}\n\n.dashboard-toc-download-button-disabled {\n  cursor: wait;\n  padding: 3px 6px;\n  border-radius: 2px;\n  display: flex;\n  align-items: center;\n  color: white;\n  background-color: #575b5b;\n}\n\n.dashboard-toc-download-icon {\n  margin-right: 4px;\n}\n\n.dashboard-toc-download-icon .jp-icon3 {\n  fill: white;\n}\n", ""]);
-            const i = l
+                i = e.n(a)()(t());
+            i.push([n.id, ".dashboard-TableOfContents-content {\n  flex: 1 1 auto;\n  margin: 0;\n  padding: 0;\n  list-style-type: none;\n  overflow: auto;\n  background-color: var(--jp-layout-color1);\n}\n\n.dashboard-TableOfContents-content li {\n  display: flex;\n  flex-direction: row;\n  padding: 4px 12px;\n  -webkit-user-select: none;\n  -moz-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n  cursor: pointer;\n  padding-top: 8px;\n  padding-bottom: 8px;\n  width: 100%;\n}\n\n.dashboard-TableOfContents {\n  display: flex;\n  flex-direction: column;\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size1);\n  height: 100%;\n  width: 100%;\n}\n\n.dashboard-TableOfContents .dashboard-stack-panel-header {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  text-transform: uppercase;\n  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\n  flex: 0 0 auto;\n  font-size: var(--jp-ui-font-size0);\n  font-weight: 600;\n  letter-spacing: 1px;\n  margin: 0;\n  padding: 8px 12px;\n}\n\n.dashboard-toc-toolbar-icon,\n.dashboard-toc-toolbar-icon-selected {\n  float: left;\n  padding: 0;\n  margin: 4px;\n  display: flex;\n  cursor: pointer;\n  justify-content: center;\n  align-items: center;\n  background-repeat: no-repeat;\n  background-color: transparent;\n  background-size: 100%;\n  background-position: center;\n  height: 24px;\n  width: 24px;\n  border-radius: 2px;\n}\n\n[data-jp-theme-light='true'] .dashboard-toc-toolbar-icon:hover {\n  background-color: var(--jp-input-background);\n}\n\n[data-jp-theme-light='false'] .dashboard-toc-toolbar-icon:hover {\n  background-color: #3a3a3a;\n}\n\n[data-jp-theme-light='true'] .dashboard-toc-toolbar-icon-selected {\n  background-color: var(--jp-layout-color2);\n}\n\n[data-jp-theme-light='false'] .dashboard-toc-toolbar-icon-selected {\n  background-color: #565656;\n}\n\n.dashboard-toc-toolbar {\n  position: relative;\n  width: 100%;\n  margin: 0;\n  padding: 0 2px;\n  user-select: none;\n  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\n  height: 36px;\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n}\n\n.dashboard-toc-toolbar-compartment {\n  display: flex;\n}\n\n.dashboard-toc-entry-holder {\n  flex-grow: 1;\n  display: flex;\n  flex-direction: row;\n  padding: 2px 0;\n  margin: 0;\n  overflow: hidden;\n}\n\n.dashboard-toc-cell-item {\n  padding-left: 10px;\n  font-size: var(--jp-ui-font-size1);\n\n  /* single line */\n  white-space: nowrap;\n  overflow: hidden;\n\n  /* add ellipsis (...) if content overflows */\n  text-overflow: ellipsis;\n}\n\n.dashboard-toc-Collapser-child {\n  display: block;\n  background: transparent;\n  width: 100%;\n  box-sizing: border-box;\n  position: absolute;\n  top: 0;\n  bottom: 0;\n}\n\n.dashboard-toc-Collapser-child:hover {\n  box-shadow: var(--jp-elevation-z2);\n  background: var(--jp-brand-color1);\n  opacity: var(--jp-cell-collapser-not-active-hover-opacity);\n}\n\n.dashboard-toc-active-cell .dashboard-toc-Collapser-child {\n  background: var(--jp-brand-color1);\n}\n\n.dashboard-toc-entry-holder:hover .dashboard-toc-Collapser-child {\n  box-shadow: var(--jp-elevation-z2);\n  background: var(--jp-brand-color1);\n  opacity: var(--jp-cell-collapser-not-active-hover-opacity);\n}\n\n.dashboard-toc-active-cell .dashboard-toc-Collapser-child:hover {\n  background: var(--jp-brand-color0);\n  opacity: 1;\n}\n\n.dashboard-toc-active-cell:hover .dashboard-toc-Collapser-child {\n  background: var(--jp-brand-color0);\n  opacity: 1;\n}\n\n.dashboard-TableOfContents-content code {\n  font-size: inherit;\n}\n\n.dashboard-toc-Ellipses {\n  height: 16px;\n  margin-left: auto;\n}\n\n.dashboard-toc-Ellipses:hover {\n  border: 1px solid var(--jp-border-color1);\n  box-shadow: 0 0 2px 0 rgba(0 0 0 / 25%);\n  background-color: var(--jp-layout-color0);\n}\n\n.dashboard-toc-level-size-2 {\n  margin-left: 16px;\n}\n\n.dashboard-toc-level-size-3 {\n  margin-left: 36px;\n}\n\n.dashboard-toc-level-size-4 {\n  margin-left: 56px;\n}\n\n.dashboard-toc-level-size-5 {\n  margin-left: 76px;\n}\n\n.dashboard-TableOfContents-placeholder {\n  text-align: center;\n}\n\n.dashboard-TableOfContents-placeholderContent {\n  color: var(--jp-content-font-color2);\n  padding: 25px 30px 8px;\n}\n\n.dashboard-toc-react-component {\n  display: flex;\n  align-items: center;\n  border-radius: 2px;\n  padding: 2px;\n  min-width: 52px;\n  margin-left: 5px;\n  font-size: small;\n  text-align: center;\n  word-wrap: break-word;\n}\n\n.dashboard-toc-react-text {\n  width: 100%;\n  color: var(--jp-inverse-layout-color0);\n}\n\n.dashboard-toc-header-title {\n  overflow: hidden;\n  white-space: nowrap;\n  text-overflow: ellipsis;\n  margin-right: 5px;\n}\n\n.dashboard-toc-download-button {\n  cursor: pointer;\n  padding: 3px 6px;\n  border-radius: 2px;\n  display: flex;\n  align-items: center;\n  color: white;\n  background-color: var(--jp-brand-color1);\n}\n\n.dashboard-toc-download-button:hover {\n  background-color: var(--jp-brand-color0);\n}\n\n.dashboard-toc-download-button-disabled {\n  cursor: wait;\n  padding: 3px 6px;\n  border-radius: 2px;\n  display: flex;\n  align-items: center;\n  color: white;\n  background-color: #575b5b;\n}\n\n.dashboard-toc-download-icon {\n  margin-right: 4px;\n}\n\n.dashboard-toc-download-icon .jp-icon3 {\n  fill: white;\n}\n", ""]);
+            const d = i
         },
         3612: (n, o, e) => {
             e.d(o, {
-                Z: () => i
+                Z: () => d
             });
             var r = e(8081),
                 t = e.n(r),
                 a = e(3645),
-                l = e.n(a)()(t());
-            l.push([n.id, ".dashboard-toc-code-cell-div {\n  display: inline-flex;\n  overflow: hidden;\n  flex-grow: 1;\n}\n\n.dashboard-toc-code-span {\n  width: 100%;\n  overflow: hidden;\n  cursor: pointer;\n  background: var(--jp-layout-color0);\n  border: var(--jp-border-width) solid var(--jp-layout-color3);\n  max-height: 38px;\n  min-height: 24px;\n}\n\n/* target all children of dashboard-toc-cell-input and change the font-size */\n.dashboard-toc-cell-input * {\n  font-size: 9px;\n  overflow: hidden;\n}\n\n.dashboard-toc-code-cell-prompt {\n  flex: 0 0 27px;\n  color: var(--jp-cell-prompt-not-active-font-color);\n  opacity: var(--jp-cell-prompt-not-active-opacity);\n  font-family: var(--jp-cell-prompt-font-family);\n  padding: var(--jp-code-padding);\n  padding-right: 0;\n  padding-left: 0;\n  letter-spacing: var(--jp-cell-prompt-letter-spacing);\n  line-height: var(--jp-code-line-height);\n  font-size: 8px;\n  border: var(--jp-border-width) solid transparent;\n  text-align: left;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  -webkit-user-select: none;\n  -moz-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n", ""]);
-            const i = l
+                i = e.n(a)()(t());
+            i.push([n.id, ".dashboard-toc-code-cell-div {\n  display: inline-flex;\n  overflow: hidden;\n  flex-grow: 1;\n}\n\n.dashboard-toc-code-span {\n  width: 100%;\n  overflow: hidden;\n  cursor: pointer;\n  background: var(--jp-layout-color0);\n  border: var(--jp-border-width) solid var(--jp-layout-color3);\n  max-height: 38px;\n  min-height: 24px;\n}\n\n/* target all children of dashboard-toc-cell-input and change the font-size */\n.dashboard-toc-cell-input * {\n  font-size: 9px;\n  overflow: hidden;\n}\n\n.dashboard-toc-code-cell-prompt {\n  flex: 0 0 27px;\n  color: var(--jp-cell-prompt-not-active-font-color);\n  opacity: var(--jp-cell-prompt-not-active-opacity);\n  font-family: var(--jp-cell-prompt-font-family);\n  padding: var(--jp-code-padding);\n  padding-right: 0;\n  padding-left: 0;\n  letter-spacing: var(--jp-cell-prompt-letter-spacing);\n  line-height: var(--jp-code-line-height);\n  font-size: 8px;\n  border: var(--jp-border-width) solid transparent;\n  text-align: left;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  -webkit-user-select: none;\n  -moz-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n", ""]);
+            const d = i
         },
         939: (n, o, e) => {
             e.d(o, {
-                Z: () => i
+                Z: () => d
             });
             var r = e(8081),
                 t = e.n(r),
                 a = e(3645),
-                l = e.n(a)()(t());
-            l.push([n.id, ".unianalytics-link-container {\n  border: 1px solid var(--jp-inverse-layout-color4);\n  border-radius: 5px;\n  display: flex;\n  align-items: center;\n  margin: 0;\n  padding: 0;\n}\n\n.unianalytics-link {\n  padding: 5px 15px;\n  flex: 1;\n  max-width: 90%;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n\n.unianalytics-link-button-container {\n  padding: 5px;\n  border-left: 1px solid var(--jp-inverse-layout-color4);\n  display: flex;\n  align-items: center;\n  margin-left: auto;\n}\n\n.unianalytics-link-button {\n  border: none;\n  background: transparent;\n  cursor: pointer;\n  display: flex;\n  align-items: center;\n}\n", ""]);
-            const i = l
+                i = e.n(a)()(t());
+            i.push([n.id, ".unianalytics-link-container {\n  border: 1px solid var(--jp-inverse-layout-color4);\n  border-radius: 5px;\n  display: flex;\n  align-items: center;\n  margin: 0;\n  padding: 0;\n}\n\n.unianalytics-link {\n  padding: 5px 15px;\n  flex: 1;\n  max-width: 90%;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n\n.unianalytics-link-button-container {\n  padding: 5px;\n  border-left: 1px solid var(--jp-inverse-layout-color4);\n  display: flex;\n  align-items: center;\n  margin-left: auto;\n}\n\n.unianalytics-link-button {\n  border: none;\n  background: transparent;\n  cursor: pointer;\n  display: flex;\n  align-items: center;\n}\n", ""]);
+            const d = i
         },
         3645: n => {
             n.exports = function(n) {
                 var o = [];
                 return o.toString = function() {
                     return this.map((function(o) {
                         var e = "",
                             r = void 0 !== o[5];
                         return o[4] && (e += "@supports (".concat(o[4], ") {")), o[2] && (e += "@media ".concat(o[2], " {")), r && (e += "@layer".concat(o[5].length > 0 ? " ".concat(o[5]) : "", " {")), e += n(o), r && (e += "}"), o[2] && (e += "}"), o[4] && (e += "}"), e
                     })).join("")
                 }, o.i = function(n, e, r, t, a) {
                     "string" == typeof n && (n = [
                         [null, n, void 0]
                     ]);
-                    var l = {};
+                    var i = {};
                     if (r)
-                        for (var i = 0; i < this.length; i++) {
-                            var d = this[i][0];
-                            null != d && (l[d] = !0)
+                        for (var d = 0; d < this.length; d++) {
+                            var l = this[d][0];
+                            null != l && (i[l] = !0)
                         }
                     for (var c = 0; c < n.length; c++) {
-                        var s = [].concat(n[c]);
-                        r && l[s[0]] || (void 0 !== a && (void 0 === s[5] || (s[1] = "@layer".concat(s[5].length > 0 ? " ".concat(s[5]) : "", " {").concat(s[1], "}")), s[5] = a), e && (s[2] ? (s[1] = "@media ".concat(s[2], " {").concat(s[1], "}"), s[2] = e) : s[2] = e), t && (s[4] ? (s[1] = "@supports (".concat(s[4], ") {").concat(s[1], "}"), s[4] = t) : s[4] = "".concat(t)), o.push(s))
+                        var p = [].concat(n[c]);
+                        r && i[p[0]] || (void 0 !== a && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = a), e && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = e) : p[2] = e), t && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = t) : p[4] = "".concat(t)), o.push(p))
                     }
                 }, o
             }
         },
         8081: n => {
             n.exports = function(n) {
                 return n[1]
@@ -95,40 +95,40 @@
                     if (o[r].identifier === n) {
                         e = r;
                         break
                     } return e
             }
 
             function r(n, r) {
-                for (var a = {}, l = [], i = 0; i < n.length; i++) {
-                    var d = n[i],
-                        c = r.base ? d[0] + r.base : d[0],
-                        s = a[c] || 0,
-                        p = "".concat(c, " ").concat(s);
-                    a[c] = s + 1;
-                    var u = e(p),
+                for (var a = {}, i = [], d = 0; d < n.length; d++) {
+                    var l = n[d],
+                        c = r.base ? l[0] + r.base : l[0],
+                        p = a[c] || 0,
+                        s = "".concat(c, " ").concat(p);
+                    a[c] = p + 1;
+                    var u = e(s),
                         b = {
-                            css: d[1],
-                            media: d[2],
-                            sourceMap: d[3],
-                            supports: d[4],
-                            layer: d[5]
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
                         };
                     if (-1 !== u) o[u].references++, o[u].updater(b);
                     else {
                         var h = t(b, r);
-                        r.byIndex = i, o.splice(i, 0, {
-                            identifier: p,
+                        r.byIndex = d, o.splice(d, 0, {
+                            identifier: s,
                             updater: h,
                             references: 1
                         })
                     }
-                    l.push(p)
+                    i.push(s)
                 }
-                return l
+                return i
             }
 
             function t(n, o) {
                 var e = o.domAPI(o);
                 return e.update(n),
                     function(o) {
                         if (o) {
@@ -137,23 +137,23 @@
                         } else e.remove()
                     }
             }
             n.exports = function(n, t) {
                 var a = r(n = n || [], t = t || {});
                 return function(n) {
                     n = n || [];
-                    for (var l = 0; l < a.length; l++) {
-                        var i = e(a[l]);
-                        o[i].references--
-                    }
-                    for (var d = r(n, t), c = 0; c < a.length; c++) {
-                        var s = e(a[c]);
-                        0 === o[s].references && (o[s].updater(), o.splice(s, 1))
+                    for (var i = 0; i < a.length; i++) {
+                        var d = e(a[i]);
+                        o[d].references--
+                    }
+                    for (var l = r(n, t), c = 0; c < a.length; c++) {
+                        var p = e(a[c]);
+                        0 === o[p].references && (o[p].updater(), o.splice(p, 1))
                     }
-                    a = d
+                    a = l
                 }
             }
         },
         569: n => {
             var o = {};
             n.exports = function(n, e) {
                 var r = function(n) {
@@ -221,34 +221,34 @@
             }
         },
         5546: (n, o, e) => {
             e.r(o);
             var r = e(3379),
                 t = e.n(r),
                 a = e(7795),
-                l = e.n(a),
-                i = e(569),
-                d = e.n(i),
+                i = e.n(a),
+                d = e(569),
+                l = e.n(d),
                 c = e(3565),
-                s = e.n(c),
-                p = e(9216),
-                u = e.n(p),
+                p = e.n(c),
+                s = e(9216),
+                u = e.n(s),
                 b = e(4589),
                 h = e.n(b),
                 f = e(1150),
                 x = {};
-            x.styleTagTransform = h(), x.setAttributes = s(), x.insert = d().bind(null, "head"), x.domAPI = l(), x.insertStyleElement = u(), t()(f.Z, x), f.Z && f.Z.locals && f.Z.locals;
+            x.styleTagTransform = h(), x.setAttributes = p(), x.insert = l().bind(null, "head"), x.domAPI = i(), x.insertStyleElement = u(), t()(f.Z, x), f.Z && f.Z.locals && f.Z.locals;
             var g = e(939),
-                v = {};
-            v.styleTagTransform = h(), v.setAttributes = s(), v.insert = d().bind(null, "head"), v.domAPI = l(), v.insertStyleElement = u(), t()(g.Z, v), g.Z && g.Z.locals && g.Z.locals;
-            var m = e(3630),
-                y = {};
-            y.styleTagTransform = h(), y.setAttributes = s(), y.insert = d().bind(null, "head"), y.domAPI = l(), y.insertStyleElement = u(), t()(m.Z, y), m.Z && m.Z.locals && m.Z.locals;
-            var w = e(7563),
+                m = {};
+            m.styleTagTransform = h(), m.setAttributes = p(), m.insert = l().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = u(), t()(g.Z, m), g.Z && g.Z.locals && g.Z.locals;
+            var v = e(3630),
+                w = {};
+            w.styleTagTransform = h(), w.setAttributes = p(), w.insert = l().bind(null, "head"), w.domAPI = i(), w.insertStyleElement = u(), t()(v.Z, w), v.Z && v.Z.locals && v.Z.locals;
+            var y = e(7563),
                 j = {};
-            j.styleTagTransform = h(), j.setAttributes = s(), j.insert = d().bind(null, "head"), j.domAPI = l(), j.insertStyleElement = u(), t()(w.Z, j), w.Z && w.Z.locals && w.Z.locals;
+            j.styleTagTransform = h(), j.setAttributes = p(), j.insert = l().bind(null, "head"), j.domAPI = i(), j.insertStyleElement = u(), t()(y.Z, j), y.Z && y.Z.locals && y.Z.locals;
             var k = e(3612),
                 z = {};
-            z.styleTagTransform = h(), z.setAttributes = s(), z.insert = d().bind(null, "head"), z.domAPI = l(), z.insertStyleElement = u(), t()(k.Z, z), k.Z && k.Z.locals && k.Z.locals
+            z.styleTagTransform = h(), z.setAttributes = p(), z.insert = l().bind(null, "head"), z.domAPI = i(), z.insertStyleElement = u(), t()(k.Z, z), k.Z && k.Z.locals && k.Z.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/563.b613f734176cb51510ef.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/563.b613f734176cb51510ef.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/638.d37271636c4d956096de.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/638.d37271636c4d956096de.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/708.323c3614d31a5918cfaf.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/708.323c3614d31a5918cfaf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/744.329dc4d1ed2f5c918266.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/744.329dc4d1ed2f5c918266.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/798.33a8f0893a66574e9259.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/798.33a8f0893a66574e9259.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js.LICENSE.txt` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/981.ebb9e1d6122980b5ff0e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/remoteEntry.8cd70c149b116f11f59e.js` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/remoteEntry.f90079a80d3ca2c7e110.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, o, n, d, i, l, u, f, c, s, b, p, h, v, m, y, g, j, w, P, _, k, O, S = {
             4479: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(39), t.e(29), t.e(120)]).then((() => () => t(8859))),
-                        "./extension": () => Promise.all([t.e(39), t.e(29), t.e(120)]).then((() => () => t(8859))),
+                        "./index": () => Promise.all([t.e(39), t.e(29), t.e(419)]).then((() => () => t(575))),
+                        "./extension": () => Promise.all([t.e(39), t.e(29), t.e(419)]).then((() => () => t(575))),
                         "./style": () => t.e(546).then((() => () => t(5546)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -60,42 +60,42 @@
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         10: "1e5c908a94fc4b83c2e5",
         18: "759fbf2374edc42b5c3e",
         29: "9b0cb1475dcac2b485f3",
         39: "5a3b28a79ba693a9b627",
-        120: "f9ab87c96623964d015f",
         211: "583fddc965c583e61532",
         308: "d9da4ce35f354c6f12e1",
         373: "37ddee9d229ac254f896",
         376: "d960746fd943a4ef55b8",
+        419: "8d7c0e30d3f058138a25",
         426: "a7015f9dfda310972c1b",
         459: "75a9fe630dfdb00e65b4",
-        546: "a8f5ba1be2a764c64287",
+        546: "d5da555479f21a401709",
         563: "b613f734176cb51510ef",
         638: "d37271636c4d956096de",
         704: "4e17d862a476ae3df8ae",
         708: "323c3614d31a5918cfaf",
         744: "329dc4d1ed2f5c918266",
         798: "33a8f0893a66574e9259",
         981: "ebb9e1d6122980b5ff0e"
     } [e] + ".js?v=" + {
         10: "1e5c908a94fc4b83c2e5",
         18: "759fbf2374edc42b5c3e",
         29: "9b0cb1475dcac2b485f3",
         39: "5a3b28a79ba693a9b627",
-        120: "f9ab87c96623964d015f",
         211: "583fddc965c583e61532",
         308: "d9da4ce35f354c6f12e1",
         373: "37ddee9d229ac254f896",
         376: "d960746fd943a4ef55b8",
+        419: "8d7c0e30d3f058138a25",
         426: "a7015f9dfda310972c1b",
         459: "75a9fe630dfdb00e65b4",
-        546: "a8f5ba1be2a764c64287",
+        546: "d5da555479f21a401709",
         563: "b613f734176cb51510ef",
         638: "d37271636c4d956096de",
         704: "4e17d862a476ae3df8ae",
         708: "323c3614d31a5918cfaf",
         744: "329dc4d1ed2f5c918266",
         798: "33a8f0893a66574e9259",
         981: "ebb9e1d6122980b5ff0e"
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : d > i.from)) && (o[r] = {
                             get: t,
                             from: d,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (i("@reduxjs/toolkit", "1.9.7", (() => x.e(426).then((() => () => x(8426))))), i("chart.js", "4.4.1", (() => x.e(708).then((() => () => x(4708))))), i("jupyterlab_unianalytics_dashboard", "4.0.8", (() => Promise.all([x.e(39), x.e(29), x.e(120)]).then((() => () => x(8859))))), i("marked", "11.1.1", (() => x.e(308).then((() => () => x(3308))))), i("react-bootstrap-icons", "1.10.3", (() => Promise.all([x.e(744), x.e(29)]).then((() => () => x(1744))))), i("react-bootstrap", "2.10.0", (() => Promise.all([x.e(18), x.e(29), x.e(704)]).then((() => () => x(1018))))), i("react-chartjs-2", "5.2.0", (() => Promise.all([x.e(29), x.e(459), x.e(563)]).then((() => () => x(5376))))), i("react-redux", "8.1.3", (() => Promise.all([x.e(981), x.e(29), x.e(704)]).then((() => () => x(2981)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@reduxjs/toolkit", "1.9.7", (() => x.e(426).then((() => () => x(8426))))), i("chart.js", "4.4.1", (() => x.e(708).then((() => () => x(4708))))), i("jupyterlab_unianalytics_dashboard", "4.0.9", (() => Promise.all([x.e(39), x.e(29), x.e(419)]).then((() => () => x(575))))), i("marked", "11.1.1", (() => x.e(308).then((() => () => x(3308))))), i("react-bootstrap-icons", "1.10.3", (() => Promise.all([x.e(744), x.e(29)]).then((() => () => x(1744))))), i("react-bootstrap", "2.10.0", (() => Promise.all([x.e(18), x.e(29), x.e(704)]).then((() => () => x(1018))))), i("react-chartjs-2", "5.2.0", (() => Promise.all([x.e(29), x.e(459), x.e(563)]).then((() => () => x(5376))))), i("react-redux", "8.1.3", (() => Promise.all([x.e(981), x.e(29), x.e(704)]).then((() => () => x(2981)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -271,49 +271,49 @@
         var n = x.I(r);
         return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
     })(((e, r, t, a) => (l(e, t), m(b(r, t, a) || v(r, e, t, a) || u(r, t))))), j = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && b(r, t, a);
         return n ? m(n) : o()
     })), P = {}, _ = {
         6029: () => j("default", "react", [1, 18, 2, 0]),
-        1121: () => j("default", "@jupyterlab/codeeditor", [1, 4, 1, 2]),
-        1810: () => j("default", "@jupyterlab/services", [1, 7, 1, 2]),
-        2445: () => j("default", "@jupyterlab/notebook", [1, 4, 1, 2]),
+        1778: () => g("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
         2535: () => w("default", "react-bootstrap-icons", [1, 1, 10, 3], (() => x.e(744).then((() => () => x(1744))))),
         2779: () => w("default", "marked", [1, 11, 1, 1], (() => x.e(308).then((() => () => x(3308))))),
-        3074: () => g("default", "@jupyterlab/outputarea", [1, 4, 1, 2]),
+        3452: () => j("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
+        3471: () => j("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
         3748: () => w("default", "@reduxjs/toolkit", [1, 1, 9, 5], (() => x.e(426).then((() => () => x(8426))))),
-        4351: () => j("default", "@jupyterlab/coreutils", [1, 6, 1, 2]),
+        4008: () => j("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
         4882: () => j("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => j("default", "@lumino/signaling", [1, 2, 0, 0]),
-        4991: () => j("default", "@jupyterlab/settingregistry", [1, 4, 1, 2]),
-        6249: () => j("default", "@jupyterlab/filebrowser", [1, 4, 1, 2]),
-        7388: () => j("default", "@jupyterlab/codemirror", [1, 4, 1, 2]),
-        7403: () => j("default", "@jupyterlab/apputils", [1, 4, 2, 2]),
+        6311: () => j("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
+        7217: () => j("default", "@jupyterlab/services", [1, 7, 1, 5]),
         7717: () => j("default", "@lumino/disposable", [1, 2, 0, 0]),
-        7750: () => j("default", "@jupyterlab/application", [1, 4, 1, 2]),
         7760: () => w("default", "react-redux", [1, 8, 0, 5], (() => Promise.all([x.e(981), x.e(704)]).then((() => () => x(2981))))),
+        7777: () => j("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
         7885: () => w("default", "react-chartjs-2", [1, 5, 2, 0], (() => Promise.all([x.e(459), x.e(798)]).then((() => () => x(5376))))),
+        8031: () => j("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
+        8048: () => j("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         8352: () => w("default", "chart.js", [1, 4, 4, 1], (() => x.e(708).then((() => () => x(4708))))),
-        8448: () => j("default", "@jupyterlab/ui-components", [1, 4, 1, 2]),
-        8547: () => j("default", "@jupyterlab/rendermime", [1, 4, 1, 2]),
+        8368: () => j("default", "@jupyterlab/application", [1, 4, 1, 5]),
         8559: () => w("default", "react-bootstrap", [1, 2, 10, 0], (() => Promise.all([x.e(18), x.e(704)]).then((() => () => x(1018))))),
+        8797: () => j("default", "@jupyterlab/notebook", [1, 4, 1, 5]),
+        9510: () => j("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
         7704: () => j("default", "react-dom", [1, 18, 2, 0]),
         6459: () => w("default", "chart.js", [1, 4, 1, 1], (() => x.e(708).then((() => () => x(4708))))),
         1373: () => j("default", "@codemirror/language", [1, 6, 0, 0]),
         6211: () => j("default", "@codemirror/view", [1, 6, 9, 6]),
         851: () => j("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => j("default", "@lezer/highlight", [1, 1, 0, 0]),
         8204: () => j("default", "@codemirror/state", [1, 6, 2, 0])
     }, k = {
         29: [6029],
-        120: [1121, 1810, 2445, 2535, 2779, 3074, 3748, 4351, 4882, 4901, 4991, 6249, 7388, 7403, 7717, 7750, 7760, 7885, 8352, 8448, 8547, 8559],
         211: [6211],
         373: [1373],
         376: [851, 7138, 8204],
+        419: [1778, 2535, 2779, 3452, 3471, 3748, 4008, 4882, 4901, 6311, 7217, 7717, 7760, 7777, 7885, 8031, 8048, 8352, 8368, 8559, 8797, 9510],
         459: [6459],
         704: [7704]
     }, O = {}, x.f.consumes = (e, r) => {
         x.o(k, e) && k[e].forEach((e => {
             if (x.o(P, e)) return r.push(P[e]);
             if (!O[e]) {
                 var t = r => {
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/jupyterlab_unianalytics_dashboard/labextension/static/third-party-licenses.json` & `jupyterlab_unianalytics_dashboard-4.0.9/jupyterlab_unianalytics_dashboard/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/schema/plugin.json` & `jupyterlab_unianalytics_dashboard-4.0.9/schema/plugin.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666666%*

 * *Differences: {"'properties'": "{'commonDashboardSettings': {'properties': {delete: ['realTime']}}}"}*

```diff
@@ -20,20 +20,14 @@
         "commonDashboardSettings": {
             "properties": {
                 "dashboardCollection": {
                     "default": true,
                     "description": "Whether to enable the collection of interaction clicks with the dashboard extension to better understand what features are more or less used.",
                     "title": "Collect clicks relative to dashboard usage",
                     "type": "boolean"
-                },
-                "realTime": {
-                    "default": true,
-                    "description": "Whether to only display currently connected users data (true), or consider historical data according to the selected time limit filter value (false)",
-                    "title": "Activate real-time dashboard",
-                    "type": "boolean"
                 }
             },
             "title": "Dashboard Settings",
             "type": "object"
         },
         "tocDashboardSettings": {
             "properties": {
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/handler.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/index.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/chat-dashboard/ChatContainer.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/chat-dashboard/ChatContainer.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import React, { useEffect, useState } from 'react';
 import { Button } from 'react-bootstrap';
-import { refreshIcon, runIcon } from '@jupyterlab/ui-components';
+import { runIcon } from '@jupyterlab/ui-components';
+import { ArrowClockwise as RefreshLogo } from 'react-bootstrap-icons';
 import { BACKEND_API_URL } from '../utils/constants';
 import ConnectionComponent from './ConnectionComponent';
 import { fetchWithCredentials } from '../utils/utils';
 
 const ChatContainer = (props: { notebookId: string }) => {
   const [connectedUsers, setConnectedUsers] = useState<string[]>([]);
   const [selectedUser, setSelectedUser] = useState<string | null>(null);
@@ -49,18 +50,18 @@
     <div style={{ width: '100%', padding: '15px' }}>
       <div style={{ display: 'flex', width: '100%', paddingBottom: '15px' }}>
         <div style={{ color: 'white', fontSize: '20px', fontWeight: '500' }}>
           Chat with Users
         </div>
         <div className="breadcrumb-buttons-container">
           <Button
-            className="breadcrumb-button"
+            className="dashboard-button"
             onClick={() => requestConnectedUsers()}
           >
-            <refreshIcon.react elementSize="large" className="labicon-logo" />
+            <RefreshLogo className="dashboard-icon" />
           </Button>
         </div>
       </div>
       <div style={{ display: 'flex', flexDirection: 'column', flex: '1' }}>
         <div style={{ width: '100%', maxHeight: '50%', overflowY: 'auto' }}>
           {connectedUsers.map((userId: string) => (
             <ConnectionComponent
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/chat-dashboard/ConnectionComponent.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/chat-dashboard/ConnectionComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/ChatDashboardPanel.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/ChatDashboardPanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/DashboardPanel.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/DashboardPanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/PanelManager.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/PanelManager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/TocDashboardPanel.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/TocDashboardPanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/VisuDashboardPanel.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/VisuDashboardPanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/dashboard-widgets/WebsocketManager.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/dashboard-widgets/WebsocketManager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/icons/index.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/icons/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/plugins/dashboards.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/plugins/dashboards.ts`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import { NotebookPanel } from '@jupyterlab/notebook';
 import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { PanelManager } from '../dashboard-widgets/PanelManager';
 import { VisuDashboardPanel } from '../dashboard-widgets/VisuDashboardPanel';
 import { TocDashboardPanel } from '../dashboard-widgets/TocDashboardPanel';
 // import { ChatDashboardPanel } from '../dashboard-widgets/ChatDashboardPanel';
-import { displayRealTime } from '../redux/reducers/CommonDashboardReducer';
 import { InteractionRecorder } from '../utils/interactionRecorder';
 import { DashboardClickOrigin } from '../utils/interfaces';
 import { addDashboardNotebookExtensions } from '../widget-extensions';
 
 const dispatch = store.dispatch as AppDispatch;
 
 export async function activateDashboardPlugins(
@@ -149,27 +148,19 @@
     }
     const notebookPanel = widget as NotebookPanel;
     panelManager.panel = notebookPanel;
   }
 
   function onSettingsChanged(settings: ISettingRegistry.ISettings) {
     const commonDashboardSettings = settings.composite.commonDashboardSettings;
-    let isRealTimeActivated;
     if (commonDashboardSettings) {
-      isRealTimeActivated = (commonDashboardSettings as any).realTime;
       InteractionRecorder.setPermission(
         (commonDashboardSettings as any).dashboardCollection || false
       );
     } else {
-      isRealTimeActivated = (settings.default('commonDashboardSettings') as any)
-        ?.realTime;
       InteractionRecorder.setPermission(
         (settings.default('commonDashboardSettings') as any)
           ?.dashboardCollection || false
       );
     }
-
-    if (isRealTimeActivated !== null || isRealTimeActivated !== undefined) {
-      dispatch(displayRealTime(isRealTimeActivated));
-    }
   }
 }
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/plugins/uploadNotebook.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/plugins/uploadNotebook.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/redux/store.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/redux/store.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,29 @@
 import { configureStore } from '@reduxjs/toolkit';
 import ToCDashboardReducer from './reducers/ToCDashboardReducer';
 import SideDashboardReducer from './reducers/SideDashboardReducer';
-import CommonDashboard from './reducers/CommonDashboardReducer';
+import CommonDashboard, {
+  initialCommonDashboardState
+} from './reducers/CommonDashboardReducer';
+import { STORAGE_KEY } from '../utils/constants';
+import { localStorageMiddleware } from './localStorage';
+
+const preloadedState = {
+  // if commondashboard is already defined in localStorage, use it as part of the initial state
+  commondashboard: localStorage.getItem(STORAGE_KEY)
+    ? JSON.parse(localStorage.getItem(STORAGE_KEY) as string)
+    : initialCommonDashboardState
+};
 
 export const store = configureStore({
   reducer: {
     tocdashboard: ToCDashboardReducer,
     sidedashboard: SideDashboardReducer,
     commondashboard: CommonDashboard
-  }
+  },
+  middleware: getDefaultMiddleware =>
+    getDefaultMiddleware().concat(localStorageMiddleware),
+  preloadedState: preloadedState
 });
 
 export type RootState = ReturnType<typeof store.getState>;
 export type AppDispatch = typeof store.dispatch;
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/redux/reducers/CommonDashboardReducer.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/redux/reducers/ToCDashboardReducer.ts`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 import { createSlice, PayloadAction } from '@reduxjs/toolkit';
-import { NotebookCell, CommonDashboardState } from '../types';
+import { ToCState } from '../types';
 
-export const initialCommonDashboardState: CommonDashboardState = {
-  notebookCells: null,
-  timeWindow: 'null',
-  refreshBoolean: false,
-  displayRealTime: true
+export const initialToCDashboardState: ToCState = {
+  displayDashboard: true,
+  hasNotebookId: false
 };
 
-export const commonDashboardSlice = createSlice({
-  name: 'commondashboard',
-  initialState: initialCommonDashboardState,
+export const tocDashboardSlice = createSlice({
+  name: 'tocdashboard',
+  initialState: initialToCDashboardState,
   reducers: {
-    setTimeWindow: (state, action: PayloadAction<string>) => {
-      state.timeWindow = action.payload;
+    setDisplayHideDashboard: (state, action: PayloadAction<boolean>) => {
+      state.displayDashboard = action.payload;
     },
-    setNotebookCells: (state, action: PayloadAction<NotebookCell[] | null>) => {
-      state.notebookCells = action.payload;
-    },
-    refreshDashboards: state => {
-      state.refreshBoolean = !state.refreshBoolean;
-    },
-    displayRealTime: (state, action: PayloadAction<boolean>) => {
-      state.displayRealTime = action.payload;
+    setHasNotebookId: (state, action: PayloadAction<boolean>) => {
+      state.hasNotebookId = action.payload;
     }
   }
 });
 
-export const {
-  setTimeWindow,
-  setNotebookCells,
-  refreshDashboards,
-  displayRealTime
-} = commonDashboardSlice.actions;
+export const { setDisplayHideDashboard, setHasNotebookId } =
+  tocDashboardSlice.actions;
 
-export default commonDashboardSlice.reducer;
+export default tocDashboardSlice.reducer;
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/redux/reducers/SideDashboardReducer.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/redux/reducers/SideDashboardReducer.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/PageRouter.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/PageRouter.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/cell/CellInput.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/CellInput.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/cell/CellOutput.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/CellOutput.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/cell/MarkdownComponent.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/cell/MarkdownComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/layout/GridSystem.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/layout/GridSystem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/layout/TopBreadcrumb.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/layout/TopBreadcrumb.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import { Stack, Button } from 'react-bootstrap';
 
 import { useSelector } from 'react-redux';
 import { RootState } from '../../../redux/store';
 import { store, AppDispatch } from '../../../redux/store';
 import { navigateToHistory } from '../../../redux/reducers/SideDashboardReducer';
 import { refreshDashboards } from '../../../redux/reducers/CommonDashboardReducer';
-import { refreshIcon } from '@jupyterlab/ui-components';
+import { ArrowClockwise as RefreshLogo } from 'react-bootstrap-icons';
 import { InteractionRecorder } from '../../../utils/interactionRecorder';
 import { DashboardClickOrigin } from '../../../utils/interfaces';
 
 const dispatch = store.dispatch as AppDispatch;
 
 const TopBreadcrumb = (): JSX.Element => {
   const navigationState = useSelector(
@@ -49,24 +49,24 @@
             {value.pageName}
           </div>
         );
       })}
 
       <div className="breadcrumb-buttons-container">
         <Button
-          className="breadcrumb-button"
+          className="dashboard-button"
           onClick={() => {
             InteractionRecorder.sendInteraction({
               click_type: 'ON',
               signal_origin: DashboardClickOrigin.DASHBOARD_REFRESH_BUTTON
             });
             dispatch(refreshDashboards());
           }}
         >
-          <refreshIcon.react elementSize="large" className="labicon-logo" />
+          <RefreshLogo className="dashboard-icon" />
         </Button>
       </div>
     </Stack>
   );
 };
 
 export default TopBreadcrumb;
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/notebook/ChartContainer.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/notebook/ChartContainer.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/notebook/CodeExecComponent.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/notebook/CodeExecComponent.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import React, { useEffect, useState } from 'react';
 import { ChartData } from 'chart.js';
 import { BACKEND_API_URL } from '../../../utils/constants';
 import ChartContainer from './ChartContainer';
 import { Bar } from 'react-chartjs-2';
 import { codeExecOptions } from '../../../utils/chartOptions';
-import { IChartProps } from '../../pages/Notebook';
 import { useSelector } from 'react-redux';
 import { RootState } from '../../../redux/store';
-import { fetchWithCredentials } from '../../../utils/utils';
+import {
+  fetchWithCredentials,
+  generateQueryArgsString
+} from '../../../utils/utils';
 
-const CodeExecComponent = (props: IChartProps) => {
+const CodeExecComponent = (props: { notebookId: string }) => {
   const [codeExecData, setCodeExecData] = useState<ChartData<'bar'>>({
     labels: [],
     datasets: []
   });
 
-  const displayRealTime = useSelector(
-    (state: RootState) => state.commondashboard.displayRealTime
+  const dashboardQueryArgsRedux = useSelector(
+    (state: RootState) => state.commondashboard.dashboardQueryArgs
+  );
+  const refreshRequired = useSelector(
+    (state: RootState) => state.commondashboard.refreshBoolean
+  );
+  const notebookCells = useSelector(
+    (state: RootState) => state.commondashboard.notebookCells
   );
 
   // fetching execution data
   useEffect(() => {
     fetchWithCredentials(
-      `${BACKEND_API_URL}/dashboard/${props.notebookId}/user_code_execution?timeWindow=${props.timeWindow}&displayRealTime=${displayRealTime}`
+      `${BACKEND_API_URL}/dashboard/${props.notebookId}/user_code_execution?${generateQueryArgsString(dashboardQueryArgsRedux, props.notebookId)}`
     )
       .then(response => response.json())
       .then(data => {
         // filter elements of notebookCells that are of type 'code'
         const codeCells =
-          props.notebookCells?.filter(cell => cell.cellType === 'code') || [];
+          notebookCells?.filter(cell => cell.cellType === 'code') || [];
 
         const chartData: ChartData<'bar'> = {
           labels: Array.from(
             { length: codeCells.length },
             (_, index) => index + 1
           ),
           datasets: [
@@ -75,15 +83,15 @@
             chartData.datasets[2].data[index] = parseFloat(
               matchingData.code_exec_ok_pct
             );
           }
         });
         setCodeExecData(chartData);
       });
-  }, [props.timeWindow, props.refreshRequired]);
+  }, [dashboardQueryArgsRedux, refreshRequired]);
 
   return (
     <ChartContainer
       PassedComponent={<Bar data={codeExecData} options={codeExecOptions} />}
       title="Code cell execution across users"
     />
   );
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/notebook/TimeSpentComponent.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/notebook/TimeSpentComponent.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 import React, { useEffect, useState } from 'react';
 import { ChartData } from 'chart.js';
 import { BACKEND_API_URL } from '../../../utils/constants';
 import { NotebookCell } from '../../../redux/types';
 import ChartContainer from './ChartContainer';
 import { Scatter } from 'react-chartjs-2';
 import { timeSpentOptions } from '../../../utils/chartOptions';
-import { IChartProps } from '../../pages/Notebook';
 import { useSelector } from 'react-redux';
 import { RootState } from '../../../redux/store';
-import { fetchWithCredentials } from '../../../utils/utils';
+import {
+  fetchWithCredentials,
+  generateQueryArgsString
+} from '../../../utils/utils';
 
-const TimeSpentComponent = (props: IChartProps) => {
+const TimeSpentComponent = (props: { notebookId: string }) => {
   const [timeSpentData, setTimeSpentData] = useState<ChartData<'scatter'>>({
     labels: [],
     datasets: []
   });
 
-  const displayRealTime = useSelector(
-    (state: RootState) => state.commondashboard.displayRealTime
+  const dashboardQueryArgsRedux = useSelector(
+    (state: RootState) => state.commondashboard.dashboardQueryArgs
+  );
+  const refreshRequired = useSelector(
+    (state: RootState) => state.commondashboard.refreshBoolean
+  );
+  const notebookCells = useSelector(
+    (state: RootState) => state.commondashboard.notebookCells
   );
 
   // fetching access time data
   useEffect(() => {
     fetchWithCredentials(
-      `${BACKEND_API_URL}/dashboard/${props.notebookId}/user_cell_time?timeWindow=${props.timeWindow}&displayRealTime=${displayRealTime}`
+      `${BACKEND_API_URL}/dashboard/${props.notebookId}/user_cell_time?${generateQueryArgsString(dashboardQueryArgsRedux, props.notebookId)}`
     )
       .then(response => response.json())
       .then(data => {
         const chartData: ChartData<'scatter'> = {
-          labels: props.notebookCells
+          labels: notebookCells
             ? Array.from(
-                { length: props.notebookCells.length },
+                { length: notebookCells.length },
                 (_, index) => index + 1
               )
             : [],
           datasets: [
             {
               label: 'time spent on a cell by a user',
               data:
-                props.notebookCells?.flatMap(
-                  (cell: NotebookCell, index: number) => {
-                    const foundData = data.find(
-                      (item: any) => item.cell === cell.id
-                    );
-                    if (foundData) {
-                      return foundData.durations.map((d: number) => ({
-                        x: index + 1,
-                        y: d
-                      }));
-                    }
-                    return [];
+                notebookCells?.flatMap((cell: NotebookCell, index: number) => {
+                  const foundData = data.find(
+                    (item: any) => item.cell === cell.id
+                  );
+                  if (foundData) {
+                    return foundData.durations.map((d: number) => ({
+                      x: index + 1,
+                      y: d
+                    }));
                   }
-                ) || [],
+                  return [];
+                }) || [],
               backgroundColor: 'rgba(54, 162, 235, 0.2)',
               borderColor: 'rgba(54, 162, 235, 1)',
               borderWidth: 1,
               pointRadius: 1
             }
           ]
         };
         setTimeSpentData(chartData);
       });
-  }, [props.timeWindow, props.refreshRequired]);
+  }, [dashboardQueryArgsRedux, refreshRequired]);
 
   return (
     <ChartContainer
       PassedComponent={
         <Scatter data={timeSpentData} options={timeSpentOptions} />
       }
       title="Amount of time spent on each cell"
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/components/placeholder/SidebarPlaceholder.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/components/placeholder/SidebarPlaceholder.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/side-dashboard/pages/Cell.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/side-dashboard/pages/Cell.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import React, { useState, useEffect, useRef } from 'react';
-import {
-  Row,
-  Col,
-  Card,
-  Form,
-  ToggleButton,
-  ButtonGroup
-} from 'react-bootstrap';
-import { BACKEND_API_URL } from '../../utils/constants';
+import { Row, Form, ToggleButton, ButtonGroup } from 'react-bootstrap';
+import { BACKEND_API_URL, DropdownSortingValues } from '../../utils/constants';
 
 import { useSelector } from 'react-redux';
 import { RootState } from '../../redux/store';
 import { CellLayer } from '../../redux/types';
 import CellOutput from '../components/cell/CellOutput';
 import CellInput from '../components/cell/CellInput';
 import TimeDropDown from '../components/buttons/TimeDropDown';
 import SortDropDown from '../components/buttons/SortDropDown';
 
 import MarkdownComponent from '../components/cell/MarkdownComponent';
 import { IRenderMime } from '@jupyterlab/rendermime';
 import { InteractionRecorder } from '../../utils/interactionRecorder';
 import { DashboardClickOrigin } from '../../utils/interfaces';
-import { fetchWithCredentials } from '../../utils/utils';
+import {
+  fetchWithCredentials,
+  generateQueryArgsString
+} from '../../utils/utils';
+import ExecutionComponent from '../components/cell/ExecutionComponent';
+import GroupDropDown from '../components/buttons/GroupDropDown';
 
 interface ICellPageProps {
   notebookId: string;
   sanitizer: IRenderMime.ISanitizer;
 }
 
 // function to wait for a small delay before updating the value of the filter box input state value
@@ -49,22 +47,22 @@
 
   // declaring a 2nd boolean since state updates are async, which wouldn't be quick enough for the 2nd useEffect check
   let isAlreadyFetching = false;
 
   const navigationState = useSelector(
     (state: RootState) => state.sidedashboard.navigationState
   );
-  const timeWindow = useSelector(
-    (state: RootState) => state.commondashboard.timeWindow
-  );
   const refreshRequired = useSelector(
     (state: RootState) => state.commondashboard.refreshBoolean
   );
-  const displayRealTime = useSelector(
-    (state: RootState) => state.commondashboard.displayRealTime
+  const dashboardQueryArgsRedux = useSelector(
+    (state: RootState) => state.commondashboard.dashboardQueryArgs
+  );
+  const sortByRedux = useSelector(
+    (state: RootState) => state.commondashboard.sortBy
   );
 
   // filter header content
 
   const [showInputs, setShowInputs] = useState<boolean>(true);
   const [showOutputs, setShowOutputs] = useState<boolean>(true);
 
@@ -75,16 +73,14 @@
   const executionFilters = [
     { name: 'All', value: 1, status: 'all' },
     { name: 'Success', value: 2, status: 'ok' },
     { name: 'Error', value: 3, status: 'error' }
   ];
   const filterStatus = executionFilters.map(filter => filter.status);
 
-  const [orderBy, setOrderBy] = useState<string>('timeDesc'); // timeDesc (default), timeAsc, inputDesc, inputAsc, outputDesc, outputAsc
-
   // sorting
 
   const orderAndSetData = (data: any): void => {
     // filter the data based on the input value
     const searchTerm = inputFilterText.toLowerCase();
 
     if (searchTerm.length > 0) {
@@ -96,81 +92,73 @@
               .toLowerCase()
               .includes(searchTerm))
         );
       });
     }
 
     // sort the data according to the selected criterion
-    data.sort((a: any, b: any) => {
-      switch (orderBy) {
-        case 'timeDesc':
-          return new Date(a.t_finish) < new Date(b.t_finish) ? 1 : -1;
-        case 'timeAsc':
-          return new Date(a.t_finish) > new Date(b.t_finish) ? 1 : -1;
-        case 'inputAsc':
-          return a.cell_input.length - b.cell_input.length;
-        case 'inputDesc':
-          return b.cell_input.length - a.cell_input.length;
-        case 'outputAsc':
-          return a.cell_output_length - b.cell_output_length;
-        case 'outputDesc':
-          return b.cell_output_length - a.cell_output_length;
-        default:
-          return 0;
-      }
-    });
+    const sortByCriterion = sortByRedux[props.notebookId] || 'timeDesc';
+    const selectedSorting = DropdownSortingValues.find(
+      (sorting: any) => sorting.key === sortByCriterion
+    );
+    if (selectedSorting) {
+      data.sort(selectedSorting.method);
+    }
     setRenderedData(data);
   };
 
   // fetching
 
   const content = (navigationState[navigationState.length - 1] as CellLayer)
     .content;
 
   useEffect(() => {
     isAlreadyFetching = true;
     fetchWithCredentials(
-      `${BACKEND_API_URL}/dashboard/${props.notebookId}/cell/${content.cellId}?timeWindow=${timeWindow}&displayRealTime=${displayRealTime}`
+      `${BACKEND_API_URL}/dashboard/${props.notebookId}/cell/${content.cellId}?${generateQueryArgsString(dashboardQueryArgsRedux, props.notebookId)}`
     )
       .then(response => response.json())
       .then(data => {
         originalData.current = data;
         orderAndSetData(data);
         isAlreadyFetching = false;
       });
-  }, [navigationState, timeWindow, refreshRequired]);
+  }, [navigationState, dashboardQueryArgsRedux, refreshRequired]);
 
   useEffect(() => {
     if (!isAlreadyFetching) {
       // to avoid sorting twice upon first render
       const data = [...originalData.current];
       orderAndSetData(data);
     }
-  }, [orderBy, inputFilterText]);
+  }, [sortByRedux, inputFilterText]);
 
   return (
     <>
       <div className="dashboard-title-container">
         <div className="dashboard-title-text">Cell ({content.cellId})</div>
         <div className="dashboard-dropdown-container">
-          <SortDropDown setOrderBy={setOrderBy} />
-          <TimeDropDown />
+          <SortDropDown notebookId={props.notebookId} />
+          <GroupDropDown notebookId={props.notebookId} />
+          <TimeDropDown notebookId={props.notebookId} />
         </div>
       </div>
       {/* Filter Bar */}
-      <Form className="cell-filter-container">
+      <Form
+        className="cell-filter-container"
+        onSubmit={e => e.preventDefault()} // avoid refreshing the browser window
+      >
         <div className="cell-radio-container">
           <ButtonGroup size="sm">
             <ToggleButton
               style={{ marginRight: '3px' }}
               key="0"
               id="code-checkbox"
               type="radio"
               variant="outline-primary"
-              // name="radio"
               value="Code"
               checked={showInputs}
               onClick={event => {
                 if (showInputs && !showOutputs) {
                   // Prevent unchecking both checkboxes
                   event.preventDefault();
                 } else {
@@ -186,20 +174,19 @@
               Code
             </ToggleButton>
             <ToggleButton
               key="1"
               id="output-checkbox"
               type="radio"
               variant="outline-primary"
-              // name="radio"
               value="Output"
               checked={showOutputs}
               onClick={event => {
                 if (!showInputs && showOutputs) {
-                  // Prevent unchecking both checkboxes
+                  // prevent unchecking both checkboxes
                   event.preventDefault();
                 } else {
                   InteractionRecorder.sendInteraction({
                     click_type: showOutputs ? 'OFF' : 'ON',
                     signal_origin:
                       DashboardClickOrigin.CELL_DASHBOARD_FILTER_CODE_OUTPUT
                   });
@@ -247,64 +234,52 @@
         {/* Cell Executions */}
         {renderedData.map((value: { [key: string]: any }, index: number) => {
           return (
             <Row key={index}>
               {/* for markdown executions, consider that the execution status is 'ok', not an error */}
               {value.cell_type === 'MarkdownExecution' &&
               ['all', 'ok'].includes(filterStatus[radioValue - 1]) ? (
-                <Col md={12}>
-                  <Card className="cell-card">
-                    <Card.Body style={{ gap: '10px' }}>
-                      <Row className="cell-card-wrapper">
-                        <Col md={12} className="cell-user-title">
-                          <Card.Text>User {index + 1}</Card.Text>
-                        </Col>
-                        <Col md={12}>
-                          <MarkdownComponent
-                            markdownContent={value.cell_input}
-                            sanitizer={props.sanitizer}
-                          />
-                        </Col>
-                      </Row>
-                    </Card.Body>
-                  </Card>
-                </Col>
+                <ExecutionComponent
+                  value={value}
+                  index={index}
+                  ExecutionContent={
+                    <MarkdownComponent
+                      markdownContent={value.cell_input}
+                      sanitizer={props.sanitizer}
+                    />
+                  }
+                />
               ) : (
                 <>
                   {(radioValue === 1 ||
                     filterStatus[radioValue - 1] === value.status) && (
-                    <Col md={12}>
-                      <Card className="cell-card">
-                        <Card.Body style={{ gap: '10px' }}>
-                          <Row className="cell-card-wrapper">
-                            <Col md={12} className="cell-user-title">
-                              <Card.Text>User {index + 1}</Card.Text>
-                            </Col>
-                            <Col md={12}>
-                              {showInputs && (
-                                <CellInput
-                                  cell_input={value.cell_input}
-                                  language_mimetype={value.language_mimetype}
-                                  className="cell-content-container"
-                                />
-                              )}
-                              {showInputs &&
-                                showOutputs &&
-                                value.cell_output_model.length > 0 && <br />}
-                              {showOutputs &&
-                                value.cell_output_model.length > 0 && (
-                                  <CellOutput
-                                    cell_output_model={value.cell_output_model}
-                                  />
-                                )}
-                            </Col>
-                          </Row>
-                        </Card.Body>
-                      </Card>
-                    </Col>
+                    <ExecutionComponent
+                      value={value}
+                      index={index}
+                      ExecutionContent={
+                        <>
+                          {showInputs && (
+                            <CellInput
+                              cell_input={value.cell_input}
+                              language_mimetype={value.language_mimetype}
+                              className="cell-content-container"
+                            />
+                          )}
+                          {showInputs &&
+                            showOutputs &&
+                            value.cell_output_model.length > 0 && <br />}
+                          {showOutputs &&
+                            value.cell_output_model.length > 0 && (
+                              <CellOutput
+                                cell_output_model={value.cell_output_model}
+                              />
+                            )}
+                        </>
+                      }
+                    />
                   )}
                 </>
               )}
             </Row>
           );
         })}
       </>
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/ExportCSVButton.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/ExportCSVButton.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import { downloadIcon } from '@jupyterlab/ui-components';
 import { BACKEND_API_URL } from '../utils/constants';
 import { showDialog, Dialog } from '@jupyterlab/apputils';
 import { fetchWithCredentials } from '../utils/utils';
 
 type ValueCallback = (time: Date) => void;
 
-const convertToLocaleString = (date: Date): string => {
+export const convertToLocaleString = (date: Date): string => {
   // using the Sweden format, since they use the ISO Format to represent dates as expected by the datetime-local input
   return date.toLocaleString('sv-SE').slice(0, -3); // removing seconds
 };
 
 const DialogBodyComponent = (props: {
   startT1: Date;
   startT2: Date;
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/TocReactComponent.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/TocReactComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/tocDashboardItem.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/tocDashboardItem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/tocDashboardTree.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/tocDashboardTree.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import { INotebookHeading } from '../utils/headings';
 import { TocDashboardItem } from './tocDashboardItem';
 import { ItemRenderer } from '../utils/interfaces';
 import { APP_ID, BACKEND_API_URL, Selectors } from '../utils/constants';
 import { LocationData } from '../utils/interfaces';
 import { CommandRegistry } from '@lumino/commands';
 import { CompatibilityManager } from '../utils/compatibility';
-import { fetchWithCredentials } from '../utils/utils';
+import { fetchWithCredentials, generateQueryArgsString } from '../utils/utils';
 
 interface ITOCTreeProps {
   headings: INotebookHeading[];
   itemRenderer: ItemRenderer;
   notebookPanel: NotebookPanel;
   commands: CommandRegistry;
   notebookCells: string[] | null | undefined;
@@ -24,34 +24,31 @@
 
   const shouldDisplayDashboardRedux = useSelector(
     (state: RootState) => state.tocdashboard.displayDashboard
   );
   const refreshRequired = useSelector(
     (state: RootState) => state.commondashboard.refreshBoolean
   );
-  const timeWindow = useSelector(
-    (state: RootState) => state.commondashboard.timeWindow
-  );
-  const displayRealTime = useSelector(
-    (state: RootState) => state.commondashboard.displayRealTime
+  const dashboardQueryArgsRedux = useSelector(
+    (state: RootState) => state.commondashboard.dashboardQueryArgs
   );
 
   // only fetch again when the list of cells actually changed
   useEffect(() => {
     fetchToCData();
     // callback to reset the locationData
     return () => {
       setLocationData(null);
     };
   }, [props.notebookCells, props.notebookPanel]);
 
   //  or when a refresh is requested (for smoother refresh, don't reset locationData here)
   useEffect(() => {
     fetchToCData();
-  }, [refreshRequired, timeWindow]);
+  }, [refreshRequired, dashboardQueryArgsRedux]);
 
   // id to make sure only the last request resolves
   const currentRequestId = useRef<string>('12345678');
   const fetchToCData = async (): Promise<void> => {
     const notebookId = CompatibilityManager.getMetadataComp(
       props.notebookPanel.model,
       Selectors.notebookId
@@ -61,15 +58,15 @@
       return;
     }
     try {
       const newRequestId = crypto.randomUUID();
       currentRequestId.current = newRequestId;
 
       const response = await fetchWithCredentials(
-        `${BACKEND_API_URL}/dashboard/${notebookId}/toc?timeWindow=${timeWindow}&displayRealTime=${displayRealTime}`
+        `${BACKEND_API_URL}/dashboard/${notebookId}/toc?${generateQueryArgsString(dashboardQueryArgsRedux, notebookId)}`
       );
 
       // check that it's the response from the current request and not a subsequent
       if (newRequestId === currentRequestId.current) {
         if (response.ok) {
           const data = await response.json();
           setLocationData(data.data);
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/index.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/options_manager.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/options_manager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/render.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/render.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/toolbar_generator.tsx` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/toolbar_generator.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/toc-dashboard/generator/utils.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/toc-dashboard/generator/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/utils/chartOptions.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/utils/chartOptions.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/utils/compatibility.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/utils/compatibility.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/utils/interactionRecorder.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/utils/interactionRecorder.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/utils/interfaces.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/utils/interfaces.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/utils/utils.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/utils/utils.ts`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,27 @@
   ACCESS_TOKEN_KEY,
   APP_ID,
   BACKEND_API_URL,
   REFRESH_TOKEN_KEY,
   Selectors
 } from './constants';
 import { CompatibilityManager } from './compatibility';
+import { IDashboardQueryArgs } from '../redux/types';
+
+export const generateQueryArgsString = (
+  queryArgs: IDashboardQueryArgs,
+  notebookId: string
+) => {
+  return (
+    // use true for displayRealTime by default when it's not defined
+    `displayRealTime=${queryArgs.displayRealTime[notebookId] ?? true}` +
+    `${queryArgs.t1ISOString[notebookId] ? '&t1=' + queryArgs.t1ISOString[notebookId] : ''}` +
+    `${queryArgs.selectedGroups[notebookId]?.length > 0 ? '&selectedGroups=' + encodeURIComponent(JSON.stringify(queryArgs.selectedGroups[notebookId])) : ''}`
+  );
+};
 
 // adds the necessary request options to authenticate the user on the protected route (without overwriting the provided options)
 export const fetchWithCredentials = async (
   url: string,
   options?: RequestInit
 ): Promise<Response> => {
   const response = await customFetch(url, options);
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/widget-extensions/CellButton.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/widget-extensions/CellButton.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/widget-extensions/NotebookButton.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/widget-extensions/NotebookButton.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/src/widget-extensions/index.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/src/widget-extensions/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/base.css` & `jupyterlab_unianalytics_dashboard-4.0.9/style/base.css`

 * *Files 26% similar despite different names*

```diff
@@ -52,16 +52,59 @@
 }
 
 .dashboard-export-dialog-calendar-container {
   display: flex;
   flex-wrap: wrap;
   justify-content: center;
   gap: 15px;
+  cursor: default;
+  padding: 20px;
 }
 
 .dashboard-export-dialog-calendar {
   border: 1px solid var(--jp-brand-color1);
   border-radius: 3px;
   display: flex;
   flex-direction: column;
   padding: 20px;
+  cursor: pointer;
+}
+
+.dashboard-calendar-container {
+  display: flex;
+  flex-direction: column;
+  align-items: center;
+  justify-content: center;
+  gap: 12px;
+  padding: 14px 20px;
+}
+
+input.dashboard-calendar-input {
+  cursor: pointer;
+}
+
+body[data-jp-theme-light='false'] input.dashboard-calendar-input {
+  color-scheme: dark;
+}
+
+.dashboard-calendar-input-wrapper {
+  display: flex;
+  justify-content: space-between;
+  align-items: center;
+  gap: 15px;
+}
+
+.dashboard-calendar-input-wrapper.disabled {
+  opacity: 0.4;
+  cursor: not-allowed;
+}
+
+.dashboard-calendar-input-wrapper.disabled input.dashboard-calendar-input {
+  pointer-events: none;
+  background-color: var(--jp-layout-color4);
+}
+
+.dashboard-calendar-button-container {
+  display: flex;
+  justify-content: space-between;
+  padding: 20px 15px 5px;
 }
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/reactVisu.css` & `jupyterlab_unianalytics_dashboard-4.0.9/style/reactVisu.css`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .dashboard-panel {
   background-color: var(--jp-layout-color1);
 }
 
 .dashboard-react-widget {
   display: flex;
   height: 100%;
-  min-width: 320px !important;
+  min-width: 335px !important;
 }
 
 .page-container {
   display: flex;
   overflow-y: auto;
   scrollbar-gutter: stable;
   padding: 20px;
@@ -53,39 +53,29 @@
   opacity: 1;
   background-color: var(--jp-brand-color1);
   color: white;
 }
 
 .breadcrumb-buttons-container {
   margin-left: auto;
-}
-
-.breadcrumb-button {
-  margin-left: 6px;
-  background-color: var(--jp-brand-color1) !important;
-  border: none !important;
-}
-
-.breadcrumb-button:hover {
-  background-color: var(--jp-brand-color0) !important;
+  position: relative;
 }
 
 .dashboard-title-container {
   display: flex;
   margin-bottom: 15px;
   justify-content: space-between;
+  align-items: center;
 }
 
 .dashboard-title-text {
   white-space: nowrap; /* Prevent text from wrapping */
   overflow: hidden; /* Hide overflowing content */
   text-overflow: ellipsis;
-
-  /* max-width: 80%; */
-  font-size: 22px;
+  font-size: 18px;
   color: var(--jp-inverse-layout-color1);
   font-weight: 700;
 }
 
 .card {
   color: var(--jp-inverse-layout-color1) !important;
   background-color: var(--jp-layout-color2) !important;
@@ -126,66 +116,90 @@
 }
 
 .cell-radio-container .btn-group .btn {
   display: flex;
   align-items: center;
 }
 
+.cell-radio-container .btn-outline-primary {
+  border: solid 1px var(--jp-brand-color1);
+}
+
 .dashboard-dropdown-container {
   display: flex;
   margin-left: 10px;
   gap: 5px;
 }
 
-.custom-dropdown .dropdown-menu {
-  background-color: var(--jp-layout-color3);
+.custom-dropdown .dropdown-menu,
+.custom-dropdown .dropdown-item,
+.custom-dropdown .dropdown-header {
+  background-color: var(--jp-layout-color2) !important;
+  color: var(--jp-inverse-layout-color1) !important;
 }
 
-.custom-dropdown .dropdown-item {
-  color: var(--jp-inverse-layout-color1);
+.custom-dropdown .dropdown-item:hover,
+.custom-dropdown .dropdown-item.highlighted {
+  background-color: var(--jp-layout-color3) !important;
 }
 
-.custom-dropdown .dropdown-item:hover {
-  background-color: var(--jp-layout-color2);
-  color: var(--jp-inverse-layout-color1);
+.custom-dropdown .dropdown-toggle::after {
+  display: none !important;
 }
 
-.custom-dropdown .dropdown-header {
-  color: var(--jp-inverse-layout-color3);
+.custom-dropdown .dropdown-menu {
+  border-width: 2px;
+}
+
+button.dashboard-button {
+  width: 32px;
+  height: 32px;
+  display: flex;
+  justify-content: center;
+  align-items: center;
 }
 
 .cell-user-title {
   display: flex;
   justify-content: center;
   align-items: center;
   font-size: 13px;
   font-weight: 500;
   padding: 0 0 10px;
 }
 
+.cell-execution-displayed-time {
+  display: flex;
+  justify-content: end;
+  font-size: 12px;
+  font-weight: 400;
+  padding-top: 12px;
+}
+
 .cell-content-container {
   max-height: 320px;
   overflow: auto;
   padding: 10px;
   background-color: var(--jp-layout-color0);
   border: solid 1px var(--bs-card-border-color);
   border-radius: 3px;
   cursor: pointer;
 }
 
 .cell-content-container:hover {
   cursor: text;
 }
 
-.logo {
-  width: 18px;
-  height: 18px;
+.dashboard-icon {
+  width: 20px;
+  height: auto;
+  position: absolute;
 }
 
-.labicon-logo .jp-icon3 {
+.dashboard-icon .jp-icon3 {
   fill: white;
 }
 
 .no-data-card {
   margin: 10px 0;
   text-align: center;
   padding: 30px 0;
@@ -216,7 +230,49 @@
   margin-right: 10px;
 }
 
 .send-icon {
   display: flex;
   justify-content: center;
 }
+
+.custom-dropdown-container {
+  display: flex;
+  align-items: center;
+  justify-content: center;
+  padding: 6px 0;
+}
+
+.group-dropdown-scroll {
+  max-height: 215px;
+  overflow-y: auto;
+}
+
+.group-dropdown-scroll.disabled {
+  opacity: 0.4;
+  cursor: not-allowed;
+}
+
+.custom-dropdown-item {
+  padding: 8px 10px 4px 12px;
+}
+
+.custom-dropdown-item,
+.custom-dropdown-item * {
+  cursor: pointer !important;
+}
+
+.custom-dropdown-item.disabled,
+.custom-dropdown-item.disabled * {
+  cursor: not-allowed !important;
+}
+
+.custom-dropdown-item:hover:not(.disabled) {
+  background-color: var(--jp-layout-color3) !important;
+}
+
+.custom-dropdown-item label {
+  max-width: 190px;
+  overflow-x: hidden;
+  white-space: nowrap;
+  text-overflow: ellipsis;
+}
```

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/tocDashboard.css` & `jupyterlab_unianalytics_dashboard-4.0.9/style/tocDashboard.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/tocDashboardEditor.css` & `jupyterlab_unianalytics_dashboard-4.0.9/style/tocDashboardEditor.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/upload.css` & `jupyterlab_unianalytics_dashboard-4.0.9/style/upload.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/icons/analytics.svg` & `jupyterlab_unianalytics_dashboard-4.0.9/style/icons/analytics.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/icons/eyeSlash.svg` & `jupyterlab_unianalytics_dashboard-4.0.9/style/icons/eyeSlash.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/style/icons/folder.svg` & `jupyterlab_unianalytics_dashboard-4.0.9/style/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/README.md` & `jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/yarn.lock` & `jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/ui-tests/tests/jupyterlab_unianalytics_dashboard.spec.ts` & `jupyterlab_unianalytics_dashboard-4.0.9/ui-tests/tests/jupyterlab_unianalytics_dashboard.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/.gitignore` & `jupyterlab_unianalytics_dashboard-4.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/LICENSE` & `jupyterlab_unianalytics_dashboard-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/README.md` & `jupyterlab_unianalytics_dashboard-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/pyproject.toml` & `jupyterlab_unianalytics_dashboard-4.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_dashboard-4.0.8/PKG-INFO` & `jupyterlab_unianalytics_dashboard-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_unianalytics_dashboard
-Version: 4.0.8
+Version: 4.0.9
+Dynamic: Keywords
 Summary: A JupyterLab dashboard extension to visualize data from students.
 Project-URL: Homepage, https://github.com/chili-epfl/jupyter-dashboard-visu-extension
 Project-URL: Bug Tracker, https://github.com/chili-epfl/jupyter-dashboard-visu-extension/issues
 Project-URL: Repository, https://github.com/chili-epfl/jupyter-dashboard-visu-extension.git
 Author-email: Raphael Marietan <raphael.marietan@hotmail.com>
 License: BSD 3-Clause License
```

