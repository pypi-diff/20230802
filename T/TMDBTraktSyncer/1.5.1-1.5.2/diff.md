# Comparing `tmp/TMDBTraktSyncer-1.5.1.tar.gz` & `tmp/TMDBTraktSyncer-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.5.1.tar", last modified: Sun Jul 30 07:04:21 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.5.2.tar", last modified: Wed Aug  2 07:24:20 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.5.1.tar` & `TMDBTraktSyncer-1.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 07:04:21.456208 TMDBTraktSyncer-1.5.1/
--rw-rw-rw-   0        0        0     1079 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/LICENSE
--rw-rw-rw-   0        0        0    11433 2023-07-30 07:04:21.455197 TMDBTraktSyncer-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    10684 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 07:04:21.420200 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    18069 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4548 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0    10181 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0     4058 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     7120 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     8014 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:04:21.453207 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    11433 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 07:04:21.457198 TMDBTraktSyncer-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:24:20.063530 TMDBTraktSyncer-1.5.2/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0    11433 2023-08-02 07:24:20.062541 TMDBTraktSyncer-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10684 2023-08-02 07:21:38.000000 TMDBTraktSyncer-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 07:24:20.031531 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    18069 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4548 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0    10181 2023-08-02 06:33:13.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4058 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7120 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     8014 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:24:20.060531 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11433 2023-08-02 07:24:19.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-08-02 07:24:19.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:24:19.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-02 07:24:19.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 07:24:19.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 07:24:19.000000 TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:24:20.063530 TMDBTraktSyncer-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-08-02 07:20:58.000000 TMDBTraktSyncer-1.5.2/setup.py
```

### Comparing `TMDBTraktSyncer-1.5.1/LICENSE` & `TMDBTraktSyncer-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/PKG-INFO` & `TMDBTraktSyncer-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TMDBTraktSyncer-1.5.1/README.md` & `TMDBTraktSyncer-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/errorHandling.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     print("Please submit the error to GitHub with the following information:")
     print("-" * 50)
     print(traceback_info)
     print("-" * 50)
     print(f"Submit the error here: {github_issue_url}")
     print("-" * 50)
 
-def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
+def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=5):
     if headers is None:
         headers = {
             'Content-Type': 'application/json',
             'trakt-api-version': '2',
             'trakt-api-key': VC.trakt_client_id,
             'Authorization': f'Bearer {VC.trakt_access_token}'
         }
 
-    retry_delay = 5  # seconds between retries
+    retry_delay = 1  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
         try:
             if payload is None:
                 if params:
@@ -94,22 +94,22 @@
         520: "Service Unavailable - Cloudflare error",
         521: "Service Unavailable - Cloudflare error",
         522: "Service Unavailable - Cloudflare error"
     }
 
     return error_messages.get(status_code, "Unknown error")
 
-def make_tmdb_request(url, headers=None, payload=None, max_retries=3):
+def make_tmdb_request(url, headers=None, payload=None, max_retries=5):
     if headers is None:
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {VC.tmdb_v4_token}'
         }
 
-    retry_delay = 5  # seconds between retries
+    retry_delay = 1  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
         try:
             if payload is None:
                 response = requests.get(url, headers=headers)
```

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorLogger.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/SOURCES.txt` & `TMDBTraktSyncer-1.5.2/TMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.5.1/setup.py` & `TMDBTraktSyncer-1.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.1'
+VERSION = '1.5.2'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
@@ -33,8 +33,8 @@
     ],
     entry_points={
         'console_scripts': [
             'TMDBTraktSyncer = TMDBTraktSyncer.TMDBTraktSyncer:main'
         ]
     },
     python_requires='>=3.6'
-)
+)
```

