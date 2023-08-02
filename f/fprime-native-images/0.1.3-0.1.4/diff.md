# Comparing `tmp/fprime-native-images-0.1.3.tar.gz` & `tmp/fprime-native-images-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-native-images-0.1.3.tar", last modified: Wed Aug  2 17:55:18 2023, max compression
+gzip compressed data, was "fprime-native-images-0.1.4.tar", last modified: Wed Aug  2 18:55:12 2023, max compression
```

## Comparing `fprime-native-images-0.1.3.tar` & `fprime-native-images-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.822933 fprime-native-images-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/.github/workflows/native-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/env-setup
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/java
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/native-images
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/publish
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.822933 fprime-native-images-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/src/fprime_native_images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/src/fprime_native_images/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/templates/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.200608 fprime-native-images-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.192608 fprime-native-images-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.196608 fprime-native-images-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/.github/workflows/native-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 18:55:12.200608 fprime-native-images-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/env-setup
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/native-images
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/publish
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:55:12.200608 fprime-native-images-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.192608 fprime-native-images-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.196608 fprime-native-images-0.1.4/src/fprime_native_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/src/fprime_native_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/src/fprime_native_images/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/src/fprime_native_images/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/src/fprime_native_images/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.200608 fprime-native-images-0.1.4/src/fprime_native_images/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 18:55:02.000000 fprime-native-images-0.1.4/src/fprime_native_images/templates/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:12.200608 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 18:55:12.000000 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 18:55:12.000000 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:55:12.000000 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 18:55:12.000000 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 18:55:12.000000 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 18:55:12.000000 fprime-native-images-0.1.4/src/fprime_native_images.egg-info/top_level.txt
```

### Comparing `fprime-native-images-0.1.3/.github/workflows/native-build.yml` & `fprime-native-images-0.1.4/.github/workflows/native-build.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/.github/workflows/publish.yml` & `fprime-native-images-0.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/LICENSE` & `fprime-native-images-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/action.yml` & `fprime-native-images-0.1.4/action.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/env-setup` & `fprime-native-images-0.1.4/env-setup`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/native-images` & `fprime-native-images-0.1.4/native-images`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/publish` & `fprime-native-images-0.1.4/publish`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/pyproject.toml` & `fprime-native-images-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Developers",
 ]
 dependencies = [
     "Jinja2>=2.11.3",
     "build",
     'importlib-metadata; python_version<"3.8"',
 ]
-version="0.1.3"
+version="0.1.4"
 
 [project.scripts]
 fprime-native-packager="fprime_native_images.__main__:main"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `fprime-native-images-0.1.3/src/fprime_native_images/__main__.py` & `fprime-native-images-0.1.4/src/fprime_native_images/__main__.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/src/fprime_native_images/jar.py` & `fprime-native-images-0.1.4/src/fprime_native_images/jar.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/src/fprime_native_images/package.py` & `fprime-native-images-0.1.4/src/fprime_native_images/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import platform
+import stat
 import sys
 import subprocess
 from pathlib import Path
 from typing import List, Union
 
 from jinja2 import Environment, PackageLoader
 
@@ -32,15 +32,15 @@
         if tool.suffix not in extensions:
             print(f"[INFO] Skipping {tool} with unaccepted extension")
             continue
         print(f"[INFO] Building package around {tool} with tag {package_tag}")
         directory = generate_tool_package(tool, environment, working)
         # Patch for +x ensuring tools are executable
         st = os.stat(str(tool.resolve()))
-        os.chmod(str(tool.resolve()), st.st_mode | st.S_IEXEC)
+        os.chmod(str(tool.resolve()), st.st_mode | stat.S_IEXEC)
         build_wheel(directory, outdir, package_tag)
 
 
 def generate_tool_package(tool: Path, environment: Environment, working: Path) -> Path:
     """ Build a PIP package for a given tool
 
     Builds a package for a given tool using setuptools. This wraps the setup call suplying the given package and given
```

### Comparing `fprime-native-images-0.1.3/src/fprime_native_images/templates/setup.py.j2` & `fprime-native-images-0.1.4/src/fprime_native_images/templates/setup.py.j2`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.3/src/fprime_native_images.egg-info/SOURCES.txt` & `fprime-native-images-0.1.4/src/fprime_native_images.egg-info/SOURCES.txt`

 * *Files identical despite different names*

