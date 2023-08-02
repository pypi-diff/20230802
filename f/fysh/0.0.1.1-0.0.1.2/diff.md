# Comparing `tmp/fysh-0.0.1.1.tar.gz` & `tmp/fysh-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fysh-0.0.1.1.tar", max compression
+gzip compressed data, was "fysh-0.0.1.2.tar", max compression
```

## Comparing `fysh-0.0.1.1.tar` & `fysh-0.0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3472 2023-08-02 06:43:04.771724 fysh-0.0.1.1/README.md
--rw-r--r--   0        0        0     1813 2023-08-02 06:43:04.775724 fysh-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0      154 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/__init__.py
--rw-r--r--   0        0        0       30 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/__main__.py
--rw-r--r--   0        0        0     3928 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/cli.py
--rw-r--r--   0        0        0     3969 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/asset/asset.py
--rw-r--r--   0        0        0      946 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/asset/image.py
--rw-r--r--   0        0        0        0 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/asset/text.py
--rw-r--r--   0        0        0        0 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/cache/test.py
--rw-r--r--   0        0        0     1407 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/dataset/dataset.py
--rw-r--r--   0        0        0     4852 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/ffysh_pytorch.py
--rw-r--r--   0        0        0     1685 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/api.py
--rw-r--r--   0        0        0     1641 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/authorization.py
--rw-r--r--   0        0        0       45 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/errors.py
--rw-r--r--   0        0        0      456 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/file.py
--rw-r--r--   0        0        0     1531 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/internals/project.py
--rw-r--r--   0        0        0      789 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/pytorch/ffysh_dataset.py
--rw-r--r--   0        0        0      728 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/pytorch/image_dataset.py
--rw-r--r--   0        0        0    18576 2023-08-02 06:43:04.775724 fysh-0.0.1.1/src/ffysh/modules/stream/stream.py
--rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 fysh-0.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-08-02 06:58:09.224680 fysh-0.0.1.2/README.md
+-rw-r--r--   0        0        0     1814 2023-08-02 06:58:09.224680 fysh-0.0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/__init__.py
+-rw-r--r--   0        0        0       30 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/__main__.py
+-rw-r--r--   0        0        0     3928 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/cli.py
+-rw-r--r--   0        0        0     3969 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/asset/asset.py
+-rw-r--r--   0        0        0      946 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/asset/image.py
+-rw-r--r--   0        0        0        0 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/asset/text.py
+-rw-r--r--   0        0        0        0 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/cache/test.py
+-rw-r--r--   0        0        0     1407 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/dataset/dataset.py
+-rw-r--r--   0        0        0     4852 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/ffysh_pytorch.py
+-rw-r--r--   0        0        0     1685 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/internals/api.py
+-rw-r--r--   0        0        0     1641 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/internals/authorization.py
+-rw-r--r--   0        0        0       45 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/internals/errors.py
+-rw-r--r--   0        0        0      456 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/internals/file.py
+-rw-r--r--   0        0        0     1531 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/internals/project.py
+-rw-r--r--   0        0        0      789 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/pytorch/ffysh_dataset.py
+-rw-r--r--   0        0        0      728 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/pytorch/image_dataset.py
+-rw-r--r--   0        0        0    18576 2023-08-02 06:58:09.228680 fysh-0.0.1.2/src/ffysh/modules/stream/stream.py
+-rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 fysh-0.0.1.2/PKG-INFO
```

### Comparing `fysh-0.0.1.1/README.md` & `fysh-0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/pyproject.toml` & `fysh-0.0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fysh"
-version = "0.0.1.1"
+version = "0.0.1.2"
 description = "Command Line Interface tool for flockfysh."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/ffysh"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
@@ -36,15 +36,15 @@
 lit = "^16.0.6"
 markupsafe = "^2.1.3"
 mpmath = "^1.3.0"
 multidict = "^6.0.4"
 networkx = "^3.1"
 nvidia-cublas-cu11 = "^11.11.3.6"
 nvidia-cuda-cupti-cu11 = "^11.8.87"
