# Comparing `tmp/cached_path-1.3.5.tar.gz` & `tmp/cached_path-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cached_path-1.3.5.tar", last modified: Sat Jul 15 16:22:22 2023, max compression
+gzip compressed data, was "cached_path-1.4.0.tar", last modified: Wed Aug  2 15:47:09 2023, max compression
```

## Comparing `cached_path-1.3.5.tar` & `cached_path-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.888085 cached_path-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-15 16:21:43.000000 cached_path-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-15 16:22:22.884085 cached_path-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-15 16:21:43.000000 cached_path-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.884085 cached_path-1.3.5/cached_path/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/_cached_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/cache_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.884085 cached_path-1.3.5/cached_path/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/beaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/scheme_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.884085 cached_path-1.3.5/cached_path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-15 16:21:43.000000 cached_path-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:22:22.888085 cached_path-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-15 16:21:43.000000 cached_path-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:47:09.449977 cached_path-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-08-02 15:46:31.000000 cached_path-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-02 15:47:09.449977 cached_path-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-08-02 15:46:31.000000 cached_path-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:47:09.445978 cached_path-1.4.0/cached_path/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/_cached_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/cache_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:47:09.449977 cached_path-1.4.0/cached_path/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/beaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/schemes/scheme_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-02 15:46:31.000000 cached_path-1.4.0/cached_path/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:47:09.445978 cached_path-1.4.0/cached_path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-02 15:47:09.000000 cached_path-1.4.0/cached_path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-02 15:47:09.000000 cached_path-1.4.0/cached_path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:47:09.000000 cached_path-1.4.0/cached_path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 15:47:09.000000 cached_path-1.4.0/cached_path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 15:47:09.000000 cached_path-1.4.0/cached_path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-02 15:46:31.000000 cached_path-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:47:09.449977 cached_path-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 15:46:31.000000 cached_path-1.4.0/setup.py
```

### Comparing `cached_path-1.3.5/LICENSE` & `cached_path-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/PKG-INFO` & `cached_path-1.4.0/cached_path.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cached_path
-Version: 1.3.5
+Name: cached-path
+Version: 1.4.0
 Home-page: https://github.com/allenai/cached_path
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Keywords: allennlp cached_path file utils
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cached_path Version: 1.3.5 Home-page: https://
+Metadata-Version: 2.1 Name: cached-path Version: 1.4.0 Home-page: https://
 github.com/allenai/cached_path Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Keywords:
 allennlp cached_path file utils Classifier: Intended Audience :: Science/
 Research Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `cached_path-1.3.5/README.md` & `cached_path-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/__init__.py` & `cached_path-1.4.0/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/_cached_path.py` & `cached_path-1.4.0/cached_path/_cached_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,45 +173,43 @@
         # URL, so get it from the cache (downloading if necessary)
         file_path, etag = get_from_cache(url_or_filename, cache_dir, quiet=quiet, progress=progress)
 
         if extract_archive and (is_zipfile(file_path) or tarfile.is_tarfile(file_path)):
             # This is the path the file should be extracted to.
             # For example ~/.cached_path/cache/234234.21341 -> ~/.cached_path/cache/234234.21341-extracted
             extraction_path = file_path.parent / (file_path.name + "-extracted")
-
+    elif parsed.scheme == "file":
+        return cached_path(url_or_filename.replace("file://", "", 1))
     else:
         orig_url_or_filename = url_or_filename
         url_or_filename = Path(url_or_filename).expanduser()
         cache_dir = Path(cache_dir if cache_dir else get_cache_dir()).expanduser()
         cache_dir.mkdir(parents=True, exist_ok=True)
 
         if url_or_filename.exists():
             # File, and it exists.
             file_path = url_or_filename
             # Normalize the path.
             url_or_filename = url_or_filename.resolve()
-
             if (
                 extract_archive
                 and file_path.is_file()
                 and (is_zipfile(file_path) or tarfile.is_tarfile(file_path))
             ):
                 # We'll use a unique directory within the cache to root to extract the archive to.
                 # The name of the directory is a hash of the resource file path and it's modification
                 # time. That way, if the file changes, we'll know when to extract it again.
                 extraction_name = (
                     resource_to_filename(url_or_filename, str(os.path.getmtime(file_path)))
                     + "-extracted"
                 )
                 extraction_path = cache_dir / extraction_name
-
         elif parsed.scheme == "":
             # File, but it doesn't exist.
             raise FileNotFoundError(f"file {url_or_filename} not found")
-
         else:
             # Something unknown
             raise ValueError(f"unable to parse {orig_url_or_filename} as a URL or as a local path")
 
     if extraction_path is not None:
         # If the extracted directory already exists (and is non-empty), then no
         # need to create a lock file and extract again unless `force_extract=True`.
```

### Comparing `cached_path-1.3.5/cached_path/cache_file.py` & `cached_path-1.4.0/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/common.py` & `cached_path-1.4.0/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/file_lock.py` & `cached_path-1.4.0/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/meta.py` & `cached_path-1.4.0/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/progress.py` & `cached_path-1.4.0/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/__init__.py` & `cached_path-1.4.0/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/beaker.py` & `cached_path-1.4.0/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/gs.py` & `cached_path-1.4.0/cached_path/schemes/gs.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/hf.py` & `cached_path-1.4.0/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/http.py` & `cached_path-1.4.0/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/s3.py` & `cached_path-1.4.0/cached_path/schemes/s3.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/schemes/scheme_client.py` & `cached_path-1.4.0/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/testing.py` & `cached_path-1.4.0/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path/util.py` & `cached_path-1.4.0/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/cached_path.egg-info/PKG-INFO` & `cached_path-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cached-path
-Version: 1.3.5
+Name: cached_path
+Version: 1.4.0
 Home-page: https://github.com/allenai/cached_path
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Keywords: allennlp cached_path file utils
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cached-path Version: 1.3.5 Home-page: https://
+Metadata-Version: 2.1 Name: cached_path Version: 1.4.0 Home-page: https://
 github.com/allenai/cached_path Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Keywords:
 allennlp cached_path file utils Classifier: Intended Audience :: Science/
 Research Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `cached_path-1.3.5/cached_path.egg-info/SOURCES.txt` & `cached_path-1.4.0/cached_path.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.5/setup.py` & `cached_path-1.4.0/setup.py`

 * *Files identical despite different names*

