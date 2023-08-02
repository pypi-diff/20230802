# Comparing `tmp/kaparoo_python-0.1.2.tar.gz` & `tmp/kaparoo_python-0.1.3.tar.gz`

## Comparing `kaparoo_python-0.1.2.tar` & `kaparoo_python-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/beartype/__init__.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/beartype/numerics.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/directory.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/existence.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/utils/optional.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/utils/types.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/LICENSE
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/README.md
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/beartype/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/beartype/numerics.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/filesystem/directory.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/filesystem/existence.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/filesystem/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/kaparoo/utils/types.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/README.md
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 kaparoo_python-0.1.3/PKG-INFO
```

### Comparing `kaparoo_python-0.1.2/kaparoo/beartype/numerics.py` & `kaparoo_python-0.1.3/kaparoo/beartype/numerics.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/kaparoo/filesystem/__init__.py` & `kaparoo_python-0.1.3/kaparoo/filesystem/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
     "dir_exists",
     "dirs_exist",
     "file_exists",
     "files_exist",
     "path_exists",
     "paths_exist",
     # directory
-    "empty_dir",
-    "empty_dirs",
+    "dir_empty",
+    "dirs_empty",
     "get_dirs",
     "get_files",
     "get_paths",
     "make_dirs",
 )
 
 from kaparoo.filesystem.directory import (
-    empty_dir,
-    empty_dirs,
+    dir_empty,
+    dirs_empty,
     get_dirs,
     get_files,
     get_paths,
     make_dirs,
 )
 from kaparoo.filesystem.exceptions import (
     AbsolutePathError,
```

### Comparing `kaparoo_python-0.1.2/kaparoo/filesystem/directory.py` & `kaparoo_python-0.1.3/kaparoo/filesystem/directory.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 
 __all__ = (
     # create
     "make_dirs",
     # empty
-    "empty_dir",
-    "empty_dirs",
+    "dir_empty",
+    "dirs_empty",
     # search
     "get_paths",
     "get_files",
     "get_dirs",
 )
 
 import os
@@ -62,42 +62,42 @@
 
 
 # ========================== #
 #            Empty           #
 # ========================== #
 
 
-def empty_dir_unsafe(path: StrPath) -> bool:
+def dir_empty_unsafe(path: StrPath) -> bool:
     return not os.listdir(path)
 
 
-def empty_dirs_unsafe(*paths: StrPath, root: StrPath | None = None) -> bool:
+def dirs_empty_unsafe(*paths: StrPath, root: StrPath | None = None) -> bool:
     if root is not None:
         paths = tuple(os.path.join(root, p) for p in paths)
-    return all(empty_dir_unsafe(p) for p in paths)
+    return all(dir_empty_unsafe(p) for p in paths)
 
 
-def empty_dir(path: StrPath) -> bool:
+def dir_empty(path: StrPath) -> bool:
     """Check if a given directory is empty.
 
     Args:
         path: The directory path to check for emptiness.
 
     Returns:
         True if the directory is empty, False otherwise.
 
     Raises:
         DirectoryNotFoundError: If the path does not exist.
         NotADirectoryError: If the path exists but is not a directory.
     """
     path = check_if_dir_exists(path)
-    return empty_dir_unsafe(path)
+    return dir_empty_unsafe(path)
 
 
-def empty_dirs(*paths: StrPath, root: StrPath | None = None) -> bool:
+def dirs_empty(*paths: StrPath, root: StrPath | None = None) -> bool:
     """Check if all the given directories are empty.
 
     Args:
         *paths: Multiple directory paths to check for emptiness.
         root: The root directory to resolve relative paths. If provided, all paths
             will be resolved relative to the `root` directory. Defaults to None.
 
@@ -108,15 +108,15 @@
         AbsolutePathError: If `root` is given and any of `paths` is an absolute path.
         DirectoryNotFoundError: If the root directory does not exist.
         DirectoryNotFoundError: If any of `paths` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
         NotADirectoryError: If any of `paths` exists but is not a directory.
     """
     paths = check_if_dirs_exist(*paths, root=root)
-    return all(empty_dir_unsafe(p) for p in paths)
+    return all(dir_empty_unsafe(p) for p in paths)
 
 
 # ========================== #
 #           Search           #
 # ========================== #
 
 
@@ -202,16 +202,15 @@
     """
 
     root = check_if_dir_exists(root)
 
     if not isinstance(pattern, str):
         pattern = "*"
 
-    matched = root.rglob(pattern) if recursive else root.glob(pattern)
-    paths = [p for p in matched]
+    paths = list(root.rglob(pattern) if recursive else root.glob(pattern))
 
     if root in paths:
         paths.remove(root)
 
     if not ignores:
         ignores = []
 
@@ -319,17 +318,17 @@
         file_condition = lambda p: p.is_file()  # noqa: E731
     else:
         file_condition = lambda p: p.is_file() and condition(p)  # type: ignore[misc] # noqa: E501, E731
 
     file_paths = get_paths(
         root,
         pattern=pattern,
-        num_samples=num_samples,
         ignores=ignores,
         condition=file_condition,
+        num_samples=num_samples,
         recursive=recursive,
         stringify=stringify,
     )
 
     return file_paths
 
 
@@ -418,15 +417,15 @@
         dir_condition = lambda p: p.is_dir()  # noqa: E731
     else:
         dir_condition = lambda p: p.is_dir() and condition(p)  # type: ignore[misc] # noqa: E501, E731
 
     dir_paths = get_paths(
         root,
         pattern=pattern,
-        num_samples=num_samples,
         ignores=ignores,
         condition=dir_condition,
+        num_samples=num_samples,
         recursive=recursive,
         stringify=stringify,
     )
 
     return dir_paths
```

### Comparing `kaparoo_python-0.1.2/kaparoo/filesystem/exceptions.py` & `kaparoo_python-0.1.3/kaparoo/filesystem/exceptions.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/kaparoo/filesystem/existence.py` & `kaparoo_python-0.1.3/kaparoo/filesystem/existence.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/kaparoo/filesystem/utils.py` & `kaparoo_python-0.1.3/kaparoo/filesystem/utils.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/kaparoo/utils/optional.py` & `kaparoo_python-0.1.3/kaparoo/utils/optional.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/.gitignore` & `kaparoo_python-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/LICENSE` & `kaparoo_python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/README.md` & `kaparoo_python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/pyproject.toml` & `kaparoo_python-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.2/PKG-INFO` & `kaparoo_python-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

