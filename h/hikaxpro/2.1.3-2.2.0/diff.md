# Comparing `tmp/hikaxpro-2.1.3.tar.gz` & `tmp/hikaxpro-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikaxpro-2.1.3.tar", last modified: Tue May  9 21:19:21 2023, max compression
+gzip compressed data, was "hikaxpro-2.2.0.tar", last modified: Wed Aug  2 09:13:18 2023, max compression
```

## Comparing `hikaxpro-2.1.3.tar` & `hikaxpro-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.750901 hikaxpro-2.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.750901 hikaxpro-2.1.3/src/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.750901 hikaxpro-2.1.3/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/helpers/sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/helpers/xmlBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/src/hikaxpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 21:19:21.000000 hikaxpro-2.1.3/src/hikaxpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/hikaxpro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/models/SessionLogin.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/models/SessionLoginCap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:19:21.754901 hikaxpro-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/tests/test_hikaxpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-09 21:19:10.000000 hikaxpro-2.1.3/tests/test_xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/helpers/sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/helpers/xmlBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/hikaxpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 09:13:18.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 09:13:17.000000 hikaxpro-2.2.0/src/hikaxpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/hikaxpro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.008483 hikaxpro-2.2.0/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/models/SessionLogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/models/SessionLoginCap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:13:18.012483 hikaxpro-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/tests/test_hikaxpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-02 09:13:05.000000 hikaxpro-2.2.0/tests/test_xmlBuilder.py
```

### Comparing `hikaxpro-2.1.3/LICENSE` & `hikaxpro-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.3/PKG-INFO` & `hikaxpro-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.1.3
+Version: 2.2.0
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hikaxpro-2.1.3/pyproject.toml` & `hikaxpro-2.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hikaxpro"
-version = "2.1.3"
+version = "2.2.0"
 description = "Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel"
 readme = "README.md"
 authors = [
     { name = "Günkut Zeybek", email = "gunkut.zeybek@gmail.com" },
     { name = "Petr Leo Compel", email = "petrleocompel@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["hikvision", "ISAPI", "homeassistant"]
 dependencies = [
-    "requests"    
+    "requests"
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 repository = "https://github.com/petrleocompel/hikaxpro/"
 
 [project.optional-dependencies]
 dev = ["pytest", "requests_mock"]
 
 [tool.bumpver]
-current_version = "2.1.3"
+current_version = "2.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore: release version {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `hikaxpro-2.1.3/src/consts.py` & `hikaxpro-2.2.0/src/consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,21 @@
     BypassZone = "/ISAPI/SecurityCP/control/bypass/"
     RecoverBypassZone = "/ISAPI/SecurityCP/control/Recoverbypass/"
     InterfaceInfo = "/ISAPI/System/Network/interfaces"
     AreaArmStatus = "/ISAPI/SecurityCP/status/armStatus"
     SirenStatus = "/ISAPI/SecurityCP/status/sirenStatus"
     RepeaterStatus = "/ISAPI/SecurityCP/status/repeaterStatus"
     KeypadStatus = "/ISAPI/SecurityCP/status/keypadStatus"
+    OutputStatus = "/ISAPI/SecurityCP/status/outputStatus"
+    BatteriesStatus = "/ISAPI/SecurityCP/status/batteries"
+    HostCapabilities = "/ISAPI/SecurityCP/control/capabilities"
+    SystemDeviceInfo = "/ISAPI/System/deviceInfo"
+    OutputConfig = "/ISAPI/SecurityCP/Configuration/outputs"
+    SirensConfig = "/ISAPI/SecurityCP/Configuration/wirelessSiren"
+
 
 
 class Method:
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
```

### Comparing `hikaxpro-2.1.3/src/helpers/sha256.py` & `hikaxpro-2.2.0/src/helpers/sha256.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.3/src/helpers/xmlBuilder.py` & `hikaxpro-2.2.0/src/helpers/xmlBuilder.py`

 * *Files identical despite different names*

### Comparing `hikaxpro-2.1.3/src/hikaxpro.egg-info/PKG-INFO` & `hikaxpro-2.2.0/src/hikaxpro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikaxpro
-Version: 2.1.3
+Version: 2.2.0
 Summary: Hikvision AX Pro alarm kit ISAPI integration for home assistant alarm panel
 Author-email: Günkut Zeybek <gunkut.zeybek@gmail.com>, Petr Leo Compel <petrleocompel@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 smartha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `hikaxpro-2.1.3/src/hikaxpro.py` & `hikaxpro-2.2.0/src/hikaxpro.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,28 +68,36 @@
 
         session_id = HikAxPro._root_get_value(root, namespaces, "xmlns:sessionID")
         challenge = HikAxPro._root_get_value(root, namespaces, "xmlns:challenge")
         salt = HikAxPro._root_get_value(root, namespaces, "xmlns:salt")
         salt2 = HikAxPro._root_get_value(root, namespaces, "xmlns:salt2")
         is_irreversible = True if HikAxPro._root_get_value(root, namespaces, "xmlns:isIrreversible", False) == 'true' else False
         iterations = HikAxPro._root_get_value(root, namespaces, "xmlns:iterations")
+        session_id_version = HikAxPro._root_get_value(root, namespaces, "xmlns:sessionIDVersion", None)
         if iterations is not None:
             iterations = int(iterations)
         session_cap = SessionLoginCap.SessionLoginCap(
             session_id=session_id,
+            session_id_version=session_id_version,
             challenge=challenge,
             salt=salt,
             salt2=salt2,
             is_irreversible=is_irreversible,
             iterations=iterations
         )
         return session_cap
 
     def encode_password(self, session_cap: SessionLoginCap.SessionLoginCap):
-        if session_cap.is_irreversible:
+        if session_cap.session_id_version == "2" and session_cap.is_irreversible:
+            result = sha256.sha256(f"{self.username}{session_cap.salt}{self.password}")
+            result = sha256.sha256(f"{result}{session_cap.challenge}")
+
+            for i in range(2, session_cap.iterations):
+                result = sha256.sha256(result)
+        elif session_cap.is_irreversible:
             result = sha256.sha256(f"{self.username}{session_cap.salt}{self.password}")
             result = sha256.sha256(f"{self.username}{session_cap.salt2}{result}")
             result = sha256.sha256(f"{result}{session_cap.challenge}")
 
             for i in range(2, session_cap.iterations):
                 result = sha256.sha256(result)
         else:
@@ -105,15 +113,16 @@
 
         encoded_password = self.encode_password(params)
 
         xml = xmlBuilder.serialize_object(
             SessionLogin.SessionLogin(
                 params.session_id,
                 self.username,
-                encoded_password
+                encoded_password,
+                params.session_id_version
             )
         )
 
         dt = datetime.now()
         timestamp = datetime.timestamp(dt)
         session_login_url = f"http://{self.host}{consts.Endpoints.Session_Login}?timeStamp={int(timestamp)}"
         result = False
```

### Comparing `hikaxpro-2.1.3/tests/test_hikaxpro.py` & `hikaxpro-2.2.0/tests/test_hikaxpro.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,27 +49,41 @@
 
 def test_encodePassword_Irrevesible(theaxpro):
     sessionID = ''
     challange = '82360cd6ffd7beda4398cf67bfbd1ea9'
     iteration = 100
     salt = '22CF57B6ADE75214A4C87042B3272630C55EF5D782AB3BE4C9EC4DA1CD95AF3B'
     salt2 = '7BEB8CA39D05B89CABC4003FDCBA5AE73556CB8008BCEE3CBCA48CABC3AC201B'
-    sessionCap = SessionLoginCap.SessionLoginCap(sessionID, challange, salt, salt2, True, iteration)    
+    sessionCap = SessionLoginCap.SessionLoginCap(sessionID, "2.1", challange, salt, salt2, True, iteration)
 
     encodedPassword = theaxpro.encode_password(sessionCap)
 
     assert encodedPassword == "777b95a40f8b5b9ca25101d3c73168adb340f2001b611a74104c34352962d647"
 
+
+def test_encodePassword_Irrevesible_olderVersion():
+    theaxpro = hikaxpro.HikAxPro("192.168.72.136", "dalferin", "test123456")
+    sessionID = "2c9ac7c6d7002d6bc1359c59c7968fd6683569cf47ad149826cf1e5c84cbb7"
+    challange = "9524eedd2912a46ef2c0fcfa27e412c1"
+    iteration = 100
+    salt = "bef6d541c1ac37f74d90b9d3dc642ab6ea54b17d653b10f24464867b6dbeacb5"
+    salt2 = None
+    sessionCap = SessionLoginCap.SessionLoginCap(sessionID, "2.1", challange, salt, salt2, True, iteration)
+
+    encodedPassword = theaxpro.encode_password(sessionCap)
+
+    assert encodedPassword == '86c59b2a28aafd52ccbd@a46f06200e50467cec0758eb32a8c5d5cce5b55abc'
+
 def test_encodePassword_Not_Irreversible(theaxpro):
     sessionID = ''
     challange = '82360cd6ffd7beda4398cf67bfbd1ea9'
     iteration = 100
     salt = '22CF57B6ADE75214A4C87042B3272630C55EF5D782AB3BE4C9EC4DA1CD95AF3B'
     salt2 = '7BEB8CA39D05B89CABC4003FDCBA5AE73556CB8008BCEE3CBCA48CABC3AC201B'
-    sessionCap = SessionLoginCap.SessionLoginCap(sessionID, challange, salt, salt2, False, iteration)    
+    sessionCap = SessionLoginCap.SessionLoginCap(sessionID, "2", challange, salt, salt2, False, iteration)
 
     encodedPassword = theaxpro.encode_password(sessionCap)
     assert encodedPassword == "2b31a14ba59914a8e5e5510063e5d500ef322e76bc6c160df6a86b35c1e89ddd"
 
 @requests_mock.Mocker(kw='mock')
 def test_connect_successfull(theaxpro, **kwargs):  
     url = f"http://{theaxpro.host}{consts.Endpoints.Session_Capabilities}{theaxpro.username}"
```

### Comparing `hikaxpro-2.1.3/tests/test_xmlBuilder.py` & `hikaxpro-2.2.0/tests/test_xmlBuilder.py`

 * *Files identical despite different names*

