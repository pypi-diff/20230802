# Comparing `tmp/epubgen-0.4.1.tar.gz` & `tmp/epubgen-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubgen-0.4.1.tar", last modified: Sun Jul 30 18:07:45 2023, max compression
+gzip compressed data, was "epubgen-0.4.2.tar", last modified: Wed Aug  2 20:40:13 2023, max compression
```

## Comparing `epubgen-0.4.1.tar` & `epubgen-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 18:07:45.420667 epubgen-0.4.1/
--rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.4.1/LICENSE
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 18:07:45.420274 epubgen-0.4.1/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.4.1/README.md
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 18:07:45.416602 epubgen-0.4.1/epubgen/
--rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.4.1/epubgen/__init__.py
--rw-r--r--   0 sfluor     (501) staff       (20)     9067 2023-07-30 18:05:46.000000 epubgen-0.4.1/epubgen/epubgen.py
-drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-07-30 18:07:45.419616 epubgen-0.4.1/epubgen.egg-info/
--rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/PKG-INFO
--rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/SOURCES.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/dependency_links.txt
--rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-07-30 18:07:45.000000 epubgen-0.4.1/epubgen.egg-info/top_level.txt
--rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-07-30 18:07:19.000000 epubgen-0.4.1/pyproject.toml
--rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-07-30 18:07:45.420778 epubgen-0.4.1/setup.cfg
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-08-02 20:40:13.544473 epubgen-0.4.2/
+-rw-r--r--   0 sfluor     (501) staff       (20)     1067 2023-07-28 21:42:19.000000 epubgen-0.4.2/LICENSE
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-08-02 20:40:13.544090 epubgen-0.4.2/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      506 2023-07-30 15:36:10.000000 epubgen-0.4.2/README.md
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-08-02 20:40:13.541079 epubgen-0.4.2/epubgen/
+-rw-r--r--   0 sfluor     (501) staff       (20)       26 2023-07-30 15:23:29.000000 epubgen-0.4.2/epubgen/__init__.py
+-rw-r--r--   0 sfluor     (501) staff       (20)     9362 2023-08-02 20:09:03.000000 epubgen-0.4.2/epubgen/epubgen.py
+drwxr-xr-x   0 sfluor     (501) staff       (20)        0 2023-08-02 20:40:13.543553 epubgen-0.4.2/epubgen.egg-info/
+-rw-r--r--   0 sfluor     (501) staff       (20)      995 2023-08-02 20:40:13.000000 epubgen-0.4.2/epubgen.egg-info/PKG-INFO
+-rw-r--r--   0 sfluor     (501) staff       (20)      195 2023-08-02 20:40:13.000000 epubgen-0.4.2/epubgen.egg-info/SOURCES.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        1 2023-08-02 20:40:13.000000 epubgen-0.4.2/epubgen.egg-info/dependency_links.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)        8 2023-08-02 20:40:13.000000 epubgen-0.4.2/epubgen.egg-info/top_level.txt
+-rw-r--r--   0 sfluor     (501) staff       (20)      560 2023-08-02 20:39:33.000000 epubgen-0.4.2/pyproject.toml
+-rw-r--r--   0 sfluor     (501) staff       (20)       38 2023-08-02 20:40:13.544599 epubgen-0.4.2/setup.cfg
```

### Comparing `epubgen-0.4.1/LICENSE` & `epubgen-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epubgen-0.4.1/PKG-INFO` & `epubgen-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.4.1/epubgen/epubgen.py` & `epubgen-0.4.2/epubgen/epubgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from zipfile import ZipFile
 from datetime import datetime
 import xml.etree.ElementTree as ET
+import io
 
 CONTENT_ROOT = "EPUB/"
 TOC_PATH = "toc.xhtml"
 PACKAGE_PATH = CONTENT_ROOT + "package.opf"
 TOC_ID = "toc"
 TOC_NAME = "Table of contents"
 CSS_FILE = "stylesheet.css"
@@ -30,15 +31,16 @@
 
     Methods
     -------
     - add_page: add content to the EPUB
     - add_font: add a font to the EPUB
     - add_image: embed images in the EPUB
     - add_cover: add a cover image for the EPUB
-    - generate_epub: generate the EPUB file
+    - to_disk: generate the EPUB file and writes it to disk
+    - to_bytes: generate the EPUB file and returns a BytesIO buffer
     """
 
     def __init__(
         self, title: str, author: str, language: str, id: str, css="", rtl=False
     ):
         self.id: str = id
         self.rtl: bool = rtl
@@ -247,24 +249,33 @@
 
         if toc_title is not None:
             li = ET.Element("li")
             link = ET.SubElement(li, "a", href=path)
             link.text = toc_title
             self.toc.append(li)
 
-    def generate_epub(self, path: str):
-        """
-        Generates the EPUB and saves it at the provided path.
-        """
+    def to_bytes(self) -> io.BytesIO:
         contents = self.contents
         if self.css:
             contents.append((CONTENT_ROOT + CSS_FILE, self.css))
             self._add_to_manifest("stylesheet", CSS_FILE, "text/css")
 
         contents = contents + [
             (CONTENT_ROOT + TOC_PATH, self._generate_toc()),
             (PACKAGE_PATH, self._generate_pkg_opf()),
         ]
 
-        with ZipFile(path, "w") as zip:
+        buf = io.BytesIO()
+        with ZipFile(buf, "a") as zip:
             for path, content in contents:
                 zip.writestr(path, content)
+
+        return buf
+
+    def to_disk(self, path: str):
+        """
+        Generates the EPUB and saves it at the provided path.
+        """
+        buf : io.BytesIO = self.to_bytes()
+
+        with open(path, "wb") as file:
+            file.write(buf.getvalue())
```

### Comparing `epubgen-0.4.1/epubgen.egg-info/PKG-INFO` & `epubgen-0.4.2/epubgen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgen
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tiny library to programmatically generate .epub files
 Author: Sami Tabet
 Project-URL: Homepage, https://github.com/sfluor/epubgen
 Project-URL: Bug Tracker, https://github.com/sfluor/epubgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epubgen-0.4.1/pyproject.toml` & `epubgen-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epubgen"
-version = "0.4.1"
+version = "0.4.2"
 authors = [{ name = "Sami Tabet" }]
 description = "Tiny library to programmatically generate .epub files"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

