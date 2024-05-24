# Comparing `tmp/streamlit_nightly-1.34.1.dev20240521.tar.gz` & `tmp/streamlit_nightly-1.34.1.dev20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.34.1.dev20240521.tar", last modified: Wed May 22 06:55:07 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.34.1.dev20240522.tar", last modified: Thu May 23 06:55:27 2024, max compression
```

## Comparing `streamlit_nightly-1.34.1.dev20240521.tar` & `streamlit_nightly-1.34.1.dev20240522.tar`

### file list

```diff
@@ -1,574 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.859869 streamlit_nightly-1.34.1.dev20240521/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-22 06:55:07.859869 streamlit_nightly-1.34.1.dev20240521/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.739869 streamlit_nightly-1.34.1.dev20240521/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:55:07.859869 streamlit_nightly-1.34.1.dev20240521/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.747869 streamlit_nightly-1.34.1.dev20240521/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.747869 streamlit_nightly-1.34.1.dev20240521/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.747869 streamlit_nightly-1.34.1.dev20240521/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.747869 streamlit_nightly-1.34.1.dev20240521/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.747869 streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.751869 streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.751869 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.755869 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    23830 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.759869 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.763869 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.763869 streamlit_nightly-1.34.1.dev20240521/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.763869 streamlit_nightly-1.34.1.dev20240521/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.763869 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.763869 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.787869 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-22 06:51:15.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.791869 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.795869 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.795869 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.795869 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.795869 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.799869 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.799869 streamlit_nightly-1.34.1.dev20240521/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-22 06:51:44.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.739869 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.799869 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/8148.49dfd2ce.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.831869 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1168.14f7c6ff.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3513.7dedbda2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4113.99983645.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/474.7eb0c6cd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5345.73d26e5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5441.1b94928f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6013.4ba2d616.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6950.70fe55c2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    51109 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8148.f80eec24.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9336.3e046ad7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4405422 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/main.9db3e91c.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/main.9db3e91c.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.851869 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-22 06:55:04.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.851869 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.851869 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.851869 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.851869 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.851869 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.855869 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.855869 streamlit_nightly-1.34.1.dev20240521/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.855869 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.859869 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-22 06:55:06.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23316 2024-05-22 06:55:06.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:55:06.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 06:55:06.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:51:12.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 06:55:06.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 06:55:06.000000 streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:55:07.859869 streamlit_nightly-1.34.1.dev20240521/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-22 06:49:39.000000 streamlit_nightly-1.34.1.dev20240521/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.028568 streamlit_nightly-1.34.1.dev20240522/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.036568 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.040568 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.044568 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23830 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.044568 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.048568 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.052568 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.076568 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-23 06:51:46.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.080568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.080568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.084568 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.088568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-23 06:52:14.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.024568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.088568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/8148.49dfd2ce.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.120568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1168.14f7c6ff.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3513.7dedbda2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/474.7eb0c6cd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5345.73d26e5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5441.1b94928f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6950.70fe55c2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51115 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8148.a17a918e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9336.3e046ad7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4405422 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.136568 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-23 06:55:24.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.136568 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.140568 streamlit_nightly-1.34.1.dev20240522/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23316 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:51:43.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 06:55:25.000000 streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:55:27.144568 streamlit_nightly-1.34.1.dev20240522/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-23 06:50:22.000000 streamlit_nightly-1.34.1.dev20240522/tests/testutil.py
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240522/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240521
+Version: 1.34.1.dev20240522
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/bin/streamlit.cmd` & `streamlit_nightly-1.34.1.dev20240522/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/setup.py` & `streamlit_nightly-1.34.1.dev20240522/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.34.1.dev20240521"  # PEP-440
+VERSION = "1.34.1.dev20240522"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/__main__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/case_converters.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/cli_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/code_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/color_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/column_config.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/commands/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/commands/execution_control.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/commands/logo.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/logo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/commands/page_config.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/types/base_custom_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from streamlit import util
 from streamlit.errors import StreamlitAPIException
 
+if TYPE_CHECKING:
+    from streamlit.runtime.state.common import WidgetCallback
+
 
 class MarshallComponentException(StreamlitAPIException):
     """Class for exceptions generated during custom component marshalling."""
 
     pass
 
 
@@ -52,18 +55,25 @@
         return util.repr_(self)
 
     def __call__(
         self,
         *args,
         default: Any = None,
         key: str | None = None,
+        on_change: WidgetCallback | None = None,
         **kwargs,
     ) -> Any:
         """An alias for create_instance."""
