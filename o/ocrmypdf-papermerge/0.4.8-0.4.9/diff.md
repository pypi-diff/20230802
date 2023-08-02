# Comparing `tmp/ocrmypdf_papermerge-0.4.8.tar.gz` & `tmp/ocrmypdf_papermerge-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrmypdf_papermerge-0.4.8.tar", max compression
+gzip compressed data, was "ocrmypdf_papermerge-0.4.9.tar", max compression
```

## Comparing `ocrmypdf_papermerge-0.4.8.tar` & `ocrmypdf_papermerge-0.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10231 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/LICENSE
--rw-r--r--   0        0        0      459 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/README.md
--rw-r--r--   0        0        0      448 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/changelog.md
--rw-r--r--   0        0        0        0 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/__init__.py
--rw-r--r--   0        0        0      594 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_preview.py
--rw-r--r--   0        0        0      919 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_svg.py
--rw-r--r--   0        0        0     1767 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/hocr.py
--rw-r--r--   0        0        0      664 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/image.py
--rw-r--r--   0        0        0     2116 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/plugin.py
--rw-r--r--   0        0        0      479 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/render.py
--rw-r--r--   0        0        0      312 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/templates/page.html.j2
--rw-r--r--   0        0        0      611 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/templates/page.svg.j2
--rw-r--r--   0        0        0     2544 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/utils.py
--rw-r--r--   0        0        0     1375 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 ocrmypdf_papermerge-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    10231 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/LICENSE
+-rw-r--r--   0        0        0      459 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/README.md
+-rw-r--r--   0        0        0      515 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/changelog.md
+-rw-r--r--   0        0        0        0 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/__init__.py
+-rw-r--r--   0        0        0      667 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/generate_preview.py
+-rw-r--r--   0        0        0      919 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/generate_svg.py
+-rw-r--r--   0        0        0     1768 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/hocr.py
+-rw-r--r--   0        0        0      665 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/image.py
+-rw-r--r--   0        0        0     2169 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/plugin.py
+-rw-r--r--   0        0        0      480 2023-08-02 07:15:09.519276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/render.py
+-rw-r--r--   0        0        0      312 2023-08-02 07:15:09.523276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/templates/page.html.j2
+-rw-r--r--   0        0        0      612 2023-08-02 07:15:09.523276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/templates/page.svg.j2
+-rw-r--r--   0        0        0     2545 2023-08-02 07:15:09.523276 ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/utils.py
+-rw-r--r--   0        0        0     1435 2023-08-02 07:15:09.523276 ocrmypdf_papermerge-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 ocrmypdf_papermerge-0.4.9/PKG-INFO
```

### Comparing `ocrmypdf_papermerge-0.4.8/LICENSE` & `ocrmypdf_papermerge-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_preview.py` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/generate_preview.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from pathlib import Path
+
 from PIL import Image
 
 from .utils import get_result_file_path
 
 
-def generate_preview(input_file, options):
+def generate_preview(
+    input_file: Path | str,
+    preview_width: int,
+    sidecar_dir: Path | str
+) -> None:
     """
     Generates page preview as jpeg
     """
     output_file_path = get_result_file_path(
         input_file_path=str(input_file),
-        output_dir=options.sidecar_dir,
+        output_dir=str(sidecar_dir),
         output_ext="jpg"
     )
 
     im = Image.open(input_file)
 
-    width = options.preview_width
-    wpercent = (width / float(im.size[0]))
+    wpercent = (preview_width / float(im.size[0]))
     height = int((float(im.size[1]) * float(wpercent)))
-    im = im.resize((width, height), Image.ANTIALIAS)
+    im = im.resize((preview_width, height), Image.LANCZOS)
 
     im.save(output_file_path, quality=50, format='JPEG')
```

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_svg.py` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/generate_svg.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/hocr.py` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/hocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+
 from lxml import html
 
 
 class BBox:
 
     PATTERN = r"(?P<x1>\d+)\s+(?P<y1>\d+)\s+(?P<x2>\d+)\s+(?P<y2>\d+)"
```

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/image.py` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
-from PIL import Image
 from io import BytesIO
 
