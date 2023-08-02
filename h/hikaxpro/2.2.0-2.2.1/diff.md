# Comparing `tmp/hikaxpro-2.2.0.tar.gz` & `tmp/hikaxpro-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikaxpro-2.2.0.tar", last modified: Wed Aug  2 09:13:18 2023, max compression
+gzip compressed data, was "hikaxpro-2.2.1.tar", last modified: Wed Aug  2 19:56:05 2023, max compression
```

## Comparing `hikaxpro-2.2.0.tar` & `hikaxpro-2.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/helpers/sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/helpers/xmlBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/hikaxpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 09:13:18.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/hikaxpro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/models/SessionLogin.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/models/SessionLoginCap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/tests/test_hikaxpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/tests/test_xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/helpers/sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/helpers/xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/src/hikaxpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-02 19:56:05.000000 hikaxpro-2.2.1/src/hikaxpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 19:56:05.000000 hikaxpro-2.2.1/src/hikaxpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:56:05.000000 hikaxpro-2.2.1/src/hikaxpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 19:56:05.000000 hikaxpro-2.2.1/src/hikaxpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 19:56:05.000000 hikaxpro-2.2.1/src/hikaxpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/hikaxpro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/models/SessionLogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/models/SessionLoginCap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:05.342210 hikaxpro-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/tests/test_hikaxpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-02 19:55:55.000000 hikaxpro-2.2.1/tests/test_xmlBuilder.py
```

### Comparing `hikaxpro-2.2.0/LICENSE` & `hikaxpro-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.2.0/PKG-INFO` & `hikaxpro-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.2.0
+Version: 2.2.1
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hikaxpro-2.2.0/pyproject.toml` & `hikaxpro-2.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hikaxpro"
-version = "2.2.0"
+version = "2.2.1"
 description = "Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel"
 readme = "README.md"
 authors = [
     { name = "Günkut Zeybek", email = "gunkut.zeybek@gmail.com" },
     { name = "Petr Leo Compel", email = "petrleocompel@gmail.com" }
 ]
 license = { file = "LICENSE" }
@@ -26,15 +26,15 @@
 [project.urls]
 repository = "https://github.com/petrleocompel/hikaxpro/"
 
 [project.optional-dependencies]
 dev = ["pytest", "requests_mock"]
 
 [tool.bumpver]
-current_version = "2.2.0"
+current_version = "2.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore: release version {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `hikaxpro-2.2.0/src/consts.py` & `hikaxpro-2.2.1/src/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     KeypadStatus = "/ISAPI/SecurityCP/status/keypadStatus"
     OutputStatus = "/ISAPI/SecurityCP/status/outputStatus"
     BatteriesStatus = "/ISAPI/SecurityCP/status/batteries"
     HostCapabilities = "/ISAPI/SecurityCP/control/capabilities"
     SystemDeviceInfo = "/ISAPI/System/deviceInfo"
     OutputConfig = "/ISAPI/SecurityCP/Configuration/outputs"
     SirensConfig = "/ISAPI/SecurityCP/Configuration/wirelessSiren"
-
+    OutputControl = "/ISAPI/SecurityCP/control/outputs/{}"
 
 
 class Method:
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
```

### Comparing `hikaxpro-2.2.0/src/helpers/sha256.py` & `hikaxpro-2.2.1/src/helpers/sha256.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.2.0/src/helpers/xmlBuilder.py` & `hikaxpro-2.2.1/src/helpers/xmlBuilder.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.2.0/src/hikaxpro.egg-info/PKG-INFO` & `hikaxpro-2.2.1/src/hikaxpro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.2.0
+Version: 2.2.1
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hikaxpro-2.2.0/src/hikaxpro.py` & `hikaxpro-2.2.1/src/hikaxpro.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.2.0/tests/test_hikaxpro.py` & `hikaxpro-2.2.1/tests/test_hikaxpro.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.2.0/tests/test_xmlBuilder.py` & `hikaxpro-2.2.1/tests/test_xmlBuilder.py`

 * *Files identical despite different names*