-nvidia-cuda-nvrtc-cu11 = "^11.8.89"
+nvidia-cuda-nvrtc-cu11 = "^11.7.89"
 nvidia-cuda-runtime-cu11 = "^11.8.89"
 nvidia-cudnn-cu11 = "^8.9.2.26"
 nvidia-cufft-cu11 = "^10.9.0.58"
 nvidia-curand-cu11 = "^10.3.0.86"
 nvidia-cusolver-cu11 = "^11.4.1.48"
 nvidia-cusparse-cu11 = "^11.7.5.86"
 nvidia-nccl-cu11 = "^2.18.3"
@@ -67,8 +67,8 @@
 pytest = {version="^7.0.1", python = ">=3.7,<4.0"}
 
 [tool.poetry.scripts]
 ffysh = "ffysh.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `fysh-0.0.1.1/src/ffysh/cli.py` & `fysh-0.0.1.2/src/ffysh/cli.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/asset/asset.py` & `fysh-0.0.1.2/src/ffysh/modules/asset/asset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/asset/image.py` & `fysh-0.0.1.2/src/ffysh/modules/asset/image.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/dataset/dataset.py` & `fysh-0.0.1.2/src/ffysh/modules/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/ffysh_pytorch.py` & `fysh-0.0.1.2/src/ffysh/modules/ffysh_pytorch.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/internals/api.py` & `fysh-0.0.1.2/src/ffysh/modules/internals/api.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/internals/authorization.py` & `fysh-0.0.1.2/src/ffysh/modules/internals/authorization.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/internals/project.py` & `fysh-0.0.1.2/src/ffysh/modules/internals/project.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/pytorch/ffysh_dataset.py` & `fysh-0.0.1.2/src/ffysh/modules/pytorch/ffysh_dataset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/pytorch/image_dataset.py` & `fysh-0.0.1.2/src/ffysh/modules/pytorch/image_dataset.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/src/ffysh/modules/stream/stream.py` & `fysh-0.0.1.2/src/ffysh/modules/stream/stream.py`

 * *Files identical despite different names*

### Comparing `fysh-0.0.1.1/PKG-INFO` & `fysh-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fysh
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Command Line Interface tool for flockfysh.
 Home-page: https://github.com/flockfysh/ffysh
 License: MIT
 Keywords: files,manipulation,data science
 Author: Ansh
 Author-email: teamnebulaco@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -32,15 +32,15 @@
 Requires-Dist: lit (>=16.0.6,<17.0.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: mpmath (>=1.3.0,<2.0.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: nvidia-cublas-cu11 (>=11.11.3.6,<12.0.0.0)
 Requires-Dist: nvidia-cuda-cupti-cu11 (>=11.8.87,<12.0.0)
-Requires-Dist: nvidia-cuda-nvrtc-cu11 (>=11.8.89,<12.0.0)
+Requires-Dist: nvidia-cuda-nvrtc-cu11 (>=11.7.89,<12.0.0)
 Requires-Dist: nvidia-cuda-runtime-cu11 (>=11.8.89,<12.0.0)
 Requires-Dist: nvidia-cudnn-cu11 (>=8.9.2.26,<9.0.0.0)
 Requires-Dist: nvidia-cufft-cu11 (>=10.9.0.58,<11.0.0.0)
 Requires-Dist: nvidia-curand-cu11 (>=10.3.0.86,<11.0.0.0)
 Requires-Dist: nvidia-cusolver-cu11 (>=11.4.1.48,<12.0.0.0)
 Requires-Dist: nvidia-cusparse-cu11 (>=11.7.5.86,<12.0.0.0)
 Requires-Dist: nvidia-nccl-cu11 (>=2.18.3,<3.0.0)
```

