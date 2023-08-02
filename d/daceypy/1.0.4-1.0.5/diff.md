# Comparing `tmp/daceypy-1.0.4.tar.gz` & `tmp/daceypy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daceypy-1.0.4.tar", last modified: Sat Jan 28 16:41:04 2023, max compression
+gzip compressed data, was "daceypy-1.0.5.tar", last modified: Wed Aug  2 17:50:14 2023, max compression
```

## Comparing `daceypy-1.0.4.tar` & `daceypy-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-01-28 16:41:04.536665 daceypy-1.0.4/
--rw-r--r--   0 giovanni   (501) staff       (20)    11357 2023-01-25 23:48:41.000000 daceypy-1.0.4/LICENSE
--rw-r--r--   0 giovanni   (501) staff       (20)     1771 2023-01-25 23:48:41.000000 daceypy-1.0.4/NOTICE
--rw-r--r--   0 giovanni   (501) staff       (20)     1803 2023-01-28 16:41:04.536775 daceypy-1.0.4/PKG-INFO
--rw-r--r--   0 giovanni   (501) staff       (20)      881 2023-01-28 16:12:16.000000 daceypy-1.0.4/README.md
-drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-01-28 16:41:04.528047 daceypy-1.0.4/daceypy/
--rw-r--r--   0 giovanni   (501) staff       (20)    82495 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/_DA.py
--rw-r--r--   0 giovanni   (501) staff       (20)     8058 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/_DACEException.py
--rw-r--r--   0 giovanni   (501) staff       (20)     1858 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/_Monomial.py
--rw-r--r--   0 giovanni   (501) staff       (20)      983 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/_PrettyType.py
--rw-r--r--   0 giovanni   (501) staff       (20)     1355 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/__init__.py
--rw-r--r--   0 giovanni   (501) staff       (20)    35563 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/_array.py
--rw-r--r--   0 giovanni   (501) staff       (20)    10743 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/_compiledDA.py
--rw-r--r--   0 giovanni   (501) staff       (20)       22 2023-01-28 16:12:35.000000 daceypy-1.0.4/daceypy/_version.py
--rw-r--r--   0 giovanni   (501) staff       (20)    24319 2023-01-28 12:43:16.000000 daceypy-1.0.4/daceypy/core.py
--rw-r--r--   0 giovanni   (501) staff       (20)     2078 2023-01-28 13:19:22.000000 daceypy-1.0.4/daceypy/get_platform.py
-drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-01-28 16:41:04.536413 daceypy-1.0.4/daceypy/lib/
--rwxr-xr-x   0 giovanni   (501) staff       (20)   109486 2023-01-28 12:57:41.000000 daceypy-1.0.4/daceypy/lib/dace_darwin-arm64.dylib
--rw-r--r--   0 giovanni   (501) staff       (20)   125048 2023-01-28 12:40:34.000000 daceypy-1.0.4/daceypy/lib/dace_darwin-x86_64.dylib
--rwxr-xr-x   0 giovanni   (501) staff       (20)    98760 2023-01-28 13:23:30.000000 daceypy-1.0.4/daceypy/lib/dace_linux-aarch64.so
--rw-r--r--   0 giovanni   (501) staff       (20)   105204 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/lib/dace_linux-i686.so
--rw-r--r--   0 giovanni   (501) staff       (20)   108760 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/lib/dace_linux-x86_64.so
--rw-------   0 giovanni   (501) staff       (20)    71168 2023-01-28 13:05:02.000000 daceypy-1.0.4/daceypy/lib/dace_windows-arm64.dll
--rw-r--r--   0 giovanni   (501) staff       (20)    84992 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/lib/dace_windows-x64.dll
--rw-r--r--   0 giovanni   (501) staff       (20)    72704 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/lib/dace_windows-x86.dll
--rw-r--r--   0 giovanni   (501) staff       (20)    14173 2023-01-25 23:48:41.000000 daceypy-1.0.4/daceypy/op.py
-drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-01-28 16:41:04.530173 daceypy-1.0.4/daceypy.egg-info/
--rw-r--r--   0 giovanni   (501) staff       (20)     1803 2023-01-28 16:41:04.000000 daceypy-1.0.4/daceypy.egg-info/PKG-INFO
--rw-r--r--   0 giovanni   (501) staff       (20)      695 2023-01-28 16:41:04.000000 daceypy-1.0.4/daceypy.egg-info/SOURCES.txt
--rw-r--r--   0 giovanni   (501) staff       (20)        1 2023-01-28 16:41:04.000000 daceypy-1.0.4/daceypy.egg-info/dependency_links.txt
--rw-r--r--   0 giovanni   (501) staff       (20)       14 2023-01-28 16:41:04.000000 daceypy-1.0.4/daceypy.egg-info/requires.txt
--rw-r--r--   0 giovanni   (501) staff       (20)        8 2023-01-28 16:41:04.000000 daceypy-1.0.4/daceypy.egg-info/top_level.txt
--rw-r--r--   0 giovanni   (501) staff       (20)       81 2023-01-25 23:48:41.000000 daceypy-1.0.4/pyproject.toml
--rw-r--r--   0 giovanni   (501) staff       (20)      995 2023-01-28 16:41:04.537097 daceypy-1.0.4/setup.cfg
+drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-08-02 17:50:14.736939 daceypy-1.0.5/
+-rw-r--r--   0 giovanni   (501) staff       (20)    11357 2023-01-25 23:48:41.000000 daceypy-1.0.5/LICENSE
+-rw-r--r--   0 giovanni   (501) staff       (20)     1771 2023-01-25 23:48:41.000000 daceypy-1.0.5/NOTICE
+-rw-r--r--   0 giovanni   (501) staff       (20)     1803 2023-08-02 17:50:14.737017 daceypy-1.0.5/PKG-INFO
+-rw-r--r--   0 giovanni   (501) staff       (20)      881 2023-08-02 17:17:58.000000 daceypy-1.0.5/README.md
+drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-08-02 17:50:14.732710 daceypy-1.0.5/daceypy/
+-rw-r--r--   0 giovanni   (501) staff       (20)    82466 2023-08-02 17:45:34.000000 daceypy-1.0.5/daceypy/_DA.py
+-rw-r--r--   0 giovanni   (501) staff       (20)     8058 2023-01-25 23:48:41.000000 daceypy-1.0.5/daceypy/_DACEException.py
+-rw-r--r--   0 giovanni   (501) staff       (20)     1858 2023-01-25 23:48:41.000000 daceypy-1.0.5/daceypy/_Monomial.py
+-rw-r--r--   0 giovanni   (501) staff       (20)      983 2023-01-25 23:48:41.000000 daceypy-1.0.5/daceypy/_PrettyType.py
+-rw-r--r--   0 giovanni   (501) staff       (20)     1355 2023-08-02 17:17:58.000000 daceypy-1.0.5/daceypy/__init__.py
+-rw-r--r--   0 giovanni   (501) staff       (20)    35563 2023-08-02 17:17:58.000000 daceypy-1.0.5/daceypy/_array.py
+-rw-r--r--   0 giovanni   (501) staff       (20)    10743 2023-01-25 23:48:41.000000 daceypy-1.0.5/daceypy/_compiledDA.py
+-rw-r--r--   0 giovanni   (501) staff       (20)       22 2023-08-02 17:45:34.000000 daceypy-1.0.5/daceypy/_version.py
+-rw-r--r--   0 giovanni   (501) staff       (20)    24319 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/core.py
+-rw-r--r--   0 giovanni   (501) staff       (20)     2078 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/get_platform.py
+drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-08-02 17:50:14.736685 daceypy-1.0.5/daceypy/lib/
+-rwxr-xr-x   0 giovanni   (501) staff       (20)   109486 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_darwin-arm64.dylib
+-rw-r--r--   0 giovanni   (501) staff       (20)   125048 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_darwin-x86_64.dylib
+-rwxr-xr-x   0 giovanni   (501) staff       (20)    98760 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_linux-aarch64.so
+-rw-r--r--   0 giovanni   (501) staff       (20)   105204 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_linux-i686.so
+-rw-r--r--   0 giovanni   (501) staff       (20)   108760 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_linux-x86_64.so
+-rw-r--r--   0 giovanni   (501) staff       (20)    71168 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_windows-arm64.dll
+-rw-r--r--   0 giovanni   (501) staff       (20)    84992 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_windows-x64.dll
+-rw-r--r--   0 giovanni   (501) staff       (20)    72704 2023-01-28 16:57:58.000000 daceypy-1.0.5/daceypy/lib/dace_windows-x86.dll
+-rw-r--r--   0 giovanni   (501) staff       (20)    14173 2023-01-25 23:48:41.000000 daceypy-1.0.5/daceypy/op.py
+drwxr-xr-x   0 giovanni   (501) staff       (20)        0 2023-08-02 17:50:14.733449 daceypy-1.0.5/daceypy.egg-info/
+-rw-r--r--   0 giovanni   (501) staff       (20)     1803 2023-08-02 17:50:14.000000 daceypy-1.0.5/daceypy.egg-info/PKG-INFO
+-rw-r--r--   0 giovanni   (501) staff       (20)      695 2023-08-02 17:50:14.000000 daceypy-1.0.5/daceypy.egg-info/SOURCES.txt
+-rw-r--r--   0 giovanni   (501) staff       (20)        1 2023-08-02 17:50:14.000000 daceypy-1.0.5/daceypy.egg-info/dependency_links.txt
+-rw-r--r--   0 giovanni   (501) staff       (20)       14 2023-08-02 17:50:14.000000 daceypy-1.0.5/daceypy.egg-info/requires.txt
+-rw-r--r--   0 giovanni   (501) staff       (20)        8 2023-08-02 17:50:14.000000 daceypy-1.0.5/daceypy.egg-info/top_level.txt
+-rw-r--r--   0 giovanni   (501) staff       (20)       81 2023-01-25 23:48:41.000000 daceypy-1.0.5/pyproject.toml
+-rw-r--r--   0 giovanni   (501) staff       (20)      995 2023-08-02 17:50:14.737265 daceypy-1.0.5/setup.cfg
```

### Comparing `daceypy-1.0.4/LICENSE` & `daceypy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/NOTICE` & `daceypy-1.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/PKG-INFO` & `daceypy-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daceypy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python wrapper of DACE, the Differential Algebra Computational Toolbox.
 Home-page: https://github.com/giovannipurpura/daceypy
 Author: Giovanni Purpura
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `daceypy-1.0.4/README.md` & `daceypy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/_DA.py` & `daceypy-1.0.5/daceypy/_DA.py`

 * *Files 1% similar despite different names*

