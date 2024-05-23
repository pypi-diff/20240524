# Comparing `tmp/surya_ocr-0.4.7.tar.gz` & `tmp/surya_ocr-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.7.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.8.tar", max compression
```

## Comparing `surya_ocr-0.4.7.tar` & `surya_ocr-0.4.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0    35085 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/LICENSE
--rw-r--r--   0        0        0    25008 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/README.md
--rw-r--r--   0        0        0     3084 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/detect_text.py
--rw-r--r--   0        0        0     6909 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/ocr_text.py
--rw-r--r--   0        0        0     1344 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/reading_order.py
--rw-r--r--   0        0        0      616 2024-05-18 04:03:18.838365 surya_ocr-0.4.7/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/benchmark/util.py
--rw-r--r--   0        0        0     5447 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/detection.py
--rw-r--r--   0        0        0      603 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/input/load.py
--rw-r--r--   0        0        0     3570 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/languages.py
--rw-r--r--   0        0        0     8728 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/layout.py
--rw-r--r--   0        0        0     5901 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1567 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/ordering/model.py
--rw-r--r--   0        0        0     6199 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2841 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/recognition/model.py
--rw-r--r--   0        0        0     9296 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     4133 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/ocr.py
--rw-r--r--   0        0        0     5838 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/ordering.py
--rw-r--r--   0        0        0     5806 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7785 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/postprocessing/util.py
--rw-r--r--   0        0        0     3898 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/recognition.py
--rw-r--r--   0        0        0     4490 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/schema.py
--rw-r--r--   0        0        0     3776 2024-05-18 04:03:18.982366 surya_ocr-0.4.7/surya/settings.py
--rw-r--r--   0        0        0    26351 1970-01-01 00:00:00.000000 surya_ocr-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/LICENSE
+-rw-r--r--   0        0        0    25008 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/README.md
+-rw-r--r--   0        0        0     3084 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/ocr_app.py
+-rw-r--r--   0        0        0     4112 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/ocr_text.py
+-rw-r--r--   0        0        0     1344 2024-05-23 23:12:59.437462 surya_ocr-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-23 23:12:59.437462 surya_ocr-0.4.8/reading_order.py
+-rw-r--r--   0        0        0      616 2024-05-23 23:12:59.437462 surya_ocr-0.4.8/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/util.py
+-rw-r--r--   0        0        0     5467 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/input/load.py
+-rw-r--r--   0        0        0     3642 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/languages.py
+-rw-r--r--   0        0        0     8723 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/layout.py
+-rw-r--r--   0        0        0    13801 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/detection/processor.py
+-rw-r--r--   0        0        0     5938 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1567 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     5738 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    32140 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0     2762 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2841 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     8188 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     3953 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/ocr.py
+-rw-r--r--   0        0        0     5838 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/ordering.py
+-rw-r--r--   0        0        0     5806 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7803 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/util.py
+-rw-r--r--   0        0        0     4004 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/recognition.py
+-rw-r--r--   0        0        0     4490 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/schema.py
+-rw-r--r--   0        0        0     3776 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/settings.py
+-rw-r--r--   0        0        0    26351 1970-01-01 00:00:00.000000 surya_ocr-0.4.8/PKG-INFO
```

### Comparing `surya_ocr-0.4.7/LICENSE` & `surya_ocr-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/README.md` & `surya_ocr-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/detect_layout.py` & `surya_ocr-0.4.8/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/detect_text.py` & `surya_ocr-0.4.8/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/ocr_app.py` & `surya_ocr-0.4.8/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/ocr_text.py` & `surya_ocr-0.4.8/ocr_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/pyproject.toml` & `surya_ocr-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.7"
+version = "0.4.8"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
```

### Comparing `surya_ocr-0.4.7/reading_order.py` & `surya_ocr-0.4.8/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/run_ocr_app.py` & `surya_ocr-0.4.8/run_ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/benchmark/bbox.py` & `surya_ocr-0.4.8/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/benchmark/metrics.py` & `surya_ocr-0.4.8/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/benchmark/tesseract.py` & `surya_ocr-0.4.8/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/benchmark/util.py` & `surya_ocr-0.4.8/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/detection.py` & `surya_ocr-0.4.8/surya/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 import numpy as np
 from PIL import Image
 
 from surya.model.detection.segformer import SegformerForRegressionMask
 from surya.postprocessing.heatmap import get_and_clean_boxes
 from surya.postprocessing.affinity import get_vertical_lines
