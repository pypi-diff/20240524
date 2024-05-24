# Comparing `tmp/mindee-4.7.0.tar.gz` & `tmp/mindee-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-4.7.0.tar", last modified: Tue May 21 08:46:19 2024, max compression
+gzip compressed data, was "mindee-4.8.0.tar", last modified: Fri May 24 14:45:30 2024, max compression
```

## Comparing `mindee-4.7.0.tar` & `mindee-4.8.0.tar`

### file list

```diff
@@ -1,340 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 08:45:58.000000 mindee-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-21 08:46:19.922949 mindee-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-21 08:45:58.000000 mindee-4.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.874949 mindee-4.7.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/error/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/geometry_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/mimetype_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/mindee_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/mindee_http_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/polygon_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/quadrilateral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/mindee_http/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/base_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/mindee_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/response_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.882949 mindee-4.7.0/mindee/parsing/common/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/async_predict_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.882949 mindee-4.7.0/mindee/parsing/common/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/extras/cropper_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/extras/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/feedback_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.882949 mindee-4.7.0/mindee/parsing/common/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/mvision_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr_word.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/predict_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/product.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/string_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/summary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/parsing/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/line_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/parsing/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/generated/generated_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/generated/generated_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/parsing/standard/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/position.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/product/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/product/barcode_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/barcode_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/cropper/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/cropper_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/cropper_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/custom/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/custom_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/custom_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/eu/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/eu/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/financial_document/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/financial_document_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/financial_document_v1_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/petrol_receipt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/international_id/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v2_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/invoice_v4_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/invoice_v4_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/material_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/material_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/multi_receipts_detector/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/multi_receipts_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/passport/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/passport/passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/passport/passport_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/receipt/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v4_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v5_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v5_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/resume/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_education.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_professional_experience.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_social_networks_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/us/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/mindee/product/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/mindee/product/us/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/mindee/product/us/w9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/w9_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/w9_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/w9_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:46:04.000000 mindee-4.7.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 08:45:58.000000 mindee-4.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-21 08:46:19.926950 mindee-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 08:45:58.000000 mindee-4.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/barcode_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/barcode_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/cropper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/cropper/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/cropper/test_cropper_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/eu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/eu/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/driver_license/test_driver_license_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/financial_document/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/financial_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/financial_document/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/financial_document/test_financial_document_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/international_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/international_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/international_id/test_international_id_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/international_id/test_international_id_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/invoice/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/invoice/test_invoice_v4_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/material_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/material_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/material_certificate/test_material_certificate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/multi_receipts_detector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/multi_receipts_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/passport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/passport/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/passport/test_passport_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/proof_of_address/test_proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/receipt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v4_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v5_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/resume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/resume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/resume/test_resume_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/us/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/tests/product/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/tests/product/us/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/tests/product/us/w9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/w9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/w9/test_w9_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/w9/test_w9_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.390962 mindee-4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 14:45:12.000000 mindee-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-24 14:45:30.390962 mindee-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-24 14:45:12.000000 mindee-4.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.342962 mindee-4.8.0/mindee/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19798 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.346962 mindee-4.8.0/mindee/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/error/geometry_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/error/mimetype_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/error/mindee_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/error/mindee_http_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.346962 mindee-4.8.0/mindee/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/polygon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/geometry/quadrilateral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.346962 mindee-4.8.0/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/input/local_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.350962 mindee-4.8.0/mindee/mindee_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/mindee_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/mindee_http/base_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/mindee_http/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/mindee_http/mindee_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/mindee_http/response_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.350962 mindee-4.8.0/mindee/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.350962 mindee-4.8.0/mindee/parsing/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/async_predict_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.350962 mindee-4.8.0/mindee/parsing/common/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/extras/cropper_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/extras/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/feedback_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.354962 mindee-4.8.0/mindee/parsing/common/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/ocr/mvision_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/ocr/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/ocr/ocr_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/ocr/ocr_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/ocr/ocr_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/predict_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/string_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/common/summary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.354962 mindee-4.8.0/mindee/parsing/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/custom/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/custom/line_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/custom/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.354962 mindee-4.8.0/mindee/parsing/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/generated/generated_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/generated/generated_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.354962 mindee-4.8.0/mindee/parsing/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/parsing/standard/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.354962 mindee-4.8.0/mindee/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/barcode_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/barcode_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/barcode_reader/barcode_reader_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/barcode_reader/barcode_reader_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/cropper/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/cropper/cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/cropper/cropper_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/cropper/cropper_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/custom/custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/custom/custom_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/custom/custom_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/eu/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/driver_license/driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/driver_license/driver_license_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/driver_license/driver_license_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/license_plate/license_plate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/eu/license_plate/license_plate_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/financial_document/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/financial_document/financial_document_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/financial_document/financial_document_v1_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.358962 mindee-4.8.0/mindee/product/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.362962 mindee-4.8.0/mindee/product/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.362962 mindee-4.8.0/mindee/product/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/carte_grise/carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.362962 mindee-4.8.0/mindee/product/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.362962 mindee-4.8.0/mindee/product/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/id_card_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/id_card_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/id_card_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/id_card_v2_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/id_card/id_card_v2_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.362962 mindee-4.8.0/mindee/product/fr/petrol_receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/petrol_receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.366962 mindee-4.8.0/mindee/product/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/generated/generated_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/generated/generated_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/generated/generated_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/generated/generated_v1_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.366962 mindee-4.8.0/mindee/product/international_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/international_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/international_id/international_id_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/international_id/international_id_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/international_id/international_id_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/international_id/international_id_v2_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.366962 mindee-4.8.0/mindee/product/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice/invoice_v4_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice/invoice_v4_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.366962 mindee-4.8.0/mindee/product/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice_splitter/invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.366962 mindee-4.8.0/mindee/product/material_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/material_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/material_certificate/material_certificate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/material_certificate/material_certificate_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.370962 mindee-4.8.0/mindee/product/multi_receipts_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/multi_receipts_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.370962 mindee-4.8.0/mindee/product/passport/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/passport/passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/passport/passport_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.370962 mindee-4.8.0/mindee/product/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/proof_of_address/proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/proof_of_address/proof_of_address_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.370962 mindee-4.8.0/mindee/product/receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/receipt/receipt_v4_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/receipt/receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/receipt/receipt_v5_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/receipt/receipt_v5_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.370962 mindee-4.8.0/mindee/product/resume/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1_education.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1_professional_experience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/resume/resume_v1_social_networks_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.370962 mindee-4.8.0/mindee/product/us/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.374962 mindee-4.8.0/mindee/product/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/bank_check/bank_check_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/bank_check/bank_check_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.374962 mindee-4.8.0/mindee/product/us/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/driver_license/driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/driver_license/driver_license_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/driver_license/driver_license_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.374962 mindee-4.8.0/mindee/product/us/w9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/w9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/w9/w9_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/w9/w9_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/product/us/w9/w9_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-24 14:45:12.000000 mindee-4.8.0/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-24 14:45:30.000000 mindee-4.8.0/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-24 14:45:30.000000 mindee-4.8.0/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:45:30.000000 mindee-4.8.0/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 14:45:30.000000 mindee-4.8.0/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:45:16.000000 mindee-4.8.0/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-24 14:45:30.000000 mindee-4.8.0/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 14:45:30.000000 mindee-4.8.0/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-24 14:45:12.000000 mindee-4.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-24 14:45:30.390962 mindee-4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-24 14:45:12.000000 mindee-4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.374962 mindee-4.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/fields/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/barcode_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/barcode_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/barcode_reader/test_barcode_reader_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/cropper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/cropper/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/cropper/test_cropper_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/eu/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/eu/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/eu/driver_license/test_driver_license_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/eu/license_plate/test_license_plate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/financial_document/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/financial_document/test_financial_document_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.378962 mindee-4.8.0/tests/product/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/carte_grise/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/id_card/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/id_card/test_id_card_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/id_card/test_id_card_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/fr/id_card/test_id_card_v2_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/international_id/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/international_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/international_id/test_international_id_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/international_id/test_international_id_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/invoice/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/invoice/test_invoice_v4_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/material_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/material_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/material_certificate/test_material_certificate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.382962 mindee-4.8.0/tests/product/multi_receipts_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/multi_receipts_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/passport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/passport/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/passport/test_passport_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/proof_of_address/test_proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/receipt/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/receipt/test_receipt_v4_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/receipt/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/receipt/test_receipt_v5_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/resume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/resume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/resume/test_resume_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/us/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/bank_check/test_bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/bank_check/test_bank_check_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/us/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/driver_license/test_driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/driver_license/test_driver_license_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:30.386962 mindee-4.8.0/tests/product/us/w9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/w9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/w9/test_w9_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/product/us/w9/test_w9_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-24 14:45:12.000000 mindee-4.8.0/tests/test_pkg_versions.py
```

### Comparing `mindee-4.7.0/LICENSE` & `mindee-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/PKG-INFO` & `mindee-4.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 4.7.0
+Version: 4.8.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: opensource@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
@@ -20,16 +20,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pikepdf~=8.6; python_version >= "3.8"
-Requires-Dist: pikepdf==6.2.9; python_version < "3.8"
+Requires-Dist: pypdfium2<5,>=4.0
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests~=2.31
 Provides-Extra: dev
 Requires-Dist: pylint==2.17.7; extra == "dev"
 Requires-Dist: setuptools==51.3.3; extra == "dev"
 Requires-Dist: pre-commit~=2.21.0; extra == "dev"
 Requires-Dist: types-pytz~=2023.3; extra == "dev"
