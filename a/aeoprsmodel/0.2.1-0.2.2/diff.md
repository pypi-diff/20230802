# Comparing `tmp/aeoprsmodel-0.2.1.tar.gz` & `tmp/aeoprsmodel-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aeoprsmodel-0.2.1.tar", last modified: Wed Aug  2 14:59:58 2023, max compression
+gzip compressed data, was "dist/aeoprsmodel-0.2.2.tar", last modified: Wed Aug  2 15:08:55 2023, max compression
```

## Comparing `aeoprsmodel-0.2.1.tar` & `aeoprsmodel-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/
--rw-r--r--   0 container   (501) dialout     (20)   246007 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/PKG-INFO
--rw-r--r--   0 container   (501) dialout     (20)   216392 2023-08-02 14:59:53.000000 aeoprsmodel-0.2.1/README.md
--rw-r--r--   0 container   (501) dialout     (20)       38 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/setup.cfg
--rw-r--r--   0 container   (501) dialout     (20)      602 2023-08-02 14:59:53.000000 aeoprsmodel-0.2.1/setup.py
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/src/
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/src/aeoprs/
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/src/aeoprs/core/
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/src/aeoprs/core/models/
--rw-r--r--   0 container   (501) dialout     (20)        0 2023-08-02 14:59:53.000000 aeoprsmodel-0.2.1/src/aeoprs/core/models/__init__.py
--rw-r--r--   0 container   (501) dialout     (20)     2628 2023-08-02 14:59:53.000000 aeoprsmodel-0.2.1/src/aeoprs/core/models/mapper.py
--rw-r--r--   0 container   (501) dialout     (20)    29010 2023-08-02 14:59:53.000000 aeoprsmodel-0.2.1/src/aeoprs/core/models/model.py
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/src/aeoprsmodel.egg-info/
--rw-r--r--   0 container   (501) dialout     (20)   246007 2023-08-02 14:59:57.000000 aeoprsmodel-0.2.1/src/aeoprsmodel.egg-info/PKG-INFO
--rw-r--r--   0 container   (501) dialout     (20)      274 2023-08-02 14:59:58.000000 aeoprsmodel-0.2.1/src/aeoprsmodel.egg-info/SOURCES.txt
--rw-r--r--   0 container   (501) dialout     (20)        1 2023-08-02 14:59:57.000000 aeoprsmodel-0.2.1/src/aeoprsmodel.egg-info/dependency_links.txt
--rw-r--r--   0 container   (501) dialout     (20)        7 2023-08-02 14:59:57.000000 aeoprsmodel-0.2.1/src/aeoprsmodel.egg-info/top_level.txt
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/
+-rw-r--r--   0 container   (501) dialout     (20)   246007 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/PKG-INFO
+-rw-r--r--   0 container   (501) dialout     (20)   216392 2023-08-02 15:08:49.000000 aeoprsmodel-0.2.2/README.md
+-rw-r--r--   0 container   (501) dialout     (20)       38 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/setup.cfg
+-rw-r--r--   0 container   (501) dialout     (20)      602 2023-08-02 15:08:49.000000 aeoprsmodel-0.2.2/setup.py
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprs/
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprs/core/
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprs/core/models/
+-rw-r--r--   0 container   (501) dialout     (20)        0 2023-08-02 15:08:49.000000 aeoprsmodel-0.2.2/src/aeoprs/core/models/__init__.py
+-rw-r--r--   0 container   (501) dialout     (20)     2628 2023-08-02 15:08:49.000000 aeoprsmodel-0.2.2/src/aeoprs/core/models/mapper.py
+-rw-r--r--   0 container   (501) dialout     (20)    28955 2023-08-02 15:08:49.000000 aeoprsmodel-0.2.2/src/aeoprs/core/models/model.py
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprsmodel.egg-info/
+-rw-r--r--   0 container   (501) dialout     (20)   246007 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprsmodel.egg-info/PKG-INFO
+-rw-r--r--   0 container   (501) dialout     (20)      274 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprsmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 container   (501) dialout     (20)        1 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprsmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 container   (501) dialout     (20)        7 2023-08-02 15:08:55.000000 aeoprsmodel-0.2.2/src/aeoprsmodel.egg-info/top_level.txt
```

### Comparing `aeoprsmodel-0.2.1/PKG-INFO` & `aeoprsmodel-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeoprsmodel
-Version: 0.2.1
+Version: 0.2.2
 Summary: ARLAS Earth Observation Product Registration Service Model
 Home-page: UNKNOWN
 Author: Gisaïa
 License: UNKNOWN
 Description: # AEOPRS Model
         
         This package contains the data model for sending requests to ARLAS Earth Observation Product Registration Services.
```

### Comparing `aeoprsmodel-0.2.1/README.md` & `aeoprsmodel-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aeoprsmodel-0.2.1/setup.py` & `aeoprsmodel-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aeoprsmodel",
-    version="0.2.1",                        
+    version="0.2.2",                        
     author="Gisaïa",                     
     description="ARLAS Earth Observation Product Registration Service Model",
     long_description=long_description,      
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    
     python_requires='>=3.11',     
     py_modules=["aeoprs.core.models.model","aeoprs.core.models.mapper"],
```

### Comparing `aeoprsmodel-0.2.1/src/aeoprs/core/models/mapper.py` & `aeoprsmodel-0.2.2/src/aeoprs/core/models/mapper.py`

 * *Files identical despite different names*

### Comparing `aeoprsmodel-0.2.1/src/aeoprs/core/models/model.py` & `aeoprsmodel-0.2.2/src/aeoprs/core/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import json
 from datetime import datetime as Datetime
 from enum import Enum
 from typing import (TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar,
                     Union, cast)
 
 from pydantic import BaseModel, Extra, Field
 from pydantic.fields import FieldInfo
-from pydantic.json import pydantic_encoder
 
 class ProcessingLevel(Enum):
     RAW="RAW"
     L1="L1"
     L2="L2"
     L3="L3"
     L4="L4"
```

### Comparing `aeoprsmodel-0.2.1/src/aeoprsmodel.egg-info/PKG-INFO` & `aeoprsmodel-0.2.2/src/aeoprsmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeoprsmodel
-Version: 0.2.1
+Version: 0.2.2
 Summary: ARLAS Earth Observation Product Registration Service Model
 Home-page: UNKNOWN
 Author: Gisaïa
 License: UNKNOWN
 Description: # AEOPRS Model
         
         This package contains the data model for sending requests to ARLAS Earth Observation Product Registration Services.
```