```diff
@@ -792,31 +792,31 @@
     def assign(self, *args, **kwargs) -> None:
         i = c = da = None
 
         # Process keyword arguments
         for kw, val in kwargs.items():
             if kw == "i":
                 i = val
-                if not isinstance(i, int) or i is not None:
+                if not isinstance(i, int):
                     raise TypeError(
                         "Keyword argument i must be of type int, "
-                        f"(\"{type(i)}\") was given")
+                        f"\"{type(i).__name__}\" was given")
             elif kw == "c":
                 c = val
-                if not isinstance(c, float) or c is not None:
+                if not isinstance(c, float):
                     raise TypeError(
                         "Keyword argument c must be of type float, "
-                        f"(\"{type(c)}\") was given")
+                        f"\"{type(c).__name__}\" was given")
             elif kw == "da":
                 da = val
-                if not isinstance(c, (DA, bytes, str)) or c is not None:
+                if not isinstance(da, (DA, bytes, str)):
                     raise TypeError(
                         "Keyword argument da must be of type "
                         "DA or bytes or str, "
-                        f"(\"{type(da)}\") was given")
+                        f"\"{type(da).__name__}\" was given")
                 if args or len(kwargs) > 1:
                     raise TypeError(
                         "No other argument can be passed when da is used")
             else:
                 raise TypeError(f"Unexpected keyword argument '{kw}'")
 
         # Get positional arguments
```

