# Comparing `tmp/dashtable2-1.4.8.tar.gz` & `tmp/dashtable2-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashtable2-1.4.8.tar", last modified: Mon May 20 19:48:23 2024, max compression
+gzip compressed data, was "dashtable2-1.4.9.tar", last modified: Fri May 24 08:03:13 2024, max compression
```

## Comparing `dashtable2-1.4.8.tar` & `dashtable2-1.4.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.950433 dashtable2-1.4.8/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1068 2024-05-20 13:11:43.000000 dashtable2-1.4.8/LICENSE.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1107 2024-05-20 19:48:23.950433 dashtable2-1.4.8/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)      480 2024-05-20 13:40:39.000000 dashtable2-1.4.8/README.md
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.940432 dashtable2-1.4.8/dashtable/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      418 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.941433 dashtable2-1.4.8/dashtable/dashutils/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      441 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1134 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/add_cushions.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      760 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/center_line.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3239 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/checks.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      326 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/ensure_table_strings.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      547 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/make_empty_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      798 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/make_span.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      436 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/multis_2_mono.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3789 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/dashutils/spans.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.942432 dashtable2-1.4.8/dashtable/data2md/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       29 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2md/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1886 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2md/data2md.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      546 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2md/get_column_width.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.942432 dashtable2-1.4.8/dashtable/data2rst/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       31 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.943432 dashtable2-1.4.8/dashtable/data2rst/cell/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      296 2024-05-20 18:22:16.000000 dashtable2-1.4.8/dashtable/data2rst/cell/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3643 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/cell/cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1291 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/cell/center_cell_text.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/cell/get_longest_line_length.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      203 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/cell/is_only.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     5234 2024-05-20 19:47:48.000000 dashtable2-1.4.8/dashtable/data2rst/cell/merge.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1796 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/cell/v_center_cell_text.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3661 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/data2rst.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2085 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/get_output_column_widths.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1558 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/get_output_row_heights.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1867 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/make_cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1501 2024-05-20 18:22:16.000000 dashtable2-1.4.8/dashtable/data2rst/merge_all_cells.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      937 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2rst/table_cells_2_spans.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.944433 dashtable2-1.4.8/dashtable/data2simplerst/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       73 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2simplerst/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     4528 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2simplerst/data2simplerst.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      463 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/data2simplerst/row_includes_spans.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      135 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/exceptions.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.944433 dashtable2-1.4.8/dashtable/grid2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/grid2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3471 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/grid2data/grid2data.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.945433 dashtable2-1.4.8/dashtable/html2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1630 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/extract_spans.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2693 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/extract_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      483 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/find_unassigned_table_cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1058 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/get_html_column_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      454 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/get_html_row_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      586 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/headers_present.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1089 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/html2data.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.946432 dashtable2-1.4.8/dashtable/html2data/restructify/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1768 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/add_links.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.948433 dashtable2-1.4.8/dashtable/html2data/restructify/converters/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      619 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      350 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_a.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_b.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      486 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_blockquote.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      105 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_br.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_cite.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      312 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_dd.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      442 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_div.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      129 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_em.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      155 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_h1.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      160 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_h2.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_h3.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      151 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_i.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      288 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_img.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1201 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_li.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      368 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_p.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      272 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_strong.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_tt.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      771 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/process_tag.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1126 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2data/restructify/restructify.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1658 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2md.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2571 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/html2rst.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.949432 dashtable2-1.4.8/dashtable/simple2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/simple2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3651 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/simple2data/simple2data.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      512 2024-05-20 13:11:43.000000 dashtable2-1.4.8/dashtable/simple2data/truncate_empty_lines.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 19:48:23.950433 dashtable2-1.4.8/dashtable2.egg-info/
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1107 2024-05-20 19:48:23.000000 dashtable2-1.4.8/dashtable2.egg-info/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3087 2024-05-20 19:48:23.000000 dashtable2-1.4.8/dashtable2.egg-info/SOURCES.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-05-20 19:48:23.000000 dashtable2-1.4.8/dashtable2.egg-info/dependency_links.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       37 2024-05-20 19:48:23.000000 dashtable2-1.4.8/dashtable2.egg-info/requires.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       10 2024-05-20 19:48:23.000000 dashtable2-1.4.8/dashtable2.egg-info/top_level.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-05-20 19:48:23.950433 dashtable2-1.4.8/setup.cfg
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1488 2024-05-20 16:14:28.000000 dashtable2-1.4.8/setup.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.059308 dashtable2-1.4.9/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1068 2024-05-20 13:11:43.000000 dashtable2-1.4.9/LICENSE.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1107 2024-05-24 08:03:13.059308 dashtable2-1.4.9/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      480 2024-05-20 13:40:39.000000 dashtable2-1.4.9/README.md
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.050308 dashtable2-1.4.9/dashtable/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      418 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.051308 dashtable2-1.4.9/dashtable/dashutils/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      441 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1134 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/add_cushions.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      760 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/center_line.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3239 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/checks.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      326 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/ensure_table_strings.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      547 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/make_empty_table.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      798 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/make_span.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      436 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/dashutils/multis_2_mono.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3812 2024-05-24 08:00:51.000000 dashtable2-1.4.9/dashtable/dashutils/spans.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.051308 dashtable2-1.4.9/dashtable/data2md/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       29 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2md/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1886 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2md/data2md.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      546 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2md/get_column_width.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.052308 dashtable2-1.4.9/dashtable/data2rst/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       31 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.053308 dashtable2-1.4.9/dashtable/data2rst/cell/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      296 2024-05-20 18:22:16.000000 dashtable2-1.4.9/dashtable/data2rst/cell/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3918 2024-05-24 07:44:26.000000 dashtable2-1.4.9/dashtable/data2rst/cell/cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1291 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/cell/center_cell_text.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/cell/get_longest_line_length.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      203 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/cell/is_only.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     4794 2024-05-24 07:44:26.000000 dashtable2-1.4.9/dashtable/data2rst/cell/merge.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1796 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/cell/v_center_cell_text.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3769 2024-05-24 08:00:51.000000 dashtable2-1.4.9/dashtable/data2rst/data2rst.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2085 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/get_output_column_widths.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1558 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/get_output_row_heights.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1867 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2rst/make_cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)    13431 2024-05-24 07:44:26.000000 dashtable2-1.4.9/dashtable/data2rst/merge_all_cells.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      931 2024-05-24 08:00:51.000000 dashtable2-1.4.9/dashtable/data2rst/table_cells_2_spans.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.053308 dashtable2-1.4.9/dashtable/data2simplerst/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       73 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2simplerst/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     4528 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2simplerst/data2simplerst.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      463 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/data2simplerst/row_includes_spans.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      135 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/exceptions.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.054308 dashtable2-1.4.9/dashtable/grid2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/grid2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3471 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/grid2data/grid2data.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.055308 dashtable2-1.4.9/dashtable/html2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1630 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/extract_spans.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2693 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/extract_table.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      483 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/find_unassigned_table_cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1058 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/get_html_column_count.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      454 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/get_html_row_count.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      586 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/headers_present.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1089 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/html2data.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.055308 dashtable2-1.4.9/dashtable/html2data/restructify/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1768 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/add_links.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.058308 dashtable2-1.4.9/dashtable/html2data/restructify/converters/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      619 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      350 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_a.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_b.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      486 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_blockquote.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      105 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_br.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_cite.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      312 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_dd.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      442 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_div.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      129 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_em.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      155 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_h1.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      160 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_h2.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_h3.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      151 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_i.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      288 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_img.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1201 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_li.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      368 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_p.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      272 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_strong.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_tt.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      771 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/process_tag.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1126 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2data/restructify/restructify.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1658 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2md.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2571 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/html2rst.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.058308 dashtable2-1.4.9/dashtable/simple2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/simple2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3651 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/simple2data/simple2data.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      512 2024-05-20 13:11:43.000000 dashtable2-1.4.9/dashtable/simple2data/truncate_empty_lines.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-24 08:03:13.059308 dashtable2-1.4.9/dashtable2.egg-info/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1107 2024-05-24 08:03:12.000000 dashtable2-1.4.9/dashtable2.egg-info/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3087 2024-05-24 08:03:13.000000 dashtable2-1.4.9/dashtable2.egg-info/SOURCES.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-05-24 08:03:12.000000 dashtable2-1.4.9/dashtable2.egg-info/dependency_links.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       37 2024-05-24 08:03:12.000000 dashtable2-1.4.9/dashtable2.egg-info/requires.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       10 2024-05-24 08:03:12.000000 dashtable2-1.4.9/dashtable2.egg-info/top_level.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-05-24 08:03:13.059308 dashtable2-1.4.9/setup.cfg
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1488 2024-05-20 16:14:28.000000 dashtable2-1.4.9/setup.py
```

### Comparing `dashtable2-1.4.8/LICENSE.txt` & `dashtable2-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/PKG-INFO` & `dashtable2-1.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashtable2
-Version: 1.4.8
+Version: 1.4.9
 Summary: A library for converting a HTML tables into ASCII tables, rowspan and colspan allowed!
 Home-page: https://github.com/PasaOpasen/dashtable2
 Author: doakey3 & gustavklopp & pasaopasen
 Author-email: qtckpuhdsa@gmail.com
 License: MIT
 Keywords: text table,conversion,documentation
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dashtable2-1.4.8/dashtable/dashutils/add_cushions.py` & `dashtable2-1.4.9/dashtable/dashutils/add_cushions.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/dashutils/center_line.py` & `dashtable2-1.4.9/dashtable/dashutils/center_line.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/dashutils/checks.py` & `dashtable2-1.4.9/dashtable/dashutils/checks.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/dashutils/make_empty_table.py` & `dashtable2-1.4.9/dashtable/dashutils/make_empty_table.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/dashutils/make_span.py` & `dashtable2-1.4.9/dashtable/dashutils/make_span.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/dashutils/spans.py` & `dashtable2-1.4.9/dashtable/dashutils/spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-def get_span(spans, row, column):
+def get_span(spans, row: int, column: int):
     """
     Gets the span containing the [row, column] pair
 
     Parameters
     ----------
     spans : list of lists of lists
         A list containing spans, which are lists of [row, column] pairs
         that define where a span is inside a table.
+    row :
+    column :
 
     Returns
     -------
     span : list of lists
         A span containing the [row, column] pair
     """