+from PIL import Image
+
 
 def image_to_base64(image_path):
     """
     Converts image to base64 encoded string.
 
     image_path: path to input image
```

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/plugin.py` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from ocrmypdf import hookimpl
-from ocrmypdf.builtin_plugins.tesseract_ocr import TesseractOcrEngine
 from ocrmypdf._exec import tesseract
+from ocrmypdf.builtin_plugins.tesseract_ocr import TesseractOcrEngine
 
 from .generate_preview import generate_preview
 from .generate_svg import generate_svg
-from .utils import (
-    copy_hocr,
-    copy_txt
-)
+from .utils import copy_hocr, copy_txt
 
 
 class CustomEngine(TesseractOcrEngine):
 
     @staticmethod
     def generate_hocr(input_file, output_hocr, output_text, options):
         tesseract.generate_hocr(
@@ -26,15 +23,16 @@
             user_words=options.user_words,
             user_patterns=options.user_patterns,
             thresholding=options.tesseract_thresholding
         )
         # jpeg thumbnail preview image
         generate_preview(
             input_file=str(input_file),
-            options=options
+            preview_width=options.preview_width,
+            sidecar_dir=options.sidecar_dir
         )
         # svg | html with embedded raster image plus
         # mapped hocr text
         generate_svg(
             input_file=str(input_file),
             input_hocr=output_hocr,
             options=options
```

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/templates/page.svg.j2` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/templates/page.svg.j2`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 000001f0: 7472 616e 7370 6172 656e 7422 0a20 2020  transparent".   
 00000200: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
 00000210: 3d22 302e 3422 3e0a 2020 2020 2020 2020  ="0.4">.        
 00000220: 2020 2020 7b7b 776f 7264 2e74 6578 747d      {{word.text}
 00000230: 7d0a 2020 2020 2020 2020 3c2f 7465 7874  }.        </text
 00000240: 3e0a 2020 2020 7b25 2065 6e64 666f 7220  >.    {% endfor 
 00000250: 257d 0a20 2020 3c2f 673e 0a0a 0a3c 2f73  %}.   </g>...</s
-00000260: 7667 3e                                  vg>
+00000260: 7667 3e0a                                vg>.
```

### Comparing `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/utils.py` & `ocrmypdf_papermerge-0.4.9/ocrmypdf_papermerge/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     if not isinstance(input_file_path, str):
         raise ValueError("Expecting a string as input")
 
     if len(input_file_path) < 6:  # page number has 6 digits
         raise ValueError("Expecting a string at least 6 characters long")
 
     PATTERN = r"(?P<page_num>\d{6})"
+
     match = re.search(PATTERN, input_file_path)
     if match:
         return match.group('page_num')
 
     # always should match, otherwise there is something wrong
     # with input. Maybe OCRmyPDF output format changed?
     raise ValueError("get_page_number did not match")
```

### Comparing `ocrmypdf_papermerge-0.4.8/pyproject.toml` & `ocrmypdf_papermerge-0.4.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocrmypdf-papermerge"
-version = "0.4.8"
+version = "0.4.9"
 description = "OCRmyPDF plugin to generate SVG files for Papermerge"
 authors = ["Eugen Ciur <eugen@papermerge.com>"]
 maintainers = ["Eugen Ciur <eugen@papermerge.com>"]
 license = "Apache-2.0"
 include = ["LICENSE", "changelog.md", "README.md", "ocrmypdf_papermerge/templates/*"]
 readme = "README.md"
 classifiers = [
@@ -30,14 +30,17 @@
 lxml = "^4.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pycodestyle = "^2.8.0"
 taskipy = "^1.10.2"
 
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.3.3"
+
 [tool.taskipy.tasks]
 test = "python -m pytest"
 lint = "pycodestyle tests/ ocrmypdf_papermerge/"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ocrmypdf_papermerge-0.4.8/PKG-INFO` & `ocrmypdf_papermerge-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrmypdf-papermerge
-Version: 0.4.8
+Version: 0.4.9
 Summary: OCRmyPDF plugin to generate SVG files for Papermerge
 Home-page: https://github.com/papermerge/OCRmyPDF_papermerge
 License: Apache-2.0
 Keywords: OCR,PDF,OCRmyPDF,Document Management System
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Maintainer: Eugen Ciur
```

