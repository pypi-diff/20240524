# Comparing `tmp/pdftext-0.3.7.tar.gz` & `tmp/pdftext-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.7.tar", max compression
+gzip compressed data, was "pdftext-0.3.8.tar", max compression
```

## Comparing `pdftext-0.3.7.tar` & `pdftext-0.3.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-05-07 20:14:47.002582 pdftext-0.3.7/LICENSE
--rw-r--r--   0        0        0     7170 2024-05-07 20:14:47.002582 pdftext-0.3.7/README.md
--rw-r--r--   0        0        0     1726 2024-05-07 20:14:47.002582 pdftext-0.3.7/extract_text.py
--rw-r--r--   0        0        0    14097 2024-05-07 20:14:47.002582 pdftext-0.3.7/models/dt.joblib
--rw-r--r--   0        0        0     2426 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/extraction.py
--rw-r--r--   0        0        0     7382 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/model.py
--rw-r--r--   0        0        0     3880 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4613 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3222 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/postprocessing.py
--rw-r--r--   0        0        0      488 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-05-07 20:14:47.002582 pdftext-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-05-23 19:30:54.933288 pdftext-0.3.8/LICENSE
+-rw-r--r--   0        0        0     7180 2024-05-23 19:30:54.933288 pdftext-0.3.8/README.md
+-rw-r--r--   0        0        0     1904 2024-05-23 19:30:54.933288 pdftext-0.3.8/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-05-23 19:30:54.933288 pdftext-0.3.8/models/dt.joblib
+-rw-r--r--   0        0        0     3700 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/extraction.py
+-rw-r--r--   0        0        0     7382 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/model.py
+-rw-r--r--   0        0        0     3811 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4613 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3222 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      569 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-05-23 19:30:54.933288 pdftext-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     8156 1970-01-01 00:00:00.000000 pdftext-0.3.8/PKG-INFO
```

### Comparing `pdftext-0.3.7/LICENSE` & `pdftext-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.7/README.md` & `pdftext-0.3.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--sort` will attempt to sort in reading order if specified.
 - `--keep_hyphens` will keep hyphens in the output (they will be stripped and words joined otherwise)
 - `--pages` will specify pages (comma separated) to extract
+- `--workers` specifies the number of parallel workers to use
 
 ## JSON
 
 This command outputs structured blocks and lines with font and other information.
 
 ```shell
 pdftext PDF_PATH --out_path output.txt --json
@@ -38,14 +39,15 @@
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--json` specifies json output
 - `--sort` will attempt to sort in reading order if specified.
 - `--pages` will specify pages (comma separated) to extract
 - `--keep_chars` will keep individual characters in the json output
+- `--workers` specifies the number of parallel workers to use
 
 The output will be a json list, with each item in the list corresponding to a single page in the input pdf (in order).  Each page will include the following keys:
 
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
@@ -67,29 +69,25 @@
 If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
 
 # Programmatic usage
 
 Extract plain text:
 
 ```python
-import pypdfium2 as pdfium
 from pdftext.extraction import plain_text_output
 
-pdf = pdfium.PdfDocument(PDF_PATH)
-text = plain_text_output(pdf, sort=False, hyphens=False, page_range=[1,2,3]) # Optional arguments explained above
+text = plain_text_output(PDF_PATH, sort=False, hyphens=False, page_range=[1,2,3]) # Optional arguments explained above
 ```
 
 Extract structured blocks and lines:
 
 ```python
-import pypdfium2 as pdfium
 from pdftext.extraction import dictionary_output
 
-pdf = pdfium.PdfDocument(PDF_PATH)
-text = dictionary_output(pdf, sort=False, page_range=[1,2,3], keep_chars=False) # Optional arguments explained above
+text = dictionary_output(PDF_PATH, sort=False, page_range=[1,2,3], keep_chars=False) # Optional arguments explained above
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
 I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
```

### Comparing `pdftext-0.3.7/extract_text.py` & `pdftext-0.3.8/extract_text.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,28 @@
     parser.add_argument("pdf_path", type=str, help="Path to the PDF file")
     parser.add_argument("--out_path", type=str, help="Path to the output text file, defaults to stdout", default=None)
     parser.add_argument("--json", action="store_true", help="Output json instead of plain text", default=False)
     parser.add_argument("--sort", action="store_true", help="Attempt to sort the text by reading order", default=False)
     parser.add_argument("--keep_hyphens", action="store_true", help="Keep hyphens in words", default=False)
     parser.add_argument("--pages", type=str, help="Comma separated pages to extract, like 1,2,3", default=None)
     parser.add_argument("--keep_chars", action="store_true", help="Keep character level information", default=False)
