# Comparing `tmp/aeoprsmodel-0.1.tar.gz` & `tmp/aeoprsmodel-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aeoprsmodel-0.1.tar", last modified: Tue Aug  1 15:33:53 2023, max compression
+gzip compressed data, was "dist/aeoprsmodel-0.2.tar", last modified: Wed Aug  2 09:11:50 2023, max compression
```

## Comparing `aeoprsmodel-0.1.tar` & `aeoprsmodel-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/
--rw-r--r--   0 container   (501) dialout     (20)      425 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/PKG-INFO
--rw-r--r--   0 container   (501) dialout     (20)      132 2023-08-01 15:33:49.000000 aeoprsmodel-0.1/README.md
--rw-r--r--   0 container   (501) dialout     (20)       38 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/setup.cfg
--rw-r--r--   0 container   (501) dialout     (20)      600 2023-08-01 15:33:49.000000 aeoprsmodel-0.1/setup.py
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprs/
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprs/core/
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprs/core/models/
--rw-r--r--   0 container   (501) dialout     (20)        0 2023-08-01 15:33:49.000000 aeoprsmodel-0.1/src/aeoprs/core/models/__init__.py
--rw-r--r--   0 container   (501) dialout     (20)     2640 2023-08-01 15:33:49.000000 aeoprsmodel-0.1/src/aeoprs/core/models/mapper.py
--rw-r--r--   0 container   (501) dialout     (20)    29010 2023-08-01 15:33:49.000000 aeoprsmodel-0.1/src/aeoprs/core/models/model.py
-drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprsmodel.egg-info/
--rw-r--r--   0 container   (501) dialout     (20)      425 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprsmodel.egg-info/PKG-INFO
--rw-r--r--   0 container   (501) dialout     (20)      274 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprsmodel.egg-info/SOURCES.txt
--rw-r--r--   0 container   (501) dialout     (20)        1 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprsmodel.egg-info/dependency_links.txt
--rw-r--r--   0 container   (501) dialout     (20)        7 2023-08-01 15:33:53.000000 aeoprsmodel-0.1/src/aeoprsmodel.egg-info/top_level.txt
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/
+-rw-r--r--   0 container   (501) dialout     (20)      425 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/PKG-INFO
+-rw-r--r--   0 container   (501) dialout     (20)      132 2023-08-02 09:11:46.000000 aeoprsmodel-0.2/README.md
+-rw-r--r--   0 container   (501) dialout     (20)       38 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/setup.cfg
+-rw-r--r--   0 container   (501) dialout     (20)      600 2023-08-02 09:11:46.000000 aeoprsmodel-0.2/setup.py
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprs/
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprs/core/
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprs/core/models/
+-rw-r--r--   0 container   (501) dialout     (20)        0 2023-08-02 09:11:46.000000 aeoprsmodel-0.2/src/aeoprs/core/models/__init__.py
+-rw-r--r--   0 container   (501) dialout     (20)     2628 2023-08-02 09:11:46.000000 aeoprsmodel-0.2/src/aeoprs/core/models/mapper.py
+-rw-r--r--   0 container   (501) dialout     (20)    29010 2023-08-02 09:11:46.000000 aeoprsmodel-0.2/src/aeoprs/core/models/model.py
+drwxr-xr-x   0 container   (501) dialout     (20)        0 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprsmodel.egg-info/
+-rw-r--r--   0 container   (501) dialout     (20)      425 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprsmodel.egg-info/PKG-INFO
+-rw-r--r--   0 container   (501) dialout     (20)      274 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprsmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 container   (501) dialout     (20)        1 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprsmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 container   (501) dialout     (20)        7 2023-08-02 09:11:50.000000 aeoprsmodel-0.2/src/aeoprsmodel.egg-info/top_level.txt
```

### Comparing `aeoprsmodel-0.1/setup.py` & `aeoprsmodel-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aeoprsmodel",
-    version="0.1",                        
+    version="0.2",                        
     author="Gisaïa",                     
     description="ARLAS Earth Observation Product Registration Service Model",
     long_description=long_description,      
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    
     python_requires='>=3.11',     
     py_modules=["aeoprs.core.models.model","aeoprs.core.models.mapper"],
```

### Comparing `aeoprsmodel-0.1/src/aeoprs/core/models/mapper.py` & `aeoprsmodel-0.2/src/aeoprs/core/models/mapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
      Args:
          item (Item): The item
 
      Returns:
          dict: The dictionary. Keys contain : as namespace seperator
      """
-     dictionary=item.model_dump(exclude_unset=True, by_alias=True, exclude_none=True)
+     dictionary=item.dict(exclude_unset=True, by_alias=True, exclude_none=True)
      return __replaceKeys(dictionary, "__", ":")
 
 def to_arlaseo_dict(item: Item)->dict:
      """ create a dictionnary from the Item. Keys contain __ as namespace seperator
 
      Args:
          item (Item): The item
 
      Returns:
          dict: The dictionary. Keys contain __ as namespace seperator
      """
-     dictionary=item.model_dump(exclude_unset=True, by_alias=False, exclude_none=True)
+     dictionary=item.dict(exclude_unset=True, by_alias=False, exclude_none=True)
      return __replaceKeys(dictionary, ":", "__")
 
 def to_arlaseo_json(item: Item)->str:
      """ create a json from the Item. Keys contain __ as namespace seperator
 
      Args:
          item (Item): The item
```

### Comparing `aeoprsmodel-0.1/src/aeoprs/core/models/model.py` & `aeoprsmodel-0.2/src/aeoprs/core/models/model.py`

 * *Files identical despite different names*

