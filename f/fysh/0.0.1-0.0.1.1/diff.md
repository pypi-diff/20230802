# Comparing `tmp/fysh-0.0.1.tar.gz` & `tmp/fysh-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fysh-0.0.1.tar", max compression
+gzip compressed data, was "fysh-0.0.1.1.tar", max compression
```

## Comparing `fysh-0.0.1.tar` & `fysh-0.0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3472 2023-08-02 06:33:17.421422 fysh-0.0.1/README.md
--rw-r--r--   0        0        0     1810 2023-08-02 06:33:17.425422 fysh-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      154 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/__init__.py
--rw-r--r--   0        0        0       30 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/__main__.py
--rw-r--r--   0        0        0     3928 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/cli.py
--rw-r--r--   0        0        0     3969 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/asset/asset.py
--rw-r--r--   0        0        0      946 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/asset/image.py
--rw-r--r--   0        0        0        0 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/asset/text.py
--rw-r--r--   0        0        0        0 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/cache/test.py
--rw-r--r--   0        0        0     1407 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/dataset/dataset.py
--rw-r--r--   0        0        0     4852 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/ffysh_pytorch.py
--rw-r--r--   0        0        0     1685 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/internals/api.py
--rw-r--r--   0        0        0     1641 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/internals/authorization.py
--rw-r--r--   0        0        0       45 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/internals/errors.py
--rw-r--r--   0        0        0      456 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/internals/file.py
--rw-r--r--   0        0        0     1531 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/internals/project.py
--rw-r--r--   0        0        0      789 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/pytorch/ffysh_dataset.py
--rw-r--r--   0        0        0      728 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/pytorch/image_dataset.py
--rw-r--r--   0        0        0    18576 2023-08-02 06:33:17.425422 fysh-0.0.1/src/ffysh/modules/stream/stream.py
--rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 fysh-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-08-02 06:43:04.771724 fysh-0.0.1.1/README.md
+-rw-r--r--   0        0        0     1813 2023-08-02 06:43:04.775724 fysh-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/__init__.py
+-rw-r--r--   0        0        0       30 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/__main__.py
+-rw-r--r--   0        0        0     3928 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/cli.py
+-rw-r--r--   0        0        0     3969 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/asset/asset.py
+-rw-r--r--   0        0        0      946 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/asset/image.py
+-rw-r--r--   0        0        0        0 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/asset/text.py
+-rw-r--r--   0        0        0        0 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/cache/test.py
+-rw-r--r--   0        0        0     1407 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/dataset/dataset.py
+-rw-r--r--   0        0        0     4852 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/ffysh_pytorch.py
+-rw-r--r--   0        0        0     1685 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/api.py
+-rw-r--r--   0        0        0     1641 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/authorization.py
+-rw-r--r--   0        0        0       45 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/errors.py
+-rw-r--r--   0        0        0      456 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/file.py
+-rw-r--r--   0        0        0     1531 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/project.py
+-rw-r--r--   0        0        0      789 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/pytorch/ffysh_dataset.py
+-rw-r--r--   0        0        0      728 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/pytorch/image_dataset.py
+-rw-r--r--   0        0        0    18576 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/stream/stream.py
+-rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 fysh-0.0.1.1/PKG-INFO
```

### Comparing `fysh-0.0.1/README.md` & `fysh-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/pyproject.toml` & `fysh-0.0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fysh"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Command Line Interface tool for flockfysh."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/ffysh"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
@@ -51,15 +51,15 @@
 nvidia-nvtx-cu11 = "^11.8.86"
 ordered-set = "^4.1.0"
 pillow = "^10.0.0"
 pipreqs = "^0.4.13"
 psutil = "^5.9.5"
 requests = "^2.31.0"
 sympy = "^1.12"
-torch = "^2.0.1"
+torch = ">=2.0.0"
 torchvision = "^0.15.2"
 triton = "^2.0.0.post1"
 typing-extensions = "^4.7.1"
 urllib3 = "^2.0.4"
 yarg = "^0.1.9"
 yarl = "^1.9.2"
```

### Comparing `fysh-0.0.1/src/ffysh/cli.py` & `fysh-0.0.1.1/src/ffysh/cli.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/asset/asset.py` & `fysh-0.0.1.1/src/ffysh/modules/asset/asset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/asset/image.py` & `fysh-0.0.1.1/src/ffysh/modules/asset/image.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/dataset/dataset.py` & `fysh-0.0.1.1/src/ffysh/modules/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/ffysh_pytorch.py` & `fysh-0.0.1.1/src/ffysh/modules/ffysh_pytorch.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/internals/api.py` & `fysh-0.0.1.1/src/ffysh/modules/internals/api.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/internals/authorization.py` & `fysh-0.0.1.1/src/ffysh/modules/internals/authorization.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/internals/project.py` & `fysh-0.0.1.1/src/ffysh/modules/internals/project.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/pytorch/ffysh_dataset.py` & `fysh-0.0.1.1/src/ffysh/modules/pytorch/ffysh_dataset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/pytorch/image_dataset.py` & `fysh-0.0.1.1/src/ffysh/modules/pytorch/image_dataset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/src/ffysh/modules/stream/stream.py` & `fysh-0.0.1.1/src/ffysh/modules/stream/stream.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1/PKG-INFO` & `fysh-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fysh
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Command Line Interface tool for flockfysh.
 Home-page: https://github.com/flockfysh/ffysh
 License: MIT
 Keywords: files,manipulation,data science
 Author: Ansh
 Author-email: teamnebulaco@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -47,15 +47,15 @@
 Requires-Dist: nvidia-nvtx-cu11 (>=11.8.86,<12.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pipreqs (>=0.4.13,<0.5.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sympy (>=1.12,<2.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torch (>=2.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Requires-Dist: triton (>=2.0.0.post1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: urllib3 (>=2.0.4,<3.0.0)
 Requires-Dist: yarg (>=0.1.9,<0.2.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Repository, https://github.com/flockfysh/ffysh
```