-        return self.create_instance(*args, default=default, key=key, **kwargs)
+        return self.create_instance(
+            *args,
+            default=default,
+            key=key,
+            on_change=on_change,
+            **kwargs,
+        )
 
     @property
     def abspath(self) -> str | None:
         if self._path is None:
             return None
         return os.path.abspath(self._path)
 
@@ -98,14 +108,15 @@
 
     @abstractmethod
     def create_instance(
         self,
         *args,
         default: Any = None,
         key: str | None = None,
+        on_change: WidgetCallback | None = None,
         **kwargs,
     ) -> Any:
         """Create a new instance of the component.
 
         Parameters
         ----------
         *args
@@ -114,14 +125,16 @@
         default: any or None
             The default return value for the component. This is returned when
             the component's frontend hasn't yet specified a value with
             `setComponentValue`.
         key: str or None
             If not None, this is the user key we use to generate the
             component's "widget ID".
+        on_change: WidgetCallback or None
+            An optional callback invoked when the widget's value changes. No arguments are passed to it.
         **kwargs
             Keyword args to pass to the component.
 
         Raises
         ------
         MarshallComponentException
             Raised when args is not empty or component cannot be marshalled.
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/components.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/components/v1/custom_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from streamlit.runtime.scriptrunner import get_script_run_ctx
 from streamlit.runtime.state import NoValue, register_widget
 from streamlit.runtime.state.common import compute_widget_id
 from streamlit.type_util import to_bytes
 
 if TYPE_CHECKING:
     from streamlit.delta_generator import DeltaGenerator
+    from streamlit.runtime.state.common import WidgetCallback
 
 
 class MarshallComponentException(StreamlitAPIException):
     """Class for exceptions generated during custom component marshalling."""
 
     pass
 
@@ -45,25 +46,33 @@
     """A Custom Component declaration."""
 
     def __call__(
         self,
         *args,
         default: Any = None,
         key: str | None = None,
+        on_change: WidgetCallback | None = None,
         **kwargs,
     ) -> Any:
         """An alias for create_instance."""
-        return self.create_instance(*args, default=default, key=key, **kwargs)
+        return self.create_instance(
+            *args,
+            default=default,
+            key=key,
+            on_change=on_change,
+            **kwargs,
+        )
 
     @gather_metrics("create_instance")
     def create_instance(
         self,
         *args,
         default: Any = None,
         key: str | None = None,
+        on_change: WidgetCallback | None = None,
         **kwargs,
     ) -> Any:
         """Create a new instance of the component.
 
         Parameters
         ----------
         *args
@@ -72,14 +81,16 @@
         default: any or None
             The default return value for the component. This is returned when
             the component's frontend hasn't yet specified a value with
             `setComponentValue`.
         key: str or None
             If not None, this is the user key we use to generate the
             component's "widget ID".
+        on_change: WidgetCallback or None
+            An optional callback invoked when the widget's value changes. No arguments are passed to it.
         **kwargs
             Keyword args to pass to the component.
 
         Returns
         -------
         any or None
             The component's widget value.
@@ -191,14 +202,15 @@
                 element_type="component_instance",
                 element_proto=element.component_instance,
                 user_key=key,
                 widget_func_name=self.name,
                 deserializer=deserialize_component,
                 serializer=lambda x: x,
                 ctx=ctx,
+                on_change_handler=on_change,
             )
             widget_value = component_state.value
 
             if key is not None:
                 marshall_element_args()
 
             if widget_value is None:
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/config.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/config_option.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/config_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/connections/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/connections/base_connection.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/connections/util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/constants.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/cursor.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/delta_generator.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/deprecation_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/development.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/echo.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/alert.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/arrow.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/balloons.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/code.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/dialog_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,21 +82,21 @@
 
 
 # 'title' can be a function since `dialog_decorator` is a decorator. We just call it 'title' here though
 # to make the user-doc more friendly as we want the user to pass a title, not a function.
 # The user is supposed to call it like @st.dialog("my_title") , which makes 'title' a positional arg, hence
 # this 'trick'. The overload is required to have a good type hint for the decorated function args.
 @overload