+    parser.add_argument("--workers", type=int, help="Number of workers to use for parallel processing", default=None)
     args = parser.parse_args()
 
-    pdf_doc = pdfium.PdfDocument(args.pdf_path)
     pages = None
     if args.pages is not None:
+        pdf_doc = pdfium.PdfDocument(args.pdf_path)
         pages = [int(p) for p in args.pages.split(",")]
         assert all(p <= len(pdf_doc) for p in pages), "Invalid page number(s) provided"
 
     if args.json:
-        text = dictionary_output(pdf_doc, sort=args.sort, page_range=pages, keep_chars=args.keep_chars)
+        text = dictionary_output(args.pdf_path, sort=args.sort, page_range=pages, keep_chars=args.keep_chars, workers=args.workers)
         text = json.dumps(text)
     else:
-        text = plain_text_output(pdf_doc, sort=args.sort, hyphens=args.keep_hyphens, page_range=pages)
+        text = plain_text_output(args.pdf_path, sort=args.sort, hyphens=args.keep_hyphens, page_range=pages, workers=args.workers)
 
     if args.out_path is None:
         print(text)
     else:
         with open(args.out_path, "w+") as f:
             f.write(text)
```

### Comparing `pdftext-0.3.7/models/dt.joblib` & `pdftext-0.3.8/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.7/pdftext/extraction.py` & `pdftext-0.3.8/pdftext/extraction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,72 @@
+from functools import partial
 from typing import List
+from concurrent.futures import ProcessPoolExecutor
+import math
+import pypdfium2 as pdfium
 
 from pdftext.inference import inference
 from pdftext.model import get_model
 from pdftext.pdf.chars import get_pdfium_chars
 from pdftext.pdf.utils import unnormalize_bbox
 from pdftext.postprocessing import merge_text, sort_blocks, postprocess_text, handle_hyphens
+from pdftext.settings import settings
 
 
-def _get_pages(pdf_doc, model=None, page_range=None):
-    if model is None:
-        model = get_model()
-    text_chars = get_pdfium_chars(pdf_doc, page_range=page_range)
+def _get_page_range(pdf_path, model, page_range):
+    pdf_doc = pdfium.PdfDocument(pdf_path)
+    text_chars = get_pdfium_chars(pdf_doc, page_range)
     pages = inference(text_chars, model)
     return pages
 
 
