# Comparing `tmp/pyscfg-0.2.0.tar.gz` & `tmp/pyscfg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyscfg-0.2.0.tar", last modified: Fri Oct 22 18:22:38 2021, max compression
+gzip compressed data, was "dist\pyscfg-0.2.1.tar", last modified: Wed Aug  2 09:40:17 2023, max compression
```

## Comparing `pyscfg-0.2.0.tar` & `pyscfg-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-10-22 18:22:38.000000 pyscfg-0.2.0/
--rw-rw-rw-   0        0        0     5614 2021-10-22 18:22:38.000000 pyscfg-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3764 2021-10-22 18:08:25.000000 pyscfg-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg/
--rw-rw-rw-   0        0        0      355 2021-10-22 18:08:25.000000 pyscfg-0.2.0/pyscfg/__init__.py
--rw-rw-rw-   0        0        0     8122 2021-10-22 18:08:25.000000 pyscfg-0.2.0/pyscfg/core.py
--rw-rw-rw-   0        0        0      635 2021-01-23 20:19:56.000000 pyscfg-0.2.0/pyscfg/helpers.py
--rw-rw-rw-   0        0        0     3749 2021-10-22 18:08:25.000000 pyscfg-0.2.0/pyscfg/stores.py
-drwxrwxrwx   0        0        0        0 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg.egg-info/
--rw-rw-rw-   0        0        0     5614 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-10-22 18:22:38.000000 pyscfg-0.2.0/pyscfg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-10-22 18:22:38.000000 pyscfg-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1191 2021-10-22 18:08:25.000000 pyscfg-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:40:17.000000 pyscfg-0.2.1/
+-rw-rw-rw-   0        0        0     5614 2023-08-02 09:40:17.000000 pyscfg-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3764 2021-10-22 18:08:25.000000 pyscfg-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg/
+-rw-rw-rw-   0        0        0      355 2021-10-22 18:08:25.000000 pyscfg-0.2.1/pyscfg/__init__.py
+-rw-rw-rw-   0        0        0     8175 2023-08-02 09:16:05.000000 pyscfg-0.2.1/pyscfg/core.py
+-rw-rw-rw-   0        0        0      635 2021-01-23 20:19:56.000000 pyscfg-0.2.1/pyscfg/helpers.py
+-rw-rw-rw-   0        0        0     3749 2021-10-22 18:08:25.000000 pyscfg-0.2.1/pyscfg/stores.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg.egg-info/
+-rw-rw-rw-   0        0        0     5614 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 09:40:17.000000 pyscfg-0.2.1/pyscfg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:40:17.000000 pyscfg-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1191 2023-08-02 09:34:14.000000 pyscfg-0.2.1/setup.py
```

### Comparing `pyscfg-0.2.0/PKG-INFO` & `pyscfg-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscfg
-Version: 0.2.0
+Version: 0.2.1
 Summary: simple handling of user configuration
 Home-page: UNKNOWN
 Author: Christopher Mertens
 Author-email: suppetia@gmx.de
 License: UNKNOWN
 Project-URL: Github, https://github.com/suppetia/pyscfg
 Description: # pyscfg - _Python Simple Configuration_
```

### Comparing `pyscfg-0.2.0/README.md` & `pyscfg-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyscfg-0.2.0/pyscfg/core.py` & `pyscfg-0.2.1/pyscfg/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
         # init the configs with some default values if there are no values stored for this values
         if defaults:
             if isinstance(defaults, str):
                 defaults = get_store(filename=defaults).load()
             data = defaults
 
         store_data = store.load()
-        data.update(store_data)
+        data.update(ConfigsDict._flatten_dict(store_data))
+        store.save(data)
 
         super().__init__(data=data, data_store=store)
 
     def __repr__(self):
         return f"SimpleConfigs({str(self._configs)} \
             ,\n\tstore:{type(self._data_store) if self._data_store is not None else self._data_store})"
```

### Comparing `pyscfg-0.2.0/pyscfg/helpers.py` & `pyscfg-0.2.1/pyscfg/helpers.py`

 * *Files identical despite different names*

### Comparing `pyscfg-0.2.0/pyscfg/stores.py` & `pyscfg-0.2.1/pyscfg/stores.py`

 * *Files identical despite different names*

### Comparing `pyscfg-0.2.0/pyscfg.egg-info/PKG-INFO` & `pyscfg-0.2.1/pyscfg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscfg
-Version: 0.2.0
+Version: 0.2.1
 Summary: simple handling of user configuration
 Home-page: UNKNOWN
 Author: Christopher Mertens
 Author-email: suppetia@gmx.de
 License: UNKNOWN
 Project-URL: Github, https://github.com/suppetia/pyscfg
 Description: # pyscfg - _Python Simple Configuration_
```

### Comparing `pyscfg-0.2.0/setup.py` & `pyscfg-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 name = "pyscfg"
-version = "0.2.0"
+version = "0.2.1"
 
 # get list of requirements
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 # get README as long description
 with open('README.md', encoding='utf-8') as f:
```