### Comparing `daceypy-1.0.4/daceypy/_DACEException.py` & `daceypy-1.0.5/daceypy/_DACEException.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/_Monomial.py` & `daceypy-1.0.5/daceypy/_Monomial.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/_PrettyType.py` & `daceypy-1.0.5/daceypy/_PrettyType.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/__init__.py` & `daceypy-1.0.5/daceypy/__init__.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/_array.py` & `daceypy-1.0.5/daceypy/_array.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/_compiledDA.py` & `daceypy-1.0.5/daceypy/_compiledDA.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/core.py` & `daceypy-1.0.5/daceypy/core.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/get_platform.py` & `daceypy-1.0.5/daceypy/get_platform.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_darwin-arm64.dylib` & `daceypy-1.0.5/daceypy/lib/dace_darwin-arm64.dylib`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_darwin-x86_64.dylib` & `daceypy-1.0.5/daceypy/lib/dace_darwin-x86_64.dylib`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_linux-aarch64.so` & `daceypy-1.0.5/daceypy/lib/dace_linux-aarch64.so`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_linux-i686.so` & `daceypy-1.0.5/daceypy/lib/dace_linux-i686.so`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_linux-x86_64.so` & `daceypy-1.0.5/daceypy/lib/dace_linux-x86_64.so`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_windows-arm64.dll` & `daceypy-1.0.5/daceypy/lib/dace_windows-arm64.dll`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_windows-x64.dll` & `daceypy-1.0.5/daceypy/lib/dace_windows-x64.dll`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/lib/dace_windows-x86.dll` & `daceypy-1.0.5/daceypy/lib/dace_windows-x86.dll`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy/op.py` & `daceypy-1.0.5/daceypy/op.py`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/daceypy.egg-info/PKG-INFO` & `daceypy-1.0.5/daceypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daceypy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python wrapper of DACE, the Differential Algebra Computational Toolbox.
 Home-page: https://github.com/giovannipurpura/daceypy
 Author: Giovanni Purpura
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `daceypy-1.0.4/daceypy.egg-info/SOURCES.txt` & `daceypy-1.0.5/daceypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daceypy-1.0.4/setup.cfg` & `daceypy-1.0.5/setup.cfg`

 * *Files identical despite different names*

