# Comparing `tmp/Flask-SimplePay-1.4.tar.gz` & `tmp/Flask-SimplePay-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SimplePay-1.4.tar", last modified: Wed Aug  2 10:01:47 2023, max compression
+gzip compressed data, was "Flask-SimplePay-1.5.tar", last modified: Wed Aug  2 10:22:32 2023, max compression
```

## Comparing `Flask-SimplePay-1.4.tar` & `Flask-SimplePay-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:01:47.193023 Flask-SimplePay-1.4/
-drwxrwxrwx   0        0        0        0 2023-08-02 10:01:47.172019 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/
--rw-rw-rw-   0        0        0     1579 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 10:01:46.000000 Flask-SimplePay-1.4/Flask_SimplePay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.4/LICENSE
--rw-rw-rw-   0        0        0     1579 2023-08-02 10:01:47.194020 Flask-SimplePay-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 10:01:47.191075 Flask-SimplePay-1.4/flask_simplepay/
--rw-rw-rw-   0        0        0       79 2023-06-06 13:16:12.000000 Flask-SimplePay-1.4/flask_simplepay/__init__.py
--rw-rw-rw-   0        0        0     6245 2023-08-02 09:58:21.000000 Flask-SimplePay-1.4/flask_simplepay/core.py
--rw-rw-rw-   0        0        0     6210 2023-06-06 13:16:09.000000 Flask-SimplePay-1.4/flask_simplepay/model.py
--rw-rw-rw-   0        0        0      561 2023-08-02 09:59:35.000000 Flask-SimplePay-1.4/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-08-02 10:01:47.196020 Flask-SimplePay-1.4/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-08-02 09:59:35.000000 Flask-SimplePay-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:22:32.872579 Flask-SimplePay-1.5/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:22:32.865577 Flask-SimplePay-1.5/Flask_SimplePay.egg-info/
+-rw-rw-rw-   0        0        0     1579 2023-08-02 10:22:32.000000 Flask-SimplePay-1.5/Flask_SimplePay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-08-02 10:22:32.000000 Flask-SimplePay-1.5/Flask_SimplePay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:22:32.000000 Flask-SimplePay-1.5/Flask_SimplePay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 10:22:32.000000 Flask-SimplePay-1.5/Flask_SimplePay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-06-06 07:26:34.000000 Flask-SimplePay-1.5/LICENSE
+-rw-rw-rw-   0        0        0     1579 2023-08-02 10:22:32.872579 Flask-SimplePay-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1247 2023-06-06 07:26:34.000000 Flask-SimplePay-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:22:32.871574 Flask-SimplePay-1.5/flask_simplepay/
+-rw-rw-rw-   0        0        0       79 2023-06-06 13:16:12.000000 Flask-SimplePay-1.5/flask_simplepay/__init__.py
+-rw-rw-rw-   0        0        0     6994 2023-08-02 10:21:30.000000 Flask-SimplePay-1.5/flask_simplepay/core.py
+-rw-rw-rw-   0        0        0     6210 2023-06-06 13:16:09.000000 Flask-SimplePay-1.5/flask_simplepay/model.py
+-rw-rw-rw-   0        0        0      561 2023-08-02 10:21:58.000000 Flask-SimplePay-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-08-02 10:22:32.874575 Flask-SimplePay-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-08-02 10:21:59.000000 Flask-SimplePay-1.5/setup.py
```

### Comparing `Flask-SimplePay-1.4/Flask_SimplePay.egg-info/PKG-INFO` & `Flask-SimplePay-1.5/Flask_SimplePay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.4
+Version: 1.5
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
 Author-email: gerelorant@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Flask-SimplePay-1.4/LICENSE` & `Flask-SimplePay-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.4/PKG-INFO` & `Flask-SimplePay-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SimplePay
