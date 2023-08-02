# Comparing `tmp/NotifPy-0.0.1.tar.gz` & `tmp/NotifPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotifPy-0.0.1.tar", last modified: Wed Aug  2 15:20:58 2023, max compression
+gzip compressed data, was "NotifPy-0.0.2.tar", last modified: Wed Aug  2 16:40:42 2023, max compression
```

## Comparing `NotifPy-0.0.1.tar` & `NotifPy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:20:58.093214 NotifPy-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-08-02 13:31:49.000000 NotifPy-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-02 15:20:58.073217 NotifPy-0.0.1/NotifPy/
--rw-rw-rw-   0        0        0     2523 2023-08-02 14:41:28.000000 NotifPy-0.0.1/NotifPy/EmailNotif.py
--rw-rw-rw-   0        0        0      927 2023-08-02 14:16:23.000000 NotifPy-0.0.1/NotifPy/SMSNotif.py
--rw-rw-rw-   0        0        0        0 2023-08-02 13:20:01.000000 NotifPy-0.0.1/NotifPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:20:58.091216 NotifPy-0.0.1/NotifPy.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-08-02 15:20:58.000000 NotifPy-0.0.1/NotifPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-08-02 15:20:58.000000 NotifPy-0.0.1/NotifPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:20:58.000000 NotifPy-0.0.1/NotifPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 15:20:58.000000 NotifPy-0.0.1/NotifPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2942 2023-08-02 15:20:58.093214 NotifPy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2495 2023-08-02 15:14:13.000000 NotifPy-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-08-02 13:28:49.000000 NotifPy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      543 2023-08-02 15:20:58.101215 NotifPy-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 16:40:42.192705 NotifPy-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-08-02 13:31:49.000000 NotifPy-0.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-02 16:40:42.168706 NotifPy-0.0.2/NotifPy/
+-rw-rw-rw-   0        0        0     2523 2023-08-02 14:41:28.000000 NotifPy-0.0.2/NotifPy/EmailNotif.py
+-rw-rw-rw-   0        0        0      927 2023-08-02 14:16:23.000000 NotifPy-0.0.2/NotifPy/SMSNotif.py
+-rw-rw-rw-   0        0        0        0 2023-08-02 13:20:01.000000 NotifPy-0.0.2/NotifPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:40:42.191717 NotifPy-0.0.2/NotifPy.egg-info/
+-rw-rw-rw-   0        0        0     2979 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2979 2023-08-02 16:40:42.193705 NotifPy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2495 2023-08-02 15:14:13.000000 NotifPy-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-08-02 13:28:49.000000 NotifPy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      580 2023-08-02 16:40:42.195705 NotifPy-0.0.2/setup.cfg
```

### Comparing `NotifPy-0.0.1/LICENSE` & `NotifPy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NotifPy-0.0.1/NotifPy/EmailNotif.py` & `NotifPy-0.0.2/NotifPy/EmailNotif.py`

 * *Files identical despite different names*

### Comparing `NotifPy-0.0.1/NotifPy/SMSNotif.py` & `NotifPy-0.0.2/NotifPy/SMSNotif.py`

 * *Files identical despite different names*

### Comparing `NotifPy-0.0.1/NotifPy.egg-info/PKG-INFO` & `NotifPy-0.0.2/NotifPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NotifPy
-Version: 0.0.1
-Summary: For generating A E S T H E T I C ascii art
+Version: 0.0.2
+Summary: NotifPy is here to send alert, notification and promotion related email and SMS
 Home-page: https://github.com/ArianFotouhi
 Author: Arian
 Author-email: arianspiderman@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NotifPy-0.0.1/PKG-INFO` & `NotifPy-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NotifPy
-Version: 0.0.1
-Summary: For generating A E S T H E T I C ascii art
+Version: 0.0.2
+Summary: NotifPy is here to send alert, notification and promotion related email and SMS
 Home-page: https://github.com/ArianFotouhi
 Author: Arian
 Author-email: arianspiderman@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NotifPy-0.0.1/README.md` & `NotifPy-0.0.2/README.md`

 * *Files identical despite different names*

