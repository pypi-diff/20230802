# Comparing `tmp/Flask-SimplePay-1.3.tar.gz` & `tmp/Flask-SimplePay-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SimplePay-1.3.tar", last modified: Sat Jul  1 06:28:59 2023, max compression
+gzip compressed data, was "Flask-SimplePay-1.4.tar", last modified: Wed Aug  2 10:01:47 2023, max compression
```

## Comparing `Flask-SimplePay-1.3.tar` & `Flask-SimplePay-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:28:59.197876 Flask-SimplePay-1.3/
-drwxrwxrwx   0        0        0        0 2023-07-01 06:28:59.189442 Flask-SimplePay-1.3/Flask_SimplePay.egg-info/
--rw-rw-rw-   0        0        0     1579 2023-07-01 06:28:59.000000 Flask-SimplePay-1.3/Flask_SimplePay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-01 06:28:59.000000 Flask-SimplePay-1.3/Flask_SimplePay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:28:59.000000 Flask-SimplePay-1.3/Flask_SimplePay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-01 06:28:59.000000 Flask-SimplePay-1.3/Flask_SimplePay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.3/LICENSE
--rw-rw-rw-   0        0        0     1579 2023-07-01 06:28:59.197876 Flask-SimplePay-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 06:28:59.195875 Flask-SimplePay-1.3/flask_simplepay/
--rw-rw-rw-   0        0        0       79 2023-06-06 13:16:12.000000 Flask-SimplePay-1.3/flask_simplepay/__init__.py
--rw-rw-rw-   0        0        0     6227 2023-07-01 06:26:12.000000 Flask-SimplePay-1.3/flask_simplepay/core.py
--rw-rw-rw-   0        0        0     6210 2023-06-06 13:16:09.000000 Flask-SimplePay-1.3/flask_simplepay/model.py
--rw-rw-rw-   0        0        0      561 2023-07-01 05:55:42.000000 Flask-SimplePay-1.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-01 06:28:59.199874 Flask-SimplePay-1.3/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-07-01 06:28:31.000000 Flask-SimplePay-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:01:47.193023 Flask-SimplePay-1.4/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:01:47.172019 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/
+-rw-rw-rw-   0        0        0     1579 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.4/LICENSE
+-rw-rw-rw-   0        0        0     1579 2023-08-02 10:01:47.194020 Flask-SimplePay-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:01:47.191075 Flask-SimplePay-1.4/flask_simplepay/
+-rw-rw-rw-   0        0        0       79 2023-06-06 13:16:12.000000 Flask-SimplePay-1.4/flask_simplepay/__init__.py
+-rw-rw-rw-   0        0        0     6245 2023-08-02 09:58:21.000000 Flask-SimplePay-1.4/flask_simplepay/core.py
+-rw-rw-rw-   0        0        0     6210 2023-06-06 13:16:09.000000 Flask-SimplePay-1.4/flask_simplepay/model.py
+-rw-rw-rw-   0        0        0      561 2023-08-02 09:59:35.000000 Flask-SimplePay-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-08-02 10:01:47.196020 Flask-SimplePay-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-08-02 09:59:35.000000 Flask-SimplePay-1.4/setup.py
```

### Comparing `Flask-SimplePay-1.3/Flask_SimplePay.egg-info/PKG-INFO` & `Flask-SimplePay-1.4/Flask_SimplePay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.3
+Version: 1.4
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
 Author-email: gerelorant@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Flask-SimplePay-1.3/LICENSE` & `Flask-SimplePay-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.3/PKG-INFO` & `Flask-SimplePay-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.3
+Version: 1.4
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
 Author-email: gerelorant@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Flask-SimplePay-1.3/README.md` & `Flask-SimplePay-1.4/README.md`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.3/flask_simplepay/core.py` & `Flask-SimplePay-1.4/flask_simplepay/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,24 +110,24 @@
             self.db.session.commit()
 
             return resp
 
         @self.blueprint.route('/ipn', methods=['POST'])
         def ipn():
 
-            # addr = self.app.config.get('SIMPLE_HOST', '94.199.53.96')
-            # if request.remote_addr != addr:
-            #     return abort(403)
+            addr = self.app.config.get('SIMPLE_HOST', '94.199.53.96')
+            if request.remote_addr != addr:
+                return abort(403)
 
-            data = request.json
-            if json is None:
+            data = dict(request.json or request.values)
+            if data is None:
                 return abort(400)
 
             transaction = self.transaction_class.query\
-                .get(data.get('orderRef'), 0)
+                .get(data.get('orderRef', 0))
 
             if transaction is None:
                 return abort(404)
 
             transaction.method = data['method']
             transaction.status = data['status']
             finish = iso8601.parse_date(data['finishDate'])
```

### Comparing `Flask-SimplePay-1.3/flask_simplepay/model.py` & `Flask-SimplePay-1.4/flask_simplepay/model.py`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.3/pyproject.toml` & `Flask-SimplePay-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Flask-SimplePay"
-version = "1.3"
+version = "1.4"
 authors = [
   { name="Gere Lóránt", email="gerelorant@gmail.com" },
 ]
 description = "OTP SimplePay payment extension for Flask"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Flask-SimplePay-1.3/setup.py` & `Flask-SimplePay-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Flask-SimplePay',
-    version='1.3',
+    version='1.4',
     packages=['flask_simplepay'],
     url='https://github.com/gerelorant/Flask-SimplePay',
     license='MIT',
     author='Gere Lóránt',
     author_email='gerelorant@gmail.com',
     description='OTP SimplePay payment extension for Flask',
     include_package_data=True,
```