```

### Comparing `mindee-4.7.0/README.md` & `mindee-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/cli.py` & `mindee-4.8.0/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/client.py` & `mindee-4.8.0/mindee/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from time import sleep
 from typing import BinaryIO, Dict, Optional, Type, Union
 
 from mindee.error.mindee_error import MindeeClientError, MindeeError
 from mindee.error.mindee_http_error import handle_error
+from mindee.input import LocalResponse
 from mindee.input.page_options import PageOptions
 from mindee.input.sources import (
     Base64Input,
     BytesInput,
     FileInput,
     LocalInputSource,
     PathInput,
@@ -174,14 +175,31 @@
             input_source,
             endpoint,
             include_words,
             close_file,
             cropper,
         )
 
+    def load_prediction(
+        self, product_class: Type[Inference], local_response: LocalResponse
+    ) -> Union[AsyncPredictResponse, PredictResponse]:
+        """
+        Load a prediction.
+
+        :param product_class: Class of the product to use.
+        :param local_response: Local response to load.
+        :return: A valid prediction.
+        """
+        try:
+            if local_response.as_dict.get("job"):
+                return AsyncPredictResponse(product_class, local_response.as_dict)
+            return PredictResponse(product_class, local_response.as_dict)
+        except KeyError as exc:
+            raise MindeeError("No prediction found in local response.") from exc
+
     def parse_queued(
         self,
         product_class: Type[Inference],
         queue_id: str,
         endpoint: Optional[Endpoint] = None,
     ) -> AsyncPredictResponse:
         """
```

### Comparing `mindee-4.7.0/mindee/error/mindee_error.py` & `mindee-4.8.0/mindee/error/mindee_error.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/error/mindee_http_error.py` & `mindee-4.8.0/mindee/error/mindee_http_error.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/geometry/__init__.py` & `mindee-4.8.0/mindee/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/geometry/bbox.py` & `mindee-4.8.0/mindee/geometry/bbox.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/geometry/minmax.py` & `mindee-4.8.0/mindee/geometry/minmax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/geometry/polygon.py` & `mindee-4.8.0/mindee/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/geometry/polygon_utils.py` & `mindee-4.8.0/mindee/geometry/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/geometry/quadrilateral.py` & `mindee-4.8.0/mindee/geometry/quadrilateral.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/input/page_options.py` & `mindee-4.8.0/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/input/sources.py` & `mindee-4.8.0/mindee/input/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import mimetypes
 import os
 import tempfile
 from enum import Enum
 from pathlib import Path
 from typing import BinaryIO, Optional, Sequence, Tuple, Union
 
-import pikepdf
+import pypdfium2 as pdfium
 
 from mindee.error.mimetype_error import MimeTypeError
 from mindee.error.mindee_error import MindeeError, MindeeSourceError
 from mindee.input.page_options import KEEP_ONLY, REMOVE
 from mindee.logger import logger
 
 mimetypes.add_type("image/heic", ".heic")
@@ -113,16 +113,16 @@
     def count_doc_pages(self) -> int:
         """
         Count the pages in the PDF.
 
         :return: the number of pages.
         """
         self.file_object.seek(0)
-        with pikepdf.open(self.file_object) as pdf:
-            return len(pdf.pages)
+        pdf = pdfium.PdfDocument(self.file_object)
+        return len(pdf)
 
     def process_pdf(
         self,
         behavior: str,
         on_min_pages: int,
         page_indexes: Sequence,
     ) -> None:
@@ -159,48 +159,34 @@
         """
         Create a new PDF from pages and set it to ``file_object``.
 
         :param page_numbers: List of pages number to use for merging in the original PDF.
         :return: None
         """
         self.file_object.seek(0)
-        new_pdf = pikepdf.Pdf.new()
-        with pikepdf.open(self.file_object) as pdf:
-            for page_id in page_numbers:
-                page = pdf.pages[page_id]
-                new_pdf.pages.append(page)
+        new_pdf = pdfium.PdfDocument.new()
+        pdf = pdfium.PdfDocument(self.file_object)
+        new_pdf.import_pages(pdf, list(page_numbers))
         self.file_object.close()
-        self.file_object = io.BytesIO()
-        new_pdf.save(self.file_object)
+        bytes_io = io.BytesIO()
+        new_pdf.save(bytes_io)
+        self.file_object = bytes_io
 
     def is_pdf_empty(self) -> bool:
         """
         Check if the PDF is empty.
 
         :return: ``True`` if the PDF is empty
         """
         self.file_object.seek(0)
-        with pikepdf.open(self.file_object) as pdf:
-            for page in pdf.pages:
-                # mypy incorrectly identifies the "/Length" key's value as
-                # an object rather than an int.
-                try:
-                    total_size = page["/Contents"]["/Length"]
-                except ValueError:
-                    total_size = 0  # type: ignore
-                    for content in page["/Contents"]:  # type: ignore
-                        total_size += content["/Length"]
-                has_data = total_size > 1000  # type: ignore
-
-                has_font = "/Font" in page["/Resources"].keys()
-                has_xobj = "/XObject" in page["/Resources"].keys()
-
-                if has_font or has_xobj or has_data:
-                    return False
-            return True
+        pdf = pdfium.PdfDocument(self.file_object)
+        for page in pdf:
+            for _ in page.get_objects():
+                return False
+        return True
 
     def read_contents(self, close_file: bool) -> Tuple[str, bytes]:
         """
         Read the contents of the input file.
 
         :param close_file: whether to close the file after reading
         :return: a Tuple with the file name and binary data
