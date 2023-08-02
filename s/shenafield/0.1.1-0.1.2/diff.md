# Comparing `tmp/shenafield-0.1.1.tar.gz` & `tmp/shenafield-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shenafield-0.1.1.tar", max compression
+gzip compressed data, was "shenafield-0.1.2.tar", max compression
```

## Comparing `shenafield-0.1.1.tar` & `shenafield-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-02 18:43:21.155094 shenafield-0.1.1/README.md
--rw-r--r--   0        0        0      457 2023-08-02 19:19:47.789220 shenafield-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      114 2023-08-02 18:46:02.270388 shenafield-0.1.1/shenafield/__init__.py
--rw-r--r--   0        0        0     2253 2023-08-02 19:06:53.142981 shenafield-0.1.1/shenafield/cli.py
--rw-r--r--   0        0        0     1588 2023-08-02 19:02:57.734223 shenafield-0.1.1/shenafield/shenafield.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 shenafield-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-08-02 19:24:40.289219 shenafield-0.1.2/README.md
+-rw-r--r--   0        0        0      457 2023-08-02 19:24:53.257187 shenafield-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-08-02 18:46:02.270388 shenafield-0.1.2/shenafield/__init__.py
+-rw-r--r--   0        0        0     2253 2023-08-02 19:06:53.142981 shenafield-0.1.2/shenafield/cli.py
+-rw-r--r--   0        0        0     1588 2023-08-02 19:02:57.734223 shenafield-0.1.2/shenafield/shenafield.py
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 shenafield-0.1.2/PKG-INFO
```

### Comparing `shenafield-0.1.1/shenafield/cli.py` & `shenafield-0.1.2/shenafield/cli.py`

 * *Files identical despite different names*

### Comparing `shenafield-0.1.1/shenafield/shenafield.py` & `shenafield-0.1.2/shenafield/shenafield.py`

 * *Files identical despite different names*

