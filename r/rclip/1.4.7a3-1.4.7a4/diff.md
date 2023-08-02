# Comparing `tmp/rclip-1.4.7a3.tar.gz` & `tmp/rclip-1.4.7a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.7a3.tar", max compression
+gzip compressed data, was "rclip-1.4.7a4.tar", max compression
```

## Comparing `rclip-1.4.7a3.tar` & `rclip-1.4.7a4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-02 07:26:10.701555 rclip-1.4.7a3/LICENSE
--rw-r--r--   0        0        0     5249 2023-08-02 07:26:10.701555 rclip-1.4.7a3/README.md
--rw-r--r--   0        0        0     1559 2023-08-02 07:26:10.701555 rclip-1.4.7a3/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-02 07:26:10.701555 rclip-1.4.7a3/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-02 07:26:10.701555 rclip-1.4.7a3/rclip/main.py
--rw-r--r--   0        0        0     5212 2023-08-02 07:26:10.701555 rclip-1.4.7a3/rclip/model.py
--rw-r--r--   0        0        0     4746 2023-08-02 07:26:10.701555 rclip-1.4.7a3/rclip/utils.py
--rw-r--r--   0        0        0     6757 1970-01-01 00:00:00.000000 rclip-1.4.7a3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-02 07:29:55.723745 rclip-1.4.7a4/LICENSE
+-rw-r--r--   0        0        0     5249 2023-08-02 07:29:55.723745 rclip-1.4.7a4/README.md
+-rw-r--r--   0        0        0     1559 2023-08-02 07:29:55.723745 rclip-1.4.7a4/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-02 07:29:55.723745 rclip-1.4.7a4/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-02 07:29:55.723745 rclip-1.4.7a4/rclip/main.py
+-rw-r--r--   0        0        0     5212 2023-08-02 07:29:55.723745 rclip-1.4.7a4/rclip/model.py
+-rw-r--r--   0        0        0     4746 2023-08-02 07:29:55.723745 rclip-1.4.7a4/rclip/utils.py
+-rw-r--r--   0        0        0     6757 1970-01-01 00:00:00.000000 rclip-1.4.7a4/PKG-INFO
```

### Comparing `rclip-1.4.7a3/LICENSE` & `rclip-1.4.7a4/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a3/README.md` & `rclip-1.4.7a4/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a3/pyproject.toml` & `rclip-1.4.7a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.7a3"
+version = "1.4.7a4"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.7a3/rclip/db.py` & `rclip-1.4.7a4/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a3/rclip/main.py` & `rclip-1.4.7a4/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a3/rclip/model.py` & `rclip-1.4.7a4/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a3/rclip/utils.py` & `rclip-1.4.7a4/rclip/utils.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.7a3/PKG-INFO` & `rclip-1.4.7a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.7a3
+Version: 1.4.7a4
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
```