-def plain_text_output(pdf_doc, sort=False, model=None, hyphens=False, page_range=None) -> str:
-    text = paginated_plain_text_output(pdf_doc, sort=sort, model=model, hyphens=hyphens, page_range=page_range)
+def _get_pages(pdf_path, model=None, page_range=None, workers=None):
+    if model is None:
+        model = get_model()
+
+    pdf_doc = pdfium.PdfDocument(pdf_path)
+    if page_range is None:
+        page_range = range(len(pdf_doc))
+
+    if workers is not None:
+        workers = min(workers, len(page_range) // settings.WORKER_PAGE_THRESHOLD) # It's inefficient to have too many workers, since we batch in inference
+
+    if workers is None or workers <= 1:
+        text_chars = get_pdfium_chars(pdf_doc, page_range)
+        return inference(text_chars, model)
+
+    func = partial(_get_page_range, pdf_path, model)
+    page_range = list(page_range)
+
+    pages_per_worker = math.ceil(len(page_range) / workers)
+    page_range_chunks = [page_range[i * pages_per_worker:(i + 1) * pages_per_worker] for i in range(workers)]
+
+    with ProcessPoolExecutor(max_workers=workers) as executor:
+        pages = list(executor.map(func, page_range_chunks))
+
+    ordered_pages = [page for sublist in pages for page in sublist]
+
+    return ordered_pages
+
+
+def plain_text_output(pdf_path, sort=False, model=None, hyphens=False, page_range=None, workers=None) -> str:
+    text = paginated_plain_text_output(pdf_path, sort=sort, model=model, hyphens=hyphens, page_range=page_range, workers=workers)
     return "\n".join(text)
 
 
-def paginated_plain_text_output(pdf_doc, sort=False, model=None, hyphens=False, page_range=None) -> List[str]:
-    pages = _get_pages(pdf_doc, model, page_range)
+def paginated_plain_text_output(pdf_path, sort=False, model=None, hyphens=False, page_range=None, workers=None) -> List[str]:
+    pages = _get_pages(pdf_path, model, page_range, workers=workers)
     text = []
     for page in pages:
         text.append(merge_text(page, sort=sort, hyphens=hyphens).strip())
     return text
 
 
-def dictionary_output(pdf_doc, sort=False, model=None, page_range=None, keep_chars=False):
-    pages = _get_pages(pdf_doc, model, page_range)
+def dictionary_output(pdf_path, sort=False, model=None, page_range=None, keep_chars=False, workers=None):
+    pages = _get_pages(pdf_path, model, page_range, workers=workers)
     for page in pages:
         for block in page["blocks"]:
             bad_keys = [key for key in block.keys() if key not in ["lines", "bbox"]]
             for key in bad_keys:
                 del block[key]
             for line in block["lines"]:
                 bad_keys = [key for key in line.keys() if key not in ["bbox", "spans"]]
```

### Comparing `pdftext-0.3.7/pdftext/inference.py` & `pdftext-0.3.8/pdftext/inference.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.7/pdftext/pdf/chars.py` & `pdftext-0.3.8/pdftext/pdf/chars.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,16 @@
         # If we hit the region with the previous fontname, we can bail out
         if fontname == prev_fontname and fontflags == prev_fontflags:
             break
         text_chars["chars"][j]["font"]["name"] = fontname
         text_chars["chars"][j]["font"]["flags"] = fontflags
 
 
-def get_pdfium_chars(pdf, fontname_sample_freq=settings.FONTNAME_SAMPLE_FREQ, page_range=None):
+def get_pdfium_chars(pdf, page_range, fontname_sample_freq=settings.FONTNAME_SAMPLE_FREQ):
     blocks = []
-    if page_range is None:
-        page_range = range(len(pdf))
 
     for page_idx in page_range:
         page = pdf.get_page(page_idx)
         text_page = page.get_textpage()
         mediabox = page.get_mediabox()
         page_rotation = page.get_rotation()
         bbox = page.get_bbox()
```

### Comparing `pdftext-0.3.7/pdftext/pdf/utils.py` & `pdftext-0.3.8/pdftext/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.7/pdftext/postprocessing.py` & `pdftext-0.3.8/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.7/pyproject.toml` & `pdftext-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.7"
+version = "0.3.8"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.7/PKG-INFO` & `pdftext-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.7
+Version: 0.3.8
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -46,14 +46,15 @@
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--sort` will attempt to sort in reading order if specified.
 - `--keep_hyphens` will keep hyphens in the output (they will be stripped and words joined otherwise)
 - `--pages` will specify pages (comma separated) to extract
+- `--workers` specifies the number of parallel workers to use
 
 ## JSON
 
 This command outputs structured blocks and lines with font and other information.
 
 ```shell
 pdftext PDF_PATH --out_path output.txt --json
@@ -61,14 +62,15 @@
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--json` specifies json output
 - `--sort` will attempt to sort in reading order if specified.
 - `--pages` will specify pages (comma separated) to extract
 - `--keep_chars` will keep individual characters in the json output
+- `--workers` specifies the number of parallel workers to use
 
 The output will be a json list, with each item in the list corresponding to a single page in the input pdf (in order).  Each page will include the following keys:
 
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
@@ -90,29 +92,25 @@
 If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
 
 # Programmatic usage
 
 Extract plain text:
 
 ```python
-import pypdfium2 as pdfium
 from pdftext.extraction import plain_text_output
 
-pdf = pdfium.PdfDocument(PDF_PATH)
-text = plain_text_output(pdf, sort=False, hyphens=False, page_range=[1,2,3]) # Optional arguments explained above
+text = plain_text_output(PDF_PATH, sort=False, hyphens=False, page_range=[1,2,3]) # Optional arguments explained above
 ```
 
 Extract structured blocks and lines:
 
 ```python
-import pypdfium2 as pdfium
 from pdftext.extraction import dictionary_output
 
-pdf = pdfium.PdfDocument(PDF_PATH)
-text = dictionary_output(pdf, sort=False, page_range=[1,2,3], keep_chars=False) # Optional arguments explained above
+text = dictionary_output(PDF_PATH, sort=False, page_range=[1,2,3], keep_chars=False) # Optional arguments explained above
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
 I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
```

