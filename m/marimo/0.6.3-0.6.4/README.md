# Comparing `tmp/marimo-0.6.3.tar.gz` & `tmp/marimo-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marimo-0.6.3.tar", last modified: Thu May 23 04:51:18 2024, max compression
+gzip compressed data, was "marimo-0.6.4.tar", last modified: Thu May 23 17:56:01 2024, max compression
```

## Comparing `marimo-0.6.3.tar` & `marimo-0.6.4.tar`

### file list

```diff
@@ -1,752 +1,752 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.292627 marimo-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 04:50:08.000000 marimo-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 04:50:08.000000 marimo-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-23 04:51:18.292627 marimo-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-23 04:50:08.000000 marimo-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.136627 marimo-0.6.3/marimo/
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.140627 marimo-0.6.3/marimo/_ast/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_ast/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.140627 marimo-0.6.3/marimo/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/cli_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.140627 marimo-0.6.3/marimo/_cli/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/convert/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/convert/ipynb.py
--rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/convert/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/convert/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/envinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.140627 marimo-0.6.3/marimo/_cli/export/
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/export/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/parse_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/print.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.140627 marimo-0.6.3/marimo/_config/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_config/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.144627 marimo-0.6.3/marimo/_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_dependencies/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.144627 marimo-0.6.3/marimo/_islands/
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_islands/island_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.144627 marimo-0.6.3/marimo/_lsp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.144627 marimo-0.6.3/marimo/_lsp/copilot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.152627 marimo-0.6.3/marimo/_lsp/copilot/dist/
--rw-r--r--   0 runner    (1001) docker     (127)  2139874 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/agent.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.128627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.128627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.152627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/arm64/
--rw-r--r--   0 runner    (1001) docker     (127)   162128 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/arm64/kerberos.node
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.152627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/x64/
--rw-r--r--   0 runner    (1001) docker     (127)   141920 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/x64/kerberos.node
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.128627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.152627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/arm64/
--rw-r--r--   0 runner    (1001) docker     (127)  1278608 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/arm64/kerberos.node
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.156627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/x64/
--rw-r--r--   0 runner    (1001) docker     (127)  1295480 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/x64/kerberos.node
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.128627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/win32/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.156627 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/win32/x64/
--rw-r--r--   0 runner    (1001) docker     (127)   699168 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/win32/x64/kerberos.node
--rw-r--r--   0 runner    (1001) docker     (127)   140576 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/crypt32.node
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.128627 marimo-0.6.3/marimo/_lsp/copilot/dist/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.160627 marimo-0.6.3/marimo/_lsp/copilot/dist/resources/cl100k/
--rw-r--r--   0 runner    (1001) docker     (127)  2505007 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/resources/cl100k/tokenizer_cushman002.json
--rw-r--r--   0 runner    (1001) docker     (127)   916647 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/resources/cl100k/vocab_cushman002.bpe
--rw-r--r--   0 runner    (1001) docker     (127)   179802 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-go.wasm
--rw-r--r--   0 runner    (1001) docker     (127)   233302 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-javascript.wasm
--rw-r--r--   0 runner    (1001) docker     (127)   261745 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-python.wasm
--rw-r--r--   0 runner    (1001) docker     (127)   990787 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-ruby.wasm
--rw-r--r--   0 runner    (1001) docker     (127)  1041338 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-tsx.wasm
--rw-r--r--   0 runner    (1001) docker     (127)   994008 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-typescript.wasm
--rw-r--r--   0 runner    (1001) docker     (127)   186526 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter.wasm
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/copilot/info.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83596 2024-05-23 04:50:27.000000 marimo-0.6.3/marimo/_lsp/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.164627 marimo-0.6.3/marimo/_messaging/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/cell_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/completion_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/console_output_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/mimetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_messaging/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.164627 marimo-0.6.3/marimo/_output/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.164627 marimo-0.6.3/marimo/_output/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/doc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.168627 marimo-0.6.3/marimo/_output/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/altair_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/anywidget_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/bokeh_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/formatter_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/holoviews_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/ipython_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/leafmap_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/matplotlib_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/pandas_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/plotly_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/seaborn_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatters/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/hypertext.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/justify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.168627 marimo-0.6.3/marimo/_output/md_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/md_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/md_extensions/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/rich_help.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.168627 marimo-0.6.3/marimo/_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.168627 marimo-0.6.3/marimo/_plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/core/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/core/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/core/web_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.172627 marimo-0.6.3/marimo/_plugins/stateless/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/callout.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/flex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/json_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/mermaid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.172627 marimo-0.6.3/marimo/_plugins/stateless/mpl/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/mpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/mpl/_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/nav_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/plain_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/stat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.172627 marimo-0.6.3/marimo/_plugins/stateless/status/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/status/_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/stateless/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.172627 marimo-0.6.3/marimo/_plugins/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.176627 marimo-0.6.3/marimo/_plugins/ui/_core/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_core/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_core/ui_element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.176627 marimo-0.6.3/marimo/_plugins/ui/_impl/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/altair_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.176627 marimo-0.6.3/marimo/_plugins/ui/_impl/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/charts/altair_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/data_explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.176627 marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/from_anywidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    46506 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.180627 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/default_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/pandas_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/polars_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/pyarrow_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/table_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tables/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.180627 marimo-0.6.3/marimo/_plugins/ui/_impl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/ui/_impl/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.180627 marimo-0.6.3/marimo/_pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_pyodide/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_pyodide/pyodide_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_pyodide/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.184627 marimo-0.6.3/marimo/_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/cell_lifecycle_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/cell_lifecycle_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/complete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.184627 marimo-0.6.3/marimo/_runtime/context/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/context/kernel_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/context/script_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/context/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/context/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/input_override.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.184627 marimo-0.6.3/marimo/_runtime/layout/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/layout/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/marimo_pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.184627 marimo-0.6.3/marimo/_runtime/output/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/output/_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.188627 marimo-0.6.3/marimo/_runtime/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/conda_package_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/module_name_to_conda_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    28299 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/module_name_to_pypi_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/module_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/package_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/pypi_package_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/packages/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/redirect_streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.188627 marimo-0.6.3/marimo/_runtime/reload/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/reload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/reload/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/reload/module_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.188627 marimo-0.6.3/marimo/_runtime/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/cell_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/execution_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/hooks_on_finish.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/hooks_post_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/hooks_pre_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runner/hooks_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)    55011 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.188627 marimo-0.6.3/marimo/_runtime/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/utils/set_ui_element_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/validate_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/virtual_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_runtime/win32_interrupt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.192627 marimo-0.6.3/marimo/_server/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.192627 marimo-0.6.3/marimo/_server/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/deps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.196627 marimo-0.6.3/marimo/_server/api/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/editing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/file_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/endpoints/ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/interrupt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/lifespans.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.196627 marimo-0.6.3/marimo/_server/export/
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/export/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/file_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.196627 marimo-0.6.3/marimo/_server/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/files/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/files/os_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.196627 marimo-0.6.3/marimo/_server/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/print.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/recents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.196627 marimo-0.6.3/marimo/_server/session/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/session/session_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    28244 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.196627 marimo-0.6.3/marimo/_server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/templates/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_server/uvicorn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.204627 marimo-0.6.3/marimo/_smoke_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/admonitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/altair_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/anywidget_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/arrays_and_dicts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.208627 marimo-0.6.3/marimo/_smoke_tests/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1055.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1064.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1072.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1086.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1107.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1140.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1161.py
--rw-r--r--   0 runner    (1001) docker     (127)    42796 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1165.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1241.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1270.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1271.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1273.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1274.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1279.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1291.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1311.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1312.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1319.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1351.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/1362.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/846.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/852.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/877.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/881.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/924.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/altair_bug.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/bugs/key_with_period.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/carousel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.208627 marimo-0.6.3/marimo/_smoke_tests/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/charts/1mil_flights.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/code_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.208627 marimo-0.6.3/marimo/_smoke_tests/custom_server/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/custom_server/my_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/data_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/full_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/import_named_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/iplot.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/lens_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/md.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/named_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/nav_menus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/pdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/raise_error_on_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/raise_exception_on_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/scripting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/stdin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.208627 marimo-0.6.3/marimo/_smoke_tests/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/altair_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/holoviews_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/ipython_display.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/pandas_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/plotly_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/rich_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/third_party/seaborn_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_smoke_tests/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.208627 marimo-0.6.3/marimo/_snippets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.216627 marimo-0.6.3/marimo/_snippets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-0.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-1.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-2.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-4.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-5.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-7.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/altair-8.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/cli-args-0.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-0.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-10.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-11.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-12.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-13.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-14.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-15.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-16.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-17.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-18.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-19.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-2.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-20.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-21.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-22.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-23.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-24.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-25.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-3.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-4.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-5.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-6.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-7.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-8.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/pandas-9.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/query-params-0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/data/query-params-1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_snippets/snippets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.216627 marimo-0.6.3/marimo/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    39067 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.276627 marimo-0.6.3/marimo/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/CarouselComponent-C12Ecb2K.css
--rw-r--r--   0 runner    (1001) docker     (127)   111027 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/CarouselComponent-DtCAwyzo.js
--rw-r--r--   0 runner    (1001) docker     (127)   128198 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ConnectedDataExplorerComponent-DKdMG7z6.js
--rw-r--r--   0 runner    (1001) docker     (127)   201708 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/FiraMono-Bold-CLVRCuM9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   169056 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/FiraMono-Medium-DU3aDxX5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170204 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/FiraMono-Regular-BTCkDNvf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_AMS-Regular-BQhdFMY1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_AMS-Regular-DMm9YOAa.woff
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_AMS-Regular-DRggAlZN.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Bold-ATXxdsX0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Bold-BEiXGLvX.woff
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Bold-Dq_IR9rO.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Regular-CTRA-rTL.woff
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Regular-Di6jR-x-.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Regular-wX97UBjC.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Bold-BdnERNNW.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Bold-BsDP51OF.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Bold-CL6g_b3V.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Regular-CB_wures.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Regular-CTYiF6lA.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Regular-Dxdc4cR9.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Bold-Cx986IdX.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Bold-Jm3AIy58.woff
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Bold-waoOVXN0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-BoldItalic-DxDJ3AOS.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-BoldItalic-DzxPMmG6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-BoldItalic-SpSLRI95.woff
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Italic-3WenGoN9.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Italic-BMLOBm91.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Italic-NWA7e6Wa.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Regular-B22Nviop.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Regular-Dr94JaBh.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Regular-ypZvNtVU.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Math-BoldItalic-B3XSjfu4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Math-BoldItalic-CZnvNsCZ.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Math-BoldItalic-iY-2wyZ7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Math-Italic-DA0__PXp.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Math-Italic-flOr_0UB.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Math-Italic-t53AETM-.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Bold-CFMepnvq.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Bold-D1sUS0GD.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Bold-DbIhKOiC.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Italic-C3H0VqGB.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Italic-DN2j7dab.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Italic-YYjJ1zSn.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Regular-BNo7hRIc.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Regular-CS6fqUqJ.woff
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Regular-DDBCnlJ7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Script-Regular-C5JkGWo-.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Script-Regular-D3wIWfF6.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Script-Regular-D5yQViql.woff
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size1-Regular-C195tn64.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size1-Regular-Dbsnue_I.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size1-Regular-mCD8mA8B.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size2-Regular-B7gKUWhC.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size2-Regular-Dy4dx90m.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size2-Regular-oD1tc_U0.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size3-Regular-CTq5MqoE.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size3-Regular-DgpXs0kz.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size4-Regular-BF-4gkZK.woff
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size4-Regular-DWFBv043.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Size4-Regular-Dl5lxZxV.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Typewriter-Regular-C0xS9mPB.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Typewriter-Regular-CO6r4hn1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/KaTeX_Typewriter-Regular-D3Ib7_Hf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   212004 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/Lora-VariableFont_wght-B2ootaw-.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   288340 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/PTSans-Bold-D9fedIX3.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   278612 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/PTSans-Regular-CxL0S8W7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/Tableau10-B3EzvwxR.js
--rw-r--r--   0 runner    (1001) docker     (127)   740123 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/VegaLite-BQwzJofD.js
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/_baseEach-BrSWFoJM.js
--rw-r--r--   0 runner    (1001) docker     (127)   427678 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/any-language-editor-D3MTmtyo.js
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/apl-CXdQSnD-.js
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/arc-DIImc9ZO.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/array-DmjLdZ15.js
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/asciiarmor-D5V0T9Cu.js
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/asn1-BhA3SgW2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/asterisk-B46aRdXb.js
--rw-r--r--   0 runner    (1001) docker     (127)    36266 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/blockDiagram-91b80b7a-DPH13Qrf.js
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/brainfuck-CtZaYBKt.js
--rw-r--r--   0 runner    (1001) docker     (127)    66791 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/c4Diagram-b2a90758-CAH0Datt.js
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/channel-DCiFYtzP.js
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/classDiagram-30eddba6-Bz0cJX-U.js
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/classDiagram-v2-f2df5561-BxNEwu6g.js
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/clike-BPCXT8V3.js
--rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/clojure-DR_hEDJv.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/clone-BL0WSZ3Z.js
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/cmake-DXn5xaP-.js
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/cobol-DJhTY0fG.js
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/coffeescript-BTDxI-eT.js
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/commonlisp-D09g7coK.js
--rw-r--r--   0 runner    (1001) docker     (127)    59346 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/createText-6b48ae7d-129t9twG.js
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/crystal-CRzZ78HM.js
--rw-r--r--   0 runner    (1001) docker     (127)    26935 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/css-ZjFoif2m.js
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/cypher-gJDei3ni.js
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/d-BShv7fp-.js
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/diff-UJJ5BM9S.js
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/dockerfile-BLgfkd__.js
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/dtd-DI9Herc-.js
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/dylan-CHJ5qNM_.js
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ebnf-B-Df8AvO.js
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ecl-DPFc0Uaf.js
--rw-r--r--   0 runner    (1001) docker     (127)    34123 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/edges-d32062c0-CFY3bIwa.js
--rw-r--r--   0 runner    (1001) docker     (127)   488283 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/edit-page-CIzFhPq5.js
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/edit-page-CwGzkSpM.css
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/eiffel-BZ5y0wDL.js
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/elm-D7xaZ7Da.js
--rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/erDiagram-47591fe2-CJ2SMwAy.js
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/erlang-BuqgqA5h.js
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/factor-Bm2WRyNM.js
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/fcl-CVaBTCzQ.js
--rw-r--r--   0 runner    (1001) docker     (127)    45479 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/flowDb-4b19a42f-4mXsCvSf.js
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/flowDiagram-5540d9b9-msf8H4Jk.js
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/flowDiagram-v2-3b53844e-BRBAHwua.js
--rw-r--r--   0 runner    (1001) docker     (127)  1496785 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/flowchart-elk-definition-5fe447d6-tgRhUdQk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/forth-Dri_5nFc.js
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/fortran-DL7KluxX.js
--rw-r--r--   0 runner    (1001) docker     (127)    42449 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ganttDiagram-9a3bba1f-Clnqsx9q.js
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/gas-5kEe4nk0.js
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/gherkin-B6X1vGSW.js
--rw-r--r--   0 runner    (1001) docker     (127)    38271 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/gitGraphDiagram-96e6b4ee-BUgJQeEj.js
--rw-r--r--   0 runner    (1001) docker     (127)   371126 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/gradient-yHQUC_QB.png
--rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/graph-SHnEHiLi.js
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/groovy-BfRUB6GO.js
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/haskell-CmdsSjFB.js
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/haxe-75PMBtaN.js
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/home-page-BmvI7Tzs.js
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/http-BKJkqRj4.js
--rw-r--r--   0 runner    (1001) docker     (127)   307050 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/icons-6JftBaIY.js
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/icons-D-PkNarU.css
--rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/idl-pcmmZuaN.js
--rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-0fF0Xoai.js
--rw-r--r--   0 runner    (1001) docker     (127)   101285 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-7VEF_U3p.js
--rw-r--r--   0 runner    (1001) docker     (127)    70671 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-BuR6fZZm.js
--rw-r--r--   0 runner    (1001) docker     (127)    39890 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-C2GbrbZr.js
--rw-r--r--   0 runner    (1001) docker     (127)   167140 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-CC7Qmxzq.css
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-ChUg6Fde.js
--rw-r--r--   0 runner    (1001) docker     (127)    94582 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-Ck0jzFpb.js
--rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-ClCDnvOE.js
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-CohQOVlj.js
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-CzWuvzvc.js
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-D4als0Dc.js
--rw-r--r--   0 runner    (1001) docker     (127)    20483 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-DgcwnKY7.js
--rw-r--r--   0 runner    (1001) docker     (127)  1911856 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-Dq6tg2Hn.js
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-DzhIfGoT.js
--rw-r--r--   0 runner    (1001) docker     (127)    30678 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-O7K-_bwp.js
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-S9qVQ2oC.js
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-VNKARDPQ.js
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-fc10efb0-C3SRzTfT.js
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/index-jW3n8_hn.js
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/infoDiagram-bcd20f53-BIy3DJKx.js
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/init-DLRA0X12.js
--rw-r--r--   0 runner    (1001) docker     (127)    16569 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/javascript-DY1Qj14w.js
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/jinja2-DhgKlfW7.js
--rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/journeyDiagram-4fe6b3dc-C_g7a5O5.js
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/julia-DjdwvFuI.js
--rw-r--r--   0 runner    (1001) docker     (127)   266157 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/katex-BnMoLUs3.js
--rw-r--r--   0 runner    (1001) docker     (127)    26820 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/layout-DDD1odkP.js
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/line-Dz7yhIWK.js
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/linear-DF6Se9n2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/livescript-B19OIWEP.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/lua-8DXOpKDz.js
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mathematica-IIbmv7SK.js
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mbox-DoeuZPxA.js
--rw-r--r--   0 runner    (1001) docker     (127)   190576 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mermaid-BDDPrcgz.js
--rw-r--r--   0 runner    (1001) docker     (127)   462371 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mindmap-definition-f354de21-BT0462Yo.js
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mirc-DkvFAiy5.js
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mllike-B8DYu8SS.js
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/modelica-DSrSSXCg.js
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mscgen-B2igx18G.js
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/mumps-zvxmGV4l.js
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/nginx-B4hAVlXN.js
--rw-r--r--   0 runner    (1001) docker     (127)    45435 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/noise-60BoTA8O.png
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/nsis-Csd3_MSv.js
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ntriples-FFvkTduk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/octave-C4hdQ5Hf.js
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ordinal-DDUp3AbE.js
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/oz-qQq7irPq.js
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/pascal-CZ0JYm71.js
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/path-qnb_ma6O.js
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/perl-tdMlh9QA.js
--rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/pieDiagram-79897490-DVu-KYPX.js
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/pig-CwGJVRC4.js
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/powershell-D1ly3AHC.js
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/properties-_nPj978X.js
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/protobuf-B4y9do6W.js
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/pug-BNyZbGOm.js
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/puppet-Bc-yJKzi.js
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/python-DD-Q2bae.js
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/q-B0kTJ4cI.js
--rw-r--r--   0 runner    (1001) docker     (127)    29143 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/quadrantDiagram-62f64e94-CU-4FuJa.js
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/r-BA4EbLKE.js
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/range-CtcPcB_L.js
--rw-r--r--   0 runner    (1001) docker     (127)  3627419 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/react-plotly-Bf9tHX8H.js
--rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/requirementDiagram-05bf5f74-BsI08XXR.js
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/rpm-DI_rRufH.js
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ruby-CR-u2WLS.js
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/run-page-BflrRP7S.js
--rw-r--r--   0 runner    (1001) docker     (127)    21255 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sankeyDiagram-97764748-BQdZQP_-.js
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sas-Bqaci40L.js
--rw-r--r--   0 runner    (1001) docker     (127)    67039 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/save-worker-f86VBHv4.js
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/scheme-qjP0V5Ag.js
--rw-r--r--   0 runner    (1001) docker     (127)    83341 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sequenceDiagram-acc0e65c-Dsgiz64s.js
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/shell-BLav31RL.js
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sieve-r025o_jW.js
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/simple-mode-Ckv7_vD8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/smalltalk-C7J3IyEP.js
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/solr-78MBEUkU.js
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sortBy-D0xI_7yL.js
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sparql-BRLJFz69.js
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/spreadsheet-CGlWr0eM.js
--rw-r--r--   0 runner    (1001) docker     (127)    37034 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/sql-BP5jFf-w.js
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/stateDiagram-0ff1cf1a-lr9-t8r1.js
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/stateDiagram-v2-9a9d610d-DwjKCx-9.js
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/step-BEJ6WznM.js
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/stex-Ba7Sj9VR.js
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/styles-3ed67cfa-QdZmR4us.js
--rw-r--r--   0 runner    (1001) docker     (127)    37103 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/styles-991ebdfc-CV9pCNxb.js
--rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/styles-d20c7d72-BOwpCRGP.js
--rw-r--r--   0 runner    (1001) docker     (127)    25768 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/stylus-C-RTeXnz.js
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/svgDrawCommon-5ccd53ef-BK5P1sG2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/swift-Cbprqdc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/tcl-B2fODqDH.js
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/textile-BuVhTOzU.js
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/tiddlywiki-BgR6AEZu.js
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/tiki-CI-ztowC.js
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/time-CUBsQdfc.js
--rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/timeline-definition-fea2a41d-B6Whk07l.js
--rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/timer-D8GWrtRJ.js
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/toml-BQXy8elZ.js
--rw-r--r--   0 runner    (1001) docker     (127)    24911 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/transform-DGMfQOK3.js
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/troff-Ce85hlLp.js
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ttcn-C4reStyN.js
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/ttcn-cfg-Ce4xWtqN.js
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/turtle-BkSuIpt-.js
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/useMarimoWebSocket-BjNzCf7j.css
--rw-r--r--   0 runner    (1001) docker     (127)   130058 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/useMarimoWebSocket-DFV8TeGX.js
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/vb-coDLL1b7.js
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/vbscript-MdTt_wcJ.js
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/vega-component-CZ4hZbd6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/velocity-BdD_26Jv.js
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/verilog-B4LBqg_1.js
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/vhdl-BRDI21CQ.js
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/webidl-CGwyPRYs.js
--rw-r--r--   0 runner    (1001) docker     (127)    69134 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/worker-DRJqITgt.js
--rw-r--r--   0 runner    (1001) docker     (127)    69835 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/worker-DeVBMRpt.js
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/xquery-BZBLoTvf.js
--rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/xychartDiagram-ab372869-DViGpnfl.js
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/yacas-I8QjZlxf.js
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/assets/z80-D8p3gKXp.js
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/invalid_kernel_id.html
--rw-r--r--   0 runner    (1001) docker     (127)    65475 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-23 04:50:24.000000 marimo-0.6.3/marimo/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.280627 marimo-0.6.3/marimo/_tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/fileformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/for_jupyter_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/markdown_format.md
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_tutorials/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.284627 marimo-0.6.3/marimo/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.284627 marimo-0.6.3/marimo/_utils/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/deep_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/distributor.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/exiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/format_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/marimo_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/parse_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/rst_to_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/typed_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/_utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 04:50:08.000000 marimo-0.6.3/marimo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:51:18.284627 marimo-0.6.3/marimo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-23 04:51:18.000000 marimo-0.6.3/marimo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-05-23 04:51:18.000000 marimo-0.6.3/marimo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 04:51:18.000000 marimo-0.6.3/marimo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 04:51:18.000000 marimo-0.6.3/marimo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 04:51:18.000000 marimo-0.6.3/marimo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 04:51:18.000000 marimo-0.6.3/marimo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-05-23 04:50:08.000000 marimo-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 04:51:18.292627 marimo-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-23 04:50:08.000000 marimo-0.6.3/third_party.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20490 2024-05-23 04:50:08.000000 marimo-0.6.3/third_party_licenses.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.912661 marimo-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 17:54:52.000000 marimo-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 17:54:52.000000 marimo-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-23 17:56:01.912661 marimo-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-23 17:54:52.000000 marimo-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.764661 marimo-0.6.4/marimo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.764661 marimo-0.6.4/marimo/_ast/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_ast/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/cli_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_cli/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/convert/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/convert/ipynb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/convert/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/convert/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/envinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_cli/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/export/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/parse_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_config/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_dependencies/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_islands/
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_islands/island_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_lsp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.768661 marimo-0.6.4/marimo/_lsp/copilot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.780661 marimo-0.6.4/marimo/_lsp/copilot/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)  2139874 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/agent.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.756661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.756661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.780661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/arm64/
+-rw-r--r--   0 runner    (1001) docker     (127)   162128 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/arm64/kerberos.node
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.780661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/x64/
+-rw-r--r--   0 runner    (1001) docker     (127)   141920 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/x64/kerberos.node
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.756661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.780661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/arm64/
+-rw-r--r--   0 runner    (1001) docker     (127)  1278608 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/arm64/kerberos.node
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.780661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/x64/
+-rw-r--r--   0 runner    (1001) docker     (127)  1295480 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/x64/kerberos.node
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.756661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/win32/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.784661 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/win32/x64/
+-rw-r--r--   0 runner    (1001) docker     (127)   699168 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/win32/x64/kerberos.node
+-rw-r--r--   0 runner    (1001) docker     (127)   140576 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/crypt32.node
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.756661 marimo-0.6.4/marimo/_lsp/copilot/dist/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.788661 marimo-0.6.4/marimo/_lsp/copilot/dist/resources/cl100k/
+-rw-r--r--   0 runner    (1001) docker     (127)  2505007 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/resources/cl100k/tokenizer_cushman002.json
+-rw-r--r--   0 runner    (1001) docker     (127)   916647 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/resources/cl100k/vocab_cushman002.bpe
+-rw-r--r--   0 runner    (1001) docker     (127)   179802 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-go.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)   233302 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-javascript.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)   261745 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-python.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)   990787 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-ruby.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)  1041338 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-tsx.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)   994008 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-typescript.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)   186526 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter.wasm
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/copilot/info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83596 2024-05-23 17:55:12.000000 marimo-0.6.4/marimo/_lsp/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.792661 marimo-0.6.4/marimo/_messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/cell_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/completion_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/console_output_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/mimetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_messaging/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.792661 marimo-0.6.4/marimo/_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.792661 marimo-0.6.4/marimo/_output/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/doc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.796661 marimo-0.6.4/marimo/_output/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/altair_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/anywidget_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/bokeh_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/formatter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/holoviews_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/ipython_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/leafmap_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/matplotlib_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/pandas_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/plotly_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/seaborn_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/hypertext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/justify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.796661 marimo-0.6.4/marimo/_output/md_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/md_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/md_extensions/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/rich_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.796661 marimo-0.6.4/marimo/_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.796661 marimo-0.6.4/marimo/_plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/core/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/core/web_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.800661 marimo-0.6.4/marimo/_plugins/stateless/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/callout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/flex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/json_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/mermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.800661 marimo-0.6.4/marimo/_plugins/stateless/mpl/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/mpl/_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/nav_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/plain_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/stat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.800661 marimo-0.6.4/marimo/_plugins/stateless/status/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/status/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/stateless/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.800661 marimo-0.6.4/marimo/_plugins/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.800661 marimo-0.6.4/marimo/_plugins/ui/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_core/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_core/ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.804661 marimo-0.6.4/marimo/_plugins/ui/_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/altair_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.804661 marimo-0.6.4/marimo/_plugins/ui/_impl/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/charts/altair_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/data_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.804661 marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/from_anywidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46506 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.804661 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/default_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/pandas_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/polars_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/pyarrow_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/table_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tables/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.804661 marimo-0.6.4/marimo/_plugins/ui/_impl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/ui/_impl/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.804661 marimo-0.6.4/marimo/_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_pyodide/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_pyodide/pyodide_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_pyodide/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.808661 marimo-0.6.4/marimo/_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/cell_lifecycle_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/cell_lifecycle_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/complete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.808661 marimo-0.6.4/marimo/_runtime/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/context/kernel_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/context/script_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/context/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/context/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19678 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/input_override.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.808661 marimo-0.6.4/marimo/_runtime/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/layout/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/marimo_pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.808661 marimo-0.6.4/marimo/_runtime/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/output/_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.812661 marimo-0.6.4/marimo/_runtime/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/conda_package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/module_name_to_conda_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28299 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/module_name_to_pypi_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/module_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/package_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/pypi_package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/packages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/redirect_streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.812661 marimo-0.6.4/marimo/_runtime/reload/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/reload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/reload/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/reload/module_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.812661 marimo-0.6.4/marimo/_runtime/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/cell_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/execution_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/hooks_on_finish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/hooks_post_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/hooks_pre_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runner/hooks_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55011 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.812661 marimo-0.6.4/marimo/_runtime/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/utils/set_ui_element_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/validate_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/virtual_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_runtime/win32_interrupt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.816661 marimo-0.6.4/marimo/_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.816661 marimo-0.6.4/marimo/_server/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.820661 marimo-0.6.4/marimo/_server/api/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/editing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/file_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/endpoints/ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/lifespans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.820661 marimo-0.6.4/marimo/_server/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/export/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/file_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.820661 marimo-0.6.4/marimo/_server/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/files/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/files/os_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.820661 marimo-0.6.4/marimo/_server/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/recents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.820661 marimo-0.6.4/marimo/_server/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/session/session_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28244 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.820661 marimo-0.6.4/marimo/_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/templates/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_server/uvicorn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.828661 marimo-0.6.4/marimo/_smoke_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/admonitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/altair_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/anywidget_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/arrays_and_dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.832661 marimo-0.6.4/marimo/_smoke_tests/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1055.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1064.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1072.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1086.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1107.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1140.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1161.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42796 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1165.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1241.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1270.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1271.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1273.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1274.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1279.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1291.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1312.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1319.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1351.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/1362.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/846.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/852.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/877.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/881.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/altair_bug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/bugs/key_with_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/carousel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.832661 marimo-0.6.4/marimo/_smoke_tests/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/charts/1mil_flights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/code_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.832661 marimo-0.6.4/marimo/_smoke_tests/custom_server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/custom_server/my_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/data_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/full_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/import_named_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/iplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/lens_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/named_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/nav_menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/pdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/raise_error_on_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/raise_exception_on_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/stdin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.836661 marimo-0.6.4/marimo/_smoke_tests/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/altair_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/holoviews_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/ipython_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/pandas_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/plotly_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/rich_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/third_party/seaborn_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_smoke_tests/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.836661 marimo-0.6.4/marimo/_snippets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.840661 marimo-0.6.4/marimo/_snippets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/altair-8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/cli-args-0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-17.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-22.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-23.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-25.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/pandas-9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/query-params-0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/data/query-params-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_snippets/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.844661 marimo-0.6.4/marimo/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39067 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.900661 marimo-0.6.4/marimo/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/CarouselComponent-C12Ecb2K.css
+-rw-r--r--   0 runner    (1001) docker     (127)   111027 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/CarouselComponent-ml4W_PuP.js
+-rw-r--r--   0 runner    (1001) docker     (127)   128198 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ConnectedDataExplorerComponent-B6WI1UcR.js
+-rw-r--r--   0 runner    (1001) docker     (127)   201708 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/FiraMono-Bold-CLVRCuM9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   169056 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/FiraMono-Medium-DU3aDxX5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170204 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/FiraMono-Regular-BTCkDNvf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_AMS-Regular-BQhdFMY1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_AMS-Regular-DMm9YOAa.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_AMS-Regular-DRggAlZN.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Bold-ATXxdsX0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Bold-BEiXGLvX.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Bold-Dq_IR9rO.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Regular-CTRA-rTL.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Regular-Di6jR-x-.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Regular-wX97UBjC.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Bold-BdnERNNW.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Bold-BsDP51OF.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Bold-CL6g_b3V.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Regular-CB_wures.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Regular-CTYiF6lA.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Regular-Dxdc4cR9.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Bold-Cx986IdX.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Bold-Jm3AIy58.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Bold-waoOVXN0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-BoldItalic-DxDJ3AOS.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-BoldItalic-DzxPMmG6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-BoldItalic-SpSLRI95.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Italic-3WenGoN9.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Italic-BMLOBm91.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Italic-NWA7e6Wa.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Regular-B22Nviop.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Regular-Dr94JaBh.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Regular-ypZvNtVU.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Math-BoldItalic-B3XSjfu4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Math-BoldItalic-CZnvNsCZ.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Math-BoldItalic-iY-2wyZ7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Math-Italic-DA0__PXp.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Math-Italic-flOr_0UB.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Math-Italic-t53AETM-.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Bold-CFMepnvq.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Bold-D1sUS0GD.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Bold-DbIhKOiC.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Italic-C3H0VqGB.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Italic-DN2j7dab.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Italic-YYjJ1zSn.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Regular-BNo7hRIc.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Regular-CS6fqUqJ.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Regular-DDBCnlJ7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Script-Regular-C5JkGWo-.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Script-Regular-D3wIWfF6.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Script-Regular-D5yQViql.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size1-Regular-C195tn64.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size1-Regular-Dbsnue_I.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size1-Regular-mCD8mA8B.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size2-Regular-B7gKUWhC.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size2-Regular-Dy4dx90m.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size2-Regular-oD1tc_U0.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size3-Regular-CTq5MqoE.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size3-Regular-DgpXs0kz.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size4-Regular-BF-4gkZK.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size4-Regular-DWFBv043.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Size4-Regular-Dl5lxZxV.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Typewriter-Regular-C0xS9mPB.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Typewriter-Regular-CO6r4hn1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/KaTeX_Typewriter-Regular-D3Ib7_Hf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   212004 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/Lora-VariableFont_wght-B2ootaw-.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   288340 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/PTSans-Bold-D9fedIX3.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   278612 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/PTSans-Regular-CxL0S8W7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/Tableau10-B3EzvwxR.js
+-rw-r--r--   0 runner    (1001) docker     (127)   740123 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/VegaLite-rQgmZ7vL.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/_baseEach-FAhoh2N5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   427678 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/any-language-editor-Dzf9Jczi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/apl-CXdQSnD-.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/arc-DIImc9ZO.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/array-DmjLdZ15.js
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/asciiarmor-D5V0T9Cu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/asn1-BhA3SgW2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/asterisk-B46aRdXb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36266 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/blockDiagram-91b80b7a-DSsN5jAx.js
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/brainfuck-CtZaYBKt.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66791 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/c4Diagram-b2a90758-f1UFjA-x.js
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/channel-BmGrl1HB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/classDiagram-30eddba6-BabWtcIB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/classDiagram-v2-f2df5561-D5SEk3xC.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/clike-BPCXT8V3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/clojure-DR_hEDJv.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/clone-CrCyWe3U.js
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/cmake-DXn5xaP-.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/cobol-DJhTY0fG.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/coffeescript-BTDxI-eT.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/commonlisp-D09g7coK.js
+-rw-r--r--   0 runner    (1001) docker     (127)    59346 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/createText-6b48ae7d-BgOE7dMp.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/crystal-CRzZ78HM.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26935 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/css-ZjFoif2m.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/cypher-gJDei3ni.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/d-BShv7fp-.js
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/diff-UJJ5BM9S.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/dockerfile-BLgfkd__.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/dtd-DI9Herc-.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/dylan-CHJ5qNM_.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ebnf-B-Df8AvO.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ecl-DPFc0Uaf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34123 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/edges-d32062c0-CU6OCHwI.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/edit-page-CwGzkSpM.css
+-rw-r--r--   0 runner    (1001) docker     (127)   488251 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/edit-page-DnXnHWMg.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/eiffel-BZ5y0wDL.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/elm-D7xaZ7Da.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/erDiagram-47591fe2-UyJH0JYd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/erlang-BuqgqA5h.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/factor-Bm2WRyNM.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/fcl-CVaBTCzQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45479 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/flowDb-4b19a42f-Cf4l3Vi7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/flowDiagram-5540d9b9-CuVcDbrT.js
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/flowDiagram-v2-3b53844e-By9U58mT.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1496785 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/flowchart-elk-definition-5fe447d6-BpUsl4Jm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/forth-Dri_5nFc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/fortran-DL7KluxX.js
+-rw-r--r--   0 runner    (1001) docker     (127)    42449 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ganttDiagram-9a3bba1f-W6mmWQNE.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/gas-5kEe4nk0.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/gherkin-B6X1vGSW.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38271 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/gitGraphDiagram-96e6b4ee-BKc9lhir.js
+-rw-r--r--   0 runner    (1001) docker     (127)   371126 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/gradient-yHQUC_QB.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/graph-Dl9Z7r13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/groovy-BfRUB6GO.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/haskell-CmdsSjFB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/haxe-75PMBtaN.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/home-page-BL9ArKPs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/http-BKJkqRj4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/icons-D-PkNarU.css
+-rw-r--r--   0 runner    (1001) docker     (127)   307467 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/icons-DtRVr9-T.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/idl-pcmmZuaN.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-1IpQZ_Yu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-AJ6VyMaJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-BH1DvUFb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-BYVYp6Ei.js
+-rw-r--r--   0 runner    (1001) docker     (127)    94582 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-CB4e2-IR.js
+-rw-r--r--   0 runner    (1001) docker     (127)   167140 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-CC7Qmxzq.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70671 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-CE06HdF7.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1911856 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-Cd3MtTMQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    39890 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-DCESMHe2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20483 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-DahJleVt.js
+-rw-r--r--   0 runner    (1001) docker     (127)   101285 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-DgOauLen.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-DqGPWGPa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-DtyNPFfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-KIzq3vhX.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-XFgu4285.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-fc10efb0-CJWvKICv.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-rXOiTwQN.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30678 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-wbyGdlc1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/index-yuQsQmno.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/infoDiagram-bcd20f53-CAV4G93w.js
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/init-DLRA0X12.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16569 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/javascript-DY1Qj14w.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/jinja2-DhgKlfW7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/journeyDiagram-4fe6b3dc-DOB96Qnq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/julia-DjdwvFuI.js
+-rw-r--r--   0 runner    (1001) docker     (127)   266157 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/katex-BnMoLUs3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26820 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/layout-BdT9zkSH.js
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/line-Dz7yhIWK.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/linear-JxYcrfvc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/livescript-B19OIWEP.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/lua-8DXOpKDz.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mathematica-IIbmv7SK.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mbox-DoeuZPxA.js
+-rw-r--r--   0 runner    (1001) docker     (127)   190576 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mermaid-BI4dofVe.js
+-rw-r--r--   0 runner    (1001) docker     (127)   462371 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mindmap-definition-f354de21-CQ2IslvL.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mirc-DkvFAiy5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mllike-B8DYu8SS.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/modelica-DSrSSXCg.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mscgen-B2igx18G.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/mumps-zvxmGV4l.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/nginx-B4hAVlXN.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45435 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/noise-60BoTA8O.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/nsis-Csd3_MSv.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ntriples-FFvkTduk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/octave-C4hdQ5Hf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ordinal-DDUp3AbE.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/oz-qQq7irPq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/pascal-CZ0JYm71.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/path-qnb_ma6O.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/perl-tdMlh9QA.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/pieDiagram-79897490-DznITiVM.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/pig-CwGJVRC4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/powershell-D1ly3AHC.js
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/properties-_nPj978X.js
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/protobuf-B4y9do6W.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/pug-BNyZbGOm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/puppet-Bc-yJKzi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/python-DD-Q2bae.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/q-B0kTJ4cI.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29143 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/quadrantDiagram-62f64e94-Df4mAWqb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/r-BA4EbLKE.js
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/range-CtcPcB_L.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3627419 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/react-plotly-C4-ZLKix.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/requirementDiagram-05bf5f74-DyUtzGOy.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/rpm-DI_rRufH.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ruby-CR-u2WLS.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/run-page-D_UJForb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21255 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sankeyDiagram-97764748-DvvFNiJT.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sas-Bqaci40L.js
+-rw-r--r--   0 runner    (1001) docker     (127)    67039 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/save-worker-f86VBHv4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/scheme-qjP0V5Ag.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83341 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sequenceDiagram-acc0e65c-DquwX6r9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/shell-BLav31RL.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sieve-r025o_jW.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/simple-mode-Ckv7_vD8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/smalltalk-C7J3IyEP.js
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/solr-78MBEUkU.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sortBy-DwX0cqqB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sparql-BRLJFz69.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/spreadsheet-CGlWr0eM.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37034 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/sql-BP5jFf-w.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/stateDiagram-0ff1cf1a-DjUkVeHK.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/stateDiagram-v2-9a9d610d-C6LzE_mY.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/step-BEJ6WznM.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/stex-Ba7Sj9VR.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/styles-3ed67cfa-Cg_XeDUz.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37103 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/styles-991ebdfc-vxk4XA-a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/styles-d20c7d72-DtCcJufV.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25768 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/stylus-C-RTeXnz.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/svgDrawCommon-5ccd53ef-DsDJYju_.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/swift-Cbprqdc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/tcl-B2fODqDH.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/textile-BuVhTOzU.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/tiddlywiki-BgR6AEZu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/tiki-CI-ztowC.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/time-CLRyKR-T.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/timeline-definition-fea2a41d-DQvyLJzo.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/timer-D8GWrtRJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/toml-BQXy8elZ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24911 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/transform-DNjxe6pi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/troff-Ce85hlLp.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ttcn-C4reStyN.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/ttcn-cfg-Ce4xWtqN.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/turtle-BkSuIpt-.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/useMarimoWebSocket-BjNzCf7j.css
+-rw-r--r--   0 runner    (1001) docker     (127)   130058 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/useMarimoWebSocket-Butgv0ej.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/vb-coDLL1b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/vbscript-MdTt_wcJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/vega-component-B9WTop1f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/velocity-BdD_26Jv.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/verilog-B4LBqg_1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/vhdl-BRDI21CQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/webidl-CGwyPRYs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69134 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/worker-DRJqITgt.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69835 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/worker-DeVBMRpt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/xquery-BZBLoTvf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/xychartDiagram-ab372869-1vV9tLRe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/yacas-I8QjZlxf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/assets/z80-D8p3gKXp.js
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/invalid_kernel_id.html
+-rw-r--r--   0 runner    (1001) docker     (127)    65475 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-23 17:55:09.000000 marimo-0.6.4/marimo/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.904661 marimo-0.6.4/marimo/_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/fileformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/for_jupyter_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/markdown_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_tutorials/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.908661 marimo-0.6.4/marimo/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.908661 marimo-0.6.4/marimo/_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/deep_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/exiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/format_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/marimo_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/parse_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/rst_to_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/typed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/_utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:54:53.000000 marimo-0.6.4/marimo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:56:01.908661 marimo-0.6.4/marimo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-23 17:56:01.000000 marimo-0.6.4/marimo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-05-23 17:56:01.000000 marimo-0.6.4/marimo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:56:01.000000 marimo-0.6.4/marimo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 17:56:01.000000 marimo-0.6.4/marimo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 17:56:01.000000 marimo-0.6.4/marimo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 17:56:01.000000 marimo-0.6.4/marimo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-05-23 17:54:53.000000 marimo-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:56:01.912661 marimo-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-23 17:54:53.000000 marimo-0.6.4/third_party.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20490 2024-05-23 17:54:53.000000 marimo-0.6.4/third_party_licenses.txt
```

### Comparing `marimo-0.6.3/LICENSE` & `marimo-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/PKG-INFO` & `marimo-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marimo
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library for making reactive notebooks and apps
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `marimo-0.6.3/README.md` & `marimo-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/__init__.py` & `marimo-0.6.4/marimo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     "style",
     "tabs",
     "tree",
     "ui",
     "video",
     "vstack",
 ]
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 from marimo._ast.app import App
 from marimo._ast.cell import Cell
 from marimo._islands.island_generator import MarimoIslandGenerator
 from marimo._output.doc import doc
 from marimo._output.formatting import as_html
 from marimo._output.hypertext import Html
```

### Comparing `marimo-0.6.3/marimo/_ast/app.py` & `marimo-0.6.4/marimo/_ast/app.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_ast/cell.py` & `marimo-0.6.4/marimo/_ast/cell.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_ast/codegen.py` & `marimo-0.6.4/marimo/_ast/codegen.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_ast/compiler.py` & `marimo-0.6.4/marimo/_ast/compiler.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_ast/visitor.py` & `marimo-0.6.4/marimo/_ast/visitor.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/cli.py` & `marimo-0.6.4/marimo/_cli/cli.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/convert/commands.py` & `marimo-0.6.4/marimo/_cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/convert/ipynb.py` & `marimo-0.6.4/marimo/_cli/convert/ipynb.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/convert/markdown.py` & `marimo-0.6.4/marimo/_cli/convert/markdown.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/convert/utils.py` & `marimo-0.6.4/marimo/_cli/convert/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/envinfo.py` & `marimo-0.6.4/marimo/_cli/envinfo.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/export/commands.py` & `marimo-0.6.4/marimo/_cli/export/commands.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/file_path.py` & `marimo-0.6.4/marimo/_cli/file_path.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/parse_args.py` & `marimo-0.6.4/marimo/_cli/parse_args.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_cli/upgrade.py` & `marimo-0.6.4/marimo/_cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_config/config.py` & `marimo-0.6.4/marimo/_config/config.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_config/manager.py` & `marimo-0.6.4/marimo/_config/manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_config/utils.py` & `marimo-0.6.4/marimo/_config/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_dependencies/dependencies.py` & `marimo-0.6.4/marimo/_dependencies/dependencies.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_islands/island_generator.py` & `marimo-0.6.4/marimo/_islands/island_generator.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_loggers.py` & `marimo-0.6.4/marimo/_loggers.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/agent.js` & `marimo-0.6.4/marimo/_lsp/copilot/dist/agent.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/arm64/kerberos.node` & `marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/arm64/kerberos.node`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/darwin/x64/kerberos.node` & `marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/darwin/x64/kerberos.node`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/arm64/kerberos.node` & `marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/arm64/kerberos.node`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/linux/x64/kerberos.node` & `marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/linux/x64/kerberos.node`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/compiled/win32/x64/kerberos.node` & `marimo-0.6.4/marimo/_lsp/copilot/dist/compiled/win32/x64/kerberos.node`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/crypt32.node` & `marimo-0.6.4/marimo/_lsp/copilot/dist/crypt32.node`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/resources/cl100k/tokenizer_cushman002.json` & `marimo-0.6.4/marimo/_lsp/copilot/dist/resources/cl100k/tokenizer_cushman002.json`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/resources/cl100k/vocab_cushman002.bpe` & `marimo-0.6.4/marimo/_lsp/copilot/dist/resources/cl100k/vocab_cushman002.bpe`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-go.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-go.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-javascript.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-javascript.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-python.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-python.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-ruby.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-ruby.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-tsx.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-tsx.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter-typescript.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter-typescript.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/copilot/dist/tree-sitter.wasm` & `marimo-0.6.4/marimo/_lsp/copilot/dist/tree-sitter.wasm`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_lsp/index.js` & `marimo-0.6.4/marimo/_lsp/index.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/cell_output.py` & `marimo-0.6.4/marimo/_messaging/cell_output.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/console_output_worker.py` & `marimo-0.6.4/marimo/_messaging/console_output_worker.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/errors.py` & `marimo-0.6.4/marimo/_messaging/errors.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/ops.py` & `marimo-0.6.4/marimo/_messaging/ops.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/streams.py` & `marimo-0.6.4/marimo/_messaging/streams.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/tracebacks.py` & `marimo-0.6.4/marimo/_messaging/tracebacks.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_messaging/types.py` & `marimo-0.6.4/marimo/_messaging/types.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/builder.py` & `marimo-0.6.4/marimo/_output/builder.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/data/data.py` & `marimo-0.6.4/marimo/_output/data/data.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/doc.py` & `marimo-0.6.4/marimo/_output/doc.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/altair_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/altair_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/anywidget_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/anywidget_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/bokeh_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/bokeh_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/cell.py` & `marimo-0.6.4/marimo/_output/formatters/cell.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/formatter_factory.py` & `marimo-0.6.4/marimo/_output/formatters/formatter_factory.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/formatters.py` & `marimo-0.6.4/marimo/_output/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/holoviews_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/holoviews_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/ipython_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/ipython_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/leafmap_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/leafmap_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/matplotlib_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/matplotlib_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/pandas_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/pandas_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/plotly_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/plotly_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/seaborn_formatters.py` & `marimo-0.6.4/marimo/_output/formatters/seaborn_formatters.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/structures.py` & `marimo-0.6.4/marimo/_output/formatters/structures.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatters/utils.py` & `marimo-0.6.4/marimo/_output/formatters/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/formatting.py` & `marimo-0.6.4/marimo/_output/formatting.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/hypertext.py` & `marimo-0.6.4/marimo/_output/hypertext.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/justify.py` & `marimo-0.6.4/marimo/_output/justify.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/md.py` & `marimo-0.6.4/marimo/_output/md.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/md_extensions/external_links.py` & `marimo-0.6.4/marimo/_output/md_extensions/external_links.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/mime.py` & `marimo-0.6.4/marimo/_output/mime.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/mpl.py` & `marimo-0.6.4/marimo/_output/mpl.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/rich_help.py` & `marimo-0.6.4/marimo/_output/rich_help.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_output/utils.py` & `marimo-0.6.4/marimo/_output/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/core/json_encoder.py` & `marimo-0.6.4/marimo/_plugins/core/json_encoder.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/core/media.py` & `marimo-0.6.4/marimo/_plugins/core/media.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/core/web_component.py` & `marimo-0.6.4/marimo/_plugins/core/web_component.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/accordion.py` & `marimo-0.6.4/marimo/_plugins/stateless/accordion.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/audio.py` & `marimo-0.6.4/marimo/_plugins/stateless/audio.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/callout.py` & `marimo-0.6.4/marimo/_plugins/stateless/callout.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/carousel.py` & `marimo-0.6.4/marimo/_plugins/stateless/carousel.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/download.py` & `marimo-0.6.4/marimo/_plugins/stateless/download.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/flex.py` & `marimo-0.6.4/marimo/_plugins/stateless/flex.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/icon.py` & `marimo-0.6.4/marimo/_plugins/stateless/icon.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/image.py` & `marimo-0.6.4/marimo/_plugins/stateless/image.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/json_output.py` & `marimo-0.6.4/marimo/_plugins/stateless/json_output.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/lazy.py` & `marimo-0.6.4/marimo/_plugins/stateless/lazy.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/mermaid.py` & `marimo-0.6.4/marimo/_plugins/stateless/mermaid.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/mpl/_mpl.py` & `marimo-0.6.4/marimo/_plugins/stateless/mpl/_mpl.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/nav_menu.py` & `marimo-0.6.4/marimo/_plugins/stateless/nav_menu.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/pdf.py` & `marimo-0.6.4/marimo/_plugins/stateless/pdf.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/plain_text.py` & `marimo-0.6.4/marimo/_plugins/stateless/plain_text.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/routes.py` & `marimo-0.6.4/marimo/_plugins/stateless/routes.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/sidebar.py` & `marimo-0.6.4/marimo/_plugins/stateless/sidebar.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/stat.py` & `marimo-0.6.4/marimo/_plugins/stateless/stat.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/status/_progress.py` & `marimo-0.6.4/marimo/_plugins/stateless/status/_progress.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/style.py` & `marimo-0.6.4/marimo/_plugins/stateless/style.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/tabs.py` & `marimo-0.6.4/marimo/_plugins/stateless/tabs.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/tree.py` & `marimo-0.6.4/marimo/_plugins/stateless/tree.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/stateless/video.py` & `marimo-0.6.4/marimo/_plugins/stateless/video.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/__init__.py` & `marimo-0.6.4/marimo/_plugins/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_core/ids.py` & `marimo-0.6.4/marimo/_plugins/ui/_core/ids.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_core/registry.py` & `marimo-0.6.4/marimo/_plugins/ui/_core/registry.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_core/ui_element.py` & `marimo-0.6.4/marimo/_plugins/ui/_core/ui_element.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/altair_chart.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/altair_chart.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/array.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/array.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/batch.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/batch.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/charts/altair_transformer.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/charts/altair_transformer.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/data_explorer.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/data_explorer.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/dataframe.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/dataframe.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/handlers.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/handlers.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/dataframes/transforms.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/dataframes/transforms.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/dictionary.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/dictionary.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/from_anywidget.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/from_anywidget.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/input.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/input.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/microphone.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/microphone.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/plotly.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/plotly.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/refresh.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/refresh.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/switch.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/switch.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/table.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/table.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tables/default_table.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tables/default_table.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tables/pandas_table.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tables/pandas_table.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tables/polars_table.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tables/polars_table.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tables/pyarrow_table.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tables/pyarrow_table.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tables/table_manager.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tables/table_manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tables/utils.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tables/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/tabs.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/tabs.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_plugins/ui/_impl/utils/dataframe.py` & `marimo-0.6.4/marimo/_plugins/ui/_impl/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_pyodide/bootstrap.py` & `marimo-0.6.4/marimo/_pyodide/bootstrap.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_pyodide/pyodide_session.py` & `marimo-0.6.4/marimo/_pyodide/pyodide_session.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_pyodide/streams.py` & `marimo-0.6.4/marimo/_pyodide/streams.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/capture.py` & `marimo-0.6.4/marimo/_runtime/capture.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/cell_lifecycle_item.py` & `marimo-0.6.4/marimo/_runtime/cell_lifecycle_item.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/cell_lifecycle_registry.py` & `marimo-0.6.4/marimo/_runtime/cell_lifecycle_registry.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/complete.py` & `marimo-0.6.4/marimo/_runtime/complete.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/context/kernel_context.py` & `marimo-0.6.4/marimo/_runtime/context/kernel_context.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/context/script_context.py` & `marimo-0.6.4/marimo/_runtime/context/script_context.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/context/types.py` & `marimo-0.6.4/marimo/_runtime/context/types.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/context/utils.py` & `marimo-0.6.4/marimo/_runtime/context/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/control_flow.py` & `marimo-0.6.4/marimo/_runtime/control_flow.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/dataflow.py` & `marimo-0.6.4/marimo/_runtime/dataflow.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/functions.py` & `marimo-0.6.4/marimo/_runtime/functions.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/handlers.py` & `marimo-0.6.4/marimo/_runtime/handlers.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/layout/layout.py` & `marimo-0.6.4/marimo/_runtime/layout/layout.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/marimo_pdb.py` & `marimo-0.6.4/marimo/_runtime/marimo_pdb.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/output/_output.py` & `marimo-0.6.4/marimo/_runtime/output/_output.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/conda_package_manager.py` & `marimo-0.6.4/marimo/_runtime/packages/conda_package_manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/module_name_to_pypi_name.py` & `marimo-0.6.4/marimo/_runtime/packages/module_name_to_pypi_name.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/module_registry.py` & `marimo-0.6.4/marimo/_runtime/packages/module_registry.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/package_manager.py` & `marimo-0.6.4/marimo/_runtime/packages/package_manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/package_managers.py` & `marimo-0.6.4/marimo/_runtime/packages/package_managers.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/pypi_package_manager.py` & `marimo-0.6.4/marimo/_runtime/packages/pypi_package_manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/packages/utils.py` & `marimo-0.6.4/marimo/_runtime/packages/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/params.py` & `marimo-0.6.4/marimo/_runtime/params.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/patches.py` & `marimo-0.6.4/marimo/_runtime/patches.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/redirect_streams.py` & `marimo-0.6.4/marimo/_runtime/redirect_streams.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/reload/autoreload.py` & `marimo-0.6.4/marimo/_runtime/reload/autoreload.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/reload/module_watcher.py` & `marimo-0.6.4/marimo/_runtime/reload/module_watcher.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/requests.py` & `marimo-0.6.4/marimo/_runtime/requests.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runner/cell_runner.py` & `marimo-0.6.4/marimo/_runtime/runner/cell_runner.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runner/hooks.py` & `marimo-0.6.4/marimo/_runtime/runner/hooks.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runner/hooks_on_finish.py` & `marimo-0.6.4/marimo/_runtime/runner/hooks_on_finish.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runner/hooks_post_execution.py` & `marimo-0.6.4/marimo/_runtime/runner/hooks_post_execution.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runner/hooks_pre_execution.py` & `marimo-0.6.4/marimo/_runtime/runner/hooks_pre_execution.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runner/hooks_preparation.py` & `marimo-0.6.4/marimo/_runtime/runner/hooks_preparation.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/runtime.py` & `marimo-0.6.4/marimo/_runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/state.py` & `marimo-0.6.4/marimo/_runtime/state.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/utils/set_ui_element_request_manager.py` & `marimo-0.6.4/marimo/_runtime/utils/set_ui_element_request_manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/validate_graph.py` & `marimo-0.6.4/marimo/_runtime/validate_graph.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/virtual_file.py` & `marimo-0.6.4/marimo/_runtime/virtual_file.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_runtime/win32_interrupt_handler.py` & `marimo-0.6.4/marimo/_runtime/win32_interrupt_handler.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/auth.py` & `marimo-0.6.4/marimo/_server/api/auth.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/deps.py` & `marimo-0.6.4/marimo/_server/api/deps.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/ai.py` & `marimo-0.6.4/marimo/_server/api/endpoints/ai.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/assets.py` & `marimo-0.6.4/marimo/_server/api/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/config.py` & `marimo-0.6.4/marimo/_server/api/endpoints/config.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/documentation.py` & `marimo-0.6.4/marimo/_server/api/endpoints/documentation.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/editing.py` & `marimo-0.6.4/marimo/_server/api/endpoints/editing.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/execution.py` & `marimo-0.6.4/marimo/_server/api/endpoints/execution.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/export.py` & `marimo-0.6.4/marimo/_server/api/endpoints/export.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/file_explorer.py` & `marimo-0.6.4/marimo/_server/api/endpoints/file_explorer.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/files.py` & `marimo-0.6.4/marimo/_server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/health.py` & `marimo-0.6.4/marimo/_server/api/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/home.py` & `marimo-0.6.4/marimo/_server/api/endpoints/home.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/login.py` & `marimo-0.6.4/marimo/_server/api/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/endpoints/ws.py` & `marimo-0.6.4/marimo/_server/api/endpoints/ws.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/interrupt.py` & `marimo-0.6.4/marimo/_server/api/interrupt.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/lifespans.py` & `marimo-0.6.4/marimo/_server/api/lifespans.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/middleware.py` & `marimo-0.6.4/marimo/_server/api/middleware.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/router.py` & `marimo-0.6.4/marimo/_server/api/router.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/status.py` & `marimo-0.6.4/marimo/_server/api/status.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/api/utils.py` & `marimo-0.6.4/marimo/_server/api/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/asgi.py` & `marimo-0.6.4/marimo/_server/asgi.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/export/__init__.py` & `marimo-0.6.4/marimo/_server/export/__init__.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/export/exporter.py` & `marimo-0.6.4/marimo/_server/export/exporter.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/export/utils.py` & `marimo-0.6.4/marimo/_server/export/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/file_manager.py` & `marimo-0.6.4/marimo/_server/file_manager.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/file_router.py` & `marimo-0.6.4/marimo/_server/file_router.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/files/file_system.py` & `marimo-0.6.4/marimo/_server/files/file_system.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/files/os_file_system.py` & `marimo-0.6.4/marimo/_server/files/os_file_system.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/main.py` & `marimo-0.6.4/marimo/_server/main.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/model.py` & `marimo-0.6.4/marimo/_server/model.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/models/base.py` & `marimo-0.6.4/marimo/_server/models/base.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/models/files.py` & `marimo-0.6.4/marimo/_server/models/files.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/models/home.py` & `marimo-0.6.4/marimo/_server/models/home.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/models/models.py` & `marimo-0.6.4/marimo/_server/models/models.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/models/test_base.py` & `marimo-0.6.4/marimo/_server/models/test_base.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/print.py` & `marimo-0.6.4/marimo/_server/print.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/recents.py` & `marimo-0.6.4/marimo/_server/recents.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/router.py` & `marimo-0.6.4/marimo/_server/router.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/session/session_view.py` & `marimo-0.6.4/marimo/_server/session/session_view.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/sessions.py` & `marimo-0.6.4/marimo/_server/sessions.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/start.py` & `marimo-0.6.4/marimo/_server/start.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/templates/templates.py` & `marimo-0.6.4/marimo/_server/templates/templates.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/tokens.py` & `marimo-0.6.4/marimo/_server/tokens.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/utils.py` & `marimo-0.6.4/marimo/_server/utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_server/uvicorn_utils.py` & `marimo-0.6.4/marimo/_server/uvicorn_utils.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/admonitions.py` & `marimo-0.6.4/marimo/_smoke_tests/admonitions.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/altair_charts.py` & `marimo-0.6.4/marimo/_smoke_tests/altair_charts.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/ansi.py` & `marimo-0.6.4/marimo/_smoke_tests/ansi.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/anywidget_compat.py` & `marimo-0.6.4/marimo/_smoke_tests/anywidget_compat.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/arrays_and_dicts.py` & `marimo-0.6.4/marimo/_smoke_tests/arrays_and_dicts.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1064.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1064.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1072.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1072.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1140.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1140.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1161.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1161.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1165.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1165.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1271.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1271.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1273.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1273.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1279.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1279.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1291.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1291.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1311.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1311.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1319.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1319.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1351.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1351.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/1362.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/1362.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/846.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/846.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/852.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/852.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/924.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/924.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/altair_bug.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/altair_bug.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/bugs/key_with_period.py` & `marimo-0.6.4/marimo/_smoke_tests/bugs/key_with_period.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/carousel.py` & `marimo-0.6.4/marimo/_smoke_tests/carousel.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/charts/1mil_flights.py` & `marimo-0.6.4/marimo/_smoke_tests/charts/1mil_flights.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/code_editor.py` & `marimo-0.6.4/marimo/_smoke_tests/code_editor.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/custom_server/my_server.py` & `marimo-0.6.4/marimo/_smoke_tests/custom_server/my_server.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/data_explorer.py` & `marimo-0.6.4/marimo/_smoke_tests/data_explorer.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/dataframe.py` & `marimo-0.6.4/marimo/_smoke_tests/dataframe.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/debounce.py` & `marimo-0.6.4/marimo/_smoke_tests/debounce.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/forms.py` & `marimo-0.6.4/marimo/_smoke_tests/forms.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/full_width.py` & `marimo-0.6.4/marimo/_smoke_tests/full_width.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/grid.py` & `marimo-0.6.4/marimo/_smoke_tests/grid.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/icons.py` & `marimo-0.6.4/marimo/_smoke_tests/icons.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/import_named_cells.py` & `marimo-0.6.4/marimo/_smoke_tests/import_named_cells.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/inputs.py` & `marimo-0.6.4/marimo/_smoke_tests/inputs.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/iplot.py` & `marimo-0.6.4/marimo/_smoke_tests/iplot.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/latex.py` & `marimo-0.6.4/marimo/_smoke_tests/latex.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/layout.py` & `marimo-0.6.4/marimo/_smoke_tests/layout.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/lazy.py` & `marimo-0.6.4/marimo/_smoke_tests/lazy.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/lens_test.py` & `marimo-0.6.4/marimo/_smoke_tests/lens_test.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/md.py` & `marimo-0.6.4/marimo/_smoke_tests/md.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/media.py` & `marimo-0.6.4/marimo/_smoke_tests/media.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/named_cells.py` & `marimo-0.6.4/marimo/_smoke_tests/named_cells.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/nav_menus.py` & `marimo-0.6.4/marimo/_smoke_tests/nav_menus.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/output.py` & `marimo-0.6.4/marimo/_smoke_tests/output.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/pdf.py` & `marimo-0.6.4/marimo/_smoke_tests/pdf.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/query_params.py` & `marimo-0.6.4/marimo/_smoke_tests/query_params.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/refresh.py` & `marimo-0.6.4/marimo/_smoke_tests/refresh.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/routes.py` & `marimo-0.6.4/marimo/_smoke_tests/routes.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/scale.py` & `marimo-0.6.4/marimo/_smoke_tests/scale.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/sidebar.py` & `marimo-0.6.4/marimo/_smoke_tests/sidebar.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/state.py` & `marimo-0.6.4/marimo/_smoke_tests/state.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/stats.py` & `marimo-0.6.4/marimo/_smoke_tests/stats.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/status.py` & `marimo-0.6.4/marimo/_smoke_tests/status.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/stop.py` & `marimo-0.6.4/marimo/_smoke_tests/stop.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/third_party/altair_example.py` & `marimo-0.6.4/marimo/_smoke_tests/third_party/altair_example.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/third_party/holoviews_example.py` & `marimo-0.6.4/marimo/_smoke_tests/third_party/holoviews_example.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/third_party/ipython_display.py` & `marimo-0.6.4/marimo/_smoke_tests/third_party/ipython_display.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/third_party/plotly_example.py` & `marimo-0.6.4/marimo/_smoke_tests/third_party/plotly_example.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/third_party/seaborn_example.py` & `marimo-0.6.4/marimo/_smoke_tests/third_party/seaborn_example.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_smoke_tests/ws.py` & `marimo-0.6.4/marimo/_smoke_tests/ws.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-0.py` & `marimo-0.6.4/marimo/_snippets/data/altair-0.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-1.py` & `marimo-0.6.4/marimo/_snippets/data/altair-1.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-2.py` & `marimo-0.6.4/marimo/_snippets/data/altair-2.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-3.py` & `marimo-0.6.4/marimo/_snippets/data/altair-3.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-4.py` & `marimo-0.6.4/marimo/_snippets/data/altair-4.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-5.py` & `marimo-0.6.4/marimo/_snippets/data/altair-5.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-6.py` & `marimo-0.6.4/marimo/_snippets/data/altair-6.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-7.py` & `marimo-0.6.4/marimo/_snippets/data/altair-7.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/altair-8.py` & `marimo-0.6.4/marimo/_snippets/data/altair-8.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/cli-args-0.py` & `marimo-0.6.4/marimo/_snippets/data/cli-args-0.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-0.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-0.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-1.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-1.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-10.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-10.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-11.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-11.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-12.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-12.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-14.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-14.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-15.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-15.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-17.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-17.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-18.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-18.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-19.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-19.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-2.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-2.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-20.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-20.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-21.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-21.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-22.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-22.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-23.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-23.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-24.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-24.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-25.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-25.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-3.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-3.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-4.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-4.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-5.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-5.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-6.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-6.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-7.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-7.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-8.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-8.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/pandas-9.py` & `marimo-0.6.4/marimo/_snippets/data/pandas-9.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/query-params-0.py` & `marimo-0.6.4/marimo/_snippets/data/query-params-0.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/data/query-params-1.py` & `marimo-0.6.4/marimo/_snippets/data/query-params-1.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_snippets/snippets.py` & `marimo-0.6.4/marimo/_snippets/snippets.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/android-chrome-192x192.png` & `marimo-0.6.4/marimo/_static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/android-chrome-512x512.png` & `marimo-0.6.4/marimo/_static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/apple-touch-icon.png` & `marimo-0.6.4/marimo/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/CarouselComponent-C12Ecb2K.css` & `marimo-0.6.4/marimo/_static/assets/CarouselComponent-C12Ecb2K.css`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/CarouselComponent-DtCAwyzo.js` & `marimo-0.6.4/marimo/_static/assets/CarouselComponent-ml4W_PuP.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     r as e,
     R as t,
     V as s,
     j as i,
     e as r,
     B as a
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 
 function n(e) {
     return null !== e && "object" == typeof e && "constructor" in e && e.constructor === Object
 }
 
 function l(e, t) {
     void 0 === e && (e = {}), void 0 === t && (t = {}), Object.keys(t).forEach((s => {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/ConnectedDataExplorerComponent-DKdMG7z6.js` & `marimo-0.6.4/marimo/_static/assets/ConnectedDataExplorerComponent-B6WI1UcR.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -30,27 +30,27 @@
     u as O,
     eD as k,
     ei as M,
     T as I,
     X as U,
     R as F,
     g9 as D
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     i as j,
     c as _,
     N as P,
     V as R
-} from "./VegaLite-BQwzJofD.js";
-import "./time-CUBsQdfc.js";
+} from "./VegaLite-rQgmZ7vL.js";
+import "./time-CLRyKR-T.js";
 import "./timer-D8GWrtRJ.js";
-import "./linear-DF6Se9n2.js";
+import "./linear-JxYcrfvc.js";
 import "./init-DLRA0X12.js";
 import "./range-CtcPcB_L.js";
-import "./index-ChUg6Fde.js";
+import "./index-AJ6VyMaJ.js";
 import "./ordinal-DDUp3AbE.js";
 import "./arc-DIImc9ZO.js";
 import "./path-qnb_ma6O.js";
 import "./step-BEJ6WznM.js";
 import "./array-DmjLdZ15.js";
 import "./line-Dz7yhIWK.js";
 /**
```

### Comparing `marimo-0.6.3/marimo/_static/assets/FiraMono-Bold-CLVRCuM9.ttf` & `marimo-0.6.4/marimo/_static/assets/FiraMono-Bold-CLVRCuM9.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/FiraMono-Medium-DU3aDxX5.ttf` & `marimo-0.6.4/marimo/_static/assets/FiraMono-Medium-DU3aDxX5.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/FiraMono-Regular-BTCkDNvf.ttf` & `marimo-0.6.4/marimo/_static/assets/FiraMono-Regular-BTCkDNvf.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_AMS-Regular-BQhdFMY1.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_AMS-Regular-BQhdFMY1.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_AMS-Regular-DMm9YOAa.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_AMS-Regular-DMm9YOAa.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_AMS-Regular-DRggAlZN.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_AMS-Regular-DRggAlZN.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Bold-ATXxdsX0.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Bold-ATXxdsX0.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Bold-BEiXGLvX.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Bold-BEiXGLvX.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Bold-Dq_IR9rO.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Bold-Dq_IR9rO.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Regular-CTRA-rTL.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Regular-CTRA-rTL.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Regular-Di6jR-x-.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Regular-Di6jR-x-.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Caligraphic-Regular-wX97UBjC.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Caligraphic-Regular-wX97UBjC.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Bold-BdnERNNW.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Bold-BdnERNNW.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Bold-BsDP51OF.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Bold-BsDP51OF.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Bold-CL6g_b3V.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Bold-CL6g_b3V.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Regular-CB_wures.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Regular-CB_wures.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Regular-CTYiF6lA.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Regular-CTYiF6lA.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Fraktur-Regular-Dxdc4cR9.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Fraktur-Regular-Dxdc4cR9.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Bold-Cx986IdX.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Bold-Cx986IdX.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Bold-Jm3AIy58.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Bold-Jm3AIy58.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Bold-waoOVXN0.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Bold-waoOVXN0.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-BoldItalic-DxDJ3AOS.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-BoldItalic-DxDJ3AOS.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-BoldItalic-DzxPMmG6.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-BoldItalic-DzxPMmG6.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-BoldItalic-SpSLRI95.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-BoldItalic-SpSLRI95.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Italic-3WenGoN9.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Italic-3WenGoN9.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Italic-BMLOBm91.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Italic-BMLOBm91.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Italic-NWA7e6Wa.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Italic-NWA7e6Wa.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Regular-B22Nviop.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Regular-B22Nviop.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Regular-Dr94JaBh.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Regular-Dr94JaBh.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Main-Regular-ypZvNtVU.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Main-Regular-ypZvNtVU.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Math-BoldItalic-B3XSjfu4.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Math-BoldItalic-B3XSjfu4.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Math-BoldItalic-CZnvNsCZ.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Math-BoldItalic-CZnvNsCZ.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Math-BoldItalic-iY-2wyZ7.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Math-BoldItalic-iY-2wyZ7.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Math-Italic-DA0__PXp.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Math-Italic-DA0__PXp.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Math-Italic-flOr_0UB.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Math-Italic-flOr_0UB.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Math-Italic-t53AETM-.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Math-Italic-t53AETM-.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Bold-CFMepnvq.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Bold-CFMepnvq.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Bold-D1sUS0GD.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Bold-D1sUS0GD.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Bold-DbIhKOiC.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Bold-DbIhKOiC.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Italic-C3H0VqGB.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Italic-C3H0VqGB.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Italic-DN2j7dab.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Italic-DN2j7dab.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Italic-YYjJ1zSn.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Italic-YYjJ1zSn.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Regular-BNo7hRIc.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Regular-BNo7hRIc.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Regular-CS6fqUqJ.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Regular-CS6fqUqJ.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_SansSerif-Regular-DDBCnlJ7.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_SansSerif-Regular-DDBCnlJ7.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Script-Regular-C5JkGWo-.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Script-Regular-C5JkGWo-.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Script-Regular-D3wIWfF6.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Script-Regular-D3wIWfF6.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Script-Regular-D5yQViql.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Script-Regular-D5yQViql.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size1-Regular-C195tn64.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size1-Regular-C195tn64.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size1-Regular-Dbsnue_I.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size1-Regular-Dbsnue_I.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size1-Regular-mCD8mA8B.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size1-Regular-mCD8mA8B.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size2-Regular-B7gKUWhC.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size2-Regular-B7gKUWhC.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size2-Regular-Dy4dx90m.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size2-Regular-Dy4dx90m.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size2-Regular-oD1tc_U0.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size2-Regular-oD1tc_U0.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size3-Regular-CTq5MqoE.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size3-Regular-CTq5MqoE.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size3-Regular-DgpXs0kz.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size3-Regular-DgpXs0kz.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size4-Regular-BF-4gkZK.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size4-Regular-BF-4gkZK.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size4-Regular-DWFBv043.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size4-Regular-DWFBv043.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Size4-Regular-Dl5lxZxV.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Size4-Regular-Dl5lxZxV.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Typewriter-Regular-C0xS9mPB.woff` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Typewriter-Regular-C0xS9mPB.woff`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Typewriter-Regular-CO6r4hn1.woff2` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Typewriter-Regular-CO6r4hn1.woff2`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/KaTeX_Typewriter-Regular-D3Ib7_Hf.ttf` & `marimo-0.6.4/marimo/_static/assets/KaTeX_Typewriter-Regular-D3Ib7_Hf.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/Lora-VariableFont_wght-B2ootaw-.ttf` & `marimo-0.6.4/marimo/_static/assets/Lora-VariableFont_wght-B2ootaw-.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/PTSans-Bold-D9fedIX3.ttf` & `marimo-0.6.4/marimo/_static/assets/PTSans-Bold-D9fedIX3.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/PTSans-Regular-CxL0S8W7.ttf` & `marimo-0.6.4/marimo/_static/assets/PTSans-Regular-CxL0S8W7.ttf`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/VegaLite-BQwzJofD.js` & `marimo-0.6.4/marimo/_static/assets/VegaLite-rQgmZ7vL.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -122,30 +122,30 @@
     i9 as dt,
     ia as ht,
     ib as pt,
     ic as mt,
     id as gt,
     R as yt,
     ie as vt
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     m as bt,
     a as xt,
     r as wt,
     d as _t,
     l as kt,
     i as Et,
     h as $t,
     n as At,
     c as Dt,
     u as St,
     b as Ft,
     t as Ct,
     e as Mt
-} from "./time-CUBsQdfc.js";
+} from "./time-CLRyKR-T.js";
 import {
     n as Ot,
     a as Nt,
     i as zt,
     b as Rt,
     d as Tt,
     c as Pt,
@@ -156,15 +156,15 @@
     t as qt,
     g as Ut,
     h as Wt,
     j as Ht,
     k as Gt,
     m as Vt,
     p as Xt
-} from "./linear-DF6Se9n2.js";
+} from "./linear-JxYcrfvc.js";
 import {
     r as Yt
 } from "./range-CtcPcB_L.js";
 import {
     R as Jt,
     r as Qt,
     a as Kt,
@@ -189,15 +189,15 @@
     t as vn,
     u as bn,
     d as xn
 } from "./timer-D8GWrtRJ.js";
 import {
     i as wn,
     e as _n
-} from "./index-ChUg6Fde.js";
+} from "./index-AJ6VyMaJ.js";
 import {
     i as kn,
     a as En
 } from "./init-DLRA0X12.js";
 import {
     I as $n,
     o as An,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/_baseEach-BrSWFoJM.js` & `marimo-0.6.4/marimo/_static/assets/_baseEach-FAhoh2N5.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -11,19 +11,19 @@
     jq as s,
     jr as l,
     iH as c,
     js as v,
     jt as j,
     jj as d,
     ik as g
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     e as h,
     d as b
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 var p = n ? n.isConcatSpreadable : void 0;
 
 function m(n) {
     return r(n) || t(n) || !!(p && n && n[p])
 }
 
 function O(n, r, t, e, a) {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/any-language-editor-D3MTmtyo.js` & `marimo-0.6.4/marimo/_static/assets/any-language-editor-Dzf9Jczi.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -35,56 +35,56 @@
     j9 as U,
     ja as Z,
     Y as v,
     r as _,
     j as g,
     eD as W,
     dS as F
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     less as H
-} from "./index-DzhIfGoT.js";
+} from "./index-1IpQZ_Yu.js";
 import {
     sass as z
-} from "./index-DgcwnKY7.js";
+} from "./index-DahJleVt.js";
 import {
     json as V
-} from "./index-S9qVQ2oC.js";
+} from "./index-DqGPWGPa.js";
 import {
     xml as E
-} from "./index-CohQOVlj.js";
+} from "./index-KIzq3vhX.js";
 import {
     sql as D,
     MySQL as N,
     PostgreSQL as J
-} from "./index-ClCDnvOE.js";
+} from "./index-yuQsQmno.js";
 import {
     java as C
-} from "./index-C2GbrbZr.js";
+} from "./index-DCESMHe2.js";
 import {
     rust as B
-} from "./index-BuR6fZZm.js";
+} from "./index-CE06HdF7.js";
 import {
     cpp as K
-} from "./index-7VEF_U3p.js";
+} from "./index-DgOauLen.js";
 import {
     php as L
-} from "./index-Ck0jzFpb.js";
+} from "./index-CB4e2-IR.js";
 import {
     liquid as I
-} from "./index-0fF0Xoai.js";
+} from "./index-BYVYp6Ei.js";
 import {
     wast as A
-} from "./index-jW3n8_hn.js";
+} from "./index-BH1DvUFb.js";
 import {
     vue as M
-} from "./index-CzWuvzvc.js";
+} from "./index-DtyNPFfa.js";
 import {
     angular as OO
-} from "./index-D4als0Dc.js";
+} from "./index-XFgu4285.js";
 import {
     apl as $O
 } from "./apl-CXdQSnD-.js";
 import {
     asciiArmor as iO
 } from "./asciiarmor-D5V0T9Cu.js";
 import {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/apl-CXdQSnD-.js` & `marimo-0.6.4/marimo/_static/assets/apl-CXdQSnD-.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/arc-DIImc9ZO.js` & `marimo-0.6.4/marimo/_static/assets/arc-DIImc9ZO.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/asciiarmor-D5V0T9Cu.js` & `marimo-0.6.4/marimo/_static/assets/asciiarmor-D5V0T9Cu.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/asn1-BhA3SgW2.js` & `marimo-0.6.4/marimo/_static/assets/asn1-BhA3SgW2.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/asterisk-B46aRdXb.js` & `marimo-0.6.4/marimo/_static/assets/asterisk-B46aRdXb.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/blockDiagram-91b80b7a-DPH13Qrf.js` & `marimo-0.6.4/marimo/_static/assets/blockDiagram-91b80b7a-DSsN5jAx.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,48 +2,48 @@
     c as e,
     _ as t,
     h as i,
     l as s,
     y as n,
     K as r,
     n as o
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     c as l
-} from "./clone-BL0WSZ3Z.js";
+} from "./clone-CrCyWe3U.js";
 import {
     i as a,
     c,
     b as h,
     d as u,
     a as d,
     p as g
-} from "./edges-d32062c0-CFY3bIwa.js";
+} from "./edges-d32062c0-CU6OCHwI.js";
 import {
     G as y
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     s as p
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     o as b
 } from "./ordinal-DDUp3AbE.js";
 import {
     c as x
-} from "./channel-DCiFYtzP.js";
+} from "./channel-BmGrl1HB.js";
 import {
     s as f
 } from "./Tableau10-B3EzvwxR.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
-import "./createText-6b48ae7d-129t9twG.js";
+import "./createText-6b48ae7d-BgOE7dMp.js";
 import "./line-Dz7yhIWK.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
-import "./_baseEach-BrSWFoJM.js";
+import "./_baseEach-FAhoh2N5.js";
 import "./timer-D8GWrtRJ.js";
 import "./init-DLRA0X12.js";
 var m, L, S = function() {
     var e = function(e, t, i, s) {
             for (i = i || {}, s = e.length; s--; i[e[s]] = t);
             return i
         },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/brainfuck-CtZaYBKt.js` & `marimo-0.6.4/marimo/_static/assets/brainfuck-CtZaYBKt.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/c4Diagram-b2a90758-CAH0Datt.js` & `marimo-0.6.4/marimo/_static/assets/c4Diagram-b2a90758-f1UFjA-x.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9,23 +9,23 @@
     f as l,
     l as o,
     h,
     w as d,
     i as u,
     j as p,
     k as y
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as f
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     d as b,
     g
-} from "./svgDrawCommon-5ccd53ef-BK5P1sG2.js";
-import "./index-Dq6tg2Hn.js";
+} from "./svgDrawCommon-5ccd53ef-DsDJYju_.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 var _ = function() {
     var t = function(t, e, n, a) {
             for (n = n || {}, a = t.length; a--; n[t[a]] = e);
             return n
         },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/classDiagram-30eddba6-Bz0cJX-U.js` & `marimo-0.6.4/marimo/_static/assets/classDiagram-30eddba6-BabWtcIB.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
 import {
     p as t,
     d as e,
     s as a
-} from "./styles-991ebdfc-CV9pCNxb.js";
+} from "./styles-991ebdfc-vxk4XA-a.js";
 import {
     s as r
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     G as i
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     l as n
-} from "./layout-DDD1odkP.js";
+} from "./layout-BdT9zkSH.js";
 import {
     c as d,
     l as o,
     h as s,
     x as p,
     Q as l
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     l as c
 } from "./line-Dz7yhIWK.js";
 import {
     a as g
 } from "./step-BEJ6WznM.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./timer-D8GWrtRJ.js";
-import "./_baseEach-BrSWFoJM.js";
-import "./sortBy-D0xI_7yL.js";
+import "./_baseEach-FAhoh2N5.js";
+import "./sortBy-DwX0cqqB.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 let h = 0;
 const f = function(t) {
         let e = t.id;
         return t.type && (e += "<" + l(t.type) + ">"), e
     },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/classDiagram-v2-f2df5561-BxNEwu6g.js` & `marimo-0.6.4/marimo/_static/assets/classDiagram-v2-f2df5561-D5SEk3xC.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,44 +1,44 @@
 import {
     p as e,
     d as t,
     s as l
-} from "./styles-991ebdfc-CV9pCNxb.js";
+} from "./styles-991ebdfc-vxk4XA-a.js";
 import {
     s as o
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     G as a
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     l as s,
     c as i,
     x as n,
     q as r,
     n as d,
     p as c,
     i as p
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     r as b
-} from "./index-fc10efb0-C3SRzTfT.js";
-import "./layout-DDD1odkP.js";
+} from "./index-fc10efb0-CJWvKICv.js";
+import "./layout-BdT9zkSH.js";
 import {
     c as f
 } from "./step-BEJ6WznM.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./timer-D8GWrtRJ.js";
-import "./_baseEach-BrSWFoJM.js";
-import "./clone-BL0WSZ3Z.js";
-import "./edges-d32062c0-CFY3bIwa.js";
-import "./createText-6b48ae7d-129t9twG.js";
+import "./_baseEach-FAhoh2N5.js";
+import "./clone-CrCyWe3U.js";
+import "./edges-d32062c0-CU6OCHwI.js";
+import "./createText-6b48ae7d-BgOE7dMp.js";
 import "./line-Dz7yhIWK.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
-import "./sortBy-D0xI_7yL.js";
+import "./sortBy-DwX0cqqB.js";
 const y = e => p.sanitizeText(e, i());
 let g = {
     dividerMargin: 10,
     padding: 5,
     textHeight: 10,
     curve: void 0
 };
```

### Comparing `marimo-0.6.3/marimo/_static/assets/clike-BPCXT8V3.js` & `marimo-0.6.4/marimo/_static/assets/clike-BPCXT8V3.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/clojure-DR_hEDJv.js` & `marimo-0.6.4/marimo/_static/assets/clojure-DR_hEDJv.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/cmake-DXn5xaP-.js` & `marimo-0.6.4/marimo/_static/assets/cmake-DXn5xaP-.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/cobol-DJhTY0fG.js` & `marimo-0.6.4/marimo/_static/assets/cobol-DJhTY0fG.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/coffeescript-BTDxI-eT.js` & `marimo-0.6.4/marimo/_static/assets/coffeescript-BTDxI-eT.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/commonlisp-D09g7coK.js` & `marimo-0.6.4/marimo/_static/assets/commonlisp-D09g7coK.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/createText-6b48ae7d-129t9twG.js` & `marimo-0.6.4/marimo/_static/assets/createText-6b48ae7d-BgOE7dMp.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     l as e,
     N as n,
     O as t
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 const r = {};
 
 function i(e, n, t) {
     if (function(e) {
             return Boolean(e && "object" == typeof e)
         }(e)) {
         if ("value" in e) return "html" !== e.type || t ? e.value : "";
```

### Comparing `marimo-0.6.3/marimo/_static/assets/crystal-CRzZ78HM.js` & `marimo-0.6.4/marimo/_static/assets/crystal-CRzZ78HM.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/css-ZjFoif2m.js` & `marimo-0.6.4/marimo/_static/assets/css-ZjFoif2m.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/cypher-gJDei3ni.js` & `marimo-0.6.4/marimo/_static/assets/cypher-gJDei3ni.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/d-BShv7fp-.js` & `marimo-0.6.4/marimo/_static/assets/d-BShv7fp-.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/dockerfile-BLgfkd__.js` & `marimo-0.6.4/marimo/_static/assets/dockerfile-BLgfkd__.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/dtd-DI9Herc-.js` & `marimo-0.6.4/marimo/_static/assets/dtd-DI9Herc-.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/dylan-CHJ5qNM_.js` & `marimo-0.6.4/marimo/_static/assets/dylan-CHJ5qNM_.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ebnf-B-Df8AvO.js` & `marimo-0.6.4/marimo/_static/assets/ebnf-B-Df8AvO.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ecl-DPFc0Uaf.js` & `marimo-0.6.4/marimo/_static/assets/ecl-DPFc0Uaf.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/edges-d32062c0-CFY3bIwa.js` & `marimo-0.6.4/marimo/_static/assets/edges-d32062c0-CU6OCHwI.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     o as t,
     c as e,
     d as a,
     N as r,
     l as n,
     x as i
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     c as l
-} from "./createText-6b48ae7d-129t9twG.js";
+} from "./createText-6b48ae7d-BgOE7dMp.js";
 import {
     l as o
 } from "./line-Dz7yhIWK.js";
 import {
     a as d
 } from "./step-BEJ6WznM.js";
 const h = {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/edit-page-CIzFhPq5.js` & `marimo-0.6.4/marimo/_static/assets/edit-page-DnXnHWMg.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -364,15 +364,15 @@
     eS as Pi,
     eT as Ai,
     eU as _i,
     eV as Ri,
     eW as zi,
     eX as Li,
     eY as Bi
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     K as Fi,
     B as Hi,
     M as Vi,
     b as $i,
     C as Wi,
     a as Ui,
@@ -385,15 +385,15 @@
     h as Ji,
     L as Qi,
     k as ea,
     u as ta,
     P as na,
     S as ra,
     j as oa
-} from "./icons-6JftBaIY.js";
+} from "./icons-DtRVr9-T.js";
 import {
     b as ia,
     c as aa,
     v as sa,
     N as la,
     V as ca,
     d as da,
@@ -412,32 +412,32 @@
     u as Ea,
     n as Sa,
     A as Ca,
     a as Na,
     C as ja,
     T as Ia,
     o as Oa
-} from "./useMarimoWebSocket-DFV8TeGX.js";
+} from "./useMarimoWebSocket-Butgv0ej.js";
 import {
     s as Ma,
     i as Da,
     T as Ta,
     a as Pa
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     d as Aa
 } from "./timer-D8GWrtRJ.js";
 import {
     i as _a,
     e as Ra
-} from "./index-ChUg6Fde.js";
+} from "./index-AJ6VyMaJ.js";
 import {
     s as za
-} from "./sortBy-D0xI_7yL.js";
-import "./_baseEach-BrSWFoJM.js";
+} from "./sortBy-DwX0cqqB.js";
+import "./_baseEach-FAhoh2N5.js";
 /**
  * @license lucide-react v0.378.0 - ISC
  *
  * This source code is licensed under the ISC license.
  * See the LICENSE file in the root directory of this source tree.
  */
 const La = n("ArrowLeft", [
@@ -4926,17 +4926,15 @@
     ld = kt.define(),
     cd = Et.define({
         create: () => St.none,
         update(e, t) {
             let n = e.map(t.changes);
             for (const r of t.effects) r.is(sd) ? n = e.update({
                 add: [ad.range(r.value.from, r.value.to)]
-            }) : r.is(ld) && (n = e.update({
-                filter: (e, t) => e !== r.value.from || t !== r.value.to
-            }));
+            }) : r.is(ld) && (n = St.none);
             return n
         },
         provide: e => wt.decorations.from(e)
     });
 class dd {
     constructor(e, n) {
         t(this, "view"), t(this, "commandKey"), t(this, "hoveredRange"), t(this, "onClick"), t(this, "mousemove", (e => {
@@ -4958,38 +4956,38 @@
                     to: r,
                     position: t
                 }, this.view.dispatch({
                     effects: sd.of(this.hoveredRange)
                 })
             } else this.clearUnderline()
         })), t(this, "keydown", (e => {
-            "Meta" === e.key && (this.commandKey = !0)
+            "Meta" !== e.key && "Ctrl" !== e.key || (this.commandKey = !0)
         })), t(this, "click", (e => {
             if (this.hoveredRange) {
                 const t = this.view.state.doc.sliceString(this.hoveredRange.from, this.hoveredRange.to);
                 e.preventDefault(), e.stopPropagation(), this.onClick(this.view, t), this.view.dispatch({
                     selection: {
                         head: this.hoveredRange.position,
                         anchor: this.hoveredRange.position
                     }
                 })
             }
         })), t(this, "keyup", (e => {
-            "Meta" === e.key && (this.commandKey = !1, this.clearUnderline())
+            "Meta" !== e.key && "Ctrl" !== e.key || (this.commandKey = !1, this.clearUnderline())
         })), this.view = e, this.commandKey = !1, this.hoveredRange = null, this.onClick = n, window.addEventListener("mousemove", this.mousemove), window.addEventListener("keydown", this.keydown), window.addEventListener("keyup", this.keyup), this.view.dom.addEventListener("click", this.click)
     }
     update(e) {
         (e.docChanged || e.viewportChanged) && this.clearUnderline()
     }
     destroy() {
         window.removeEventListener("mousemove", this.mousemove), window.removeEventListener("keydown", this.keydown), window.removeEventListener("keyup", this.keyup)
     }
     clearUnderline() {
         this.hoveredRange && (this.view.dispatch({
-            effects: ld.of(this.hoveredRange)
+            effects: ld.of(null)
         }), this.hoveredRange = null)
     }
 }
 const ud = (e, t) => [wt.lineWrapping, mn(), vn(), yn(), xn(), bn(), wn(), kn(), En({
             position: "fixed",
             parent: document.querySelector("#App") ?? void 0
         }), Bc(), "dark" === t ? Sn : [],
```

### Comparing `marimo-0.6.3/marimo/_static/assets/edit-page-CwGzkSpM.css` & `marimo-0.6.4/marimo/_static/assets/edit-page-CwGzkSpM.css`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/eiffel-BZ5y0wDL.js` & `marimo-0.6.4/marimo/_static/assets/eiffel-BZ5y0wDL.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/elm-D7xaZ7Da.js` & `marimo-0.6.4/marimo/_static/assets/elm-D7xaZ7Da.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/erDiagram-47591fe2-CJ2SMwAy.js` & `marimo-0.6.4/marimo/_static/assets/erDiagram-47591fe2-UyJH0JYd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,34 +7,34 @@
     u as n,
     v as s,
     l as o,
     y as c,
     x as l,
     h,
     Q as d
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     G as y
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     s as u
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     l as p
-} from "./layout-DDD1odkP.js";
+} from "./layout-BdT9zkSH.js";
 import {
     l as _
 } from "./line-Dz7yhIWK.js";
 import {
     a as f
 } from "./step-BEJ6WznM.js";
-import "./index-Dq6tg2Hn.js";
-import "./_baseEach-BrSWFoJM.js";
+import "./index-Cd3MtTMQ.js";
+import "./_baseEach-FAhoh2N5.js";
 import "./timer-D8GWrtRJ.js";
-import "./sortBy-D0xI_7yL.js";
+import "./sortBy-DwX0cqqB.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 const m = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
 const E = [];
 for (let F = 0; F < 256; ++F) E.push((F + 256).toString(16).slice(1));
 
 function g(t) {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/erlang-BuqgqA5h.js` & `marimo-0.6.4/marimo/_static/assets/erlang-BuqgqA5h.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/factor-Bm2WRyNM.js` & `marimo-0.6.4/marimo/_static/assets/factor-Bm2WRyNM.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/fcl-CVaBTCzQ.js` & `marimo-0.6.4/marimo/_static/assets/fcl-CVaBTCzQ.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/flowDb-4b19a42f-4mXsCvSf.js` & `marimo-0.6.4/marimo/_static/assets/flowDb-4b19a42f-Cf4l3Vi7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 import {
     s as t
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     c as e,
     t as s,
     s as u,
     g as i,
     a as n,
     b as r,
     u as a,
     v as c,
     l as o,
     x as l,
     y as h,
     i as A
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 var d = function() {
     var t = function(t, e, s, u) {
             for (s = s || {}, u = t.length; u--; s[t[u]] = e);
             return s
         },
         e = [1, 4],
         s = [1, 3],
```

### Comparing `marimo-0.6.3/marimo/_static/assets/flowDiagram-5540d9b9-msf8H4Jk.js` & `marimo-0.6.4/marimo/_static/assets/flowDiagram-5540d9b9-CuVcDbrT.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,62 +1,62 @@
 import {
     p as s,
     f as r
-} from "./flowDb-4b19a42f-4mXsCvSf.js";
+} from "./flowDb-4b19a42f-Cf4l3Vi7.js";
 import {
     h as a,
     f as t,
     G as o
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     s as e
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     n as m,
     o as i,
     c as p,
     r as f,
     i as c,
     l as n,
     p as j,
     q as l
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     u as b,
     r as d,
     p as h,
     l as u,
     d as w
-} from "./layout-DDD1odkP.js";
+} from "./layout-BdT9zkSH.js";
 import {
     a as x,
     b as g,
     i as y,
     c as k,
     e as A,
     d as E,
     f as G,
     g as v,
     s as B
-} from "./styles-3ed67cfa-QdZmR4us.js";
+} from "./styles-3ed67cfa-Cg_XeDUz.js";
 import {
     l as D
 } from "./line-Dz7yhIWK.js";
 import {
     c as M
 } from "./step-BEJ6WznM.js";
-import "./index-Dq6tg2Hn.js";
-import "./_baseEach-BrSWFoJM.js";
+import "./index-Cd3MtTMQ.js";
+import "./_baseEach-FAhoh2N5.js";
 import "./timer-D8GWrtRJ.js";
-import "./sortBy-D0xI_7yL.js";
-import "./index-fc10efb0-C3SRzTfT.js";
-import "./clone-BL0WSZ3Z.js";
-import "./edges-d32062c0-CFY3bIwa.js";
-import "./createText-6b48ae7d-129t9twG.js";
-import "./channel-DCiFYtzP.js";
+import "./sortBy-DwX0cqqB.js";
+import "./index-fc10efb0-CJWvKICv.js";
+import "./clone-CrCyWe3U.js";
+import "./edges-d32062c0-CU6OCHwI.js";
+import "./createText-6b48ae7d-BgOE7dMp.js";
+import "./channel-BmGrl1HB.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 
 function T(s) {
     if (!s.ok) throw new Error(s.status + " " + s.statusText);
     return s.text()
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/flowchart-elk-definition-5fe447d6-tgRhUdQk.js` & `marimo-0.6.4/marimo/_static/assets/flowchart-elk-definition-5fe447d6-BpUsl4Jm.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,42 @@
 import {
     d as n,
     p as t
-} from "./flowDb-4b19a42f-4mXsCvSf.js";
+} from "./flowDb-4b19a42f-Cf4l3Vi7.js";
 import {
     s as e
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     i,
     a as r,
     l as c,
     b as a,
     k as o,
     m as u
-} from "./edges-d32062c0-CFY3bIwa.js";
+} from "./edges-d32062c0-CU6OCHwI.js";
 import {
     l as s,
     _ as h,
     q as f,
     n as l,
     p as b,
     i as w
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     fm as d,
     gd as g
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     c as p
 } from "./step-BEJ6WznM.js";
 import {
     l as m
 } from "./line-Dz7yhIWK.js";
 import "./timer-D8GWrtRJ.js";
-import "./createText-6b48ae7d-129t9twG.js";
+import "./createText-6b48ae7d-BgOE7dMp.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 
 function v(n) {
     throw new Error('Could not dynamically require "' + n + '". Please configure the dynamicRequireTargets or/and ignoreDynamicRequires option of @rollup/plugin-commonjs appropriately for this require call to work.')
 }
 var k = {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/forth-Dri_5nFc.js` & `marimo-0.6.4/marimo/_static/assets/forth-Dri_5nFc.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/fortran-DL7KluxX.js` & `marimo-0.6.4/marimo/_static/assets/fortran-DL7KluxX.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ganttDiagram-9a3bba1f-Clnqsx9q.js` & `marimo-0.6.4/marimo/_static/assets/ganttDiagram-9a3bba1f-W6mmWQNE.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     a as o,
     y as c,
     k as l,
     l as d,
     h as u,
     i as h,
     x as f
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     fm as m,
     gd as y,
     jJ as k,
     jI as p,
     jG as g,
     jF as b,
@@ -27,27 +27,27 @@
     k3 as w,
     k4 as _,
     k5 as $,
     k6 as D,
     k7 as C,
     k8 as S,
     jH as M
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     s as E
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     t as A,
     m as Y,
     a as L,
     i as I
-} from "./time-CUBsQdfc.js";
+} from "./time-CLRyKR-T.js";
 import {
     k as F
-} from "./linear-DF6Se9n2.js";
+} from "./linear-JxYcrfvc.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 import "./init-DLRA0X12.js";
 
 function O(t) {
     return t
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/gas-5kEe4nk0.js` & `marimo-0.6.4/marimo/_static/assets/gas-5kEe4nk0.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/gherkin-B6X1vGSW.js` & `marimo-0.6.4/marimo/_static/assets/gherkin-B6X1vGSW.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/gitGraphDiagram-96e6b4ee-BUgJQeEj.js` & `marimo-0.6.4/marimo/_static/assets/gitGraphDiagram-96e6b4ee-BKc9lhir.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8,19 +8,19 @@
     v as s,
     l as c,
     i as o,
     y as l,
     x as h,
     R as m,
     S as y
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as u
-} from "./transform-DGMfQOK3.js";
-import "./index-Dq6tg2Hn.js";
+} from "./transform-DNjxe6pi.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 var p = function() {
     var t = function(t, e, r, i) {
             for (r = r || {}, i = t.length; i--; r[t[i]] = e);
             return r
         },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/gradient-yHQUC_QB.png` & `marimo-0.6.4/marimo/_static/assets/gradient-yHQUC_QB.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/graph-SHnEHiLi.js` & `marimo-0.6.4/marimo/_static/assets/graph-Dl9Z7r13.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -19,38 +19,38 @@
     ji as p,
     jV as g,
     jW as j,
     jX as m,
     jY as y,
     jZ as w,
     ix as C
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     z as E,
     A,
     B as N,
     C as D,
     D as L,
     E as O,
     F,
     G as x,
     H as M,
     I as P
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     b as S,
     a as I,
     h as U,
     c as B
-} from "./_baseEach-BrSWFoJM.js";
+} from "./_baseEach-FAhoh2N5.js";
 import {
     e as G,
     b as V,
     f as k
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 
 function z(e, t) {
     for (var r = -1, n = null == e ? 0 : e.length; ++r < n && !1 !== t(e[r], r, e););
     return e
 }
 
 function R(e, t, r, n) {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/groovy-BfRUB6GO.js` & `marimo-0.6.4/marimo/_static/assets/groovy-BfRUB6GO.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/haskell-CmdsSjFB.js` & `marimo-0.6.4/marimo/_static/assets/haskell-CmdsSjFB.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/haxe-75PMBtaN.js` & `marimo-0.6.4/marimo/_static/assets/haxe-75PMBtaN.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/home-page-BmvI7Tzs.js` & `marimo-0.6.4/marimo/_static/assets/home-page-BL9ArKPs.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -16,23 +16,23 @@
     t as p,
     e as m,
     g as f,
     f as g,
     h as b,
     k as j,
     l as v
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     u as k,
     S as w,
     C as N,
     a as y,
     M as z,
     P as I
-} from "./icons-6JftBaIY.js";
+} from "./icons-DtRVr9-T.js";
 /**
  * @license lucide-react v0.378.0 - ISC
  *
  * This source code is licensed under the ISC license.
  * See the LICENSE file in the root directory of this source tree.
  */
 const C = e("ExternalLink", [
```

### Comparing `marimo-0.6.3/marimo/_static/assets/http-BKJkqRj4.js` & `marimo-0.6.4/marimo/_static/assets/http-BKJkqRj4.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/icons-6JftBaIY.js` & `marimo-0.6.4/marimo/_static/assets/icons-DtRVr9-T.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -100,15 +100,15 @@
     aH as Ae,
     fv as Ie,
     fw as Be,
     aJ as Fe,
     bE as We,
     cH as He,
     bH as Ke
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 /**
  * @license lucide-react v0.378.0 - ISC
  *
  * This source code is licensed under the ISC license.
  * See the LICENSE file in the root directory of this source tree.
  */
 const Ue = n("PowerOff", [
@@ -4977,15 +4977,15 @@
 function st(e, ...t) {
     if (e)
         for (var n = 0; n < e.length; ++n) e[n](...t)
 }
 let at;
 try {
     at = new RegExp("[\\w\\p{Alphabetic}\\p{Number}_]", "u")
-} catch (Cd) {
+} catch (Gu) {
     at = /[\w]/
 }
 
 function ct(e, t) {
     var n = e.cm6;
     if (!n.state.readOnly) {
         var r = "input.type.compose";
@@ -6950,15 +6950,15 @@
             location: e
         }
     })
 };
 var Gn = Dn.DOMException;
 try {
     new Gn
-} catch (xd) {
+} catch (Xu) {
     (Gn = function(e, t) {
         this.message = e, this.name = t;
         var n = Error(e);
         this.stack = n.stack
     }).prototype = Object.create(Error.prototype), Gn.prototype.constructor = Gn
 }
 
@@ -7363,16 +7363,16 @@
         }, t.prototype.sendData = function(e, t) {
             return void 0 === t && (t = 5e3), hr(this, void 0, void 0, (function() {
                 var n, r, o;
                 return fr(this, (function(i) {
                     n = this.transportRequestManager.addRequest(e, t), r = gr.getNotifications(e);
                     try {
                         this.connection.send(JSON.stringify(this.parseData(e))), this.transportRequestManager.settlePendingRequest(r)
-                    } catch (xd) {
-                        o = new vr.JSONRPCError(xd.message, vr.ERR_UNKNOWN, xd), this.transportRequestManager.settlePendingRequest(r, o), this.transportRequestManager.settlePendingRequest(gr.getBatchRequests(e), o), n = Promise.reject(o)
+                    } catch (Xu) {
+                        o = new vr.JSONRPCError(Xu.message, vr.ERR_UNKNOWN, Xu), this.transportRequestManager.settlePendingRequest(r, o), this.transportRequestManager.settlePendingRequest(gr.getBatchRequests(e), o), n = Promise.reject(o)
                     }
                     return [2, n]
                 }))
             }))
         }, t.prototype.close = function() {
             this.connection.close()
         }, t
@@ -7890,2008 +7890,2048 @@
             get: function() {
                 return c.JSONRPCError
             }
         });
         var l = t(Pr);
         e.Client = l.default, e.default = l.default
     }($t);
-var qr = {},
-    Lr = {},
-    Ar = {},
+var qr, Lr, Ar = {},
     Ir = {},
     Br = {},
-    Fr = {};
+    Fr = {},
+    Wr = {},
+    Hr = {};
 
-function Wr(e) {
-    return "string" == typeof e || e instanceof String
-}
+function Kr() {
+    if (qr) return Hr;
 
-function Hr(e) {
-    return Array.isArray(e)
-}
-Object.defineProperty(Fr, "__esModule", {
-    value: !0
-}), Fr.stringArray = Fr.array = Fr.func = Fr.error = Fr.number = Fr.string = Fr.boolean = void 0, Fr.boolean = function(e) {
-    return !0 === e || !1 === e
-}, Fr.string = Wr, Fr.number = function(e) {
-    return "number" == typeof e || e instanceof Number
-}, Fr.error = function(e) {
-    return e instanceof Error
-}, Fr.func = function(e) {
-    return "function" == typeof e
-}, Fr.array = Hr, Fr.stringArray = function(e) {
-    return Hr(e) && e.every((e => Wr(e)))
-}, Object.defineProperty(Br, "__esModule", {
-    value: !0
-}), Br.Message = Br.NotificationType9 = Br.NotificationType8 = Br.NotificationType7 = Br.NotificationType6 = Br.NotificationType5 = Br.NotificationType4 = Br.NotificationType3 = Br.NotificationType2 = Br.NotificationType1 = Br.NotificationType0 = Br.NotificationType = Br.RequestType9 = Br.RequestType8 = Br.RequestType7 = Br.RequestType6 = Br.RequestType5 = Br.RequestType4 = Br.RequestType3 = Br.RequestType2 = Br.RequestType1 = Br.RequestType = Br.RequestType0 = Br.AbstractMessageSignature = Br.ParameterStructures = Br.ResponseError = Br.ErrorCodes = void 0;
-const Kr = Fr;
-var Ur, Vr, $r, zr;
-(Vr = Ur || (Br.ErrorCodes = Ur = {})).ParseError = -32700, Vr.InvalidRequest = -32600, Vr.MethodNotFound = -32601, Vr.InvalidParams = -32602, Vr.InternalError = -32603, Vr.jsonrpcReservedErrorRangeStart = -32099, Vr.serverErrorStart = -32099, Vr.MessageWriteError = -32099, Vr.MessageReadError = -32098, Vr.PendingResponseRejected = -32097, Vr.ConnectionInactive = -32096, Vr.ServerNotInitialized = -32002, Vr.UnknownErrorCode = -32001, Vr.jsonrpcReservedErrorRangeEnd = -32e3, Vr.serverErrorEnd = -32e3;
-class Jr extends Error {
-    constructor(e, t, n) {
-        super(t), this.code = Kr.number(e) ? e : Ur.UnknownErrorCode, this.data = n, Object.setPrototypeOf(this, Jr.prototype)
-    }
-    toJson() {
-        const e = {
-            code: this.code,
-            message: this.message
-        };
-        return void 0 !== this.data && (e.data = this.data), e
-    }
-}
-Br.ResponseError = Jr;
-class Qr {
-    constructor(e) {
-        this.kind = e
-    }
-    static is(e) {
-        return e === Qr.auto || e === Qr.byName || e === Qr.byPosition
-    }
-    toString() {
-        return this.kind
-    }
-}
-Br.ParameterStructures = Qr, Qr.auto = new Qr("auto"), Qr.byPosition = new Qr("byPosition"), Qr.byName = new Qr("byName");
-class Gr {
-    constructor(e, t) {
-        this.method = e, this.numberOfParams = t
+    function e(e) {
+        return "string" == typeof e || e instanceof String
     }
-    get parameterStructures() {
-        return Qr.auto
+
+    function t(e) {
+        return Array.isArray(e)
     }
+    return qr = 1, Object.defineProperty(Hr, "__esModule", {
+        value: !0
+    }), Hr.stringArray = Hr.array = Hr.func = Hr.error = Hr.number = Hr.string = Hr.boolean = void 0, Hr.boolean = function(e) {
+        return !0 === e || !1 === e
+    }, Hr.string = e, Hr.number = function(e) {
+        return "number" == typeof e || e instanceof Number
+    }, Hr.error = function(e) {
+        return e instanceof Error
+    }, Hr.func = function(e) {
+        return "function" == typeof e
+    }, Hr.array = t, Hr.stringArray = function(n) {
+        return t(n) && n.every((t => e(t)))
+    }, Hr
 }
-Br.AbstractMessageSignature = Gr;
-Br.RequestType0 = class extends Gr {
-    constructor(e) {
-        super(e, 0)
-    }
-};
-Br.RequestType = class extends Gr {
-    constructor(e, t = Qr.auto) {
-        super(e, 1), this._parameterStructures = t
-    }
-    get parameterStructures() {
-        return this._parameterStructures
-    }
-};
-Br.RequestType1 = class extends Gr {
-    constructor(e, t = Qr.auto) {
-        super(e, 1), this._parameterStructures = t
-    }
-    get parameterStructures() {
-        return this._parameterStructures
-    }
-};
-Br.RequestType2 = class extends Gr {
-    constructor(e) {
-        super(e, 2)
-    }
-};
-Br.RequestType3 = class extends Gr {
-    constructor(e) {
-        super(e, 3)
-    }
-};
-Br.RequestType4 = class extends Gr {
-    constructor(e) {
-        super(e, 4)
-    }
-};
-Br.RequestType5 = class extends Gr {
-    constructor(e) {
-        super(e, 5)
-    }
-};
-Br.RequestType6 = class extends Gr {
-    constructor(e) {
-        super(e, 6)
-    }
-};
-Br.RequestType7 = class extends Gr {
-    constructor(e) {
-        super(e, 7)
-    }
-};
-Br.RequestType8 = class extends Gr {
-    constructor(e) {
-        super(e, 8)
-    }
-};
-Br.RequestType9 = class extends Gr {
-    constructor(e) {
-        super(e, 9)
-    }
-};
-Br.NotificationType = class extends Gr {
-    constructor(e, t = Qr.auto) {
-        super(e, 1), this._parameterStructures = t
-    }
-    get parameterStructures() {
-        return this._parameterStructures
-    }
-};
-Br.NotificationType0 = class extends Gr {
-    constructor(e) {
-        super(e, 0)
-    }
-};
-Br.NotificationType1 = class extends Gr {
-    constructor(e, t = Qr.auto) {
-        super(e, 1), this._parameterStructures = t
-    }
-    get parameterStructures() {
-        return this._parameterStructures
-    }
-};
-Br.NotificationType2 = class extends Gr {
-    constructor(e) {
-        super(e, 2)
-    }
-};
-Br.NotificationType3 = class extends Gr {
-    constructor(e) {
-        super(e, 3)
-    }
-};
-Br.NotificationType4 = class extends Gr {
-    constructor(e) {
-        super(e, 4)
-    }
-};
-Br.NotificationType5 = class extends Gr {
-    constructor(e) {
-        super(e, 5)
-    }
-};
-Br.NotificationType6 = class extends Gr {
-    constructor(e) {
-        super(e, 6)
-    }
-};
-Br.NotificationType7 = class extends Gr {
-    constructor(e) {
-        super(e, 7)
-    }
-};
-Br.NotificationType8 = class extends Gr {
-    constructor(e) {
-        super(e, 8)
-    }
-};
-Br.NotificationType9 = class extends Gr {
-    constructor(e) {
-        super(e, 9)
-    }
-}, (zr = $r || (Br.Message = $r = {})).isRequest = function(e) {
-    const t = e;
-    return t && Kr.string(t.method) && (Kr.string(t.id) || Kr.number(t.id))
-}, zr.isNotification = function(e) {
-    const t = e;
-    return t && Kr.string(t.method) && void 0 === e.id
-}, zr.isResponse = function(e) {
-    const t = e;
-    return t && (void 0 !== t.result || !!t.error) && (Kr.string(t.id) || Kr.number(t.id) || null === t.id)
-};
-var Xr, Zr, Yr, eo = {};
-Object.defineProperty(eo, "__esModule", {
-    value: !0
-}), eo.LRUCache = eo.LinkedMap = eo.Touch = void 0, (Yr = Zr || (eo.Touch = Zr = {})).None = 0, Yr.First = 1, Yr.AsOld = Yr.First, Yr.Last = 2, Yr.AsNew = Yr.Last;
-class to {
-    constructor() {
-        this[Xr] = "LinkedMap", this._map = new Map, this._head = void 0, this._tail = void 0, this._size = 0, this._state = 0
-    }
-    clear() {
-        this._map.clear(), this._head = void 0, this._tail = void 0, this._size = 0, this._state++
-    }
-    isEmpty() {
-        return !this._head && !this._tail
-    }
-    get size() {
-        return this._size
-    }
-    get first() {
-        var e;
-        return null == (e = this._head) ? void 0 : e.value
+
+function Ur() {
+    if (Lr) return Wr;
+    Lr = 1, Object.defineProperty(Wr, "__esModule", {
+        value: !0
+    }), Wr.Message = Wr.NotificationType9 = Wr.NotificationType8 = Wr.NotificationType7 = Wr.NotificationType6 = Wr.NotificationType5 = Wr.NotificationType4 = Wr.NotificationType3 = Wr.NotificationType2 = Wr.NotificationType1 = Wr.NotificationType0 = Wr.NotificationType = Wr.RequestType9 = Wr.RequestType8 = Wr.RequestType7 = Wr.RequestType6 = Wr.RequestType5 = Wr.RequestType4 = Wr.RequestType3 = Wr.RequestType2 = Wr.RequestType1 = Wr.RequestType = Wr.RequestType0 = Wr.AbstractMessageSignature = Wr.ParameterStructures = Wr.ResponseError = Wr.ErrorCodes = void 0;
+    const e = Kr();
+    var t, n, r, o;
+    (n = t || (Wr.ErrorCodes = t = {})).ParseError = -32700, n.InvalidRequest = -32600, n.MethodNotFound = -32601, n.InvalidParams = -32602, n.InternalError = -32603, n.jsonrpcReservedErrorRangeStart = -32099, n.serverErrorStart = -32099, n.MessageWriteError = -32099, n.MessageReadError = -32098, n.PendingResponseRejected = -32097, n.ConnectionInactive = -32096, n.ServerNotInitialized = -32002, n.UnknownErrorCode = -32001, n.jsonrpcReservedErrorRangeEnd = -32e3, n.serverErrorEnd = -32e3;
+    class i extends Error {
+        constructor(n, r, o) {
+            super(r), this.code = e.number(n) ? n : t.UnknownErrorCode, this.data = o, Object.setPrototypeOf(this, i.prototype)
+        }
+        toJson() {
+            const e = {
+                code: this.code,
+                message: this.message
+            };
+            return void 0 !== this.data && (e.data = this.data), e
+        }
     }
-    get last() {
-        var e;
-        return null == (e = this._tail) ? void 0 : e.value
+    Wr.ResponseError = i;
+    class s {
+        constructor(e) {
+            this.kind = e
+        }
+        static is(e) {
+            return e === s.auto || e === s.byName || e === s.byPosition
+        }
+        toString() {
+            return this.kind
+        }
     }
-    has(e) {
-        return this._map.has(e)
+    Wr.ParameterStructures = s, s.auto = new s("auto"), s.byPosition = new s("byPosition"), s.byName = new s("byName");
+    class a {
+        constructor(e, t) {
+            this.method = e, this.numberOfParams = t
+        }
+        get parameterStructures() {
+            return s.auto
+        }
     }
-    get(e, t = Zr.None) {
-        const n = this._map.get(e);
-        if (n) return t !== Zr.None && this.touch(n, t), n.value
-    }
-    set(e, t, n = Zr.None) {
-        let r = this._map.get(e);
-        if (r) r.value = t, n !== Zr.None && this.touch(r, n);
-        else {
-            switch (r = {
-                    key: e,
-                    value: t,
-                    next: void 0,
-                    previous: void 0
-                }, n) {
-                case Zr.None:
-                    this.addItemLast(r);
-                    break;
-                case Zr.First:
-                    this.addItemFirst(r);
-                    break;
-                case Zr.Last:
-                default:
-                    this.addItemLast(r)
-            }
-            this._map.set(e, r), this._size++
-        }
-        return this
-    }
-    delete(e) {
-        return !!this.remove(e)
-    }
-    remove(e) {
-        const t = this._map.get(e);
-        if (t) return this._map.delete(e), this.removeItem(t), this._size--, t.value
-    }
-    shift() {
-        if (!this._head && !this._tail) return;
-        if (!this._head || !this._tail) throw new Error("Invalid list");
-        const e = this._head;
-        return this._map.delete(e.key), this.removeItem(e), this._size--, e.value
-    }
-    forEach(e, t) {
-        const n = this._state;
-        let r = this._head;
-        for (; r;) {
-            if (t ? e.bind(t)(r.value, r.key, this) : e(r.value, r.key, this), this._state !== n) throw new Error("LinkedMap got modified during iteration.");
-            r = r.next
-        }
-    }
-    keys() {
-        const e = this._state;
-        let t = this._head;
-        const n = {
-            [Symbol.iterator]: () => n,
-            next: () => {
-                if (this._state !== e) throw new Error("LinkedMap got modified during iteration.");
-                if (t) {
-                    const e = {
-                        value: t.key,
-                        done: !1
-                    };
-                    return t = t.next, e
-                }
-                return {
-                    value: void 0,
-                    done: !0
+    Wr.AbstractMessageSignature = a;
+    Wr.RequestType0 = class extends a {
+        constructor(e) {
+            super(e, 0)
+        }
+    };
+    Wr.RequestType = class extends a {
+        constructor(e, t = s.auto) {
+            super(e, 1), this._parameterStructures = t
+        }
+        get parameterStructures() {
+            return this._parameterStructures
+        }
+    };
+    Wr.RequestType1 = class extends a {
+        constructor(e, t = s.auto) {
+            super(e, 1), this._parameterStructures = t
+        }
+        get parameterStructures() {
+            return this._parameterStructures
+        }
+    };
+    Wr.RequestType2 = class extends a {
+        constructor(e) {
+            super(e, 2)
+        }
+    };
+    Wr.RequestType3 = class extends a {
+        constructor(e) {
+            super(e, 3)
+        }
+    };
+    Wr.RequestType4 = class extends a {
+        constructor(e) {
+            super(e, 4)
+        }
+    };
+    Wr.RequestType5 = class extends a {
+        constructor(e) {
+            super(e, 5)
+        }
+    };
+    Wr.RequestType6 = class extends a {
+        constructor(e) {
+            super(e, 6)
+        }
+    };
+    Wr.RequestType7 = class extends a {
+        constructor(e) {
+            super(e, 7)
+        }
+    };
+    Wr.RequestType8 = class extends a {
+        constructor(e) {
+            super(e, 8)
+        }
+    };
+    Wr.RequestType9 = class extends a {
+        constructor(e) {
+            super(e, 9)
+        }
+    };
+    Wr.NotificationType = class extends a {
+        constructor(e, t = s.auto) {
+            super(e, 1), this._parameterStructures = t
+        }
+        get parameterStructures() {
+            return this._parameterStructures
+        }
+    };
+    Wr.NotificationType0 = class extends a {
+        constructor(e) {
+            super(e, 0)
+        }
+    };
+    Wr.NotificationType1 = class extends a {
+        constructor(e, t = s.auto) {
+            super(e, 1), this._parameterStructures = t
+        }
+        get parameterStructures() {
+            return this._parameterStructures
+        }
+    };
+    Wr.NotificationType2 = class extends a {
+        constructor(e) {
+            super(e, 2)
+        }
+    };
+    Wr.NotificationType3 = class extends a {
+        constructor(e) {
+            super(e, 3)
+        }
+    };
+    Wr.NotificationType4 = class extends a {
+        constructor(e) {
+            super(e, 4)
+        }
+    };
+    Wr.NotificationType5 = class extends a {
+        constructor(e) {
+            super(e, 5)
+        }
+    };
+    Wr.NotificationType6 = class extends a {
+        constructor(e) {
+            super(e, 6)
+        }
+    };
+    Wr.NotificationType7 = class extends a {
+        constructor(e) {
+            super(e, 7)
+        }
+    };
+    Wr.NotificationType8 = class extends a {
+        constructor(e) {
+            super(e, 8)
+        }
+    };
+    return Wr.NotificationType9 = class extends a {
+        constructor(e) {
+            super(e, 9)
+        }
+    }, (o = r || (Wr.Message = r = {})).isRequest = function(t) {
+        const n = t;
+        return n && e.string(n.method) && (e.string(n.id) || e.number(n.id))
+    }, o.isNotification = function(t) {
+        const n = t;
+        return n && e.string(n.method) && void 0 === t.id
+    }, o.isResponse = function(t) {
+        const n = t;
+        return n && (void 0 !== n.result || !!n.error) && (e.string(n.id) || e.number(n.id) || null === n.id)
+    }, Wr
+}
+var Vr, $r = {};
+
+function zr() {
+    if (Vr) return $r;
+    var e, t, n;
+    Vr = 1, Object.defineProperty($r, "__esModule", {
+        value: !0
+    }), $r.LRUCache = $r.LinkedMap = $r.Touch = void 0, (n = t || ($r.Touch = t = {})).None = 0, n.First = 1, n.AsOld = n.First, n.Last = 2, n.AsNew = n.Last;
+    class r {
+        constructor() {
+            this[e] = "LinkedMap", this._map = new Map, this._head = void 0, this._tail = void 0, this._size = 0, this._state = 0
+        }
+        clear() {
+            this._map.clear(), this._head = void 0, this._tail = void 0, this._size = 0, this._state++
+        }
+        isEmpty() {
+            return !this._head && !this._tail
+        }
+        get size() {
+            return this._size
+        }
+        get first() {
+            var e;
+            return null == (e = this._head) ? void 0 : e.value
+        }
+        get last() {
+            var e;
+            return null == (e = this._tail) ? void 0 : e.value
+        }
+        has(e) {
+            return this._map.has(e)
+        }
+        get(e, n = t.None) {
+            const r = this._map.get(e);
+            if (r) return n !== t.None && this.touch(r, n), r.value
+        }
+        set(e, n, r = t.None) {
+            let o = this._map.get(e);
+            if (o) o.value = n, r !== t.None && this.touch(o, r);
+            else {
+                switch (o = {
+                        key: e,
+                        value: n,
+                        next: void 0,
+                        previous: void 0
+                    }, r) {
+                    case t.None:
+                        this.addItemLast(o);
+                        break;
+                    case t.First:
+                        this.addItemFirst(o);
+                        break;
+                    case t.Last:
+                    default:
+                        this.addItemLast(o)
                 }
+                this._map.set(e, o), this._size++
             }
-        };
-        return n
-    }
-    values() {
-        const e = this._state;
-        let t = this._head;
-        const n = {
-            [Symbol.iterator]: () => n,
-            next: () => {
-                if (this._state !== e) throw new Error("LinkedMap got modified during iteration.");
-                if (t) {
-                    const e = {
-                        value: t.value,
-                        done: !1
-                    };
-                    return t = t.next, e
-                }
-                return {
-                    value: void 0,
-                    done: !0
+            return this
+        }
+        delete(e) {
+            return !!this.remove(e)
+        }
+        remove(e) {
+            const t = this._map.get(e);
+            if (t) return this._map.delete(e), this.removeItem(t), this._size--, t.value
+        }
+        shift() {
+            if (!this._head && !this._tail) return;
+            if (!this._head || !this._tail) throw new Error("Invalid list");
+            const e = this._head;
+            return this._map.delete(e.key), this.removeItem(e), this._size--, e.value
+        }
+        forEach(e, t) {
+            const n = this._state;
+            let r = this._head;
+            for (; r;) {
+                if (t ? e.bind(t)(r.value, r.key, this) : e(r.value, r.key, this), this._state !== n) throw new Error("LinkedMap got modified during iteration.");
+                r = r.next
+            }
+        }
+        keys() {
+            const e = this._state;
+            let t = this._head;
+            const n = {
+                [Symbol.iterator]: () => n,
+                next: () => {
+                    if (this._state !== e) throw new Error("LinkedMap got modified during iteration.");
+                    if (t) {
+                        const e = {
+                            value: t.key,
+                            done: !1
+                        };
+                        return t = t.next, e
+                    }
+                    return {
+                        value: void 0,
+                        done: !0
+                    }
                 }
-            }
-        };
-        return n
-    }
-    entries() {
-        const e = this._state;
-        let t = this._head;
-        const n = {
-            [Symbol.iterator]: () => n,
-            next: () => {
-                if (this._state !== e) throw new Error("LinkedMap got modified during iteration.");
-                if (t) {
-                    const e = {
-                        value: [t.key, t.value],
-                        done: !1
-                    };
-                    return t = t.next, e
+            };
+            return n
+        }
+        values() {
+            const e = this._state;
+            let t = this._head;
+            const n = {
+                [Symbol.iterator]: () => n,
+                next: () => {
+                    if (this._state !== e) throw new Error("LinkedMap got modified during iteration.");
+                    if (t) {
+                        const e = {
+                            value: t.value,
+                            done: !1
+                        };
+                        return t = t.next, e
+                    }
+                    return {
+                        value: void 0,
+                        done: !0
+                    }
                 }
-                return {
-                    value: void 0,
-                    done: !0
+            };
+            return n
+        }
+        entries() {
+            const e = this._state;
+            let t = this._head;
+            const n = {
+                [Symbol.iterator]: () => n,
+                next: () => {
+                    if (this._state !== e) throw new Error("LinkedMap got modified during iteration.");
+                    if (t) {
+                        const e = {
+                            value: [t.key, t.value],
+                            done: !1
+                        };
+                        return t = t.next, e
+                    }
+                    return {
+                        value: void 0,
+                        done: !0
+                    }
                 }
+            };
+            return n
+        } [(e = Symbol.toStringTag, Symbol.iterator)]() {
+            return this.entries()
+        }
+        trimOld(e) {
+            if (e >= this.size) return;
+            if (0 === e) return void this.clear();
+            let t = this._head,
+                n = this.size;
+            for (; t && n > e;) this._map.delete(t.key), t = t.next, n--;
+            this._head = t, this._size = n, t && (t.previous = void 0), this._state++
+        }
+        addItemFirst(e) {
+            if (this._head || this._tail) {
+                if (!this._head) throw new Error("Invalid list");
+                e.next = this._head, this._head.previous = e
+            } else this._tail = e;
+            this._head = e, this._state++
+        }
+        addItemLast(e) {
+            if (this._head || this._tail) {
+                if (!this._tail) throw new Error("Invalid list");
+                e.previous = this._tail, this._tail.next = e
+            } else this._head = e;
+            this._tail = e, this._state++
+        }
+        removeItem(e) {
+            if (e === this._head && e === this._tail) this._head = void 0, this._tail = void 0;
+            else if (e === this._head) {
+                if (!e.next) throw new Error("Invalid list");
+                e.next.previous = void 0, this._head = e.next
+            } else if (e === this._tail) {
+                if (!e.previous) throw new Error("Invalid list");
+                e.previous.next = void 0, this._tail = e.previous
+            } else {
+                const t = e.next,
+                    n = e.previous;
+                if (!t || !n) throw new Error("Invalid list");
+                t.previous = n, n.next = t
             }
-        };
-        return n
-    } [(Xr = Symbol.toStringTag, Symbol.iterator)]() {
-        return this.entries()
-    }
-    trimOld(e) {
-        if (e >= this.size) return;
-        if (0 === e) return void this.clear();
-        let t = this._head,
-            n = this.size;
-        for (; t && n > e;) this._map.delete(t.key), t = t.next, n--;
-        this._head = t, this._size = n, t && (t.previous = void 0), this._state++
-    }
-    addItemFirst(e) {
-        if (this._head || this._tail) {
-            if (!this._head) throw new Error("Invalid list");
-            e.next = this._head, this._head.previous = e
-        } else this._tail = e;
-        this._head = e, this._state++
-    }
-    addItemLast(e) {
-        if (this._head || this._tail) {
-            if (!this._tail) throw new Error("Invalid list");
-            e.previous = this._tail, this._tail.next = e
-        } else this._head = e;
-        this._tail = e, this._state++
-    }
-    removeItem(e) {
-        if (e === this._head && e === this._tail) this._head = void 0, this._tail = void 0;
-        else if (e === this._head) {
-            if (!e.next) throw new Error("Invalid list");
-            e.next.previous = void 0, this._head = e.next
-        } else if (e === this._tail) {
-            if (!e.previous) throw new Error("Invalid list");
-            e.previous.next = void 0, this._tail = e.previous
-        } else {
-            const t = e.next,
-                n = e.previous;
-            if (!t || !n) throw new Error("Invalid list");
-            t.previous = n, n.next = t
-        }
-        e.next = void 0, e.previous = void 0, this._state++
-    }
-    touch(e, t) {
-        if (!this._head || !this._tail) throw new Error("Invalid list");
-        if (t === Zr.First || t === Zr.Last)
-            if (t === Zr.First) {
-                if (e === this._head) return;
+            e.next = void 0, e.previous = void 0, this._state++
+        }
+        touch(e, n) {
+            if (!this._head || !this._tail) throw new Error("Invalid list");
+            if (n === t.First || n === t.Last)
+                if (n === t.First) {
+                    if (e === this._head) return;
+                    const t = e.next,
+                        n = e.previous;
+                    e === this._tail ? (n.next = void 0, this._tail = n) : (t.previous = n, n.next = t), e.previous = void 0, e.next = this._head, this._head.previous = e, this._head = e, this._state++
+                } else if (n === t.Last) {
+                if (e === this._tail) return;
                 const t = e.next,
                     n = e.previous;
-                e === this._tail ? (n.next = void 0, this._tail = n) : (t.previous = n, n.next = t), e.previous = void 0, e.next = this._head, this._head.previous = e, this._head = e, this._state++
-            } else if (t === Zr.Last) {
-            if (e === this._tail) return;
-            const t = e.next,
-                n = e.previous;
-            e === this._head ? (t.previous = void 0, this._head = t) : (t.previous = n, n.next = t), e.next = void 0, e.previous = this._tail, this._tail.next = e, this._tail = e, this._state++
+                e === this._head ? (t.previous = void 0, this._head = t) : (t.previous = n, n.next = t), e.next = void 0, e.previous = this._tail, this._tail.next = e, this._tail = e, this._state++
+            }
         }
-    }
-    toJSON() {
-        const e = [];
-        return this.forEach(((t, n) => {
-            e.push([n, t])
-        })), e
-    }
-    fromJSON(e) {
-        this.clear();
-        for (const [t, n] of e) this.set(t, n)
-    }
-}
-eo.LinkedMap = to;
-eo.LRUCache = class extends to {
-    constructor(e, t = 1) {
-        super(), this._limit = e, this._ratio = Math.min(Math.max(0, t), 1)
-    }
-    get limit() {
-        return this._limit
-    }
-    set limit(e) {
-        this._limit = e, this.checkTrim()
-    }
-    get ratio() {
-        return this._ratio
-    }
-    set ratio(e) {
-        this._ratio = Math.min(Math.max(0, e), 1), this.checkTrim()
-    }
-    get(e, t = Zr.AsNew) {
-        return super.get(e, t)
-    }
-    peek(e) {
-        return super.get(e, Zr.None)
-    }
-    set(e, t) {
-        return super.set(e, t, Zr.Last), this.checkTrim(), this
-    }
-    checkTrim() {
-        this.size > this._limit && this.trimOld(Math.round(this._limit * this._ratio))
-    }
-};
-var no, ro = {};
-Object.defineProperty(ro, "__esModule", {
-    value: !0
-}), ro.Disposable = void 0, (no || (ro.Disposable = no = {})).create = function(e) {
-    return {
-        dispose: e
-    }
-};
-var oo = {},
-    io = {};
-let so;
-
-function ao() {
-    if (void 0 === so) throw new Error("No runtime abstraction layer installed");
-    return so
-}
-Object.defineProperty(io, "__esModule", {
-    value: !0
-}), (ao || (ao = {})).install = function(e) {
-    if (void 0 === e) throw new Error("No runtime abstraction layer provided");
-    so = e
-}, io.default = ao, Object.defineProperty(oo, "__esModule", {
-    value: !0
-}), oo.Emitter = oo.Event = void 0;
-const co = io;
-var lo;
-! function(e) {
-    const t = {
-        dispose() {}
-    };
-    e.None = function() {
-        return t
-    }
-}(lo || (oo.Event = lo = {}));
-class uo {
-    add(e, t = null, n) {
-        this._callbacks || (this._callbacks = [], this._contexts = []), this._callbacks.push(e), this._contexts.push(t), Array.isArray(n) && n.push({
-            dispose: () => this.remove(e, t)
-        })
-    }
-    remove(e, t = null) {
-        if (!this._callbacks) return;
-        let n = !1;
-        for (let r = 0, o = this._callbacks.length; r < o; r++)
-            if (this._callbacks[r] === e) {
-                if (this._contexts[r] === t) return this._callbacks.splice(r, 1), void this._contexts.splice(r, 1);
-                n = !0
-            } if (n) throw new Error("When adding a listener with a context, you should remove it with the same context")
-    }
-    invoke(...e) {
-        if (!this._callbacks) return [];
-        const t = [],
-            n = this._callbacks.slice(0),
-            r = this._contexts.slice(0);
-        for (let i = 0, s = n.length; i < s; i++) try {
-            t.push(n[i].apply(r[i], e))
-        } catch (o) {
-            (0, co.default)().console.error(o)
+        toJSON() {
+            const e = [];
+            return this.forEach(((t, n) => {
+                e.push([n, t])
+            })), e
         }
-        return t
-    }
-    isEmpty() {
-        return !this._callbacks || 0 === this._callbacks.length
-    }
-    dispose() {
-        this._callbacks = void 0, this._contexts = void 0
-    }
-}
-class ho {
-    constructor(e) {
-        this._options = e
-    }
-    get event() {
-        return this._event || (this._event = (e, t, n) => {
-            this._callbacks || (this._callbacks = new uo), this._options && this._options.onFirstListenerAdd && this._callbacks.isEmpty() && this._options.onFirstListenerAdd(this), this._callbacks.add(e, t);
-            const r = {
-                dispose: () => {
-                    this._callbacks && (this._callbacks.remove(e, t), r.dispose = ho._noop, this._options && this._options.onLastListenerRemove && this._callbacks.isEmpty() && this._options.onLastListenerRemove(this))
-                }
-            };
-            return Array.isArray(n) && n.push(r), r
-        }), this._event
-    }
-    fire(e) {
-        this._callbacks && this._callbacks.invoke.call(this._callbacks, e)
-    }
-    dispose() {
-        this._callbacks && (this._callbacks.dispose(), this._callbacks = void 0)
-    }
-}
-oo.Emitter = ho, ho._noop = function() {};
-var fo = {};
-Object.defineProperty(fo, "__esModule", {
-    value: !0
-}), fo.CancellationTokenSource = fo.CancellationToken = void 0;
-const po = io,
-    mo = Fr,
-    go = oo;
-var vo, yo;
-(yo = vo || (fo.CancellationToken = vo = {})).None = Object.freeze({
-    isCancellationRequested: !1,
-    onCancellationRequested: go.Event.None
-}), yo.Cancelled = Object.freeze({
-    isCancellationRequested: !0,
-    onCancellationRequested: go.Event.None
-}), yo.is = function(e) {
-    const t = e;
-    return t && (t === yo.None || t === yo.Cancelled || mo.boolean(t.isCancellationRequested) && !!t.onCancellationRequested)
-};
-const bo = Object.freeze((function(e, t) {
-    const n = (0, po.default)().timer.setTimeout(e.bind(t), 0);
-    return {
-        dispose() {
-            n.dispose()
+        fromJSON(e) {
+            this.clear();
+            for (const [t, n] of e) this.set(t, n)
         }
     }
-}));
-class wo {
-    constructor() {
-        this._isCancelled = !1
-    }
-    cancel() {
-        this._isCancelled || (this._isCancelled = !0, this._emitter && (this._emitter.fire(void 0), this.dispose()))
-    }
-    get isCancellationRequested() {
-        return this._isCancelled
-    }
-    get onCancellationRequested() {
-        return this._isCancelled ? bo : (this._emitter || (this._emitter = new go.Emitter), this._emitter.event)
-    }
-    dispose() {
-        this._emitter && (this._emitter.dispose(), this._emitter = void 0)
-    }
-}
-fo.CancellationTokenSource = class {
-    get token() {
-        return this._token || (this._token = new wo), this._token
-    }
-    cancel() {
-        this._token ? this._token.cancel() : this._token = vo.Cancelled
-    }
-    dispose() {
-        this._token ? this._token instanceof wo && this._token.dispose() : this._token = vo.None
-    }
-};
-var Co = {};
-Object.defineProperty(Co, "__esModule", {
-    value: !0
-}), Co.SharedArrayReceiverStrategy = Co.SharedArraySenderStrategy = void 0;
-const xo = fo;
-var ko, Ro;
-(Ro = ko || (ko = {})).Continue = 0, Ro.Cancelled = 1;
-Co.SharedArraySenderStrategy = class {
-    constructor() {
-        this.buffers = new Map
-    }
-    enableCancellation(e) {
-        if (null === e.id) return;
-        const t = new SharedArrayBuffer(4);
-        new Int32Array(t, 0, 1)[0] = ko.Continue, this.buffers.set(e.id, t), e.$cancellationData = t
-    }
-    async sendCancellation(e, t) {
-        const n = this.buffers.get(t);
-        if (void 0 === n) return;
-        const r = new Int32Array(n, 0, 1);
-        Atomics.store(r, 0, ko.Cancelled)
-    }
-    cleanup(e) {
-        this.buffers.delete(e)
-    }
-    dispose() {
-        this.buffers.clear()
-    }
-};
-class To {
-    constructor(e) {
-        this.data = new Int32Array(e, 0, 1)
-    }
-    get isCancellationRequested() {
-        return Atomics.load(this.data, 0) === ko.Cancelled
-    }
-    get onCancellationRequested() {
-        throw new Error("Cancellation over SharedArrayBuffer doesn't support cancellation events")
-    }
+    $r.LinkedMap = r;
+    return $r.LRUCache = class extends r {
+        constructor(e, t = 1) {
+            super(), this._limit = e, this._ratio = Math.min(Math.max(0, t), 1)
+        }
+        get limit() {
+            return this._limit
+        }
+        set limit(e) {
+            this._limit = e, this.checkTrim()
+        }
+        get ratio() {
+            return this._ratio
+        }
+        set ratio(e) {
+            this._ratio = Math.min(Math.max(0, e), 1), this.checkTrim()
+        }
+        get(e, n = t.AsNew) {
+            return super.get(e, n)
+        }
+        peek(e) {
+            return super.get(e, t.None)
+        }
+        set(e, n) {
+            return super.set(e, n, t.Last), this.checkTrim(), this
+        }
+        checkTrim() {
+            this.size > this._limit && this.trimOld(Math.round(this._limit * this._ratio))
+        }
+    }, $r
 }
-class So {
-    constructor(e) {
-        this.token = new To(e)
+var Jr, Qr = {};
+var Gr, Xr, Zr = {},
+    Yr = {};
+
+function eo() {
+    if (Gr) return Yr;
+    let e;
+
+    function t() {
+        if (void 0 === e) throw new Error("No runtime abstraction layer installed");
+        return e
     }
-    cancel() {}
-    dispose() {}
+    return Gr = 1, Object.defineProperty(Yr, "__esModule", {
+        value: !0
+    }), (t || (t = {})).install = function(t) {
+        if (void 0 === t) throw new Error("No runtime abstraction layer provided");
+        e = t
+    }, Yr.default = t, Yr
 }
-Co.SharedArrayReceiverStrategy = class {
-    constructor() {
-        this.kind = "request"
-    }
-    createCancellationTokenSource(e) {
-        const t = e.$cancellationData;
-        return void 0 === t ? new xo.CancellationTokenSource : new So(t)
-    }
-};
-var Mo = {},
-    Do = {};
-Object.defineProperty(Do, "__esModule", {
-    value: !0
-}), Do.Semaphore = void 0;
-const _o = io;
-Do.Semaphore = class {
-    constructor(e = 1) {
-        if (e <= 0) throw new Error("Capacity must be greater than 0");
-        this._capacity = e, this._active = 0, this._waiting = []
-    }
-    lock(e) {
-        return new Promise(((t, n) => {
-            this._waiting.push({
-                thunk: e,
-                resolve: t,
-                reject: n
-            }), this.runNext()
-        }))
-    }
-    get active() {
-        return this._active
-    }
-    runNext() {
-        0 !== this._waiting.length && this._active !== this._capacity && (0, _o.default)().timer.setImmediate((() => this.doRunNext()))
-    }
-    doRunNext() {
-        if (0 === this._waiting.length || this._active === this._capacity) return;
-        const e = this._waiting.shift();
-        if (this._active++, this._active > this._capacity) throw new Error("To many thunks active");
-        try {
-            const t = e.thunk();
-            t instanceof Promise ? t.then((t => {
-                this._active--, e.resolve(t), this.runNext()
-            }), (t => {
-                this._active--, e.reject(t), this.runNext()
-            })) : (this._active--, e.resolve(t), this.runNext())
-        } catch (xd) {
-            this._active--, e.reject(xd), this.runNext()
+
+function to() {
+    if (Xr) return Zr;
+    Xr = 1, Object.defineProperty(Zr, "__esModule", {
+        value: !0
+    }), Zr.Emitter = Zr.Event = void 0;
+    const e = eo();
+    var t;
+    ! function(e) {
+        const t = {
+            dispose() {}
+        };
+        e.None = function() {
+            return t
         }
-    }
-}, Object.defineProperty(Mo, "__esModule", {
-    value: !0
-}), Mo.ReadableStreamMessageReader = Mo.AbstractMessageReader = Mo.MessageReader = void 0;
-const Eo = io,
-    Po = Fr,
-    Oo = oo,
-    No = Do;
-var jo, qo;
-(jo || (Mo.MessageReader = jo = {})).is = function(e) {
-    let t = e;
-    return t && Po.func(t.listen) && Po.func(t.dispose) && Po.func(t.onError) && Po.func(t.onClose) && Po.func(t.onPartialMessage)
-};
-class Lo {
-    constructor() {
-        this.errorEmitter = new Oo.Emitter, this.closeEmitter = new Oo.Emitter, this.partialMessageEmitter = new Oo.Emitter
-    }
-    dispose() {
-        this.errorEmitter.dispose(), this.closeEmitter.dispose()
-    }
-    get onError() {
-        return this.errorEmitter.event
-    }
-    fireError(e) {
-        this.errorEmitter.fire(this.asError(e))
-    }
-    get onClose() {
-        return this.closeEmitter.event
-    }
-    fireClose() {
-        this.closeEmitter.fire(void 0)
-    }
-    get onPartialMessage() {
-        return this.partialMessageEmitter.event
-    }
-    firePartialMessage(e) {
-        this.partialMessageEmitter.fire(e)
-    }
-    asError(e) {
-        return e instanceof Error ? e : new Error(`Reader received error. Reason: ${Po.string(e.message)?e.message:"unknown"}`)
-    }
-}
-Mo.AbstractMessageReader = Lo, (qo || (qo = {})).fromOptions = function(e) {
-    let t, n;
-    const r = new Map;
-    let o;
-    const i = new Map;
-    if (void 0 === e || "string" == typeof e) t = e ?? "utf-8";
-    else {
-        if (t = e.charset ?? "utf-8", void 0 !== e.contentDecoder && (n = e.contentDecoder, r.set(n.name, n)), void 0 !== e.contentDecoders)
-            for (const t of e.contentDecoders) r.set(t.name, t);
-        if (void 0 !== e.contentTypeDecoder && (o = e.contentTypeDecoder, i.set(o.name, o)), void 0 !== e.contentTypeDecoders)
-            for (const t of e.contentTypeDecoders) i.set(t.name, t)
-    }
-    return void 0 === o && (o = (0, Eo.default)().applicationJson.decoder, i.set(o.name, o)), {
-        charset: t,
-        contentDecoder: n,
-        contentDecoders: r,
-        contentTypeDecoder: o,
-        contentTypeDecoders: i
-    }
-};
-Mo.ReadableStreamMessageReader = class extends Lo {
-    constructor(e, t) {
-        super(), this.readable = e, this.options = qo.fromOptions(t), this.buffer = (0, Eo.default)().messageBuffer.create(this.options.charset), this._partialMessageTimeout = 1e4, this.nextMessageLength = -1, this.messageToken = 0, this.readSemaphore = new No.Semaphore(1)
-    }
-    set partialMessageTimeout(e) {
-        this._partialMessageTimeout = e
-    }
-    get partialMessageTimeout() {
-        return this._partialMessageTimeout
-    }
-    listen(e) {
-        this.nextMessageLength = -1, this.messageToken = 0, this.partialMessageTimer = void 0, this.callback = e;
-        const t = this.readable.onData((e => {
-            this.onData(e)
-        }));
-        return this.readable.onError((e => this.fireError(e))), this.readable.onClose((() => this.fireClose())), t
-    }
-    onData(e) {
-        try {
-            for (this.buffer.append(e);;) {
-                if (-1 === this.nextMessageLength) {
-                    const e = this.buffer.tryReadHeaders(!0);
-                    if (!e) return;
-                    const t = e.get("content-length");
-                    if (!t) return void this.fireError(new Error(`Header must provide a Content-Length property.\n${JSON.stringify(Object.fromEntries(e))}`));
-                    const n = parseInt(t);
-                    if (isNaN(n)) return void this.fireError(new Error(`Content-Length value must be a number. Got ${t}`));
-                    this.nextMessageLength = n
-                }
-                const e = this.buffer.tryReadBody(this.nextMessageLength);
-                if (void 0 === e) return void this.setPartialMessageTimer();
-                this.clearPartialMessageTimer(), this.nextMessageLength = -1, this.readSemaphore.lock((async () => {
-                    const t = void 0 !== this.options.contentDecoder ? await this.options.contentDecoder.decode(e) : e,
-                        n = await this.options.contentTypeDecoder.decode(t, this.options);
-                    this.callback(n)
-                })).catch((e => {
-                    this.fireError(e)
-                }))
+    }(t || (Zr.Event = t = {}));
+    class n {
+        add(e, t = null, n) {
+            this._callbacks || (this._callbacks = [], this._contexts = []), this._callbacks.push(e), this._contexts.push(t), Array.isArray(n) && n.push({
+                dispose: () => this.remove(e, t)
+            })
+        }
+        remove(e, t = null) {
+            if (!this._callbacks) return;
+            let n = !1;
+            for (let r = 0, o = this._callbacks.length; r < o; r++)
+                if (this._callbacks[r] === e) {
+                    if (this._contexts[r] === t) return this._callbacks.splice(r, 1), void this._contexts.splice(r, 1);
+                    n = !0
+                } if (n) throw new Error("When adding a listener with a context, you should remove it with the same context")
+        }
+        invoke(...t) {
+            if (!this._callbacks) return [];
+            const n = [],
+                r = this._callbacks.slice(0),
+                o = this._contexts.slice(0);
+            for (let s = 0, a = r.length; s < a; s++) try {
+                n.push(r[s].apply(o[s], t))
+            } catch (i) {
+                (0, e.default)().console.error(i)
             }
-        } catch (t) {
-            this.fireError(t)
+            return n
         }
-    }
-    clearPartialMessageTimer() {
-        this.partialMessageTimer && (this.partialMessageTimer.dispose(), this.partialMessageTimer = void 0)
-    }
-    setPartialMessageTimer() {
-        this.clearPartialMessageTimer(), this._partialMessageTimeout <= 0 || (this.partialMessageTimer = (0, Eo.default)().timer.setTimeout(((e, t) => {
-            this.partialMessageTimer = void 0, e === this.messageToken && (this.firePartialMessage({
-                messageToken: e,
-                waitingTime: t
-            }), this.setPartialMessageTimer())
-        }), this._partialMessageTimeout, this.messageToken, this._partialMessageTimeout))
-    }
-};
-var Ao = {};
-Object.defineProperty(Ao, "__esModule", {
-    value: !0
-}), Ao.WriteableStreamMessageWriter = Ao.AbstractMessageWriter = Ao.MessageWriter = void 0;
-const Io = io,
-    Bo = Fr,
-    Fo = Do,
-    Wo = oo;
-var Ho, Ko;
-(Ho || (Ao.MessageWriter = Ho = {})).is = function(e) {
-    let t = e;
-    return t && Bo.func(t.dispose) && Bo.func(t.onClose) && Bo.func(t.onError) && Bo.func(t.write)
-};
-class Uo {
-    constructor() {
-        this.errorEmitter = new Wo.Emitter, this.closeEmitter = new Wo.Emitter
-    }
-    dispose() {
-        this.errorEmitter.dispose(), this.closeEmitter.dispose()
-    }
-    get onError() {
-        return this.errorEmitter.event
-    }
-    fireError(e, t, n) {
-        this.errorEmitter.fire([this.asError(e), t, n])
-    }
-    get onClose() {
-        return this.closeEmitter.event
-    }
-    fireClose() {
-        this.closeEmitter.fire(void 0)
-    }
-    asError(e) {
-        return e instanceof Error ? e : new Error(`Writer received error. Reason: ${Bo.string(e.message)?e.message:"unknown"}`)
-    }
-}
-Ao.AbstractMessageWriter = Uo, (Ko || (Ko = {})).fromOptions = function(e) {
-    return void 0 === e || "string" == typeof e ? {
-        charset: e ?? "utf-8",
-        contentTypeEncoder: (0, Io.default)().applicationJson.encoder
-    } : {
-        charset: e.charset ?? "utf-8",
-        contentEncoder: e.contentEncoder,
-        contentTypeEncoder: e.contentTypeEncoder ?? (0, Io.default)().applicationJson.encoder
-    }
-};
-Ao.WriteableStreamMessageWriter = class extends Uo {
-    constructor(e, t) {
-        super(), this.writable = e, this.options = Ko.fromOptions(t), this.errorCount = 0, this.writeSemaphore = new Fo.Semaphore(1), this.writable.onError((e => this.fireError(e))), this.writable.onClose((() => this.fireClose()))
-    }
-    async write(e) {
-        return this.writeSemaphore.lock((async () => this.options.contentTypeEncoder.encode(e, this.options).then((e => void 0 !== this.options.contentEncoder ? this.options.contentEncoder.encode(e) : e)).then((t => {
-            const n = [];
-            return n.push("Content-Length: ", t.byteLength.toString(), "\r\n"), n.push("\r\n"), this.doWrite(e, n, t)
-        }), (e => {
-            throw this.fireError(e), e
-        }))))
-    }
-    async doWrite(e, t, n) {
-        try {
-            return await this.writable.write(t.join(""), "ascii"), this.writable.write(n)
-        } catch (r) {
-            return this.handleError(r, e), Promise.reject(r)
+        isEmpty() {
+            return !this._callbacks || 0 === this._callbacks.length
+        }
+        dispose() {
+            this._callbacks = void 0, this._contexts = void 0
         }
     }
-    handleError(e, t) {
-        this.errorCount++, this.fireError(e, t, this.errorCount)
-    }
-    end() {
-        this.writable.end()
-    }
-};
-var Vo = {};
-Object.defineProperty(Vo, "__esModule", {
-    value: !0
-}), Vo.AbstractMessageBuffer = void 0;
-Vo.AbstractMessageBuffer = class {
-    constructor(e = "utf-8") {
-        this._encoding = e, this._chunks = [], this._totalLength = 0
-    }
-    get encoding() {
-        return this._encoding
-    }
-    append(e) {
-        const t = "string" == typeof e ? this.fromString(e, this._encoding) : e;
-        this._chunks.push(t), this._totalLength += t.byteLength
-    }
-    tryReadHeaders(e = !1) {
-        if (0 === this._chunks.length) return;
-        let t = 0,
-            n = 0,
-            r = 0,
-            o = 0;
-        e: for (; n < this._chunks.length;) {
-            const e = this._chunks[n];
-            for (r = 0; r < e.length;) {
-                switch (e[r]) {
-                    case 13:
-                        switch (t) {
-                            case 0:
-                                t = 1;
-                                break;
-                            case 2:
-                                t = 3;
-                                break;
-                            default:
-                                t = 0
-                        }
-                        break;
-                    case 10:
-                        switch (t) {
-                            case 1:
-                                t = 2;
-                                break;
-                            case 3:
-                                t = 4, r++;
-                                break e;
-                            default:
-                                t = 0
-                        }
-                        break;
-                    default:
-                        t = 0
-                }
-                r++
-            }
-            o += e.byteLength, n++
+    class r {
+        constructor(e) {
+            this._options = e
+        }
+        get event() {
+            return this._event || (this._event = (e, t, o) => {
+                this._callbacks || (this._callbacks = new n), this._options && this._options.onFirstListenerAdd && this._callbacks.isEmpty() && this._options.onFirstListenerAdd(this), this._callbacks.add(e, t);
+                const i = {
+                    dispose: () => {
+                        this._callbacks && (this._callbacks.remove(e, t), i.dispose = r._noop, this._options && this._options.onLastListenerRemove && this._callbacks.isEmpty() && this._options.onLastListenerRemove(this))
+                    }
+                };
+                return Array.isArray(o) && o.push(i), i
+            }), this._event
         }
-        if (4 !== t) return;
-        const i = this._read(o + r),
-            s = new Map,
-            a = this.toString(i, "ascii").split("\r\n");
-        if (a.length < 2) return s;
-        for (let c = 0; c < a.length - 2; c++) {
-            const t = a[c],
-                n = t.indexOf(":");
-            if (-1 === n) throw new Error(`Message header must separate key and value using ':'\n${t}`);
-            const r = t.substr(0, n),
-                o = t.substr(n + 1).trim();
-            s.set(e ? r.toLowerCase() : r, o)
-        }
-        return s
-    }
-    tryReadBody(e) {
-        if (!(this._totalLength < e)) return this._read(e)
-    }
-    get numberOfBytes() {
-        return this._totalLength
-    }
-    _read(e) {
-        if (0 === e) return this.emptyBuffer();
-        if (e > this._totalLength) throw new Error("Cannot read so many bytes!");
-        if (this._chunks[0].byteLength === e) {
-            const t = this._chunks[0];
-            return this._chunks.shift(), this._totalLength -= e, this.asNative(t)
-        }
-        if (this._chunks[0].byteLength > e) {
-            const t = this._chunks[0],
-                n = this.asNative(t, e);
-            return this._chunks[0] = t.slice(e), this._totalLength -= e, n
-        }
-        const t = this.allocNative(e);
-        let n = 0;
-        for (; e > 0;) {
-            const r = this._chunks[0];
-            if (r.byteLength > e) {
-                const o = r.slice(0, e);
-                t.set(o, n), n += e, this._chunks[0] = r.slice(e), this._totalLength -= e, e -= e
-            } else t.set(r, n), n += r.byteLength, this._chunks.shift(), this._totalLength -= r.byteLength, e -= r.byteLength
+        fire(e) {
+            this._callbacks && this._callbacks.invoke.call(this._callbacks, e)
+        }
+        dispose() {
+            this._callbacks && (this._callbacks.dispose(), this._callbacks = void 0)
         }
-        return t
     }
-};
-var $o = {};
-! function(e) {
-    Object.defineProperty(e, "__esModule", {
+    return Zr.Emitter = r, r._noop = function() {}, Zr
+}
+var no, ro = {};
+
+function oo() {
+    if (no) return ro;
+    no = 1, Object.defineProperty(ro, "__esModule", {
         value: !0
-    }), e.createMessageConnection = e.ConnectionOptions = e.MessageStrategy = e.CancellationStrategy = e.CancellationSenderStrategy = e.CancellationReceiverStrategy = e.RequestCancellationReceiverStrategy = e.IdCancellationReceiverStrategy = e.ConnectionStrategy = e.ConnectionError = e.ConnectionErrors = e.LogTraceNotification = e.SetTraceNotification = e.TraceFormat = e.TraceValues = e.Trace = e.NullLogger = e.ProgressType = e.ProgressToken = void 0;
-    const t = io,
-        n = Fr,
-        r = Br,
-        o = eo,
-        i = oo,
-        s = fo;
-    var a, c, l, u, d, h, f, p, m, g, v, y, b, w, C, x, k, R, T, S, M, D, _, E, P, O, N;
-    (a || (a = {})).type = new r.NotificationType("$/cancelRequest"), (c || (e.ProgressToken = c = {})).is = function(e) {
-        return "string" == typeof e || "number" == typeof e
-    }, (l || (l = {})).type = new r.NotificationType("$/progress");
-    e.ProgressType = class {
-            constructor() {}
-        }, (u || (u = {})).is = function(e) {
-            return n.func(e)
-        }, e.NullLogger = Object.freeze({
-            error: () => {},
-            warn: () => {},
-            info: () => {},
-            log: () => {}
-        }), (h = d || (e.Trace = d = {}))[h.Off = 0] = "Off", h[h.Messages = 1] = "Messages", h[h.Compact = 2] = "Compact", h[h.Verbose = 3] = "Verbose", (p = f || (e.TraceValues = f = {})).Off = "off", p.Messages = "messages", p.Compact = "compact", p.Verbose = "verbose",
-        function(e) {
-            e.fromString = function(t) {
-                if (!n.string(t)) return e.Off;
-                switch (t = t.toLowerCase()) {
-                    case "off":
-                    default:
-                        return e.Off;
-                    case "messages":
-                        return e.Messages;
-                    case "compact":
-                        return e.Compact;
-                    case "verbose":
-                        return e.Verbose
-                }
-            }, e.toString = function(t) {
-                switch (t) {
-                    case e.Off:
-                        return "off";
-                    case e.Messages:
-                        return "messages";
-                    case e.Compact:
-                        return "compact";
-                    case e.Verbose:
-                        return "verbose";
-                    default:
-                        return "off"
-                }
-            }
-        }(d || (e.Trace = d = {})), (g = m || (e.TraceFormat = m = {})).Text = "text", g.JSON = "json",
-        function(e) {
-            e.fromString = function(t) {
-                return n.string(t) && "json" === (t = t.toLowerCase()) ? e.JSON : e.Text
+    }), ro.CancellationTokenSource = ro.CancellationToken = void 0;
+    const e = eo(),
+        t = Kr(),
+        n = to();
+    var r, o;
+    (o = r || (ro.CancellationToken = r = {})).None = Object.freeze({
+        isCancellationRequested: !1,
+        onCancellationRequested: n.Event.None
+    }), o.Cancelled = Object.freeze({
+        isCancellationRequested: !0,
+        onCancellationRequested: n.Event.None
+    }), o.is = function(e) {
+        const n = e;
+        return n && (n === o.None || n === o.Cancelled || t.boolean(n.isCancellationRequested) && !!n.onCancellationRequested)
+    };
+    const i = Object.freeze((function(t, n) {
+        const r = (0, e.default)().timer.setTimeout(t.bind(n), 0);
+        return {
+            dispose() {
+                r.dispose()
             }
-        }(m || (e.TraceFormat = m = {})), (v || (e.SetTraceNotification = v = {})).type = new r.NotificationType("$/setTrace"), (y || (e.LogTraceNotification = y = {})).type = new r.NotificationType("$/logTrace"), (w = b || (e.ConnectionErrors = b = {}))[w.Closed = 1] = "Closed", w[w.Disposed = 2] = "Disposed", w[w.AlreadyListening = 3] = "AlreadyListening";
-    class j extends Error {
-        constructor(e, t) {
-            super(t), this.code = e, Object.setPrototypeOf(this, j.prototype)
+        }
+    }));
+    class s {
+        constructor() {
+            this._isCancelled = !1
+        }
+        cancel() {
+            this._isCancelled || (this._isCancelled = !0, this._emitter && (this._emitter.fire(void 0), this.dispose()))
+        }
+        get isCancellationRequested() {
+            return this._isCancelled
+        }
+        get onCancellationRequested() {
+            return this._isCancelled ? i : (this._emitter || (this._emitter = new n.Emitter), this._emitter.event)
+        }
+        dispose() {
+            this._emitter && (this._emitter.dispose(), this._emitter = void 0)
         }
     }
-    e.ConnectionError = j, (C || (e.ConnectionStrategy = C = {})).is = function(e) {
-        const t = e;
-        return t && n.func(t.cancelUndispatched)
-    }, (x || (e.IdCancellationReceiverStrategy = x = {})).is = function(e) {
-        const t = e;
-        return t && (void 0 === t.kind || "id" === t.kind) && n.func(t.createCancellationTokenSource) && (void 0 === t.dispose || n.func(t.dispose))
-    }, (k || (e.RequestCancellationReceiverStrategy = k = {})).is = function(e) {
-        const t = e;
-        return t && "request" === t.kind && n.func(t.createCancellationTokenSource) && (void 0 === t.dispose || n.func(t.dispose))
-    }, (T = R || (e.CancellationReceiverStrategy = R = {})).Message = Object.freeze({
-        createCancellationTokenSource: e => new s.CancellationTokenSource
-    }), T.is = function(e) {
-        return x.is(e) || k.is(e)
-    }, (M = S || (e.CancellationSenderStrategy = S = {})).Message = Object.freeze({
-        sendCancellation: (e, t) => e.sendNotification(a.type, {
-            id: t
-        }),
-        cleanup(e) {}
-    }), M.is = function(e) {
-        const t = e;
-        return t && n.func(t.sendCancellation) && n.func(t.cleanup)
-    }, (_ = D || (e.CancellationStrategy = D = {})).Message = Object.freeze({
-        receiver: R.Message,
-        sender: S.Message
-    }), _.is = function(e) {
-        const t = e;
-        return t && R.is(t.receiver) && S.is(t.sender)
-    }, (E || (e.MessageStrategy = E = {})).is = function(e) {
-        const t = e;
-        return t && n.func(t.handleMessage)
-    }, (P || (e.ConnectionOptions = P = {})).is = function(e) {
-        const t = e;
-        return t && (D.is(t.cancellationStrategy) || C.is(t.connectionStrategy) || E.is(t.messageStrategy))
-    }, (N = O || (O = {}))[N.New = 1] = "New", N[N.Listening = 2] = "Listening", N[N.Closed = 3] = "Closed", N[N.Disposed = 4] = "Disposed", e.createMessageConnection = function(h, f, p, g) {
-        const w = void 0 !== p ? p : e.NullLogger;
-        let C = 0,
-            k = 0,
-            R = 0;
-        const T = "2.0";
-        let S;
-        const M = new Map;
-        let _;
-        const P = new Map,
-            N = new Map;
-        let q, L, A = new o.LinkedMap,
-            I = new Map,
-            B = new Set,
-            F = new Map,
-            W = d.Off,
-            H = m.Text,
-            K = O.New;
-        const U = new i.Emitter,
-            V = new i.Emitter,
-            $ = new i.Emitter,
-            z = new i.Emitter,
-            J = new i.Emitter,
-            Q = g && g.cancellationStrategy ? g.cancellationStrategy : D.Message;
-
-        function G(e) {
-            if (null === e) throw new Error("Can't send requests with id null since the response can't be correlated.");
-            return "req-" + e.toString()
-        }
-
-        function X(e, t) {
-            var n;
-            r.Message.isRequest(t) ? e.set(G(t.id), t) : r.Message.isResponse(t) ? e.set(null === (n = t.id) ? "res-unknown-" + (++R).toString() : "res-" + n.toString(), t) : e.set("not-" + (++k).toString(), t)
-        }
-
-        function Z(e) {}
-
-        function Y() {
-            return K === O.Listening
-        }
-
-        function ee() {
-            return K === O.Closed
-        }
-
-        function te() {
-            return K === O.Disposed
-        }
-
-        function ne() {
-            K !== O.New && K !== O.Listening || (K = O.Closed, V.fire(void 0))
-        }
-
-        function re() {
-            q || 0 === A.size || (q = (0, t.default)().timer.setImmediate((() => {
-                q = void 0,
-                    function() {
-                        if (0 === A.size) return;
-                        const e = A.shift();
-                        try {
-                            const t = null == g ? void 0 : g.messageStrategy;
-                            E.is(t) ? t.handleMessage(e, oe) : oe(e)
-                        } finally {
-                            re()
-                        }
-                    }()
-            })))
+    return ro.CancellationTokenSource = class {
+        get token() {
+            return this._token || (this._token = new s), this._token
+        }
+        cancel() {
+            this._token ? this._token.cancel() : this._token = r.Cancelled
+        }
+        dispose() {
+            this._token ? this._token instanceof s && this._token.dispose() : this._token = r.None
         }
+    }, ro
+}
+var io, so = {};
+var ao, co, lo = {},
+    uo = {};
 
-        function oe(e) {
-            r.Message.isRequest(e) ? function(e) {
-                if (te()) return;
+function ho() {
+    if (ao) return uo;
+    ao = 1, Object.defineProperty(uo, "__esModule", {
+        value: !0
+    }), uo.Semaphore = void 0;
+    const e = eo();
+    return uo.Semaphore = class {
+        constructor(e = 1) {
+            if (e <= 0) throw new Error("Capacity must be greater than 0");
+            this._capacity = e, this._active = 0, this._waiting = []
+        }
+        lock(e) {
+            return new Promise(((t, n) => {
+                this._waiting.push({
+                    thunk: e,
+                    resolve: t,
+                    reject: n
+                }), this.runNext()
+            }))
+        }
+        get active() {
+            return this._active
+        }
+        runNext() {
+            0 !== this._waiting.length && this._active !== this._capacity && (0, e.default)().timer.setImmediate((() => this.doRunNext()))
+        }
+        doRunNext() {
+            if (0 === this._waiting.length || this._active === this._capacity) return;
+            const e = this._waiting.shift();
+            if (this._active++, this._active > this._capacity) throw new Error("To many thunks active");
+            try {
+                const t = e.thunk();
+                t instanceof Promise ? t.then((t => {
+                    this._active--, e.resolve(t), this.runNext()
+                }), (t => {
+                    this._active--, e.reject(t), this.runNext()
+                })) : (this._active--, e.resolve(t), this.runNext())
+            } catch (Xu) {
+                this._active--, e.reject(Xu), this.runNext()
+            }
+        }
+    }, uo
+}
+var fo, po = {};
+var mo, go = {};
+var vo, yo, bo = {};
 
-                function t(t, n, o) {
-                    const i = {
-                        jsonrpc: T,
-                        id: e.id
-                    };
-                    t instanceof r.ResponseError ? i.error = t.toJson() : i.result = void 0 === t ? null : t, ae(i, n, o), f.write(i).catch((() => w.error("Sending response failed.")))
+function wo() {
+    return vo || (vo = 1, function(e) {
+        Object.defineProperty(e, "__esModule", {
+            value: !0
+        }), e.createMessageConnection = e.ConnectionOptions = e.MessageStrategy = e.CancellationStrategy = e.CancellationSenderStrategy = e.CancellationReceiverStrategy = e.RequestCancellationReceiverStrategy = e.IdCancellationReceiverStrategy = e.ConnectionStrategy = e.ConnectionError = e.ConnectionErrors = e.LogTraceNotification = e.SetTraceNotification = e.TraceFormat = e.TraceValues = e.Trace = e.NullLogger = e.ProgressType = e.ProgressToken = void 0;
+        const t = eo(),
+            n = Kr(),
+            r = Ur(),
+            o = zr(),
+            i = to(),
+            s = oo();
+        var a, c, l, u, d, h, f, p, m, g, v, y, b, w, C, x, k, R, T, S, M, D, _, E, P, O, N;
+        (a || (a = {})).type = new r.NotificationType("$/cancelRequest"), (c || (e.ProgressToken = c = {})).is = function(e) {
+            return "string" == typeof e || "number" == typeof e
+        }, (l || (l = {})).type = new r.NotificationType("$/progress");
+        e.ProgressType = class {
+                constructor() {}
+            }, (u || (u = {})).is = function(e) {
+                return n.func(e)
+            }, e.NullLogger = Object.freeze({
+                error: () => {},
+                warn: () => {},
+                info: () => {},
+                log: () => {}
+            }), (h = d || (e.Trace = d = {}))[h.Off = 0] = "Off", h[h.Messages = 1] = "Messages", h[h.Compact = 2] = "Compact", h[h.Verbose = 3] = "Verbose", (p = f || (e.TraceValues = f = {})).Off = "off", p.Messages = "messages", p.Compact = "compact", p.Verbose = "verbose",
+            function(e) {
+                e.fromString = function(t) {
+                    if (!n.string(t)) return e.Off;
+                    switch (t = t.toLowerCase()) {
+                        case "off":
+                        default:
+                            return e.Off;
+                        case "messages":
+                            return e.Messages;
+                        case "compact":
+                            return e.Compact;
+                        case "verbose":
+                            return e.Verbose
+                    }
+                }, e.toString = function(t) {
+                    switch (t) {
+                        case e.Off:
+                            return "off";
+                        case e.Messages:
+                            return "messages";
+                        case e.Compact:
+                            return "compact";
+                        case e.Verbose:
+                            return "verbose";
+                        default:
+                            return "off"
+                    }
                 }
-
-                function o(t, n, r) {
-                    const o = {
-                        jsonrpc: T,
-                        id: e.id,
-                        error: t.toJson()
-                    };
-                    ae(o, n, r), f.write(o).catch((() => w.error("Sending response failed.")))
+            }(d || (e.Trace = d = {})), (g = m || (e.TraceFormat = m = {})).Text = "text", g.JSON = "json",
+            function(e) {
+                e.fromString = function(t) {
+                    return n.string(t) && "json" === (t = t.toLowerCase()) ? e.JSON : e.Text
                 }
+            }(m || (e.TraceFormat = m = {})), (v || (e.SetTraceNotification = v = {})).type = new r.NotificationType("$/setTrace"), (y || (e.LogTraceNotification = y = {})).type = new r.NotificationType("$/logTrace"), (w = b || (e.ConnectionErrors = b = {}))[w.Closed = 1] = "Closed", w[w.Disposed = 2] = "Disposed", w[w.AlreadyListening = 3] = "AlreadyListening";
+        class j extends Error {
+            constructor(e, t) {
+                super(t), this.code = e, Object.setPrototypeOf(this, j.prototype)
+            }
+        }
+        e.ConnectionError = j, (C || (e.ConnectionStrategy = C = {})).is = function(e) {
+            const t = e;
+            return t && n.func(t.cancelUndispatched)
+        }, (x || (e.IdCancellationReceiverStrategy = x = {})).is = function(e) {
+            const t = e;
+            return t && (void 0 === t.kind || "id" === t.kind) && n.func(t.createCancellationTokenSource) && (void 0 === t.dispose || n.func(t.dispose))
+        }, (k || (e.RequestCancellationReceiverStrategy = k = {})).is = function(e) {
+            const t = e;
+            return t && "request" === t.kind && n.func(t.createCancellationTokenSource) && (void 0 === t.dispose || n.func(t.dispose))
+        }, (T = R || (e.CancellationReceiverStrategy = R = {})).Message = Object.freeze({
+            createCancellationTokenSource: e => new s.CancellationTokenSource
+        }), T.is = function(e) {
+            return x.is(e) || k.is(e)
+        }, (M = S || (e.CancellationSenderStrategy = S = {})).Message = Object.freeze({
+            sendCancellation: (e, t) => e.sendNotification(a.type, {
+                id: t
+            }),
+            cleanup(e) {}
+        }), M.is = function(e) {
+            const t = e;
+            return t && n.func(t.sendCancellation) && n.func(t.cleanup)
+        }, (_ = D || (e.CancellationStrategy = D = {})).Message = Object.freeze({
+            receiver: R.Message,
+            sender: S.Message
+        }), _.is = function(e) {
+            const t = e;
+            return t && R.is(t.receiver) && S.is(t.sender)
+        }, (E || (e.MessageStrategy = E = {})).is = function(e) {
+            const t = e;
+            return t && n.func(t.handleMessage)
+        }, (P || (e.ConnectionOptions = P = {})).is = function(e) {
+            const t = e;
+            return t && (D.is(t.cancellationStrategy) || C.is(t.connectionStrategy) || E.is(t.messageStrategy))
+        }, (N = O || (O = {}))[N.New = 1] = "New", N[N.Listening = 2] = "Listening", N[N.Closed = 3] = "Closed", N[N.Disposed = 4] = "Disposed", e.createMessageConnection = function(h, f, p, g) {
+            const w = void 0 !== p ? p : e.NullLogger;
+            let C = 0,
+                k = 0,
+                R = 0;
+            const T = "2.0";
+            let S;
+            const M = new Map;
+            let _;
+            const P = new Map,
+                N = new Map;
+            let q, L, A = new o.LinkedMap,
+                I = new Map,
+                B = new Set,
+                F = new Map,
+                W = d.Off,
+                H = m.Text,
+                K = O.New;
+            const U = new i.Emitter,
+                V = new i.Emitter,
+                $ = new i.Emitter,
+                z = new i.Emitter,
+                J = new i.Emitter,
+                Q = g && g.cancellationStrategy ? g.cancellationStrategy : D.Message;
+
+            function G(e) {
+                if (null === e) throw new Error("Can't send requests with id null since the response can't be correlated.");
+                return "req-" + e.toString()
+            }
+
+            function X(e, t) {
+                var n;
+                r.Message.isRequest(t) ? e.set(G(t.id), t) : r.Message.isResponse(t) ? e.set(null === (n = t.id) ? "res-unknown-" + (++R).toString() : "res-" + n.toString(), t) : e.set("not-" + (++k).toString(), t)
+            }
+
+            function Z(e) {}
+
+            function Y() {
+                return K === O.Listening
+            }
+
+            function ee() {
+                return K === O.Closed
+            }
+
+            function te() {
+                return K === O.Disposed
+            }
+
+            function ne() {
+                K !== O.New && K !== O.Listening || (K = O.Closed, V.fire(void 0))
+            }
+
+            function re() {
+                q || 0 === A.size || (q = (0, t.default)().timer.setImmediate((() => {
+                    q = void 0,
+                        function() {
+                            if (0 === A.size) return;
+                            const e = A.shift();
+                            try {
+                                const t = null == g ? void 0 : g.messageStrategy;
+                                E.is(t) ? t.handleMessage(e, oe) : oe(e)
+                            } finally {
+                                re()
+                            }
+                        }()
+                })))
+            }
 
-                function i(t, n, r) {
-                    void 0 === t && (t = null);
-                    const o = {
-                        jsonrpc: T,
-                        id: e.id,
-                        result: t
-                    };
-                    ae(o, n, r), f.write(o).catch((() => w.error("Sending response failed.")))
-                }! function(e) {
-                    if (W === d.Off || !L) return;
-                    if (H === m.Text) {
-                        let t;
-                        W !== d.Verbose && W !== d.Compact || !e.params || (t = `Params: ${se(e.params)}\n\n`), L.log(`Received request '${e.method} - (${e.id})'.`, t)
-                    } else le("receive-request", e)
-                }(e);
-                const s = M.get(e.method);
-                let a, c;
-                s && (a = s.type, c = s.handler);
-                const l = Date.now();
-                if (c || S) {
-                    const s = e.id ?? String(Date.now()),
-                        d = x.is(Q.receiver) ? Q.receiver.createCancellationTokenSource(s) : Q.receiver.createCancellationTokenSource(e);
-                    null !== e.id && B.has(e.id) && d.cancel(), null !== e.id && F.set(s, d);
-                    try {
-                        let u;
-                        if (c)
-                            if (void 0 === e.params) {
-                                if (void 0 !== a && 0 !== a.numberOfParams) return void o(new r.ResponseError(r.ErrorCodes.InvalidParams, `Request ${e.method} defines ${a.numberOfParams} params but received none.`), e.method, l);
-                                u = c(d.token)
-                            } else if (Array.isArray(e.params)) {
-                            if (void 0 !== a && a.parameterStructures === r.ParameterStructures.byName) return void o(new r.ResponseError(r.ErrorCodes.InvalidParams, `Request ${e.method} defines parameters by name but received parameters by position`), e.method, l);
-                            u = c(...e.params, d.token)
-                        } else {
-                            if (void 0 !== a && a.parameterStructures === r.ParameterStructures.byPosition) return void o(new r.ResponseError(r.ErrorCodes.InvalidParams, `Request ${e.method} defines parameters by position but received parameters by name`), e.method, l);
-                            u = c(e.params, d.token)
-                        } else S && (u = S(e.method, e.params, d.token));
-                        const h = u;
-                        u ? h.then ? h.then((n => {
-                            F.delete(s), t(n, e.method, l)
-                        }), (t => {
-                            F.delete(s), t instanceof r.ResponseError ? o(t, e.method, l) : t && n.string(t.message) ? o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed with message: ${t.message}`), e.method, l) : o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed unexpectedly without providing any details.`), e.method, l)
-                        })) : (F.delete(s), t(u, e.method, l)) : (F.delete(s), i(u, e.method, l))
-                    } catch (u) {
-                        F.delete(s), u instanceof r.ResponseError ? t(u, e.method, l) : u && n.string(u.message) ? o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed with message: ${u.message}`), e.method, l) : o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed unexpectedly without providing any details.`), e.method, l)
-                    }
-                } else o(new r.ResponseError(r.ErrorCodes.MethodNotFound, `Unhandled method ${e.method}`), e.method, l)
-            }(e) : r.Message.isNotification(e) ? function(e) {
-                if (te()) return;
-                let t, n;
-                if (e.method === a.type.method) {
-                    const t = e.params.id;
-                    return B.delete(t), void ce(e)
-                } {
-                    const r = P.get(e.method);
-                    r && (n = r.handler, t = r.type)
-                }
-                if (n || _) try {
-                    if (ce(e), n)
-                        if (void 0 === e.params) void 0 !== t && 0 !== t.numberOfParams && t.parameterStructures !== r.ParameterStructures.byName && w.error(`Notification ${e.method} defines ${t.numberOfParams} params but received none.`), n();
-                        else if (Array.isArray(e.params)) {
-                        const o = e.params;
-                        e.method === l.type.method && 2 === o.length && c.is(o[0]) ? n({
-                            token: o[0],
-                            value: o[1]
-                        }) : (void 0 !== t && (t.parameterStructures === r.ParameterStructures.byName && w.error(`Notification ${e.method} defines parameters by name but received parameters by position`), t.numberOfParams !== e.params.length && w.error(`Notification ${e.method} defines ${t.numberOfParams} params but received ${o.length} arguments`)), n(...o))
-                    } else void 0 !== t && t.parameterStructures === r.ParameterStructures.byPosition && w.error(`Notification ${e.method} defines parameters by position but received parameters by name`), n(e.params);
-                    else _ && _(e.method, e.params)
-                } catch (o) {
-                    o.message ? w.error(`Notification handler '${e.method}' failed with message: ${o.message}`) : w.error(`Notification handler '${e.method}' failed unexpectedly.`)
-                } else $.fire(e)
-            }(e) : r.Message.isResponse(e) ? function(e) {
-                if (te()) return;
-                if (null === e.id) e.error ? w.error(`Received response message without id: Error is: \n${JSON.stringify(e.error,void 0,4)}`) : w.error("Received response message without id. No further error information provided.");
-                else {
-                    const n = e.id,
-                        o = I.get(n);
-                    if (function(e, t) {
-                            if (W === d.Off || !L) return;
-                            if (H === m.Text) {
-                                let n;
-                                if (W !== d.Verbose && W !== d.Compact || (e.error && e.error.data ? n = `Error data: ${se(e.error.data)}\n\n` : e.result ? n = `Result: ${se(e.result)}\n\n` : void 0 === e.error && (n = "No result returned.\n\n")), t) {
-                                    const r = e.error ? ` Request failed: ${e.error.message} (${e.error.code}).` : "";
-                                    L.log(`Received response '${t.method} - (${e.id})' in ${Date.now()-t.timerStart}ms.${r}`, n)
-                                } else L.log(`Received response ${e.id} without active response promise.`, n)
-                            } else le("receive-response", e)
-                        }(e, o), void 0 !== o) {
-                        I.delete(n);
+            function oe(e) {
+                r.Message.isRequest(e) ? function(e) {
+                    if (te()) return;
+
+                    function t(t, n, o) {
+                        const i = {
+                            jsonrpc: T,
+                            id: e.id
+                        };
+                        t instanceof r.ResponseError ? i.error = t.toJson() : i.result = void 0 === t ? null : t, ae(i, n, o), f.write(i).catch((() => w.error("Sending response failed.")))
+                    }
+
+                    function o(t, n, r) {
+                        const o = {
+                            jsonrpc: T,
+                            id: e.id,
+                            error: t.toJson()
+                        };
+                        ae(o, n, r), f.write(o).catch((() => w.error("Sending response failed.")))
+                    }
+
+                    function i(t, n, r) {
+                        void 0 === t && (t = null);
+                        const o = {
+                            jsonrpc: T,
+                            id: e.id,
+                            result: t
+                        };
+                        ae(o, n, r), f.write(o).catch((() => w.error("Sending response failed.")))
+                    }! function(e) {
+                        if (W === d.Off || !L) return;
+                        if (H === m.Text) {
+                            let t;
+                            W !== d.Verbose && W !== d.Compact || !e.params || (t = `Params: ${se(e.params)}\n\n`), L.log(`Received request '${e.method} - (${e.id})'.`, t)
+                        } else le("receive-request", e)
+                    }(e);
+                    const s = M.get(e.method);
+                    let a, c;
+                    s && (a = s.type, c = s.handler);
+                    const l = Date.now();
+                    if (c || S) {
+                        const s = e.id ?? String(Date.now()),
+                            d = x.is(Q.receiver) ? Q.receiver.createCancellationTokenSource(s) : Q.receiver.createCancellationTokenSource(e);
+                        null !== e.id && B.has(e.id) && d.cancel(), null !== e.id && F.set(s, d);
                         try {
-                            if (e.error) {
-                                const t = e.error;
-                                o.reject(new r.ResponseError(t.code, t.message, t.data))
+                            let u;
+                            if (c)
+                                if (void 0 === e.params) {
+                                    if (void 0 !== a && 0 !== a.numberOfParams) return void o(new r.ResponseError(r.ErrorCodes.InvalidParams, `Request ${e.method} defines ${a.numberOfParams} params but received none.`), e.method, l);
+                                    u = c(d.token)
+                                } else if (Array.isArray(e.params)) {
+                                if (void 0 !== a && a.parameterStructures === r.ParameterStructures.byName) return void o(new r.ResponseError(r.ErrorCodes.InvalidParams, `Request ${e.method} defines parameters by name but received parameters by position`), e.method, l);
+                                u = c(...e.params, d.token)
                             } else {
-                                if (void 0 === e.result) throw new Error("Should never happen.");
-                                o.resolve(e.result)
+                                if (void 0 !== a && a.parameterStructures === r.ParameterStructures.byPosition) return void o(new r.ResponseError(r.ErrorCodes.InvalidParams, `Request ${e.method} defines parameters by position but received parameters by name`), e.method, l);
+                                u = c(e.params, d.token)
+                            } else S && (u = S(e.method, e.params, d.token));
+                            const h = u;
+                            u ? h.then ? h.then((n => {
+                                F.delete(s), t(n, e.method, l)
+                            }), (t => {
+                                F.delete(s), t instanceof r.ResponseError ? o(t, e.method, l) : t && n.string(t.message) ? o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed with message: ${t.message}`), e.method, l) : o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed unexpectedly without providing any details.`), e.method, l)
+                            })) : (F.delete(s), t(u, e.method, l)) : (F.delete(s), i(u, e.method, l))
+                        } catch (u) {
+                            F.delete(s), u instanceof r.ResponseError ? t(u, e.method, l) : u && n.string(u.message) ? o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed with message: ${u.message}`), e.method, l) : o(new r.ResponseError(r.ErrorCodes.InternalError, `Request ${e.method} failed unexpectedly without providing any details.`), e.method, l)
+                        }
+                    } else o(new r.ResponseError(r.ErrorCodes.MethodNotFound, `Unhandled method ${e.method}`), e.method, l)
+                }(e) : r.Message.isNotification(e) ? function(e) {
+                    if (te()) return;
+                    let t, n;
+                    if (e.method === a.type.method) {
+                        const t = e.params.id;
+                        return B.delete(t), void ce(e)
+                    } {
+                        const r = P.get(e.method);
+                        r && (n = r.handler, t = r.type)
+                    }
+                    if (n || _) try {
+                        if (ce(e), n)
+                            if (void 0 === e.params) void 0 !== t && 0 !== t.numberOfParams && t.parameterStructures !== r.ParameterStructures.byName && w.error(`Notification ${e.method} defines ${t.numberOfParams} params but received none.`), n();
+                            else if (Array.isArray(e.params)) {
+                            const o = e.params;
+                            e.method === l.type.method && 2 === o.length && c.is(o[0]) ? n({
+                                token: o[0],
+                                value: o[1]
+                            }) : (void 0 !== t && (t.parameterStructures === r.ParameterStructures.byName && w.error(`Notification ${e.method} defines parameters by name but received parameters by position`), t.numberOfParams !== e.params.length && w.error(`Notification ${e.method} defines ${t.numberOfParams} params but received ${o.length} arguments`)), n(...o))
+                        } else void 0 !== t && t.parameterStructures === r.ParameterStructures.byPosition && w.error(`Notification ${e.method} defines parameters by position but received parameters by name`), n(e.params);
+                        else _ && _(e.method, e.params)
+                    } catch (o) {
+                        o.message ? w.error(`Notification handler '${e.method}' failed with message: ${o.message}`) : w.error(`Notification handler '${e.method}' failed unexpectedly.`)
+                    } else $.fire(e)
+                }(e) : r.Message.isResponse(e) ? function(e) {
+                    if (te()) return;
+                    if (null === e.id) e.error ? w.error(`Received response message without id: Error is: \n${JSON.stringify(e.error,void 0,4)}`) : w.error("Received response message without id. No further error information provided.");
+                    else {
+                        const n = e.id,
+                            o = I.get(n);
+                        if (function(e, t) {
+                                if (W === d.Off || !L) return;
+                                if (H === m.Text) {
+                                    let n;
+                                    if (W !== d.Verbose && W !== d.Compact || (e.error && e.error.data ? n = `Error data: ${se(e.error.data)}\n\n` : e.result ? n = `Result: ${se(e.result)}\n\n` : void 0 === e.error && (n = "No result returned.\n\n")), t) {
+                                        const r = e.error ? ` Request failed: ${e.error.message} (${e.error.code}).` : "";
+                                        L.log(`Received response '${t.method} - (${e.id})' in ${Date.now()-t.timerStart}ms.${r}`, n)
+                                    } else L.log(`Received response ${e.id} without active response promise.`, n)
+                                } else le("receive-response", e)
+                            }(e, o), void 0 !== o) {
+                            I.delete(n);
+                            try {
+                                if (e.error) {
+                                    const t = e.error;
+                                    o.reject(new r.ResponseError(t.code, t.message, t.data))
+                                } else {
+                                    if (void 0 === e.result) throw new Error("Should never happen.");
+                                    o.resolve(e.result)
+                                }
+                            } catch (t) {
+                                t.message ? w.error(`Response handler '${o.method}' failed with message: ${t.message}`) : w.error(`Response handler '${o.method}' failed unexpectedly.`)
                             }
-                        } catch (t) {
-                            t.message ? w.error(`Response handler '${o.method}' failed with message: ${t.message}`) : w.error(`Response handler '${o.method}' failed unexpectedly.`)
                         }
                     }
+                }(e) : function(e) {
+                    if (!e) return void w.error("Received empty message.");
+                    w.error(`Received message which is neither a response nor a notification message:\n${JSON.stringify(e,null,4)}`);
+                    const t = e;
+                    if (n.string(t.id) || n.number(t.id)) {
+                        const e = t.id,
+                            n = I.get(e);
+                        n && n.reject(new Error("The received response has neither a result nor an error property."))
+                    }
+                }(e)
+            }
+            h.onClose(ne), h.onError((function(e) {
+                U.fire([e, void 0, void 0])
+            })), f.onClose(ne), f.onError((function(e) {
+                U.fire(e)
+            }));
+            const ie = e => {
+                try {
+                    if (r.Message.isNotification(e) && e.method === a.type.method) {
+                        const t = e.params.id,
+                            n = G(t),
+                            o = A.get(n);
+                        if (r.Message.isRequest(o)) {
+                            const r = null == g ? void 0 : g.connectionStrategy,
+                                i = r && r.cancelUndispatched ? r.cancelUndispatched(o, Z) : void 0;
+                            if (i && (void 0 !== i.error || void 0 !== i.result)) return A.delete(n), F.delete(t), i.id = o.id, ae(i, e.method, Date.now()), void f.write(i).catch((() => w.error("Sending response for canceled message failed.")))
+                        }
+                        const i = F.get(t);
+                        if (void 0 !== i) return i.cancel(), void ce(e);
+                        B.add(t)
+                    }
+                    X(A, e)
+                } finally {
+                    re()
+                }
+            };
+
+            function se(e) {
+                if (null != e) switch (W) {
+                    case d.Verbose:
+                        return JSON.stringify(e, null, 4);
+                    case d.Compact:
+                        return JSON.stringify(e);
+                    default:
+                        return
                 }
-            }(e) : function(e) {
-                if (!e) return void w.error("Received empty message.");
-                w.error(`Received message which is neither a response nor a notification message:\n${JSON.stringify(e,null,4)}`);
-                const t = e;
-                if (n.string(t.id) || n.number(t.id)) {
-                    const e = t.id,
-                        n = I.get(e);
-                    n && n.reject(new Error("The received response has neither a result nor an error property."))
-                }
-            }(e)
-        }
-        h.onClose(ne), h.onError((function(e) {
-            U.fire([e, void 0, void 0])
-        })), f.onClose(ne), f.onError((function(e) {
-            U.fire(e)
-        }));
-        const ie = e => {
-            try {
-                if (r.Message.isNotification(e) && e.method === a.type.method) {
-                    const t = e.params.id,
-                        n = G(t),
-                        o = A.get(n);
-                    if (r.Message.isRequest(o)) {
-                        const r = null == g ? void 0 : g.connectionStrategy,
-                            i = r && r.cancelUndispatched ? r.cancelUndispatched(o, Z) : void 0;
-                        if (i && (void 0 !== i.error || void 0 !== i.result)) return A.delete(n), F.delete(t), i.id = o.id, ae(i, e.method, Date.now()), void f.write(i).catch((() => w.error("Sending response for canceled message failed.")))
-                    }
-                    const i = F.get(t);
-                    if (void 0 !== i) return i.cancel(), void ce(e);
-                    B.add(t)
-                }
-                X(A, e)
-            } finally {
-                re()
             }
-        };
 
-        function se(e) {
-            if (null != e) switch (W) {
-                case d.Verbose:
-                    return JSON.stringify(e, null, 4);
-                case d.Compact:
-                    return JSON.stringify(e);
-                default:
-                    return
+            function ae(e, t, n) {
+                if (W !== d.Off && L)
+                    if (H === m.Text) {
+                        let r;
+                        W !== d.Verbose && W !== d.Compact || (e.error && e.error.data ? r = `Error data: ${se(e.error.data)}\n\n` : e.result ? r = `Result: ${se(e.result)}\n\n` : void 0 === e.error && (r = "No result returned.\n\n")), L.log(`Sending response '${t} - (${e.id})'. Processing request took ${Date.now()-n}ms`, r)
+                    } else le("send-response", e)
             }
-        }
 
-        function ae(e, t, n) {
-            if (W !== d.Off && L)
-                if (H === m.Text) {
-                    let r;
-                    W !== d.Verbose && W !== d.Compact || (e.error && e.error.data ? r = `Error data: ${se(e.error.data)}\n\n` : e.result ? r = `Result: ${se(e.result)}\n\n` : void 0 === e.error && (r = "No result returned.\n\n")), L.log(`Sending response '${t} - (${e.id})'. Processing request took ${Date.now()-n}ms`, r)
-                } else le("send-response", e)
-        }
+            function ce(e) {
+                if (W !== d.Off && L && e.method !== y.type.method)
+                    if (H === m.Text) {
+                        let t;
+                        W !== d.Verbose && W !== d.Compact || (t = e.params ? `Params: ${se(e.params)}\n\n` : "No parameters provided.\n\n"), L.log(`Received notification '${e.method}'.`, t)
+                    } else le("receive-notification", e)
+            }
 
-        function ce(e) {
-            if (W !== d.Off && L && e.method !== y.type.method)
-                if (H === m.Text) {
-                    let t;
-                    W !== d.Verbose && W !== d.Compact || (t = e.params ? `Params: ${se(e.params)}\n\n` : "No parameters provided.\n\n"), L.log(`Received notification '${e.method}'.`, t)
-                } else le("receive-notification", e)
-        }
+            function le(e, t) {
+                if (!L || W === d.Off) return;
+                const n = {
+                    isLSPMessage: !0,
+                    type: e,
+                    message: t,
+                    timestamp: Date.now()
+                };
+                L.log(n)
+            }
 
-        function le(e, t) {
-            if (!L || W === d.Off) return;
-            const n = {
-                isLSPMessage: !0,
-                type: e,
-                message: t,
-                timestamp: Date.now()
-            };
-            L.log(n)
-        }
+            function ue() {
+                if (ee()) throw new j(b.Closed, "Connection is closed.");
+                if (te()) throw new j(b.Disposed, "Connection is disposed.")
+            }
 
-        function ue() {
-            if (ee()) throw new j(b.Closed, "Connection is closed.");
-            if (te()) throw new j(b.Disposed, "Connection is disposed.")
-        }
+            function de(e) {
+                return void 0 === e ? null : e
+            }
 
-        function de(e) {
-            return void 0 === e ? null : e
-        }
+            function he(e) {
+                return null === e ? void 0 : e
+            }
 
-        function he(e) {
-            return null === e ? void 0 : e
-        }
+            function fe(e) {
+                return null != e && !Array.isArray(e) && "object" == typeof e
+            }
 
-        function fe(e) {
-            return null != e && !Array.isArray(e) && "object" == typeof e
-        }
+            function pe(e, t) {
+                switch (e) {
+                    case r.ParameterStructures.auto:
+                        return fe(t) ? he(t) : [de(t)];
+                    case r.ParameterStructures.byName:
+                        if (!fe(t)) throw new Error("Received parameters by name but param is not an object literal.");
+                        return he(t);
+                    case r.ParameterStructures.byPosition:
+                        return [de(t)];
+                    default:
+                        throw new Error(`Unknown parameter structure ${e.toString()}`)
+                }
+            }
 
-        function pe(e, t) {
-            switch (e) {
-                case r.ParameterStructures.auto:
-                    return fe(t) ? he(t) : [de(t)];
-                case r.ParameterStructures.byName:
-                    if (!fe(t)) throw new Error("Received parameters by name but param is not an object literal.");
-                    return he(t);
-                case r.ParameterStructures.byPosition:
-                    return [de(t)];
-                default:
-                    throw new Error(`Unknown parameter structure ${e.toString()}`)
+            function me(e, t) {
+                let n;
+                const r = e.numberOfParams;
+                switch (r) {
+                    case 0:
+                        n = void 0;
+                        break;
+                    case 1:
+                        n = pe(e.parameterStructures, t[0]);
+                        break;
+                    default:
+                        n = [];
+                        for (let e = 0; e < t.length && e < r; e++) n.push(de(t[e]));
+                        if (t.length < r)
+                            for (let e = t.length; e < r; e++) n.push(null)
+                }
+                return n
             }
+            const ge = {
+                sendNotification: (e, ...t) => {
+                    let o, i;
+                    if (ue(), n.string(e)) {
+                        o = e;
+                        const n = t[0];
+                        let s = 0,
+                            a = r.ParameterStructures.auto;
+                        r.ParameterStructures.is(n) && (s = 1, a = n);
+                        let c = t.length;
+                        const l = c - s;
+                        switch (l) {
+                            case 0:
+                                i = void 0;
+                                break;
+                            case 1:
+                                i = pe(a, t[s]);
+                                break;
+                            default:
+                                if (a === r.ParameterStructures.byName) throw new Error(`Received ${l} parameters for 'by Name' notification parameter structure.`);
+                                i = t.slice(s, c).map((e => de(e)))
+                        }
+                    } else {
+                        const n = t;
+                        o = e.method, i = me(e, n)
+                    }
+                    const s = {
+                        jsonrpc: T,
+                        method: o,
+                        params: i
+                    };
+                    return function(e) {
+                        if (W !== d.Off && L)
+                            if (H === m.Text) {
+                                let t;
+                                W !== d.Verbose && W !== d.Compact || (t = e.params ? `Params: ${se(e.params)}\n\n` : "No parameters provided.\n\n"), L.log(`Sending notification '${e.method}'.`, t)
+                            } else le("send-notification", e)
+                    }(s), f.write(s).catch((e => {
+                        throw w.error("Sending notification failed."), e
+                    }))
+                },
+                onNotification: (e, t) => {
+                    let r;
+                    return ue(), n.func(e) ? _ = e : t && (n.string(e) ? (r = e, P.set(e, {
+                        type: void 0,
+                        handler: t
+                    })) : (r = e.method, P.set(e.method, {
+                        type: e,
+                        handler: t
+                    }))), {
+                        dispose: () => {
+                            void 0 !== r ? P.delete(r) : _ = void 0
+                        }
+                    }
+                },
+                onProgress: (e, t, n) => {
+                    if (N.has(t)) throw new Error(`Progress handler for token ${t} already registered`);
+                    return N.set(t, n), {
+                        dispose: () => {
+                            N.delete(t)
+                        }
+                    }
+                },
+                sendProgress: (e, t, n) => ge.sendNotification(l.type, {
+                    token: t,
+                    value: n
+                }),
+                onUnhandledProgress: z.event,
+                sendRequest: (e, ...t) => {
+                    let o, i, a;
+                    if (ue(), function() {
+                            if (!Y()) throw new Error("Call listen() first.")
+                        }(), n.string(e)) {
+                        o = e;
+                        const n = t[0],
+                            c = t[t.length - 1];
+                        let l = 0,
+                            u = r.ParameterStructures.auto;
+                        r.ParameterStructures.is(n) && (l = 1, u = n);
+                        let d = t.length;
+                        s.CancellationToken.is(c) && (d -= 1, a = c);
+                        const h = d - l;
+                        switch (h) {
+                            case 0:
+                                i = void 0;
+                                break;
+                            case 1:
+                                i = pe(u, t[l]);
+                                break;
+                            default:
+                                if (u === r.ParameterStructures.byName) throw new Error(`Received ${h} parameters for 'by Name' request parameter structure.`);
+                                i = t.slice(l, d).map((e => de(e)))
+                        }
+                    } else {
+                        const n = t;
+                        o = e.method, i = me(e, n);
+                        const r = e.numberOfParams;
+                        a = s.CancellationToken.is(n[r]) ? n[r] : void 0
+                    }
+                    const c = C++;
+                    let l;
+                    a && (l = a.onCancellationRequested((() => {
+                        const e = Q.sender.sendCancellation(ge, c);
+                        return void 0 === e ? (w.log(`Received no promise from cancellation strategy when cancelling id ${c}`), Promise.resolve()) : e.catch((() => {
+                            w.log(`Sending cancellation messages for id ${c} failed`)
+                        }))
+                    })));
+                    const u = {
+                        jsonrpc: T,
+                        id: c,
+                        method: o,
+                        params: i
+                    };
+                    return function(e) {
+                        if (W !== d.Off && L)
+                            if (H === m.Text) {
+                                let t;
+                                W !== d.Verbose && W !== d.Compact || !e.params || (t = `Params: ${se(e.params)}\n\n`), L.log(`Sending request '${e.method} - (${e.id})'.`, t)
+                            } else le("send-request", e)
+                    }(u), "function" == typeof Q.sender.enableCancellation && Q.sender.enableCancellation(u), new Promise((async (e, t) => {
+                        const n = {
+                            method: o,
+                            timerStart: Date.now(),
+                            resolve: t => {
+                                e(t), Q.sender.cleanup(c), null == l || l.dispose()
+                            },
+                            reject: e => {
+                                t(e), Q.sender.cleanup(c), null == l || l.dispose()
+                            }
+                        };
+                        try {
+                            await f.write(u), I.set(c, n)
+                        } catch (i) {
+                            throw w.error("Sending request failed."), n.reject(new r.ResponseError(r.ErrorCodes.MessageWriteError, i.message ? i.message : "Unknown reason")), i
+                        }
+                    }))
+                },
+                onRequest: (e, t) => {
+                    ue();
+                    let r = null;
+                    return u.is(e) ? (r = void 0, S = e) : n.string(e) ? (r = null, void 0 !== t && (r = e, M.set(e, {
+                        handler: t,
+                        type: void 0
+                    }))) : void 0 !== t && (r = e.method, M.set(e.method, {
+                        type: e,
+                        handler: t
+                    })), {
+                        dispose: () => {
+                            null !== r && (void 0 !== r ? M.delete(r) : S = void 0)
+                        }
+                    }
+                },
+                hasPendingResponse: () => I.size > 0,
+                trace: async (e, t, r) => {
+                    let o = !1,
+                        i = m.Text;
+                    void 0 !== r && (n.boolean(r) ? o = r : (o = r.sendNotification || !1, i = r.traceFormat || m.Text)), W = e, H = i, L = W === d.Off ? void 0 : t, !o || ee() || te() || await ge.sendNotification(v.type, {
+                        value: d.toString(e)
+                    })
+                },
+                onError: U.event,
+                onClose: V.event,
+                onUnhandledNotification: $.event,
+                onDispose: J.event,
+                end: () => {
+                    f.end()
+                },
+                dispose: () => {
+                    if (te()) return;
+                    K = O.Disposed, J.fire(void 0);
+                    const e = new r.ResponseError(r.ErrorCodes.PendingResponseRejected, "Pending response rejected since connection got disposed");
+                    for (const t of I.values()) t.reject(e);
+                    I = new Map, F = new Map, B = new Set, A = new o.LinkedMap, n.func(f.dispose) && f.dispose(), n.func(h.dispose) && h.dispose()
+                },
+                listen: () => {
+                    ue(),
+                        function() {
+                            if (Y()) throw new j(b.AlreadyListening, "Connection is already listening")
+                        }(), K = O.Listening, h.listen(ie)
+                },
+                inspect: () => {
+                    (0, t.default)().console.log("inspect")
+                }
+            };
+            return ge.onNotification(y.type, (e => {
+                if (W === d.Off || !L) return;
+                const t = W === d.Verbose || W === d.Compact;
+                L.log(e.message, t ? e.verbose : void 0)
+            })), ge.onNotification(l.type, (e => {
+                const t = N.get(e.token);
+                t ? t(e.value) : z.fire(e)
+            })), ge
         }
+    }(bo)), bo
+}
 
-        function me(e, t) {
-            let n;
-            const r = e.numberOfParams;
-            switch (r) {
-                case 0:
-                    n = void 0;
-                    break;
-                case 1:
-                    n = pe(e.parameterStructures, t[0]);
-                    break;
-                default:
-                    n = [];
-                    for (let e = 0; e < t.length && e < r; e++) n.push(de(t[e]));
-                    if (t.length < r)
-                        for (let e = t.length; e < r; e++) n.push(null)
+function Co() {
+    return yo || (yo = 1, function(e) {
+        Object.defineProperty(e, "__esModule", {
+            value: !0
+        }), e.ProgressType = e.ProgressToken = e.createMessageConnection = e.NullLogger = e.ConnectionOptions = e.ConnectionStrategy = e.AbstractMessageBuffer = e.WriteableStreamMessageWriter = e.AbstractMessageWriter = e.MessageWriter = e.ReadableStreamMessageReader = e.AbstractMessageReader = e.MessageReader = e.SharedArrayReceiverStrategy = e.SharedArraySenderStrategy = e.CancellationToken = e.CancellationTokenSource = e.Emitter = e.Event = e.Disposable = e.LRUCache = e.Touch = e.LinkedMap = e.ParameterStructures = e.NotificationType9 = e.NotificationType8 = e.NotificationType7 = e.NotificationType6 = e.NotificationType5 = e.NotificationType4 = e.NotificationType3 = e.NotificationType2 = e.NotificationType1 = e.NotificationType0 = e.NotificationType = e.ErrorCodes = e.ResponseError = e.RequestType9 = e.RequestType8 = e.RequestType7 = e.RequestType6 = e.RequestType5 = e.RequestType4 = e.RequestType3 = e.RequestType2 = e.RequestType1 = e.RequestType0 = e.RequestType = e.Message = e.RAL = void 0, e.MessageStrategy = e.CancellationStrategy = e.CancellationSenderStrategy = e.CancellationReceiverStrategy = e.ConnectionError = e.ConnectionErrors = e.LogTraceNotification = e.SetTraceNotification = e.TraceFormat = e.TraceValues = e.Trace = void 0;
+        const t = Ur();
+        Object.defineProperty(e, "Message", {
+            enumerable: !0,
+            get: function() {
+                return t.Message
             }
-            return n
-        }
-        const ge = {
-            sendNotification: (e, ...t) => {
-                let o, i;
-                if (ue(), n.string(e)) {
-                    o = e;
-                    const n = t[0];
-                    let s = 0,
-                        a = r.ParameterStructures.auto;
-                    r.ParameterStructures.is(n) && (s = 1, a = n);
-                    let c = t.length;
-                    const l = c - s;
-                    switch (l) {
-                        case 0:
-                            i = void 0;
-                            break;
-                        case 1:
-                            i = pe(a, t[s]);
-                            break;
-                        default:
-                            if (a === r.ParameterStructures.byName) throw new Error(`Received ${l} parameters for 'by Name' notification parameter structure.`);
-                            i = t.slice(s, c).map((e => de(e)))
-                    }
-                } else {
-                    const n = t;
-                    o = e.method, i = me(e, n)
+        }), Object.defineProperty(e, "RequestType", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType
+            }
+        }), Object.defineProperty(e, "RequestType0", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType0
+            }
+        }), Object.defineProperty(e, "RequestType1", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType1
+            }
+        }), Object.defineProperty(e, "RequestType2", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType2
+            }
+        }), Object.defineProperty(e, "RequestType3", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType3
+            }
+        }), Object.defineProperty(e, "RequestType4", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType4
+            }
+        }), Object.defineProperty(e, "RequestType5", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType5
+            }
+        }), Object.defineProperty(e, "RequestType6", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType6
+            }
+        }), Object.defineProperty(e, "RequestType7", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType7
+            }
+        }), Object.defineProperty(e, "RequestType8", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType8
+            }
+        }), Object.defineProperty(e, "RequestType9", {
+            enumerable: !0,
+            get: function() {
+                return t.RequestType9
+            }
+        }), Object.defineProperty(e, "ResponseError", {
+            enumerable: !0,
+            get: function() {
+                return t.ResponseError
+            }
+        }), Object.defineProperty(e, "ErrorCodes", {
+            enumerable: !0,
+            get: function() {
+                return t.ErrorCodes
+            }
+        }), Object.defineProperty(e, "NotificationType", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType
+            }
+        }), Object.defineProperty(e, "NotificationType0", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType0
+            }
+        }), Object.defineProperty(e, "NotificationType1", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType1
+            }
+        }), Object.defineProperty(e, "NotificationType2", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType2
+            }
+        }), Object.defineProperty(e, "NotificationType3", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType3
+            }
+        }), Object.defineProperty(e, "NotificationType4", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType4
+            }
+        }), Object.defineProperty(e, "NotificationType5", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType5
+            }
+        }), Object.defineProperty(e, "NotificationType6", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType6
+            }
+        }), Object.defineProperty(e, "NotificationType7", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType7
+            }
+        }), Object.defineProperty(e, "NotificationType8", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType8
+            }
+        }), Object.defineProperty(e, "NotificationType9", {
+            enumerable: !0,
+            get: function() {
+                return t.NotificationType9
+            }
+        }), Object.defineProperty(e, "ParameterStructures", {
+            enumerable: !0,
+            get: function() {
+                return t.ParameterStructures
+            }
+        });
+        const n = zr();
+        Object.defineProperty(e, "LinkedMap", {
+            enumerable: !0,
+            get: function() {
+                return n.LinkedMap
+            }
+        }), Object.defineProperty(e, "LRUCache", {
+            enumerable: !0,
+            get: function() {
+                return n.LRUCache
+            }
+        }), Object.defineProperty(e, "Touch", {
+            enumerable: !0,
+            get: function() {
+                return n.Touch
+            }
+        });
+        const r = (Jr || (Jr = 1, Object.defineProperty(Qr, "__esModule", {
+            value: !0
+        }), Qr.Disposable = void 0, (o || (Qr.Disposable = o = {})).create = function(e) {
+            return {
+                dispose: e
+            }
+        }), Qr);
+        var o;
+        Object.defineProperty(e, "Disposable", {
+            enumerable: !0,
+            get: function() {
+                return r.Disposable
+            }
+        });
+        const i = to();
+        Object.defineProperty(e, "Event", {
+            enumerable: !0,
+            get: function() {
+                return i.Event
+            }
+        }), Object.defineProperty(e, "Emitter", {
+            enumerable: !0,
+            get: function() {
+                return i.Emitter
+            }
+        });
+        const s = oo();
+        Object.defineProperty(e, "CancellationTokenSource", {
+            enumerable: !0,
+            get: function() {
+                return s.CancellationTokenSource
+            }
+        }), Object.defineProperty(e, "CancellationToken", {
+            enumerable: !0,
+            get: function() {
+                return s.CancellationToken
+            }
+        });
+        const a = function() {
+            if (io) return so;
+            io = 1, Object.defineProperty(so, "__esModule", {
+                value: !0
+            }), so.SharedArrayReceiverStrategy = so.SharedArraySenderStrategy = void 0;
+            const e = oo();
+            var t, n;
+            (n = t || (t = {})).Continue = 0, n.Cancelled = 1, so.SharedArraySenderStrategy = class {
+                constructor() {
+                    this.buffers = new Map
+                }
+                enableCancellation(e) {
+                    if (null === e.id) return;
+                    const n = new SharedArrayBuffer(4);
+                    new Int32Array(n, 0, 1)[0] = t.Continue, this.buffers.set(e.id, n), e.$cancellationData = n
+                }
+                async sendCancellation(e, n) {
+                    const r = this.buffers.get(n);
+                    if (void 0 === r) return;
+                    const o = new Int32Array(r, 0, 1);
+                    Atomics.store(o, 0, t.Cancelled)
                 }
-                const s = {
-                    jsonrpc: T,
-                    method: o,
-                    params: i
-                };
-                return function(e) {
-                    if (W !== d.Off && L)
-                        if (H === m.Text) {
-                            let t;
-                            W !== d.Verbose && W !== d.Compact || (t = e.params ? `Params: ${se(e.params)}\n\n` : "No parameters provided.\n\n"), L.log(`Sending notification '${e.method}'.`, t)
-                        } else le("send-notification", e)
-                }(s), f.write(s).catch((e => {
-                    throw w.error("Sending notification failed."), e
-                }))
-            },
-            onNotification: (e, t) => {
-                let r;
-                return ue(), n.func(e) ? _ = e : t && (n.string(e) ? (r = e, P.set(e, {
-                    type: void 0,
-                    handler: t
-                })) : (r = e.method, P.set(e.method, {
-                    type: e,
-                    handler: t
-                }))), {
-                    dispose: () => {
-                        void 0 !== r ? P.delete(r) : _ = void 0
-                    }
+                cleanup(e) {
+                    this.buffers.delete(e)
                 }
-            },
-            onProgress: (e, t, n) => {
-                if (N.has(t)) throw new Error(`Progress handler for token ${t} already registered`);
-                return N.set(t, n), {
-                    dispose: () => {
-                        N.delete(t)
-                    }
+                dispose() {
+                    this.buffers.clear()
                 }
-            },
-            sendProgress: (e, t, n) => ge.sendNotification(l.type, {
-                token: t,
-                value: n
-            }),
-            onUnhandledProgress: z.event,
-            sendRequest: (e, ...t) => {
-                let o, i, a;
-                if (ue(), function() {
-                        if (!Y()) throw new Error("Call listen() first.")
-                    }(), n.string(e)) {
-                    o = e;
-                    const n = t[0],
-                        c = t[t.length - 1];
-                    let l = 0,
-                        u = r.ParameterStructures.auto;
-                    r.ParameterStructures.is(n) && (l = 1, u = n);
-                    let d = t.length;
-                    s.CancellationToken.is(c) && (d -= 1, a = c);
-                    const h = d - l;
-                    switch (h) {
-                        case 0:
-                            i = void 0;
-                            break;
-                        case 1:
-                            i = pe(u, t[l]);
-                            break;
-                        default:
-                            if (u === r.ParameterStructures.byName) throw new Error(`Received ${h} parameters for 'by Name' request parameter structure.`);
-                            i = t.slice(l, d).map((e => de(e)))
-                    }
-                } else {
-                    const n = t;
-                    o = e.method, i = me(e, n);
-                    const r = e.numberOfParams;
-                    a = s.CancellationToken.is(n[r]) ? n[r] : void 0
-                }
-                const c = C++;
-                let l;
-                a && (l = a.onCancellationRequested((() => {
-                    const e = Q.sender.sendCancellation(ge, c);
-                    return void 0 === e ? (w.log(`Received no promise from cancellation strategy when cancelling id ${c}`), Promise.resolve()) : e.catch((() => {
-                        w.log(`Sending cancellation messages for id ${c} failed`)
-                    }))
-                })));
-                const u = {
-                    jsonrpc: T,
-                    id: c,
-                    method: o,
-                    params: i
-                };
-                return function(e) {
-                    if (W !== d.Off && L)
-                        if (H === m.Text) {
-                            let t;
-                            W !== d.Verbose && W !== d.Compact || !e.params || (t = `Params: ${se(e.params)}\n\n`), L.log(`Sending request '${e.method} - (${e.id})'.`, t)
-                        } else le("send-request", e)
-                }(u), "function" == typeof Q.sender.enableCancellation && Q.sender.enableCancellation(u), new Promise((async (e, t) => {
-                    const n = {
-                        method: o,
-                        timerStart: Date.now(),
-                        resolve: t => {
-                            e(t), Q.sender.cleanup(c), null == l || l.dispose()
-                        },
-                        reject: e => {
-                            t(e), Q.sender.cleanup(c), null == l || l.dispose()
+            };
+            class r {
+                constructor(e) {
+                    this.data = new Int32Array(e, 0, 1)
+                }
+                get isCancellationRequested() {
+                    return Atomics.load(this.data, 0) === t.Cancelled
+                }
+                get onCancellationRequested() {
+                    throw new Error("Cancellation over SharedArrayBuffer doesn't support cancellation events")
+                }
+            }
+            class o {
+                constructor(e) {
+                    this.token = new r(e)
+                }
+                cancel() {}
+                dispose() {}
+            }
+            return so.SharedArrayReceiverStrategy = class {
+                constructor() {
+                    this.kind = "request"
+                }
+                createCancellationTokenSource(t) {
+                    const n = t.$cancellationData;
+                    return void 0 === n ? new e.CancellationTokenSource : new o(n)
+                }
+            }, so
+        }();
+        Object.defineProperty(e, "SharedArraySenderStrategy", {
+            enumerable: !0,
+            get: function() {
+                return a.SharedArraySenderStrategy
+            }
+        }), Object.defineProperty(e, "SharedArrayReceiverStrategy", {
+            enumerable: !0,
+            get: function() {
+                return a.SharedArrayReceiverStrategy
+            }
+        });
+        const c = function() {
+            if (co) return lo;
+            co = 1, Object.defineProperty(lo, "__esModule", {
+                value: !0
+            }), lo.ReadableStreamMessageReader = lo.AbstractMessageReader = lo.MessageReader = void 0;
+            const e = eo(),
+                t = Kr(),
+                n = to(),
+                r = ho();
+            var o, i;
+            (o || (lo.MessageReader = o = {})).is = function(e) {
+                let n = e;
+                return n && t.func(n.listen) && t.func(n.dispose) && t.func(n.onError) && t.func(n.onClose) && t.func(n.onPartialMessage)
+            };
+            class s {
+                constructor() {
+                    this.errorEmitter = new n.Emitter, this.closeEmitter = new n.Emitter, this.partialMessageEmitter = new n.Emitter
+                }
+                dispose() {
+                    this.errorEmitter.dispose(), this.closeEmitter.dispose()
+                }
+                get onError() {
+                    return this.errorEmitter.event
+                }
+                fireError(e) {
+                    this.errorEmitter.fire(this.asError(e))
+                }
+                get onClose() {
+                    return this.closeEmitter.event
+                }
+                fireClose() {
+                    this.closeEmitter.fire(void 0)
+                }
+                get onPartialMessage() {
+                    return this.partialMessageEmitter.event
+                }
+                firePartialMessage(e) {
+                    this.partialMessageEmitter.fire(e)
+                }
+                asError(e) {
+                    return e instanceof Error ? e : new Error(`Reader received error. Reason: ${t.string(e.message)?e.message:"unknown"}`)
+                }
+            }
+            return lo.AbstractMessageReader = s, (i || (i = {})).fromOptions = function(t) {
+                let n, r;
+                const o = new Map;
+                let i;
+                const s = new Map;
+                if (void 0 === t || "string" == typeof t) n = t ?? "utf-8";
+                else {
+                    if (n = t.charset ?? "utf-8", void 0 !== t.contentDecoder && (r = t.contentDecoder, o.set(r.name, r)), void 0 !== t.contentDecoders)
+                        for (const e of t.contentDecoders) o.set(e.name, e);
+                    if (void 0 !== t.contentTypeDecoder && (i = t.contentTypeDecoder, s.set(i.name, i)), void 0 !== t.contentTypeDecoders)
+                        for (const e of t.contentTypeDecoders) s.set(e.name, e)
+                }
+                return void 0 === i && (i = (0, e.default)().applicationJson.decoder, s.set(i.name, i)), {
+                    charset: n,
+                    contentDecoder: r,
+                    contentDecoders: o,
+                    contentTypeDecoder: i,
+                    contentTypeDecoders: s
+                }
+            }, lo.ReadableStreamMessageReader = class extends s {
+                constructor(t, n) {
+                    super(), this.readable = t, this.options = i.fromOptions(n), this.buffer = (0, e.default)().messageBuffer.create(this.options.charset), this._partialMessageTimeout = 1e4, this.nextMessageLength = -1, this.messageToken = 0, this.readSemaphore = new r.Semaphore(1)
+                }
+                set partialMessageTimeout(e) {
+                    this._partialMessageTimeout = e
+                }
+                get partialMessageTimeout() {
+                    return this._partialMessageTimeout
+                }
+                listen(e) {
+                    this.nextMessageLength = -1, this.messageToken = 0, this.partialMessageTimer = void 0, this.callback = e;
+                    const t = this.readable.onData((e => {
+                        this.onData(e)
+                    }));
+                    return this.readable.onError((e => this.fireError(e))), this.readable.onClose((() => this.fireClose())), t
+                }
+                onData(e) {
+                    try {
+                        for (this.buffer.append(e);;) {
+                            if (-1 === this.nextMessageLength) {
+                                const e = this.buffer.tryReadHeaders(!0);
+                                if (!e) return;
+                                const t = e.get("content-length");
+                                if (!t) return void this.fireError(new Error(`Header must provide a Content-Length property.\n${JSON.stringify(Object.fromEntries(e))}`));
+                                const n = parseInt(t);
+                                if (isNaN(n)) return void this.fireError(new Error(`Content-Length value must be a number. Got ${t}`));
+                                this.nextMessageLength = n
+                            }
+                            const e = this.buffer.tryReadBody(this.nextMessageLength);
+                            if (void 0 === e) return void this.setPartialMessageTimer();
+                            this.clearPartialMessageTimer(), this.nextMessageLength = -1, this.readSemaphore.lock((async () => {
+                                const t = void 0 !== this.options.contentDecoder ? await this.options.contentDecoder.decode(e) : e,
+                                    n = await this.options.contentTypeDecoder.decode(t, this.options);
+                                this.callback(n)
+                            })).catch((e => {
+                                this.fireError(e)
+                            }))
                         }
-                    };
+                    } catch (t) {
+                        this.fireError(t)
+                    }
+                }
+                clearPartialMessageTimer() {
+                    this.partialMessageTimer && (this.partialMessageTimer.dispose(), this.partialMessageTimer = void 0)
+                }
+                setPartialMessageTimer() {
+                    this.clearPartialMessageTimer(), this._partialMessageTimeout <= 0 || (this.partialMessageTimer = (0, e.default)().timer.setTimeout(((e, t) => {
+                        this.partialMessageTimer = void 0, e === this.messageToken && (this.firePartialMessage({
+                            messageToken: e,
+                            waitingTime: t
+                        }), this.setPartialMessageTimer())
+                    }), this._partialMessageTimeout, this.messageToken, this._partialMessageTimeout))
+                }
+            }, lo
+        }();
+        Object.defineProperty(e, "MessageReader", {
+            enumerable: !0,
+            get: function() {
+                return c.MessageReader
+            }
+        }), Object.defineProperty(e, "AbstractMessageReader", {
+            enumerable: !0,
+            get: function() {
+                return c.AbstractMessageReader
+            }
+        }), Object.defineProperty(e, "ReadableStreamMessageReader", {
+            enumerable: !0,
+            get: function() {
+                return c.ReadableStreamMessageReader
+            }
+        });
+        const l = function() {
+            if (fo) return po;
+            fo = 1, Object.defineProperty(po, "__esModule", {
+                value: !0
+            }), po.WriteableStreamMessageWriter = po.AbstractMessageWriter = po.MessageWriter = void 0;
+            const e = eo(),
+                t = Kr(),
+                n = ho(),
+                r = to();
+            var o, i;
+            (o || (po.MessageWriter = o = {})).is = function(e) {
+                let n = e;
+                return n && t.func(n.dispose) && t.func(n.onClose) && t.func(n.onError) && t.func(n.write)
+            };
+            class s {
+                constructor() {
+                    this.errorEmitter = new r.Emitter, this.closeEmitter = new r.Emitter
+                }
+                dispose() {
+                    this.errorEmitter.dispose(), this.closeEmitter.dispose()
+                }
+                get onError() {
+                    return this.errorEmitter.event
+                }
+                fireError(e, t, n) {
+                    this.errorEmitter.fire([this.asError(e), t, n])
+                }
+                get onClose() {
+                    return this.closeEmitter.event
+                }
+                fireClose() {
+                    this.closeEmitter.fire(void 0)
+                }
+                asError(e) {
+                    return e instanceof Error ? e : new Error(`Writer received error. Reason: ${t.string(e.message)?e.message:"unknown"}`)
+                }
+            }
+            return po.AbstractMessageWriter = s, (i || (i = {})).fromOptions = function(t) {
+                return void 0 === t || "string" == typeof t ? {
+                    charset: t ?? "utf-8",
+                    contentTypeEncoder: (0, e.default)().applicationJson.encoder
+                } : {
+                    charset: t.charset ?? "utf-8",
+                    contentEncoder: t.contentEncoder,
+                    contentTypeEncoder: t.contentTypeEncoder ?? (0, e.default)().applicationJson.encoder
+                }
+            }, po.WriteableStreamMessageWriter = class extends s {
+                constructor(e, t) {
+                    super(), this.writable = e, this.options = i.fromOptions(t), this.errorCount = 0, this.writeSemaphore = new n.Semaphore(1), this.writable.onError((e => this.fireError(e))), this.writable.onClose((() => this.fireClose()))
+                }
+                async write(e) {
+                    return this.writeSemaphore.lock((async () => this.options.contentTypeEncoder.encode(e, this.options).then((e => void 0 !== this.options.contentEncoder ? this.options.contentEncoder.encode(e) : e)).then((t => {
+                        const n = [];
+                        return n.push("Content-Length: ", t.byteLength.toString(), "\r\n"), n.push("\r\n"), this.doWrite(e, n, t)
+                    }), (e => {
+                        throw this.fireError(e), e
+                    }))))
+                }
+                async doWrite(e, t, n) {
                     try {
-                        await f.write(u), I.set(c, n)
-                    } catch (i) {
-                        throw w.error("Sending request failed."), n.reject(new r.ResponseError(r.ErrorCodes.MessageWriteError, i.message ? i.message : "Unknown reason")), i
+                        return await this.writable.write(t.join(""), "ascii"), this.writable.write(n)
+                    } catch (r) {
+                        return this.handleError(r, e), Promise.reject(r)
                     }
-                }))
-            },
-            onRequest: (e, t) => {
-                ue();
-                let r = null;
-                return u.is(e) ? (r = void 0, S = e) : n.string(e) ? (r = null, void 0 !== t && (r = e, M.set(e, {
-                    handler: t,
-                    type: void 0
-                }))) : void 0 !== t && (r = e.method, M.set(e.method, {
-                    type: e,
-                    handler: t
-                })), {
-                    dispose: () => {
-                        null !== r && (void 0 !== r ? M.delete(r) : S = void 0)
+                }
+                handleError(e, t) {
+                    this.errorCount++, this.fireError(e, t, this.errorCount)
+                }
+                end() {
+                    this.writable.end()
+                }
+            }, po
+        }();
+        Object.defineProperty(e, "MessageWriter", {
+            enumerable: !0,
+            get: function() {
+                return l.MessageWriter
+            }
+        }), Object.defineProperty(e, "AbstractMessageWriter", {
+            enumerable: !0,
+            get: function() {
+                return l.AbstractMessageWriter
+            }
+        }), Object.defineProperty(e, "WriteableStreamMessageWriter", {
+            enumerable: !0,
+            get: function() {
+                return l.WriteableStreamMessageWriter
+            }
+        });
+        const u = (mo || (mo = 1, Object.defineProperty(go, "__esModule", {
+            value: !0
+        }), go.AbstractMessageBuffer = void 0, go.AbstractMessageBuffer = class {
+            constructor(e = "utf-8") {
+                this._encoding = e, this._chunks = [], this._totalLength = 0
+            }
+            get encoding() {
+                return this._encoding
+            }
+            append(e) {
+                const t = "string" == typeof e ? this.fromString(e, this._encoding) : e;
+                this._chunks.push(t), this._totalLength += t.byteLength
+            }
+            tryReadHeaders(e = !1) {
+                if (0 === this._chunks.length) return;
+                let t = 0,
+                    n = 0,
+                    r = 0,
+                    o = 0;
+                e: for (; n < this._chunks.length;) {
+                    const e = this._chunks[n];
+                    for (r = 0; r < e.length;) {
+                        switch (e[r]) {
+                            case 13:
+                                switch (t) {
+                                    case 0:
+                                        t = 1;
+                                        break;
+                                    case 2:
+                                        t = 3;
+                                        break;
+                                    default:
+                                        t = 0
+                                }
+                                break;
+                            case 10:
+                                switch (t) {
+                                    case 1:
+                                        t = 2;
+                                        break;
+                                    case 3:
+                                        t = 4, r++;
+                                        break e;
+                                    default:
+                                        t = 0
+                                }
+                                break;
+                            default:
+                                t = 0
+                        }
+                        r++
                     }
+                    o += e.byteLength, n++
                 }
-            },
-            hasPendingResponse: () => I.size > 0,
-            trace: async (e, t, r) => {
-                let o = !1,
-                    i = m.Text;
-                void 0 !== r && (n.boolean(r) ? o = r : (o = r.sendNotification || !1, i = r.traceFormat || m.Text)), W = e, H = i, L = W === d.Off ? void 0 : t, !o || ee() || te() || await ge.sendNotification(v.type, {
-                    value: d.toString(e)
-                })
-            },
-            onError: U.event,
-            onClose: V.event,
-            onUnhandledNotification: $.event,
-            onDispose: J.event,
-            end: () => {
-                f.end()
-            },
-            dispose: () => {
-                if (te()) return;
-                K = O.Disposed, J.fire(void 0);
-                const e = new r.ResponseError(r.ErrorCodes.PendingResponseRejected, "Pending response rejected since connection got disposed");
-                for (const t of I.values()) t.reject(e);
-                I = new Map, F = new Map, B = new Set, A = new o.LinkedMap, n.func(f.dispose) && f.dispose(), n.func(h.dispose) && h.dispose()
-            },
-            listen: () => {
-                ue(),
-                    function() {
-                        if (Y()) throw new j(b.AlreadyListening, "Connection is already listening")
-                    }(), K = O.Listening, h.listen(ie)
-            },
-            inspect: () => {
-                (0, t.default)().console.log("inspect")
+                if (4 !== t) return;
+                const i = this._read(o + r),
+                    s = new Map,
+                    a = this.toString(i, "ascii").split("\r\n");
+                if (a.length < 2) return s;
+                for (let c = 0; c < a.length - 2; c++) {
+                    const t = a[c],
+                        n = t.indexOf(":");
+                    if (-1 === n) throw new Error(`Message header must separate key and value using ':'\n${t}`);
+                    const r = t.substr(0, n),
+                        o = t.substr(n + 1).trim();
+                    s.set(e ? r.toLowerCase() : r, o)
+                }
+                return s
+            }
+            tryReadBody(e) {
+                if (!(this._totalLength < e)) return this._read(e)
+            }
+            get numberOfBytes() {
+                return this._totalLength
+            }
+            _read(e) {
+                if (0 === e) return this.emptyBuffer();
+                if (e > this._totalLength) throw new Error("Cannot read so many bytes!");
+                if (this._chunks[0].byteLength === e) {
+                    const t = this._chunks[0];
+                    return this._chunks.shift(), this._totalLength -= e, this.asNative(t)
+                }
+                if (this._chunks[0].byteLength > e) {
+                    const t = this._chunks[0],
+                        n = this.asNative(t, e);
+                    return this._chunks[0] = t.slice(e), this._totalLength -= e, n
+                }
+                const t = this.allocNative(e);
+                let n = 0;
+                for (; e > 0;) {
+                    const r = this._chunks[0];
+                    if (r.byteLength > e) {
+                        const o = r.slice(0, e);
+                        t.set(o, n), n += e, this._chunks[0] = r.slice(e), this._totalLength -= e, e -= e
+                    } else t.set(r, n), n += r.byteLength, this._chunks.shift(), this._totalLength -= r.byteLength, e -= r.byteLength
+                }
+                return t
             }
-        };
-        return ge.onNotification(y.type, (e => {
-            if (W === d.Off || !L) return;
-            const t = W === d.Verbose || W === d.Compact;
-            L.log(e.message, t ? e.verbose : void 0)
-        })), ge.onNotification(l.type, (e => {
-            const t = N.get(e.token);
-            t ? t(e.value) : z.fire(e)
-        })), ge
-    }
-}($o),
-function(e) {
-    Object.defineProperty(e, "__esModule", {
-        value: !0
-    }), e.ProgressType = e.ProgressToken = e.createMessageConnection = e.NullLogger = e.ConnectionOptions = e.ConnectionStrategy = e.AbstractMessageBuffer = e.WriteableStreamMessageWriter = e.AbstractMessageWriter = e.MessageWriter = e.ReadableStreamMessageReader = e.AbstractMessageReader = e.MessageReader = e.SharedArrayReceiverStrategy = e.SharedArraySenderStrategy = e.CancellationToken = e.CancellationTokenSource = e.Emitter = e.Event = e.Disposable = e.LRUCache = e.Touch = e.LinkedMap = e.ParameterStructures = e.NotificationType9 = e.NotificationType8 = e.NotificationType7 = e.NotificationType6 = e.NotificationType5 = e.NotificationType4 = e.NotificationType3 = e.NotificationType2 = e.NotificationType1 = e.NotificationType0 = e.NotificationType = e.ErrorCodes = e.ResponseError = e.RequestType9 = e.RequestType8 = e.RequestType7 = e.RequestType6 = e.RequestType5 = e.RequestType4 = e.RequestType3 = e.RequestType2 = e.RequestType1 = e.RequestType0 = e.RequestType = e.Message = e.RAL = void 0, e.MessageStrategy = e.CancellationStrategy = e.CancellationSenderStrategy = e.CancellationReceiverStrategy = e.ConnectionError = e.ConnectionErrors = e.LogTraceNotification = e.SetTraceNotification = e.TraceFormat = e.TraceValues = e.Trace = void 0;
-    const t = Br;
-    Object.defineProperty(e, "Message", {
-        enumerable: !0,
-        get: function() {
-            return t.Message
-        }
-    }), Object.defineProperty(e, "RequestType", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType
-        }
-    }), Object.defineProperty(e, "RequestType0", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType0
-        }
-    }), Object.defineProperty(e, "RequestType1", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType1
-        }
-    }), Object.defineProperty(e, "RequestType2", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType2
-        }
-    }), Object.defineProperty(e, "RequestType3", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType3
-        }
-    }), Object.defineProperty(e, "RequestType4", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType4
-        }
-    }), Object.defineProperty(e, "RequestType5", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType5
-        }
-    }), Object.defineProperty(e, "RequestType6", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType6
-        }
-    }), Object.defineProperty(e, "RequestType7", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType7
-        }
-    }), Object.defineProperty(e, "RequestType8", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType8
-        }
-    }), Object.defineProperty(e, "RequestType9", {
-        enumerable: !0,
-        get: function() {
-            return t.RequestType9
-        }
-    }), Object.defineProperty(e, "ResponseError", {
-        enumerable: !0,
-        get: function() {
-            return t.ResponseError
-        }
-    }), Object.defineProperty(e, "ErrorCodes", {
-        enumerable: !0,
-        get: function() {
-            return t.ErrorCodes
-        }
-    }), Object.defineProperty(e, "NotificationType", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType
-        }
-    }), Object.defineProperty(e, "NotificationType0", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType0
-        }
-    }), Object.defineProperty(e, "NotificationType1", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType1
-        }
-    }), Object.defineProperty(e, "NotificationType2", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType2
-        }
-    }), Object.defineProperty(e, "NotificationType3", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType3
-        }
-    }), Object.defineProperty(e, "NotificationType4", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType4
-        }
-    }), Object.defineProperty(e, "NotificationType5", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType5
-        }
-    }), Object.defineProperty(e, "NotificationType6", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType6
-        }
-    }), Object.defineProperty(e, "NotificationType7", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType7
-        }
-    }), Object.defineProperty(e, "NotificationType8", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType8
-        }
-    }), Object.defineProperty(e, "NotificationType9", {
-        enumerable: !0,
-        get: function() {
-            return t.NotificationType9
-        }
-    }), Object.defineProperty(e, "ParameterStructures", {
-        enumerable: !0,
-        get: function() {
-            return t.ParameterStructures
-        }
-    });
-    const n = eo;
-    Object.defineProperty(e, "LinkedMap", {
-        enumerable: !0,
-        get: function() {
-            return n.LinkedMap
-        }
-    }), Object.defineProperty(e, "LRUCache", {
-        enumerable: !0,
-        get: function() {
-            return n.LRUCache
-        }
-    }), Object.defineProperty(e, "Touch", {
-        enumerable: !0,
-        get: function() {
-            return n.Touch
-        }
-    });
-    const r = ro;
-    Object.defineProperty(e, "Disposable", {
-        enumerable: !0,
-        get: function() {
-            return r.Disposable
-        }
-    });
-    const o = oo;
-    Object.defineProperty(e, "Event", {
-        enumerable: !0,
-        get: function() {
-            return o.Event
-        }
-    }), Object.defineProperty(e, "Emitter", {
-        enumerable: !0,
-        get: function() {
-            return o.Emitter
-        }
-    });
-    const i = fo;
-    Object.defineProperty(e, "CancellationTokenSource", {
-        enumerable: !0,
-        get: function() {
-            return i.CancellationTokenSource
-        }
-    }), Object.defineProperty(e, "CancellationToken", {
-        enumerable: !0,
-        get: function() {
-            return i.CancellationToken
-        }
-    });
-    const s = Co;
-    Object.defineProperty(e, "SharedArraySenderStrategy", {
-        enumerable: !0,
-        get: function() {
-            return s.SharedArraySenderStrategy
-        }
-    }), Object.defineProperty(e, "SharedArrayReceiverStrategy", {
-        enumerable: !0,
-        get: function() {
-            return s.SharedArrayReceiverStrategy
-        }
-    });
-    const a = Mo;
-    Object.defineProperty(e, "MessageReader", {
-        enumerable: !0,
-        get: function() {
-            return a.MessageReader
-        }
-    }), Object.defineProperty(e, "AbstractMessageReader", {
-        enumerable: !0,
-        get: function() {
-            return a.AbstractMessageReader
-        }
-    }), Object.defineProperty(e, "ReadableStreamMessageReader", {
-        enumerable: !0,
-        get: function() {
-            return a.ReadableStreamMessageReader
-        }
-    });
-    const c = Ao;
-    Object.defineProperty(e, "MessageWriter", {
-        enumerable: !0,
-        get: function() {
-            return c.MessageWriter
-        }
-    }), Object.defineProperty(e, "AbstractMessageWriter", {
-        enumerable: !0,
-        get: function() {
-            return c.AbstractMessageWriter
-        }
-    }), Object.defineProperty(e, "WriteableStreamMessageWriter", {
-        enumerable: !0,
-        get: function() {
-            return c.WriteableStreamMessageWriter
-        }
-    });
-    const l = Vo;
-    Object.defineProperty(e, "AbstractMessageBuffer", {
-        enumerable: !0,
-        get: function() {
-            return l.AbstractMessageBuffer
-        }
-    });
-    const u = $o;
-    Object.defineProperty(e, "ConnectionStrategy", {
-        enumerable: !0,
-        get: function() {
-            return u.ConnectionStrategy
-        }
-    }), Object.defineProperty(e, "ConnectionOptions", {
-        enumerable: !0,
-        get: function() {
-            return u.ConnectionOptions
-        }
-    }), Object.defineProperty(e, "NullLogger", {
-        enumerable: !0,
-        get: function() {
-            return u.NullLogger
-        }
-    }), Object.defineProperty(e, "createMessageConnection", {
-        enumerable: !0,
-        get: function() {
-            return u.createMessageConnection
-        }
-    }), Object.defineProperty(e, "ProgressToken", {
-        enumerable: !0,
-        get: function() {
-            return u.ProgressToken
-        }
-    }), Object.defineProperty(e, "ProgressType", {
-        enumerable: !0,
-        get: function() {
-            return u.ProgressType
-        }
-    }), Object.defineProperty(e, "Trace", {
-        enumerable: !0,
-        get: function() {
-            return u.Trace
-        }
-    }), Object.defineProperty(e, "TraceValues", {
-        enumerable: !0,
-        get: function() {
-            return u.TraceValues
-        }
-    }), Object.defineProperty(e, "TraceFormat", {
-        enumerable: !0,
-        get: function() {
-            return u.TraceFormat
-        }
-    }), Object.defineProperty(e, "SetTraceNotification", {
-        enumerable: !0,
-        get: function() {
-            return u.SetTraceNotification
-        }
-    }), Object.defineProperty(e, "LogTraceNotification", {
-        enumerable: !0,
-        get: function() {
-            return u.LogTraceNotification
-        }
-    }), Object.defineProperty(e, "ConnectionErrors", {
-        enumerable: !0,
-        get: function() {
-            return u.ConnectionErrors
-        }
-    }), Object.defineProperty(e, "ConnectionError", {
-        enumerable: !0,
-        get: function() {
-            return u.ConnectionError
-        }
-    }), Object.defineProperty(e, "CancellationReceiverStrategy", {
-        enumerable: !0,
-        get: function() {
-            return u.CancellationReceiverStrategy
-        }
-    }), Object.defineProperty(e, "CancellationSenderStrategy", {
-        enumerable: !0,
-        get: function() {
-            return u.CancellationSenderStrategy
-        }
-    }), Object.defineProperty(e, "CancellationStrategy", {
-        enumerable: !0,
-        get: function() {
-            return u.CancellationStrategy
-        }
-    }), Object.defineProperty(e, "MessageStrategy", {
-        enumerable: !0,
-        get: function() {
-            return u.MessageStrategy
-        }
-    });
-    const d = io;
-    e.RAL = d.default
-}(Ir), Object.defineProperty(Ar, "__esModule", {
+        }), go);
+        Object.defineProperty(e, "AbstractMessageBuffer", {
+            enumerable: !0,
+            get: function() {
+                return u.AbstractMessageBuffer
+            }
+        });
+        const d = wo();
+        Object.defineProperty(e, "ConnectionStrategy", {
+            enumerable: !0,
+            get: function() {
+                return d.ConnectionStrategy
+            }
+        }), Object.defineProperty(e, "ConnectionOptions", {
+            enumerable: !0,
+            get: function() {
+                return d.ConnectionOptions
+            }
+        }), Object.defineProperty(e, "NullLogger", {
+            enumerable: !0,
+            get: function() {
+                return d.NullLogger
+            }
+        }), Object.defineProperty(e, "createMessageConnection", {
+            enumerable: !0,
+            get: function() {
+                return d.createMessageConnection
+            }
+        }), Object.defineProperty(e, "ProgressToken", {
+            enumerable: !0,
+            get: function() {
+                return d.ProgressToken
+            }
+        }), Object.defineProperty(e, "ProgressType", {
+            enumerable: !0,
+            get: function() {
+                return d.ProgressType
+            }
+        }), Object.defineProperty(e, "Trace", {
+            enumerable: !0,
+            get: function() {
+                return d.Trace
+            }
+        }), Object.defineProperty(e, "TraceValues", {
+            enumerable: !0,
+            get: function() {
+                return d.TraceValues
+            }
+        }), Object.defineProperty(e, "TraceFormat", {
+            enumerable: !0,
+            get: function() {
+                return d.TraceFormat
+            }
+        }), Object.defineProperty(e, "SetTraceNotification", {
+            enumerable: !0,
+            get: function() {
+                return d.SetTraceNotification
+            }
+        }), Object.defineProperty(e, "LogTraceNotification", {
+            enumerable: !0,
+            get: function() {
+                return d.LogTraceNotification
+            }
+        }), Object.defineProperty(e, "ConnectionErrors", {
+            enumerable: !0,
+            get: function() {
+                return d.ConnectionErrors
+            }
+        }), Object.defineProperty(e, "ConnectionError", {
+            enumerable: !0,
+            get: function() {
+                return d.ConnectionError
+            }
+        }), Object.defineProperty(e, "CancellationReceiverStrategy", {
+            enumerable: !0,
+            get: function() {
+                return d.CancellationReceiverStrategy
+            }
+        }), Object.defineProperty(e, "CancellationSenderStrategy", {
+            enumerable: !0,
+            get: function() {
+                return d.CancellationSenderStrategy
+            }
+        }), Object.defineProperty(e, "CancellationStrategy", {
+            enumerable: !0,
+            get: function() {
+                return d.CancellationStrategy
+            }
+        }), Object.defineProperty(e, "MessageStrategy", {
+            enumerable: !0,
+            get: function() {
+                return d.MessageStrategy
+            }
+        });
+        const h = eo();
+        e.RAL = h.default
+    }(Fr)), Fr
+}
+Object.defineProperty(Br, "__esModule", {
     value: !0
 });
-const zo = Ir;
-class Jo extends zo.AbstractMessageBuffer {
+const xo = Co();
+class ko extends xo.AbstractMessageBuffer {
     constructor(e = "utf-8") {
         super(e), this.asciiDecoder = new TextDecoder("ascii")
     }
     emptyBuffer() {
-        return Jo.emptyBuffer
+        return ko.emptyBuffer
     }
     fromString(e, t) {
         return (new TextEncoder).encode(e)
     }
     toString(e, t) {
         return "ascii" === t ? this.asciiDecoder.decode(e) : new TextDecoder(t).decode(e)
     }
     asNative(e, t) {
         return void 0 === t ? e : e.slice(0, t)
     }
     allocNative(e) {
         return new Uint8Array(e)
     }
 }
-Jo.emptyBuffer = new Uint8Array(0);
-class Qo {
+ko.emptyBuffer = new Uint8Array(0);
+class Ro {
     constructor(e) {
-        this.socket = e, this._onData = new zo.Emitter, this._messageListener = e => {
+        this.socket = e, this._onData = new xo.Emitter, this._messageListener = e => {
             e.data.arrayBuffer().then((e => {
                 this._onData.fire(new Uint8Array(e))
             }), (() => {
-                (0, zo.RAL)().console.error("Converting blob to array buffer failed.")
+                (0, xo.RAL)().console.error("Converting blob to array buffer failed.")
             }))
         }, this.socket.addEventListener("message", this._messageListener)
     }
     onClose(e) {
-        return this.socket.addEventListener("close", e), zo.Disposable.create((() => this.socket.removeEventListener("close", e)))
+        return this.socket.addEventListener("close", e), xo.Disposable.create((() => this.socket.removeEventListener("close", e)))
     }
     onError(e) {
-        return this.socket.addEventListener("error", e), zo.Disposable.create((() => this.socket.removeEventListener("error", e)))
+        return this.socket.addEventListener("error", e), xo.Disposable.create((() => this.socket.removeEventListener("error", e)))
     }
     onEnd(e) {
-        return this.socket.addEventListener("end", e), zo.Disposable.create((() => this.socket.removeEventListener("end", e)))
+        return this.socket.addEventListener("end", e), xo.Disposable.create((() => this.socket.removeEventListener("end", e)))
     }
     onData(e) {
         return this._onData.event(e)
     }
 }
-class Go {
+class To {
     constructor(e) {
         this.socket = e
     }
     onClose(e) {
-        return this.socket.addEventListener("close", e), zo.Disposable.create((() => this.socket.removeEventListener("close", e)))
+        return this.socket.addEventListener("close", e), xo.Disposable.create((() => this.socket.removeEventListener("close", e)))
     }
     onError(e) {
-        return this.socket.addEventListener("error", e), zo.Disposable.create((() => this.socket.removeEventListener("error", e)))
+        return this.socket.addEventListener("error", e), xo.Disposable.create((() => this.socket.removeEventListener("error", e)))
     }
     onEnd(e) {
-        return this.socket.addEventListener("end", e), zo.Disposable.create((() => this.socket.removeEventListener("end", e)))
+        return this.socket.addEventListener("end", e), xo.Disposable.create((() => this.socket.removeEventListener("end", e)))
     }
     write(e, t) {
         if ("string" == typeof e) {
             if (void 0 !== t && "utf-8" !== t) throw new Error(`In a Browser environments only utf-8 text encoding is supported. But got encoding: ${t}`);
             this.socket.send(e)
         } else this.socket.send(e);
         return Promise.resolve()
     }
     end() {
         this.socket.close()
     }
 }
-const Xo = new TextEncoder,
-    Zo = Object.freeze({
+const So = new TextEncoder,
+    Mo = Object.freeze({
         messageBuffer: Object.freeze({
-            create: e => new Jo(e)
+            create: e => new ko(e)
         }),
         applicationJson: Object.freeze({
             encoder: Object.freeze({
                 name: "application/json",
                 encode: (e, t) => {
                     if ("utf-8" !== t.charset) throw new Error(`In a Browser environments only utf-8 text encoding is supported. But got encoding: ${t.charset}`);
-                    return Promise.resolve(Xo.encode(JSON.stringify(e, void 0, 0)))
+                    return Promise.resolve(So.encode(JSON.stringify(e, void 0, 0)))
                 }
             }),
             decoder: Object.freeze({
                 name: "application/json",
                 decode: (e, t) => {
                     if (!(e instanceof Uint8Array)) throw new Error("In a Browser environments only Uint8Arrays are supported.");
                     return Promise.resolve(JSON.parse(new TextDecoder(t.charset).decode(e)))
                 }
             })
         }),
         stream: Object.freeze({
-            asReadableStream: e => new Qo(e),
-            asWritableStream: e => new Go(e)
+            asReadableStream: e => new Ro(e),
+            asWritableStream: e => new To(e)
         }),
         console: console,
         timer: Object.freeze({
             setTimeout(e, t, ...n) {
                 const r = setTimeout(e, t, ...n);
                 return {
                     dispose: () => clearTimeout(r)
@@ -9908,19 +9948,19 @@
                 return {
                     dispose: () => clearInterval(r)
                 }
             }
         })
     });
 
-function Yo() {
-    return Zo
-}(Yo || (Yo = {})).install = function() {
-        zo.RAL.install(Zo)
-    }, Ar.default = Yo,
+function Do() {
+    return Mo
+}(Do || (Do = {})).install = function() {
+        xo.RAL.install(Mo)
+    }, Br.default = Do,
     function(e) {
         var t = Y && Y.__createBinding || (Object.create ? function(e, t, n, r) {
                 void 0 === r && (r = n);
                 var o = Object.getOwnPropertyDescriptor(t, n);
                 o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
                     enumerable: !0,
                     get: function() {
@@ -9932,17 +9972,17 @@
             }),
             n = Y && Y.__exportStar || function(e, n) {
                 for (var r in e) "default" === r || Object.prototype.hasOwnProperty.call(n, r) || t(n, e, r)
             };
         Object.defineProperty(e, "__esModule", {
             value: !0
         }), e.createMessageConnection = e.BrowserMessageWriter = e.BrowserMessageReader = void 0;
-        Ar.default.install();
-        const r = Ir;
-        n(Ir, e);
+        Br.default.install();
+        const r = Co();
+        n(Co(), e);
         class o extends r.AbstractMessageReader {
             constructor(e) {
                 super(), this._onData = new r.Emitter, this._messageListener = e => {
                     this._onData.fire(e.data)
                 }, e.addEventListener("error", (e => this.fireError(e))), e.onmessage = this._messageListener
             }
             listen(e) {
@@ -9967,531 +10007,531 @@
             end() {}
         }
         e.BrowserMessageWriter = i, e.createMessageConnection = function(e, t, n, o) {
             return void 0 === n && (n = r.NullLogger), r.ConnectionStrategy.is(o) && (o = {
                 connectionStrategy: o
             }), (0, r.createMessageConnection)(e, t, n, o)
         }
-    }(Lr);
-var ei, ti, ni, ri, oi, ii, si, ai, ci, li, ui, di, hi, fi, pi, mi, gi, vi, yi, bi, wi, Ci, xi, ki, Ri, Ti, Si, Mi, Di, _i, Ei, Pi, Oi, Ni, ji, qi, Li, Ai, Ii, Bi, Fi, Wi, Hi, Ki, Ui, Vi, $i, zi, Ji, Qi, Gi, Xi, Zi, Yi, es, ts, ns, rs, os, is, ss, as, cs, ls, us, ds, hs, fs, ps, ms, gs, vs, ys, bs, ws, Cs, xs, ks, Rs, Ts, Ss, Ms, Ds, _s, Es, Ps, Os, Ns, js, qs, Ls, As, Is, Bs, Fs, Ws, Hs, Ks, Us, Vs, $s, zs, Js, Qs, Gs, Xs, Zs, Ys, ea, ta, na, ra, oa, ia, sa, aa, ca, la, ua, da, ha, fa, pa, ma, ga, va, ya, ba, wa, Ca, xa, ka, Ra = Lr,
-    Ta = {};
-(ei || (ei = {})).is = function(e) {
+    }(Ir);
+var _o, Eo, Po, Oo, No, jo, qo, Lo, Ao, Io, Bo, Fo, Wo, Ho, Ko, Uo, Vo, $o, zo, Jo, Qo, Go, Xo, Zo, Yo, ei, ti, ni, ri, oi, ii, si, ai, ci, li, ui, di, hi, fi, pi, mi, gi, vi, yi, bi, wi, Ci, xi, ki, Ri, Ti, Si, Mi, Di, _i, Ei, Pi, Oi, Ni, ji, qi, Li, Ai, Ii, Bi, Fi, Wi, Hi, Ki, Ui, Vi, $i, zi, Ji, Qi, Gi, Xi, Zi, Yi, es, ts, ns, rs, os, is, ss, as, cs, ls, us, ds, hs, fs, ps, ms, gs, vs, ys, bs, ws, Cs, xs, ks, Rs, Ts, Ss, Ms, Ds, _s, Es, Ps, Os, Ns, js, qs, Ls, As, Is, Bs, Fs, Ws, Hs, Ks, Us, Vs, $s, zs, Js, Qs, Gs, Xs, Zs, Ys = Ir,
+    ea = {};
+(_o || (_o = {})).is = function(e) {
     return "string" == typeof e
-}, (ti || (ti = {})).is = function(e) {
+}, (Eo || (Eo = {})).is = function(e) {
     return "string" == typeof e
-}, (ri = ni || (ni = {})).MIN_VALUE = -2147483648, ri.MAX_VALUE = 2147483647, ri.is = function(e) {
-    return "number" == typeof e && ri.MIN_VALUE <= e && e <= ri.MAX_VALUE
-}, (ii = oi || (oi = {})).MIN_VALUE = 0, ii.MAX_VALUE = 2147483647, ii.is = function(e) {
-    return "number" == typeof e && ii.MIN_VALUE <= e && e <= ii.MAX_VALUE
-}, (ai = si || (si = {})).create = function(e, t) {
-    return e === Number.MAX_VALUE && (e = oi.MAX_VALUE), t === Number.MAX_VALUE && (t = oi.MAX_VALUE), {
+}, (Oo = Po || (Po = {})).MIN_VALUE = -2147483648, Oo.MAX_VALUE = 2147483647, Oo.is = function(e) {
+    return "number" == typeof e && Oo.MIN_VALUE <= e && e <= Oo.MAX_VALUE
+}, (jo = No || (No = {})).MIN_VALUE = 0, jo.MAX_VALUE = 2147483647, jo.is = function(e) {
+    return "number" == typeof e && jo.MIN_VALUE <= e && e <= jo.MAX_VALUE
+}, (Lo = qo || (qo = {})).create = function(e, t) {
+    return e === Number.MAX_VALUE && (e = No.MAX_VALUE), t === Number.MAX_VALUE && (t = No.MAX_VALUE), {
         line: e,
         character: t
     }
-}, ai.is = function(e) {
+}, Lo.is = function(e) {
     let t = e;
-    return _a.objectLiteral(t) && _a.uinteger(t.line) && _a.uinteger(t.character)
-}, (li = ci || (ci = {})).create = function(e, t, n, r) {
-    if (_a.uinteger(e) && _a.uinteger(t) && _a.uinteger(n) && _a.uinteger(r)) return {
-        start: si.create(e, t),
-        end: si.create(n, r)
+    return oa.objectLiteral(t) && oa.uinteger(t.line) && oa.uinteger(t.character)
+}, (Io = Ao || (Ao = {})).create = function(e, t, n, r) {
+    if (oa.uinteger(e) && oa.uinteger(t) && oa.uinteger(n) && oa.uinteger(r)) return {
+        start: qo.create(e, t),
+        end: qo.create(n, r)
     };
-    if (si.is(e) && si.is(t)) return {
+    if (qo.is(e) && qo.is(t)) return {
         start: e,
         end: t
     };
     throw new Error(`Range#create called with invalid arguments[${e}, ${t}, ${n}, ${r}]`)
-}, li.is = function(e) {
+}, Io.is = function(e) {
     let t = e;
-    return _a.objectLiteral(t) && si.is(t.start) && si.is(t.end)
-}, (di = ui || (ui = {})).create = function(e, t) {
+    return oa.objectLiteral(t) && qo.is(t.start) && qo.is(t.end)
+}, (Fo = Bo || (Bo = {})).create = function(e, t) {
     return {
         uri: e,
         range: t
     }
-}, di.is = function(e) {
+}, Fo.is = function(e) {
     let t = e;
-    return _a.objectLiteral(t) && ci.is(t.range) && (_a.string(t.uri) || _a.undefined(t.uri))
-}, (fi = hi || (hi = {})).create = function(e, t, n, r) {
+    return oa.objectLiteral(t) && Ao.is(t.range) && (oa.string(t.uri) || oa.undefined(t.uri))
+}, (Ho = Wo || (Wo = {})).create = function(e, t, n, r) {
     return {
         targetUri: e,
         targetRange: t,
         targetSelectionRange: n,
         originSelectionRange: r
     }
-}, fi.is = function(e) {
+}, Ho.is = function(e) {
     let t = e;
-    return _a.objectLiteral(t) && ci.is(t.targetRange) && _a.string(t.targetUri) && ci.is(t.targetSelectionRange) && (ci.is(t.originSelectionRange) || _a.undefined(t.originSelectionRange))
-}, (mi = pi || (pi = {})).create = function(e, t, n, r) {
+    return oa.objectLiteral(t) && Ao.is(t.targetRange) && oa.string(t.targetUri) && Ao.is(t.targetSelectionRange) && (Ao.is(t.originSelectionRange) || oa.undefined(t.originSelectionRange))
+}, (Uo = Ko || (Ko = {})).create = function(e, t, n, r) {
     return {
         red: e,
         green: t,
         blue: n,
         alpha: r
     }
-}, mi.is = function(e) {
+}, Uo.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && _a.numberRange(t.red, 0, 1) && _a.numberRange(t.green, 0, 1) && _a.numberRange(t.blue, 0, 1) && _a.numberRange(t.alpha, 0, 1)
-}, (vi = gi || (gi = {})).create = function(e, t) {
+    return oa.objectLiteral(t) && oa.numberRange(t.red, 0, 1) && oa.numberRange(t.green, 0, 1) && oa.numberRange(t.blue, 0, 1) && oa.numberRange(t.alpha, 0, 1)
+}, ($o = Vo || (Vo = {})).create = function(e, t) {
     return {
         range: e,
         color: t
     }
-}, vi.is = function(e) {
+}, $o.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && ci.is(t.range) && pi.is(t.color)
-}, (bi = yi || (yi = {})).create = function(e, t, n) {
+    return oa.objectLiteral(t) && Ao.is(t.range) && Ko.is(t.color)
+}, (Jo = zo || (zo = {})).create = function(e, t, n) {
     return {
         label: e,
         textEdit: t,
         additionalTextEdits: n
     }
-}, bi.is = function(e) {
+}, Jo.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && _a.string(t.label) && (_a.undefined(t.textEdit) || qi.is(t)) && (_a.undefined(t.additionalTextEdits) || _a.typedArray(t.additionalTextEdits, qi.is))
-}, (Ci = wi || (wi = {})).Comment = "comment", Ci.Imports = "imports", Ci.Region = "region", (ki = xi || (xi = {})).create = function(e, t, n, r, o, i) {
+    return oa.objectLiteral(t) && oa.string(t.label) && (oa.undefined(t.textEdit) || ui.is(t)) && (oa.undefined(t.additionalTextEdits) || oa.typedArray(t.additionalTextEdits, ui.is))
+}, (Go = Qo || (Qo = {})).Comment = "comment", Go.Imports = "imports", Go.Region = "region", (Zo = Xo || (Xo = {})).create = function(e, t, n, r, o, i) {
     const s = {
         startLine: e,
         endLine: t
     };
-    return _a.defined(n) && (s.startCharacter = n), _a.defined(r) && (s.endCharacter = r), _a.defined(o) && (s.kind = o), _a.defined(i) && (s.collapsedText = i), s
-}, ki.is = function(e) {
+    return oa.defined(n) && (s.startCharacter = n), oa.defined(r) && (s.endCharacter = r), oa.defined(o) && (s.kind = o), oa.defined(i) && (s.collapsedText = i), s
+}, Zo.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && _a.uinteger(t.startLine) && _a.uinteger(t.startLine) && (_a.undefined(t.startCharacter) || _a.uinteger(t.startCharacter)) && (_a.undefined(t.endCharacter) || _a.uinteger(t.endCharacter)) && (_a.undefined(t.kind) || _a.string(t.kind))
-}, (Ti = Ri || (Ri = {})).create = function(e, t) {
+    return oa.objectLiteral(t) && oa.uinteger(t.startLine) && oa.uinteger(t.startLine) && (oa.undefined(t.startCharacter) || oa.uinteger(t.startCharacter)) && (oa.undefined(t.endCharacter) || oa.uinteger(t.endCharacter)) && (oa.undefined(t.kind) || oa.string(t.kind))
+}, (ei = Yo || (Yo = {})).create = function(e, t) {
     return {
         location: e,
         message: t
     }
-}, Ti.is = function(e) {
+}, ei.is = function(e) {
     let t = e;
-    return _a.defined(t) && ui.is(t.location) && _a.string(t.message)
-}, (Mi = Si || (Si = {})).Error = 1, Mi.Warning = 2, Mi.Information = 3, Mi.Hint = 4, (_i = Di || (Di = {})).Unnecessary = 1, _i.Deprecated = 2, (Ei || (Ei = {})).is = function(e) {
+    return oa.defined(t) && Bo.is(t.location) && oa.string(t.message)
+}, (ni = ti || (ti = {})).Error = 1, ni.Warning = 2, ni.Information = 3, ni.Hint = 4, (oi = ri || (ri = {})).Unnecessary = 1, oi.Deprecated = 2, (ii || (ii = {})).is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && _a.string(t.href)
-}, (Oi = Pi || (Pi = {})).create = function(e, t, n, r, o, i) {
+    return oa.objectLiteral(t) && oa.string(t.href)
+}, (ai = si || (si = {})).create = function(e, t, n, r, o, i) {
     let s = {
         range: e,
         message: t
     };
-    return _a.defined(n) && (s.severity = n), _a.defined(r) && (s.code = r), _a.defined(o) && (s.source = o), _a.defined(i) && (s.relatedInformation = i), s
-}, Oi.is = function(e) {
+    return oa.defined(n) && (s.severity = n), oa.defined(r) && (s.code = r), oa.defined(o) && (s.source = o), oa.defined(i) && (s.relatedInformation = i), s
+}, ai.is = function(e) {
     var t;
     let n = e;
-    return _a.defined(n) && ci.is(n.range) && _a.string(n.message) && (_a.number(n.severity) || _a.undefined(n.severity)) && (_a.integer(n.code) || _a.string(n.code) || _a.undefined(n.code)) && (_a.undefined(n.codeDescription) || _a.string(null === (t = n.codeDescription) || void 0 === t ? void 0 : t.href)) && (_a.string(n.source) || _a.undefined(n.source)) && (_a.undefined(n.relatedInformation) || _a.typedArray(n.relatedInformation, Ri.is))
-}, (ji = Ni || (Ni = {})).create = function(e, t, ...n) {
+    return oa.defined(n) && Ao.is(n.range) && oa.string(n.message) && (oa.number(n.severity) || oa.undefined(n.severity)) && (oa.integer(n.code) || oa.string(n.code) || oa.undefined(n.code)) && (oa.undefined(n.codeDescription) || oa.string(null === (t = n.codeDescription) || void 0 === t ? void 0 : t.href)) && (oa.string(n.source) || oa.undefined(n.source)) && (oa.undefined(n.relatedInformation) || oa.typedArray(n.relatedInformation, Yo.is))
+}, (li = ci || (ci = {})).create = function(e, t, ...n) {
     let r = {
         title: e,
         command: t
     };
-    return _a.defined(n) && n.length > 0 && (r.arguments = n), r
-}, ji.is = function(e) {
+    return oa.defined(n) && n.length > 0 && (r.arguments = n), r
+}, li.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.string(t.title) && _a.string(t.command)
-}, (Li = qi || (qi = {})).replace = function(e, t) {
+    return oa.defined(t) && oa.string(t.title) && oa.string(t.command)
+}, (di = ui || (ui = {})).replace = function(e, t) {
     return {
         range: e,
         newText: t
     }
-}, Li.insert = function(e, t) {
+}, di.insert = function(e, t) {
     return {
         range: {
             start: e,
             end: e
         },
         newText: t
     }
-}, Li.del = function(e) {
+}, di.del = function(e) {
     return {
         range: e,
         newText: ""
     }
-}, Li.is = function(e) {
+}, di.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && _a.string(t.newText) && ci.is(t.range)
-}, (Ii = Ai || (Ai = {})).create = function(e, t, n) {
+    return oa.objectLiteral(t) && oa.string(t.newText) && Ao.is(t.range)
+}, (fi = hi || (hi = {})).create = function(e, t, n) {
     const r = {
         label: e
     };
     return void 0 !== t && (r.needsConfirmation = t), void 0 !== n && (r.description = n), r
-}, Ii.is = function(e) {
+}, fi.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && _a.string(t.label) && (_a.boolean(t.needsConfirmation) || void 0 === t.needsConfirmation) && (_a.string(t.description) || void 0 === t.description)
-}, (Bi || (Bi = {})).is = function(e) {
+    return oa.objectLiteral(t) && oa.string(t.label) && (oa.boolean(t.needsConfirmation) || void 0 === t.needsConfirmation) && (oa.string(t.description) || void 0 === t.description)
+}, (pi || (pi = {})).is = function(e) {
     const t = e;
-    return _a.string(t)
-}, (Wi = Fi || (Fi = {})).replace = function(e, t, n) {
+    return oa.string(t)
+}, (gi = mi || (mi = {})).replace = function(e, t, n) {
     return {
         range: e,
         newText: t,
         annotationId: n
     }
-}, Wi.insert = function(e, t, n) {
+}, gi.insert = function(e, t, n) {
     return {
         range: {
             start: e,
             end: e
         },
         newText: t,
         annotationId: n
     }
-}, Wi.del = function(e, t) {
+}, gi.del = function(e, t) {
     return {
         range: e,
         newText: "",
         annotationId: t
     }
-}, Wi.is = function(e) {
+}, gi.is = function(e) {
     const t = e;
-    return qi.is(t) && (Ai.is(t.annotationId) || Bi.is(t.annotationId))
-}, (Ki = Hi || (Hi = {})).create = function(e, t) {
+    return ui.is(t) && (hi.is(t.annotationId) || pi.is(t.annotationId))
+}, (yi = vi || (vi = {})).create = function(e, t) {
     return {
         textDocument: e,
         edits: t
     }
-}, Ki.is = function(e) {
+}, yi.is = function(e) {
     let t = e;
-    return _a.defined(t) && ts.is(t.textDocument) && Array.isArray(t.edits)
-}, (Vi = Ui || (Ui = {})).create = function(e, t, n) {
+    return oa.defined(t) && Ei.is(t.textDocument) && Array.isArray(t.edits)
+}, (wi = bi || (bi = {})).create = function(e, t, n) {
     let r = {
         kind: "create",
         uri: e
     };
     return void 0 === t || void 0 === t.overwrite && void 0 === t.ignoreIfExists || (r.options = t), void 0 !== n && (r.annotationId = n), r
-}, Vi.is = function(e) {
+}, wi.is = function(e) {
     let t = e;
-    return t && "create" === t.kind && _a.string(t.uri) && (void 0 === t.options || (void 0 === t.options.overwrite || _a.boolean(t.options.overwrite)) && (void 0 === t.options.ignoreIfExists || _a.boolean(t.options.ignoreIfExists))) && (void 0 === t.annotationId || Bi.is(t.annotationId))
-}, (zi = $i || ($i = {})).create = function(e, t, n, r) {
+    return t && "create" === t.kind && oa.string(t.uri) && (void 0 === t.options || (void 0 === t.options.overwrite || oa.boolean(t.options.overwrite)) && (void 0 === t.options.ignoreIfExists || oa.boolean(t.options.ignoreIfExists))) && (void 0 === t.annotationId || pi.is(t.annotationId))
+}, (xi = Ci || (Ci = {})).create = function(e, t, n, r) {
     let o = {
         kind: "rename",
         oldUri: e,
         newUri: t
     };
     return void 0 === n || void 0 === n.overwrite && void 0 === n.ignoreIfExists || (o.options = n), void 0 !== r && (o.annotationId = r), o
-}, zi.is = function(e) {
+}, xi.is = function(e) {
     let t = e;
-    return t && "rename" === t.kind && _a.string(t.oldUri) && _a.string(t.newUri) && (void 0 === t.options || (void 0 === t.options.overwrite || _a.boolean(t.options.overwrite)) && (void 0 === t.options.ignoreIfExists || _a.boolean(t.options.ignoreIfExists))) && (void 0 === t.annotationId || Bi.is(t.annotationId))
-}, (Qi = Ji || (Ji = {})).create = function(e, t, n) {
+    return t && "rename" === t.kind && oa.string(t.oldUri) && oa.string(t.newUri) && (void 0 === t.options || (void 0 === t.options.overwrite || oa.boolean(t.options.overwrite)) && (void 0 === t.options.ignoreIfExists || oa.boolean(t.options.ignoreIfExists))) && (void 0 === t.annotationId || pi.is(t.annotationId))
+}, (Ri = ki || (ki = {})).create = function(e, t, n) {
     let r = {
         kind: "delete",
         uri: e
     };
     return void 0 === t || void 0 === t.recursive && void 0 === t.ignoreIfNotExists || (r.options = t), void 0 !== n && (r.annotationId = n), r
-}, Qi.is = function(e) {
+}, Ri.is = function(e) {
     let t = e;
-    return t && "delete" === t.kind && _a.string(t.uri) && (void 0 === t.options || (void 0 === t.options.recursive || _a.boolean(t.options.recursive)) && (void 0 === t.options.ignoreIfNotExists || _a.boolean(t.options.ignoreIfNotExists))) && (void 0 === t.annotationId || Bi.is(t.annotationId))
-}, (Gi || (Gi = {})).is = function(e) {
+    return t && "delete" === t.kind && oa.string(t.uri) && (void 0 === t.options || (void 0 === t.options.recursive || oa.boolean(t.options.recursive)) && (void 0 === t.options.ignoreIfNotExists || oa.boolean(t.options.ignoreIfNotExists))) && (void 0 === t.annotationId || pi.is(t.annotationId))
+}, (Ti || (Ti = {})).is = function(e) {
     let t = e;
-    return t && (void 0 !== t.changes || void 0 !== t.documentChanges) && (void 0 === t.documentChanges || t.documentChanges.every((e => _a.string(e.kind) ? Ui.is(e) || $i.is(e) || Ji.is(e) : Hi.is(e))))
+    return t && (void 0 !== t.changes || void 0 !== t.documentChanges) && (void 0 === t.documentChanges || t.documentChanges.every((e => oa.string(e.kind) ? bi.is(e) || Ci.is(e) || ki.is(e) : vi.is(e))))
 };
-class Sa {
+class ta {
     constructor(e, t) {
         this.edits = e, this.changeAnnotations = t
     }
     insert(e, t, n) {
         let r, o;
-        if (void 0 === n ? r = qi.insert(e, t) : Bi.is(n) ? (o = n, r = Fi.insert(e, t, n)) : (this.assertChangeAnnotations(this.changeAnnotations), o = this.changeAnnotations.manage(n), r = Fi.insert(e, t, o)), this.edits.push(r), void 0 !== o) return o
+        if (void 0 === n ? r = ui.insert(e, t) : pi.is(n) ? (o = n, r = mi.insert(e, t, n)) : (this.assertChangeAnnotations(this.changeAnnotations), o = this.changeAnnotations.manage(n), r = mi.insert(e, t, o)), this.edits.push(r), void 0 !== o) return o
     }
     replace(e, t, n) {
         let r, o;
-        if (void 0 === n ? r = qi.replace(e, t) : Bi.is(n) ? (o = n, r = Fi.replace(e, t, n)) : (this.assertChangeAnnotations(this.changeAnnotations), o = this.changeAnnotations.manage(n), r = Fi.replace(e, t, o)), this.edits.push(r), void 0 !== o) return o
+        if (void 0 === n ? r = ui.replace(e, t) : pi.is(n) ? (o = n, r = mi.replace(e, t, n)) : (this.assertChangeAnnotations(this.changeAnnotations), o = this.changeAnnotations.manage(n), r = mi.replace(e, t, o)), this.edits.push(r), void 0 !== o) return o
     }
     delete(e, t) {
         let n, r;
-        if (void 0 === t ? n = qi.del(e) : Bi.is(t) ? (r = t, n = Fi.del(e, t)) : (this.assertChangeAnnotations(this.changeAnnotations), r = this.changeAnnotations.manage(t), n = Fi.del(e, r)), this.edits.push(n), void 0 !== r) return r
+        if (void 0 === t ? n = ui.del(e) : pi.is(t) ? (r = t, n = mi.del(e, t)) : (this.assertChangeAnnotations(this.changeAnnotations), r = this.changeAnnotations.manage(t), n = mi.del(e, r)), this.edits.push(n), void 0 !== r) return r
     }
     add(e) {
         this.edits.push(e)
     }
     all() {
         return this.edits
     }
     clear() {
         this.edits.splice(0, this.edits.length)
     }
     assertChangeAnnotations(e) {
         if (void 0 === e) throw new Error("Text edit change is not configured to manage change annotations.")
     }
 }
-class Ma {
+class na {
     constructor(e) {
         this._annotations = void 0 === e ? Object.create(null) : e, this._counter = 0, this._size = 0
     }
     all() {
         return this._annotations
     }
     get size() {
         return this._size
     }
     manage(e, t) {
         let n;
-        if (Bi.is(e) ? n = e : (n = this.nextId(), t = e), void 0 !== this._annotations[n]) throw new Error(`Id ${n} is already in use.`);
+        if (pi.is(e) ? n = e : (n = this.nextId(), t = e), void 0 !== this._annotations[n]) throw new Error(`Id ${n} is already in use.`);
         if (void 0 === t) throw new Error(`No annotation provided for id ${n}`);
         return this._annotations[n] = t, this._size++, n
     }
     nextId() {
         return this._counter++, this._counter.toString()
     }
-}(Zi = Xi || (Xi = {})).create = function(e) {
+}(Mi = Si || (Si = {})).create = function(e) {
     return {
         uri: e
     }
-}, Zi.is = function(e) {
+}, Mi.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.string(t.uri)
-}, (es = Yi || (Yi = {})).create = function(e, t) {
+    return oa.defined(t) && oa.string(t.uri)
+}, (_i = Di || (Di = {})).create = function(e, t) {
     return {
         uri: e,
         version: t
     }
-}, es.is = function(e) {
+}, _i.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.string(t.uri) && _a.integer(t.version)
-}, (ns = ts || (ts = {})).create = function(e, t) {
+    return oa.defined(t) && oa.string(t.uri) && oa.integer(t.version)
+}, (Pi = Ei || (Ei = {})).create = function(e, t) {
     return {
         uri: e,
         version: t
     }
-}, ns.is = function(e) {
+}, Pi.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.string(t.uri) && (null === t.version || _a.integer(t.version))
-}, (os = rs || (rs = {})).create = function(e, t, n, r) {
+    return oa.defined(t) && oa.string(t.uri) && (null === t.version || oa.integer(t.version))
+}, (Ni = Oi || (Oi = {})).create = function(e, t, n, r) {
     return {
         uri: e,
         languageId: t,
         version: n,
         text: r
     }
-}, os.is = function(e) {
+}, Ni.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.string(t.uri) && _a.string(t.languageId) && _a.integer(t.version) && _a.string(t.text)
-}, (ss = is || (is = {})).PlainText = "plaintext", ss.Markdown = "markdown", ss.is = function(e) {
+    return oa.defined(t) && oa.string(t.uri) && oa.string(t.languageId) && oa.integer(t.version) && oa.string(t.text)
+}, (qi = ji || (ji = {})).PlainText = "plaintext", qi.Markdown = "markdown", qi.is = function(e) {
     const t = e;
-    return t === ss.PlainText || t === ss.Markdown
-}, (as || (as = {})).is = function(e) {
+    return t === qi.PlainText || t === qi.Markdown
+}, (Li || (Li = {})).is = function(e) {
     const t = e;
-    return _a.objectLiteral(e) && is.is(t.kind) && _a.string(t.value)
-}, (ls = cs || (cs = {})).Text = 1, ls.Method = 2, ls.Function = 3, ls.Constructor = 4, ls.Field = 5, ls.Variable = 6, ls.Class = 7, ls.Interface = 8, ls.Module = 9, ls.Property = 10, ls.Unit = 11, ls.Value = 12, ls.Enum = 13, ls.Keyword = 14, ls.Snippet = 15, ls.Color = 16, ls.File = 17, ls.Reference = 18, ls.Folder = 19, ls.EnumMember = 20, ls.Constant = 21, ls.Struct = 22, ls.Event = 23, ls.Operator = 24, ls.TypeParameter = 25, (ds = us || (us = {})).PlainText = 1, ds.Snippet = 2, (hs || (hs = {})).Deprecated = 1, (ps = fs || (fs = {})).create = function(e, t, n) {
+    return oa.objectLiteral(e) && ji.is(t.kind) && oa.string(t.value)
+}, (Ii = Ai || (Ai = {})).Text = 1, Ii.Method = 2, Ii.Function = 3, Ii.Constructor = 4, Ii.Field = 5, Ii.Variable = 6, Ii.Class = 7, Ii.Interface = 8, Ii.Module = 9, Ii.Property = 10, Ii.Unit = 11, Ii.Value = 12, Ii.Enum = 13, Ii.Keyword = 14, Ii.Snippet = 15, Ii.Color = 16, Ii.File = 17, Ii.Reference = 18, Ii.Folder = 19, Ii.EnumMember = 20, Ii.Constant = 21, Ii.Struct = 22, Ii.Event = 23, Ii.Operator = 24, Ii.TypeParameter = 25, (Fi = Bi || (Bi = {})).PlainText = 1, Fi.Snippet = 2, (Wi || (Wi = {})).Deprecated = 1, (Ki = Hi || (Hi = {})).create = function(e, t, n) {
     return {
         newText: e,
         insert: t,
         replace: n
     }
-}, ps.is = function(e) {
+}, Ki.is = function(e) {
     const t = e;
-    return t && _a.string(t.newText) && ci.is(t.insert) && ci.is(t.replace)
-}, (gs = ms || (ms = {})).asIs = 1, gs.adjustIndentation = 2, (vs || (vs = {})).is = function(e) {
+    return t && oa.string(t.newText) && Ao.is(t.insert) && Ao.is(t.replace)
+}, (Vi = Ui || (Ui = {})).asIs = 1, Vi.adjustIndentation = 2, ($i || ($i = {})).is = function(e) {
     const t = e;
-    return t && (_a.string(t.detail) || void 0 === t.detail) && (_a.string(t.description) || void 0 === t.description)
-}, (ys || (ys = {})).create = function(e) {
+    return t && (oa.string(t.detail) || void 0 === t.detail) && (oa.string(t.description) || void 0 === t.description)
+}, (zi || (zi = {})).create = function(e) {
     return {
         label: e
     }
-}, (bs || (bs = {})).create = function(e, t) {
+}, (Ji || (Ji = {})).create = function(e, t) {
     return {
         items: e || [],
         isIncomplete: !!t
     }
-}, (Cs = ws || (ws = {})).fromPlainText = function(e) {
+}, (Gi = Qi || (Qi = {})).fromPlainText = function(e) {
     return e.replace(/[\\`*_{}[\]()#+\-.!]/g, "\\$&")
-}, Cs.is = function(e) {
+}, Gi.is = function(e) {
     const t = e;
-    return _a.string(t) || _a.objectLiteral(t) && _a.string(t.language) && _a.string(t.value)
-}, (xs || (xs = {})).is = function(e) {
+    return oa.string(t) || oa.objectLiteral(t) && oa.string(t.language) && oa.string(t.value)
+}, (Xi || (Xi = {})).is = function(e) {
     let t = e;
-    return !!t && _a.objectLiteral(t) && (as.is(t.contents) || ws.is(t.contents) || _a.typedArray(t.contents, ws.is)) && (void 0 === e.range || ci.is(e.range))
-}, (ks || (ks = {})).create = function(e, t) {
+    return !!t && oa.objectLiteral(t) && (Li.is(t.contents) || Qi.is(t.contents) || oa.typedArray(t.contents, Qi.is)) && (void 0 === e.range || Ao.is(e.range))
+}, (Zi || (Zi = {})).create = function(e, t) {
     return t ? {
         label: e,
         documentation: t
     } : {
         label: e
     }
-}, (Rs || (Rs = {})).create = function(e, t, ...n) {
+}, (Yi || (Yi = {})).create = function(e, t, ...n) {
     let r = {
         label: e
     };
-    return _a.defined(t) && (r.documentation = t), _a.defined(n) ? r.parameters = n : r.parameters = [], r
-}, (Ss = Ts || (Ts = {})).Text = 1, Ss.Read = 2, Ss.Write = 3, (Ms || (Ms = {})).create = function(e, t) {
+    return oa.defined(t) && (r.documentation = t), oa.defined(n) ? r.parameters = n : r.parameters = [], r
+}, (ts = es || (es = {})).Text = 1, ts.Read = 2, ts.Write = 3, (ns || (ns = {})).create = function(e, t) {
     let n = {
         range: e
     };
-    return _a.number(t) && (n.kind = t), n
-}, (_s = Ds || (Ds = {})).File = 1, _s.Module = 2, _s.Namespace = 3, _s.Package = 4, _s.Class = 5, _s.Method = 6, _s.Property = 7, _s.Field = 8, _s.Constructor = 9, _s.Enum = 10, _s.Interface = 11, _s.Function = 12, _s.Variable = 13, _s.Constant = 14, _s.String = 15, _s.Number = 16, _s.Boolean = 17, _s.Array = 18, _s.Object = 19, _s.Key = 20, _s.Null = 21, _s.EnumMember = 22, _s.Struct = 23, _s.Event = 24, _s.Operator = 25, _s.TypeParameter = 26, (Es || (Es = {})).Deprecated = 1, (Ps || (Ps = {})).create = function(e, t, n, r, o) {
+    return oa.number(t) && (n.kind = t), n
+}, (os = rs || (rs = {})).File = 1, os.Module = 2, os.Namespace = 3, os.Package = 4, os.Class = 5, os.Method = 6, os.Property = 7, os.Field = 8, os.Constructor = 9, os.Enum = 10, os.Interface = 11, os.Function = 12, os.Variable = 13, os.Constant = 14, os.String = 15, os.Number = 16, os.Boolean = 17, os.Array = 18, os.Object = 19, os.Key = 20, os.Null = 21, os.EnumMember = 22, os.Struct = 23, os.Event = 24, os.Operator = 25, os.TypeParameter = 26, (is || (is = {})).Deprecated = 1, (ss || (ss = {})).create = function(e, t, n, r, o) {
     let i = {
         name: e,
         kind: t,
         location: {
             uri: r,
             range: n
         }
     };
     return o && (i.containerName = o), i
-}, (Os || (Os = {})).create = function(e, t, n, r) {
+}, (as || (as = {})).create = function(e, t, n, r) {
     return void 0 !== r ? {
         name: e,
         kind: t,
         location: {
             uri: n,
             range: r
         }
     } : {
         name: e,
         kind: t,
         location: {
             uri: n
         }
     }
-}, (js = Ns || (Ns = {})).create = function(e, t, n, r, o, i) {
+}, (ls = cs || (cs = {})).create = function(e, t, n, r, o, i) {
     let s = {
         name: e,
         detail: t,
         kind: n,
         range: r,
         selectionRange: o
     };
     return void 0 !== i && (s.children = i), s
-}, js.is = function(e) {
+}, ls.is = function(e) {
     let t = e;
-    return t && _a.string(t.name) && _a.number(t.kind) && ci.is(t.range) && ci.is(t.selectionRange) && (void 0 === t.detail || _a.string(t.detail)) && (void 0 === t.deprecated || _a.boolean(t.deprecated)) && (void 0 === t.children || Array.isArray(t.children)) && (void 0 === t.tags || Array.isArray(t.tags))
-}, (Ls = qs || (qs = {})).Empty = "", Ls.QuickFix = "quickfix", Ls.Refactor = "refactor", Ls.RefactorExtract = "refactor.extract", Ls.RefactorInline = "refactor.inline", Ls.RefactorRewrite = "refactor.rewrite", Ls.Source = "source", Ls.SourceOrganizeImports = "source.organizeImports", Ls.SourceFixAll = "source.fixAll", (Is = As || (As = {})).Invoked = 1, Is.Automatic = 2, (Fs = Bs || (Bs = {})).create = function(e, t, n) {
+    return t && oa.string(t.name) && oa.number(t.kind) && Ao.is(t.range) && Ao.is(t.selectionRange) && (void 0 === t.detail || oa.string(t.detail)) && (void 0 === t.deprecated || oa.boolean(t.deprecated)) && (void 0 === t.children || Array.isArray(t.children)) && (void 0 === t.tags || Array.isArray(t.tags))
+}, (ds = us || (us = {})).Empty = "", ds.QuickFix = "quickfix", ds.Refactor = "refactor", ds.RefactorExtract = "refactor.extract", ds.RefactorInline = "refactor.inline", ds.RefactorRewrite = "refactor.rewrite", ds.Source = "source", ds.SourceOrganizeImports = "source.organizeImports", ds.SourceFixAll = "source.fixAll", (fs = hs || (hs = {})).Invoked = 1, fs.Automatic = 2, (ms = ps || (ps = {})).create = function(e, t, n) {
     let r = {
         diagnostics: e
     };
     return null != t && (r.only = t), null != n && (r.triggerKind = n), r
-}, Fs.is = function(e) {
+}, ms.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.typedArray(t.diagnostics, Pi.is) && (void 0 === t.only || _a.typedArray(t.only, _a.string)) && (void 0 === t.triggerKind || t.triggerKind === As.Invoked || t.triggerKind === As.Automatic)
-}, (Hs = Ws || (Ws = {})).create = function(e, t, n) {
+    return oa.defined(t) && oa.typedArray(t.diagnostics, si.is) && (void 0 === t.only || oa.typedArray(t.only, oa.string)) && (void 0 === t.triggerKind || t.triggerKind === hs.Invoked || t.triggerKind === hs.Automatic)
+}, (vs = gs || (gs = {})).create = function(e, t, n) {
     let r = {
             title: e
         },
         o = !0;
-    return "string" == typeof t ? (o = !1, r.kind = t) : Ni.is(t) ? r.command = t : r.edit = t, o && void 0 !== n && (r.kind = n), r
-}, Hs.is = function(e) {
+    return "string" == typeof t ? (o = !1, r.kind = t) : ci.is(t) ? r.command = t : r.edit = t, o && void 0 !== n && (r.kind = n), r
+}, vs.is = function(e) {
     let t = e;
-    return t && _a.string(t.title) && (void 0 === t.diagnostics || _a.typedArray(t.diagnostics, Pi.is)) && (void 0 === t.kind || _a.string(t.kind)) && (void 0 !== t.edit || void 0 !== t.command) && (void 0 === t.command || Ni.is(t.command)) && (void 0 === t.isPreferred || _a.boolean(t.isPreferred)) && (void 0 === t.edit || Gi.is(t.edit))
-}, (Us = Ks || (Ks = {})).create = function(e, t) {
+    return t && oa.string(t.title) && (void 0 === t.diagnostics || oa.typedArray(t.diagnostics, si.is)) && (void 0 === t.kind || oa.string(t.kind)) && (void 0 !== t.edit || void 0 !== t.command) && (void 0 === t.command || ci.is(t.command)) && (void 0 === t.isPreferred || oa.boolean(t.isPreferred)) && (void 0 === t.edit || Ti.is(t.edit))
+}, (bs = ys || (ys = {})).create = function(e, t) {
     let n = {
         range: e
     };
-    return _a.defined(t) && (n.data = t), n
-}, Us.is = function(e) {
+    return oa.defined(t) && (n.data = t), n
+}, bs.is = function(e) {
     let t = e;
-    return _a.defined(t) && ci.is(t.range) && (_a.undefined(t.command) || Ni.is(t.command))
-}, ($s = Vs || (Vs = {})).create = function(e, t) {
+    return oa.defined(t) && Ao.is(t.range) && (oa.undefined(t.command) || ci.is(t.command))
+}, (Cs = ws || (ws = {})).create = function(e, t) {
     return {
         tabSize: e,
         insertSpaces: t
     }
-}, $s.is = function(e) {
+}, Cs.is = function(e) {
     let t = e;
-    return _a.defined(t) && _a.uinteger(t.tabSize) && _a.boolean(t.insertSpaces)
-}, (Js = zs || (zs = {})).create = function(e, t, n) {
+    return oa.defined(t) && oa.uinteger(t.tabSize) && oa.boolean(t.insertSpaces)
+}, (ks = xs || (xs = {})).create = function(e, t, n) {
     return {
         range: e,
         target: t,
         data: n
     }
-}, Js.is = function(e) {
+}, ks.is = function(e) {
     let t = e;
-    return _a.defined(t) && ci.is(t.range) && (_a.undefined(t.target) || _a.string(t.target))
-}, (Gs = Qs || (Qs = {})).create = function(e, t) {
+    return oa.defined(t) && Ao.is(t.range) && (oa.undefined(t.target) || oa.string(t.target))
+}, (Ts = Rs || (Rs = {})).create = function(e, t) {
     return {
         range: e,
         parent: t
     }
-}, Gs.is = function(e) {
+}, Ts.is = function(e) {
     let t = e;
-    return _a.objectLiteral(t) && ci.is(t.range) && (void 0 === t.parent || Gs.is(t.parent))
-}, (Zs = Xs || (Xs = {})).namespace = "namespace", Zs.type = "type", Zs.class = "class", Zs.enum = "enum", Zs.interface = "interface", Zs.struct = "struct", Zs.typeParameter = "typeParameter", Zs.parameter = "parameter", Zs.variable = "variable", Zs.property = "property", Zs.enumMember = "enumMember", Zs.event = "event", Zs.function = "function", Zs.method = "method", Zs.macro = "macro", Zs.keyword = "keyword", Zs.modifier = "modifier", Zs.comment = "comment", Zs.string = "string", Zs.number = "number", Zs.regexp = "regexp", Zs.operator = "operator", Zs.decorator = "decorator", (ea = Ys || (Ys = {})).declaration = "declaration", ea.definition = "definition", ea.readonly = "readonly", ea.static = "static", ea.deprecated = "deprecated", ea.abstract = "abstract", ea.async = "async", ea.modification = "modification", ea.documentation = "documentation", ea.defaultLibrary = "defaultLibrary", (ta || (ta = {})).is = function(e) {
+    return oa.objectLiteral(t) && Ao.is(t.range) && (void 0 === t.parent || Ts.is(t.parent))
+}, (Ms = Ss || (Ss = {})).namespace = "namespace", Ms.type = "type", Ms.class = "class", Ms.enum = "enum", Ms.interface = "interface", Ms.struct = "struct", Ms.typeParameter = "typeParameter", Ms.parameter = "parameter", Ms.variable = "variable", Ms.property = "property", Ms.enumMember = "enumMember", Ms.event = "event", Ms.function = "function", Ms.method = "method", Ms.macro = "macro", Ms.keyword = "keyword", Ms.modifier = "modifier", Ms.comment = "comment", Ms.string = "string", Ms.number = "number", Ms.regexp = "regexp", Ms.operator = "operator", Ms.decorator = "decorator", (_s = Ds || (Ds = {})).declaration = "declaration", _s.definition = "definition", _s.readonly = "readonly", _s.static = "static", _s.deprecated = "deprecated", _s.abstract = "abstract", _s.async = "async", _s.modification = "modification", _s.documentation = "documentation", _s.defaultLibrary = "defaultLibrary", (Es || (Es = {})).is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && (void 0 === t.resultId || "string" == typeof t.resultId) && Array.isArray(t.data) && (0 === t.data.length || "number" == typeof t.data[0])
-}, (ra = na || (na = {})).create = function(e, t) {
+    return oa.objectLiteral(t) && (void 0 === t.resultId || "string" == typeof t.resultId) && Array.isArray(t.data) && (0 === t.data.length || "number" == typeof t.data[0])
+}, (Os = Ps || (Ps = {})).create = function(e, t) {
     return {
         range: e,
         text: t
     }
-}, ra.is = function(e) {
+}, Os.is = function(e) {
     const t = e;
-    return null != t && ci.is(t.range) && _a.string(t.text)
-}, (ia = oa || (oa = {})).create = function(e, t, n) {
+    return null != t && Ao.is(t.range) && oa.string(t.text)
+}, (js = Ns || (Ns = {})).create = function(e, t, n) {
     return {
         range: e,
         variableName: t,
         caseSensitiveLookup: n
     }
-}, ia.is = function(e) {
+}, js.is = function(e) {
     const t = e;
-    return null != t && ci.is(t.range) && _a.boolean(t.caseSensitiveLookup) && (_a.string(t.variableName) || void 0 === t.variableName)
-}, (aa = sa || (sa = {})).create = function(e, t) {
+    return null != t && Ao.is(t.range) && oa.boolean(t.caseSensitiveLookup) && (oa.string(t.variableName) || void 0 === t.variableName)
+}, (Ls = qs || (qs = {})).create = function(e, t) {
     return {
         range: e,
         expression: t
     }
-}, aa.is = function(e) {
+}, Ls.is = function(e) {
     const t = e;
-    return null != t && ci.is(t.range) && (_a.string(t.expression) || void 0 === t.expression)
-}, (la = ca || (ca = {})).create = function(e, t) {
+    return null != t && Ao.is(t.range) && (oa.string(t.expression) || void 0 === t.expression)
+}, (Is = As || (As = {})).create = function(e, t) {
     return {
         frameId: e,
         stoppedLocation: t
     }
-}, la.is = function(e) {
+}, Is.is = function(e) {
     const t = e;
-    return _a.defined(t) && ci.is(e.stoppedLocation)
-}, (da = ua || (ua = {})).Type = 1, da.Parameter = 2, da.is = function(e) {
+    return oa.defined(t) && Ao.is(e.stoppedLocation)
+}, (Fs = Bs || (Bs = {})).Type = 1, Fs.Parameter = 2, Fs.is = function(e) {
     return 1 === e || 2 === e
-}, (fa = ha || (ha = {})).create = function(e) {
+}, (Hs = Ws || (Ws = {})).create = function(e) {
     return {
         value: e
     }
-}, fa.is = function(e) {
+}, Hs.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && (void 0 === t.tooltip || _a.string(t.tooltip) || as.is(t.tooltip)) && (void 0 === t.location || ui.is(t.location)) && (void 0 === t.command || Ni.is(t.command))
-}, (ma = pa || (pa = {})).create = function(e, t, n) {
+    return oa.objectLiteral(t) && (void 0 === t.tooltip || oa.string(t.tooltip) || Li.is(t.tooltip)) && (void 0 === t.location || Bo.is(t.location)) && (void 0 === t.command || ci.is(t.command))
+}, (Us = Ks || (Ks = {})).create = function(e, t, n) {
     const r = {
         position: e,
         label: t
     };
     return void 0 !== n && (r.kind = n), r
-}, ma.is = function(e) {
+}, Us.is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && si.is(t.position) && (_a.string(t.label) || _a.typedArray(t.label, ha.is)) && (void 0 === t.kind || ua.is(t.kind)) && void 0 === t.textEdits || _a.typedArray(t.textEdits, qi.is) && (void 0 === t.tooltip || _a.string(t.tooltip) || as.is(t.tooltip)) && (void 0 === t.paddingLeft || _a.boolean(t.paddingLeft)) && (void 0 === t.paddingRight || _a.boolean(t.paddingRight))
-}, (ga || (ga = {})).createSnippet = function(e) {
+    return oa.objectLiteral(t) && qo.is(t.position) && (oa.string(t.label) || oa.typedArray(t.label, Ws.is)) && (void 0 === t.kind || Bs.is(t.kind)) && void 0 === t.textEdits || oa.typedArray(t.textEdits, ui.is) && (void 0 === t.tooltip || oa.string(t.tooltip) || Li.is(t.tooltip)) && (void 0 === t.paddingLeft || oa.boolean(t.paddingLeft)) && (void 0 === t.paddingRight || oa.boolean(t.paddingRight))
+}, (Vs || (Vs = {})).createSnippet = function(e) {
     return {
         kind: "snippet",
         value: e
     }
-}, (va || (va = {})).create = function(e, t, n, r) {
+}, ($s || ($s = {})).create = function(e, t, n, r) {
     return {
         insertText: e,
         filterText: t,
         range: n,
         command: r
     }
-}, (ya || (ya = {})).create = function(e) {
+}, (zs || (zs = {})).create = function(e) {
     return {
         items: e
     }
-}, (wa = ba || (ba = {})).Invoked = 0, wa.Automatic = 1, (Ca || (Ca = {})).create = function(e, t) {
+}, (Qs = Js || (Js = {})).Invoked = 0, Qs.Automatic = 1, (Gs || (Gs = {})).create = function(e, t) {
     return {
         range: e,
         text: t
     }
-}, (xa || (xa = {})).create = function(e, t) {
+}, (Xs || (Xs = {})).create = function(e, t) {
     return {
         triggerKind: e,
         selectedCompletionInfo: t
     }
-}, (ka || (ka = {})).is = function(e) {
+}, (Zs || (Zs = {})).is = function(e) {
     const t = e;
-    return _a.objectLiteral(t) && ti.is(t.uri) && _a.string(t.name)
+    return oa.objectLiteral(t) && Eo.is(t.uri) && oa.string(t.name)
 };
-var Da, _a;
+var ra, oa;
 ! function(e) {
     function t(e, n) {
         if (e.length <= 1) return e;
         const r = e.length / 2 | 0,
             o = e.slice(0, r),
             i = e.slice(r);
         t(o, n), t(i, n);
@@ -10503,18 +10543,18 @@
             e[c++] = t <= 0 ? o[s++] : i[a++]
         }
         for (; s < o.length;) e[c++] = o[s++];
         for (; a < i.length;) e[c++] = i[a++];
         return e
     }
     e.create = function(e, t, n, r) {
-        return new Ea(e, t, n, r)
+        return new ia(e, t, n, r)
     }, e.is = function(e) {
         let t = e;
-        return !!(_a.defined(t) && _a.string(t.uri) && (_a.undefined(t.languageId) || _a.string(t.languageId)) && _a.uinteger(t.lineCount) && _a.func(t.getText) && _a.func(t.positionAt) && _a.func(t.offsetAt))
+        return !!(oa.defined(t) && oa.string(t.uri) && (oa.undefined(t.languageId) || oa.string(t.languageId)) && oa.uinteger(t.lineCount) && oa.func(t.getText) && oa.func(t.positionAt) && oa.func(t.offsetAt))
     }, e.applyEdits = function(e, n) {
         let r = e.getText(),
             o = t(n, ((e, t) => {
                 let n = e.range.start.line - t.range.start.line;
                 return 0 === n ? e.range.start.character - t.range.start.character : n
             })),
             i = r.length;
@@ -10523,16 +10563,16 @@
                 s = e.offsetAt(n.range.start),
                 a = e.offsetAt(n.range.end);
             if (!(a <= i)) throw new Error("Overlapping edit");
             r = r.substring(0, s) + n.newText + r.substring(a, r.length), i = s
         }
         return r
     }
-}(Da || (Da = {}));
-class Ea {
+}(ra || (ra = {}));
+class ia {
     constructor(e, t, n, r) {
         this._uri = e, this._languageId = t, this._version = n, this._content = r, this._lineOffsets = void 0
     }
     get uri() {
         return this._uri
     }
     get languageId() {
@@ -10567,21 +10607,21 @@
         return this._lineOffsets
     }
     positionAt(e) {
         e = Math.max(Math.min(e, this._content.length), 0);
         let t = this.getLineOffsets(),
             n = 0,
             r = t.length;
-        if (0 === r) return si.create(0, e);
+        if (0 === r) return qo.create(0, e);
         for (; n < r;) {
             let o = Math.floor((n + r) / 2);
             t[o] > e ? r = o : n = o + 1
         }
         let o = n - 1;
-        return si.create(o, e - t[o])
+        return qo.create(o, e - t[o])
     }
     offsetAt(e) {
         let t = this.getLineOffsets();
         if (e.line >= t.length) return this._content.length;
         if (e.line < 0) return 0;
         let n = t[e.line],
             r = e.line + 1 < t.length ? t[e.line + 1] : this._content.length;
@@ -10611,541 +10651,541 @@
     }, e.func = function(e) {
         return "[object Function]" === t.call(e)
     }, e.objectLiteral = function(e) {
         return null !== e && "object" == typeof e
     }, e.typedArray = function(e, t) {
         return Array.isArray(e) && e.every(t)
     }
-}(_a || (_a = {}));
-const Pa = ee(Object.freeze(Object.defineProperty({
+}(oa || (oa = {}));
+const sa = ee(Object.freeze(Object.defineProperty({
     __proto__: null,
     get AnnotatedTextEdit() {
-        return Fi
+        return mi
     },
     get ChangeAnnotation() {
-        return Ai
+        return hi
     },
     get ChangeAnnotationIdentifier() {
-        return Bi
+        return pi
     },
     get CodeAction() {
-        return Ws
+        return gs
     },
     get CodeActionContext() {
-        return Bs
+        return ps
     },
     get CodeActionKind() {
-        return qs
+        return us
     },
     get CodeActionTriggerKind() {
-        return As
+        return hs
     },
     get CodeDescription() {
-        return Ei
+        return ii
     },
     get CodeLens() {
-        return Ks
+        return ys
     },
     get Color() {
-        return pi
+        return Ko
     },
     get ColorInformation() {
-        return gi
+        return Vo
     },
     get ColorPresentation() {
-        return yi
+        return zo
     },
     get Command() {
-        return Ni
+        return ci
     },
     get CompletionItem() {
-        return ys
+        return zi
     },
     get CompletionItemKind() {
-        return cs
+        return Ai
     },
     get CompletionItemLabelDetails() {
-        return vs
+        return $i
     },
     get CompletionItemTag() {
-        return hs
+        return Wi
     },
     get CompletionList() {
-        return bs
+        return Ji
     },
     get CreateFile() {
-        return Ui
+        return bi
     },
     get DeleteFile() {
-        return Ji
+        return ki
     },
     get Diagnostic() {
-        return Pi
+        return si
     },
     get DiagnosticRelatedInformation() {
-        return Ri
+        return Yo
     },
     get DiagnosticSeverity() {
-        return Si
+        return ti
     },
     get DiagnosticTag() {
-        return Di
+        return ri
     },
     get DocumentHighlight() {
-        return Ms
+        return ns
     },
     get DocumentHighlightKind() {
-        return Ts
+        return es
     },
     get DocumentLink() {
-        return zs
+        return xs
     },
     get DocumentSymbol() {
-        return Ns
+        return cs
     },
     get DocumentUri() {
-        return ei
+        return _o
     },
     EOL: ["\n", "\r\n", "\r"],
     get FoldingRange() {
-        return xi
+        return Xo
     },
     get FoldingRangeKind() {
-        return wi
+        return Qo
     },
     get FormattingOptions() {
-        return Vs
+        return ws
     },
     get Hover() {
-        return xs
+        return Xi
     },
     get InlayHint() {
-        return pa
+        return Ks
     },
     get InlayHintKind() {
-        return ua
+        return Bs
     },
     get InlayHintLabelPart() {
-        return ha
+        return Ws
     },
     get InlineCompletionContext() {
-        return xa
+        return Xs
     },
     get InlineCompletionItem() {
-        return va
+        return $s
     },
     get InlineCompletionList() {
-        return ya
+        return zs
     },
     get InlineCompletionTriggerKind() {
-        return ba
+        return Js
     },
     get InlineValueContext() {
-        return ca
+        return As
     },
     get InlineValueEvaluatableExpression() {
-        return sa
+        return qs
     },
     get InlineValueText() {
-        return na
+        return Ps
     },
     get InlineValueVariableLookup() {
-        return oa
+        return Ns
     },
     get InsertReplaceEdit() {
-        return fs
+        return Hi
     },
     get InsertTextFormat() {
-        return us
+        return Bi
     },
     get InsertTextMode() {
-        return ms
+        return Ui
     },
     get Location() {
-        return ui
+        return Bo
     },
     get LocationLink() {
-        return hi
+        return Wo
     },
     get MarkedString() {
-        return ws
+        return Qi
     },
     get MarkupContent() {
-        return as
+        return Li
     },
     get MarkupKind() {
-        return is
+        return ji
     },
     get OptionalVersionedTextDocumentIdentifier() {
-        return ts
+        return Ei
     },
     get ParameterInformation() {
-        return ks
+        return Zi
     },
     get Position() {
-        return si
+        return qo
     },
     get Range() {
-        return ci
+        return Ao
     },
     get RenameFile() {
-        return $i
+        return Ci
     },
     get SelectedCompletionInfo() {
-        return Ca
+        return Gs
     },
     get SelectionRange() {
-        return Qs
+        return Rs
     },
     get SemanticTokenModifiers() {
-        return Ys
+        return Ds
     },
     get SemanticTokenTypes() {
-        return Xs
+        return Ss
     },
     get SemanticTokens() {
-        return ta
+        return Es
     },
     get SignatureInformation() {
-        return Rs
+        return Yi
     },
     get StringValue() {
-        return ga
+        return Vs
     },
     get SymbolInformation() {
-        return Ps
+        return ss
     },
     get SymbolKind() {
-        return Ds
+        return rs
     },
     get SymbolTag() {
-        return Es
+        return is
     },
     get TextDocument() {
-        return Da
+        return ra
     },
     get TextDocumentEdit() {
-        return Hi
+        return vi
     },
     get TextDocumentIdentifier() {
-        return Xi
+        return Si
     },
     get TextDocumentItem() {
-        return rs
+        return Oi
     },
     get TextEdit() {
-        return qi
+        return ui
     },
     get URI() {
-        return ti
+        return Eo
     },
     get VersionedTextDocumentIdentifier() {
-        return Yi
+        return Di
     },
     WorkspaceChange: class {
         constructor(e) {
-            this._textEditChanges = Object.create(null), void 0 !== e ? (this._workspaceEdit = e, e.documentChanges ? (this._changeAnnotations = new Ma(e.changeAnnotations), e.changeAnnotations = this._changeAnnotations.all(), e.documentChanges.forEach((e => {
-                if (Hi.is(e)) {
-                    const t = new Sa(e.edits, this._changeAnnotations);
+            this._textEditChanges = Object.create(null), void 0 !== e ? (this._workspaceEdit = e, e.documentChanges ? (this._changeAnnotations = new na(e.changeAnnotations), e.changeAnnotations = this._changeAnnotations.all(), e.documentChanges.forEach((e => {
+                if (vi.is(e)) {
+                    const t = new ta(e.edits, this._changeAnnotations);
                     this._textEditChanges[e.textDocument.uri] = t
                 }
             }))) : e.changes && Object.keys(e.changes).forEach((t => {
-                const n = new Sa(e.changes[t]);
+                const n = new ta(e.changes[t]);
                 this._textEditChanges[t] = n
             }))) : this._workspaceEdit = {}
         }
         get edit() {
             return this.initDocumentChanges(), void 0 !== this._changeAnnotations && (0 === this._changeAnnotations.size ? this._workspaceEdit.changeAnnotations = void 0 : this._workspaceEdit.changeAnnotations = this._changeAnnotations.all()), this._workspaceEdit
         }
         getTextEditChange(e) {
-            if (ts.is(e)) {
+            if (Ei.is(e)) {
                 if (this.initDocumentChanges(), void 0 === this._workspaceEdit.documentChanges) throw new Error("Workspace edit is not configured for document changes.");
                 const t = {
                     uri: e.uri,
                     version: e.version
                 };
                 let n = this._textEditChanges[t.uri];
                 if (!n) {
                     const e = [],
                         r = {
                             textDocument: t,
                             edits: e
                         };
-                    this._workspaceEdit.documentChanges.push(r), n = new Sa(e, this._changeAnnotations), this._textEditChanges[t.uri] = n
+                    this._workspaceEdit.documentChanges.push(r), n = new ta(e, this._changeAnnotations), this._textEditChanges[t.uri] = n
                 }
                 return n
             } {
                 if (this.initChanges(), void 0 === this._workspaceEdit.changes) throw new Error("Workspace edit is not configured for normal text edit changes.");
                 let t = this._textEditChanges[e];
                 if (!t) {
                     let n = [];
-                    this._workspaceEdit.changes[e] = n, t = new Sa(n), this._textEditChanges[e] = t
+                    this._workspaceEdit.changes[e] = n, t = new ta(n), this._textEditChanges[e] = t
                 }
                 return t
             }
         }
         initDocumentChanges() {
-            void 0 === this._workspaceEdit.documentChanges && void 0 === this._workspaceEdit.changes && (this._changeAnnotations = new Ma, this._workspaceEdit.documentChanges = [], this._workspaceEdit.changeAnnotations = this._changeAnnotations.all())
+            void 0 === this._workspaceEdit.documentChanges && void 0 === this._workspaceEdit.changes && (this._changeAnnotations = new na, this._workspaceEdit.documentChanges = [], this._workspaceEdit.changeAnnotations = this._changeAnnotations.all())
         }
         initChanges() {
             void 0 === this._workspaceEdit.documentChanges && void 0 === this._workspaceEdit.changes && (this._workspaceEdit.changes = Object.create(null))
         }
         createFile(e, t, n) {
             if (this.initDocumentChanges(), void 0 === this._workspaceEdit.documentChanges) throw new Error("Workspace edit is not configured for document changes.");
             let r, o, i;
-            if (Ai.is(t) || Bi.is(t) ? r = t : n = t, void 0 === r ? o = Ui.create(e, n) : (i = Bi.is(r) ? r : this._changeAnnotations.manage(r), o = Ui.create(e, n, i)), this._workspaceEdit.documentChanges.push(o), void 0 !== i) return i
+            if (hi.is(t) || pi.is(t) ? r = t : n = t, void 0 === r ? o = bi.create(e, n) : (i = pi.is(r) ? r : this._changeAnnotations.manage(r), o = bi.create(e, n, i)), this._workspaceEdit.documentChanges.push(o), void 0 !== i) return i
         }
         renameFile(e, t, n, r) {
             if (this.initDocumentChanges(), void 0 === this._workspaceEdit.documentChanges) throw new Error("Workspace edit is not configured for document changes.");
             let o, i, s;
-            if (Ai.is(n) || Bi.is(n) ? o = n : r = n, void 0 === o ? i = $i.create(e, t, r) : (s = Bi.is(o) ? o : this._changeAnnotations.manage(o), i = $i.create(e, t, r, s)), this._workspaceEdit.documentChanges.push(i), void 0 !== s) return s
+            if (hi.is(n) || pi.is(n) ? o = n : r = n, void 0 === o ? i = Ci.create(e, t, r) : (s = pi.is(o) ? o : this._changeAnnotations.manage(o), i = Ci.create(e, t, r, s)), this._workspaceEdit.documentChanges.push(i), void 0 !== s) return s
         }
         deleteFile(e, t, n) {
             if (this.initDocumentChanges(), void 0 === this._workspaceEdit.documentChanges) throw new Error("Workspace edit is not configured for document changes.");
             let r, o, i;
-            if (Ai.is(t) || Bi.is(t) ? r = t : n = t, void 0 === r ? o = Ji.create(e, n) : (i = Bi.is(r) ? r : this._changeAnnotations.manage(r), o = Ji.create(e, n, i)), this._workspaceEdit.documentChanges.push(o), void 0 !== i) return i
+            if (hi.is(t) || pi.is(t) ? r = t : n = t, void 0 === r ? o = ki.create(e, n) : (i = pi.is(r) ? r : this._changeAnnotations.manage(r), o = ki.create(e, n, i)), this._workspaceEdit.documentChanges.push(o), void 0 !== i) return i
         }
     },
     get WorkspaceEdit() {
-        return Gi
+        return Ti
     },
     get WorkspaceFolder() {
-        return ka
+        return Zs
     },
     get WorkspaceSymbol() {
-        return Os
+        return as
     },
     get integer() {
-        return ni
+        return Po
     },
     get uinteger() {
-        return oi
+        return No
     }
 }, Symbol.toStringTag, {
     value: "Module"
 })));
-var Oa = {};
-Object.defineProperty(Oa, "__esModule", {
+var aa = {};
+Object.defineProperty(aa, "__esModule", {
     value: !0
-}), Oa.ProtocolNotificationType = Oa.ProtocolNotificationType0 = Oa.ProtocolRequestType = Oa.ProtocolRequestType0 = Oa.RegistrationType = Oa.MessageDirection = void 0;
-const Na = Lr;
-var ja, qa;
-(qa = ja || (Oa.MessageDirection = ja = {})).clientToServer = "clientToServer", qa.serverToClient = "serverToClient", qa.both = "both";
-Oa.RegistrationType = class {
+}), aa.ProtocolNotificationType = aa.ProtocolNotificationType0 = aa.ProtocolRequestType = aa.ProtocolRequestType0 = aa.RegistrationType = aa.MessageDirection = void 0;
+const ca = Ir;
+var la, ua;
+(ua = la || (aa.MessageDirection = la = {})).clientToServer = "clientToServer", ua.serverToClient = "serverToClient", ua.both = "both";
+aa.RegistrationType = class {
     constructor(e) {
         this.method = e
     }
 };
-Oa.ProtocolRequestType0 = class extends Na.RequestType0 {
+aa.ProtocolRequestType0 = class extends ca.RequestType0 {
     constructor(e) {
         super(e)
     }
 };
-Oa.ProtocolRequestType = class extends Na.RequestType {
+aa.ProtocolRequestType = class extends ca.RequestType {
     constructor(e) {
-        super(e, Na.ParameterStructures.byName)
+        super(e, ca.ParameterStructures.byName)
     }
 };
-Oa.ProtocolNotificationType0 = class extends Na.NotificationType0 {
+aa.ProtocolNotificationType0 = class extends ca.NotificationType0 {
     constructor(e) {
         super(e)
     }
 };
-Oa.ProtocolNotificationType = class extends Na.NotificationType {
+aa.ProtocolNotificationType = class extends ca.NotificationType {
     constructor(e) {
-        super(e, Na.ParameterStructures.byName)
+        super(e, ca.ParameterStructures.byName)
     }
 };
-var La = {},
-    Aa = {};
+var da = {},
+    ha = {};
 
-function Ia(e) {
+function fa(e) {
     return "string" == typeof e || e instanceof String
 }
 
-function Ba(e) {
+function pa(e) {
     return Array.isArray(e)
 }
-Object.defineProperty(Aa, "__esModule", {
+Object.defineProperty(ha, "__esModule", {
     value: !0
-}), Aa.objectLiteral = Aa.typedArray = Aa.stringArray = Aa.array = Aa.func = Aa.error = Aa.number = Aa.string = Aa.boolean = void 0, Aa.boolean = function(e) {
+}), ha.objectLiteral = ha.typedArray = ha.stringArray = ha.array = ha.func = ha.error = ha.number = ha.string = ha.boolean = void 0, ha.boolean = function(e) {
     return !0 === e || !1 === e
-}, Aa.string = Ia, Aa.number = function(e) {
+}, ha.string = fa, ha.number = function(e) {
     return "number" == typeof e || e instanceof Number
-}, Aa.error = function(e) {
+}, ha.error = function(e) {
     return e instanceof Error
-}, Aa.func = function(e) {
+}, ha.func = function(e) {
     return "function" == typeof e
-}, Aa.array = Ba, Aa.stringArray = function(e) {
-    return Ba(e) && e.every((e => Ia(e)))
-}, Aa.typedArray = function(e, t) {
+}, ha.array = pa, ha.stringArray = function(e) {
+    return pa(e) && e.every((e => fa(e)))
+}, ha.typedArray = function(e, t) {
     return Array.isArray(e) && e.every(t)
-}, Aa.objectLiteral = function(e) {
+}, ha.objectLiteral = function(e) {
     return null !== e && "object" == typeof e
 };
-var Fa = {};
-Object.defineProperty(Fa, "__esModule", {
-    value: !0
-}), Fa.ImplementationRequest = void 0;
-const Wa = Oa;
-var Ha, Ka;
-(Ka = Ha || (Fa.ImplementationRequest = Ha = {})).method = "textDocument/implementation", Ka.messageDirection = Wa.MessageDirection.clientToServer, Ka.type = new Wa.ProtocolRequestType(Ka.method);
-var Ua = {};
-Object.defineProperty(Ua, "__esModule", {
-    value: !0
-}), Ua.TypeDefinitionRequest = void 0;
-const Va = Oa;
-var $a, za;
-(za = $a || (Ua.TypeDefinitionRequest = $a = {})).method = "textDocument/typeDefinition", za.messageDirection = Va.MessageDirection.clientToServer, za.type = new Va.ProtocolRequestType(za.method);
-var Ja = {};
-Object.defineProperty(Ja, "__esModule", {
-    value: !0
-}), Ja.DidChangeWorkspaceFoldersNotification = Ja.WorkspaceFoldersRequest = void 0;
-const Qa = Oa;
-var Ga, Xa, Za, Ya;
-(Xa = Ga || (Ja.WorkspaceFoldersRequest = Ga = {})).method = "workspace/workspaceFolders", Xa.messageDirection = Qa.MessageDirection.serverToClient, Xa.type = new Qa.ProtocolRequestType0(Xa.method), (Ya = Za || (Ja.DidChangeWorkspaceFoldersNotification = Za = {})).method = "workspace/didChangeWorkspaceFolders", Ya.messageDirection = Qa.MessageDirection.clientToServer, Ya.type = new Qa.ProtocolNotificationType(Ya.method);
-var ec = {};
-Object.defineProperty(ec, "__esModule", {
+var ma = {};
+Object.defineProperty(ma, "__esModule", {
     value: !0
-}), ec.ConfigurationRequest = void 0;
-const tc = Oa;
-var nc, rc;
-(rc = nc || (ec.ConfigurationRequest = nc = {})).method = "workspace/configuration", rc.messageDirection = tc.MessageDirection.serverToClient, rc.type = new tc.ProtocolRequestType(rc.method);
-var oc = {};
-Object.defineProperty(oc, "__esModule", {
-    value: !0
-}), oc.ColorPresentationRequest = oc.DocumentColorRequest = void 0;
-const ic = Oa;
-var sc, ac, cc, lc;
-(ac = sc || (oc.DocumentColorRequest = sc = {})).method = "textDocument/documentColor", ac.messageDirection = ic.MessageDirection.clientToServer, ac.type = new ic.ProtocolRequestType(ac.method), (lc = cc || (oc.ColorPresentationRequest = cc = {})).method = "textDocument/colorPresentation", lc.messageDirection = ic.MessageDirection.clientToServer, lc.type = new ic.ProtocolRequestType(lc.method);
-var uc = {};
-Object.defineProperty(uc, "__esModule", {
-    value: !0
-}), uc.FoldingRangeRefreshRequest = uc.FoldingRangeRequest = void 0;
-const dc = Oa;
-var hc, fc, pc, mc;
-(fc = hc || (uc.FoldingRangeRequest = hc = {})).method = "textDocument/foldingRange", fc.messageDirection = dc.MessageDirection.clientToServer, fc.type = new dc.ProtocolRequestType(fc.method), (mc = pc || (uc.FoldingRangeRefreshRequest = pc = {})).method = "workspace/foldingRange/refresh", mc.messageDirection = dc.MessageDirection.serverToClient, mc.type = new dc.ProtocolRequestType0(mc.method);
+}), ma.ImplementationRequest = void 0;
+const ga = aa;
+var va, ya;
+(ya = va || (ma.ImplementationRequest = va = {})).method = "textDocument/implementation", ya.messageDirection = ga.MessageDirection.clientToServer, ya.type = new ga.ProtocolRequestType(ya.method);
+var ba = {};
+Object.defineProperty(ba, "__esModule", {
+    value: !0
+}), ba.TypeDefinitionRequest = void 0;
+const wa = aa;
+var Ca, xa;
+(xa = Ca || (ba.TypeDefinitionRequest = Ca = {})).method = "textDocument/typeDefinition", xa.messageDirection = wa.MessageDirection.clientToServer, xa.type = new wa.ProtocolRequestType(xa.method);
+var ka = {};
+Object.defineProperty(ka, "__esModule", {
+    value: !0
+}), ka.DidChangeWorkspaceFoldersNotification = ka.WorkspaceFoldersRequest = void 0;
+const Ra = aa;
+var Ta, Sa, Ma, Da;
+(Sa = Ta || (ka.WorkspaceFoldersRequest = Ta = {})).method = "workspace/workspaceFolders", Sa.messageDirection = Ra.MessageDirection.serverToClient, Sa.type = new Ra.ProtocolRequestType0(Sa.method), (Da = Ma || (ka.DidChangeWorkspaceFoldersNotification = Ma = {})).method = "workspace/didChangeWorkspaceFolders", Da.messageDirection = Ra.MessageDirection.clientToServer, Da.type = new Ra.ProtocolNotificationType(Da.method);
+var _a = {};
+Object.defineProperty(_a, "__esModule", {
+    value: !0
+}), _a.ConfigurationRequest = void 0;
+const Ea = aa;
+var Pa, Oa;
+(Oa = Pa || (_a.ConfigurationRequest = Pa = {})).method = "workspace/configuration", Oa.messageDirection = Ea.MessageDirection.serverToClient, Oa.type = new Ea.ProtocolRequestType(Oa.method);
+var Na = {};
+Object.defineProperty(Na, "__esModule", {
+    value: !0
+}), Na.ColorPresentationRequest = Na.DocumentColorRequest = void 0;
+const ja = aa;
+var qa, La, Aa, Ia;
+(La = qa || (Na.DocumentColorRequest = qa = {})).method = "textDocument/documentColor", La.messageDirection = ja.MessageDirection.clientToServer, La.type = new ja.ProtocolRequestType(La.method), (Ia = Aa || (Na.ColorPresentationRequest = Aa = {})).method = "textDocument/colorPresentation", Ia.messageDirection = ja.MessageDirection.clientToServer, Ia.type = new ja.ProtocolRequestType(Ia.method);
+var Ba = {};
+Object.defineProperty(Ba, "__esModule", {
+    value: !0
+}), Ba.FoldingRangeRefreshRequest = Ba.FoldingRangeRequest = void 0;
+const Fa = aa;
+var Wa, Ha, Ka, Ua;
+(Ha = Wa || (Ba.FoldingRangeRequest = Wa = {})).method = "textDocument/foldingRange", Ha.messageDirection = Fa.MessageDirection.clientToServer, Ha.type = new Fa.ProtocolRequestType(Ha.method), (Ua = Ka || (Ba.FoldingRangeRefreshRequest = Ka = {})).method = "workspace/foldingRange/refresh", Ua.messageDirection = Fa.MessageDirection.serverToClient, Ua.type = new Fa.ProtocolRequestType0(Ua.method);
+var Va = {};
+Object.defineProperty(Va, "__esModule", {
+    value: !0
+}), Va.DeclarationRequest = void 0;
+const $a = aa;
+var za, Ja;
+(Ja = za || (Va.DeclarationRequest = za = {})).method = "textDocument/declaration", Ja.messageDirection = $a.MessageDirection.clientToServer, Ja.type = new $a.ProtocolRequestType(Ja.method);
+var Qa = {};
+Object.defineProperty(Qa, "__esModule", {
+    value: !0
+}), Qa.SelectionRangeRequest = void 0;
+const Ga = aa;
+var Xa, Za;
+(Za = Xa || (Qa.SelectionRangeRequest = Xa = {})).method = "textDocument/selectionRange", Za.messageDirection = Ga.MessageDirection.clientToServer, Za.type = new Ga.ProtocolRequestType(Za.method);
+var Ya = {};
+Object.defineProperty(Ya, "__esModule", {
+    value: !0
+}), Ya.WorkDoneProgressCancelNotification = Ya.WorkDoneProgressCreateRequest = Ya.WorkDoneProgress = void 0;
+const ec = Ir,
+    tc = aa;
+var nc, rc, oc, ic, sc, ac;
+(rc = nc || (Ya.WorkDoneProgress = nc = {})).type = new ec.ProgressType, rc.is = function(e) {
+    return e === rc.type
+}, (ic = oc || (Ya.WorkDoneProgressCreateRequest = oc = {})).method = "window/workDoneProgress/create", ic.messageDirection = tc.MessageDirection.serverToClient, ic.type = new tc.ProtocolRequestType(ic.method), (ac = sc || (Ya.WorkDoneProgressCancelNotification = sc = {})).method = "window/workDoneProgress/cancel", ac.messageDirection = tc.MessageDirection.clientToServer, ac.type = new tc.ProtocolNotificationType(ac.method);
+var cc = {};
+Object.defineProperty(cc, "__esModule", {
+    value: !0
+}), cc.CallHierarchyOutgoingCallsRequest = cc.CallHierarchyIncomingCallsRequest = cc.CallHierarchyPrepareRequest = void 0;
+const lc = aa;
+var uc, dc, hc, fc, pc, mc;
+(dc = uc || (cc.CallHierarchyPrepareRequest = uc = {})).method = "textDocument/prepareCallHierarchy", dc.messageDirection = lc.MessageDirection.clientToServer, dc.type = new lc.ProtocolRequestType(dc.method), (fc = hc || (cc.CallHierarchyIncomingCallsRequest = hc = {})).method = "callHierarchy/incomingCalls", fc.messageDirection = lc.MessageDirection.clientToServer, fc.type = new lc.ProtocolRequestType(fc.method), (mc = pc || (cc.CallHierarchyOutgoingCallsRequest = pc = {})).method = "callHierarchy/outgoingCalls", mc.messageDirection = lc.MessageDirection.clientToServer, mc.type = new lc.ProtocolRequestType(mc.method);
 var gc = {};
 Object.defineProperty(gc, "__esModule", {
     value: !0
-}), gc.DeclarationRequest = void 0;
-const vc = Oa;
-var yc, bc;
-(bc = yc || (gc.DeclarationRequest = yc = {})).method = "textDocument/declaration", bc.messageDirection = vc.MessageDirection.clientToServer, bc.type = new vc.ProtocolRequestType(bc.method);
-var wc = {};
-Object.defineProperty(wc, "__esModule", {
-    value: !0
-}), wc.SelectionRangeRequest = void 0;
-const Cc = Oa;
-var xc, kc;
-(kc = xc || (wc.SelectionRangeRequest = xc = {})).method = "textDocument/selectionRange", kc.messageDirection = Cc.MessageDirection.clientToServer, kc.type = new Cc.ProtocolRequestType(kc.method);
-var Rc = {};
-Object.defineProperty(Rc, "__esModule", {
-    value: !0
-}), Rc.WorkDoneProgressCancelNotification = Rc.WorkDoneProgressCreateRequest = Rc.WorkDoneProgress = void 0;
-const Tc = Lr,
-    Sc = Oa;
-var Mc, Dc, _c, Ec, Pc, Oc;
-(Dc = Mc || (Rc.WorkDoneProgress = Mc = {})).type = new Tc.ProgressType, Dc.is = function(e) {
-    return e === Dc.type
-}, (Ec = _c || (Rc.WorkDoneProgressCreateRequest = _c = {})).method = "window/workDoneProgress/create", Ec.messageDirection = Sc.MessageDirection.serverToClient, Ec.type = new Sc.ProtocolRequestType(Ec.method), (Oc = Pc || (Rc.WorkDoneProgressCancelNotification = Pc = {})).method = "window/workDoneProgress/cancel", Oc.messageDirection = Sc.MessageDirection.clientToServer, Oc.type = new Sc.ProtocolNotificationType(Oc.method);
+}), gc.SemanticTokensRefreshRequest = gc.SemanticTokensRangeRequest = gc.SemanticTokensDeltaRequest = gc.SemanticTokensRequest = gc.SemanticTokensRegistrationType = gc.TokenFormat = void 0;
+const vc = aa;
+var yc, bc, wc, Cc, xc, kc, Rc, Tc, Sc, Mc, Dc;
+(yc || (gc.TokenFormat = yc = {})).Relative = "relative", (wc = bc || (gc.SemanticTokensRegistrationType = bc = {})).method = "textDocument/semanticTokens", wc.type = new vc.RegistrationType(wc.method), (xc = Cc || (gc.SemanticTokensRequest = Cc = {})).method = "textDocument/semanticTokens/full", xc.messageDirection = vc.MessageDirection.clientToServer, xc.type = new vc.ProtocolRequestType(xc.method), xc.registrationMethod = bc.method, (Rc = kc || (gc.SemanticTokensDeltaRequest = kc = {})).method = "textDocument/semanticTokens/full/delta", Rc.messageDirection = vc.MessageDirection.clientToServer, Rc.type = new vc.ProtocolRequestType(Rc.method), Rc.registrationMethod = bc.method, (Sc = Tc || (gc.SemanticTokensRangeRequest = Tc = {})).method = "textDocument/semanticTokens/range", Sc.messageDirection = vc.MessageDirection.clientToServer, Sc.type = new vc.ProtocolRequestType(Sc.method), Sc.registrationMethod = bc.method, (Dc = Mc || (gc.SemanticTokensRefreshRequest = Mc = {})).method = "workspace/semanticTokens/refresh", Dc.messageDirection = vc.MessageDirection.serverToClient, Dc.type = new vc.ProtocolRequestType0(Dc.method);
+var _c = {};
+Object.defineProperty(_c, "__esModule", {
+    value: !0
+}), _c.ShowDocumentRequest = void 0;
+const Ec = aa;
+var Pc, Oc;
+(Oc = Pc || (_c.ShowDocumentRequest = Pc = {})).method = "window/showDocument", Oc.messageDirection = Ec.MessageDirection.serverToClient, Oc.type = new Ec.ProtocolRequestType(Oc.method);
 var Nc = {};
 Object.defineProperty(Nc, "__esModule", {
     value: !0
-}), Nc.CallHierarchyOutgoingCallsRequest = Nc.CallHierarchyIncomingCallsRequest = Nc.CallHierarchyPrepareRequest = void 0;
-const jc = Oa;
-var qc, Lc, Ac, Ic, Bc, Fc;
-(Lc = qc || (Nc.CallHierarchyPrepareRequest = qc = {})).method = "textDocument/prepareCallHierarchy", Lc.messageDirection = jc.MessageDirection.clientToServer, Lc.type = new jc.ProtocolRequestType(Lc.method), (Ic = Ac || (Nc.CallHierarchyIncomingCallsRequest = Ac = {})).method = "callHierarchy/incomingCalls", Ic.messageDirection = jc.MessageDirection.clientToServer, Ic.type = new jc.ProtocolRequestType(Ic.method), (Fc = Bc || (Nc.CallHierarchyOutgoingCallsRequest = Bc = {})).method = "callHierarchy/outgoingCalls", Fc.messageDirection = jc.MessageDirection.clientToServer, Fc.type = new jc.ProtocolRequestType(Fc.method);
-var Wc = {};
-Object.defineProperty(Wc, "__esModule", {
-    value: !0
-}), Wc.SemanticTokensRefreshRequest = Wc.SemanticTokensRangeRequest = Wc.SemanticTokensDeltaRequest = Wc.SemanticTokensRequest = Wc.SemanticTokensRegistrationType = Wc.TokenFormat = void 0;
-const Hc = Oa;
-var Kc, Uc, Vc, $c, zc, Jc, Qc, Gc, Xc, Zc, Yc;
-(Kc || (Wc.TokenFormat = Kc = {})).Relative = "relative", (Vc = Uc || (Wc.SemanticTokensRegistrationType = Uc = {})).method = "textDocument/semanticTokens", Vc.type = new Hc.RegistrationType(Vc.method), (zc = $c || (Wc.SemanticTokensRequest = $c = {})).method = "textDocument/semanticTokens/full", zc.messageDirection = Hc.MessageDirection.clientToServer, zc.type = new Hc.ProtocolRequestType(zc.method), zc.registrationMethod = Uc.method, (Qc = Jc || (Wc.SemanticTokensDeltaRequest = Jc = {})).method = "textDocument/semanticTokens/full/delta", Qc.messageDirection = Hc.MessageDirection.clientToServer, Qc.type = new Hc.ProtocolRequestType(Qc.method), Qc.registrationMethod = Uc.method, (Xc = Gc || (Wc.SemanticTokensRangeRequest = Gc = {})).method = "textDocument/semanticTokens/range", Xc.messageDirection = Hc.MessageDirection.clientToServer, Xc.type = new Hc.ProtocolRequestType(Xc.method), Xc.registrationMethod = Uc.method, (Yc = Zc || (Wc.SemanticTokensRefreshRequest = Zc = {})).method = "workspace/semanticTokens/refresh", Yc.messageDirection = Hc.MessageDirection.serverToClient, Yc.type = new Hc.ProtocolRequestType0(Yc.method);
-var el = {};
-Object.defineProperty(el, "__esModule", {
-    value: !0
-}), el.ShowDocumentRequest = void 0;
-const tl = Oa;
-var nl, rl;
-(rl = nl || (el.ShowDocumentRequest = nl = {})).method = "window/showDocument", rl.messageDirection = tl.MessageDirection.serverToClient, rl.type = new tl.ProtocolRequestType(rl.method);
-var ol = {};
-Object.defineProperty(ol, "__esModule", {
-    value: !0
-}), ol.LinkedEditingRangeRequest = void 0;
-const il = Oa;
-var sl, al;
-(al = sl || (ol.LinkedEditingRangeRequest = sl = {})).method = "textDocument/linkedEditingRange", al.messageDirection = il.MessageDirection.clientToServer, al.type = new il.ProtocolRequestType(al.method);
-var cl = {};
-Object.defineProperty(cl, "__esModule", {
-    value: !0
-}), cl.WillDeleteFilesRequest = cl.DidDeleteFilesNotification = cl.DidRenameFilesNotification = cl.WillRenameFilesRequest = cl.DidCreateFilesNotification = cl.WillCreateFilesRequest = cl.FileOperationPatternKind = void 0;
-const ll = Oa;
-var ul, dl, hl, fl, pl, ml, gl, vl, yl, bl, wl, Cl, xl, kl;
-(dl = ul || (cl.FileOperationPatternKind = ul = {})).file = "file", dl.folder = "folder", (fl = hl || (cl.WillCreateFilesRequest = hl = {})).method = "workspace/willCreateFiles", fl.messageDirection = ll.MessageDirection.clientToServer, fl.type = new ll.ProtocolRequestType(fl.method), (ml = pl || (cl.DidCreateFilesNotification = pl = {})).method = "workspace/didCreateFiles", ml.messageDirection = ll.MessageDirection.clientToServer, ml.type = new ll.ProtocolNotificationType(ml.method), (vl = gl || (cl.WillRenameFilesRequest = gl = {})).method = "workspace/willRenameFiles", vl.messageDirection = ll.MessageDirection.clientToServer, vl.type = new ll.ProtocolRequestType(vl.method), (bl = yl || (cl.DidRenameFilesNotification = yl = {})).method = "workspace/didRenameFiles", bl.messageDirection = ll.MessageDirection.clientToServer, bl.type = new ll.ProtocolNotificationType(bl.method), (Cl = wl || (cl.DidDeleteFilesNotification = wl = {})).method = "workspace/didDeleteFiles", Cl.messageDirection = ll.MessageDirection.clientToServer, Cl.type = new ll.ProtocolNotificationType(Cl.method), (kl = xl || (cl.WillDeleteFilesRequest = xl = {})).method = "workspace/willDeleteFiles", kl.messageDirection = ll.MessageDirection.clientToServer, kl.type = new ll.ProtocolRequestType(kl.method);
-var Rl = {};
-Object.defineProperty(Rl, "__esModule", {
-    value: !0
-}), Rl.MonikerRequest = Rl.MonikerKind = Rl.UniquenessLevel = void 0;
-const Tl = Oa;
-var Sl, Ml, Dl, _l, El, Pl;
-(Ml = Sl || (Rl.UniquenessLevel = Sl = {})).document = "document", Ml.project = "project", Ml.group = "group", Ml.scheme = "scheme", Ml.global = "global", (_l = Dl || (Rl.MonikerKind = Dl = {})).$import = "import", _l.$export = "export", _l.local = "local", (Pl = El || (Rl.MonikerRequest = El = {})).method = "textDocument/moniker", Pl.messageDirection = Tl.MessageDirection.clientToServer, Pl.type = new Tl.ProtocolRequestType(Pl.method);
-var Ol = {};
-Object.defineProperty(Ol, "__esModule", {
-    value: !0
-}), Ol.TypeHierarchySubtypesRequest = Ol.TypeHierarchySupertypesRequest = Ol.TypeHierarchyPrepareRequest = void 0;
-const Nl = Oa;
-var jl, ql, Ll, Al, Il, Bl;
-(ql = jl || (Ol.TypeHierarchyPrepareRequest = jl = {})).method = "textDocument/prepareTypeHierarchy", ql.messageDirection = Nl.MessageDirection.clientToServer, ql.type = new Nl.ProtocolRequestType(ql.method), (Al = Ll || (Ol.TypeHierarchySupertypesRequest = Ll = {})).method = "typeHierarchy/supertypes", Al.messageDirection = Nl.MessageDirection.clientToServer, Al.type = new Nl.ProtocolRequestType(Al.method), (Bl = Il || (Ol.TypeHierarchySubtypesRequest = Il = {})).method = "typeHierarchy/subtypes", Bl.messageDirection = Nl.MessageDirection.clientToServer, Bl.type = new Nl.ProtocolRequestType(Bl.method);
-var Fl = {};
-Object.defineProperty(Fl, "__esModule", {
-    value: !0
-}), Fl.InlineValueRefreshRequest = Fl.InlineValueRequest = void 0;
-const Wl = Oa;
-var Hl, Kl, Ul, Vl;
-(Kl = Hl || (Fl.InlineValueRequest = Hl = {})).method = "textDocument/inlineValue", Kl.messageDirection = Wl.MessageDirection.clientToServer, Kl.type = new Wl.ProtocolRequestType(Kl.method), (Vl = Ul || (Fl.InlineValueRefreshRequest = Ul = {})).method = "workspace/inlineValue/refresh", Vl.messageDirection = Wl.MessageDirection.serverToClient, Vl.type = new Wl.ProtocolRequestType0(Vl.method);
-var $l = {};
-Object.defineProperty($l, "__esModule", {
-    value: !0
-}), $l.InlayHintRefreshRequest = $l.InlayHintResolveRequest = $l.InlayHintRequest = void 0;
-const zl = Oa;
-var Jl, Ql, Gl, Xl, Zl, Yl;
-(Ql = Jl || ($l.InlayHintRequest = Jl = {})).method = "textDocument/inlayHint", Ql.messageDirection = zl.MessageDirection.clientToServer, Ql.type = new zl.ProtocolRequestType(Ql.method), (Xl = Gl || ($l.InlayHintResolveRequest = Gl = {})).method = "inlayHint/resolve", Xl.messageDirection = zl.MessageDirection.clientToServer, Xl.type = new zl.ProtocolRequestType(Xl.method), (Yl = Zl || ($l.InlayHintRefreshRequest = Zl = {})).method = "workspace/inlayHint/refresh", Yl.messageDirection = zl.MessageDirection.serverToClient, Yl.type = new zl.ProtocolRequestType0(Yl.method);
-var eu = {};
-Object.defineProperty(eu, "__esModule", {
-    value: !0
-}), eu.DiagnosticRefreshRequest = eu.WorkspaceDiagnosticRequest = eu.DocumentDiagnosticRequest = eu.DocumentDiagnosticReportKind = eu.DiagnosticServerCancellationData = void 0;
-const tu = Lr,
-    nu = Aa,
-    ru = Oa;
-var ou, iu, su, au, cu, lu, uu, du, hu;
-(ou || (eu.DiagnosticServerCancellationData = ou = {})).is = function(e) {
+}), Nc.LinkedEditingRangeRequest = void 0;
+const jc = aa;
+var qc, Lc;
+(Lc = qc || (Nc.LinkedEditingRangeRequest = qc = {})).method = "textDocument/linkedEditingRange", Lc.messageDirection = jc.MessageDirection.clientToServer, Lc.type = new jc.ProtocolRequestType(Lc.method);
+var Ac = {};
+Object.defineProperty(Ac, "__esModule", {
+    value: !0
+}), Ac.WillDeleteFilesRequest = Ac.DidDeleteFilesNotification = Ac.DidRenameFilesNotification = Ac.WillRenameFilesRequest = Ac.DidCreateFilesNotification = Ac.WillCreateFilesRequest = Ac.FileOperationPatternKind = void 0;
+const Ic = aa;
+var Bc, Fc, Wc, Hc, Kc, Uc, Vc, $c, zc, Jc, Qc, Gc, Xc, Zc;
+(Fc = Bc || (Ac.FileOperationPatternKind = Bc = {})).file = "file", Fc.folder = "folder", (Hc = Wc || (Ac.WillCreateFilesRequest = Wc = {})).method = "workspace/willCreateFiles", Hc.messageDirection = Ic.MessageDirection.clientToServer, Hc.type = new Ic.ProtocolRequestType(Hc.method), (Uc = Kc || (Ac.DidCreateFilesNotification = Kc = {})).method = "workspace/didCreateFiles", Uc.messageDirection = Ic.MessageDirection.clientToServer, Uc.type = new Ic.ProtocolNotificationType(Uc.method), ($c = Vc || (Ac.WillRenameFilesRequest = Vc = {})).method = "workspace/willRenameFiles", $c.messageDirection = Ic.MessageDirection.clientToServer, $c.type = new Ic.ProtocolRequestType($c.method), (Jc = zc || (Ac.DidRenameFilesNotification = zc = {})).method = "workspace/didRenameFiles", Jc.messageDirection = Ic.MessageDirection.clientToServer, Jc.type = new Ic.ProtocolNotificationType(Jc.method), (Gc = Qc || (Ac.DidDeleteFilesNotification = Qc = {})).method = "workspace/didDeleteFiles", Gc.messageDirection = Ic.MessageDirection.clientToServer, Gc.type = new Ic.ProtocolNotificationType(Gc.method), (Zc = Xc || (Ac.WillDeleteFilesRequest = Xc = {})).method = "workspace/willDeleteFiles", Zc.messageDirection = Ic.MessageDirection.clientToServer, Zc.type = new Ic.ProtocolRequestType(Zc.method);
+var Yc = {};
+Object.defineProperty(Yc, "__esModule", {
+    value: !0
+}), Yc.MonikerRequest = Yc.MonikerKind = Yc.UniquenessLevel = void 0;
+const el = aa;
+var tl, nl, rl, ol, il, sl;
+(nl = tl || (Yc.UniquenessLevel = tl = {})).document = "document", nl.project = "project", nl.group = "group", nl.scheme = "scheme", nl.global = "global", (ol = rl || (Yc.MonikerKind = rl = {})).$import = "import", ol.$export = "export", ol.local = "local", (sl = il || (Yc.MonikerRequest = il = {})).method = "textDocument/moniker", sl.messageDirection = el.MessageDirection.clientToServer, sl.type = new el.ProtocolRequestType(sl.method);
+var al = {};
+Object.defineProperty(al, "__esModule", {
+    value: !0
+}), al.TypeHierarchySubtypesRequest = al.TypeHierarchySupertypesRequest = al.TypeHierarchyPrepareRequest = void 0;
+const cl = aa;
+var ll, ul, dl, hl, fl, pl;
+(ul = ll || (al.TypeHierarchyPrepareRequest = ll = {})).method = "textDocument/prepareTypeHierarchy", ul.messageDirection = cl.MessageDirection.clientToServer, ul.type = new cl.ProtocolRequestType(ul.method), (hl = dl || (al.TypeHierarchySupertypesRequest = dl = {})).method = "typeHierarchy/supertypes", hl.messageDirection = cl.MessageDirection.clientToServer, hl.type = new cl.ProtocolRequestType(hl.method), (pl = fl || (al.TypeHierarchySubtypesRequest = fl = {})).method = "typeHierarchy/subtypes", pl.messageDirection = cl.MessageDirection.clientToServer, pl.type = new cl.ProtocolRequestType(pl.method);
+var ml = {};
+Object.defineProperty(ml, "__esModule", {
+    value: !0
+}), ml.InlineValueRefreshRequest = ml.InlineValueRequest = void 0;
+const gl = aa;
+var vl, yl, bl, wl;
+(yl = vl || (ml.InlineValueRequest = vl = {})).method = "textDocument/inlineValue", yl.messageDirection = gl.MessageDirection.clientToServer, yl.type = new gl.ProtocolRequestType(yl.method), (wl = bl || (ml.InlineValueRefreshRequest = bl = {})).method = "workspace/inlineValue/refresh", wl.messageDirection = gl.MessageDirection.serverToClient, wl.type = new gl.ProtocolRequestType0(wl.method);
+var Cl = {};
+Object.defineProperty(Cl, "__esModule", {
+    value: !0
+}), Cl.InlayHintRefreshRequest = Cl.InlayHintResolveRequest = Cl.InlayHintRequest = void 0;
+const xl = aa;
+var kl, Rl, Tl, Sl, Ml, Dl;
+(Rl = kl || (Cl.InlayHintRequest = kl = {})).method = "textDocument/inlayHint", Rl.messageDirection = xl.MessageDirection.clientToServer, Rl.type = new xl.ProtocolRequestType(Rl.method), (Sl = Tl || (Cl.InlayHintResolveRequest = Tl = {})).method = "inlayHint/resolve", Sl.messageDirection = xl.MessageDirection.clientToServer, Sl.type = new xl.ProtocolRequestType(Sl.method), (Dl = Ml || (Cl.InlayHintRefreshRequest = Ml = {})).method = "workspace/inlayHint/refresh", Dl.messageDirection = xl.MessageDirection.serverToClient, Dl.type = new xl.ProtocolRequestType0(Dl.method);
+var _l = {};
+Object.defineProperty(_l, "__esModule", {
+    value: !0
+}), _l.DiagnosticRefreshRequest = _l.WorkspaceDiagnosticRequest = _l.DocumentDiagnosticRequest = _l.DocumentDiagnosticReportKind = _l.DiagnosticServerCancellationData = void 0;
+const El = Ir,
+    Pl = ha,
+    Ol = aa;
+var Nl, jl, ql, Ll, Al, Il, Bl, Fl, Wl;
+(Nl || (_l.DiagnosticServerCancellationData = Nl = {})).is = function(e) {
     const t = e;
-    return t && nu.boolean(t.retriggerRequest)
-}, (su = iu || (eu.DocumentDiagnosticReportKind = iu = {})).Full = "full", su.Unchanged = "unchanged", (cu = au || (eu.DocumentDiagnosticRequest = au = {})).method = "textDocument/diagnostic", cu.messageDirection = ru.MessageDirection.clientToServer, cu.type = new ru.ProtocolRequestType(cu.method), cu.partialResult = new tu.ProgressType, (uu = lu || (eu.WorkspaceDiagnosticRequest = lu = {})).method = "workspace/diagnostic", uu.messageDirection = ru.MessageDirection.clientToServer, uu.type = new ru.ProtocolRequestType(uu.method), uu.partialResult = new tu.ProgressType, (hu = du || (eu.DiagnosticRefreshRequest = du = {})).method = "workspace/diagnostic/refresh", hu.messageDirection = ru.MessageDirection.serverToClient, hu.type = new ru.ProtocolRequestType0(hu.method);
-var fu = {};
-Object.defineProperty(fu, "__esModule", {
-    value: !0
-}), fu.DidCloseNotebookDocumentNotification = fu.DidSaveNotebookDocumentNotification = fu.DidChangeNotebookDocumentNotification = fu.NotebookCellArrayChange = fu.DidOpenNotebookDocumentNotification = fu.NotebookDocumentSyncRegistrationType = fu.NotebookDocument = fu.NotebookCell = fu.ExecutionSummary = fu.NotebookCellKind = void 0;
-const pu = Pa,
-    mu = Aa,
-    gu = Oa;
-var vu, yu, bu, wu, Cu, xu, ku, Ru, Tu, Su, Mu, Du, _u, Eu, Pu, Ou, Nu, ju, qu;
-(yu = vu || (fu.NotebookCellKind = vu = {})).Markup = 1, yu.Code = 2, yu.is = function(e) {
+    return t && Pl.boolean(t.retriggerRequest)
+}, (ql = jl || (_l.DocumentDiagnosticReportKind = jl = {})).Full = "full", ql.Unchanged = "unchanged", (Al = Ll || (_l.DocumentDiagnosticRequest = Ll = {})).method = "textDocument/diagnostic", Al.messageDirection = Ol.MessageDirection.clientToServer, Al.type = new Ol.ProtocolRequestType(Al.method), Al.partialResult = new El.ProgressType, (Bl = Il || (_l.WorkspaceDiagnosticRequest = Il = {})).method = "workspace/diagnostic", Bl.messageDirection = Ol.MessageDirection.clientToServer, Bl.type = new Ol.ProtocolRequestType(Bl.method), Bl.partialResult = new El.ProgressType, (Wl = Fl || (_l.DiagnosticRefreshRequest = Fl = {})).method = "workspace/diagnostic/refresh", Wl.messageDirection = Ol.MessageDirection.serverToClient, Wl.type = new Ol.ProtocolRequestType0(Wl.method);
+var Hl = {};
+Object.defineProperty(Hl, "__esModule", {
+    value: !0
+}), Hl.DidCloseNotebookDocumentNotification = Hl.DidSaveNotebookDocumentNotification = Hl.DidChangeNotebookDocumentNotification = Hl.NotebookCellArrayChange = Hl.DidOpenNotebookDocumentNotification = Hl.NotebookDocumentSyncRegistrationType = Hl.NotebookDocument = Hl.NotebookCell = Hl.ExecutionSummary = Hl.NotebookCellKind = void 0;
+const Kl = sa,
+    Ul = ha,
+    Vl = aa;
+var $l, zl, Jl, Ql, Gl, Xl, Zl, Yl, eu, tu, nu, ru, ou, iu, su, au, cu, lu, uu;
+(zl = $l || (Hl.NotebookCellKind = $l = {})).Markup = 1, zl.Code = 2, zl.is = function(e) {
         return 1 === e || 2 === e
-    }, (wu = bu || (fu.ExecutionSummary = bu = {})).create = function(e, t) {
+    }, (Ql = Jl || (Hl.ExecutionSummary = Jl = {})).create = function(e, t) {
         const n = {
             executionOrder: e
         };
         return !0 !== t && !1 !== t || (n.success = t), n
-    }, wu.is = function(e) {
+    }, Ql.is = function(e) {
         const t = e;
-        return mu.objectLiteral(t) && pu.uinteger.is(t.executionOrder) && (void 0 === t.success || mu.boolean(t.success))
-    }, wu.equals = function(e, t) {
+        return Ul.objectLiteral(t) && Kl.uinteger.is(t.executionOrder) && (void 0 === t.success || Ul.boolean(t.success))
+    }, Ql.equals = function(e, t) {
         return e === t || null != e && null != t && e.executionOrder === t.executionOrder && e.success === t.success
     },
     function(e) {
         function t(e, n) {
             if (e === n) return !0;
             if (null == e || null == n) return !1;
             if (typeof e != typeof n) return !1;
@@ -11154,15 +11194,15 @@
                 o = Array.isArray(n);
             if (r !== o) return !1;
             if (r && o) {
                 if (e.length !== n.length) return !1;
                 for (let r = 0; r < e.length; r++)
                     if (!t(e[r], n[r])) return !1
             }
-            if (mu.objectLiteral(e) && mu.objectLiteral(n)) {
+            if (Ul.objectLiteral(e) && Ul.objectLiteral(n)) {
                 const r = Object.keys(e),
                     o = Object.keys(n);
                 if (r.length !== o.length) return !1;
                 if (r.sort(), o.sort(), !t(r, o)) return !1;
                 for (let i = 0; i < r.length; i++) {
                     const o = r[i];
                     if (!t(e[o], n[o])) return !1
@@ -11173,125 +11213,125 @@
         e.create = function(e, t) {
             return {
                 kind: e,
                 document: t
             }
         }, e.is = function(e) {
             const t = e;
-            return mu.objectLiteral(t) && vu.is(t.kind) && pu.DocumentUri.is(t.document) && (void 0 === t.metadata || mu.objectLiteral(t.metadata))
+            return Ul.objectLiteral(t) && $l.is(t.kind) && Kl.DocumentUri.is(t.document) && (void 0 === t.metadata || Ul.objectLiteral(t.metadata))
         }, e.diff = function(e, n) {
             const r = new Set;
-            return e.document !== n.document && r.add("document"), e.kind !== n.kind && r.add("kind"), e.executionSummary !== n.executionSummary && r.add("executionSummary"), void 0 === e.metadata && void 0 === n.metadata || t(e.metadata, n.metadata) || r.add("metadata"), void 0 === e.executionSummary && void 0 === n.executionSummary || bu.equals(e.executionSummary, n.executionSummary) || r.add("executionSummary"), r
+            return e.document !== n.document && r.add("document"), e.kind !== n.kind && r.add("kind"), e.executionSummary !== n.executionSummary && r.add("executionSummary"), void 0 === e.metadata && void 0 === n.metadata || t(e.metadata, n.metadata) || r.add("metadata"), void 0 === e.executionSummary && void 0 === n.executionSummary || Jl.equals(e.executionSummary, n.executionSummary) || r.add("executionSummary"), r
         }
-    }(Cu || (fu.NotebookCell = Cu = {})), (ku = xu || (fu.NotebookDocument = xu = {})).create = function(e, t, n, r) {
+    }(Gl || (Hl.NotebookCell = Gl = {})), (Zl = Xl || (Hl.NotebookDocument = Xl = {})).create = function(e, t, n, r) {
         return {
             uri: e,
             notebookType: t,
             version: n,
             cells: r
         }
-    }, ku.is = function(e) {
+    }, Zl.is = function(e) {
         const t = e;
-        return mu.objectLiteral(t) && mu.string(t.uri) && pu.integer.is(t.version) && mu.typedArray(t.cells, Cu.is)
-    }, (Tu = Ru || (fu.NotebookDocumentSyncRegistrationType = Ru = {})).method = "notebookDocument/sync", Tu.messageDirection = gu.MessageDirection.clientToServer, Tu.type = new gu.RegistrationType(Tu.method), (Mu = Su || (fu.DidOpenNotebookDocumentNotification = Su = {})).method = "notebookDocument/didOpen", Mu.messageDirection = gu.MessageDirection.clientToServer, Mu.type = new gu.ProtocolNotificationType(Mu.method), Mu.registrationMethod = Ru.method, (_u = Du || (fu.NotebookCellArrayChange = Du = {})).is = function(e) {
+        return Ul.objectLiteral(t) && Ul.string(t.uri) && Kl.integer.is(t.version) && Ul.typedArray(t.cells, Gl.is)
+    }, (eu = Yl || (Hl.NotebookDocumentSyncRegistrationType = Yl = {})).method = "notebookDocument/sync", eu.messageDirection = Vl.MessageDirection.clientToServer, eu.type = new Vl.RegistrationType(eu.method), (nu = tu || (Hl.DidOpenNotebookDocumentNotification = tu = {})).method = "notebookDocument/didOpen", nu.messageDirection = Vl.MessageDirection.clientToServer, nu.type = new Vl.ProtocolNotificationType(nu.method), nu.registrationMethod = Yl.method, (ou = ru || (Hl.NotebookCellArrayChange = ru = {})).is = function(e) {
         const t = e;
-        return mu.objectLiteral(t) && pu.uinteger.is(t.start) && pu.uinteger.is(t.deleteCount) && (void 0 === t.cells || mu.typedArray(t.cells, Cu.is))
-    }, _u.create = function(e, t, n) {
+        return Ul.objectLiteral(t) && Kl.uinteger.is(t.start) && Kl.uinteger.is(t.deleteCount) && (void 0 === t.cells || Ul.typedArray(t.cells, Gl.is))
+    }, ou.create = function(e, t, n) {
         const r = {
             start: e,
             deleteCount: t
         };
         return void 0 !== n && (r.cells = n), r
-    }, (Pu = Eu || (fu.DidChangeNotebookDocumentNotification = Eu = {})).method = "notebookDocument/didChange", Pu.messageDirection = gu.MessageDirection.clientToServer, Pu.type = new gu.ProtocolNotificationType(Pu.method), Pu.registrationMethod = Ru.method, (Nu = Ou || (fu.DidSaveNotebookDocumentNotification = Ou = {})).method = "notebookDocument/didSave", Nu.messageDirection = gu.MessageDirection.clientToServer, Nu.type = new gu.ProtocolNotificationType(Nu.method), Nu.registrationMethod = Ru.method, (qu = ju || (fu.DidCloseNotebookDocumentNotification = ju = {})).method = "notebookDocument/didClose", qu.messageDirection = gu.MessageDirection.clientToServer, qu.type = new gu.ProtocolNotificationType(qu.method), qu.registrationMethod = Ru.method;
-var Lu = {};
-Object.defineProperty(Lu, "__esModule", {
-    value: !0
-}), Lu.InlineCompletionRequest = void 0;
-const Au = Oa;
-var Iu, Bu;
-(Bu = Iu || (Lu.InlineCompletionRequest = Iu = {})).method = "textDocument/inlineCompletion", Bu.messageDirection = Au.MessageDirection.clientToServer, Bu.type = new Au.ProtocolRequestType(Bu.method),
+    }, (su = iu || (Hl.DidChangeNotebookDocumentNotification = iu = {})).method = "notebookDocument/didChange", su.messageDirection = Vl.MessageDirection.clientToServer, su.type = new Vl.ProtocolNotificationType(su.method), su.registrationMethod = Yl.method, (cu = au || (Hl.DidSaveNotebookDocumentNotification = au = {})).method = "notebookDocument/didSave", cu.messageDirection = Vl.MessageDirection.clientToServer, cu.type = new Vl.ProtocolNotificationType(cu.method), cu.registrationMethod = Yl.method, (uu = lu || (Hl.DidCloseNotebookDocumentNotification = lu = {})).method = "notebookDocument/didClose", uu.messageDirection = Vl.MessageDirection.clientToServer, uu.type = new Vl.ProtocolNotificationType(uu.method), uu.registrationMethod = Yl.method;
+var du = {};
+Object.defineProperty(du, "__esModule", {
+    value: !0
+}), du.InlineCompletionRequest = void 0;
+const hu = aa;
+var fu, pu;
+(pu = fu || (du.InlineCompletionRequest = fu = {})).method = "textDocument/inlineCompletion", pu.messageDirection = hu.MessageDirection.clientToServer, pu.type = new hu.ProtocolRequestType(pu.method),
     function(e) {
         Object.defineProperty(e, "__esModule", {
             value: !0
         }), e.WorkspaceSymbolRequest = e.CodeActionResolveRequest = e.CodeActionRequest = e.DocumentSymbolRequest = e.DocumentHighlightRequest = e.ReferencesRequest = e.DefinitionRequest = e.SignatureHelpRequest = e.SignatureHelpTriggerKind = e.HoverRequest = e.CompletionResolveRequest = e.CompletionRequest = e.CompletionTriggerKind = e.PublishDiagnosticsNotification = e.WatchKind = e.RelativePattern = e.FileChangeType = e.DidChangeWatchedFilesNotification = e.WillSaveTextDocumentWaitUntilRequest = e.WillSaveTextDocumentNotification = e.TextDocumentSaveReason = e.DidSaveTextDocumentNotification = e.DidCloseTextDocumentNotification = e.DidChangeTextDocumentNotification = e.TextDocumentContentChangeEvent = e.DidOpenTextDocumentNotification = e.TextDocumentSyncKind = e.TelemetryEventNotification = e.LogMessageNotification = e.ShowMessageRequest = e.ShowMessageNotification = e.MessageType = e.DidChangeConfigurationNotification = e.ExitNotification = e.ShutdownRequest = e.InitializedNotification = e.InitializeErrorCodes = e.InitializeRequest = e.WorkDoneProgressOptions = e.TextDocumentRegistrationOptions = e.StaticRegistrationOptions = e.PositionEncodingKind = e.FailureHandlingKind = e.ResourceOperationKind = e.UnregistrationRequest = e.RegistrationRequest = e.DocumentSelector = e.NotebookCellTextDocumentFilter = e.NotebookDocumentFilter = e.TextDocumentFilter = void 0, e.MonikerRequest = e.MonikerKind = e.UniquenessLevel = e.WillDeleteFilesRequest = e.DidDeleteFilesNotification = e.WillRenameFilesRequest = e.DidRenameFilesNotification = e.WillCreateFilesRequest = e.DidCreateFilesNotification = e.FileOperationPatternKind = e.LinkedEditingRangeRequest = e.ShowDocumentRequest = e.SemanticTokensRegistrationType = e.SemanticTokensRefreshRequest = e.SemanticTokensRangeRequest = e.SemanticTokensDeltaRequest = e.SemanticTokensRequest = e.TokenFormat = e.CallHierarchyPrepareRequest = e.CallHierarchyOutgoingCallsRequest = e.CallHierarchyIncomingCallsRequest = e.WorkDoneProgressCancelNotification = e.WorkDoneProgressCreateRequest = e.WorkDoneProgress = e.SelectionRangeRequest = e.DeclarationRequest = e.FoldingRangeRefreshRequest = e.FoldingRangeRequest = e.ColorPresentationRequest = e.DocumentColorRequest = e.ConfigurationRequest = e.DidChangeWorkspaceFoldersNotification = e.WorkspaceFoldersRequest = e.TypeDefinitionRequest = e.ImplementationRequest = e.ApplyWorkspaceEditRequest = e.ExecuteCommandRequest = e.PrepareRenameRequest = e.RenameRequest = e.PrepareSupportDefaultBehavior = e.DocumentOnTypeFormattingRequest = e.DocumentRangesFormattingRequest = e.DocumentRangeFormattingRequest = e.DocumentFormattingRequest = e.DocumentLinkResolveRequest = e.DocumentLinkRequest = e.CodeLensRefreshRequest = e.CodeLensResolveRequest = e.CodeLensRequest = e.WorkspaceSymbolResolveRequest = void 0, e.InlineCompletionRequest = e.DidCloseNotebookDocumentNotification = e.DidSaveNotebookDocumentNotification = e.DidChangeNotebookDocumentNotification = e.NotebookCellArrayChange = e.DidOpenNotebookDocumentNotification = e.NotebookDocumentSyncRegistrationType = e.NotebookDocument = e.NotebookCell = e.ExecutionSummary = e.NotebookCellKind = e.DiagnosticRefreshRequest = e.WorkspaceDiagnosticRequest = e.DocumentDiagnosticRequest = e.DocumentDiagnosticReportKind = e.DiagnosticServerCancellationData = e.InlayHintRefreshRequest = e.InlayHintResolveRequest = e.InlayHintRequest = e.InlineValueRefreshRequest = e.InlineValueRequest = e.TypeHierarchySupertypesRequest = e.TypeHierarchySubtypesRequest = e.TypeHierarchyPrepareRequest = void 0;
-        const t = Oa,
-            n = Pa,
-            r = Aa,
-            o = Fa;
+        const t = aa,
+            n = sa,
+            r = ha,
+            o = ma;
         Object.defineProperty(e, "ImplementationRequest", {
             enumerable: !0,
             get: function() {
                 return o.ImplementationRequest
             }
         });
-        const i = Ua;
+        const i = ba;
         Object.defineProperty(e, "TypeDefinitionRequest", {
             enumerable: !0,
             get: function() {
                 return i.TypeDefinitionRequest
             }
         });
-        const s = Ja;
+        const s = ka;
         Object.defineProperty(e, "WorkspaceFoldersRequest", {
             enumerable: !0,
             get: function() {
                 return s.WorkspaceFoldersRequest
             }
         }), Object.defineProperty(e, "DidChangeWorkspaceFoldersNotification", {
             enumerable: !0,
             get: function() {
                 return s.DidChangeWorkspaceFoldersNotification
             }
         });
-        const a = ec;
+        const a = _a;
         Object.defineProperty(e, "ConfigurationRequest", {
             enumerable: !0,
             get: function() {
                 return a.ConfigurationRequest
             }
         });
-        const c = oc;
+        const c = Na;
         Object.defineProperty(e, "DocumentColorRequest", {
             enumerable: !0,
             get: function() {
                 return c.DocumentColorRequest
             }
         }), Object.defineProperty(e, "ColorPresentationRequest", {
             enumerable: !0,
             get: function() {
                 return c.ColorPresentationRequest
             }
         });
-        const l = uc;
+        const l = Ba;
         Object.defineProperty(e, "FoldingRangeRequest", {
             enumerable: !0,
             get: function() {
                 return l.FoldingRangeRequest
             }
         }), Object.defineProperty(e, "FoldingRangeRefreshRequest", {
             enumerable: !0,
             get: function() {
                 return l.FoldingRangeRefreshRequest
             }
         });
-        const u = gc;
+        const u = Va;
         Object.defineProperty(e, "DeclarationRequest", {
             enumerable: !0,
             get: function() {
                 return u.DeclarationRequest
             }
         });
-        const d = wc;
+        const d = Qa;
         Object.defineProperty(e, "SelectionRangeRequest", {
             enumerable: !0,
             get: function() {
                 return d.SelectionRangeRequest
             }
         });
-        const h = Rc;
+        const h = Ya;
         Object.defineProperty(e, "WorkDoneProgress", {
             enumerable: !0,
             get: function() {
                 return h.WorkDoneProgress
             }
         }), Object.defineProperty(e, "WorkDoneProgressCreateRequest", {
             enumerable: !0,
@@ -11300,15 +11340,15 @@
             }
         }), Object.defineProperty(e, "WorkDoneProgressCancelNotification", {
             enumerable: !0,
             get: function() {
                 return h.WorkDoneProgressCancelNotification
             }
         });
-        const f = Nc;
+        const f = cc;
         Object.defineProperty(e, "CallHierarchyIncomingCallsRequest", {
             enumerable: !0,
             get: function() {
                 return f.CallHierarchyIncomingCallsRequest
             }
         }), Object.defineProperty(e, "CallHierarchyOutgoingCallsRequest", {
             enumerable: !0,
@@ -11317,15 +11357,15 @@
             }
         }), Object.defineProperty(e, "CallHierarchyPrepareRequest", {
             enumerable: !0,
             get: function() {
                 return f.CallHierarchyPrepareRequest
             }
         });
-        const p = Wc;
+        const p = gc;
         Object.defineProperty(e, "TokenFormat", {
             enumerable: !0,
             get: function() {
                 return p.TokenFormat
             }
         }), Object.defineProperty(e, "SemanticTokensRequest", {
             enumerable: !0,
@@ -11349,29 +11389,29 @@
             }
         }), Object.defineProperty(e, "SemanticTokensRegistrationType", {
             enumerable: !0,
             get: function() {
                 return p.SemanticTokensRegistrationType
             }
         });
-        const m = el;
+        const m = _c;
         Object.defineProperty(e, "ShowDocumentRequest", {
             enumerable: !0,
             get: function() {
                 return m.ShowDocumentRequest
             }
         });
-        const g = ol;
+        const g = Nc;
         Object.defineProperty(e, "LinkedEditingRangeRequest", {
             enumerable: !0,
             get: function() {
                 return g.LinkedEditingRangeRequest
             }
         });
-        const v = cl;
+        const v = Ac;
         Object.defineProperty(e, "FileOperationPatternKind", {
             enumerable: !0,
             get: function() {
                 return v.FileOperationPatternKind
             }
         }), Object.defineProperty(e, "DidCreateFilesNotification", {
             enumerable: !0,
@@ -11400,15 +11440,15 @@
             }
         }), Object.defineProperty(e, "WillDeleteFilesRequest", {
             enumerable: !0,
             get: function() {
                 return v.WillDeleteFilesRequest
             }
         });
-        const y = Rl;
+        const y = Yc;
         Object.defineProperty(e, "UniquenessLevel", {
             enumerable: !0,
             get: function() {
                 return y.UniquenessLevel
             }
         }), Object.defineProperty(e, "MonikerKind", {
             enumerable: !0,
@@ -11417,15 +11457,15 @@
             }
         }), Object.defineProperty(e, "MonikerRequest", {
             enumerable: !0,
             get: function() {
                 return y.MonikerRequest
             }
         });
-        const b = Ol;
+        const b = al;
         Object.defineProperty(e, "TypeHierarchyPrepareRequest", {
             enumerable: !0,
             get: function() {
                 return b.TypeHierarchyPrepareRequest
             }
         }), Object.defineProperty(e, "TypeHierarchySubtypesRequest", {
             enumerable: !0,
@@ -11434,27 +11474,27 @@
             }
         }), Object.defineProperty(e, "TypeHierarchySupertypesRequest", {
             enumerable: !0,
             get: function() {
                 return b.TypeHierarchySupertypesRequest
             }
         });
-        const w = Fl;
+        const w = ml;
         Object.defineProperty(e, "InlineValueRequest", {
             enumerable: !0,
             get: function() {
                 return w.InlineValueRequest
             }
         }), Object.defineProperty(e, "InlineValueRefreshRequest", {
             enumerable: !0,
             get: function() {
                 return w.InlineValueRefreshRequest
             }
         });
-        const C = $l;
+        const C = Cl;
         Object.defineProperty(e, "InlayHintRequest", {
             enumerable: !0,
             get: function() {
                 return C.InlayHintRequest
             }
         }), Object.defineProperty(e, "InlayHintResolveRequest", {
             enumerable: !0,
@@ -11463,15 +11503,15 @@
             }
         }), Object.defineProperty(e, "InlayHintRefreshRequest", {
             enumerable: !0,
             get: function() {
                 return C.InlayHintRefreshRequest
             }
         });
-        const x = eu;
+        const x = _l;
         Object.defineProperty(e, "DiagnosticServerCancellationData", {
             enumerable: !0,
             get: function() {
                 return x.DiagnosticServerCancellationData
             }
         }), Object.defineProperty(e, "DocumentDiagnosticReportKind", {
             enumerable: !0,
@@ -11490,15 +11530,15 @@
             }
         }), Object.defineProperty(e, "DiagnosticRefreshRequest", {
             enumerable: !0,
             get: function() {
                 return x.DiagnosticRefreshRequest
             }
         });
-        const k = fu;
+        const k = Hl;
         Object.defineProperty(e, "NotebookCellKind", {
             enumerable: !0,
             get: function() {
                 return k.NotebookCellKind
             }
         }), Object.defineProperty(e, "ExecutionSummary", {
             enumerable: !0,
@@ -11542,15 +11582,15 @@
             }
         }), Object.defineProperty(e, "DidCloseNotebookDocumentNotification", {
             enumerable: !0,
             get: function() {
                 return k.DidCloseNotebookDocumentNotification
             }
         });
-        const R = Lu;
+        const R = du;
         var T, S, M, D, _, E, P, O, N, j, q, L, A, I, B, F, W, H, K, U, V, $, z, J, Q, G, X, Z, Y, ee, te, ne, re, oe, ie, se, ae, ce, le, ue, de, he, fe, pe, me, ge, ve, ye, be, we, Ce, xe, ke, Re, Te, Se, Me, De, _e, Ee, Pe, Oe, Ne, je, qe, Le, Ae, Ie, Be, Fe, We, He, Ke, Ue, Ve, $e, ze, Je, Qe, Ge, Xe, Ze, Ye, et, tt, nt, rt, ot, it, st, at, ct, lt, ut, dt, ht, ft, pt, mt, gt, vt, yt, bt, wt, Ct, xt, kt, Rt, Tt, St, Mt, Dt, _t, Et, Pt, Ot, Nt, jt, qt, Lt, At;
         Object.defineProperty(e, "InlineCompletionRequest", {
             enumerable: !0,
             get: function() {
                 return R.InlineCompletionRequest
             }
         }), (T || (e.TextDocumentFilter = T = {})).is = function(e) {
@@ -11585,24 +11625,24 @@
         }, me.isFull = function(e) {
             let t = e;
             return null != t && "string" == typeof t.text && void 0 === t.range && void 0 === t.rangeLength
         }, (ve = ge || (e.DidChangeTextDocumentNotification = ge = {})).method = "textDocument/didChange", ve.messageDirection = t.MessageDirection.clientToServer, ve.type = new t.ProtocolNotificationType(ve.method), (be = ye || (e.DidCloseTextDocumentNotification = ye = {})).method = "textDocument/didClose", be.messageDirection = t.MessageDirection.clientToServer, be.type = new t.ProtocolNotificationType(be.method), (Ce = we || (e.DidSaveTextDocumentNotification = we = {})).method = "textDocument/didSave", Ce.messageDirection = t.MessageDirection.clientToServer, Ce.type = new t.ProtocolNotificationType(Ce.method), (ke = xe || (e.TextDocumentSaveReason = xe = {})).Manual = 1, ke.AfterDelay = 2, ke.FocusOut = 3, (Te = Re || (e.WillSaveTextDocumentNotification = Re = {})).method = "textDocument/willSave", Te.messageDirection = t.MessageDirection.clientToServer, Te.type = new t.ProtocolNotificationType(Te.method), (Me = Se || (e.WillSaveTextDocumentWaitUntilRequest = Se = {})).method = "textDocument/willSaveWaitUntil", Me.messageDirection = t.MessageDirection.clientToServer, Me.type = new t.ProtocolRequestType(Me.method), (_e = De || (e.DidChangeWatchedFilesNotification = De = {})).method = "workspace/didChangeWatchedFiles", _e.messageDirection = t.MessageDirection.clientToServer, _e.type = new t.ProtocolNotificationType(_e.method), (Pe = Ee || (e.FileChangeType = Ee = {})).Created = 1, Pe.Changed = 2, Pe.Deleted = 3, (Oe || (e.RelativePattern = Oe = {})).is = function(e) {
             const t = e;
             return r.objectLiteral(t) && (n.URI.is(t.baseUri) || n.WorkspaceFolder.is(t.baseUri)) && r.string(t.pattern)
         }, (je = Ne || (e.WatchKind = Ne = {})).Create = 1, je.Change = 2, je.Delete = 4, (Le = qe || (e.PublishDiagnosticsNotification = qe = {})).method = "textDocument/publishDiagnostics", Le.messageDirection = t.MessageDirection.serverToClient, Le.type = new t.ProtocolNotificationType(Le.method), (Ie = Ae || (e.CompletionTriggerKind = Ae = {})).Invoked = 1, Ie.TriggerCharacter = 2, Ie.TriggerForIncompleteCompletions = 3, (Fe = Be || (e.CompletionRequest = Be = {})).method = "textDocument/completion", Fe.messageDirection = t.MessageDirection.clientToServer, Fe.type = new t.ProtocolRequestType(Fe.method), (He = We || (e.CompletionResolveRequest = We = {})).method = "completionItem/resolve", He.messageDirection = t.MessageDirection.clientToServer, He.type = new t.ProtocolRequestType(He.method), (Ue = Ke || (e.HoverRequest = Ke = {})).method = "textDocument/hover", Ue.messageDirection = t.MessageDirection.clientToServer, Ue.type = new t.ProtocolRequestType(Ue.method), ($e = Ve || (e.SignatureHelpTriggerKind = Ve = {})).Invoked = 1, $e.TriggerCharacter = 2, $e.ContentChange = 3, (Je = ze || (e.SignatureHelpRequest = ze = {})).method = "textDocument/signatureHelp", Je.messageDirection = t.MessageDirection.clientToServer, Je.type = new t.ProtocolRequestType(Je.method), (Ge = Qe || (e.DefinitionRequest = Qe = {})).method = "textDocument/definition", Ge.messageDirection = t.MessageDirection.clientToServer, Ge.type = new t.ProtocolRequestType(Ge.method), (Ze = Xe || (e.ReferencesRequest = Xe = {})).method = "textDocument/references", Ze.messageDirection = t.MessageDirection.clientToServer, Ze.type = new t.ProtocolRequestType(Ze.method), (et = Ye || (e.DocumentHighlightRequest = Ye = {})).method = "textDocument/documentHighlight", et.messageDirection = t.MessageDirection.clientToServer, et.type = new t.ProtocolRequestType(et.method), (nt = tt || (e.DocumentSymbolRequest = tt = {})).method = "textDocument/documentSymbol", nt.messageDirection = t.MessageDirection.clientToServer, nt.type = new t.ProtocolRequestType(nt.method), (ot = rt || (e.CodeActionRequest = rt = {})).method = "textDocument/codeAction", ot.messageDirection = t.MessageDirection.clientToServer, ot.type = new t.ProtocolRequestType(ot.method), (st = it || (e.CodeActionResolveRequest = it = {})).method = "codeAction/resolve", st.messageDirection = t.MessageDirection.clientToServer, st.type = new t.ProtocolRequestType(st.method), (ct = at || (e.WorkspaceSymbolRequest = at = {})).method = "workspace/symbol", ct.messageDirection = t.MessageDirection.clientToServer, ct.type = new t.ProtocolRequestType(ct.method), (ut = lt || (e.WorkspaceSymbolResolveRequest = lt = {})).method = "workspaceSymbol/resolve", ut.messageDirection = t.MessageDirection.clientToServer, ut.type = new t.ProtocolRequestType(ut.method), (ht = dt || (e.CodeLensRequest = dt = {})).method = "textDocument/codeLens", ht.messageDirection = t.MessageDirection.clientToServer, ht.type = new t.ProtocolRequestType(ht.method), (pt = ft || (e.CodeLensResolveRequest = ft = {})).method = "codeLens/resolve", pt.messageDirection = t.MessageDirection.clientToServer, pt.type = new t.ProtocolRequestType(pt.method), (gt = mt || (e.CodeLensRefreshRequest = mt = {})).method = "workspace/codeLens/refresh", gt.messageDirection = t.MessageDirection.serverToClient, gt.type = new t.ProtocolRequestType0(gt.method), (yt = vt || (e.DocumentLinkRequest = vt = {})).method = "textDocument/documentLink", yt.messageDirection = t.MessageDirection.clientToServer, yt.type = new t.ProtocolRequestType(yt.method), (wt = bt || (e.DocumentLinkResolveRequest = bt = {})).method = "documentLink/resolve", wt.messageDirection = t.MessageDirection.clientToServer, wt.type = new t.ProtocolRequestType(wt.method), (xt = Ct || (e.DocumentFormattingRequest = Ct = {})).method = "textDocument/formatting", xt.messageDirection = t.MessageDirection.clientToServer, xt.type = new t.ProtocolRequestType(xt.method), (Rt = kt || (e.DocumentRangeFormattingRequest = kt = {})).method = "textDocument/rangeFormatting", Rt.messageDirection = t.MessageDirection.clientToServer, Rt.type = new t.ProtocolRequestType(Rt.method), (St = Tt || (e.DocumentRangesFormattingRequest = Tt = {})).method = "textDocument/rangesFormatting", St.messageDirection = t.MessageDirection.clientToServer, St.type = new t.ProtocolRequestType(St.method), (Dt = Mt || (e.DocumentOnTypeFormattingRequest = Mt = {})).method = "textDocument/onTypeFormatting", Dt.messageDirection = t.MessageDirection.clientToServer, Dt.type = new t.ProtocolRequestType(Dt.method), (_t || (e.PrepareSupportDefaultBehavior = _t = {})).Identifier = 1, (Pt = Et || (e.RenameRequest = Et = {})).method = "textDocument/rename", Pt.messageDirection = t.MessageDirection.clientToServer, Pt.type = new t.ProtocolRequestType(Pt.method), (Nt = Ot || (e.PrepareRenameRequest = Ot = {})).method = "textDocument/prepareRename", Nt.messageDirection = t.MessageDirection.clientToServer, Nt.type = new t.ProtocolRequestType(Nt.method), (qt = jt || (e.ExecuteCommandRequest = jt = {})).method = "workspace/executeCommand", qt.messageDirection = t.MessageDirection.clientToServer, qt.type = new t.ProtocolRequestType(qt.method), (At = Lt || (e.ApplyWorkspaceEditRequest = Lt = {})).method = "workspace/applyEdit", At.messageDirection = t.MessageDirection.serverToClient, At.type = new t.ProtocolRequestType("workspace/applyEdit")
-    }(La);
-var Fu = {};
-Object.defineProperty(Fu, "__esModule", {
-    value: !0
-}), Fu.createProtocolConnection = void 0;
-const Wu = Lr;
-Fu.createProtocolConnection = function(e, t, n, r) {
-        return Wu.ConnectionStrategy.is(r) && (r = {
+    }(da);
+var mu = {};
+Object.defineProperty(mu, "__esModule", {
+    value: !0
+}), mu.createProtocolConnection = void 0;
+const gu = Ir;
+mu.createProtocolConnection = function(e, t, n, r) {
+        return gu.ConnectionStrategy.is(r) && (r = {
             connectionStrategy: r
-        }), (0, Wu.createMessageConnection)(e, t, n, r)
+        }), (0, gu.createMessageConnection)(e, t, n, r)
     },
     function(e) {
         var t = Y && Y.__createBinding || (Object.create ? function(e, t, n, r) {
                 void 0 === r && (r = n);
                 var o = Object.getOwnPropertyDescriptor(t, n);
                 o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
                     enumerable: !0,
@@ -11614,23 +11654,23 @@
                 void 0 === r && (r = n), e[r] = t[n]
             }),
             n = Y && Y.__exportStar || function(e, n) {
                 for (var r in e) "default" === r || Object.prototype.hasOwnProperty.call(n, r) || t(n, e, r)
             };
         Object.defineProperty(e, "__esModule", {
             value: !0
-        }), e.LSPErrorCodes = e.createProtocolConnection = void 0, n(Lr, e), n(Pa, e), n(Oa, e), n(La, e);
-        var r, o, i = Fu;
+        }), e.LSPErrorCodes = e.createProtocolConnection = void 0, n(Ir, e), n(sa, e), n(aa, e), n(da, e);
+        var r, o, i = mu;
         Object.defineProperty(e, "createProtocolConnection", {
             enumerable: !0,
             get: function() {
                 return i.createProtocolConnection
             }
         }), (o = r || (e.LSPErrorCodes = r = {})).lspReservedErrorRangeStart = -32899, o.RequestFailed = -32803, o.ServerCancelled = -32802, o.ContentModified = -32801, o.RequestCancelled = -32800, o.lspReservedErrorRangeEnd = -32800
-    }(Ta),
+    }(ea),
     function(e) {
         var t = Y && Y.__createBinding || (Object.create ? function(e, t, n, r) {
                 void 0 === r && (r = n);
                 var o = Object.getOwnPropertyDescriptor(t, n);
                 o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
                     enumerable: !0,
                     get: function() {
@@ -11642,32 +11682,32 @@
             }),
             n = Y && Y.__exportStar || function(e, n) {
                 for (var r in e) "default" === r || Object.prototype.hasOwnProperty.call(n, r) || t(n, e, r)
             };
         Object.defineProperty(e, "__esModule", {
             value: !0
         }), e.createProtocolConnection = void 0;
-        const r = Ra;
-        n(Ra, e), n(Ta, e), e.createProtocolConnection = function(e, t, n, o) {
+        const r = Ys;
+        n(Ys, e), n(ea, e), e.createProtocolConnection = function(e, t, n, o) {
             return (0, r.createMessageConnection)(e, t, n, o)
         }
-    }(qr);
-const Hu = 1e4,
-    Ku = Object.fromEntries(Object.entries(qr.CompletionItemKind).map((([e, t]) => [t, e]))),
-    Uu = e => e.reduce(((e, t) => t), ""),
-    Vu = te.define({
-        combine: Uu
+    }(Ar);
+const vu = 1e4,
+    yu = Object.fromEntries(Object.entries(Ar.CompletionItemKind).map((([e, t]) => [t, e]))),
+    bu = e => e.reduce(((e, t) => t), ""),
+    wu = te.define({
+        combine: bu
     }),
-    $u = te.define({
-        combine: Uu
+    Cu = te.define({
+        combine: bu
     }),
-    zu = te.define({
-        combine: Uu
+    xu = te.define({
+        combine: bu
     });
-class Ju {
+class ku {
     constructor(e) {
         this.rootUri = e.rootUri, this.workspaceFolders = e.workspaceFolders, this.autoClose = e.autoClose, this.plugins = [], this.transport = e.transport, this.requestManager = new $t.RequestManager([this.transport]), this.client = new $t.Client(this.requestManager), this.client.onNotification((e => {
             this.processNotification(e)
         }));
         const t = this.transport;
         t && t.connection && t.connection.addEventListener("message", (e => {
             const n = JSON.parse(e.data);
@@ -11748,18 +11788,18 @@
     textDocumentDidOpen(e) {
         return this.notify("textDocument/didOpen", e)
     }
     textDocumentDidChange(e) {
         return this.notify("textDocument/didChange", e)
     }
     async textDocumentHover(e) {
-        return await this.request("textDocument/hover", e, Hu)
+        return await this.request("textDocument/hover", e, vu)
     }
     async textDocumentCompletion(e) {
-        return await this.request("textDocument/completion", e, Hu)
+        return await this.request("textDocument/completion", e, vu)
     }
     attachPlugin(e) {
         this.plugins.push(e)
     }
     detachPlugin(e) {
         const t = this.plugins.indexOf(e); - 1 !== t && (this.plugins.splice(t, 1), this.autoClose && this.close())
     }
@@ -11775,17 +11815,17 @@
             params: t
         })
     }
     processNotification(e) {
         for (const t of this.plugins) t.processNotification(e)
     }
 }
-class Qu {
+class Ru {
     constructor(e, t) {
-        this.view = e, this.allowHTMLContent = t, this.client = this.view.state.facet(Vu), this.documentUri = this.view.state.facet($u), this.languageId = this.view.state.facet(zu), this.documentVersion = 0, this.changesTimeout = 0, this.client.attachPlugin(this), this.initialize({
+        this.view = e, this.allowHTMLContent = t, this.client = this.view.state.facet(wu), this.documentUri = this.view.state.facet(Cu), this.languageId = this.view.state.facet(xu), this.documentVersion = 0, this.changesTimeout = 0, this.client.attachPlugin(this), this.initialize({
             documentText: this.view.state.doc.toString()
         })
     }
     update({
         docChanged: e
     }) {
         e && (this.changesTimeout && clearTimeout(this.changesTimeout), this.changesTimeout = self.setTimeout((() => {
@@ -11849,21 +11889,21 @@
             }
         });
         if (!r) return null;
         const {
             contents: o,
             range: i
         } = r;
-        let s, a = Gu(e.state.doc, {
+        let s, a = Tu(e.state.doc, {
             line: t,
             character: n
         });
-        if (i && (a = Gu(e.state.doc, i.start), s = Gu(e.state.doc, i.end)), null === a) return null;
+        if (i && (a = Tu(e.state.doc, i.start), s = Tu(e.state.doc, i.end)), null === a) return null;
         const c = document.createElement("div");
-        return c.classList.add("documentation"), this.allowHTMLContent ? c.innerHTML = Zu(o) : c.textContent = Zu(o), {
+        return c.classList.add("documentation"), this.allowHTMLContent ? c.innerHTML = Mu(o) : c.textContent = Mu(o), {
             pos: a,
             end: s,
             create: e => ({
                 dom: c
             }),
             above: !0
         }
@@ -11903,32 +11943,32 @@
             filterText: s
         }) => {
             var a;
             const c = {
                 label: t,
                 detail: e,
                 apply: null !== (a = null == r ? void 0 : r.newText) && void 0 !== a ? a : t,
-                type: n && Ku[n].toLowerCase(),
+                type: n && yu[n].toLowerCase(),
                 sortText: null != i ? i : t,
                 filterText: null != s ? s : t
             };
-            return o && (c.info = Zu(o)), c
+            return o && (c.info = Mu(o)), c
         }));
         const [a, c] = function(e) {
             const t = new Set,
                 n = new Set;
             for (const {
                     apply: o
                 }
                 of e) {
                 const [e, ...r] = o;
                 t.add(e);
                 for (const t of r) n.add(t)
             }
-            const r = Yu(t) + Yu(n) + "*$";
+            const r = Du(t) + Du(n) + "*$";
             return [new RegExp("^" + r), new RegExp(r)]
         }(s), l = e.matchBefore(c);
         let {
             pos: u
         } = e;
         if (l) {
             u = l.from;
@@ -11964,21 +12004,21 @@
     processDiagnostics(e) {
         if (e.uri !== this.documentUri) return;
         const t = e.diagnostics.map((({
             range: e,
             message: t,
             severity: n
         }) => ({
-            from: Gu(this.view.state.doc, e.start),
-            to: Gu(this.view.state.doc, e.end),
+            from: Tu(this.view.state.doc, e.start),
+            to: Tu(this.view.state.doc, e.end),
             severity: {
-                [qr.DiagnosticSeverity.Error]: "error",
-                [qr.DiagnosticSeverity.Warning]: "warning",
-                [qr.DiagnosticSeverity.Information]: "info",
-                [qr.DiagnosticSeverity.Hint]: "info"
+                [Ar.DiagnosticSeverity.Error]: "error",
+                [Ar.DiagnosticSeverity.Warning]: "warning",
+                [Ar.DiagnosticSeverity.Information]: "info",
+                [Ar.DiagnosticSeverity.Hint]: "info"
             } [n],
             message: t
         }))).filter((({
             from: e,
             to: t
         }) => null !== e && null !== t && void 0 !== e && void 0 !== t)).sort(((e, t) => {
             switch (!0) {
@@ -11989,45 +12029,45 @@
             }
             return 0
         }));
         this.view.dispatch(oe(this.view.state, t))
     }
 }
 
-function Gu(e, t) {
+function Tu(e, t) {
     if (t.line >= e.lines) return;
     const n = e.line(t.line + 1).from + t.character;
     return n > e.length ? void 0 : n
 }
 
-function Xu(e, t) {
+function Su(e, t) {
     const n = e.lineAt(t);
     return {
         line: n.number - 1,
         character: t - n.from
     }
 }
 
-function Zu(e) {
-    return Array.isArray(e) ? e.map((e => Zu(e) + "\n\n")).join("") : "string" == typeof e ? e : e.value
+function Mu(e) {
+    return Array.isArray(e) ? e.map((e => Mu(e) + "\n\n")).join("") : "string" == typeof e ? e : e.value
 }
 
-function Yu(e) {
+function Du(e) {
     let t = "",
         n = Array.from(e).join("");
     return /\w/.test(n) && (t += "\\w", n = n.replace(/\w/g, "")), `[${t}${n.replace(/[^\w\s]/g,"\\$&")}]`
 }
 
-function ed(e) {
+function _u(e) {
     return [...ie().map((t => {
         const n = se(t);
         return n === e ? null : n
     })).filter(Boolean).sort(((e, t) => e.startsWith("import") && !t.startsWith("import") ? -1 : !e.startsWith("import") && t.startsWith("import") ? 1 : 0)), e].join("\n")
 }
-class td extends Ju {
+class Eu extends ku {
     constructor() {
         super(...arguments), t(this, "documentVersion", 0)
     }
     _request(e, t) {
         return this.request(e, t)
     }
     isDisabled() {
@@ -12039,17 +12079,17 @@
     async textDocumentCompletion(e) {
         return this.isDisabled() ? [] : super.textDocumentCompletion(e)
     }
     async textDocumentDidChange(e) {
         return this.isDisabled() ? e : super.textDocumentDidChange({
             ...e,
             contentChanges: [{
-                text: ed(e.contentChanges[0].text)
+                text: _u(e.contentChanges[0].text)
             }],
-            textDocument: qr.VersionedTextDocumentIdentifier.create(e.textDocument.uri, ++this.documentVersion)
+            textDocument: Ar.VersionedTextDocumentIdentifier.create(e.textDocument.uri, ++this.documentVersion)
         })
     }
     textDocumentHover(e) {
         return this.isDisabled() ? Promise.resolve({
             contents: []
         }) : super.textDocumentHover(e)
     }
@@ -12084,129 +12124,129 @@
             doc: {
                 ...e.doc,
                 version: t
             }
         })
     }
 }
-async function nd(e) {
+async function Pu(e) {
     return new Promise(((t, n) => {
         const r = new WebSocket(e);
         r.onopen = () => {
             r.close(), t(e)
         }, r.onerror = t => {
             r.close(), n(new Error(`Failed to connect to ${e}: ${t.type}`))
         }
     }))
 }
-const rd = "/marimo.py",
-    od = "copilot",
-    id = `file://${rd}`,
-    sd = ce((() => new ad));
-class ad extends yn {
+const Ou = "/marimo.py",
+    Nu = "copilot",
+    ju = `file://${Ou}`,
+    qu = ce((() => new Lu));
+class Lu extends yn {
     constructor() {
         super(), t(this, "delegate"), this.delegate = void 0
     }
     async connect() {
         return await X(Z, (e => e.completion.copilot)), await async function(e, t = 5) {
             for (let n = 0; n < t; n++) try {
-                return await nd(e)
+                return await Pu(e)
             } catch {
                 await new Promise((e => setTimeout(e, 1e3 * (n + 1))))
             }
             throw new Error(`Failed to connect to ${e}`)
-        }(ud(), 3), this.delegate || (this.delegate = new $t.WebSocketTransport(ud())), this.delegate.connect()
+        }(Bu(), 3), this.delegate || (this.delegate = new $t.WebSocketTransport(Bu())), this.delegate.connect()
     }
     close() {
         var e;
         null == (e = this.delegate) || e.close()
     }
     async sendData(e, t) {
         var n;
         return null == (n = this.delegate) ? void 0 : n.sendData(e, t)
     }
 }
-const cd = ce((() => new td({
-    rootUri: id,
-    documentUri: id,
-    languageId: od,
+const Au = ce((() => new Eu({
+    rootUri: ju,
+    documentUri: ju,
+    languageId: Nu,
     workspaceFolders: null,
-    transport: sd()
+    transport: qu()
 })));
 
-function ld() {
+function Iu() {
     return function(e) {
         let t = null;
-        return [Vu.of(e.client || new Ju({
+        return [wu.of(e.client || new ku({
             ...e,
             autoClose: !0
-        })), $u.of(e.documentUri), zu.of(e.languageId), R.define((n => t = new Qu(n, e.allowHTMLContent))), ne(((e, n) => {
+        })), Cu.of(e.documentUri), xu.of(e.languageId), R.define((n => t = new Ru(n, e.allowHTMLContent))), ne(((e, n) => {
             var r;
-            return null !== (r = null == t ? void 0 : t.requestHoverTooltip(e, Xu(e.state.doc, n))) && void 0 !== r ? r : null
+            return null !== (r = null == t ? void 0 : t.requestHoverTooltip(e, Su(e.state.doc, n))) && void 0 !== r ? r : null
         })), re({
             override: [async e => {
                 var n, r, o;
                 if (null == t) return null;
                 const {
                     state: i,
                     pos: s,
                     explicit: a
                 } = e, c = i.doc.lineAt(s);
-                let l, u = qr.CompletionTriggerKind.Invoked;
-                return !a && (null === (o = null === (r = null === (n = t.client.capabilities) || void 0 === n ? void 0 : n.completionProvider) || void 0 === r ? void 0 : r.triggerCharacters) || void 0 === o ? void 0 : o.includes(c.text[s - c.from - 1])) && (u = qr.CompletionTriggerKind.TriggerCharacter, l = c.text[s - c.from - 1]), u !== qr.CompletionTriggerKind.Invoked || e.matchBefore(/\w+$/) ? await t.requestCompletion(e, Xu(i.doc, s), {
+                let l, u = Ar.CompletionTriggerKind.Invoked;
+                return !a && (null === (o = null === (r = null === (n = t.client.capabilities) || void 0 === n ? void 0 : n.completionProvider) || void 0 === r ? void 0 : r.triggerCharacters) || void 0 === o ? void 0 : o.includes(c.text[s - c.from - 1])) && (u = Ar.CompletionTriggerKind.TriggerCharacter, l = c.text[s - c.from - 1]), u !== Ar.CompletionTriggerKind.Invoked || e.matchBefore(/\w+$/) ? await t.requestCompletion(e, Su(i.doc, s), {
                     triggerKind: u,
                     triggerCharacter: l
                 }) : null
             }]
         })]
     }({
-        rootUri: id,
-        documentUri: id,
+        rootUri: ju,
+        documentUri: ju,
         workspaceFolders: [],
-        transport: sd(),
-        client: cd(),
-        languageId: od
+        transport: qu(),
+        client: Au(),
+        languageId: Nu
     })
 }
 
-function ud() {
+function Bu() {
     const e = `${window.location.port}0`;
     return `${"https:"===window.location.protocol?"wss":"ws"}://${window.location.hostname}:${e}/copilot`
 }
-const dd = p.memo((() => {
+const Fu = p.memo((() => {
     const [e, t] = le(Kt), [n, r] = p.useState(), [s, a] = p.useState(), [c, l] = p.useState(!1);
     p.useEffect((() => {
-        const e = cd();
+        const e = Au();
         e.initializePromise.catch((() => {
             t(!1), r("notConnected")
         })), e.signedIn().then((e => {
             t(e), r(e ? "signedIn" : "signedOut")
         })).catch((() => {
             t(!1), r("notConnected")
         }))
     }), []);
     const u = async e => {
         e.preventDefault(), l(!0);
         try {
-            const e = cd(),
+            const e = Au(),
                 {
                     verificationUri: n,
                     status: o,
                     userCode: i
                 } = await e.signInInitiate();
             "OK" === o || "AlreadySignedIn" === o ? t(!0) : (r("signingIn"), a({
                 url: n,
                 code: i
             }))
         } finally {
             l(!1)
         }
     }, d = async e => {
         if (e.preventDefault(), !s) return;
-        const n = cd();
+        const n = Au();
         try {
             l(!0);
             const {
                 status: e
             } = await n.signInConfirm({
                 userCode: s.code
             });
@@ -12218,15 +12258,15 @@
             }
             r("signInFailed")
         } finally {
             l(!1)
         }
     }, f = async e => {
         e.preventDefault();
-        const n = cd();
+        const n = Au();
         t(!1), r("signedOut"), await n.signOut()
     };
     return (() => {
         switch (n ?? (e ? "signedIn" : "connecting")) {
             case "connecting":
                 return o.jsx(ue, {
                     className: "font-normal flex",
@@ -12327,38 +12367,38 @@
                             children: "docs"
                         }), "."]
                     })]
                 })
         }
     })()
 }));
-dd.displayName = "CopilotConfig";
-const hd = ({
+Fu.displayName = "CopilotConfig";
+const Wu = ({
         children: e
     }) => o.jsx("div", {
         className: "text-md font-semibold text-muted-foreground uppercase tracking-wide  mb-1",
         children: e
     }),
-    fd = ({
+    Hu = ({
         children: e
     }) => o.jsx("div", {
         className: "text-sm font-semibold underline-offset-2 text-accent-foreground uppercase tracking-wide",
         children: e
     }),
-    pd = ({
+    Ku = ({
         children: e
     }) => o.jsx("p", {
         className: "text-sm text-muted-foreground",
         children: e
     }),
-    md = e => o.jsx("kbd", {
+    Uu = e => o.jsx("kbd", {
         className: c(e.className, "rounded-md bg-muted/40 px-2 text-[0.75rem] font-prose center border border-foreground/20 text-muted-foreground block"),
         children: e.children
     }),
-    gd = () => {
+    Vu = () => {
         const [e, t] = ge(), n = p.useRef(null), r = ve({
             resolver: ye(je),
             defaultValues: e
         }), i = async e => {
             await qe({
                 config: e
             }).then((() => {
@@ -12368,22 +12408,22 @@
         return o.jsx(we, {
             ...r,
             children: o.jsxs("form", {
                 ref: n,
                 onChange: r.handleSubmit(i),
                 className: "flex flex-col gap-5",
                 children: [o.jsxs("div", {
-                    children: [o.jsx(hd, {
+                    children: [o.jsx(Wu, {
                         children: "User Config"
-                    }), o.jsx(pd, {
+                    }), o.jsx(Ku, {
                         children: "Settings applied to all marimo notebooks"
                     })]
                 }), o.jsxs("div", {
                     className: "flex flex-col gap-3",
-                    children: [o.jsx(fd, {
+                    children: [o.jsx(Hu, {
                         children: "Editor"
                     }), o.jsx("div", {
                         children: o.jsx(Ce, {
                             control: r.control,
                             name: "save.autosave",
                             render: ({
                                 field: e
@@ -12528,15 +12568,15 @@
                                     }, e)))
                                 })
                             }), o.jsx(Me, {})]
                         })
                     })]
                 }), o.jsxs("div", {
                     className: "flex flex-col gap-3",
-                    children: [o.jsx(fd, {
+                    children: [o.jsx(Hu, {
                         children: "Display"
                     }), o.jsx(Ce, {
                         control: r.control,
                         name: "display.theme",
                         render: ({
                             field: e
                         }) => o.jsxs(xe, {
@@ -12606,15 +12646,15 @@
                             }), o.jsx(Me, {}), o.jsx(De, {
                                 children: "Where to display cell's output."
                             })]
                         })
                     })]
                 }), o.jsxs("div", {
                     className: "flex flex-col gap-3",
-                    children: [o.jsx(fd, {
+                    children: [o.jsx(Hu, {
                         children: "Package Management"
                     }), o.jsx(Ce, {
                         control: r.control,
                         disabled: s,
                         name: "package_management.manager",
                         render: ({
                             field: e
@@ -12634,15 +12674,15 @@
                                     }, e)))
                                 })
                             }), o.jsx(Me, {})]
                         })
                     })]
                 }), o.jsxs("div", {
                     className: "flex flex-col gap-3",
-                    children: [o.jsx(fd, {
+                    children: [o.jsx(Hu, {
                         children: "Runtime"
                     }), o.jsx(Ce, {
                         control: r.control,
                         name: "runtime.auto_instantiate",
                         render: ({
                             field: e
                         }) => o.jsxs(xe, {
@@ -12715,19 +12755,19 @@
                             }), o.jsx(De, {
                                 children: 'Whether marimo should automatically reload modules before executing cells. If "lazy", marimo will mark cells affected by module modifications as stale; if "autorun", affected cells will be automatically re-run.'
                             })]
                         })
                     })]
                 }), o.jsxs("div", {
                     className: "flex flex-col gap-3",
-                    children: [o.jsx(fd, {
+                    children: [o.jsx(Hu, {
                         children: "AI Assist"
                     }), o.jsxs("p", {
                         className: "text-sm text-muted-secondary",
-                        children: ["You will need to store an API key in your", " ", o.jsx(md, {
+                        children: ["You will need to store an API key in your", " ", o.jsx(Uu, {
                             className: "inline",
                             children: "~/.marimo.toml"
                         }), " file. See the", " ", o.jsx("a", {
                             className: "text-link hover:underline",
                             href: "https://docs.marimo.io/guides/ai_completion.html",
                             target: "_blank",
                             rel: "noreferrer",
@@ -12778,15 +12818,15 @@
                                     onBlur: e => t(e.target.value)
                                 })
                             }), o.jsx(Me, {})]
                         })
                     })]
                 }), o.jsxs("div", {
                     className: "flex flex-col gap-3",
-                    children: [o.jsx(fd, {
+                    children: [o.jsx(Hu, {
                         children: "GitHub Copilot"
                     }), o.jsx(Ce, {
                         control: r.control,
                         disabled: s,
                         name: "completion.copilot",
                         render: ({
                             field: e
@@ -12804,22 +12844,22 @@
                                             e.onChange(Boolean(t))
                                         }
                                     })
                                 }), o.jsx(Te, {
                                     className: "font-normal flex",
                                     children: "Enable"
                                 })]
-                            }), e.value && o.jsx(dd, {})]
+                            }), e.value && o.jsx(Fu, {})]
                         })
                     })]
                 })]
             })
         })
     },
-    vd = () => {
+    $u = () => {
         const [e, t] = Le(), n = ve({
             resolver: ye(Be),
             defaultValues: e
         });
         return p.useEffect((() => {
             window.dispatchEvent(new Event("resize"))
         }), [e.width]), o.jsx(we, {
@@ -12832,17 +12872,17 @@
                         t(e)
                     })).catch((() => {
                         t(e)
                     }))
                 })),
                 className: "flex flex-col gap-4",
                 children: [o.jsxs("div", {
-                    children: [o.jsx(hd, {
+                    children: [o.jsx(Wu, {
                         children: "Application Config"
-                    }), o.jsx(pd, {
+                    }), o.jsx(Ku, {
                         children: "Settings applied to this notebook"
                     })]
                 }), o.jsx(Ce, {
                     control: n.control,
                     name: "width",
                     render: ({
                         field: e
@@ -12887,15 +12927,15 @@
                             children: "The application title is put in the title tag in the HTML code and typically displayed in the title bar of the browser window."
                         })]
                     })
                 })]
             })
         })
     },
-    yd = ({
+    zu = ({
         showAppConfig: e = !0
     }) => o.jsxs(We, {
         children: [o.jsx(He, {
             asChild: !0,
             children: o.jsx(Ge, {
                 "aria-label": "Config",
                 "data-testid": "app-config-button",
@@ -12912,37 +12952,37 @@
             })
         }), o.jsxs(Ke, {
             className: "w-80 h-[90vh] overflow-auto",
             align: "end",
             side: "bottom",
             onFocusOutside: e => e.preventDefault(),
             children: [e && o.jsxs(o.Fragment, {
-                children: [o.jsx(vd, {}), o.jsx("div", {
+                children: [o.jsx($u, {}), o.jsx("div", {
                     className: "h-px bg-border my-4"
                 })]
-            }), o.jsx(gd, {})]
+            }), o.jsx(Vu, {})]
         })]
     }),
-    bd = e => o.jsx("svg", {
+    Ju = e => o.jsx("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         width: "1em",
         height: "1em",
         viewBox: "0 0 448 512",
         ...e,
         children: o.jsx("path", {
             d: "M439.8 200.5c-7.7-30.9-22.3-54.2-53.4-54.2h-40.1v47.4c0 36.8-31.2 67.8-66.8 67.8H172.7c-29.2 0-53.4 25-53.4 54.3v101.8c0 29 25.2 46 53.4 54.3 33.8 9.9 66.3 11.7 106.8 0 26.9-7.8 53.4-23.5 53.4-54.3v-40.7H226.2v-13.6h160.2c31.1 0 42.6-21.7 53.4-54.2 11.2-33.5 10.7-65.7 0-108.6zM286.2 404c11.1 0 20.1 9.1 20.1 20.3 0 11.3-9 20.4-20.1 20.4-11 0-20.1-9.2-20.1-20.4.1-11.3 9.1-20.3 20.1-20.3zM167.8 248.1h106.8c29.7 0 53.4-24.5 53.4-54.3V91.9c0-29-24.4-50.7-53.4-55.6-35.8-5.9-74.7-5.6-106.8.1-45.2 8-53.4 24.7-53.4 55.6v40.7h106.9v13.6h-147c-31.1 0-58.3 18.7-66.8 54.2-9.8 40.7-10.2 66.1 0 108.6 7.6 31.6 25.7 54.2 56.8 54.2H101v-48.8c0-35.3 30.5-66.4 66.8-66.4zm-6.7-142.6c-11.1 0-20.1-9.1-20.1-20.3.1-11.3 9-20.4 20.1-20.4 11 0 20.1 9.2 20.1 20.4s-9 20.3-20.1 20.3z"
         })
     }),
-    wd = e => o.jsx("svg", {
+    Qu = e => o.jsx("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         width: "1em",
         height: "1em",
         viewBox: "0 0 640 512",
         fill: "currentColor",
         ...e,
         children: o.jsx("path", {
             d: "M593.8 59.1H46.2C20.7 59.1 0 79.8 0 105.2v301.5c0 25.5 20.7 46.2 46.2 46.2h547.7c25.5 0 46.2-20.7 46.1-46.1V105.2c0-25.4-20.7-46.1-46.2-46.1zM338.5 360.6H277v-120l-61.5 76.9-61.5-76.9v120H92.3V151.4h61.5l61.5 76.9 61.5-76.9h61.5v209.2zm135.3 3.1L381.5 256H443V151.4h61.5V256H566z"
         })
     });
 export {
-    Ge as B, yd as C, md as K, od as L, wd as M, Ue as P, ze as S, Xe as a, bd as b, Lt as c, ld as d, Ut as e, cd as f, ed as g, rd as h, qt as i, Ve as j, Ft as k, Ze as u
+    Ge as B, zu as C, Uu as K, Nu as L, Qu as M, Ue as P, ze as S, Xe as a, Ju as b, Lt as c, Iu as d, Ut as e, Au as f, _u as g, Ou as h, qt as i, Ve as j, Ft as k, Ze as u
 };
```

### Comparing `marimo-0.6.3/marimo/_static/assets/icons-D-PkNarU.css` & `marimo-0.6.4/marimo/_static/assets/icons-D-PkNarU.css`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/idl-pcmmZuaN.js` & `marimo-0.6.4/marimo/_static/assets/idl-pcmmZuaN.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/index-0fF0Xoai.js` & `marimo-0.6.4/marimo/_static/assets/index-BYVYp6Ei.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     iX as t,
     iS as Q,
     j7 as o,
     iP as l,
     iJ as p,
     c7 as s,
     iI as c
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const P = new c((O => {
     let $ = O.pos;
     for (;;) {
         let {
             next: a
         } = O;
         if (a < 0) break;
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-7VEF_U3p.js` & `marimo-0.6.4/marimo/_static/assets/index-DgOauLen.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     iO as i,
     iW as a,
     iY as r,
     jb as P,
     iX as U,
     iS as t,
     iT as Y
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const S = new O((O => {
         if (76 == O.next || 85 == O.next ? O.advance() : 117 == O.next && (O.advance(), 56 == O.next && O.advance()), 82 != O.next) return;
         if (O.advance(), 34 != O.next) return;
         O.advance();
         let Q = "";
         for (; 40 != O.next;) {
             if (32 == O.next || O.next <= 13 || 41 == O.next) return;
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-BuR6fZZm.js` & `marimo-0.6.4/marimo/_static/assets/index-CE06HdF7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
     iJ as $,
     iQ as X,
     iO as i,
     iW as e,
     iY as n,
     iS as a,
     iT as S
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 
 function r(O) {
     return O >= 48 && O <= 57
 }
 
 function s(O) {
     return r(O) || 95 == O
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-C2GbrbZr.js` & `marimo-0.6.4/marimo/_static/assets/index-DCESMHe2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     iO as a,
     iW as i,
     iY as X,
     jb as e,
     iX as r,
     iS as s,
     iT as S
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const l = O({
         null: Q.null,
         instanceof: Q.operatorKeyword,
         this: Q.self,
         "new super assert open to with void": Q.keyword,
         "class interface extends implements enum var": Q.definitionKeyword,
         "module package import": Q.moduleKeyword,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-CC7Qmxzq.css` & `marimo-0.6.4/marimo/_static/assets/index-CC7Qmxzq.css`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/index-ChUg6Fde.js` & `marimo-0.6.4/marimo/_static/assets/index-AJ6VyMaJ.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     gd as t
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 
 function r(t) {
     return ((t = Math.exp(t)) + 1 / t) / 2
 }
 const e = function t(e, n, o) {
     function u(t, u) {
         var a, f, i = t[0],
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-Ck0jzFpb.js` & `marimo-0.6.4/marimo/_static/assets/index-CB4e2-IR.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     iP as z,
     iO as S,
     iW as P,
     iY as W,
     iX as T,
     iS as e,
     iT as s
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const X = {
     abstract: 4,
     and: 5,
     array: 6,
     as: 7,
     true: 8,
     false: 8,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-ClCDnvOE.js` & `marimo-0.6.4/marimo/_static/assets/index-yuQsQmno.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     iM as i,
     iO as s,
     iI as o,
     iJ as l,
     iU as c,
     iV as d,
     c7 as u
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const m = 5,
     p = 6,
     f = 20,
     g = 21,
     h = 24;
 
 function _(e) {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-CohQOVlj.js` & `marimo-0.6.4/marimo/_static/assets/index-KIzq3vhX.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     iJ as a,
     iQ as r,
     iO as l,
     iW as o,
     iS as s,
     jg as i,
     c7 as y
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 
 function $(O) {
     return 45 == O || 46 == O || 58 == O || O >= 65 && O <= 90 || 95 == O || O >= 97 && O <= 122 || O >= 161
 }
 let c = null,
     p = null,
     S = 0;
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-CzWuvzvc.js` & `marimo-0.6.4/marimo/_static/assets/index-DtyNPFfa.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     iN as e,
     iM as r,
     j7 as n,
     iP as a,
     iJ as i,
     jc as o,
     i$ as l
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const s = i.deserialize({
         version: 14,
         states: "%pOVOWOOObQPOOOpOSO'#C_OOOO'#Cp'#CpQVOWOOQxQPOOO!TQQOOQ!YQPOOOOOO,58y,58yO!_OSO,58yOOOO-E6n-E6nO!dQQO'#CqQ{QPOOO!iQPOOQ{QPOOO!qQPOOOOOO1G.e1G.eOOQO,59],59]OOQO-E6o-E6oO!yOpO'#CiO#RO`O'#CiQOQPOOO#ZO#tO'#CmO#fO!bO'#CmOOQO,59T,59TO#qOpO,59TO#vO`O,59TOOOO'#Cr'#CrO#{O#tO,59XOOQO,59X,59XOOOO'#Cs'#CsO$WO!bO,59XOOQO1G.o1G.oOOOO-E6p-E6pOOQO1G.s1G.sOOOO-E6q-E6q",
         stateData: "$g~OjOS~OQROUROkQO~OWTOXUOZUO`VO~OSXOTWO~OXUO[]OlZO~OY^O~O[_O~OT`O~OYaO~OmcOodO~OmfOogO~O^iOnhO~O_jOphO~ObkOqkOrmO~OcnOsnOtmO~OnpO~OppO~ObkOqkOrrO~OcnOsnOtrO~OWX`~",
         goto: "!^hPPPiPPPPPPPPPmPPPpPPsy!Q!WTROSRe]Re_QSORYSS[T^Rb[QlfRqlQogRso",
         nodeNames: "⚠ Content Text Interpolation InterpolationContent }} Entity Attribute VueAttributeName : Identifier @ Is ScriptAttributeValue AttributeScript AttributeScript AttributeName AttributeValue Entity Entity",
         maxTerm: 36,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-D4als0Dc.js` & `marimo-0.6.4/marimo/_static/assets/index-XFgu4285.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     iQ as e,
     iN as t,
     iM as n,
     j7 as a,
     iP as i,
     iJ as o,
     iI as p
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const Q = new p((O => {
     let r = O.pos;
     for (;;) {
         if (10 == O.next) {
             O.advance();
             break
         }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-DgcwnKY7.js` & `marimo-0.6.4/marimo/_static/assets/index-DahJleVt.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     iQ as i,
     iO as n,
     iS as t,
     iT as R,
     iW as o,
     iY as l,
     jf as S
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const r = [9, 10, 11, 12, 13, 32, 133, 160, 5760, 8192, 8193, 8194, 8195, 8196, 8197, 8198, 8199, 8200, 8201, 8202, 8232, 8233, 8239, 8287, 12288],
     d = 10;
 
 function c(O) {
     return O >= 65 && O <= 90 || O >= 97 && O <= 122 || O >= 161
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-Dq6tg2Hn.js` & `marimo-0.6.4/marimo/_static/assets/index-Cd3MtTMQ.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-const __vite__fileDeps = ["./home-page-BmvI7Tzs.js", "./icons-6JftBaIY.js", "./icons-D-PkNarU.css", "./run-page-BflrRP7S.js", "./useMarimoWebSocket-DFV8TeGX.js", "./useMarimoWebSocket-BjNzCf7j.css", "./edit-page-CIzFhPq5.js", "./transform-DGMfQOK3.js", "./timer-D8GWrtRJ.js", "./index-ChUg6Fde.js", "./sortBy-D0xI_7yL.js", "./_baseEach-BrSWFoJM.js", "./edit-page-CwGzkSpM.css", "./dockerfile-BLgfkd__.js", "./simple-mode-Ckv7_vD8.js", "./factor-Bm2WRyNM.js", "./nsis-Csd3_MSv.js", "./pug-BNyZbGOm.js", "./javascript-DY1Qj14w.js", "./CarouselComponent-DtCAwyzo.js", "./CarouselComponent-C12Ecb2K.css", "./vega-component-CZ4hZbd6.js", "./VegaLite-BQwzJofD.js", "./time-CUBsQdfc.js", "./linear-DF6Se9n2.js", "./init-DLRA0X12.js", "./range-CtcPcB_L.js", "./ordinal-DDUp3AbE.js", "./arc-DIImc9ZO.js", "./path-qnb_ma6O.js", "./step-BEJ6WznM.js", "./array-DmjLdZ15.js", "./line-Dz7yhIWK.js", "./any-language-editor-D3MTmtyo.js", "./index-DzhIfGoT.js", "./index-DgcwnKY7.js", "./index-S9qVQ2oC.js", "./index-CohQOVlj.js", "./index-ClCDnvOE.js", "./index-C2GbrbZr.js", "./index-BuR6fZZm.js", "./index-7VEF_U3p.js", "./index-Ck0jzFpb.js", "./index-0fF0Xoai.js", "./index-jW3n8_hn.js", "./index-CzWuvzvc.js", "./index-D4als0Dc.js", "./apl-CXdQSnD-.js", "./asciiarmor-D5V0T9Cu.js", "./asterisk-B46aRdXb.js", "./brainfuck-CtZaYBKt.js", "./clike-BPCXT8V3.js", "./cmake-DXn5xaP-.js", "./cobol-DJhTY0fG.js", "./coffeescript-BTDxI-eT.js", "./commonlisp-D09g7coK.js", "./crystal-CRzZ78HM.js", "./cypher-gJDei3ni.js", "./d-BShv7fp-.js", "./diff-UJJ5BM9S.js", "./dtd-DI9Herc-.js", "./dylan-CHJ5qNM_.js", "./ebnf-B-Df8AvO.js", "./ecl-DPFc0Uaf.js", "./eiffel-BZ5y0wDL.js", "./elm-D7xaZ7Da.js", "./erlang-BuqgqA5h.js", "./fcl-CVaBTCzQ.js", "./forth-Dri_5nFc.js", "./fortran-DL7KluxX.js", "./gas-5kEe4nk0.js", "./gherkin-B6X1vGSW.js", "./groovy-BfRUB6GO.js", "./haskell-CmdsSjFB.js", "./haxe-75PMBtaN.js", "./http-BKJkqRj4.js", "./idl-pcmmZuaN.js", "./jinja2-DhgKlfW7.js", "./julia-DjdwvFuI.js", "./livescript-B19OIWEP.js", "./lua-8DXOpKDz.js", "./mathematica-IIbmv7SK.js", "./mbox-DoeuZPxA.js", "./mirc-DkvFAiy5.js", "./modelica-DSrSSXCg.js", "./mscgen-B2igx18G.js", "./mumps-zvxmGV4l.js", "./nginx-B4hAVlXN.js", "./ntriples-FFvkTduk.js", "./octave-C4hdQ5Hf.js", "./oz-qQq7irPq.js", "./pascal-CZ0JYm71.js", "./perl-tdMlh9QA.js", "./pig-CwGJVRC4.js", "./powershell-D1ly3AHC.js", "./properties-_nPj978X.js", "./protobuf-B4y9do6W.js", "./puppet-Bc-yJKzi.js", "./q-B0kTJ4cI.js", "./r-BA4EbLKE.js", "./ruby-CR-u2WLS.js", "./sas-Bqaci40L.js", "./scheme-qjP0V5Ag.js", "./shell-BLav31RL.js", "./sieve-r025o_jW.js", "./smalltalk-C7J3IyEP.js", "./solr-78MBEUkU.js", "./sparql-BRLJFz69.js", "./spreadsheet-CGlWr0eM.js", "./stex-Ba7Sj9VR.js", "./stylus-C-RTeXnz.js", "./swift-Cbprqdc8.js", "./tcl-B2fODqDH.js", "./textile-BuVhTOzU.js", "./tiddlywiki-BgR6AEZu.js", "./tiki-CI-ztowC.js", "./toml-BQXy8elZ.js", "./troff-Ce85hlLp.js", "./ttcn-C4reStyN.js", "./turtle-BkSuIpt-.js", "./vb-coDLL1b7.js", "./vbscript-MdTt_wcJ.js", "./velocity-BdD_26Jv.js", "./verilog-B4LBqg_1.js", "./vhdl-BRDI21CQ.js", "./webidl-CGwyPRYs.js", "./xquery-BZBLoTvf.js", "./yacas-I8QjZlxf.js", "./z80-D8p3gKXp.js", "./ConnectedDataExplorerComponent-DKdMG7z6.js", "./mermaid-BDDPrcgz.js"],
+const __vite__fileDeps = ["./home-page-BL9ArKPs.js", "./icons-DtRVr9-T.js", "./icons-D-PkNarU.css", "./run-page-D_UJForb.js", "./useMarimoWebSocket-Butgv0ej.js", "./useMarimoWebSocket-BjNzCf7j.css", "./edit-page-DnXnHWMg.js", "./transform-DNjxe6pi.js", "./timer-D8GWrtRJ.js", "./index-AJ6VyMaJ.js", "./sortBy-DwX0cqqB.js", "./_baseEach-FAhoh2N5.js", "./edit-page-CwGzkSpM.css", "./dockerfile-BLgfkd__.js", "./simple-mode-Ckv7_vD8.js", "./factor-Bm2WRyNM.js", "./nsis-Csd3_MSv.js", "./pug-BNyZbGOm.js", "./javascript-DY1Qj14w.js", "./CarouselComponent-ml4W_PuP.js", "./CarouselComponent-C12Ecb2K.css", "./vega-component-B9WTop1f.js", "./VegaLite-rQgmZ7vL.js", "./time-CLRyKR-T.js", "./linear-JxYcrfvc.js", "./init-DLRA0X12.js", "./range-CtcPcB_L.js", "./ordinal-DDUp3AbE.js", "./arc-DIImc9ZO.js", "./path-qnb_ma6O.js", "./step-BEJ6WznM.js", "./array-DmjLdZ15.js", "./line-Dz7yhIWK.js", "./any-language-editor-Dzf9Jczi.js", "./index-1IpQZ_Yu.js", "./index-DahJleVt.js", "./index-DqGPWGPa.js", "./index-KIzq3vhX.js", "./index-yuQsQmno.js", "./index-DCESMHe2.js", "./index-CE06HdF7.js", "./index-DgOauLen.js", "./index-CB4e2-IR.js", "./index-BYVYp6Ei.js", "./index-BH1DvUFb.js", "./index-DtyNPFfa.js", "./index-XFgu4285.js", "./apl-CXdQSnD-.js", "./asciiarmor-D5V0T9Cu.js", "./asterisk-B46aRdXb.js", "./brainfuck-CtZaYBKt.js", "./clike-BPCXT8V3.js", "./cmake-DXn5xaP-.js", "./cobol-DJhTY0fG.js", "./coffeescript-BTDxI-eT.js", "./commonlisp-D09g7coK.js", "./crystal-CRzZ78HM.js", "./cypher-gJDei3ni.js", "./d-BShv7fp-.js", "./diff-UJJ5BM9S.js", "./dtd-DI9Herc-.js", "./dylan-CHJ5qNM_.js", "./ebnf-B-Df8AvO.js", "./ecl-DPFc0Uaf.js", "./eiffel-BZ5y0wDL.js", "./elm-D7xaZ7Da.js", "./erlang-BuqgqA5h.js", "./fcl-CVaBTCzQ.js", "./forth-Dri_5nFc.js", "./fortran-DL7KluxX.js", "./gas-5kEe4nk0.js", "./gherkin-B6X1vGSW.js", "./groovy-BfRUB6GO.js", "./haskell-CmdsSjFB.js", "./haxe-75PMBtaN.js", "./http-BKJkqRj4.js", "./idl-pcmmZuaN.js", "./jinja2-DhgKlfW7.js", "./julia-DjdwvFuI.js", "./livescript-B19OIWEP.js", "./lua-8DXOpKDz.js", "./mathematica-IIbmv7SK.js", "./mbox-DoeuZPxA.js", "./mirc-DkvFAiy5.js", "./modelica-DSrSSXCg.js", "./mscgen-B2igx18G.js", "./mumps-zvxmGV4l.js", "./nginx-B4hAVlXN.js", "./ntriples-FFvkTduk.js", "./octave-C4hdQ5Hf.js", "./oz-qQq7irPq.js", "./pascal-CZ0JYm71.js", "./perl-tdMlh9QA.js", "./pig-CwGJVRC4.js", "./powershell-D1ly3AHC.js", "./properties-_nPj978X.js", "./protobuf-B4y9do6W.js", "./puppet-Bc-yJKzi.js", "./q-B0kTJ4cI.js", "./r-BA4EbLKE.js", "./ruby-CR-u2WLS.js", "./sas-Bqaci40L.js", "./scheme-qjP0V5Ag.js", "./shell-BLav31RL.js", "./sieve-r025o_jW.js", "./smalltalk-C7J3IyEP.js", "./solr-78MBEUkU.js", "./sparql-BRLJFz69.js", "./spreadsheet-CGlWr0eM.js", "./stex-Ba7Sj9VR.js", "./stylus-C-RTeXnz.js", "./swift-Cbprqdc8.js", "./tcl-B2fODqDH.js", "./textile-BuVhTOzU.js", "./tiddlywiki-BgR6AEZu.js", "./tiki-CI-ztowC.js", "./toml-BQXy8elZ.js", "./troff-Ce85hlLp.js", "./ttcn-C4reStyN.js", "./turtle-BkSuIpt-.js", "./vb-coDLL1b7.js", "./vbscript-MdTt_wcJ.js", "./velocity-BdD_26Jv.js", "./verilog-B4LBqg_1.js", "./vhdl-BRDI21CQ.js", "./webidl-CGwyPRYs.js", "./xquery-BZBLoTvf.js", "./yacas-I8QjZlxf.js", "./z80-D8p3gKXp.js", "./ConnectedDataExplorerComponent-B6WI1UcR.js", "./mermaid-BI4dofVe.js"],
     __vite__mapDeps = i => i.map(i => __vite__fileDeps[i]);
 var e = Object.defineProperty,
     t = (t, n, r) => (((t, n, r) => {
         n in t ? e(t, n, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
@@ -20508,17 +20508,17 @@
         let t = null;
         const n = async () => (t || (t = e()), t), r = z.lazy((() => n()));
         return {
             preload: n,
             Component: r
         }
     },
-    I_ = D_((() => ag((() => import("./home-page-BmvI7Tzs.js")), __vite__mapDeps([0, 1, 2]), import.meta.url))),
-    L_ = D_((() => ag((() => import("./run-page-BflrRP7S.js")), __vite__mapDeps([3, 4, 5]), import.meta.url))),
-    V_ = D_((() => ag((() => import("./edit-page-CIzFhPq5.js")), __vite__mapDeps([6, 1, 2, 4, 5, 7, 8, 9, 10, 11, 12]), import.meta.url)));
+    I_ = D_((() => ag((() => import("./home-page-BL9ArKPs.js")), __vite__mapDeps([0, 1, 2]), import.meta.url))),
+    L_ = D_((() => ag((() => import("./run-page-D_UJForb.js")), __vite__mapDeps([3, 4, 5]), import.meta.url))),
+    V_ = D_((() => ag((() => import("./edit-page-DnXnHWMg.js")), __vite__mapDeps([6, 1, 2, 4, 5, 7, 8, 9, 10, 11, 12]), import.meta.url)));
 var Z_;
 "home" === (Z_ = w_) ? I_.preload(): "read" === Z_ ? L_.preload() : V_.preload();
 const q_ = F.memo((() => {
     const [e] = Qp(), [t] = Mp(), n = e.display.code_editor_font_size / 16 + "rem";
     return ee.jsx(W_, {
         children: ee.jsx(Wp, {
             variables: {
@@ -56230,73 +56230,73 @@
 }));
 
 function jue(e) {
     return new $8(H7.define(e))
 }
 
 function Mue(e) {
-    return ag((() => import("./index-ClCDnvOE.js")), [], import.meta.url).then((t => t.sql({
+    return ag((() => import("./index-yuQsQmno.js")), [], import.meta.url).then((t => t.sql({
         dialect: t[e]
     })))
 }
 const Nue = [A8.of({
     name: "C",
     extensions: ["c", "h", "ino"],
-    load: () => ag((() => import("./index-7VEF_U3p.js")), [], import.meta.url).then((e => e.cpp()))
+    load: () => ag((() => import("./index-DgOauLen.js")), [], import.meta.url).then((e => e.cpp()))
 }), A8.of({
     name: "C++",
     alias: ["cpp"],
     extensions: ["cpp", "c++", "cc", "cxx", "hpp", "h++", "hh", "hxx"],
-    load: () => ag((() => import("./index-7VEF_U3p.js")), [], import.meta.url).then((e => e.cpp()))
+    load: () => ag((() => import("./index-DgOauLen.js")), [], import.meta.url).then((e => e.cpp()))
 }), A8.of({
     name: "CQL",
     alias: ["cassandra"],
     extensions: ["cql"],
     load: () => Mue("Cassandra")
 }), A8.of({
     name: "CSS",
     extensions: ["css"],
     load: () => ag((() => Promise.resolve().then((() => Yle))), void 0, import.meta.url).then((e => e.css()))
 }), A8.of({
     name: "Go",
     extensions: ["go"],
-    load: () => ag((() => import("./index-O7K-_bwp.js")), [], import.meta.url).then((e => e.go()))
+    load: () => ag((() => import("./index-wbyGdlc1.js")), [], import.meta.url).then((e => e.go()))
 }), A8.of({
     name: "HTML",
     alias: ["xhtml"],
     extensions: ["html", "htm", "handlebars", "hbs"],
     load: () => ag((() => Promise.resolve().then((() => lue))), void 0, import.meta.url).then((e => e.html()))
 }), A8.of({
     name: "Java",
     extensions: ["java"],
-    load: () => ag((() => import("./index-C2GbrbZr.js")), [], import.meta.url).then((e => e.java()))
+    load: () => ag((() => import("./index-DCESMHe2.js")), [], import.meta.url).then((e => e.java()))
 }), A8.of({
     name: "JavaScript",
     alias: ["ecmascript", "js", "node"],
     extensions: ["js", "mjs", "cjs"],
     load: () => ag((() => Promise.resolve().then((() => Ace))), void 0, import.meta.url).then((e => e.javascript()))
 }), A8.of({
     name: "JSON",
     alias: ["json5"],
     extensions: ["json", "map"],
-    load: () => ag((() => import("./index-S9qVQ2oC.js")), [], import.meta.url).then((e => e.json()))
+    load: () => ag((() => import("./index-DqGPWGPa.js")), [], import.meta.url).then((e => e.json()))
 }), A8.of({
     name: "JSX",
     extensions: ["jsx"],
     load: () => ag((() => Promise.resolve().then((() => Ace))), void 0, import.meta.url).then((e => e.javascript({
         jsx: !0
     })))
 }), A8.of({
     name: "LESS",
     extensions: ["less"],
-    load: () => ag((() => import("./index-DzhIfGoT.js")), [], import.meta.url).then((e => e.less()))
+    load: () => ag((() => import("./index-1IpQZ_Yu.js")), [], import.meta.url).then((e => e.less()))
 }), A8.of({
     name: "Liquid",
     extensions: ["liquid"],
-    load: () => ag((() => import("./index-0fF0Xoai.js")), [], import.meta.url).then((e => e.liquid()))
+    load: () => ag((() => import("./index-BYVYp6Ei.js")), [], import.meta.url).then((e => e.liquid()))
 }), A8.of({
     name: "MariaDB SQL",
     load: () => Mue("MariaSQL")
 }), A8.of({
     name: "Markdown",
     extensions: ["md", "markdown", "mkd"],
     load: () => ag((() => Promise.resolve().then((() => Aue))), void 0, import.meta.url).then((e => e.markdown()))
@@ -56305,15 +56305,15 @@
     load: () => Mue("MSSQL")
 }), A8.of({
     name: "MySQL",
     load: () => Mue("MySQL")
 }), A8.of({
     name: "PHP",
     extensions: ["php", "php3", "php4", "php5", "php7", "phtml"],
-    load: () => ag((() => import("./index-Ck0jzFpb.js")), [], import.meta.url).then((e => e.php()))
+    load: () => ag((() => import("./index-CB4e2-IR.js")), [], import.meta.url).then((e => e.php()))
 }), A8.of({
     name: "PLSQL",
     extensions: ["pls"],
     load: () => Mue("PLSQL")
 }), A8.of({
     name: "PostgreSQL",
     load: () => Mue("PostgreSQL")
@@ -56321,25 +56321,25 @@
     name: "Python",
     extensions: ["BUILD", "bzl", "py", "pyw"],
     filename: /^(BUCK|BUILD)$/,
     load: () => ag((() => Promise.resolve().then((() => Hie))), void 0, import.meta.url).then((e => e.python()))
 }), A8.of({
     name: "Rust",
     extensions: ["rs"],
-    load: () => ag((() => import("./index-BuR6fZZm.js")), [], import.meta.url).then((e => e.rust()))
+    load: () => ag((() => import("./index-CE06HdF7.js")), [], import.meta.url).then((e => e.rust()))
 }), A8.of({
     name: "Sass",
     extensions: ["sass"],
-    load: () => ag((() => import("./index-DgcwnKY7.js")), [], import.meta.url).then((e => e.sass({
+    load: () => ag((() => import("./index-DahJleVt.js")), [], import.meta.url).then((e => e.sass({
         indented: !0
     })))
 }), A8.of({
     name: "SCSS",
     extensions: ["scss"],
-    load: () => ag((() => import("./index-DgcwnKY7.js")), [], import.meta.url).then((e => e.sass()))
+    load: () => ag((() => import("./index-DahJleVt.js")), [], import.meta.url).then((e => e.sass()))
 }), A8.of({
     name: "SQL",
     extensions: ["sql"],
     load: () => Mue("StandardSQL")
 }), A8.of({
     name: "SQLite",
     load: () => Mue("SQLite")
@@ -56356,25 +56356,25 @@
     extensions: ["ts", "mts", "cts"],
     load: () => ag((() => Promise.resolve().then((() => Ace))), void 0, import.meta.url).then((e => e.javascript({
         typescript: !0
     })))
 }), A8.of({
     name: "WebAssembly",
     extensions: ["wat", "wast"],
-    load: () => ag((() => import("./index-jW3n8_hn.js")), [], import.meta.url).then((e => e.wast()))
+    load: () => ag((() => import("./index-BH1DvUFb.js")), [], import.meta.url).then((e => e.wast()))
 }), A8.of({
     name: "XML",
     alias: ["rss", "wsdl", "xsd"],
     extensions: ["xml", "xsl", "xsd", "svg"],
-    load: () => ag((() => import("./index-CohQOVlj.js")), [], import.meta.url).then((e => e.xml()))
+    load: () => ag((() => import("./index-KIzq3vhX.js")), [], import.meta.url).then((e => e.xml()))
 }), A8.of({
     name: "YAML",
     alias: ["yml"],
     extensions: ["yaml", "yml"],
-    load: () => ag((() => import("./index-VNKARDPQ.js")), [], import.meta.url).then((e => e.yaml()))
+    load: () => ag((() => import("./index-rXOiTwQN.js")), [], import.meta.url).then((e => e.yaml()))
 }), A8.of({
     name: "APL",
     extensions: ["dyalog", "apl"],
     load: () => ag((() => import("./apl-CXdQSnD-.js")), [], import.meta.url).then((e => jue(e.apl)))
 }), A8.of({
     name: "PGP",
     alias: ["asciiarmor"],
@@ -56825,18 +56825,18 @@
 }), A8.of({
     name: "MsGenny",
     extensions: ["msgenny"],
     load: () => ag((() => import("./mscgen-B2igx18G.js")), [], import.meta.url).then((e => jue(e.msgenny)))
 }), A8.of({
     name: "Vue",
     extensions: ["vue"],
-    load: () => ag((() => import("./index-CzWuvzvc.js")), [], import.meta.url).then((e => e.vue()))
+    load: () => ag((() => import("./index-DtyNPFfa.js")), [], import.meta.url).then((e => e.vue()))
 }), A8.of({
     name: "Angular Template",
-    load: () => ag((() => import("./index-D4als0Dc.js")), [], import.meta.url).then((e => e.angular()))
+    load: () => ag((() => import("./index-XFgu4285.js")), [], import.meta.url).then((e => e.angular()))
 })];
 var Due = {
     exports: {}
 };
 Due.exports = function() {
     const e = new WeakMap,
         t = /(\n|\r\n?|\u2028|\u2029)/g,
@@ -73378,15 +73378,15 @@
             }, t)))
         }), z.Children.map(r, ((e, t) => ee.jsx(jRe, {
             value: t.toString(),
             children: e
         })))]
     })
 };
-const NRe = z.lazy((() => ag((() => import("./CarouselComponent-DtCAwyzo.js")), __vite__mapDeps([19, 20]), import.meta.url)));
+const NRe = z.lazy((() => ag((() => import("./CarouselComponent-ml4W_PuP.js")), __vite__mapDeps([19, 20]), import.meta.url)));
 const DRe = Yfe((async () => (await ag((() => import("./katex-BnMoLUs3.js")), [], import.meta.url)).default));
 const IRe = ({
     tex: e
 }) => {
     const t = F.useRef(null);
     return F.useLayoutEffect((() => {
         t.current && async function(e, t) {
@@ -74677,15 +74677,15 @@
     return OQe(1e3 * e, {
         language: "shortEn",
         largest: 2,
         spacer: "",
         maxDecimalPoints: 2
     })
 }
-const bQe = z.lazy((() => ag((() => import("./vega-component-CZ4hZbd6.js")), __vite__mapDeps([21, 22, 23, 8, 24, 25, 26, 9, 27, 28, 29, 30, 31, 32]), import.meta.url)));
+const bQe = z.lazy((() => ag((() => import("./vega-component-B9WTop1f.js")), __vite__mapDeps([21, 22, 23, 8, 24, 25, 26, 9, 27, 28, 29, 30, 31, 32]), import.meta.url)));
 const yQe = ({
         value: e,
         label: t,
         caption: n,
         bordered: r,
         direction: o
     }) => ee.jsxs("div", {
@@ -80800,15 +80800,15 @@
     return e != e && t != t
 }
 
 function YDe(e) {
     const t = z.useRef(e);
     return XDe(e, t.current) || (t.current = e), t.current
 }
-const UDe = F.lazy((() => ag((() => import("./react-plotly-Bf9tHX8H.js").then((e => e.r))), [], import.meta.url)));
+const UDe = F.lazy((() => ag((() => import("./react-plotly-C4-ZLKix.js").then((e => e.r))), [], import.meta.url)));
 
 function BDe(e) {
     return {
         autosize: void 0 === e.layout.width,
         dragmode: "select",
         height: 540,
         ...e.layout
@@ -80901,15 +80901,15 @@
     let t;
     return e.map((e => {
         const n = Array.isArray(e.data.hovertemplate) ? e.data.hovertemplate[0] : e.data.hovertemplate;
         return t = t ? t.update(n) : WDe(n), t.parse(e)
     }))
 }
 GDe.displayName = "PlotlyComponent";
-const KDe = F.lazy((() => ag((() => import("./any-language-editor-D3MTmtyo.js")), __vite__mapDeps([33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 13, 14, 60, 61, 62, 63, 64, 65, 66, 15, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 16, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128]), import.meta.url)));
+const KDe = F.lazy((() => ag((() => import("./any-language-editor-Dzf9Jczi.js")), __vite__mapDeps([33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 13, 14, 60, 61, 62, 63, 64, 65, 66, 15, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 16, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128]), import.meta.url)));
 const JDe = e => {
         const {
             theme: t
         } = Zp(), n = e.theme || t, r = e.minHeight ? `${e.minHeight}px` : "70px";
         return ee.jsx(Mme, {
             label: e.label,
             align: "top",
@@ -80922,26 +80922,26 @@
                 editable: !e.disabled,
                 value: e.value,
                 language: e.language,
                 onChange: e.setValue
             })
         })
     },
-    eIe = z.lazy((() => ag((() => import("./ConnectedDataExplorerComponent-DKdMG7z6.js")), __vite__mapDeps([129, 22, 23, 8, 24, 25, 26, 9, 27, 28, 29, 30, 31, 32]), import.meta.url))),
+    eIe = z.lazy((() => ag((() => import("./ConnectedDataExplorerComponent-B6WI1UcR.js")), __vite__mapDeps([129, 22, 23, 8, 24, 25, 26, 9, 27, 28, 29, 30, 31, 32]), import.meta.url))),
     tIe = fwe("marimo-data-explorer").withData(lp.object({
         label: lp.string().nullish(),
         data: lp.string()
     })).renderer((e => ee.jsx(Ty, {
         children: ee.jsx(eIe, {
             ...e.data,
             value: e.value,
             setValue: e.setValue
         })
     })));
-const nIe = F.lazy((() => ag((() => import("./mermaid-BDDPrcgz.js").then((e => e.a7))), __vite__mapDeps([130, 7, 8, 30]), import.meta.url)));
+const nIe = F.lazy((() => ag((() => import("./mermaid-BI4dofVe.js").then((e => e.a7))), __vite__mapDeps([130, 7, 8, 30]), import.meta.url)));
 
 function rIe(e) {
     F.useEffect(e, [])
 }
 const oIe = e => {
         const {
             css: t,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-DzhIfGoT.js` & `marimo-0.6.4/marimo/_static/assets/index-1IpQZ_Yu.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     iW as e,
     iY as S,
     iS as l,
     iT as r,
     jf as t,
     iJ as o,
     iI as i
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const $ = [9, 10, 11, 12, 13, 32, 133, 160, 5760, 8192, 8193, 8194, 8195, 8196, 8197, 8198, 8199, 8200, 8201, 8202, 8232, 8233, 8239, 8287, 12288];
 
 function y(O) {
     return O >= 65 && O <= 90 || O >= 97 && O <= 122 || O >= 161
 }
 const X = new i(((O, T) => {
         if (40 == O.next) {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-O7K-_bwp.js` & `marimo-0.6.4/marimo/_static/assets/index-wbyGdlc1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,15 @@
     iS as r,
     iT as S,
     iQ as T,
     iU as p,
     iV as W,
     jd as V,
     je as m
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const Y = new O(((O, Q) => {
     for (let e = 0, a = O.next;
         (Q.context && (a < 0 || 10 == a || 13 == a || 47 == a && 47 == O.peek(e + 1)) || 41 == a || 125 == a) && O.acceptToken(177), 32 == a || 9 == a;) a = O.peek(++e)
 }), {
     contextual: !0
 });
 let R = new Set([95, 184, 20, 12, 17, 144, 145, 142, 148, 13, 53, 25]);
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-S9qVQ2oC.js` & `marimo-0.6.4/marimo/_static/assets/index-DqGPWGPa.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     iJ as r,
     iQ as a,
     iO as t,
     iW as P,
     iY as s,
     iS as Q,
     iT as o
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const n = O({
         String: e.string,
         Number: e.number,
         "True False": e.bool,
         PropertyName: e.propertyName,
         Null: e.null,
         ",": e.separator,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-VNKARDPQ.js` & `marimo-0.6.4/marimo/_static/assets/index-rXOiTwQN.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     iJ as Q,
     iO as P,
     iW as o,
     iX as r,
     iS as c,
     iT as i,
     iQ as s
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const p = 63,
     f = class {
         constructor(O, e, t) {
             this.parent = O, this.depth = e, this.type = t, this.hash = (O ? O.hash + O.hash << 8 : 0) + e + (e << 4) + t
         }
     };
 var X, l, R;
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-fc10efb0-C3SRzTfT.js` & `marimo-0.6.4/marimo/_static/assets/index-fc10efb0-CJWvKICv.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,44 +1,44 @@
 import {
     i as e,
     G as t
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     m as n,
     l as r
-} from "./layout-DDD1odkP.js";
+} from "./layout-BdT9zkSH.js";
 import {
     c as i
-} from "./clone-BL0WSZ3Z.js";
+} from "./clone-CrCyWe3U.js";
 import {
     i as a,
     u as o,
     s,
     a as d,
     b as c,
     g as l,
     p as h,
     c as g,
     d as f,
     e as u,
     f as w,
     h as p,
     j as v
-} from "./edges-d32062c0-CFY3bIwa.js";
+} from "./edges-d32062c0-CU6OCHwI.js";
 import {
     l as m,
     c as y,
     o as x
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     c as b
-} from "./createText-6b48ae7d-129t9twG.js";
+} from "./createText-6b48ae7d-BgOE7dMp.js";
 import {
     s as E
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 
 function N(t) {
     var n = {
         options: {
             directed: t.isDirected(),
             multigraph: t.isMultigraph(),
             compound: t.isCompound()
```

### Comparing `marimo-0.6.3/marimo/_static/assets/index-jW3n8_hn.js` & `marimo-0.6.4/marimo/_static/assets/index-BH1DvUFb.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     iW as O,
     iX as o,
     iS as r,
     iT as n,
     iN as Q,
     iM as i,
     iJ as t
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 const $ = {
         __proto__: null,
         anyref: 34,
         dataref: 34,
         eqref: 34,
         externref: 34,
         i31ref: 34,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/infoDiagram-bcd20f53-BIy3DJKx.js` & `marimo-0.6.4/marimo/_static/assets/infoDiagram-bcd20f53-CAV4G93w.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     l as t,
     V as i,
     h as n
-} from "./mermaid-BDDPrcgz.js";
-import "./transform-DGMfQOK3.js";
-import "./index-Dq6tg2Hn.js";
+} from "./mermaid-BI4dofVe.js";
+import "./transform-DNjxe6pi.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 var s = function() {
     var t = function(t, i, n, s) {
             for (n = n || {}, s = t.length; s--; n[t[s]] = i);
             return n
         },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/javascript-DY1Qj14w.js` & `marimo-0.6.4/marimo/_static/assets/javascript-DY1Qj14w.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/jinja2-DhgKlfW7.js` & `marimo-0.6.4/marimo/_static/assets/jinja2-DhgKlfW7.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/journeyDiagram-4fe6b3dc-C_g7a5O5.js` & `marimo-0.6.4/marimo/_static/assets/journeyDiagram-4fe6b3dc-DOB96Qnq.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,28 +4,28 @@
     v as n,
     s as i,
     g as s,
     b as r,
     a,
     y as o,
     h as l
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as c
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     d as h,
     f as u,
     a as y,
     g as p
-} from "./svgDrawCommon-5ccd53ef-BK5P1sG2.js";
+} from "./svgDrawCommon-5ccd53ef-DsDJYju_.js";
 import {
     a as d
 } from "./arc-DIImc9ZO.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 import "./path-qnb_ma6O.js";
 var f = function() {
     var t = function(t, e, n, i) {
             for (n = n || {}, i = t.length; i--; n[t[i]] = e);
             return n
```

### Comparing `marimo-0.6.3/marimo/_static/assets/julia-DjdwvFuI.js` & `marimo-0.6.4/marimo/_static/assets/julia-DjdwvFuI.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/katex-BnMoLUs3.js` & `marimo-0.6.4/marimo/_static/assets/katex-BnMoLUs3.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/layout-DDD1odkP.js` & `marimo-0.6.4/marimo/_static/assets/layout-BdT9zkSH.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
     f as t,
     G as o,
     h as i,
     i as u,
     d as a,
     v as d,
     r as c
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     is as f,
     ik as s,
     jo as h,
     j_ as g,
     iv as v,
     ji as l,
@@ -22,38 +22,38 @@
     jj as w,
     j$ as b,
     jp as y,
     k0 as k,
     k1 as x,
     ii as E,
     k2 as N
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     c as _,
     a as I,
     d as R,
     e as M
-} from "./_baseEach-BrSWFoJM.js";
+} from "./_baseEach-FAhoh2N5.js";
 import {
     b as T,
     s as L
-} from "./sortBy-D0xI_7yL.js";
+} from "./sortBy-DwX0cqqB.js";
 import {
     h as j,
     o as C,
     b as P,
     c as S,
     d as O,
     e as G,
     f as V
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     A as B,
     L as F
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 
 function Y(n) {
     return (null == n ? 0 : n.length) ? _(n, 1) : []
 }
 var q = 1,
     z = 4;
 var A = Object.prototype,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/line-Dz7yhIWK.js` & `marimo-0.6.4/marimo/_static/assets/line-Dz7yhIWK.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/linear-DF6Se9n2.js` & `marimo-0.6.4/marimo/_static/assets/linear-JxYcrfvc.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     jK as c,
     jL as s,
     jM as l,
     jN as h,
     h0 as m,
     g_ as p,
     jO as g
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     i as v
 } from "./init-DLRA0X12.js";
 
 function y(n) {
     return null === n ? NaN : +n
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/livescript-B19OIWEP.js` & `marimo-0.6.4/marimo/_static/assets/livescript-B19OIWEP.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/lua-8DXOpKDz.js` & `marimo-0.6.4/marimo/_static/assets/lua-8DXOpKDz.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/mathematica-IIbmv7SK.js` & `marimo-0.6.4/marimo/_static/assets/mathematica-IIbmv7SK.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/mbox-DoeuZPxA.js` & `marimo-0.6.4/marimo/_static/assets/mbox-DoeuZPxA.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/mermaid-BDDPrcgz.js` & `marimo-0.6.4/marimo/_static/assets/mermaid-BI4dofVe.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-const __vite__fileDeps = ["./c4Diagram-b2a90758-CAH0Datt.js", "./transform-DGMfQOK3.js", "./index-Dq6tg2Hn.js", "./index-CC7Qmxzq.css", "./timer-D8GWrtRJ.js", "./svgDrawCommon-5ccd53ef-BK5P1sG2.js", "./step-BEJ6WznM.js", "./flowDiagram-5540d9b9-msf8H4Jk.js", "./flowDb-4b19a42f-4mXsCvSf.js", "./graph-SHnEHiLi.js", "./_baseEach-BrSWFoJM.js", "./layout-DDD1odkP.js", "./sortBy-D0xI_7yL.js", "./styles-3ed67cfa-QdZmR4us.js", "./index-fc10efb0-C3SRzTfT.js", "./clone-BL0WSZ3Z.js", "./edges-d32062c0-CFY3bIwa.js", "./createText-6b48ae7d-129t9twG.js", "./line-Dz7yhIWK.js", "./array-DmjLdZ15.js", "./path-qnb_ma6O.js", "./channel-DCiFYtzP.js", "./flowDiagram-v2-3b53844e-BRBAHwua.js", "./erDiagram-47591fe2-CJ2SMwAy.js", "./gitGraphDiagram-96e6b4ee-BUgJQeEj.js", "./ganttDiagram-9a3bba1f-Clnqsx9q.js", "./time-CUBsQdfc.js", "./linear-DF6Se9n2.js", "./init-DLRA0X12.js", "./infoDiagram-bcd20f53-BIy3DJKx.js", "./pieDiagram-79897490-DVu-KYPX.js", "./arc-DIImc9ZO.js", "./ordinal-DDUp3AbE.js", "./quadrantDiagram-62f64e94-CU-4FuJa.js", "./xychartDiagram-ab372869-DViGpnfl.js", "./range-CtcPcB_L.js", "./requirementDiagram-05bf5f74-BsI08XXR.js", "./sequenceDiagram-acc0e65c-Dsgiz64s.js", "./classDiagram-30eddba6-Bz0cJX-U.js", "./styles-991ebdfc-CV9pCNxb.js", "./classDiagram-v2-f2df5561-BxNEwu6g.js", "./stateDiagram-0ff1cf1a-lr9-t8r1.js", "./styles-d20c7d72-BOwpCRGP.js", "./stateDiagram-v2-9a9d610d-DwjKCx-9.js", "./journeyDiagram-4fe6b3dc-C_g7a5O5.js", "./flowchart-elk-definition-5fe447d6-tgRhUdQk.js", "./timeline-definition-fea2a41d-B6Whk07l.js", "./mindmap-definition-f354de21-BT0462Yo.js", "./sankeyDiagram-97764748-BQdZQP_-.js", "./Tableau10-B3EzvwxR.js", "./blockDiagram-91b80b7a-DPH13Qrf.js"],
+const __vite__fileDeps = ["./c4Diagram-b2a90758-f1UFjA-x.js", "./transform-DNjxe6pi.js", "./index-Cd3MtTMQ.js", "./index-CC7Qmxzq.css", "./timer-D8GWrtRJ.js", "./svgDrawCommon-5ccd53ef-DsDJYju_.js", "./step-BEJ6WznM.js", "./flowDiagram-5540d9b9-CuVcDbrT.js", "./flowDb-4b19a42f-Cf4l3Vi7.js", "./graph-Dl9Z7r13.js", "./_baseEach-FAhoh2N5.js", "./layout-BdT9zkSH.js", "./sortBy-DwX0cqqB.js", "./styles-3ed67cfa-Cg_XeDUz.js", "./index-fc10efb0-CJWvKICv.js", "./clone-CrCyWe3U.js", "./edges-d32062c0-CU6OCHwI.js", "./createText-6b48ae7d-BgOE7dMp.js", "./line-Dz7yhIWK.js", "./array-DmjLdZ15.js", "./path-qnb_ma6O.js", "./channel-BmGrl1HB.js", "./flowDiagram-v2-3b53844e-By9U58mT.js", "./erDiagram-47591fe2-UyJH0JYd.js", "./gitGraphDiagram-96e6b4ee-BKc9lhir.js", "./ganttDiagram-9a3bba1f-W6mmWQNE.js", "./time-CLRyKR-T.js", "./linear-JxYcrfvc.js", "./init-DLRA0X12.js", "./infoDiagram-bcd20f53-CAV4G93w.js", "./pieDiagram-79897490-DznITiVM.js", "./arc-DIImc9ZO.js", "./ordinal-DDUp3AbE.js", "./quadrantDiagram-62f64e94-Df4mAWqb.js", "./xychartDiagram-ab372869-1vV9tLRe.js", "./range-CtcPcB_L.js", "./requirementDiagram-05bf5f74-DyUtzGOy.js", "./sequenceDiagram-acc0e65c-DquwX6r9.js", "./classDiagram-30eddba6-BabWtcIB.js", "./styles-991ebdfc-vxk4XA-a.js", "./classDiagram-v2-f2df5561-D5SEk3xC.js", "./stateDiagram-0ff1cf1a-DjUkVeHK.js", "./styles-d20c7d72-DtCcJufV.js", "./stateDiagram-v2-9a9d610d-C6LzE_mY.js", "./journeyDiagram-4fe6b3dc-DOB96Qnq.js", "./flowchart-elk-definition-5fe447d6-BpUsl4Jm.js", "./timeline-definition-fea2a41d-DQvyLJzo.js", "./mindmap-definition-f354de21-CQ2IslvL.js", "./sankeyDiagram-97764748-DvvFNiJT.js", "./Tableau10-B3EzvwxR.js", "./blockDiagram-91b80b7a-DSsN5jAx.js"],
     __vite__mapDeps = i => i.map(i => __vite__fileDeps[i]);
 import {
     ig as t,
     ih as e,
     ii as i,
     ij as r,
     ik as o,
@@ -29,21 +29,21 @@
     iE as v,
     iF as F,
     r as _,
     aE as L,
     u as A,
     j as w,
     Y as E
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     b as M,
     c as O,
     d as I,
     s as q
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     a as D,
     b as z,
     d as R,
     e as N,
     h as $,
     g as P,
@@ -3561,15 +3561,15 @@
     },
     qr = {
         id: "c4",
         detector: t => /^\s*C4Context|C4Container|C4Component|C4Dynamic|C4Deployment/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./c4Diagram-b2a90758-CAH0Datt.js")), __vite__mapDeps([0, 1, 2, 3, 4, 5, 6]), import.meta.url);
+            } = await F((() => import("./c4Diagram-b2a90758-f1UFjA-x.js")), __vite__mapDeps([0, 1, 2, 3, 4, 5, 6]), import.meta.url);
             return {
                 id: "c4",
                 diagram: t
             }
         }
     },
     Dr = "flowchart",
@@ -3578,15 +3578,15 @@
         detector: (t, e) => {
             var i, r;
             return "dagre-wrapper" !== (null == (i = null == e ? void 0 : e.flowchart) ? void 0 : i.defaultRenderer) && "elk" !== (null == (r = null == e ? void 0 : e.flowchart) ? void 0 : r.defaultRenderer) && /^\s*graph/.test(t)
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./flowDiagram-5540d9b9-msf8H4Jk.js")), __vite__mapDeps([7, 8, 1, 2, 3, 4, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 6, 21]), import.meta.url);
+            } = await F((() => import("./flowDiagram-5540d9b9-CuVcDbrT.js")), __vite__mapDeps([7, 8, 1, 2, 3, 4, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 6, 21]), import.meta.url);
             return {
                 id: Dr,
                 diagram: t
             }
         }
     },
     Rr = "flowchart-v2",
@@ -3595,139 +3595,139 @@
         detector: (t, e) => {
             var i, r, o;
             return "dagre-d3" !== (null == (i = null == e ? void 0 : e.flowchart) ? void 0 : i.defaultRenderer) && "elk" !== (null == (r = null == e ? void 0 : e.flowchart) ? void 0 : r.defaultRenderer) && (!(!/^\s*graph/.test(t) || "dagre-wrapper" !== (null == (o = null == e ? void 0 : e.flowchart) ? void 0 : o.defaultRenderer)) || /^\s*flowchart/.test(t))
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./flowDiagram-v2-3b53844e-BRBAHwua.js")), __vite__mapDeps([22, 8, 1, 2, 3, 4, 13, 9, 10, 14, 11, 12, 15, 16, 17, 18, 19, 20, 6, 21]), import.meta.url);
+            } = await F((() => import("./flowDiagram-v2-3b53844e-By9U58mT.js")), __vite__mapDeps([22, 8, 1, 2, 3, 4, 13, 9, 10, 14, 11, 12, 15, 16, 17, 18, 19, 20, 6, 21]), import.meta.url);
             return {
                 id: Rr,
                 diagram: t
             }
         }
     },
     $r = {
         id: "er",
         detector: t => /^\s*erDiagram/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./erDiagram-47591fe2-CJ2SMwAy.js")), __vite__mapDeps([23, 9, 2, 3, 10, 1, 4, 11, 12, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./erDiagram-47591fe2-UyJH0JYd.js")), __vite__mapDeps([23, 9, 2, 3, 10, 1, 4, 11, 12, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: "er",
                 diagram: t
             }
         }
     },
     Pr = "gitGraph",
     Wr = {
         id: Pr,
         detector: t => /^\s*gitGraph/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./gitGraphDiagram-96e6b4ee-BUgJQeEj.js")), __vite__mapDeps([24, 1, 2, 3, 4, 6]), import.meta.url);
+            } = await F((() => import("./gitGraphDiagram-96e6b4ee-BKc9lhir.js")), __vite__mapDeps([24, 1, 2, 3, 4, 6]), import.meta.url);
             return {
                 id: Pr,
                 diagram: t
             }
         }
     },
     jr = "gantt",
     Hr = {
         id: jr,
         detector: t => /^\s*gantt/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./ganttDiagram-9a3bba1f-Clnqsx9q.js")), __vite__mapDeps([25, 2, 3, 1, 4, 26, 27, 28, 6]), import.meta.url);
+            } = await F((() => import("./ganttDiagram-9a3bba1f-W6mmWQNE.js")), __vite__mapDeps([25, 2, 3, 1, 4, 26, 27, 28, 6]), import.meta.url);
             return {
                 id: jr,
                 diagram: t
             }
         }
     },
     Ur = "info",
     Yr = {
         id: Ur,
         detector: t => /^\s*info/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./infoDiagram-bcd20f53-BIy3DJKx.js")), __vite__mapDeps([29, 1, 2, 3, 4, 6]), import.meta.url);
+            } = await F((() => import("./infoDiagram-bcd20f53-CAV4G93w.js")), __vite__mapDeps([29, 1, 2, 3, 4, 6]), import.meta.url);
             return {
                 id: Ur,
                 diagram: t
             }
         }
     },
     Vr = {
         id: "pie",
         detector: t => /^\s*pie/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./pieDiagram-79897490-DVu-KYPX.js")), __vite__mapDeps([30, 1, 2, 3, 4, 31, 20, 6, 32, 28, 19]), import.meta.url);
+            } = await F((() => import("./pieDiagram-79897490-DznITiVM.js")), __vite__mapDeps([30, 1, 2, 3, 4, 31, 20, 6, 32, 28, 19]), import.meta.url);
             return {
                 id: "pie",
                 diagram: t
             }
         }
     },
     Gr = "quadrantChart",
     Xr = {
         id: Gr,
         detector: t => /^\s*quadrantChart/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./quadrantDiagram-62f64e94-CU-4FuJa.js")), __vite__mapDeps([33, 1, 2, 3, 4, 27, 28, 6]), import.meta.url);
+            } = await F((() => import("./quadrantDiagram-62f64e94-Df4mAWqb.js")), __vite__mapDeps([33, 1, 2, 3, 4, 27, 28, 6]), import.meta.url);
             return {
                 id: Gr,
                 diagram: t
             }
         }
     },
     Zr = "xychart",
     Kr = {
         id: Zr,
         detector: t => /^\s*xychart-beta/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./xychartDiagram-ab372869-DViGpnfl.js")), __vite__mapDeps([34, 17, 1, 2, 3, 4, 28, 32, 35, 27, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./xychartDiagram-ab372869-1vV9tLRe.js")), __vite__mapDeps([34, 17, 1, 2, 3, 4, 28, 32, 35, 27, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: Zr,
                 diagram: t
             }
         }
     },
     Jr = "requirement",
     Qr = {
         id: Jr,
         detector: t => /^\s*requirement(Diagram)?/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./requirementDiagram-05bf5f74-BsI08XXR.js")), __vite__mapDeps([36, 1, 2, 3, 4, 9, 10, 11, 12, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./requirementDiagram-05bf5f74-DyUtzGOy.js")), __vite__mapDeps([36, 1, 2, 3, 4, 9, 10, 11, 12, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: Jr,
                 diagram: t
             }
         }
     },
     to = "sequence",
     eo = {
         id: to,
         detector: t => /^\s*sequenceDiagram/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./sequenceDiagram-acc0e65c-Dsgiz64s.js")), __vite__mapDeps([37, 1, 2, 3, 4, 5, 6]), import.meta.url);
+            } = await F((() => import("./sequenceDiagram-acc0e65c-DquwX6r9.js")), __vite__mapDeps([37, 1, 2, 3, 4, 5, 6]), import.meta.url);
             return {
                 id: to,
                 diagram: t
             }
         }
     },
     io = "class",
@@ -3736,15 +3736,15 @@
         detector: (t, e) => {
             var i;
             return "dagre-wrapper" !== (null == (i = null == e ? void 0 : e.class) ? void 0 : i.defaultRenderer) && /^\s*classDiagram/.test(t)
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./classDiagram-30eddba6-Bz0cJX-U.js")), __vite__mapDeps([38, 39, 1, 2, 3, 4, 9, 10, 11, 12, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./classDiagram-30eddba6-BabWtcIB.js")), __vite__mapDeps([38, 39, 1, 2, 3, 4, 9, 10, 11, 12, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: io,
                 diagram: t
             }
         }
     },
     oo = "classDiagram",
@@ -3753,15 +3753,15 @@
         detector: (t, e) => {
             var i;
             return !(!/^\s*classDiagram/.test(t) || "dagre-wrapper" !== (null == (i = null == e ? void 0 : e.class) ? void 0 : i.defaultRenderer)) || /^\s*classDiagram-v2/.test(t)
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./classDiagram-v2-f2df5561-BxNEwu6g.js")), __vite__mapDeps([40, 39, 1, 2, 3, 4, 9, 10, 14, 11, 12, 15, 16, 17, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./classDiagram-v2-f2df5561-D5SEk3xC.js")), __vite__mapDeps([40, 39, 1, 2, 3, 4, 9, 10, 14, 11, 12, 15, 16, 17, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: oo,
                 diagram: t
             }
         }
     },
     no = "state",
@@ -3770,15 +3770,15 @@
         detector: (t, e) => {
             var i;
             return "dagre-wrapper" !== (null == (i = null == e ? void 0 : e.state) ? void 0 : i.defaultRenderer) && /^\s*stateDiagram/.test(t)
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./stateDiagram-0ff1cf1a-lr9-t8r1.js")), __vite__mapDeps([41, 42, 1, 2, 3, 4, 9, 10, 11, 12, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./stateDiagram-0ff1cf1a-DjUkVeHK.js")), __vite__mapDeps([41, 42, 1, 2, 3, 4, 9, 10, 11, 12, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: no,
                 diagram: t
             }
         }
     },
     lo = "stateDiagram",
@@ -3787,29 +3787,29 @@
         detector: (t, e) => {
             var i;
             return !!/^\s*stateDiagram-v2/.test(t) || !(!/^\s*stateDiagram/.test(t) || "dagre-wrapper" !== (null == (i = null == e ? void 0 : e.state) ? void 0 : i.defaultRenderer))
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./stateDiagram-v2-9a9d610d-DwjKCx-9.js")), __vite__mapDeps([43, 42, 9, 2, 3, 10, 1, 4, 14, 11, 12, 15, 16, 17, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./stateDiagram-v2-9a9d610d-C6LzE_mY.js")), __vite__mapDeps([43, 42, 9, 2, 3, 10, 1, 4, 14, 11, 12, 15, 16, 17, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: lo,
                 diagram: t
             }
         }
     },
     co = "journey",
     uo = {
         id: co,
         detector: t => /^\s*journey/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./journeyDiagram-4fe6b3dc-C_g7a5O5.js")), __vite__mapDeps([44, 1, 2, 3, 4, 5, 31, 20, 6]), import.meta.url);
+            } = await F((() => import("./journeyDiagram-4fe6b3dc-DOB96Qnq.js")), __vite__mapDeps([44, 1, 2, 3, 4, 5, 31, 20, 6]), import.meta.url);
             return {
                 id: co,
                 diagram: t
             }
         }
     },
     po = function(t, e, i, r) {
@@ -3927,71 +3927,71 @@
         detector: (t, e) => {
             var i;
             return !!(/^\s*flowchart-elk/.test(t) || /^\s*flowchart|graph/.test(t) && "elk" === (null == (i = null == e ? void 0 : e.flowchart) ? void 0 : i.defaultRenderer))
         },
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./flowchart-elk-definition-5fe447d6-tgRhUdQk.js")), __vite__mapDeps([45, 8, 1, 2, 3, 4, 16, 17, 18, 19, 20, 6]), import.meta.url);
+            } = await F((() => import("./flowchart-elk-definition-5fe447d6-BpUsl4Jm.js")), __vite__mapDeps([45, 8, 1, 2, 3, 4, 16, 17, 18, 19, 20, 6]), import.meta.url);
             return {
                 id: Ho,
                 diagram: t
             }
         }
     },
     Yo = "timeline",
     Vo = {
         id: Yo,
         detector: t => /^\s*timeline/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./timeline-definition-fea2a41d-B6Whk07l.js")), __vite__mapDeps([46, 1, 2, 3, 4, 31, 20, 6]), import.meta.url);
+            } = await F((() => import("./timeline-definition-fea2a41d-DQvyLJzo.js")), __vite__mapDeps([46, 1, 2, 3, 4, 31, 20, 6]), import.meta.url);
             return {
                 id: Yo,
                 diagram: t
             }
         }
     },
     Go = "mindmap",
     Xo = {
         id: Go,
         detector: t => /^\s*mindmap/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./mindmap-definition-f354de21-BT0462Yo.js")), __vite__mapDeps([47, 2, 3, 1, 4, 17, 6]), import.meta.url);
+            } = await F((() => import("./mindmap-definition-f354de21-CQ2IslvL.js")), __vite__mapDeps([47, 2, 3, 1, 4, 17, 6]), import.meta.url);
             return {
                 id: Go,
                 diagram: t
             }
         }
     },
     Zo = "sankey",
     Ko = {
         id: Zo,
         detector: t => /^\s*sankey-beta/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./sankeyDiagram-97764748-BQdZQP_-.js")), __vite__mapDeps([48, 1, 2, 3, 4, 32, 28, 49, 6]), import.meta.url);
+            } = await F((() => import("./sankeyDiagram-97764748-DvvFNiJT.js")), __vite__mapDeps([48, 1, 2, 3, 4, 32, 28, 49, 6]), import.meta.url);
             return {
                 id: Zo,
                 diagram: t
             }
         }
     },
     Jo = "block",
     Qo = {
         id: Jo,
         detector: t => /^\s*block-beta/.test(t),
         loader: async () => {
             const {
                 diagram: t
-            } = await F((() => import("./blockDiagram-91b80b7a-DPH13Qrf.js")), __vite__mapDeps([50, 15, 9, 2, 3, 10, 1, 4, 16, 17, 18, 19, 20, 6, 32, 28, 21, 49]), import.meta.url);
+            } = await F((() => import("./blockDiagram-91b80b7a-DSsN5jAx.js")), __vite__mapDeps([50, 15, 9, 2, 3, 10, 1, 4, 16, 17, 18, 19, 20, 6, 32, 28, 21, 49]), import.meta.url);
             return {
                 id: Jo,
                 diagram: t
             }
         }
     };
 let ta = !1;
```

### Comparing `marimo-0.6.3/marimo/_static/assets/mindmap-definition-f354de21-BT0462Yo.js` & `marimo-0.6.4/marimo/_static/assets/mindmap-definition-f354de21-CQ2IslvL.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,25 +5,25 @@
     q as r,
     W as i,
     d as a,
     a4 as o,
     a5 as s,
     a6 as l,
     Y as u
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     fm as c,
     gd as h
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     s as d
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     c as p
-} from "./createText-6b48ae7d-129t9twG.js";
+} from "./createText-6b48ae7d-BgOE7dMp.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 var g = function(e) {
         var t = typeof e;
         return null != e && ("object" == t || "function" == t)
     },
     f = "object" == typeof c && c && c.Object === Object && c,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/mirc-DkvFAiy5.js` & `marimo-0.6.4/marimo/_static/assets/mirc-DkvFAiy5.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/mllike-B8DYu8SS.js` & `marimo-0.6.4/marimo/_static/assets/mllike-B8DYu8SS.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/modelica-DSrSSXCg.js` & `marimo-0.6.4/marimo/_static/assets/modelica-DSrSSXCg.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/mscgen-B2igx18G.js` & `marimo-0.6.4/marimo/_static/assets/mscgen-B2igx18G.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/mumps-zvxmGV4l.js` & `marimo-0.6.4/marimo/_static/assets/mumps-zvxmGV4l.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/nginx-B4hAVlXN.js` & `marimo-0.6.4/marimo/_static/assets/nginx-B4hAVlXN.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/noise-60BoTA8O.png` & `marimo-0.6.4/marimo/_static/assets/noise-60BoTA8O.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/nsis-Csd3_MSv.js` & `marimo-0.6.4/marimo/_static/assets/nsis-Csd3_MSv.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ntriples-FFvkTduk.js` & `marimo-0.6.4/marimo/_static/assets/ntriples-FFvkTduk.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/octave-C4hdQ5Hf.js` & `marimo-0.6.4/marimo/_static/assets/octave-C4hdQ5Hf.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ordinal-DDUp3AbE.js` & `marimo-0.6.4/marimo/_static/assets/ordinal-DDUp3AbE.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/oz-qQq7irPq.js` & `marimo-0.6.4/marimo/_static/assets/oz-qQq7irPq.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/pascal-CZ0JYm71.js` & `marimo-0.6.4/marimo/_static/assets/pascal-CZ0JYm71.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/path-qnb_ma6O.js` & `marimo-0.6.4/marimo/_static/assets/path-qnb_ma6O.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/perl-tdMlh9QA.js` & `marimo-0.6.4/marimo/_static/assets/perl-tdMlh9QA.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/pieDiagram-79897490-DVu-KYPX.js` & `marimo-0.6.4/marimo/_static/assets/pieDiagram-79897490-DznITiVM.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -10,16 +10,16 @@
     d as o,
     c,
     l as h,
     X as u,
     V as y,
     Y as p,
     h as f
-} from "./mermaid-BDDPrcgz.js";
-import "./transform-DGMfQOK3.js";
+} from "./mermaid-BI4dofVe.js";
+import "./transform-DNjxe6pi.js";
 import {
     a as g
 } from "./arc-DIImc9ZO.js";
 import {
     o as d
 } from "./ordinal-DDUp3AbE.js";
 import {
@@ -27,15 +27,15 @@
 } from "./array-DmjLdZ15.js";
 import {
     c as _
 } from "./path-qnb_ma6O.js";
 import {
     t as x
 } from "./step-BEJ6WznM.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./timer-D8GWrtRJ.js";
 import "./init-DLRA0X12.js";
 
 function b(t, e) {
     return e < t ? -1 : e > t ? 1 : e >= t ? 0 : NaN
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/pig-CwGJVRC4.js` & `marimo-0.6.4/marimo/_static/assets/pig-CwGJVRC4.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/powershell-D1ly3AHC.js` & `marimo-0.6.4/marimo/_static/assets/powershell-D1ly3AHC.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/properties-_nPj978X.js` & `marimo-0.6.4/marimo/_static/assets/properties-_nPj978X.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/protobuf-B4y9do6W.js` & `marimo-0.6.4/marimo/_static/assets/protobuf-B4y9do6W.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/pug-BNyZbGOm.js` & `marimo-0.6.4/marimo/_static/assets/pug-BNyZbGOm.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/puppet-Bc-yJKzi.js` & `marimo-0.6.4/marimo/_static/assets/puppet-Bc-yJKzi.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/python-DD-Q2bae.js` & `marimo-0.6.4/marimo/_static/assets/python-DD-Q2bae.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/q-B0kTJ4cI.js` & `marimo-0.6.4/marimo/_static/assets/q-B0kTJ4cI.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/quadrantDiagram-62f64e94-CU-4FuJa.js` & `marimo-0.6.4/marimo/_static/assets/quadrantDiagram-62f64e94-Df4mAWqb.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -8,22 +8,22 @@
     u as s,
     v as o,
     a as l,
     b as h,
     y as c,
     h as d,
     d as u
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as x
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     k as g
-} from "./linear-DF6Se9n2.js";
-import "./index-Dq6tg2Hn.js";
+} from "./linear-JxYcrfvc.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 import "./init-DLRA0X12.js";
 var f = function() {
     var t = function(t, i, e, a) {
             for (e = e || {}, a = t.length; a--; e[t[a]] = i);
             return e
```

### Comparing `marimo-0.6.3/marimo/_static/assets/r-BA4EbLKE.js` & `marimo-0.6.4/marimo/_static/assets/r-BA4EbLKE.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/react-plotly-Bf9tHX8H.js` & `marimo-0.6.4/marimo/_static/assets/react-plotly-C4-ZLKix.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     r as t,
     fz as e,
     gd as r
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 
 function n(t, e) {
     for (var r = 0; r < e.length; r++) {
         const n = e[r];
         if ("string" != typeof n && !Array.isArray(n))
             for (const e in n)
                 if ("default" !== e && !(e in t)) {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/requirementDiagram-05bf5f74-BsI08XXR.js` & `marimo-0.6.4/marimo/_static/assets/requirementDiagram-05bf5f74-DyUtzGOy.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,32 +4,32 @@
     g as i,
     b as n,
     a as r,
     l as s,
     y as a,
     h as o,
     i as l
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as c
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     G as h
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     l as u
-} from "./layout-DDD1odkP.js";
+} from "./layout-BdT9zkSH.js";
 import {
     l as y
 } from "./line-Dz7yhIWK.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
-import "./_baseEach-BrSWFoJM.js";
-import "./sortBy-D0xI_7yL.js";
+import "./_baseEach-FAhoh2N5.js";
+import "./sortBy-DwX0cqqB.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 var d = function() {
     var t = function(t, e, i, n) {
             for (i = i || {}, n = t.length; n--; i[t[n]] = e);
             return i
         },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/rpm-DI_rRufH.js` & `marimo-0.6.4/marimo/_static/assets/rpm-DI_rRufH.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ruby-CR-u2WLS.js` & `marimo-0.6.4/marimo/_static/assets/ruby-CR-u2WLS.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/run-page-BflrRP7S.js` & `marimo-0.6.4/marimo/_static/assets/run-page-D_UJForb.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17,22 +17,22 @@
     E as p,
     F as j,
     G as u,
     t as y,
     H as f,
     I as k,
     J as g
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     R as w,
     u as v,
     A as N,
     a as C,
     C as I
-} from "./useMarimoWebSocket-DFV8TeGX.js";
+} from "./useMarimoWebSocket-Butgv0ej.js";
 const T = ({
         appConfig: r
     }) => {
         const {
             setCells: l
         } = e();
         s.useEffect((() => (w.INSTANCE.start(t), () => {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/sankeyDiagram-97764748-BQdZQP_-.js` & `marimo-0.6.4/marimo/_static/assets/sankeyDiagram-97764748-DvvFNiJT.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,25 +6,25 @@
     b as s,
     v as r,
     u as o,
     y as l,
     i as c,
     t as a,
     q as h
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as u
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     o as f
 } from "./ordinal-DDUp3AbE.js";
 import {
     s as y
 } from "./Tableau10-B3EzvwxR.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 import "./init-DLRA0X12.js";
 
 function d(t, n) {
     return t < n ? -1 : t > n ? 1 : t >= n ? 0 : NaN
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/sas-Bqaci40L.js` & `marimo-0.6.4/marimo/_static/assets/sas-Bqaci40L.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/save-worker-f86VBHv4.js` & `marimo-0.6.4/marimo/_static/assets/save-worker-f86VBHv4.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/scheme-qjP0V5Ag.js` & `marimo-0.6.4/marimo/_static/assets/scheme-qjP0V5Ag.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/sequenceDiagram-acc0e65c-Dsgiz64s.js` & `marimo-0.6.4/marimo/_static/assets/sequenceDiagram-acc0e65c-DquwX6r9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -16,27 +16,27 @@
     $ as u,
     a0 as x,
     k as y,
     r as m,
     _ as b,
     Y as f,
     a1 as T
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as E
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     d as w,
     a as P,
     g as _,
     b as L,
     c as v,
     e as k
-} from "./svgDrawCommon-5ccd53ef-BK5P1sG2.js";
-import "./index-Dq6tg2Hn.js";
+} from "./svgDrawCommon-5ccd53ef-DsDJYju_.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 var I = function() {
     var t = function(t, e, a, r) {
             for (a = a || {}, r = t.length; r--; a[t[r]] = e);
             return a
         },
```

### Comparing `marimo-0.6.3/marimo/_static/assets/shell-BLav31RL.js` & `marimo-0.6.4/marimo/_static/assets/shell-BLav31RL.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/sieve-r025o_jW.js` & `marimo-0.6.4/marimo/_static/assets/sieve-r025o_jW.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/simple-mode-Ckv7_vD8.js` & `marimo-0.6.4/marimo/_static/assets/simple-mode-Ckv7_vD8.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/smalltalk-C7J3IyEP.js` & `marimo-0.6.4/marimo/_static/assets/smalltalk-C7J3IyEP.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/solr-78MBEUkU.js` & `marimo-0.6.4/marimo/_static/assets/solr-78MBEUkU.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/sortBy-D0xI_7yL.js` & `marimo-0.6.4/marimo/_static/assets/sortBy-DwX0cqqB.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 import {
     b as r,
     a as n,
     c as t
-} from "./_baseEach-BrSWFoJM.js";
+} from "./_baseEach-FAhoh2N5.js";
 import {
     ik as e,
     jh as i,
     ji as a,
     iv as u,
     jj as o,
     jk as f
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     e as s,
     b as c,
     c as l
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 
 function v(n, t) {
     var i = -1,
         a = e(n) ? Array(n.length) : [];
     return r(n, (function(r, n, e) {
         a[++i] = t(r, n, e)
     })), a
```

### Comparing `marimo-0.6.3/marimo/_static/assets/sparql-BRLJFz69.js` & `marimo-0.6.4/marimo/_static/assets/sparql-BRLJFz69.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/spreadsheet-CGlWr0eM.js` & `marimo-0.6.4/marimo/_static/assets/spreadsheet-CGlWr0eM.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/sql-BP5jFf-w.js` & `marimo-0.6.4/marimo/_static/assets/sql-BP5jFf-w.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/stateDiagram-0ff1cf1a-lr9-t8r1.js` & `marimo-0.6.4/marimo/_static/assets/stateDiagram-0ff1cf1a-DjUkVeHK.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
 import {
     p as t,
     d as e,
     s as a
-} from "./styles-d20c7d72-BOwpCRGP.js";
+} from "./styles-d20c7d72-DtCcJufV.js";
 import {
     s as i
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     G as r
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     l as n
-} from "./layout-DDD1odkP.js";
+} from "./layout-BdT9zkSH.js";
 import {
     c as s,
     l as d,
     h as o,
     i as g,
     x as p
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     l as h
 } from "./line-Dz7yhIWK.js";
 import {
     a as c
 } from "./step-BEJ6WznM.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./timer-D8GWrtRJ.js";
-import "./_baseEach-BrSWFoJM.js";
-import "./sortBy-D0xI_7yL.js";
+import "./_baseEach-FAhoh2N5.js";
+import "./sortBy-DwX0cqqB.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 const l = (t, e) => {
         const a = t.append("text").attr("x", 2 * s().state.padding).attr("y", s().state.textHeight + 1.3 * s().state.padding).attr("font-size", s().state.fontSize).attr("class", "state-title").text(e.descriptions[0]).node().getBBox(),
             i = a.height,
             r = t.append("text").attr("x", s().state.padding).attr("y", i + .4 * s().state.padding + s().state.dividerMargin + s().state.textHeight).attr("class", "state-description");
         let n = !0,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/stateDiagram-v2-9a9d610d-DwjKCx-9.js` & `marimo-0.6.4/marimo/_static/assets/stateDiagram-v2-9a9d610d-C6LzE_mY.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,43 +3,43 @@
     d as t,
     s,
     D as o,
     a as r,
     S as a,
     b as i,
     c as n
-} from "./styles-d20c7d72-BOwpCRGP.js";
+} from "./styles-d20c7d72-DtCcJufV.js";
 import {
     G as d
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     s as c
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     l,
     c as p,
     x as b,
     h as g,
     i as h
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     r as m
-} from "./index-fc10efb0-C3SRzTfT.js";
-import "./layout-DDD1odkP.js";
-import "./index-Dq6tg2Hn.js";
-import "./_baseEach-BrSWFoJM.js";
+} from "./index-fc10efb0-CJWvKICv.js";
+import "./layout-BdT9zkSH.js";
+import "./index-Cd3MtTMQ.js";
+import "./_baseEach-FAhoh2N5.js";
 import "./timer-D8GWrtRJ.js";
 import "./step-BEJ6WznM.js";
-import "./clone-BL0WSZ3Z.js";
-import "./edges-d32062c0-CFY3bIwa.js";
-import "./createText-6b48ae7d-129t9twG.js";
+import "./clone-CrCyWe3U.js";
+import "./edges-d32062c0-CU6OCHwI.js";
+import "./createText-6b48ae7d-BgOE7dMp.js";
 import "./line-Dz7yhIWK.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
-import "./sortBy-D0xI_7yL.js";
+import "./sortBy-DwX0cqqB.js";
 const y = "rect",
     u = "rectWithTitle",
     f = "statediagram",
     x = `${f}-state`,
     w = "transition",
     $ = `${w} note-edge`,
     j = `${f}-note`,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/step-BEJ6WznM.js` & `marimo-0.6.4/marimo/_static/assets/step-BEJ6WznM.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/stex-Ba7Sj9VR.js` & `marimo-0.6.4/marimo/_static/assets/stex-Ba7Sj9VR.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/styles-3ed67cfa-QdZmR4us.js` & `marimo-0.6.4/marimo/_static/assets/styles-3ed67cfa-Cg_XeDUz.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
 import {
     G as e
-} from "./graph-SHnEHiLi.js";
+} from "./graph-Dl9Z7r13.js";
 import {
     S as t,
     r as n,
     g as r,
     s as o
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     J as l,
     n as a,
     l as s,
     o as i,
     c,
     i as d,
     r as p,
     p as b,
     x as f,
     q as w,
     K as u
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     r as g
-} from "./index-fc10efb0-C3SRzTfT.js";
+} from "./index-fc10efb0-CJWvKICv.js";
 import {
     ix as h
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     c as y
-} from "./channel-DCiFYtzP.js";
+} from "./channel-BmGrl1HB.js";
 import {
     c as k
 } from "./step-BEJ6WznM.js";
 
 function x(e) {
     return "string" == typeof e ? new t([document.querySelectorAll(e)], [document.documentElement]) : new t([r(e)], n)
 }
```

### Comparing `marimo-0.6.3/marimo/_static/assets/styles-991ebdfc-CV9pCNxb.js` & `marimo-0.6.4/marimo/_static/assets/styles-991ebdfc-vxk4XA-a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 import {
     s as t
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     s as e,
     g as s,
     a as n,
     b as i,
     c as u,
     u as r,
     v as a,
     i as o,
     y as c,
     l,
     x as h,
     d as A,
     Q as p
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 var d = function() {
     var t = function(t, e, s, n) {
             for (s = s || {}, n = t.length; n--; s[t[n]] = e);
             return s
         },
         e = [1, 17],
         s = [1, 18],
```

### Comparing `marimo-0.6.3/marimo/_static/assets/styles-d20c7d72-BOwpCRGP.js` & `marimo-0.6.4/marimo/_static/assets/styles-d20c7d72-DtCcJufV.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     b as n,
     u as r,
     v as o,
     l as a,
     i as c,
     y as l,
     a2 as h
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 var u = function() {
     var t = function(t, e, s, i) {
             for (s = s || {}, i = t.length; i--; s[t[i]] = e);
             return s
         },
         e = [1, 2],
         s = [1, 3],
```

### Comparing `marimo-0.6.3/marimo/_static/assets/stylus-C-RTeXnz.js` & `marimo-0.6.4/marimo/_static/assets/stylus-C-RTeXnz.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/svgDrawCommon-5ccd53ef-BK5P1sG2.js` & `marimo-0.6.4/marimo/_static/assets/svgDrawCommon-5ccd53ef-DsDJYju_.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     m as t,
     k as a
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 const r = (t, a) => {
         const r = t.append("rect");
         if (r.attr("x", a.x), r.attr("y", a.y), r.attr("fill", a.fill), r.attr("stroke", a.stroke), r.attr("width", a.width), r.attr("height", a.height), a.name && r.attr("name", a.name), void 0 !== a.rx && r.attr("rx", a.rx), void 0 !== a.ry && r.attr("ry", a.ry), void 0 !== a.attrs)
             for (const s in a.attrs) r.attr(s, a.attrs[s]);
         return void 0 !== a.class && r.attr("class", a.class), r
     },
     s = (t, a) => {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/swift-Cbprqdc8.js` & `marimo-0.6.4/marimo/_static/assets/swift-Cbprqdc8.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/tcl-B2fODqDH.js` & `marimo-0.6.4/marimo/_static/assets/tcl-B2fODqDH.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/textile-BuVhTOzU.js` & `marimo-0.6.4/marimo/_static/assets/textile-BuVhTOzU.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/tiddlywiki-BgR6AEZu.js` & `marimo-0.6.4/marimo/_static/assets/tiddlywiki-BgR6AEZu.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/tiki-CI-ztowC.js` & `marimo-0.6.4/marimo/_static/assets/tiki-CI-ztowC.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/time-CUBsQdfc.js` & `marimo-0.6.4/marimo/_static/assets/time-CLRyKR-T.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     C as i,
     n as e,
     h as s
 } from "./timer-D8GWrtRJ.js";
 import {
     q as o,
     g as u
-} from "./linear-DF6Se9n2.js";
+} from "./linear-JxYcrfvc.js";
 import {
     i as c
 } from "./init-DLRA0X12.js";
 import {
     gT as h,
     hl as l,
     ju as f,
@@ -35,15 +35,15 @@
     h7 as x,
     jE as q,
     jF as A,
     jG as B,
     jH as C,
     jI as F,
     jJ as P
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 
 function z(t, n) {
     let r;
     if (void 0 === n)
         for (const a of t) null != a && (r < a || void 0 === r && a >= a) && (r = a);
     else {
         let a = -1;
```

### Comparing `marimo-0.6.3/marimo/_static/assets/timeline-definition-fea2a41d-B6Whk07l.js` & `marimo-0.6.4/marimo/_static/assets/timeline-definition-fea2a41d-DQvyLJzo.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,22 +3,22 @@
     y as e,
     c as n,
     l as i,
     q as s,
     a4 as r,
     a5 as a,
     a6 as o
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     s as c
-} from "./transform-DGMfQOK3.js";
+} from "./transform-DNjxe6pi.js";
 import {
     a as l
 } from "./arc-DIImc9ZO.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 import "./path-qnb_ma6O.js";
 var h = function() {
     var t = function(t, e, n, i) {
             for (n = n || {}, i = t.length; i--; n[t[i]] = e);
             return n
```

### Comparing `marimo-0.6.3/marimo/_static/assets/timer-D8GWrtRJ.js` & `marimo-0.6.4/marimo/_static/assets/timer-D8GWrtRJ.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/toml-BQXy8elZ.js` & `marimo-0.6.4/marimo/_static/assets/toml-BQXy8elZ.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/transform-DGMfQOK3.js` & `marimo-0.6.4/marimo/_static/assets/transform-DNjxe6pi.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     iG as t,
     ig as n,
     ik as e,
     iH as r,
     is as i
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     T as o,
     d as u,
     u as a,
     j as s,
     v as l,
     k as c,
```

### Comparing `marimo-0.6.3/marimo/_static/assets/troff-Ce85hlLp.js` & `marimo-0.6.4/marimo/_static/assets/troff-Ce85hlLp.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ttcn-C4reStyN.js` & `marimo-0.6.4/marimo/_static/assets/ttcn-C4reStyN.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/ttcn-cfg-Ce4xWtqN.js` & `marimo-0.6.4/marimo/_static/assets/ttcn-cfg-Ce4xWtqN.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/turtle-BkSuIpt-.js` & `marimo-0.6.4/marimo/_static/assets/turtle-BkSuIpt-.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/useMarimoWebSocket-BjNzCf7j.css` & `marimo-0.6.4/marimo/_static/assets/useMarimoWebSocket-BjNzCf7j.css`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/useMarimoWebSocket-DFV8TeGX.js` & `marimo-0.6.4/marimo/_static/assets/useMarimoWebSocket-Butgv0ej.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -99,15 +99,15 @@
     t as He,
     dp as Ie,
     g7 as Ae,
     dG as We,
     dF as qe,
     g8 as Be,
     bZ as Ge
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 /**
  * @license lucide-react v0.378.0 - ISC
  *
  * This source code is licensed under the ISC license.
  * See the LICENSE file in the root directory of this source tree.
  */
 const Fe = r("AlignEndVertical", [
```

### Comparing `marimo-0.6.3/marimo/_static/assets/vb-coDLL1b7.js` & `marimo-0.6.4/marimo/_static/assets/vb-coDLL1b7.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/vbscript-MdTt_wcJ.js` & `marimo-0.6.4/marimo/_static/assets/vbscript-MdTt_wcJ.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/vega-component-CZ4hZbd6.js` & `marimo-0.6.4/marimo/_static/assets/vega-component-B9WTop1f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,25 +8,25 @@
     Q as o,
     bW as c,
     gb as s,
     gc as l,
     aY as u,
     Y as p,
     X as d
-} from "./index-Dq6tg2Hn.js";
+} from "./index-Cd3MtTMQ.js";
 import {
     M as m,
     V as f
-} from "./VegaLite-BQwzJofD.js";
-import "./time-CUBsQdfc.js";
+} from "./VegaLite-rQgmZ7vL.js";
+import "./time-CLRyKR-T.js";
 import "./timer-D8GWrtRJ.js";
-import "./linear-DF6Se9n2.js";
+import "./linear-JxYcrfvc.js";
 import "./init-DLRA0X12.js";
 import "./range-CtcPcB_L.js";
-import "./index-ChUg6Fde.js";
+import "./index-AJ6VyMaJ.js";
 import "./ordinal-DDUp3AbE.js";
 import "./arc-DIImc9ZO.js";
 import "./path-qnb_ma6O.js";
 import "./step-BEJ6WznM.js";
 import "./array-DmjLdZ15.js";
 import "./line-Dz7yhIWK.js";
 const g = {
```

### Comparing `marimo-0.6.3/marimo/_static/assets/velocity-BdD_26Jv.js` & `marimo-0.6.4/marimo/_static/assets/velocity-BdD_26Jv.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/verilog-B4LBqg_1.js` & `marimo-0.6.4/marimo/_static/assets/verilog-B4LBqg_1.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/vhdl-BRDI21CQ.js` & `marimo-0.6.4/marimo/_static/assets/vhdl-BRDI21CQ.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/webidl-CGwyPRYs.js` & `marimo-0.6.4/marimo/_static/assets/webidl-CGwyPRYs.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/worker-DRJqITgt.js` & `marimo-0.6.4/marimo/_static/assets/worker-DRJqITgt.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/worker-DeVBMRpt.js` & `marimo-0.6.4/marimo/_static/assets/worker-DeVBMRpt.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/xquery-BZBLoTvf.js` & `marimo-0.6.4/marimo/_static/assets/xquery-BZBLoTvf.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/xychartDiagram-ab372869-DViGpnfl.js` & `marimo-0.6.4/marimo/_static/assets/xychartDiagram-ab372869-1vV9tLRe.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -10,35 +10,35 @@
     a as r,
     b as l,
     y as c,
     l as g,
     V as u,
     h as x,
     d
-} from "./mermaid-BDDPrcgz.js";
+} from "./mermaid-BI4dofVe.js";
 import {
     a as p
-} from "./createText-6b48ae7d-129t9twG.js";
-import "./transform-DGMfQOK3.js";
+} from "./createText-6b48ae7d-BgOE7dMp.js";
+import "./transform-DNjxe6pi.js";
 import {
     i as f
 } from "./init-DLRA0X12.js";
 import {
     o as y
 } from "./ordinal-DDUp3AbE.js";
 import {
     r as m
 } from "./range-CtcPcB_L.js";
 import {
     k as b
-} from "./linear-DF6Se9n2.js";
+} from "./linear-JxYcrfvc.js";
 import {
     l as A
 } from "./line-Dz7yhIWK.js";
-import "./index-Dq6tg2Hn.js";
+import "./index-Cd3MtTMQ.js";
 import "./step-BEJ6WznM.js";
 import "./timer-D8GWrtRJ.js";
 import "./array-DmjLdZ15.js";
 import "./path-qnb_ma6O.js";
 
 function w() {
     var t, i, e = y().unknown(void 0),
```

### Comparing `marimo-0.6.3/marimo/_static/assets/yacas-I8QjZlxf.js` & `marimo-0.6.4/marimo/_static/assets/yacas-I8QjZlxf.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/assets/z80-D8p3gKXp.js` & `marimo-0.6.4/marimo/_static/assets/z80-D8p3gKXp.js`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/favicon-16x16.png` & `marimo-0.6.4/marimo/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/favicon-32x32.png` & `marimo-0.6.4/marimo/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/favicon.ico` & `marimo-0.6.4/marimo/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/index.html` & `marimo-0.6.4/marimo/_static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,14 @@
     <marimo-filename hidden>{{ filename }}</marimo-filename>
     <marimo-mode data-mode='{{ mode }}' hidden></marimo-mode>
     <marimo-version data-version='{{ version }}' hidden></marimo-version>
     <marimo-user-config data-config='{{ user_config }}' hidden></marimo-user-config>
     <marimo-app-config data-config='{{ app_config }}' hidden></marimo-app-config>
     <marimo-server-token data-token='{{ server_token }}' hidden></marimo-server-token>
     <title>{{ title }}</title>
-    <script type="module" crossorigin src="./assets/index-Dq6tg2Hn.js"></script>
+    <script type="module" crossorigin src="./assets/index-Cd3MtTMQ.js"></script>
     <link rel="stylesheet" crossorigin href="./assets/index-CC7Qmxzq.css">
   </head>
   <body>
     <div id="root"></div>
   </body>
 </html>
```

### Comparing `marimo-0.6.3/marimo/_static/invalid_kernel_id.html` & `marimo-0.6.4/marimo/_static/invalid_kernel_id.html`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_static/logo.png` & `marimo-0.6.4/marimo/_static/logo.png`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/__init__.py` & `marimo-0.6.4/marimo/_tutorials/__init__.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/dataflow.py` & `marimo-0.6.4/marimo/_tutorials/dataflow.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/fileformat.py` & `marimo-0.6.4/marimo/_tutorials/fileformat.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/for_jupyter_users.py` & `marimo-0.6.4/marimo/_tutorials/for_jupyter_users.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/intro.py` & `marimo-0.6.4/marimo/_tutorials/intro.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/layout.py` & `marimo-0.6.4/marimo/_tutorials/layout.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/markdown.py` & `marimo-0.6.4/marimo/_tutorials/markdown.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/markdown_format.md` & `marimo-0.6.4/marimo/_tutorials/markdown_format.md`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/plots.py` & `marimo-0.6.4/marimo/_tutorials/plots.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_tutorials/ui.py` & `marimo-0.6.4/marimo/_tutorials/ui.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/config/config.py` & `marimo-0.6.4/marimo/_utils/config/config.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/debounce.py` & `marimo-0.6.4/marimo/_utils/debounce.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/deep_merge.py` & `marimo-0.6.4/marimo/_utils/deep_merge.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/deprecated.py` & `marimo-0.6.4/marimo/_utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/disposable.py` & `marimo-0.6.4/marimo/_utils/disposable.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/distributor.py` & `marimo-0.6.4/marimo/_utils/distributor.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/file_watcher.py` & `marimo-0.6.4/marimo/_utils/file_watcher.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/flatten.py` & `marimo-0.6.4/marimo/_utils/flatten.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/format_signature.py` & `marimo-0.6.4/marimo/_utils/format_signature.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/formatter.py` & `marimo-0.6.4/marimo/_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/health.py` & `marimo-0.6.4/marimo/_utils/health.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/log_formatter.py` & `marimo-0.6.4/marimo/_utils/log_formatter.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/marimo_path.py` & `marimo-0.6.4/marimo/_utils/marimo_path.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/parse_dataclass.py` & `marimo-0.6.4/marimo/_utils/parse_dataclass.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/paths.py` & `marimo-0.6.4/marimo/_utils/paths.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/rst_to_html.py` & `marimo-0.6.4/marimo/_utils/rst_to_html.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/signals.py` & `marimo-0.6.4/marimo/_utils/signals.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/tmpdir.py` & `marimo-0.6.4/marimo/_utils/tmpdir.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/typed_connection.py` & `marimo-0.6.4/marimo/_utils/typed_connection.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo/_utils/url.py` & `marimo-0.6.4/marimo/_utils/url.py`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/marimo.egg-info/PKG-INFO` & `marimo-0.6.4/marimo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marimo
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library for making reactive notebooks and apps
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `marimo-0.6.3/marimo.egg-info/SOURCES.txt` & `marimo-0.6.4/marimo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -390,16 +390,16 @@
 marimo/_static/favicon.ico
 marimo/_static/index.html
 marimo/_static/invalid_kernel_id.html
 marimo/_static/logo.png
 marimo/_static/manifest.json
 marimo/_static/site.webmanifest
 marimo/_static/assets/CarouselComponent-C12Ecb2K.css
-marimo/_static/assets/CarouselComponent-DtCAwyzo.js
-marimo/_static/assets/ConnectedDataExplorerComponent-DKdMG7z6.js
+marimo/_static/assets/CarouselComponent-ml4W_PuP.js
+marimo/_static/assets/ConnectedDataExplorerComponent-B6WI1UcR.js
 marimo/_static/assets/FiraMono-Bold-CLVRCuM9.ttf
 marimo/_static/assets/FiraMono-Medium-DU3aDxX5.ttf
 marimo/_static/assets/FiraMono-Regular-BTCkDNvf.ttf
 marimo/_static/assets/KaTeX_AMS-Regular-BQhdFMY1.woff2
 marimo/_static/assets/KaTeX_AMS-Regular-DMm9YOAa.woff
 marimo/_static/assets/KaTeX_AMS-Regular-DRggAlZN.ttf
 marimo/_static/assets/KaTeX_Caligraphic-Bold-ATXxdsX0.ttf
@@ -458,111 +458,111 @@
 marimo/_static/assets/KaTeX_Typewriter-Regular-C0xS9mPB.woff
 marimo/_static/assets/KaTeX_Typewriter-Regular-CO6r4hn1.woff2
 marimo/_static/assets/KaTeX_Typewriter-Regular-D3Ib7_Hf.ttf
 marimo/_static/assets/Lora-VariableFont_wght-B2ootaw-.ttf
 marimo/_static/assets/PTSans-Bold-D9fedIX3.ttf
 marimo/_static/assets/PTSans-Regular-CxL0S8W7.ttf
 marimo/_static/assets/Tableau10-B3EzvwxR.js
-marimo/_static/assets/VegaLite-BQwzJofD.js
-marimo/_static/assets/_baseEach-BrSWFoJM.js
-marimo/_static/assets/any-language-editor-D3MTmtyo.js
+marimo/_static/assets/VegaLite-rQgmZ7vL.js
+marimo/_static/assets/_baseEach-FAhoh2N5.js
+marimo/_static/assets/any-language-editor-Dzf9Jczi.js
 marimo/_static/assets/apl-CXdQSnD-.js
 marimo/_static/assets/arc-DIImc9ZO.js
 marimo/_static/assets/array-DmjLdZ15.js
 marimo/_static/assets/asciiarmor-D5V0T9Cu.js
 marimo/_static/assets/asn1-BhA3SgW2.js
 marimo/_static/assets/asterisk-B46aRdXb.js
-marimo/_static/assets/blockDiagram-91b80b7a-DPH13Qrf.js
+marimo/_static/assets/blockDiagram-91b80b7a-DSsN5jAx.js
 marimo/_static/assets/brainfuck-CtZaYBKt.js
-marimo/_static/assets/c4Diagram-b2a90758-CAH0Datt.js
-marimo/_static/assets/channel-DCiFYtzP.js
-marimo/_static/assets/classDiagram-30eddba6-Bz0cJX-U.js
-marimo/_static/assets/classDiagram-v2-f2df5561-BxNEwu6g.js
+marimo/_static/assets/c4Diagram-b2a90758-f1UFjA-x.js
+marimo/_static/assets/channel-BmGrl1HB.js
+marimo/_static/assets/classDiagram-30eddba6-BabWtcIB.js
+marimo/_static/assets/classDiagram-v2-f2df5561-D5SEk3xC.js
 marimo/_static/assets/clike-BPCXT8V3.js
 marimo/_static/assets/clojure-DR_hEDJv.js
-marimo/_static/assets/clone-BL0WSZ3Z.js
+marimo/_static/assets/clone-CrCyWe3U.js
 marimo/_static/assets/cmake-DXn5xaP-.js
 marimo/_static/assets/cobol-DJhTY0fG.js
 marimo/_static/assets/coffeescript-BTDxI-eT.js
 marimo/_static/assets/commonlisp-D09g7coK.js
-marimo/_static/assets/createText-6b48ae7d-129t9twG.js
+marimo/_static/assets/createText-6b48ae7d-BgOE7dMp.js
 marimo/_static/assets/crystal-CRzZ78HM.js
 marimo/_static/assets/css-ZjFoif2m.js
 marimo/_static/assets/cypher-gJDei3ni.js
 marimo/_static/assets/d-BShv7fp-.js
 marimo/_static/assets/diff-UJJ5BM9S.js
 marimo/_static/assets/dockerfile-BLgfkd__.js
 marimo/_static/assets/dtd-DI9Herc-.js
 marimo/_static/assets/dylan-CHJ5qNM_.js
 marimo/_static/assets/ebnf-B-Df8AvO.js
 marimo/_static/assets/ecl-DPFc0Uaf.js
-marimo/_static/assets/edges-d32062c0-CFY3bIwa.js
-marimo/_static/assets/edit-page-CIzFhPq5.js
+marimo/_static/assets/edges-d32062c0-CU6OCHwI.js
 marimo/_static/assets/edit-page-CwGzkSpM.css
+marimo/_static/assets/edit-page-DnXnHWMg.js
 marimo/_static/assets/eiffel-BZ5y0wDL.js
 marimo/_static/assets/elm-D7xaZ7Da.js
-marimo/_static/assets/erDiagram-47591fe2-CJ2SMwAy.js
+marimo/_static/assets/erDiagram-47591fe2-UyJH0JYd.js
 marimo/_static/assets/erlang-BuqgqA5h.js
 marimo/_static/assets/factor-Bm2WRyNM.js
 marimo/_static/assets/fcl-CVaBTCzQ.js
-marimo/_static/assets/flowDb-4b19a42f-4mXsCvSf.js
-marimo/_static/assets/flowDiagram-5540d9b9-msf8H4Jk.js
-marimo/_static/assets/flowDiagram-v2-3b53844e-BRBAHwua.js
-marimo/_static/assets/flowchart-elk-definition-5fe447d6-tgRhUdQk.js
+marimo/_static/assets/flowDb-4b19a42f-Cf4l3Vi7.js
+marimo/_static/assets/flowDiagram-5540d9b9-CuVcDbrT.js
+marimo/_static/assets/flowDiagram-v2-3b53844e-By9U58mT.js
+marimo/_static/assets/flowchart-elk-definition-5fe447d6-BpUsl4Jm.js
 marimo/_static/assets/forth-Dri_5nFc.js
 marimo/_static/assets/fortran-DL7KluxX.js
-marimo/_static/assets/ganttDiagram-9a3bba1f-Clnqsx9q.js
+marimo/_static/assets/ganttDiagram-9a3bba1f-W6mmWQNE.js
 marimo/_static/assets/gas-5kEe4nk0.js
 marimo/_static/assets/gherkin-B6X1vGSW.js
-marimo/_static/assets/gitGraphDiagram-96e6b4ee-BUgJQeEj.js
+marimo/_static/assets/gitGraphDiagram-96e6b4ee-BKc9lhir.js
 marimo/_static/assets/gradient-yHQUC_QB.png
-marimo/_static/assets/graph-SHnEHiLi.js
+marimo/_static/assets/graph-Dl9Z7r13.js
 marimo/_static/assets/groovy-BfRUB6GO.js
 marimo/_static/assets/haskell-CmdsSjFB.js
 marimo/_static/assets/haxe-75PMBtaN.js
-marimo/_static/assets/home-page-BmvI7Tzs.js
+marimo/_static/assets/home-page-BL9ArKPs.js
 marimo/_static/assets/http-BKJkqRj4.js
-marimo/_static/assets/icons-6JftBaIY.js
 marimo/_static/assets/icons-D-PkNarU.css
+marimo/_static/assets/icons-DtRVr9-T.js
 marimo/_static/assets/idl-pcmmZuaN.js
-marimo/_static/assets/index-0fF0Xoai.js
-marimo/_static/assets/index-7VEF_U3p.js
-marimo/_static/assets/index-BuR6fZZm.js
-marimo/_static/assets/index-C2GbrbZr.js
+marimo/_static/assets/index-1IpQZ_Yu.js
+marimo/_static/assets/index-AJ6VyMaJ.js
+marimo/_static/assets/index-BH1DvUFb.js
+marimo/_static/assets/index-BYVYp6Ei.js
+marimo/_static/assets/index-CB4e2-IR.js
 marimo/_static/assets/index-CC7Qmxzq.css
-marimo/_static/assets/index-ChUg6Fde.js
-marimo/_static/assets/index-Ck0jzFpb.js
-marimo/_static/assets/index-ClCDnvOE.js
-marimo/_static/assets/index-CohQOVlj.js
-marimo/_static/assets/index-CzWuvzvc.js
-marimo/_static/assets/index-D4als0Dc.js
-marimo/_static/assets/index-DgcwnKY7.js
-marimo/_static/assets/index-Dq6tg2Hn.js
-marimo/_static/assets/index-DzhIfGoT.js
-marimo/_static/assets/index-O7K-_bwp.js
-marimo/_static/assets/index-S9qVQ2oC.js
-marimo/_static/assets/index-VNKARDPQ.js
-marimo/_static/assets/index-fc10efb0-C3SRzTfT.js
-marimo/_static/assets/index-jW3n8_hn.js
-marimo/_static/assets/infoDiagram-bcd20f53-BIy3DJKx.js
+marimo/_static/assets/index-CE06HdF7.js
+marimo/_static/assets/index-Cd3MtTMQ.js
+marimo/_static/assets/index-DCESMHe2.js
+marimo/_static/assets/index-DahJleVt.js
+marimo/_static/assets/index-DgOauLen.js
+marimo/_static/assets/index-DqGPWGPa.js
+marimo/_static/assets/index-DtyNPFfa.js
+marimo/_static/assets/index-KIzq3vhX.js
+marimo/_static/assets/index-XFgu4285.js
+marimo/_static/assets/index-fc10efb0-CJWvKICv.js
+marimo/_static/assets/index-rXOiTwQN.js
+marimo/_static/assets/index-wbyGdlc1.js
+marimo/_static/assets/index-yuQsQmno.js
+marimo/_static/assets/infoDiagram-bcd20f53-CAV4G93w.js
 marimo/_static/assets/init-DLRA0X12.js
 marimo/_static/assets/javascript-DY1Qj14w.js
 marimo/_static/assets/jinja2-DhgKlfW7.js
-marimo/_static/assets/journeyDiagram-4fe6b3dc-C_g7a5O5.js
+marimo/_static/assets/journeyDiagram-4fe6b3dc-DOB96Qnq.js
 marimo/_static/assets/julia-DjdwvFuI.js
 marimo/_static/assets/katex-BnMoLUs3.js
-marimo/_static/assets/layout-DDD1odkP.js
+marimo/_static/assets/layout-BdT9zkSH.js
 marimo/_static/assets/line-Dz7yhIWK.js
-marimo/_static/assets/linear-DF6Se9n2.js
+marimo/_static/assets/linear-JxYcrfvc.js
 marimo/_static/assets/livescript-B19OIWEP.js
 marimo/_static/assets/lua-8DXOpKDz.js
 marimo/_static/assets/mathematica-IIbmv7SK.js
 marimo/_static/assets/mbox-DoeuZPxA.js
-marimo/_static/assets/mermaid-BDDPrcgz.js
-marimo/_static/assets/mindmap-definition-f354de21-BT0462Yo.js
+marimo/_static/assets/mermaid-BI4dofVe.js
+marimo/_static/assets/mindmap-definition-f354de21-CQ2IslvL.js
 marimo/_static/assets/mirc-DkvFAiy5.js
 marimo/_static/assets/mllike-B8DYu8SS.js
 marimo/_static/assets/modelica-DSrSSXCg.js
 marimo/_static/assets/mscgen-B2igx18G.js
 marimo/_static/assets/mumps-zvxmGV4l.js
 marimo/_static/assets/nginx-B4hAVlXN.js
 marimo/_static/assets/noise-60BoTA8O.png
@@ -570,81 +570,81 @@
 marimo/_static/assets/ntriples-FFvkTduk.js
 marimo/_static/assets/octave-C4hdQ5Hf.js
 marimo/_static/assets/ordinal-DDUp3AbE.js
 marimo/_static/assets/oz-qQq7irPq.js
 marimo/_static/assets/pascal-CZ0JYm71.js
 marimo/_static/assets/path-qnb_ma6O.js
 marimo/_static/assets/perl-tdMlh9QA.js
-marimo/_static/assets/pieDiagram-79897490-DVu-KYPX.js
+marimo/_static/assets/pieDiagram-79897490-DznITiVM.js
 marimo/_static/assets/pig-CwGJVRC4.js
 marimo/_static/assets/powershell-D1ly3AHC.js
 marimo/_static/assets/properties-_nPj978X.js
 marimo/_static/assets/protobuf-B4y9do6W.js
 marimo/_static/assets/pug-BNyZbGOm.js
 marimo/_static/assets/puppet-Bc-yJKzi.js
 marimo/_static/assets/python-DD-Q2bae.js
 marimo/_static/assets/q-B0kTJ4cI.js
-marimo/_static/assets/quadrantDiagram-62f64e94-CU-4FuJa.js
+marimo/_static/assets/quadrantDiagram-62f64e94-Df4mAWqb.js
 marimo/_static/assets/r-BA4EbLKE.js
 marimo/_static/assets/range-CtcPcB_L.js
-marimo/_static/assets/react-plotly-Bf9tHX8H.js
-marimo/_static/assets/requirementDiagram-05bf5f74-BsI08XXR.js
+marimo/_static/assets/react-plotly-C4-ZLKix.js
+marimo/_static/assets/requirementDiagram-05bf5f74-DyUtzGOy.js
 marimo/_static/assets/rpm-DI_rRufH.js
 marimo/_static/assets/ruby-CR-u2WLS.js
-marimo/_static/assets/run-page-BflrRP7S.js
-marimo/_static/assets/sankeyDiagram-97764748-BQdZQP_-.js
+marimo/_static/assets/run-page-D_UJForb.js
+marimo/_static/assets/sankeyDiagram-97764748-DvvFNiJT.js
 marimo/_static/assets/sas-Bqaci40L.js
 marimo/_static/assets/save-worker-f86VBHv4.js
 marimo/_static/assets/scheme-qjP0V5Ag.js
-marimo/_static/assets/sequenceDiagram-acc0e65c-Dsgiz64s.js
+marimo/_static/assets/sequenceDiagram-acc0e65c-DquwX6r9.js
 marimo/_static/assets/shell-BLav31RL.js
 marimo/_static/assets/sieve-r025o_jW.js
 marimo/_static/assets/simple-mode-Ckv7_vD8.js
 marimo/_static/assets/smalltalk-C7J3IyEP.js
 marimo/_static/assets/solr-78MBEUkU.js
-marimo/_static/assets/sortBy-D0xI_7yL.js
+marimo/_static/assets/sortBy-DwX0cqqB.js
 marimo/_static/assets/sparql-BRLJFz69.js
 marimo/_static/assets/spreadsheet-CGlWr0eM.js
 marimo/_static/assets/sql-BP5jFf-w.js
-marimo/_static/assets/stateDiagram-0ff1cf1a-lr9-t8r1.js
-marimo/_static/assets/stateDiagram-v2-9a9d610d-DwjKCx-9.js
+marimo/_static/assets/stateDiagram-0ff1cf1a-DjUkVeHK.js
+marimo/_static/assets/stateDiagram-v2-9a9d610d-C6LzE_mY.js
 marimo/_static/assets/step-BEJ6WznM.js
 marimo/_static/assets/stex-Ba7Sj9VR.js
-marimo/_static/assets/styles-3ed67cfa-QdZmR4us.js
-marimo/_static/assets/styles-991ebdfc-CV9pCNxb.js
-marimo/_static/assets/styles-d20c7d72-BOwpCRGP.js
+marimo/_static/assets/styles-3ed67cfa-Cg_XeDUz.js
+marimo/_static/assets/styles-991ebdfc-vxk4XA-a.js
+marimo/_static/assets/styles-d20c7d72-DtCcJufV.js
 marimo/_static/assets/stylus-C-RTeXnz.js
-marimo/_static/assets/svgDrawCommon-5ccd53ef-BK5P1sG2.js
+marimo/_static/assets/svgDrawCommon-5ccd53ef-DsDJYju_.js
 marimo/_static/assets/swift-Cbprqdc8.js
 marimo/_static/assets/tcl-B2fODqDH.js
 marimo/_static/assets/textile-BuVhTOzU.js
 marimo/_static/assets/tiddlywiki-BgR6AEZu.js
 marimo/_static/assets/tiki-CI-ztowC.js
-marimo/_static/assets/time-CUBsQdfc.js
-marimo/_static/assets/timeline-definition-fea2a41d-B6Whk07l.js
+marimo/_static/assets/time-CLRyKR-T.js
+marimo/_static/assets/timeline-definition-fea2a41d-DQvyLJzo.js
 marimo/_static/assets/timer-D8GWrtRJ.js
 marimo/_static/assets/toml-BQXy8elZ.js
-marimo/_static/assets/transform-DGMfQOK3.js
+marimo/_static/assets/transform-DNjxe6pi.js
 marimo/_static/assets/troff-Ce85hlLp.js
 marimo/_static/assets/ttcn-C4reStyN.js
 marimo/_static/assets/ttcn-cfg-Ce4xWtqN.js
 marimo/_static/assets/turtle-BkSuIpt-.js
 marimo/_static/assets/useMarimoWebSocket-BjNzCf7j.css
-marimo/_static/assets/useMarimoWebSocket-DFV8TeGX.js
+marimo/_static/assets/useMarimoWebSocket-Butgv0ej.js
 marimo/_static/assets/vb-coDLL1b7.js
 marimo/_static/assets/vbscript-MdTt_wcJ.js
-marimo/_static/assets/vega-component-CZ4hZbd6.js
+marimo/_static/assets/vega-component-B9WTop1f.js
 marimo/_static/assets/velocity-BdD_26Jv.js
 marimo/_static/assets/verilog-B4LBqg_1.js
 marimo/_static/assets/vhdl-BRDI21CQ.js
 marimo/_static/assets/webidl-CGwyPRYs.js
 marimo/_static/assets/worker-DRJqITgt.js
 marimo/_static/assets/worker-DeVBMRpt.js
 marimo/_static/assets/xquery-BZBLoTvf.js
-marimo/_static/assets/xychartDiagram-ab372869-DViGpnfl.js
+marimo/_static/assets/xychartDiagram-ab372869-1vV9tLRe.js
 marimo/_static/assets/yacas-I8QjZlxf.js
 marimo/_static/assets/z80-D8p3gKXp.js
 marimo/_tutorials/README.md
 marimo/_tutorials/__init__.py
 marimo/_tutorials/dataflow.py
 marimo/_tutorials/fileformat.py
 marimo/_tutorials/for_jupyter_users.py
```

### Comparing `marimo-0.6.3/marimo.egg-info/requires.txt` & `marimo-0.6.4/marimo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/pyproject.toml` & `marimo-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/third_party.txt` & `marimo-0.6.4/third_party.txt`

 * *Files identical despite different names*

### Comparing `marimo-0.6.3/third_party_licenses.txt` & `marimo-0.6.4/third_party_licenses.txt`

 * *Files identical despite different names*

