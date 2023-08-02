# Comparing `tmp/propelauth-fastapi-2.1.3.tar.gz` & `tmp/propelauth-fastapi-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-fastapi-2.1.3.tar", last modified: Tue Jun  6 17:38:20 2023, max compression
+gzip compressed data, was "propelauth-fastapi-2.1.4.tar", last modified: Wed Aug  2 18:16:58 2023, max compression
```

## Comparing `propelauth-fastapi-2.1.3.tar` & `propelauth-fastapi-2.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/propelauth_fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/propelauth_fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 17:38:20.000000 propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:38:20.085698 propelauth-fastapi-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-06 17:38:05.000000 propelauth-fastapi-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:16:58.173010 propelauth-fastapi-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 18:16:41.000000 propelauth-fastapi-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 18:16:58.173010 propelauth-fastapi-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 18:16:41.000000 propelauth-fastapi-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:16:58.173010 propelauth-fastapi-2.1.4/propelauth_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-08-02 18:16:41.000000 propelauth-fastapi-2.1.4/propelauth_fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:16:58.173010 propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 18:16:58.000000 propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-02 18:16:58.000000 propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:16:58.000000 propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 18:16:58.000000 propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 18:16:58.000000 propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:16:58.173010 propelauth-fastapi-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 18:16:41.000000 propelauth-fastapi-2.1.4/setup.py
```

### Comparing `propelauth-fastapi-2.1.3/LICENSE` & `propelauth-fastapi-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.3/PKG-INFO` & `propelauth-fastapi-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-fastapi
-Version: 2.1.3
+Version: 2.1.4
 Summary: A FastAPI library for managing authentication, backed by PropelAuth
 Home-page: https://github.com/propelauth/propelauth-fastapi
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.3 Summary: A
+Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.4 Summary: A
 FastAPI library for managing authentication, backed by PropelAuth Home-page:
 https://github.com/propelauth/propelauth-fastapi Author: PropelAuth Author-
 email: support@propelauth.com License: MIT Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE # PropelAuth FastAPI SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A FastAPI library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-fastapi). [PropelAuth](https://
```

### Comparing `propelauth-fastapi-2.1.3/README.md` & `propelauth-fastapi-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.3/propelauth_fastapi/__init__.py` & `propelauth-fastapi-2.1.4/propelauth_fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.3/propelauth_fastapi.egg-info/PKG-INFO` & `propelauth-fastapi-2.1.4/propelauth_fastapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-fastapi
-Version: 2.1.3
+Version: 2.1.4
 Summary: A FastAPI library for managing authentication, backed by PropelAuth
 Home-page: https://github.com/propelauth/propelauth-fastapi
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.3 Summary: A
+Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.4 Summary: A
 FastAPI library for managing authentication, backed by PropelAuth Home-page:
 https://github.com/propelauth/propelauth-fastapi Author: PropelAuth Author-
 email: support@propelauth.com License: MIT Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE # PropelAuth FastAPI SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A FastAPI library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-fastapi). [PropelAuth](https://
```

### Comparing `propelauth-fastapi-2.1.3/setup.py` & `propelauth-fastapi-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-fastapi",
-    version="2.1.3",
+    version="2.1.4",
     description="A FastAPI library for managing authentication, backed by PropelAuth",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-fastapi",
     packages=find_packages(include=["propelauth_fastapi"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["propelauth-py==3.1.3", "requests"],
+    install_requires=["propelauth-py==3.1.4", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

