# Comparing `tmp/specable-0.1.0.tar.gz` & `tmp/specable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specable-0.1.0.tar", max compression
+gzip compressed data, was "specable-0.1.1.tar", max compression
```

## Comparing `specable-0.1.0.tar` & `specable-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      367 2021-08-18 09:36:02.316157 specable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      105 2021-07-27 14:45:31.510944 specable-0.1.0/specable/__init__.py
--rw-r--r--   0        0        0      881 2021-07-27 13:56:31.095857 specable-0.1.0/specable/dicts.py
--rw-r--r--   0        0        0      768 2021-07-27 17:03:45.645689 specable-0.1.0/specable/inout.py
--rw-r--r--   0        0        0     2162 2021-07-27 17:19:57.634061 specable-0.1.0/specable/interface.py
--rw-r--r--   0        0        0     1078 2021-07-27 15:28:36.284150 specable-0.1.0/specable/specable.py
--rw-r--r--   0        0        0      623 2021-08-18 09:40:18.252332 specable-0.1.0/setup.py
--rw-r--r--   0        0        0      484 2021-08-18 09:40:18.252795 specable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-08-02 07:58:12.663283 specable-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      105 2021-07-27 14:45:31.510944 specable-0.1.1/specable/__init__.py
+-rw-r--r--   0        0        0      881 2021-07-27 13:56:31.095857 specable-0.1.1/specable/dicts.py
+-rw-r--r--   0        0        0      768 2021-07-27 17:03:45.645689 specable-0.1.1/specable/inout.py
+-rw-r--r--   0        0        0     2162 2021-07-27 17:19:57.634061 specable-0.1.1/specable/interface.py
+-rw-r--r--   0        0        0     1082 2021-11-03 13:19:26.519394 specable-0.1.1/specable/specable.py
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 specable-0.1.1/PKG-INFO
```

### Comparing `specable-0.1.0/specable/dicts.py` & `specable-0.1.1/specable/dicts.py`

 * *Files identical despite different names*

### Comparing `specable-0.1.0/specable/inout.py` & `specable-0.1.1/specable/inout.py`

 * *Files identical despite different names*

### Comparing `specable-0.1.0/specable/interface.py` & `specable-0.1.1/specable/interface.py`

 * *Files identical despite different names*

### Comparing `specable-0.1.0/specable/specable.py` & `specable-0.1.1/specable/specable.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return f"{cls.get_namespace()}/{cls.get_kind()}"
 
     @classmethod
     def get_kind(cls):
         if cls.kind is None:
             return cls.__name__.lower()
         else:
-            return kind
+            return cls.kind
 
     @classmethod
     def get_namespace(cls):
         if cls.namespace is None:
             return cls.__module__.split(".")[0]
         else:
             return cls.namespace
```