-def dialog_decorator(title: F | None, *, width: DialogWidth = "small") -> F:
+def dialog_decorator(title: F, *, width: DialogWidth = "small") -> F:
     ...
 
 
 @gather_metrics("experimental_dialog")
 def dialog_decorator(
-    title: F | None | str = "", *, width: DialogWidth = "small"
+    title: F | str, *, width: DialogWidth = "small"
 ) -> F | Callable[[F], F]:
     """Function decorator to create a modal dialog.
 
     A function decorated with ``@st.experimental_dialog`` becomes a dialog
     function. When you call a dialog function, Streamlit inserts a modal dialog
     into your app. Streamlit element commands called within the dialog function
     render inside the modal dialog.
@@ -169,21 +169,15 @@
     .. output::
         https://doc-modal-dialog.streamlit.app/
         height: 350px
 
     """
 
     func_or_title = title
-    if func_or_title is None:
-        # Support passing the params via function decorator
-        def wrapper(f: F) -> F:
-            return _dialog_decorator(non_optional_func=f, title="", width=width)
-
-        return wrapper
-    elif type(func_or_title) is str:
+    if type(func_or_title) is str:
         # Support passing the params via function decorator
         def wrapper(f: F) -> F:
             title: str = func_or_title
             return _dialog_decorator(non_optional_func=f, title=title, width=width)
 
         return wrapper
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/doc_string.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/empty.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/exception.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/form.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/heading.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/html.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/iframe.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/image.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/json.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/layouts.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/map.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/markdown.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/media.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/metric.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/progress.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/pyplot.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/snow.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/spinner.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/text.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/toast.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/vega_charts.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/vega_charts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/elements/write.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/emojis.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/env_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/error_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/errors.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/external/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/file_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/folder_black_list.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/git_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/Hello.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/hello/utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/js_number.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/logger.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/material_icon_names.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/net_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/platform.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240522/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/app_session.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/credentials.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/fragment.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/runtime.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/script_data.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/secrets.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/common.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     """Return the user key portion of a widget id, or None if the id does not
     have a user key.
 
     TODO This will incorrectly indicate no user key if the user actually provides
     "None" as a key, but we can't avoid this kind of problem while storing the
     string representation of the no-user-key sentinel as part of the widget id.
     """
-    user_key = widget_id.split("-", maxsplit=2)[-1]
+    user_key: str | None = widget_id.split("-", maxsplit=2)[-1]
     user_key = None if user_key == "None" else user_key
     return user_key
 
 
 def is_widget_id(key: str) -> bool:
     """True if the given session_state key has the structure of a widget ID."""
     return key.startswith(GENERATED_WIDGET_ID_PREFIX)
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/stats.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/source_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/asset-manifest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8291387024608501%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.7e42f54d.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.7e42f54d.js', 'static/js/8148.a17a918e.chunk.js': "*

 * *            "'./static/js/8148.a17a918e.chunk.js', delete: ['static/js/8148.f80eec24.chunk.js']}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "entrypoints": [
         "static/css/main.3aaaea00.css",
-        "static/js/main.9db3e91c.js"
+        "static/js/main.7e42f54d.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.3aaaea00.css",
-        "main.js": "./static/js/main.9db3e91c.js",
+        "main.js": "./static/js/main.7e42f54d.js",
         "static/css/3466.8b8f33d6.chunk.css": "./static/css/3466.8b8f33d6.chunk.css",
         "static/css/5441.e3b876c5.chunk.css": "./static/css/5441.e3b876c5.chunk.css",
         "static/css/8148.49dfd2ce.chunk.css": "./static/css/8148.49dfd2ce.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.14f7c6ff.chunk.js": "./static/js/1168.14f7c6ff.chunk.js",
         "static/js/1307.0f0cca93.chunk.js": "./static/js/1307.0f0cca93.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
@@ -50,15 +50,15 @@
         "static/js/7142.83028745.chunk.js": "./static/js/7142.83028745.chunk.js",
         "static/js/7175.be4076bc.chunk.js": "./static/js/7175.be4076bc.chunk.js",
         "static/js/7323.b74cc85b.chunk.js": "./static/js/7323.b74cc85b.chunk.js",
         "static/js/7483.64f23be7.chunk.js": "./static/js/7483.64f23be7.chunk.js",
         "static/js/7602.e8abc06b.chunk.js": "./static/js/7602.e8abc06b.chunk.js",
         "static/js/7805.acc6316a.chunk.js": "./static/js/7805.acc6316a.chunk.js",
         "static/js/8005.43974a35.chunk.js": "./static/js/8005.43974a35.chunk.js",