-from surya.input.processing import prepare_image, split_image, get_total_splits
+from surya.input.processing import prepare_image_detection, split_image, get_total_splits
 from surya.schema import TextDetectionResult
 from surya.settings import settings
 from tqdm import tqdm
 from concurrent.futures import ProcessPoolExecutor
 import torch.nn.functional as F
 
 
@@ -58,15 +58,15 @@
         image_splits = []
         for image_idx, image in enumerate(batch_images):
             image_parts, split_height = split_image(image, processor)
             image_splits.extend(image_parts)
             split_index.extend([image_idx] * len(image_parts))
             split_heights.extend(split_height)
 
-        image_splits = [prepare_image(image, processor) for image in image_splits]
+        image_splits = [prepare_image_detection(image, processor) for image in image_splits]
         # Batch images in dim 0
         batch = torch.stack(image_splits, dim=0).to(model.dtype).to(model.device)
 
         with torch.inference_mode():
             pred = model(pixel_values=batch)
 
         logits = pred.logits
```

### Comparing `surya_ocr-0.4.7/surya/input/langs.py` & `surya_ocr-0.4.8/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/input/load.py` & `surya_ocr-0.4.8/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/input/processing.py` & `surya_ocr-0.4.8/surya/input/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 cropped = ImageOps.pad(cropped, (img.size[0], processor_height), color=255, centering=(0, 0))
             splits.append(cropped)
             split_heights.append(height)
         return splits, split_heights
     return [img.copy()], [img_height]
 
 
-def prepare_image(img, processor):
+def prepare_image_detection(img, processor):
     new_size = (processor.size["width"], processor.size["height"])
 
     img.thumbnail(new_size, Image.Resampling.LANCZOS) # Shrink largest dimension to fit new size
     img = img.resize(new_size, Image.Resampling.LANCZOS) # Stretch smaller dimension to fit new size
 
     img = np.asarray(img, dtype=np.uint8)
     img = processor(img)["pixel_values"][0]
@@ -77,15 +77,15 @@
     for bbox in bboxes:
         line = image.crop((bbox[0], bbox[1], bbox[2], bbox[3]))
         lines.append(line)
     return lines
 
 
 def slice_polys_from_image(image: Image.Image, polys):
-    image_array = np.array(image)
+    image_array = np.array(image, dtype=np.uint8)
     lines = []
     for idx, poly in enumerate(polys):
         lines.append(slice_and_pad_poly(image_array, poly))
     return lines
 
 
 def slice_and_pad_poly(image_array: np.array, coordinates):
@@ -94,14 +94,15 @@
     bbox = [min([x[0] for x in coordinates]), min([x[1] for x in coordinates]), max([x[0] for x in coordinates]), max([x[1] for x in coordinates])]
 
     # We mask out anything not in the polygon
     cropped_polygon = image_array[bbox[1]:bbox[3], bbox[0]:bbox[2]].copy()
     coordinates = [(x - bbox[0], y - bbox[1]) for x, y in coordinates]
 
     # Pad the area outside the polygon with the pad value
-    mask = np.zeros_like(cropped_polygon, dtype=np.uint8)
+    mask = np.zeros(cropped_polygon.shape[:2], dtype=np.uint8)
     cv2.fillPoly(mask, [np.int32(coordinates)], 1)
+    mask = np.stack([mask] * 3, axis=-1)
 
     cropped_polygon[mask == 0] = settings.RECOGNITION_PAD_VALUE
     rectangle_image = Image.fromarray(cropped_polygon)
 
     return rectangle_image
