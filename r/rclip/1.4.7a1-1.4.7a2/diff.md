# Comparing `tmp/rclip-1.4.7a1.tar.gz` & `tmp/rclip-1.4.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.7a1.tar", max compression
+gzip compressed data, was "rclip-1.4.7a2.tar", max compression
```

## Comparing `rclip-1.4.7a1.tar` & `rclip-1.4.7a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-02 07:17:11.716274 rclip-1.4.7a1/LICENSE
--rw-r--r--   0        0        0     5194 2023-08-02 07:17:11.716274 rclip-1.4.7a1/README.md
--rw-r--r--   0        0        0     1559 2023-08-02 07:17:11.716274 rclip-1.4.7a1/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/main.py
--rw-r--r--   0        0        0     5212 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/model.py
--rw-r--r--   0        0        0     4746 2023-08-02 07:17:11.716274 rclip-1.4.7a1/rclip/utils.py
--rw-r--r--   0        0        0     6702 1970-01-01 00:00:00.000000 rclip-1.4.7a1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-02 07:22:55.955439 rclip-1.4.7a2/LICENSE
+-rw-r--r--   0        0        0     5249 2023-08-02 07:22:55.955439 rclip-1.4.7a2/README.md
+-rw-r--r--   0        0        0     1559 2023-08-02 07:22:55.955439 rclip-1.4.7a2/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-02 07:22:55.955439 rclip-1.4.7a2/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-02 07:22:55.955439 rclip-1.4.7a2/rclip/main.py
+-rw-r--r--   0        0        0     5212 2023-08-02 07:22:55.955439 rclip-1.4.7a2/rclip/model.py
+-rw-r--r--   0        0        0     4746 2023-08-02 07:22:55.955439 rclip-1.4.7a2/rclip/utils.py
+-rw-r--r--   0        0        0     6757 1970-01-01 00:00:00.000000 rclip-1.4.7a2/PKG-INFO
```

### Comparing `rclip-1.4.7a1/LICENSE` & `rclip-1.4.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a1/README.md` & `rclip-1.4.7a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
   ```
 </details>
 
 <details>
   <summary><strong>Linux (using <code>pip</code>)</strong></summary>
 
   ```bash
-  pip install --index-url https://download.pytorch.org/whl/cpu rclip
+  pip install --index-url https://download.pytorch.org/whl/cpu torch==2.0.1+cpu torchvision==0.15.2+cpu
+  pip install rclip
   ```
 </details>
 
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
```

### Comparing `rclip-1.4.7a1/pyproject.toml` & `rclip-1.4.7a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.7a1"
+version = "1.4.7a2"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.7a1/rclip/db.py` & `rclip-1.4.7a2/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a1/rclip/main.py` & `rclip-1.4.7a2/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a1/rclip/model.py` & `rclip-1.4.7a2/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a1/rclip/utils.py` & `rclip-1.4.7a2/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a1/PKG-INFO` & `rclip-1.4.7a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.7a1
+Version: 1.4.7a2
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
@@ -70,15 +70,16 @@
   ```
 </details>
 
 <details>
   <summary><strong>Linux (using <code>pip</code>)</strong></summary>
 
   ```bash
-  pip install --index-url https://download.pytorch.org/whl/cpu rclip
+  pip install --index-url https://download.pytorch.org/whl/cpu torch==2.0.1+cpu torchvision==0.15.2+cpu
+  pip install rclip
   ```
 </details>
 
 ## Usage
 
 ```bash
 cd photos && rclip "search query"
```

