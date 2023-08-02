# Comparing `tmp/pyuul_kmeans-0.0.1.tar.gz` & `tmp/pyuul_kmeans-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuul_kmeans-0.0.1.tar", last modified: Wed Aug  2 09:29:12 2023, max compression
+gzip compressed data, was "pyuul_kmeans-0.0.2.tar", last modified: Wed Aug  2 10:33:42 2023, max compression
```

## Comparing `pyuul_kmeans-0.0.1.tar` & `pyuul_kmeans-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 09:29:12.379416 pyuul_kmeans-0.0.1/
--rw-rw-r--   0 ouc       (1000) ouc       (1000)     1073 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/LICENSE
--rw-rw-r--   0 ouc       (1000) ouc       (1000)      891 2023-08-02 09:29:12.379416 pyuul_kmeans-0.0.1/PKG-INFO
--rw-rw-r--   0 ouc       (1000) ouc       (1000)       53 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/README.rst
-drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 09:29:12.379416 pyuul_kmeans-0.0.1/pyuul_kmeans/
--rw-rw-r--   0 ouc       (1000) ouc       (1000)    23722 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/pyuul_kmeans/VolumeMaker.py
--rw-rw-r--   0 ouc       (1000) ouc       (1000)        1 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/pyuul_kmeans/__init__.py
-drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 09:29:12.379416 pyuul_kmeans-0.0.1/pyuul_kmeans/sources/
--rw-rw-r--   0 ouc       (1000) ouc       (1000)        1 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/pyuul_kmeans/sources/__init__.py
--rw-rw-r--   0 ouc       (1000) ouc       (1000)      805 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/pyuul_kmeans/sources/globalVariables.py
--rw-rw-r--   0 ouc       (1000) ouc       (1000)    13128 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/pyuul_kmeans/sources/hashings.py
--rw-rw-r--   0 ouc       (1000) ouc       (1000)    13069 2023-08-02 09:27:18.000000 pyuul_kmeans-0.0.1/pyuul_kmeans/utils.py
-drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 09:29:12.379416 pyuul_kmeans-0.0.1/pyuul_kmeans.egg-info/
--rw-rw-r--   0 ouc       (1000) ouc       (1000)      891 2023-08-02 09:29:12.000000 pyuul_kmeans-0.0.1/pyuul_kmeans.egg-info/PKG-INFO
--rw-rw-r--   0 ouc       (1000) ouc       (1000)      352 2023-08-02 09:29:12.000000 pyuul_kmeans-0.0.1/pyuul_kmeans.egg-info/SOURCES.txt
--rw-rw-r--   0 ouc       (1000) ouc       (1000)        1 2023-08-02 09:29:12.000000 pyuul_kmeans-0.0.1/pyuul_kmeans.egg-info/dependency_links.txt
--rw-rw-r--   0 ouc       (1000) ouc       (1000)       13 2023-08-02 09:29:12.000000 pyuul_kmeans-0.0.1/pyuul_kmeans.egg-info/top_level.txt
--rw-rw-r--   0 ouc       (1000) ouc       (1000)       38 2023-08-02 09:29:12.379416 pyuul_kmeans-0.0.1/setup.cfg
--rw-rw-r--   0 ouc       (1000) ouc       (1000)     1189 2023-08-02 09:29:10.000000 pyuul_kmeans-0.0.1/setup.py
+drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 10:33:42.689345 pyuul_kmeans-0.0.2/
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)     1073 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/LICENSE
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)      891 2023-08-02 10:33:42.689345 pyuul_kmeans-0.0.2/PKG-INFO
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)       53 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/README.rst
+drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 10:33:42.689345 pyuul_kmeans-0.0.2/pyuul_kmeans/
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)    23729 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/pyuul_kmeans/VolumeMaker.py
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)        1 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/pyuul_kmeans/__init__.py
+drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 10:33:42.689345 pyuul_kmeans-0.0.2/pyuul_kmeans/sources/
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)        1 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/pyuul_kmeans/sources/__init__.py
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)      805 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/pyuul_kmeans/sources/globalVariables.py
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)    13128 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/pyuul_kmeans/sources/hashings.py
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)    13083 2023-08-02 10:32:49.000000 pyuul_kmeans-0.0.2/pyuul_kmeans/utils.py
+drwxrwxr-x   0 ouc       (1000) ouc       (1000)        0 2023-08-02 10:33:42.689345 pyuul_kmeans-0.0.2/pyuul_kmeans.egg-info/
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)      891 2023-08-02 10:33:42.000000 pyuul_kmeans-0.0.2/pyuul_kmeans.egg-info/PKG-INFO
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)      352 2023-08-02 10:33:42.000000 pyuul_kmeans-0.0.2/pyuul_kmeans.egg-info/SOURCES.txt
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)        1 2023-08-02 10:33:42.000000 pyuul_kmeans-0.0.2/pyuul_kmeans.egg-info/dependency_links.txt
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)       13 2023-08-02 10:33:42.000000 pyuul_kmeans-0.0.2/pyuul_kmeans.egg-info/top_level.txt
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)       38 2023-08-02 10:33:42.689345 pyuul_kmeans-0.0.2/setup.cfg
+-rw-rw-r--   0 ouc       (1000) ouc       (1000)     1189 2023-08-02 10:33:37.000000 pyuul_kmeans-0.0.2/setup.py
```

### Comparing `pyuul_kmeans-0.0.1/LICENSE` & `pyuul_kmeans-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuul_kmeans-0.0.1/PKG-INFO` & `pyuul_kmeans-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuul_kmeans
-Version: 0.0.1
+Version: 0.0.2
 Summary: pyuul_kmeans
 Home-page: https://github.com/
 Author: Cheng Ge
 Author-email: 13851520957@163.com
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `pyuul_kmeans-0.0.1/pyuul_kmeans/VolumeMaker.py` & `pyuul_kmeans-0.0.2/pyuul_kmeans/VolumeMaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import torch,math
-from pyuul.sources.globalVariables import *
+from pyuul_kmeans.sources.globalVariables import *
 
 import numpy as np
 import random
 
 def setup_seed(seed):
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
```

