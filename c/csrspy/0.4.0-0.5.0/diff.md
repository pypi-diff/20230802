# Comparing `tmp/csrspy-0.4.0.tar.gz` & `tmp/csrspy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csrspy-0.4.0.tar", max compression
+gzip compressed data, was "csrspy-0.5.0.tar", max compression
```

## Comparing `csrspy-0.4.0.tar` & `csrspy-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      130 2022-12-06 01:20:25.526854 csrspy-0.4.0/csrspy/__init__.py
--rw-r--r--   0        0        0     1036 2022-12-06 01:20:05.262663 csrspy-0.4.0/csrspy/enums.py
--rw-r--r--   0        0        0     5505 2022-12-06 01:20:05.262663 csrspy-0.4.0/csrspy/factories.py
--rw-r--r--   0        0        0    10830 2022-12-06 01:20:05.262663 csrspy-0.4.0/csrspy/main.py
--rw-r--r--   0        0        0      450 2022-12-06 01:20:25.874857 csrspy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 csrspy-0.4.0/setup.py
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 csrspy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-08-02 19:21:09.982944 csrspy-0.5.0/csrspy/__init__.py
+-rw-r--r--   0        0        0     1036 2023-08-02 19:19:58.547100 csrspy-0.5.0/csrspy/enums.py
+-rw-r--r--   0        0        0     8742 2023-08-02 19:19:58.547100 csrspy-0.5.0/csrspy/factories.py
+-rw-r--r--   0        0        0    12028 2023-08-02 19:19:58.547100 csrspy-0.5.0/csrspy/main.py
+-rw-r--r--   0        0        0      545 2023-08-02 19:21:10.438969 csrspy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 csrspy-0.5.0/setup.py
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 csrspy-0.5.0/PKG-INFO
```

### Comparing `csrspy-0.4.0/setup.py` & `csrspy-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['csrspy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyproj>=3.4.0,<4.0.0']
+['pyproj>=3.6,<4.0']
 
 setup_kwargs = {
     'name': 'csrspy',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'ITRF/NAD83CSRS coordinate transforms in Python',
     'long_description': 'None',
     'author': 'Taylor Denouden',
-    'author_email': 'taylordenouden@gmail.com',
+    'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