```

### Comparing `surya_ocr-0.4.7/surya/languages.py` & `surya_ocr-0.4.8/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/layout.py` & `surya_ocr-0.4.8/surya/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from surya.detection import batch_detection
 from surya.postprocessing.heatmap import keep_largest_boxes, get_and_clean_boxes, get_detected_boxes
 from surya.schema import LayoutResult, LayoutBox, TextDetectionResult
 from surya.settings import settings
 
 
-def get_regions_from_detection_result(detection_result: TextDetectionResult, heatmaps: List[Image.Image], orig_size, id2label, segment_assignment, vertical_line_width=20) -> List[LayoutBox]:
+def get_regions_from_detection_result(detection_result: TextDetectionResult, heatmaps: List[np.ndarray], orig_size, id2label, segment_assignment, vertical_line_width=20) -> List[LayoutBox]:
     logits = np.stack(heatmaps, axis=0)
     vertical_line_bboxes = [line for line in detection_result.vertical_lines]
     line_bboxes = detection_result.bboxes
 
     # Scale back to processor size
     for line in vertical_line_bboxes:
         line.rescale_bbox(orig_size, list(reversed(heatmaps[0].shape)))
@@ -122,15 +122,15 @@
 
     # Ensure we account for all text lines in the layout
     unused_lines = [line for idx, line in enumerate(line_bboxes) if idx not in used_lines]
     for bbox in unused_lines:
         new_boxes.append(LayoutBox(polygon=bbox.polygon, label="Text", confidence=.5))
 
     for bbox in new_boxes:
-        bbox.rescale(list(reversed(heatmap.shape)), orig_size)
+        bbox.rescale(list(reversed(heatmaps[0].shape)), orig_size)
 
     detected_boxes = [bbox for bbox in new_boxes if bbox.area > 16]
 
     # Remove bboxes contained inside others, unless they're captions
     contained_bbox = []
     for i, bbox in enumerate(detected_boxes):
         for j, bbox2 in enumerate(detected_boxes):
@@ -141,30 +141,30 @@
                 contained_bbox.append(j)
 
     detected_boxes = [bbox for idx, bbox in enumerate(detected_boxes) if idx not in contained_bbox]
 
     return detected_boxes
 
 
-def get_regions(heatmaps: List[Image.Image], orig_size, id2label, segment_assignment) -> List[LayoutBox]:
+def get_regions(heatmaps: List[np.ndarray], orig_size, id2label, segment_assignment) -> List[LayoutBox]:
     bboxes = []
     for i in range(1, len(id2label)):  # Skip the blank class
         heatmap = heatmaps[i]
         assert heatmap.shape == segment_assignment.shape
         heatmap[segment_assignment != i] = 0  # zero out where another segment is
         bbox = get_and_clean_boxes(heatmap, list(reversed(heatmap.shape)), orig_size)
         for bb in bbox:
             bboxes.append(LayoutBox(polygon=bb.polygon, label=id2label[i]))
         heatmaps.append(heatmap)
 
     bboxes = keep_largest_boxes(bboxes)
     return bboxes
 
 
-def parallel_get_regions(heatmaps: List[Image.Image], orig_size, id2label, detection_results=None) -> List[LayoutResult]:
+def parallel_get_regions(heatmaps: List[np.ndarray], orig_size, id2label, detection_results=None) -> LayoutResult:
     logits = np.stack(heatmaps, axis=0)
     segment_assignment = logits.argmax(axis=0)
     if detection_results is not None:
         bboxes = get_regions_from_detection_result(detection_results, heatmaps, orig_size, id2label,
                                                    segment_assignment)
     else:
         bboxes = get_regions(heatmaps, orig_size, id2label, segment_assignment)
```

### Comparing `surya_ocr-0.4.7/surya/model/detection/segformer.py` & `surya_ocr-0.4.8/surya/model/detection/segformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import gc
 import warnings
 warnings.filterwarnings("ignore", message="torch.utils._pytree._register_pytree_node is deprecated")
 
 import math
 from typing import Optional, Tuple, Union
 