-        "static/js/8148.f80eec24.chunk.js": "./static/js/8148.f80eec24.chunk.js",
+        "static/js/8148.a17a918e.chunk.js": "./static/js/8148.a17a918e.chunk.js",
         "static/js/8427.bd0a7cf3.chunk.js": "./static/js/8427.bd0a7cf3.chunk.js",
         "static/js/8477.de889fe5.chunk.js": "./static/js/8477.de889fe5.chunk.js",
         "static/js/8492.0d93bd08.chunk.js": "./static/js/8492.0d93bd08.chunk.js",
         "static/js/8536.f8de3d9a.chunk.js": "./static/js/8536.f8de3d9a.chunk.js",
         "static/js/8570.6de19120.chunk.js": "./static/js/8570.6de19120.chunk.js",
         "static/js/8691.9ccf7f89.chunk.js": "./static/js/8691.9ccf7f89.chunk.js",
         "static/js/9330.2b4c99e0.chunk.js": "./static/js/9330.2b4c99e0.chunk.js",
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/favicon.png` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/index.html` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.9db3e91c.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.7e42f54d.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/8148.49dfd2ce.chunk.css` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/8148.49dfd2ce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1168.14f7c6ff.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1168.14f7c6ff.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/3513.7dedbda2.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/3513.7dedbda2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4113.99983645.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/474.7eb0c6cd.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/474.7eb0c6cd.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5345.73d26e5d.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5345.73d26e5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5441.1b94928f.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5441.1b94928f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6013.4ba2d616.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/6950.70fe55c2.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/6950.70fe55c2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8148.f80eec24.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8148.a17a918e.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2150,15 +2150,15 @@
                         });
                     void 0 !== o && o === i || v.setStringValue({
                         id: t.id,
                         formId: t.formId
                     }, i, {
                         fromUi: !0
                     }, E)
-                })), [t.id, t.formId, v, E]), {
+                })), [t.id, t.formId, v, E, ae, Ke]), {
                     gridSelection: ce,
                     isRowSelectionActivated: ue,
                     isMultiRowSelectionActivated: me,
                     isColumnSelectionActivated: he,
                     isMultiColumnSelectionActivated: pe,
                     isRowSelected: ge,
                     isColumnSelected: fe,
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9336.3e046ad7.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9336.3e046ad7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/main.9db3e91c.js` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.9db3e91c.js.LICENSE.txt */
+/*! For license information please see main.7e42f54d.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -116110,15 +116110,15 @@
         7142: "83028745",
         7175: "be4076bc",
         7323: "b74cc85b",
         7483: "64f23be7",
         7602: "e8abc06b",
         7805: "acc6316a",
         8005: "43974a35",
-        8148: "f80eec24",
+        8148: "a17a918e",
         8427: "bd0a7cf3",
         8477: "de889fe5",
         8492: "0d93bd08",
         8536: "f8de3d9a",
         8570: "6de19120",
         8691: "9ccf7f89",
         9330: "2b4c99e0",
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/js/main.9db3e91c.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.34.1.dev20240522/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/string_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/temporary_directory.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/testing/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/testing/v1/util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/time_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/type_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/url_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/user_info.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/version.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/watcher/util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/bootstrap.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/cli.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/__init__.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/routes.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/server.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/server_util.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.34.1.dev20240522/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240521
+Version: 1.34.1.dev20240522
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.34.1.dev20240522/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -387,29 +387,29 @@
 streamlit/static/static/js/7323.b74cc85b.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
 streamlit/static/static/js/7483.64f23be7.chunk.js
 streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
 streamlit/static/static/js/7602.e8abc06b.chunk.js
 streamlit/static/static/js/7805.acc6316a.chunk.js
 streamlit/static/static/js/8005.43974a35.chunk.js
-streamlit/static/static/js/8148.f80eec24.chunk.js
+streamlit/static/static/js/8148.a17a918e.chunk.js
 streamlit/static/static/js/8427.bd0a7cf3.chunk.js
 streamlit/static/static/js/8477.de889fe5.chunk.js
 streamlit/static/static/js/8492.0d93bd08.chunk.js
 streamlit/static/static/js/8536.f8de3d9a.chunk.js
 streamlit/static/static/js/8570.6de19120.chunk.js
 streamlit/static/static/js/8691.9ccf7f89.chunk.js
 streamlit/static/static/js/9330.2b4c99e0.chunk.js
 streamlit/static/static/js/9336.3e046ad7.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.9db3e91c.js
-streamlit/static/static/js/main.9db3e91c.js.LICENSE.txt
+streamlit/static/static/js/main.7e42f54d.js
+streamlit/static/static/js/main.7e42f54d.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.34.1.dev20240521/tests/testutil.py` & `streamlit_nightly-1.34.1.dev20240522/tests/testutil.py`

 * *Files identical despite different names*