```

### Comparing `mindee-4.7.0/mindee/mindee_http/endpoint.py` & `mindee-4.8.0/mindee/mindee_http/endpoint.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/mindee_http/mindee_api.py` & `mindee-4.8.0/mindee/mindee_http/mindee_api.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/mindee_http/response_validation.py` & `mindee-4.8.0/mindee/mindee_http/response_validation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/__init__.py` & `mindee-4.8.0/mindee/parsing/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/api_request.py` & `mindee-4.8.0/mindee/parsing/common/api_request.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/api_response.py` & `mindee-4.8.0/mindee/parsing/common/api_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/async_predict_response.py` & `mindee-4.8.0/mindee/parsing/common/async_predict_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/document.py` & `mindee-4.8.0/mindee/parsing/common/document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/extras/cropper_extra.py` & `mindee-4.8.0/mindee/parsing/common/extras/cropper_extra.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/extras/extras.py` & `mindee-4.8.0/mindee/parsing/common/extras/extras.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/inference.py` & `mindee-4.8.0/mindee/parsing/common/inference.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/job.py` & `mindee-4.8.0/mindee/parsing/common/job.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/ocr/ocr_page.py` & `mindee-4.8.0/mindee/parsing/common/ocr/ocr_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/ocr/ocr_word.py` & `mindee-4.8.0/mindee/parsing/common/ocr/ocr_word.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/orientation.py` & `mindee-4.8.0/mindee/parsing/common/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/page.py` & `mindee-4.8.0/mindee/parsing/common/page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/predict_response.py` & `mindee-4.8.0/mindee/parsing/common/predict_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/prediction.py` & `mindee-4.8.0/mindee/parsing/common/prediction.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/common/summary_helper.py` & `mindee-4.8.0/mindee/parsing/common/summary_helper.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/custom/line_items.py` & `mindee-4.8.0/mindee/parsing/custom/line_items.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/custom/list.py` & `mindee-4.8.0/mindee/parsing/custom/list.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/generated/generated_list.py` & `mindee-4.8.0/mindee/parsing/generated/generated_list.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/generated/generated_object.py` & `mindee-4.8.0/mindee/parsing/generated/generated_object.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/__init__.py` & `mindee-4.8.0/mindee/parsing/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/amount.py` & `mindee-4.8.0/mindee/parsing/standard/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/base.py` & `mindee-4.8.0/mindee/parsing/standard/base.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/classification.py` & `mindee-4.8.0/mindee/parsing/standard/classification.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/company_registration.py` & `mindee-4.8.0/mindee/parsing/standard/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/date.py` & `mindee-4.8.0/mindee/parsing/standard/date.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/locale.py` & `mindee-4.8.0/mindee/parsing/standard/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/payment_details.py` & `mindee-4.8.0/mindee/parsing/standard/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/position.py` & `mindee-4.8.0/mindee/parsing/standard/position.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/tax.py` & `mindee-4.8.0/mindee/parsing/standard/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/parsing/standard/text.py` & `mindee-4.8.0/mindee/parsing/standard/text.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/__init__.py` & `mindee-4.8.0/mindee/product/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1.py` & `mindee-4.8.0/mindee/product/barcode_reader/barcode_reader_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1_document.py` & `mindee-4.8.0/mindee/product/barcode_reader/barcode_reader_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/cropper/cropper_v1.py` & `mindee-4.8.0/mindee/product/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/cropper/cropper_v1_page.py` & `mindee-4.8.0/mindee/product/cropper/cropper_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/custom/custom_v1.py` & `mindee-4.8.0/mindee/product/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/custom/custom_v1_document.py` & `mindee-4.8.0/mindee/product/custom/custom_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/custom/custom_v1_page.py` & `mindee-4.8.0/mindee/product/custom/custom_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1.py` & `mindee-4.8.0/mindee/product/eu/driver_license/driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_document.py` & `mindee-4.8.0/mindee/product/eu/driver_license/driver_license_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_page.py` & `mindee-4.8.0/mindee/product/eu/driver_license/driver_license_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1.py` & `mindee-4.8.0/mindee/product/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1_document.py` & `mindee-4.8.0/mindee/product/eu/license_plate/license_plate_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/financial_document/financial_document_v1.py` & `mindee-4.8.0/mindee/product/financial_document/financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/financial_document/financial_document_v1_document.py` & `mindee-4.8.0/mindee/product/financial_document/financial_document_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/financial_document/financial_document_v1_line_item.py` & `mindee-4.8.0/mindee/product/financial_document/financial_document_v1_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/__init__.py` & `mindee-4.8.0/mindee/product/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py` & `mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py` & `mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py` & `mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py` & `mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py` & `mindee-4.8.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1.py` & `mindee-4.8.0/mindee/product/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py` & `mindee-4.8.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py` & `mindee-4.8.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py` & `mindee-4.8.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/id_card/id_card_v1.py` & `mindee-4.8.0/mindee/product/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_document.py` & `mindee-4.8.0/mindee/product/fr/id_card/id_card_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_page.py` & `mindee-4.8.0/mindee/product/fr/id_card/id_card_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/id_card/id_card_v2.py` & `mindee-4.8.0/mindee/product/fr/id_card/id_card_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_document.py` & `mindee-4.8.0/mindee/product/fr/id_card/id_card_v2_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_page.py` & `mindee-4.8.0/mindee/product/fr/id_card/id_card_v2_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py` & `mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py` & `mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py` & `mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py` & `mindee-4.8.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/generated/generated_v1.py` & `mindee-4.8.0/mindee/product/generated/generated_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/generated/generated_v1_document.py` & `mindee-4.8.0/mindee/product/generated/generated_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/generated/generated_v1_page.py` & `mindee-4.8.0/mindee/product/generated/generated_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/generated/generated_v1_prediction.py` & `mindee-4.8.0/mindee/product/generated/generated_v1_prediction.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/international_id/international_id_v1.py` & `mindee-4.8.0/mindee/product/international_id/international_id_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/international_id/international_id_v1_document.py` & `mindee-4.8.0/mindee/product/international_id/international_id_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/international_id/international_id_v2.py` & `mindee-4.8.0/mindee/product/international_id/international_id_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/international_id/international_id_v2_document.py` & `mindee-4.8.0/mindee/product/international_id/international_id_v2_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/invoice/invoice_v4.py` & `mindee-4.8.0/mindee/product/invoice/invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/invoice/invoice_v4_document.py` & `mindee-4.8.0/mindee/product/invoice/invoice_v4_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/invoice/invoice_v4_line_item.py` & `mindee-4.8.0/mindee/product/invoice/invoice_v4_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1.py` & `mindee-4.8.0/mindee/product/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py` & `mindee-4.8.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py` & `mindee-4.8.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1.py` & `mindee-4.8.0/mindee/product/material_certificate/material_certificate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1_document.py` & `mindee-4.8.0/mindee/product/material_certificate/material_certificate_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py` & `mindee-4.8.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py` & `mindee-4.8.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/passport/passport_v1.py` & `mindee-4.8.0/mindee/product/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/passport/passport_v1_document.py` & `mindee-4.8.0/mindee/product/passport/passport_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1.py` & `mindee-4.8.0/mindee/product/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1_document.py` & `mindee-4.8.0/mindee/product/proof_of_address/proof_of_address_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/receipt/receipt_v4.py` & `mindee-4.8.0/mindee/product/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/receipt/receipt_v4_document.py` & `mindee-4.8.0/mindee/product/receipt/receipt_v4_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/receipt/receipt_v5.py` & `mindee-4.8.0/mindee/product/receipt/receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/receipt/receipt_v5_document.py` & `mindee-4.8.0/mindee/product/receipt/receipt_v5_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/receipt/receipt_v5_line_item.py` & `mindee-4.8.0/mindee/product/receipt/receipt_v5_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/__init__.py` & `mindee-4.8.0/mindee/product/resume/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1.py` & `mindee-4.8.0/mindee/product/resume/resume_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1_certificate.py` & `mindee-4.8.0/mindee/product/resume/resume_v1_certificate.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1_document.py` & `mindee-4.8.0/mindee/product/resume/resume_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1_education.py` & `mindee-4.8.0/mindee/product/resume/resume_v1_education.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1_language.py` & `mindee-4.8.0/mindee/product/resume/resume_v1_language.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1_professional_experience.py` & `mindee-4.8.0/mindee/product/resume/resume_v1_professional_experience.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/resume/resume_v1_social_networks_url.py` & `mindee-4.8.0/mindee/product/resume/resume_v1_social_networks_url.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/__init__.py` & `mindee-4.8.0/mindee/product/us/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1.py` & `mindee-4.8.0/mindee/product/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_document.py` & `mindee-4.8.0/mindee/product/us/bank_check/bank_check_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_page.py` & `mindee-4.8.0/mindee/product/us/bank_check/bank_check_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1.py` & `mindee-4.8.0/mindee/product/us/driver_license/driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_document.py` & `mindee-4.8.0/mindee/product/us/driver_license/driver_license_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_page.py` & `mindee-4.8.0/mindee/product/us/driver_license/driver_license_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/w9/w9_v1.py` & `mindee-4.8.0/mindee/product/us/w9/w9_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/product/us/w9/w9_v1_page.py` & `mindee-4.8.0/mindee/product/us/w9/w9_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee/versions.py` & `mindee-4.8.0/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/mindee.egg-info/PKG-INFO` & `mindee-4.8.0/mindee.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 4.7.0
+Version: 4.8.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: opensource@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
@@ -20,16 +20,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pikepdf~=8.6; python_version >= "3.8"
-Requires-Dist: pikepdf==6.2.9; python_version < "3.8"
+Requires-Dist: pypdfium2<5,>=4.0
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests~=2.31
 Provides-Extra: dev
 Requires-Dist: pylint==2.17.7; extra == "dev"
 Requires-Dist: setuptools==51.3.3; extra == "dev"
 Requires-Dist: pre-commit~=2.21.0; extra == "dev"
 Requires-Dist: types-pytz~=2023.3; extra == "dev"
