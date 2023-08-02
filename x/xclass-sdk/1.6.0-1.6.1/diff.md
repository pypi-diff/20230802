# Comparing `tmp/xclass_sdk-1.6.0.tar.gz` & `tmp/xclass_sdk-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xclass_sdk-1.6.0.tar", last modified: Fri Jul 21 06:19:19 2023, max compression
+gzip compressed data, was "xclass_sdk-1.6.1.tar", last modified: Wed Aug  2 02:57:21 2023, max compression
```

## Comparing `xclass_sdk-1.6.0.tar` & `xclass_sdk-1.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.896246 xclass_sdk-1.6.0/
--rw-r--r--   0 hansle     (501) staff       (20)    35148 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/LICENSE.txt
--rw-r--r--   0 hansle     (501) staff       (20)      535 2023-07-21 06:19:19.896113 xclass_sdk-1.6.0/PKG-INFO
--rw-r--r--   0 hansle     (501) staff       (20)       39 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/README.md
--rw-r--r--   0 hansle     (501) staff       (20)      607 2023-07-21 06:19:13.000000 xclass_sdk-1.6.0/pyproject.toml
--rw-r--r--   0 hansle     (501) staff       (20)       38 2023-07-21 06:19:19.896287 xclass_sdk-1.6.0/setup.cfg
-drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.892928 xclass_sdk-1.6.0/src/
-drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.894332 xclass_sdk-1.6.0/src/browser_sdk/
--rw-r--r--   0 hansle     (501) staff       (20)     1528 2023-07-17 18:12:05.000000 xclass_sdk-1.6.0/src/browser_sdk/general_app_browser.py
--rw-r--r--   0 hansle     (501) staff       (20)      748 2023-07-16 10:30:50.000000 xclass_sdk-1.6.0/src/browser_sdk/math_app_browser.py
-drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.895210 xclass_sdk-1.6.0/src/xclass_sdk/
--rw-r--r--   0 hansle     (501) staff       (20)       26 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/src/xclass_sdk/__init__.py
--rw-r--r--   0 hansle     (501) staff       (20)     2294 2023-07-20 09:05:01.000000 xclass_sdk-1.6.0/src/xclass_sdk/general_app.py
--rw-r--r--   0 hansle     (501) staff       (20)     1028 2023-07-16 10:30:50.000000 xclass_sdk-1.6.0/src/xclass_sdk/math_app.py
--rw-r--r--   0 hansle     (501) staff       (20)      980 2023-07-07 02:12:24.000000 xclass_sdk-1.6.0/src/xclass_sdk/profile.py
--rw-r--r--   0 hansle     (501) staff       (20)      833 2023-06-22 08:33:55.000000 xclass_sdk-1.6.0/src/xclass_sdk/xclass_helpers.py
-drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-07-21 06:19:19.895946 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/
--rw-r--r--   0 hansle     (501) staff       (20)      535 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/PKG-INFO
--rw-r--r--   0 hansle     (501) staff       (20)      443 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 hansle     (501) staff       (20)        1 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 hansle     (501) staff       (20)       15 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/requires.txt
--rw-r--r--   0 hansle     (501) staff       (20)       23 2023-07-21 06:19:19.000000 xclass_sdk-1.6.0/src/xclass_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-08-02 02:57:21.840039 xclass_sdk-1.6.1/
+-rw-r--r--   0 hansle     (501) staff       (20)    35148 2023-06-22 08:33:55.000000 xclass_sdk-1.6.1/LICENSE.txt
+-rw-r--r--   0 hansle     (501) staff       (20)      535 2023-08-02 02:57:21.839887 xclass_sdk-1.6.1/PKG-INFO
+-rw-r--r--   0 hansle     (501) staff       (20)       39 2023-06-22 08:33:55.000000 xclass_sdk-1.6.1/README.md
+-rw-r--r--   0 hansle     (501) staff       (20)      607 2023-08-02 02:57:17.000000 xclass_sdk-1.6.1/pyproject.toml
+-rw-r--r--   0 hansle     (501) staff       (20)       38 2023-08-02 02:57:21.840088 xclass_sdk-1.6.1/setup.cfg
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-08-02 02:57:21.835442 xclass_sdk-1.6.1/src/
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-08-02 02:57:21.838011 xclass_sdk-1.6.1/src/browser_sdk/
+-rw-r--r--   0 hansle     (501) staff       (20)     1537 2023-07-31 09:17:59.000000 xclass_sdk-1.6.1/src/browser_sdk/general_app_browser.py
+-rw-r--r--   0 hansle     (501) staff       (20)      748 2023-07-16 10:30:50.000000 xclass_sdk-1.6.1/src/browser_sdk/math_app_browser.py
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-08-02 02:57:21.838680 xclass_sdk-1.6.1/src/xclass_sdk/
+-rw-r--r--   0 hansle     (501) staff       (20)       26 2023-06-22 08:33:55.000000 xclass_sdk-1.6.1/src/xclass_sdk/__init__.py
+-rw-r--r--   0 hansle     (501) staff       (20)     2464 2023-08-02 02:56:04.000000 xclass_sdk-1.6.1/src/xclass_sdk/general_app.py
+-rw-r--r--   0 hansle     (501) staff       (20)     1028 2023-07-27 09:23:09.000000 xclass_sdk-1.6.1/src/xclass_sdk/math_app.py
+-rw-r--r--   0 hansle     (501) staff       (20)      980 2023-07-31 09:05:31.000000 xclass_sdk-1.6.1/src/xclass_sdk/profile.py
+-rw-r--r--   0 hansle     (501) staff       (20)      833 2023-06-22 08:33:55.000000 xclass_sdk-1.6.1/src/xclass_sdk/xclass_helpers.py
+drwxr-xr-x   0 hansle     (501) staff       (20)        0 2023-08-02 02:57:21.839659 xclass_sdk-1.6.1/src/xclass_sdk.egg-info/
+-rw-r--r--   0 hansle     (501) staff       (20)      535 2023-08-02 02:57:21.000000 xclass_sdk-1.6.1/src/xclass_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 hansle     (501) staff       (20)      443 2023-08-02 02:57:21.000000 xclass_sdk-1.6.1/src/xclass_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 hansle     (501) staff       (20)        1 2023-08-02 02:57:21.000000 xclass_sdk-1.6.1/src/xclass_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 hansle     (501) staff       (20)       15 2023-08-02 02:57:21.000000 xclass_sdk-1.6.1/src/xclass_sdk.egg-info/requires.txt
+-rw-r--r--   0 hansle     (501) staff       (20)       23 2023-08-02 02:57:21.000000 xclass_sdk-1.6.1/src/xclass_sdk.egg-info/top_level.txt
```

### Comparing `xclass_sdk-1.6.0/LICENSE.txt` & `xclass_sdk-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.6.0/PKG-INFO` & `xclass_sdk-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xclass_sdk
-Version: 1.6.0
+Version: 1.6.1
 Summary: X-Class SDK
 Author-email: Trung Nguyen <lantrungseo@gmail.com>
 Project-URL: Homepage, https://github.com/lantrungseo/xclass-sdk
 Project-URL: Bug Tracker, https://github.com/lantrungseo/xclass-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xclass_sdk-1.6.0/pyproject.toml` & `xclass_sdk-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "xclass_sdk"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="Trung Nguyen", email="lantrungseo@gmail.com" },
 ]
 description = "X-Class SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `xclass_sdk-1.6.0/src/browser_sdk/general_app_browser.py` & `xclass_sdk-1.6.1/src/browser_sdk/general_app_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,11 +59,11 @@
         })
         return Output(f'id-output-{len(self.listOutput) - 1}')
 
     def display(self, output, text):
         if not Element(output.id).element:
             js.console.log('not include')
         else:
