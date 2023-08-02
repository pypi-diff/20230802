# Comparing `tmp/micropub-0.1.1.tar.gz` & `tmp/micropub-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropub-0.1.1.tar", max compression
+gzip compressed data, was "micropub-0.1.2.tar", max compression
```

## Comparing `micropub-0.1.1.tar` & `micropub-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3473 2023-01-27 00:43:27.627920 micropub-0.1.1/micropub/__init__.py
--rw-r--r--   0        0        0     2737 2023-01-27 00:43:27.627920 micropub-0.1.1/micropub/__main__.py
--rw-r--r--   0        0        0      996 2023-01-27 05:18:54.652572 micropub-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 micropub-0.1.1/setup.py
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 micropub-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3473 2023-07-20 05:38:30.720873 micropub-0.1.2/micropub/__init__.py
+-rw-r--r--   0        0        0     2737 2023-02-13 00:57:16.634666 micropub-0.1.2/micropub/__main__.py
+-rw-r--r--   0        0        0      993 2023-08-02 03:47:39.376928 micropub-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 micropub-0.1.2/setup.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 micropub-0.1.2/PKG-INFO
```

### Comparing `micropub-0.1.1/micropub/__init__.py` & `micropub-0.1.2/micropub/__init__.py`

 * *Files identical despite different names*

### Comparing `micropub-0.1.1/micropub/__main__.py` & `micropub-0.1.2/micropub/__main__.py`

 * *Files identical despite different names*

### Comparing `micropub-0.1.1/pyproject.toml` & `micropub-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "micropub"
-version = "0.1.1"
+version = "0.1.2"
 description = "utilities to help implement Micropub servers and clients"
 keywords = ["IndieWeb", "Micropub"]
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "0BSD"
 
 [tool.poetry.scripts]
 micropub = "micropub.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 requests = "^2.28.2"
 txtint = ">=0.0"
 microformats = ">=0.0"
 indieauth = ">=0.0"
-requests-toolbelt = "^0.10.1"
+requests-toolbelt = "^1.0"
 
 [tool.poetry.group.dev.dependencies]
 nuitka = "^1.2.6"
 zstandard = "^0.19.0"
 ordered-set = "^4.1.0"
 gmpg = {path="../gmpg", develop=true}
 txtint = {path="../txtint", develop=true}
```

### Comparing `micropub-0.1.1/setup.py` & `micropub-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['indieauth>=0.0',
  'microformats>=0.0',
- 'requests-toolbelt>=0.10.1,<0.11.0',
+ 'requests-toolbelt>=1.0,<2.0',
  'requests>=2.28.2,<3.0.0',
  'txtint>=0.0']
 
 entry_points = \
 {'console_scripts': ['micropub = micropub.__main__:main']}
 
 setup_kwargs = {
     'name': 'micropub',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'utilities to help implement Micropub servers and clients',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

