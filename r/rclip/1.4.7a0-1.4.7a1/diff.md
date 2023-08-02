# Comparing `tmp/rclip-1.4.7a0.tar.gz` & `tmp/rclip-1.4.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.7a0.tar", max compression
+gzip compressed data, was "rclip-1.4.7a1.tar", max compression
```

## Comparing `rclip-1.4.7a0.tar` & `rclip-1.4.7a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-02 07:11:08.082285 rclip-1.4.7a0/LICENSE
--rw-r--r--   0        0        0     5023 2023-08-02 07:11:08.082285 rclip-1.4.7a0/README.md
--rw-r--r--   0        0        0     1559 2023-08-02 07:11:08.082285 rclip-1.4.7a0/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/main.py
--rw-r--r--   0        0        0     5212 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/model.py
--rw-r--r--   0        0        0     4746 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/utils.py
--rw-r--r--   0        0        0     6531 1970-01-01 00:00:00.000000 rclip-1.4.7a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-02 07:17:11.716274 rclip-1.4.7a1/LICENSE
+-rw-r--r--   0        0        0     5194 2023-08-02 07:17:11.716274 rclip-1.4.7a1/README.md
+-rw-r--r--   0        0        0     1559 2023-08-02 07:17:11.716274 rclip-1.4.7a1/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/main.py
+-rw-r--r--   0        0        0     5212 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/model.py
+-rw-r--r--   0        0        0     4746 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/utils.py
+-rw-r--r--   0        0        0     6702 1970-01-01 00:00:00.000000 rclip-1.4.7a1/PKG-INFO
```

### Comparing `rclip-1.4.7a0/LICENSE` & `rclip-1.4.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a0/README.md` & `rclip-1.4.7a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,29 @@
   ```bash
   chmod +x <downloaded AppImage filename>
   sudo mv <downloaded AppImage filename> /usr/local/bin/rclip
   ```
 </details>
 
 <details>
-  <summary><strong>macOS/Windows/Linux (using <code>pip</code>)</strong></summary>
+  <summary><strong>macOS/Windows (using <code>pip</code>)</strong></summary>
 
   ```bash
   pip install rclip
   ```
 </details>
 
+<details>
+  <summary><strong>Linux (using <code>pip</code>)</strong></summary>
+
+  ```bash
+  pip install --index-url https://download.pytorch.org/whl/cpu rclip
+  ```
+</details>
+
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
 ```
 
 <img alt="rclip usage demo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/rclip-usage.gif" width="640px" />
```

### Comparing `rclip-1.4.7a0/pyproject.toml` & `rclip-1.4.7a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.7a0"
+version = "1.4.7a1"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.7a0/rclip/db.py` & `rclip-1.4.7a1/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a0/rclip/main.py` & `rclip-1.4.7a1/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a0/rclip/model.py` & `rclip-1.4.7a1/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a0/rclip/utils.py` & `rclip-1.4.7a1/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a0/PKG-INFO` & `rclip-1.4.7a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.7a0
+Version: 1.4.7a1
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
@@ -59,21 +59,29 @@
   ```bash
   chmod +x <downloaded AppImage filename>
   sudo mv <downloaded AppImage filename> /usr/local/bin/rclip
   ```
 </details>
 
 <details>
-  <summary><strong>macOS/Windows/Linux (using <code>pip</code>)</strong></summary>
+  <summary><strong>macOS/Windows (using <code>pip</code>)</strong></summary>
 
   ```bash
   pip install rclip
   ```
 </details>
 
+<details>
+  <summary><strong>Linux (using <code>pip</code>)</strong></summary>
+
+  ```bash
+  pip install --index-url https://download.pytorch.org/whl/cpu rclip
+  ```
+</details>
+
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
 ```
 
 <img alt="rclip usage demo" src="https://raw.githubusercontent.com/yurijmikhalevich/rclip/main/resources/rclip-usage.gif" width="640px" />
```