-    for i in range(len(spans)):
-        if [row, column] in spans[i]:
-            return spans[i]
+    p = (row, column)
+    for sps in spans:
+        if p in sps:
+            return sps
 
     return None
 
 
 def get_longest_line_length(text):
     """Get the length longest line in a paragraph"""
     lines = text.split("\n")
```

### Comparing `dashtable2-1.4.8/dashtable/data2md/data2md.py` & `dashtable2-1.4.9/dashtable/data2md/data2md.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2md/get_column_width.py` & `dashtable2-1.4.9/dashtable/data2md/get_column_width.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2rst/cell/cell.py` & `dashtable2-1.4.9/dashtable/data2rst/cell/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+
+from typing import Tuple
+
 from .is_only import is_only
 
 
-class Cell():
+class Cell:
     """
     Holds the text and data for an rst text cell
     """
     def __init__(self, text, row, column, row_count, column_count):
         """
         Initializes the Cell class
 
@@ -140,10 +143,18 @@
         bottom_line = self.text.split('\n')[-1]
 
         if is_only(bottom_line, ['+', '=']):
             return True
 
         return False
 
+    @property
+    def left_top_right_bottom(self) -> Tuple[int, int, int, int]:
+        left = self.column
+        top = self.row
+        right = left + self.column_count
+        bottom = top + self.row_count
+        return left, top, right, bottom
+
     def __lt__(self, other):
         """For sorting instances of this class."""
         return [self.row, self.column] < [other.row, other.column]
```

### Comparing `dashtable2-1.4.8/dashtable/data2rst/cell/center_cell_text.py` & `dashtable2-1.4.9/dashtable/data2rst/cell/center_cell_text.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2rst/cell/v_center_cell_text.py` & `dashtable2-1.4.9/dashtable/data2rst/cell/v_center_cell_text.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2rst/data2rst.py` & `dashtable2-1.4.9/dashtable/data2rst/data2rst.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,18 @@
     table = copy.deepcopy(table)
 
     table_ok = check_table(table)
     if not table_ok == "":
         return "ERROR: " + table_ok
 
     spans = spans or []
+    spans: List[List[Tuple[int, int]]] = [
+        list(map(tuple, pairs))
+        for pairs in spans
+    ]
     for span in spans:
         span_ok = check_span(span, table)
         if not span_ok == "":
             return "ERROR: " + span_ok
 
     table = ensure_table_strings(table)
     table = add_cushions(table)
```

### Comparing `dashtable2-1.4.8/dashtable/data2rst/get_output_column_widths.py` & `dashtable2-1.4.9/dashtable/data2rst/get_output_column_widths.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2rst/get_output_row_heights.py` & `dashtable2-1.4.9/dashtable/data2rst/get_output_row_heights.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2rst/make_cell.py` & `dashtable2-1.4.9/dashtable/data2rst/make_cell.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/data2rst/table_cells_2_spans.py` & `dashtable2-1.4.9/dashtable/data2rst/table_cells_2_spans.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     """
     new_spans = []
     for row in range(len(table)):
         for column in range(len(table[row])):
             span = get_span(spans, row, column)
 
             if not span:
