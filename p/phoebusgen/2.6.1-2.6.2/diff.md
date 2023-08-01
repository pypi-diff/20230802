# Comparing `tmp/phoebusgen-2.6.1.tar.gz` & `tmp/phoebusgen-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoebusgen-2.6.1.tar", last modified: Thu Jun  8 04:39:42 2023, max compression
+gzip compressed data, was "phoebusgen-2.6.2.tar", last modified: Tue Aug  1 22:47:05 2023, max compression
```

## Comparing `phoebusgen-2.6.1.tar` & `phoebusgen-2.6.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/_shared_property_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/config/classes.bcf
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/config/color.def
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/config/font.def
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/screen/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/screen/screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/phoebusgen/widget/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67600 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/phoebusgen/widget/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.203512 phoebusgen-2.6.1/phoebusgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 04:39:42.000000 phoebusgen-2.6.1/phoebusgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:39:42.207512 phoebusgen-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/tests/test_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-06-08 04:39:29.000000 phoebusgen-2.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/phoebusgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/_shared_property_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/phoebusgen/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/phoebusgen/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/config/classes.bcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/config/color.def
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/config/font.def
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/phoebusgen/screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/screen/screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/phoebusgen/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67590 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/widget/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/phoebusgen/widget/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/phoebusgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-01 22:47:05.000000 phoebusgen-2.6.2/phoebusgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 22:47:05.000000 phoebusgen-2.6.2/phoebusgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:47:05.000000 phoebusgen-2.6.2/phoebusgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 22:47:05.000000 phoebusgen-2.6.2/phoebusgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:47:05.093368 phoebusgen-2.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/tests/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-08-01 22:46:54.000000 phoebusgen-2.6.2/versioneer.py
```

### Comparing `phoebusgen-2.6.1/LICENSE` & `phoebusgen-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/PKG-INFO` & `phoebusgen-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.6.1
+Version: 2.6.2
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.6.1/README.md` & `phoebusgen-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/__init__.py` & `phoebusgen-2.6.2/phoebusgen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/_shared_property_helpers.py` & `phoebusgen-2.6.2/phoebusgen/_shared_property_helpers.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/config/classes.bcf` & `phoebusgen-2.6.2/phoebusgen/config/classes.bcf`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/config/color.def` & `phoebusgen-2.6.2/phoebusgen/config/color.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/config/font.def` & `phoebusgen-2.6.2/phoebusgen/config/font.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/screen/__init__.py` & `phoebusgen-2.6.2/phoebusgen/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/screen/screen.py` & `phoebusgen-2.6.2/phoebusgen/screen/screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/widget/__init__.py` & `phoebusgen-2.6.2/phoebusgen/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/widget/properties.py` & `phoebusgen-2.6.2/phoebusgen/widget/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,24 +640,24 @@
     def confirmation_dialog(self, message: str, password: str = None) -> None:
         """
         Add confirmation dialog to widget, i.e. Are you sure? . Default arg for password is None (no pw)
 
         :param message: Confirmation dialog message
         :param password: Password for dialog. Stored in plain text XML
         """
-        self._shared.boolean_property(self.root, 'show_confirmation_dialog', True)
+        self._shared.boolean_property(self.root, 'show_confirm_dialog', True)
         self._shared.generic_property(self.root, 'confirm_message', message)
         if password is not None:
             self._shared.generic_property(self.root, 'password', password)
 
     def disable_confirmation_dialog(self) -> None:
         """
         Turn off confirmation dialog for widget
         """
-        self._shared.boolean_property(self.root, 'show_confirmation_dialog', False)
+        self._shared.boolean_property(self.root, 'show_confirm_dialog', False)
 
 class _MultiLine(object):
     def multi_line(self, val: bool) -> None:
         """
         Change Multi Line property for widget
 
         :param val: Use multi line?
```

### Comparing `phoebusgen-2.6.1/phoebusgen/widget/widget.py` & `phoebusgen-2.6.2/phoebusgen/widget/widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen/widget/widgets.py` & `phoebusgen-2.6.2/phoebusgen/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/phoebusgen.egg-info/PKG-INFO` & `phoebusgen-2.6.2/phoebusgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.6.1
+Version: 2.6.2
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `phoebusgen-2.6.1/phoebusgen.egg-info/SOURCES.txt` & `phoebusgen-2.6.2/phoebusgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/setup.py` & `phoebusgen-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/tests/test_screen.py` & `phoebusgen-2.6.2/tests/test_screen.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/tests/test_widget.py` & `phoebusgen-2.6.2/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/tests/test_widgets.py` & `phoebusgen-2.6.2/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.6.1/versioneer.py` & `phoebusgen-2.6.2/versioneer.py`

 * *Files identical despite different names*

