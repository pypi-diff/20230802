# Comparing `tmp/qrcode_styled-0.2.1.tar.gz` & `tmp/qrcode_styled-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrcode_styled-0.2.1.tar", max compression
+gzip compressed data, was "qrcode_styled-0.2.2.tar", max compression
```

## Comparing `qrcode_styled-0.2.1.tar` & `qrcode_styled-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1068 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/LICENSE
--rw-r--r--   0        0        0     2232 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/README.md
--rw-r--r--   0        0        0     1173 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       45 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/__init__.py
--rw-r--r--   0        0        0        0 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/base/__init__.py
--rw-r--r--   0        0        0     6382 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/base/image.py
--rw-r--r--   0        0        0     3125 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/main.py
--rw-r--r--   0        0        0        0 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/__init__.py
--rw-r--r--   0        0        0        0 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/figures/__init__.py
--rw-r--r--   0        0        0      312 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/figures/base.py
--rw-r--r--   0        0        0      457 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/figures/base.pyi
--rw-r--r--   0        0        0      659 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/figures/corner.py
--rw-r--r--   0        0        0     4752 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/figures/dot.py
--rw-r--r--   0        0        0     4601 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/pil/image.py
--rw-r--r--   0        0        0        0 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/__init__.py
--rw-r--r--   0        0        0        0 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/figures/__init__.py
--rw-r--r--   0        0        0      467 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/figures/base.py
--rw-r--r--   0        0        0      730 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/figures/base.pyi
--rw-r--r--   0        0        0     1611 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/figures/corner.py
--rw-r--r--   0        0        0     2572 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/figures/dot.py
--rw-r--r--   0        0        0     7778 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/svg/image.py
--rw-r--r--   0        0        0       76 2022-01-19 14:17:44.215266 qrcode_styled-0.2.1/qrcode_styled/types.py
--rw-r--r--   0        0        0     3199 2022-01-19 14:18:04.742829 qrcode_styled-0.2.1/setup.py
--rw-r--r--   0        0        0     3327 2022-01-19 14:18:04.743232 qrcode_styled-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2238 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/README.md
+-rw-r--r--   0        0        0     1179 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/base/__init__.py
+-rw-r--r--   0        0        0     6382 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/base/image.py
+-rw-r--r--   0        0        0     3125 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/main.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/figures/__init__.py
+-rw-r--r--   0        0        0      312 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/figures/base.py
+-rw-r--r--   0        0        0      457 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/figures/base.pyi
+-rw-r--r--   0        0        0      659 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/figures/corner.py
+-rw-r--r--   0        0        0     4752 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/figures/dot.py
+-rw-r--r--   0        0        0     4601 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/pil/image.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/figures/__init__.py
+-rw-r--r--   0        0        0      467 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/figures/base.py
+-rw-r--r--   0        0        0      730 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/figures/base.pyi
+-rw-r--r--   0        0        0     1611 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/figures/corner.py
+-rw-r--r--   0        0        0     2572 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/figures/dot.py
+-rw-r--r--   0        0        0     7778 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/svg/image.py
+-rw-r--r--   0        0        0       76 2023-08-02 08:59:52.378701 qrcode_styled-0.2.2/qrcode_styled/types.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 qrcode_styled-0.2.2/PKG-INFO
```

### Comparing `qrcode_styled-0.2.1/LICENSE` & `qrcode_styled-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/README.md` & `qrcode_styled-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 This project was initially created for internal use in [cifrazia.com](https://cifrazia.com/).
 
 We do not intend to maintain this project for wide usage, but feel free to use it, share, edit or submit pull requests.
 
 ## Features
 
 + Multiple formats:
-   + [x] SVG using `xmls`
-   + [x] PNG/WEBP, etc. using `Pillow`
+    + [x] SVG using `xmls`
+    + [x] PNG/WEBP, etc. using `Pillow`
 + Multiple styles:
-   + [x] Extra rounded corners
-   + [ ] Rounded corners
-   + [ ] Straight
-   + [ ] Dotted
+    + [x] Extra rounded corners
+    + [ ] Rounded corners
+    + [ ] Straight
+    + [ ] Dotted
 
 Check out [our documentation](https://adambrianbright.github.io/qrcode_styled/get-started/).
 
 ## Installing
 
 Using **Poetry**
 
@@ -38,23 +38,23 @@
 
 ```shell
 pip install qrcode-styled
 ```
 
 ### Requirements
 
-+ Python `>= 3.9`
-+ Pillow `>= 8.2.0`
++ Python `>= 3.10`
++ Pillow `>= 10.0`
 + qrcode `>= 6.1`
 + lxml `>= 8.2.0` (optional, for SVG rendering)
 
 ### Extras
 
 | Keyword | Description                | Packages        |
-| ------- | -------------------------- | --------------- |
+|---------|----------------------------|-----------------|
 | `svg`   | Allows you to generate SVG | `lxml >= 4.6.3` |
 
 | SVG                                | WEBp                                |
-| ---------------------------------- | ----------------------------------- |
+|------------------------------------|-------------------------------------|
 | ![Svg QRCode](./wiki/img/test.svg) | ![Svg QRCode](./wiki/img/test.webp) |
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FAdamBrianBright%2Fqrcode_styled.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FAdamBrianBright%2Fqrcode_styled?ref=badge_large)
```

### Comparing `qrcode_styled-0.2.1/pyproject.toml` & `qrcode_styled-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrcode_styled"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python port for kozakdenys/qr-code-styling"
 authors = ["Bogdan Parfenov <adam.brian.bright@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cifrazia.com"
 repository = "https://github.com/AdamBrianBright/qrcode_styled.git"
 keywords = ["cifrazia", "library", "utils", "tools", "qrcode"]
@@ -23,24 +23,22 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/AdamBrianBright/qrcode_styled/issues"
 "Contact Author" = "https://vk.com/adam_bright"
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-qrcode = "^7.3.1"
-lxml = { version = "^4.7.1", optional = true }
-Pillow = "^9.0.0"
+python = "^3.10"
+qrcode = "^7.4.2"
+lxml = { version = "^4.9.3", optional = true }
+Pillow = "^10.0.0"
 
 [tool.poetry.extras]
 svg = ["lxml"]
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-lxml-stubs = "^0.3.0"
-
-
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+lxml-stubs = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qrcode_styled-0.2.1/qrcode_styled/base/image.py` & `qrcode_styled-0.2.2/qrcode_styled/base/image.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/main.py` & `qrcode_styled-0.2.2/qrcode_styled/main.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/pil/figures/corner.py` & `qrcode_styled-0.2.2/qrcode_styled/pil/figures/corner.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/pil/figures/dot.py` & `qrcode_styled-0.2.2/qrcode_styled/pil/figures/dot.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/pil/image.py` & `qrcode_styled-0.2.2/qrcode_styled/pil/image.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/svg/figures/base.pyi` & `qrcode_styled-0.2.2/qrcode_styled/svg/figures/base.pyi`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/svg/figures/corner.py` & `qrcode_styled-0.2.2/qrcode_styled/svg/figures/corner.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/svg/figures/dot.py` & `qrcode_styled-0.2.2/qrcode_styled/svg/figures/dot.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/qrcode_styled/svg/image.py` & `qrcode_styled-0.2.2/qrcode_styled/svg/image.py`

 * *Files identical despite different names*

### Comparing `qrcode_styled-0.2.1/PKG-INFO` & `qrcode_styled-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: qrcode-styled
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python port for kozakdenys/qr-code-styling
 Home-page: https://cifrazia.com
 License: MIT
 Keywords: cifrazia,library,utils,tools,qrcode
 Author: Bogdan Parfenov
 Author-email: adam.brian.bright@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: svg
-Requires-Dist: Pillow (>=9.0.0,<10.0.0)
-Requires-Dist: lxml (>=4.7.1,<5.0.0); extra == "svg"
-Requires-Dist: qrcode (>=7.3.1,<8.0.0)
+Requires-Dist: Pillow (>=10.0.0,<11.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0) ; extra == "svg"
+Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Project-URL: Bug Tracker, https://github.com/AdamBrianBright/qrcode_styled/issues
 Project-URL: Contact Author, https://vk.com/adam_bright
 Project-URL: Repository, https://github.com/AdamBrianBright/qrcode_styled.git
 Description-Content-Type: text/markdown
 
 # Welcome
 
@@ -40,21 +41,21 @@
 This project was initially created for internal use in [cifrazia.com](https://cifrazia.com/).
 
 We do not intend to maintain this project for wide usage, but feel free to use it, share, edit or submit pull requests.
 
 ## Features
 
 + Multiple formats:
-   + [x] SVG using `xmls`
-   + [x] PNG/WEBP, etc. using `Pillow`
+    + [x] SVG using `xmls`
+    + [x] PNG/WEBP, etc. using `Pillow`
 + Multiple styles:
-   + [x] Extra rounded corners
-   + [ ] Rounded corners
-   + [ ] Straight
-   + [ ] Dotted
+    + [x] Extra rounded corners
+    + [ ] Rounded corners
+    + [ ] Straight
+    + [ ] Dotted
 
 Check out [our documentation](https://adambrianbright.github.io/qrcode_styled/get-started/).
 
 ## Installing
 
 Using **Poetry**
 
@@ -66,23 +67,23 @@
 
 ```shell
 pip install qrcode-styled
 ```
 
 ### Requirements
 
-+ Python `>= 3.9`
-+ Pillow `>= 8.2.0`
++ Python `>= 3.10`
++ Pillow `>= 10.0`
 + qrcode `>= 6.1`
 + lxml `>= 8.2.0` (optional, for SVG rendering)
 
 ### Extras
 
 | Keyword | Description                | Packages        |
-| ------- | -------------------------- | --------------- |
+|---------|----------------------------|-----------------|
 | `svg`   | Allows you to generate SVG | `lxml >= 4.6.3` |
 
 | SVG                                | WEBp                                |
-| ---------------------------------- | ----------------------------------- |
+|------------------------------------|-------------------------------------|
 | ![Svg QRCode](./wiki/img/test.svg) | ![Svg QRCode](./wiki/img/test.webp) |
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FAdamBrianBright%2Fqrcode_styled.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FAdamBrianBright%2Fqrcode_styled?ref=badge_large)
```

