# Comparing `tmp/python-objectifier-1.1.tar.gz` & `tmp/python-objectifier-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-objectifier-1.1.tar", last modified: Thu Mar  2 18:43:50 2023, max compression
+gzip compressed data, was "python-objectifier-1.2.tar", last modified: Wed Aug  2 13:01:57 2023, max compression
```

## Comparing `python-objectifier-1.1.tar` & `python-objectifier-1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 18:43:50.175090 python-objectifier-1.1/
--rw-rw-rw-   0        0        0       38 2023-03-02 18:38:58.000000 python-objectifier-1.1/.gitignore
--rw-rw-rw-   0        0        0      344 2023-03-02 18:43:50.175090 python-objectifier-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-02-27 16:50:48.000000 python-objectifier-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 18:43:50.169094 python-objectifier-1.1/objectifier/
--rw-rw-rw-   0        0        0     1183 2023-03-02 18:34:28.000000 python-objectifier-1.1/objectifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-02 18:43:50.174091 python-objectifier-1.1/python_objectifier.egg-info/
--rw-rw-rw-   0        0        0      344 2023-03-02 18:43:49.000000 python-objectifier-1.1/python_objectifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-03-02 18:43:49.000000 python-objectifier-1.1/python_objectifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 18:43:49.000000 python-objectifier-1.1/python_objectifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-02 18:43:49.000000 python-objectifier-1.1/python_objectifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-02 18:43:50.176089 python-objectifier-1.1/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-03-02 18:43:46.000000 python-objectifier-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:01:57.682433 python-objectifier-1.2/
+-rw-rw-rw-   0        0        0       38 2023-03-02 18:38:58.000000 python-objectifier-1.2/.gitignore
+-rw-rw-rw-   0        0        0     2272 2023-08-02 13:01:57.682433 python-objectifier-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2023-03-11 18:35:14.000000 python-objectifier-1.2/README.md
+-rw-rw-rw-   0        0        0      285 2023-03-30 16:24:49.000000 python-objectifier-1.2/file.json
+drwxrwxrwx   0        0        0        0 2023-08-02 13:01:57.678437 python-objectifier-1.2/objectifier/
+-rw-rw-rw-   0        0        0     1185 2023-08-02 13:01:45.000000 python-objectifier-1.2/objectifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:01:57.681434 python-objectifier-1.2/python_objectifier.egg-info/
+-rw-rw-rw-   0        0        0     2272 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 13:01:57.000000 python-objectifier-1.2/python_objectifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 13:01:57.683433 python-objectifier-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-08-02 13:01:49.000000 python-objectifier-1.2/setup.py
```

### Comparing `python-objectifier-1.1/objectifier/__init__.py` & `python-objectifier-1.2/objectifier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-class convert_dictionary_to_object(dict): # https://goodcode.io/articles/python-dict-object/
-    def __getattr__(self, name):
-        if name in self:
-            return self[name]
-        else:
-            raise AttributeError("No such attribute: " + name)
-
-    def __setattr__(self, name, value):
-        self[name] = value
-
-    def __delattr__(self, name):
-        if name in self:
-            del self[name]
-        else:
-            raise AttributeError("No such attribute: " + name)
-
 class convert_json_to_object:
     def __new__(self, item):
         if isinstance(item, dict):
-            updated_dict = convert_dictionary_to_object()
+            updated_dict = _convert_dictionary_to_object()
             for key, value in item.items():
                 if isinstance(value, (dict, list)):
                     value = convert_json_to_object(value)
                 setattr(updated_dict, key, value)
                     
             return updated_dict
 
         elif isinstance(item, list):
             for index, sub_item in enumerate(item):
                 if isinstance(sub_item, (dict, list)):
                     item[index] = convert_json_to_object(sub_item)
                 
-            return item
+            return item
+
+class _convert_dictionary_to_object(dict): # https://goodcode.io/articles/python-dict-object/
+    def __getattr__(self, name):
+        if name in self:
+            return self[name]
+        else:
+            raise AttributeError("No such attribute: " + name)
+
+    def __setattr__(self, name, value):
+        self[name] = value
+
+    def __delattr__(self, name):
+        if name in self:
+            del self[name]
+        else:
+            raise AttributeError("No such attribute: " + name)
```

