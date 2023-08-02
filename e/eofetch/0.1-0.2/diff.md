# Comparing `tmp/eofetch-0.1.tar.gz` & `tmp/eofetch-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eofetch-0.1.tar", last modified: Mon Jul 31 12:35:42 2023, max compression
+gzip compressed data, was "eofetch-0.2.tar", last modified: Wed Aug  2 10:56:10 2023, max compression
```

## Comparing `eofetch-0.1.tar` & `eofetch-0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-31 12:35:42.300947 eofetch-0.1/
--rw-r--r--   0 sander     (501) staff       (20)     1508 2023-07-31 12:31:28.000000 eofetch-0.1/LICENSE
--rw-r--r--   0 sander     (501) staff       (20)      426 2023-07-31 12:35:42.300595 eofetch-0.1/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)     2317 2023-07-31 12:28:17.000000 eofetch-0.1/README.md
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-31 12:35:42.296905 eofetch-0.1/eofetch/
--rw-r--r--   0 sander     (501) staff       (20)       28 2023-07-31 11:49:23.000000 eofetch-0.1/eofetch/__init__.py
--rw-r--r--   0 sander     (501) staff       (20)      919 2023-07-28 14:44:27.000000 eofetch-0.1/eofetch/__main__.py
--rw-r--r--   0 sander     (501) staff       (20)     2162 2023-07-28 11:32:00.000000 eofetch-0.1/eofetch/cdse.py
--rw-r--r--   0 sander     (501) staff       (20)     1397 2023-07-31 12:27:02.000000 eofetch-0.1/eofetch/fetch.py
--rw-r--r--   0 sander     (501) staff       (20)      703 2023-07-28 11:32:00.000000 eofetch-0.1/eofetch/s5ppal.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-31 12:35:42.300029 eofetch-0.1/eofetch.egg-info/
--rw-r--r--   0 sander     (501) staff       (20)      426 2023-07-31 12:35:42.000000 eofetch-0.1/eofetch.egg-info/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)      305 2023-07-31 12:35:42.000000 eofetch-0.1/eofetch.egg-info/SOURCES.txt
--rw-r--r--   0 sander     (501) staff       (20)        1 2023-07-31 12:35:42.000000 eofetch-0.1/eofetch.egg-info/dependency_links.txt
--rw-r--r--   0 sander     (501) staff       (20)       46 2023-07-31 12:35:42.000000 eofetch-0.1/eofetch.egg-info/entry_points.txt
--rw-r--r--   0 sander     (501) staff       (20)       29 2023-07-31 12:35:42.000000 eofetch-0.1/eofetch.egg-info/requires.txt
--rw-r--r--   0 sander     (501) staff       (20)        8 2023-07-31 12:35:42.000000 eofetch-0.1/eofetch.egg-info/top_level.txt
--rw-r--r--   0 sander     (501) staff       (20)       38 2023-07-31 12:35:42.301076 eofetch-0.1/setup.cfg
--rw-r--r--   0 sander     (501) staff       (20)      632 2023-07-31 12:34:11.000000 eofetch-0.1/setup.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 10:56:10.420876 eofetch-0.2/
+-rw-r--r--   0 sander     (501) staff       (20)      179 2023-08-02 10:51:59.000000 eofetch-0.2/CHANGES
+-rw-r--r--   0 sander     (501) staff       (20)     1508 2023-07-31 12:31:28.000000 eofetch-0.2/LICENSE
+-rw-r--r--   0 sander     (501) staff       (20)       16 2023-08-02 10:55:08.000000 eofetch-0.2/MANIFEST.in
+-rw-r--r--   0 sander     (501) staff       (20)      426 2023-08-02 10:56:10.420570 eofetch-0.2/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)     2317 2023-07-31 12:28:17.000000 eofetch-0.2/README.md
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 10:56:10.417981 eofetch-0.2/eofetch/
+-rw-r--r--   0 sander     (501) staff       (20)       28 2023-07-31 11:49:23.000000 eofetch-0.2/eofetch/__init__.py
+-rw-r--r--   0 sander     (501) staff       (20)      919 2023-07-28 14:44:27.000000 eofetch-0.2/eofetch/__main__.py
+-rw-r--r--   0 sander     (501) staff       (20)     2162 2023-07-28 11:32:00.000000 eofetch-0.2/eofetch/cdse.py
+-rw-r--r--   0 sander     (501) staff       (20)     1389 2023-07-31 12:55:29.000000 eofetch-0.2/eofetch/fetch.py
+-rw-r--r--   0 sander     (501) staff       (20)      703 2023-07-28 11:32:00.000000 eofetch-0.2/eofetch/s5ppal.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-08-02 10:56:10.420193 eofetch-0.2/eofetch.egg-info/
+-rw-r--r--   0 sander     (501) staff       (20)      426 2023-08-02 10:56:10.000000 eofetch-0.2/eofetch.egg-info/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)      325 2023-08-02 10:56:10.000000 eofetch-0.2/eofetch.egg-info/SOURCES.txt
+-rw-r--r--   0 sander     (501) staff       (20)        1 2023-08-02 10:56:10.000000 eofetch-0.2/eofetch.egg-info/dependency_links.txt
+-rw-r--r--   0 sander     (501) staff       (20)       50 2023-08-02 10:56:10.000000 eofetch-0.2/eofetch.egg-info/entry_points.txt
+-rw-r--r--   0 sander     (501) staff       (20)       29 2023-08-02 10:56:10.000000 eofetch-0.2/eofetch.egg-info/requires.txt
+-rw-r--r--   0 sander     (501) staff       (20)        8 2023-08-02 10:56:10.000000 eofetch-0.2/eofetch.egg-info/top_level.txt
+-rw-r--r--   0 sander     (501) staff       (20)       38 2023-08-02 10:56:10.420966 eofetch-0.2/setup.cfg
+-rw-r--r--   0 sander     (501) staff       (20)      636 2023-08-02 10:49:53.000000 eofetch-0.2/setup.py
```

### Comparing `eofetch-0.1/LICENSE` & `eofetch-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eofetch-0.1/README.md` & `eofetch-0.2/README.md`

 * *Files identical despite different names*

### Comparing `eofetch-0.1/eofetch/__main__.py` & `eofetch-0.2/eofetch/__main__.py`

 * *Files identical despite different names*

### Comparing `eofetch-0.1/eofetch/cdse.py` & `eofetch-0.2/eofetch/cdse.py`

 * *Files identical despite different names*

### Comparing `eofetch-0.1/eofetch/fetch.py` & `eofetch-0.2/eofetch/fetch.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     product = os.path.basename(products)
     if target_directory is None:
         target_directory = "."
     targetpath = os.path.join(target_directory, product)
 
     if os.path.exists(targetpath):
-        return product
+        return
 
     if not os.path.exists(target_directory):
         os.makedirs(target_directory)
 
     for mapping in MAPPING:
         if re.match(mapping, product) is not None:
             download_backend = MAPPING[mapping]
```

### Comparing `eofetch-0.1/eofetch/s5ppal.py` & `eofetch-0.2/eofetch/s5ppal.py`

 * *Files identical despite different names*

### Comparing `eofetch-0.1/setup.py` & `eofetch-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name='eofetch',
-    version='0.1',
+    version='0.2',
     description='Earth Observation Data Retrieval library',
     url="https://github.com/stcorp/eofetch",
     author='S[&]T',
     license='BSD',
     packages=['eofetch'],
-    entry_points={'console_scripts': ['eofetch = eofetch.main:main']},
+    entry_points={'console_scripts': ['eofetch = eofetch.__main__:main']},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
     ],
```