-            Element(output.id).write(text)
+            Element(output.id).element.value = text
 
     def build(self):
         js.console.log('build')
```

### Comparing `xclass_sdk-1.6.0/src/browser_sdk/math_app_browser.py` & `xclass_sdk-1.6.1/src/browser_sdk/math_app_browser.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.6.0/src/xclass_sdk/general_app.py` & `xclass_sdk-1.6.1/src/xclass_sdk/general_app.py`

 * *Files 26% similar despite different names*

```diff
@@ -55,23 +55,26 @@
         return 0
     
     def build(self, filePath):
         url = self.__API_PATH
         headers = {
             'api-key': self.__apiKey,
         }
-        with open(filePath, 'r') as file:
-            content = file.read()
-            data = {
-                'inputs': json.dumps(self.listInput),
-                'outputs':json.dumps(self.listOutput),
-                'content': content,
-                'okButton': json.dumps(self.okButton),
-                'resetButton': json.dumps(self.resetButton),
-                'name': self.name,
-                'description': self.description,
-                'appLogo': self.appLogo,
-                'author': self.author
-            }
-            response = requests.post(
-                url, files=multipartify(data), headers=headers)
-            print(response.json())
+        try:
+            with open(filePath, 'r', encoding='utf-8') as file:
+                content = file.read()
+                data = {
+                    'inputs': json.dumps(self.listInput),
+                    'outputs':json.dumps(self.listOutput),
+                    'content': content,
+                    'okButton': json.dumps(self.okButton),
+                    'resetButton': json.dumps(self.resetButton),
+                    'name': self.name,
+                    'description': self.description,
+                    'appLogo': self.appLogo,
+                    'author': self.author
+                }
+                response = requests.post(
+                    url, files=multipartify(data), headers=headers)
+                print(response.json())
+        except Exception as e:
+            print("An error occurred:", e)
```

### Comparing `xclass_sdk-1.6.0/src/xclass_sdk/math_app.py` & `xclass_sdk-1.6.1/src/xclass_sdk/math_app.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.6.0/src/xclass_sdk/profile.py` & `xclass_sdk-1.6.1/src/xclass_sdk/profile.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.6.0/src/xclass_sdk/xclass_helpers.py` & `xclass_sdk-1.6.1/src/xclass_sdk/xclass_helpers.py`

 * *Files identical despite different names*

### Comparing `xclass_sdk-1.6.0/src/xclass_sdk.egg-info/PKG-INFO` & `xclass_sdk-1.6.1/src/xclass_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xclass-sdk
-Version: 1.6.0
+Version: 1.6.1
 Summary: X-Class SDK
 Author-email: Trung Nguyen <lantrungseo@gmail.com>
 Project-URL: Homepage, https://github.com/lantrungseo/xclass-sdk
 Project-URL: Bug Tracker, https://github.com/lantrungseo/xclass-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

