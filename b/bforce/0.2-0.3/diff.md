# Comparing `tmp/bforce-0.2.tar.gz` & `tmp/bforce-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bforce-0.2.tar", last modified: Mon Jul 31 08:08:09 2023, max compression
+gzip compressed data, was "bforce-0.3.tar", last modified: Wed Aug  2 08:28:19 2023, max compression
```

## Comparing `bforce-0.2.tar` & `bforce-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-31 08:08:09.107699 bforce-0.2/
--rw-r--r--   0 voidful    (501) staff       (20)      129 2023-07-31 08:08:09.107311 bforce-0.2/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)     1738 2023-07-30 22:15:47.000000 bforce-0.2/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-31 08:08:09.098085 bforce-0.2/bforce/
--rw-r--r--   0 voidful    (501) staff       (20)       19 2023-07-30 22:03:29.000000 bforce-0.2/bforce/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)       44 2023-07-30 21:58:35.000000 bforce-0.2/bforce/exceptions.py
--rw-r--r--   0 voidful    (501) staff       (20)     3714 2023-07-30 22:06:09.000000 bforce-0.2/bforce/main.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-07-31 08:08:09.106442 bforce-0.2/bforce.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)      129 2023-07-31 08:08:08.000000 bforce-0.2/bforce.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      193 2023-07-31 08:08:08.000000 bforce-0.2/bforce.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-07-31 08:08:08.000000 bforce-0.2/bforce.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)        7 2023-07-31 08:08:08.000000 bforce-0.2/bforce.egg-info/top_level.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-07-31 08:08:09.107844 bforce-0.2/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)      122 2023-07-31 08:08:01.000000 bforce-0.2/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-02 08:28:19.538977 bforce-0.3/
+-rw-r--r--   0 voidful    (501) staff       (20)      129 2023-08-02 08:28:19.537990 bforce-0.3/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)     1738 2023-07-30 22:15:47.000000 bforce-0.3/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-02 08:28:19.531785 bforce-0.3/bforce/
+-rw-r--r--   0 voidful    (501) staff       (20)       19 2023-07-30 22:03:29.000000 bforce-0.3/bforce/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)       44 2023-07-30 21:58:35.000000 bforce-0.3/bforce/exceptions.py
+-rw-r--r--   0 voidful    (501) staff       (20)     3716 2023-08-02 08:26:32.000000 bforce-0.3/bforce/main.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-08-02 08:28:19.537459 bforce-0.3/bforce.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)      129 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      193 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        7 2023-08-02 08:28:19.000000 bforce-0.3/bforce.egg-info/top_level.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-08-02 08:28:19.539127 bforce-0.3/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)      122 2023-08-02 08:26:46.000000 bforce-0.3/setup.py
```

### Comparing `bforce-0.2/README.md` & `bforce-0.3/README.md`

 * *Files identical despite different names*

### Comparing `bforce-0.2/bforce/main.py` & `bforce-0.3/bforce/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Load cache
             cache = load_cache(cache_dir)
             # Create a key based on function name and arguments
             cache_key = f"{func.__name__}_{args}_{kwargs}"
             if cache_key in cache:
-                print(f"Loaded result from cache for function: {func.__name__} with args: {args} and kwargs: {kwargs}")
+                # print(f"Loaded result from cache for function: {func.__name__} with args: {args} and kwargs: {kwargs}")
                 return cache[cache_key]
             else:
                 result = func(*args, **kwargs)
                 # Save result to cache
                 save_cache(cache_key, result, cache_dir)
                 return result
```