-from transformers import SegformerConfig, SegformerForSemanticSegmentation, SegformerImageProcessor, \
-    SegformerDecodeHead, SegformerModel
+from transformers import SegformerConfig, SegformerForSemanticSegmentation, SegformerDecodeHead, SegformerModel
+from surya.model.detection.processor import SegformerImageProcessor
 import torch
 from torch import nn
 
 from transformers.modeling_outputs import SemanticSegmenterOutput
 from surya.settings import settings
```

### Comparing `surya_ocr-0.4.7/surya/model/ordering/decoder.py` & `surya_ocr-0.4.8/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/ordering/encoder.py` & `surya_ocr-0.4.8/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.8/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/ordering/model.py` & `surya_ocr-0.4.8/surya/model/ordering/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/ordering/processor.py` & `surya_ocr-0.4.8/surya/model/ordering/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,42 +27,33 @@
 
 class OrderImageProcessor(DonutImageProcessor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.patch_size = kwargs.get("patch_size", (4, 4))
 
-    def process_inner(self, images: List[List]):
-        # This will be in list of lists format, with height x width x channel
-        assert isinstance(images[0], (list, np.ndarray))
-
-        # convert list of lists format to array
-        if isinstance(images[0], list):
-            # numpy unit8 needed for augmentation
-            np_images = [np.array(img, dtype=np.uint8) for img in images]
-        else:
-            np_images = [img.astype(np.uint8) for img in images]
-            np_images = [img.transpose(2, 0, 1) for img in np_images] # convert to CHW format
+    def process_inner(self, images: List[np.ndarray]):
+        images = [img.transpose(2, 0, 1) for img in images] # convert to CHW format
 
-        assert np_images[0].shape[0] == 3 # RGB input images, channel dim last
+        assert images[0].shape[0] == 3 # RGB input images, channel dim last
 
         # Convert to float32 for rescale/normalize
-        np_images = [img.astype(np.float32) for img in np_images]
+        images = [img.astype(np.float32) for img in images]
 
         # Rescale and normalize
-        np_images = [
+        images = [
             self.rescale(img, scale=self.rescale_factor, input_data_format=ChannelDimension.FIRST)
-            for img in np_images
+            for img in images
         ]
-        np_images = [
+        images = [
             self.normalize(img, mean=self.image_mean, std=self.image_std, input_data_format=ChannelDimension.FIRST)
-            for img in np_images
+            for img in images
         ]
 
-        return np_images
+        return images
 
     def process_boxes(self, boxes):
         padded_boxes = []
         box_masks = []
         box_counts = []
         for b in boxes:
             # Left pad for generation
@@ -148,15 +139,15 @@
             new_images.append(img)
             new_boxes.append(box)
 
         images = new_images
         boxes = new_boxes
 
         # Convert to numpy for later processing steps
-        images = [to_numpy_array(image) for image in images]
+        images = [np.array(image) for image in images]
 
         images = self.process_inner(images)
         boxes, box_mask, box_counts = self.process_boxes(boxes)
         data = {
             "pixel_values": images,
             "input_boxes": boxes,
             "input_boxes_mask": box_mask,
```

### Comparing `surya_ocr-0.4.7/surya/model/recognition/config.py` & `surya_ocr-0.4.8/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/recognition/decoder.py` & `surya_ocr-0.4.8/surya/model/recognition/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/recognition/encoder.py` & `surya_ocr-0.4.8/surya/model/recognition/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/recognition/model.py` & `surya_ocr-0.4.8/surya/model/recognition/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/model/recognition/processor.py` & `surya_ocr-0.4.8/surya/model/recognition/processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, Union, Optional, List, Tuple
 
+import cv2
 from torch import TensorType
 from transformers import DonutImageProcessor, DonutProcessor, AutoImageProcessor, DonutSwinConfig
 from transformers.image_processing_utils import BaseImageProcessor, get_size_dict, BatchFeature
 from transformers.image_transforms import to_channel_dimension_format, pad, _rescale_for_pil_conversion, to_pil_image
 from transformers.image_utils import PILImageResampling, ImageInput, ChannelDimension, make_list_of_images, \
     valid_images, to_numpy_array, is_scaled_image, infer_channel_dimension_format, get_image_size
 import numpy as np
@@ -25,92 +26,72 @@
     def __init__(self, *args, max_size=None, train=False, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.patch_size = kwargs.get("patch_size", (4, 4))
         self.max_size = max_size
         self.train = train
 
-    def numpy_resize(self, image: np.ndarray, size, resample):
-        image = PIL.Image.fromarray(image)
-        resized = self.pil_resize(image, size, resample)
-        resized = np.array(resized, dtype=np.uint8)
-        resized_image = resized.transpose(2, 0, 1)
+    def numpy_resize(self, image: np.ndarray, size, interpolation=cv2.INTER_LANCZOS4):
+        height, width = image.shape[:2]
+        max_width, max_height = size["width"], size["height"]
 
-        return resized_image
+        if (height == max_height and width <= max_width) or (width == max_width and height <= max_height):
+            return image
 
-    def pil_resize(self, image: PIL.Image.Image, size, resample):
-        width, height = image.size
-        max_width, max_height = size["width"], size["height"]
-        if width != max_width or height != max_height:
-            # Shrink to fit within dimensions
-            width_scale = max_width / width
-            height_scale = max_height / height
-            scale = min(width_scale, height_scale)
-
-            new_width = min(int(width * scale), max_width)
-            new_height = min(int(height * scale), max_height)
-            image = image.resize((new_width, new_height), resample)
-
-        image.thumbnail((max_width, max_height), resample)
-
-        assert image.width <= max_width and image.height <= max_height
-
-        return image
-
-    def process_inner(self, images: List[List], train=False):
-        # This will be in list of lists format, with height x width x channel
-        assert isinstance(images[0], (list, np.ndarray))
-
-        # convert list of lists format to array
-        if isinstance(images[0], list):
-            # numpy unit8 needed for augmentation
-            np_images = [np.array(img, dtype=np.uint8) for img in images]
-        else:
-            np_images = [img.astype(np.uint8) for img in images]
+        scale = min(max_width / width, max_height / height)
+
+        new_width = int(width * scale)
+        new_height = int(height * scale)
+
+        resized_image = cv2.resize(image, (new_width, new_height), interpolation=interpolation)
+        resized_image = resized_image.transpose(2, 0, 1)
 
-        assert np_images[0].shape[2] == 3 # RGB input images, channel dim last
+        return resized_image
+
+    def process_inner(self, images: List[np.ndarray], train=False):
+        assert images[0].shape[2] == 3 # RGB input images, channel dim last
 
         # Rotate if the bbox is wider than it is tall
-        np_images = [self.align_long_axis(image, size=self.max_size, input_data_format=ChannelDimension.LAST) for image in np_images]
+        images = [self.align_long_axis(image, size=self.max_size, input_data_format=ChannelDimension.LAST) for image in images]
 
         # Verify that the image is wider than it is tall
-        for img in np_images:
+        for img in images:
             assert img.shape[1] >= img.shape[0]
 
         # This also applies the right channel dim format, to channel x height x width
-        np_images = [self.numpy_resize(img, self.max_size, self.resample) for img in np_images]
-        assert np_images[0].shape[0] == 3 # RGB input images, channel dim first
+        images = [self.numpy_resize(img, self.max_size, self.resample) for img in images]
+        assert images[0].shape[0] == 3 # RGB input images, channel dim first
 
         # Convert to float32 for rescale/normalize
-        np_images = [img.astype(np.float32) for img in np_images]
+        images = [img.astype(np.float32) for img in images]
 
         # Pads with 255 (whitespace)
         # Pad to max size to improve performance
         max_size = self.max_size
-        np_images = [
+        images = [
             self.pad_image(
                 image=image,
                 size=max_size,
                 random_padding=train, # Change amount of padding randomly during training
                 input_data_format=ChannelDimension.FIRST,
-                pad_value=255.0
+                pad_value=settings.RECOGNITION_PAD_VALUE
             )
-            for image in np_images
+            for image in images
         ]
         # Rescale and normalize
-        np_images = [
+        images = [
             self.rescale(img, scale=self.rescale_factor, input_data_format=ChannelDimension.FIRST)
-            for img in np_images
+            for img in images
         ]
-        np_images = [
+        images = [
             self.normalize(img, mean=self.image_mean, std=self.image_std, input_data_format=ChannelDimension.FIRST)
-            for img in np_images
+            for img in images
         ]
 
-        return np_images
+        return images
 
 
     def preprocess(
         self,
         images: ImageInput,
         do_resize: bool = None,
         size: Dict[str, int] = None,
@@ -127,23 +108,16 @@
         return_tensors: Optional[Union[str, TensorType]] = None,
         data_format: Optional[ChannelDimension] = ChannelDimension.FIRST,
         input_data_format: Optional[Union[str, ChannelDimension]] = None,
         **kwargs,
     ) -> PIL.Image.Image:
         images = make_list_of_images(images)
 
-        if not valid_images(images):
-            raise ValueError(
-                "Invalid image type. Must be of type PIL.Image.Image, numpy.ndarray, "
-                "torch.Tensor, tf.Tensor or jax.ndarray."
-            )
-
         # Convert to numpy for later processing steps
-        images = [to_numpy_array(image) for image in images]
-
+        images = [np.array(img) for img in images]
         images = self.process_inner(images, train=self.train)
         data = {"pixel_values": images}
         return BatchFeature(data=data, tensor_type=return_tensors)
 
     def pad_image(
         self,
         image: np.ndarray,
@@ -177,15 +151,15 @@
     def align_long_axis(
         self,
         image: np.ndarray,
         size: Dict[str, int],
         data_format: Optional[Union[str, ChannelDimension]] = None,
         input_data_format: Optional[Union[str, ChannelDimension]] = None,
     ) -> np.ndarray:
-        input_height, input_width = get_image_size(image, channel_dim=input_data_format)
+        input_height, input_width = image.shape[:2]
         output_height, output_width = size["height"], size["width"]
 
         if (output_width < output_height and input_width > input_height) or (
             output_width > output_height and input_width < input_height
         ):
             image = np.rot90(image, 3)
```

### Comparing `surya_ocr-0.4.7/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.8/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/ocr.py` & `surya_ocr-0.4.8/surya/ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-from collections import defaultdict
-from concurrent.futures import ProcessPoolExecutor
 from typing import List
-from tqdm import tqdm
-
-import torch
 from PIL import Image
 
 from surya.detection import batch_text_detection
 from surya.input.processing import slice_polys_from_image, slice_bboxes_from_image
-from surya.postprocessing.text import truncate_repetitions, sort_text_lines
+from surya.postprocessing.text import sort_text_lines
 from surya.recognition import batch_recognition
 from surya.schema import TextLine, OCRResult
-from surya.settings import settings
 
 
 def run_recognition(images: List[Image.Image], langs: List[List[str]], rec_model, rec_processor, bboxes: List[List[List[int]]] = None, polygons: List[List[List[List[int]]]] = None, batch_size=None) -> List[OCRResult]:
     # Polygons need to be in corner format - [[x1, y1], [x2, y2], [x3, y3], [x4, y4]], bboxes in [x1, y1, x2, y2] format
     assert bboxes is not None or polygons is not None
     assert len(images) == len(langs), "You need to pass in one list of languages for each image"
     slice_map = []
@@ -64,14 +58,15 @@
 
 def run_ocr(images: List[Image.Image], langs: List[List[str]], det_model, det_processor, rec_model, rec_processor, batch_size=None) -> List[OCRResult]:
     det_predictions = batch_text_detection(images, det_model, det_processor)
 
     all_slices = []
     slice_map = []
     all_langs = []
+
     for idx, (det_pred, image, lang) in enumerate(zip(det_predictions, images, langs)):
         polygons = [p.polygon for p in det_pred.bboxes]
         slices = slice_polys_from_image(image, polygons)
         slice_map.append(len(slices))
         all_langs.extend([lang] * len(slices))
         all_slices.extend(slices)
```

### Comparing `surya_ocr-0.4.7/surya/ordering.py` & `surya_ocr-0.4.8/surya/ordering.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/postprocessing/affinity.py` & `surya_ocr-0.4.8/surya/postprocessing/affinity.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/postprocessing/fonts.py` & `surya_ocr-0.4.8/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.8/surya/postprocessing/heatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,16 @@
 
     text_score_comb = np.clip(text_score, 0, 1).astype(np.uint8)
     label_count, labels, stats, centroids = cv2.connectedComponentsWithStats(text_score_comb, connectivity=4)
 
     det = []
     confidences = []
     max_confidence = 0
+    mask = np.zeros_like(linemap, dtype=np.uint8)
+
     for k in range(1, label_count):
         # size filtering
         size = stats[k, cv2.CC_STAT_AREA]
         if size < 10:
             continue
 
         # thresholding
@@ -136,15 +138,15 @@
             box = np.array([[l, t], [r, t], [r, b], [l, b]], dtype=np.float32)
 
         # make clock-wise order
         startidx = box.sum(axis=1).argmin()
         box = np.roll(box, 4-startidx, 0)
         box = np.array(box)
 
-        mask = np.zeros_like(linemap, dtype=np.uint8)
+        mask.fill(0)
         cv2.fillPoly(mask, [np.int32(box)], 1)
 
         roi = np.where(mask == 1, linemap, 0)
         confidence = np.mean(roi[roi != 0])
 
         if confidence > max_confidence:
             max_confidence = confidence
```

### Comparing `surya_ocr-0.4.7/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.8/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/postprocessing/math/render.py` & `surya_ocr-0.4.8/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/postprocessing/text.py` & `surya_ocr-0.4.8/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/postprocessing/util.py` & `surya_ocr-0.4.8/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/recognition.py` & `surya_ocr-0.4.8/surya/recognition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 import torch
 from PIL import Image
+from transformers import GenerationConfig
 
 from surya.postprocessing.math.latex import fix_math, contains_math
 from surya.postprocessing.text import truncate_repetitions
 from surya.settings import settings
 from tqdm import tqdm
 import numpy as np
 import torch.nn.functional as F
@@ -32,14 +33,15 @@
     confidences = []
 
     for i in tqdm(range(0, len(images), batch_size), desc="Recognizing Text"):
         batch_langs = languages[i:i+batch_size]
         has_math = ["_math" in lang for lang in batch_langs]
         batch_images = images[i:i+batch_size]
         batch_images = [image.convert("RGB") for image in batch_images]
+
         model_inputs = processor(text=[""] * len(batch_langs), images=batch_images, lang=batch_langs)
 
         batch_pixel_values = model_inputs["pixel_values"]
         batch_langs = model_inputs["langs"]
         batch_decoder_input = [[model.config.decoder_start_token_id] + lang for lang in batch_langs]
 
         batch_langs = torch.from_numpy(np.array(batch_langs, dtype=np.int64)).to(model.device)
@@ -48,14 +50,15 @@
 
         with torch.inference_mode():
             return_dict = model.generate(
                 pixel_values=batch_pixel_values,
                 decoder_input_ids=batch_decoder_input,
                 decoder_langs=batch_langs,
                 eos_token_id=processor.tokenizer.eos_id,
+                pad_token_id=processor.tokenizer.pad_token_id,
                 max_new_tokens=settings.RECOGNITION_MAX_TOKENS,
                 output_scores=True,
                 return_dict_in_generate=True
             )
             generated_ids = return_dict["sequences"]
 
             # Find confidence scores
```

### Comparing `surya_ocr-0.4.7/surya/schema.py` & `surya_ocr-0.4.8/surya/schema.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/surya/settings.py` & `surya_ocr-0.4.8/surya/settings.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.7/PKG-INFO` & `surya_ocr-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.7
+Version: 0.4.8
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