```

### Comparing `mindee-4.7.0/mindee.egg-info/SOURCES.txt` & `mindee-4.8.0/mindee.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 mindee/geometry/bbox.py
 mindee/geometry/minmax.py
 mindee/geometry/point.py
 mindee/geometry/polygon.py
 mindee/geometry/polygon_utils.py
 mindee/geometry/quadrilateral.py
 mindee/input/__init__.py
+mindee/input/local_response.py
 mindee/input/page_options.py
 mindee/input/sources.py
 mindee/mindee_http/__init__.py
 mindee/mindee_http/base_endpoint.py
 mindee/mindee_http/endpoint.py
 mindee/mindee_http/mindee_api.py
 mindee/mindee_http/response_validation.py
```

### Comparing `mindee-4.7.0/pyproject.toml` & `mindee-4.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -18,21 +18,25 @@
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 strict_equality = true
 warn_unused_ignores = true
 warn_unreachable = true
 
+[[tool.mypy.overrides]]
+module = "pypdfium2.*"
+ignore_missing_imports = true
+
 [tool.pylic]
 safe_licenses = [
   "Apache Software License",
   "MIT License",
   "Mozilla Public License 2.0 (MPL 2.0)",
   "BSD License",
-  "Historical Permission Notice and Disclaimer (HPND)",
+  "(Apache-2.0 OR BSD-3-Clause) AND LicenseRef-PdfiumThirdParty"
 ]
 
 [tool.pytest.ini_options]
 addopts = "--pyargs --cov mindee --cov-report term:skip-covered --cov-report term-missing -m 'not regression'"
 python_files = "test*.py"
 junit_family = "xunit2"
 markers = [
```

### Comparing `mindee-4.7.0/setup.cfg` & `mindee-4.8.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
-	pikepdf~=8.6;python_version>="3.8"
-	pikepdf==6.2.9;python_version<"3.8"
+	pypdfium2>=4.0,<5
 	pytz>=2023.3
 	requests~=2.31
 
 [options.entry_points]
 console_scripts = 
 	mindee-cli = mindee.cli:main
```

### Comparing `mindee-4.7.0/tests/fields/test_amount.py` & `mindee-4.8.0/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_date.py` & `mindee-4.8.0/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_field.py` & `mindee-4.8.0/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_locale.py` & `mindee-4.8.0/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_orientation.py` & `mindee-4.8.0/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_payment_details.py` & `mindee-4.8.0/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_position.py` & `mindee-4.8.0/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_tax.py` & `mindee-4.8.0/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/fields/test_text.py` & `mindee-4.8.0/tests/fields/test_text.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/__init__.py` & `mindee-4.8.0/tests/product/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1.py` & `mindee-4.8.0/tests/product/barcode_reader/test_barcode_reader_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py` & `mindee-4.8.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/cropper/test_cropper_v1.py` & `mindee-4.8.0/tests/product/cropper/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/cropper/test_cropper_v1_regression.py` & `mindee-4.8.0/tests/product/cropper/test_cropper_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/eu/driver_license/test_driver_license_v1.py` & `mindee-4.8.0/tests/product/eu/driver_license/test_driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1.py` & `mindee-4.8.0/tests/product/eu/license_plate/test_license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py` & `mindee-4.8.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/financial_document/test_financial_document_v1.py` & `mindee-4.8.0/tests/product/financial_document/test_financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/financial_document/test_financial_document_v1_regression.py` & `mindee-4.8.0/tests/product/financial_document/test_financial_document_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py` & `mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py` & `mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py` & `mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py` & `mindee-4.8.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1.py` & `mindee-4.8.0/tests/product/fr/carte_grise/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py` & `mindee-4.8.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py` & `mindee-4.8.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py` & `mindee-4.8.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1.py` & `mindee-4.8.0/tests/product/fr/id_card/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1_regression.py` & `mindee-4.8.0/tests/product/fr/id_card/test_id_card_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2.py` & `mindee-4.8.0/tests/product/fr/id_card/test_id_card_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2_regression.py` & `mindee-4.8.0/tests/product/fr/id_card/test_id_card_v2_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/international_id/test_international_id_v1.py` & `mindee-4.8.0/tests/product/international_id/test_international_id_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/international_id/test_international_id_v2.py` & `mindee-4.8.0/tests/product/international_id/test_international_id_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/invoice/test_invoice_v4.py` & `mindee-4.8.0/tests/product/invoice/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/invoice/test_invoice_v4_regression.py` & `mindee-4.8.0/tests/product/invoice/test_invoice_v4_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/material_certificate/test_material_certificate_v1.py` & `mindee-4.8.0/tests/product/material_certificate/test_material_certificate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py` & `mindee-4.8.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py` & `mindee-4.8.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/passport/test_passport_v1.py` & `mindee-4.8.0/tests/product/passport/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/passport/test_passport_v1_regression.py` & `mindee-4.8.0/tests/product/passport/test_passport_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/proof_of_address/test_proof_of_address_v1.py` & `mindee-4.8.0/tests/product/proof_of_address/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/receipt/test_receipt_v4.py` & `mindee-4.8.0/tests/product/receipt/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/receipt/test_receipt_v4_regression.py` & `mindee-4.8.0/tests/product/receipt/test_receipt_v4_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/receipt/test_receipt_v5.py` & `mindee-4.8.0/tests/product/receipt/test_receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/receipt/test_receipt_v5_regression.py` & `mindee-4.8.0/tests/product/receipt/test_receipt_v5_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/resume/test_resume_v1.py` & `mindee-4.8.0/tests/product/resume/test_resume_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1.py` & `mindee-4.8.0/tests/product/us/bank_check/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1_regression.py` & `mindee-4.8.0/tests/product/us/bank_check/test_bank_check_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1.py` & `mindee-4.8.0/tests/product/us/driver_license/test_driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1_regression.py` & `mindee-4.8.0/tests/product/us/driver_license/test_driver_license_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/us/w9/test_w9_v1.py` & `mindee-4.8.0/tests/product/us/w9/test_w9_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/product/us/w9/test_w9_v1_regression.py` & `mindee-4.8.0/tests/product/us/w9/test_w9_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/test_cli.py` & `mindee-4.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/test_geometry.py` & `mindee-4.8.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-4.7.0/tests/test_inputs.py` & `mindee-4.8.0/tests/test_inputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 from pathlib import Path
 
-import pikepdf
+import pypdfium2 as pdfium
 import pytest
 
 from mindee.error.mimetype_error import MimeTypeError
 from mindee.error.mindee_error import MindeeError, MindeeSourceError
 from mindee.input.page_options import KEEP_ONLY, REMOVE
 from mindee.input.sources import (
     Base64Input,
@@ -14,14 +14,15 @@
     PathInput,
     UrlInputSource,
 )
 from tests.product import PRODUCT_DATA_DIR
 
 FILE_TYPES_DIR = Path("./tests/data/file_types")
 
+
 #
 # PDF
 #
 
 
 def test_pdf_reconstruct_ok():
     input_obj = PathInput(FILE_TYPES_DIR / "pdf" / "multipage.pdf")
@@ -51,26 +52,27 @@
     input_obj = PathInput(FILE_TYPES_DIR / "pdf" / "multipage.pdf")
     assert input_obj.is_pdf() is True
     input_obj.process_pdf(
         behavior=KEEP_ONLY, on_min_pages=2, page_indexes=[0, -2, -1][:numb_pages]
     )
     assert input_obj.count_doc_pages() == numb_pages
 
-    # Each page in the PDF has a unique (and increasing) /Content /Length.
-    # We use this to make sure we have the correct pages
-    cut_pdf = pikepdf.open(input_obj.file_object)
-    with pikepdf.open(
-        FILE_TYPES_DIR / "pdf" / f"multipage_cut-{numb_pages}.pdf"
-    ) as pdf:
-        for idx, page in enumerate(pdf.pages):
-            assert (
-                page["/Contents"]["/Length"]
-                == cut_pdf.pages[idx]["/Contents"]["/Length"]
-            )
+    # Currently the least verbose way of comparing pages with pypdfium2
+    # I.e. each page is read & rendered as a rasterized image. These images are then compared as raw byte sequences.
+    cut_pdf = pdfium.PdfDocument(input_obj.file_object)
+    pdf = pdfium.PdfDocument(FILE_TYPES_DIR / "pdf" / f"multipage_cut-{numb_pages}.pdf")
+    for idx in range(len(pdf)):
+        pdf_page = pdf.get_page(idx)
+        pdf_page_render = pdfium.PdfPage.render(pdf_page)
+        cut_pdf_page = cut_pdf.get_page(idx)
+        cut_pdf_page_render = pdfium.PdfPage.render(cut_pdf_page)
+
+        assert bytes(pdf_page_render.buffer) == bytes(cut_pdf_page_render.buffer)
     cut_pdf.close()
+    pdf.close()
 
 
 def test_pdf_keep_5_first_pages():
     input_obj = PathInput(FILE_TYPES_DIR / "pdf" / "multipage.pdf")
     assert input_obj.is_pdf() is True
     input_obj.process_pdf(
         behavior=KEEP_ONLY, on_min_pages=2, page_indexes=[0, 1, 2, 3, 4]
```

### Comparing `mindee-4.7.0/tests/test_pkg_versions.py` & `mindee-4.8.0/tests/test_pkg_versions.py`

 * *Files identical despite different names*