-                new_spans.append([[row, column]])
+                new_spans.append([(row, column)])
 
     new_spans.extend(spans)
-    new_spans = list(sorted(new_spans))
+    new_spans = sorted(new_spans)
 
     return new_spans
```

### Comparing `dashtable2-1.4.8/dashtable/data2simplerst/data2simplerst.py` & `dashtable2-1.4.9/dashtable/data2simplerst/data2simplerst.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/grid2data/grid2data.py` & `dashtable2-1.4.9/dashtable/grid2data/grid2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/extract_spans.py` & `dashtable2-1.4.9/dashtable/html2data/extract_spans.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/extract_table.py` & `dashtable2-1.4.9/dashtable/html2data/extract_table.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/get_html_column_count.py` & `dashtable2-1.4.9/dashtable/html2data/get_html_column_count.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/headers_present.py` & `dashtable2-1.4.9/dashtable/html2data/headers_present.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/html2data.py` & `dashtable2-1.4.9/dashtable/html2data/html2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/restructify/add_links.py` & `dashtable2-1.4.9/dashtable/html2data/restructify/add_links.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/restructify/converters/__init__.py` & `dashtable2-1.4.9/dashtable/html2data/restructify/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/restructify/converters/convert_li.py` & `dashtable2-1.4.9/dashtable/html2data/restructify/converters/convert_li.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/restructify/process_tag.py` & `dashtable2-1.4.9/dashtable/html2data/restructify/process_tag.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2data/restructify/restructify.py` & `dashtable2-1.4.9/dashtable/html2data/restructify/restructify.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2md.py` & `dashtable2-1.4.9/dashtable/html2md.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/html2rst.py` & `dashtable2-1.4.9/dashtable/html2rst.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/simple2data/simple2data.py` & `dashtable2-1.4.9/dashtable/simple2data/simple2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable/simple2data/truncate_empty_lines.py` & `dashtable2-1.4.9/dashtable/simple2data/truncate_empty_lines.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/dashtable2.egg-info/PKG-INFO` & `dashtable2-1.4.9/dashtable2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashtable2
-Version: 1.4.8
+Version: 1.4.9
 Summary: A library for converting a HTML tables into ASCII tables, rowspan and colspan allowed!
 Home-page: https://github.com/PasaOpasen/dashtable2
 Author: doakey3 & gustavklopp & pasaopasen
 Author-email: qtckpuhdsa@gmail.com
 License: MIT
 Keywords: text table,conversion,documentation
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dashtable2-1.4.8/dashtable2.egg-info/SOURCES.txt` & `dashtable2-1.4.9/dashtable2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.8/setup.py` & `dashtable2-1.4.9/setup.py`

 * *Files identical despite different names*