-Version: 1.4
+Version: 1.5
 Summary: OTP SimplePay payment extension for Flask
 Home-page: https://github.com/gerelorant/Flask-SimplePay
 Author: Gere Lóránt
 Author-email: gerelorant@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Flask-SimplePay-1.4/README.md` & `Flask-SimplePay-1.5/README.md`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.4/flask_simplepay/core.py` & `Flask-SimplePay-1.5/flask_simplepay/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import base64
 import datetime as dt
+import logging
 import random
 import json
 import typing
 
 from flask import Flask, Blueprint, abort, redirect, request, make_response, \
     jsonify, flash
 from flask_sqlalchemy import SQLAlchemy
 import iso8601
 import pytz
 
 from flask_simplepay.model import TransactionMixin, OrderAddressMixin
 
 
+logger = logging.getLogger('simple_pay')
+
+
 class SimplePay(object):
     """Flask-SimplePay extension class.
 
     :param app: Flask application instance
     :param db: Flask-SQLAlchemy instance
     :param transaction_class: Transaction model class
     :param address_class: Order address model class
@@ -58,14 +62,15 @@
             'simple_pay',
             __name__,
             url_prefix='/simple_pay'
         )
 
         @self.blueprint.route('/start/<int:transaction_id>', methods=['POST'])
         def start(transaction_id: int):
+            logger.info(f'Starting transaction {transaction_id}...')
             test = request.args.get('test', False)
 
             transaction = self.transaction_class.query.get(transaction_id)
             if transaction is None:
                 return abort(404)
 
             language = request.values.get('language', None)
@@ -78,70 +83,84 @@
                     customer_email=customer_email,
                     language=language,
                     test=test)
             finally:
                 self.db.session.commit()
 
             if 'paymentUrl' in resp:
+                logger.info(f'Redirecting transaction {transaction_id}...')
                 return redirect(resp['paymentUrl'])
             else:
                 errors = resp.get('errorCodes', [])
                 error_msg = 'Hiba' if transaction.language == 'HU' else 'Error'
 
+                logger.info(f'Transaction {transaction_id} failed: {errors}')
                 flash(f'{error_msg}: {errors}')
                 return redirect(request.referrer)
 
         @self.blueprint.route('/back')
         def back():
+            logger.info(f'Back route called')
             response = request.args.get('r', None)
             if response is None:
                 return abort(400)
 
             data = json.loads(base64.b64decode(response))
             transaction = self.transaction_class.query.get(data.get('o', 0))
 
             if transaction is None:
                 return abort(404)
 
             event = data['e'].lower()
 
+
             transaction.result = event
             transaction.simple_id = data.get('t', None)
+
+            logger.info(f'Back for transaction {transaction.id} is {transaction.result}, simple ID: {transaction.simple_id}')
+
             resp = transaction.back()
             self.db.session.commit()
 
             return resp
 
         @self.blueprint.route('/ipn', methods=['POST'])
         def ipn():
+            logger.info(f'IPN called...')
 
             addr = self.app.config.get('SIMPLE_HOST', '94.199.53.96')
             if request.remote_addr != addr:
+                logger.info(f'IPN called from unknown host')
                 return abort(403)
 
             data = dict(request.json or request.values)
             if data is None:
+                logger.info(f'IPN called without data')
                 return abort(400)
 
             transaction = self.transaction_class.query\
                 .get(data.get('orderRef', 0))
 
             if transaction is None:
+                logger.info(f'IPN called with unknown transaction')
                 return abort(404)
 
             transaction.method = data['method']
             transaction.status = data['status']
             finish = iso8601.parse_date(data['finishDate'])
             transaction.finish_time = finish.astimezone(pytz.timezone('utc'))
 
             self.db.session.commit()
 
             data['receiveDate'] = dt.datetime.now().astimezone().isoformat()
 
             data = json.dumps(data).encode('utf8')
+
+            logger.info(f'IPN data: {data}')
+
             signature = transaction.signature(data)
 
             response = make_response(data)
             response.headers['Signature'] = signature
             response.headers['Content-type'] = 'application/json'
             return response
```

### Comparing `Flask-SimplePay-1.4/flask_simplepay/model.py` & `Flask-SimplePay-1.5/flask_simplepay/model.py`

 * *Files identical despite different names*

### Comparing `Flask-SimplePay-1.4/pyproject.toml` & `Flask-SimplePay-1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Flask-SimplePay"
-version = "1.4"
+version = "1.5"
 authors = [
   { name="Gere Lóránt", email="gerelorant@gmail.com" },
 ]
 description = "OTP SimplePay payment extension for Flask"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Flask-SimplePay-1.4/setup.py` & `Flask-SimplePay-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Flask-SimplePay',
-    version='1.4',
+    version='1.5',
     packages=['flask_simplepay'],
     url='https://github.com/gerelorant/Flask-SimplePay',
     license='MIT',
     author='Gere Lóránt',
     author_email='gerelorant@gmail.com',
     description='OTP SimplePay payment extension for Flask',
     include_package_data=True,
```