### Comparing `pyuul_kmeans-0.0.1/pyuul_kmeans/sources/globalVariables.py` & `pyuul_kmeans-0.0.2/pyuul_kmeans/sources/globalVariables.py`

 * *Files identical despite different names*

### Comparing `pyuul_kmeans-0.0.1/pyuul_kmeans/sources/hashings.py` & `pyuul_kmeans-0.0.2/pyuul_kmeans/sources/hashings.py`

 * *Files identical despite different names*

### Comparing `pyuul_kmeans-0.0.1/pyuul_kmeans/utils.py` & `pyuul_kmeans-0.0.2/pyuul_kmeans/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import os,torch
-from pyuul.sources.globalVariables import *
-from pyuul.sources import  hashings
+from pyuul_kmeans.sources.globalVariables import *
+from pyuul_kmeans.sources import  hashings
 
 import numpy as np
 import random
 
 def setup_seed(seed):
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
```

### Comparing `pyuul_kmeans-0.0.1/pyuul_kmeans.egg-info/PKG-INFO` & `pyuul_kmeans-0.0.2/pyuul_kmeans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuul-kmeans
-Version: 0.0.1
+Version: 0.0.2
 Summary: pyuul_kmeans
 Home-page: https://github.com/
 Author: Cheng Ge
 Author-email: 13851520957@163.com
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `pyuul_kmeans-0.0.1/setup.py` & `pyuul_kmeans-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 setup(name="pyuul_kmeans",
-      version="0.0.1",
+      version="0.0.2",
       description="pyuul_kmeans",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/",
       author="Cheng Ge",
       author_email="13851520957@163.com",
       install_requires=[],
```

