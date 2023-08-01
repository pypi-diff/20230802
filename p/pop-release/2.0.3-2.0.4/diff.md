# Comparing `tmp/pop-release-2.0.3.tar.gz` & `tmp/pop-release-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pop-release-2.0.3.tar", last modified: Tue May 25 22:51:23 2021, max compression
+gzip compressed data, was "dist/pop-release-2.0.4.tar", last modified: Tue May 25 22:53:56 2021, max compression
```

## Comparing `pop-release-2.0.3.tar` & `pop-release-2.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/
--rw-r--r--   0 akmod     (1000) akmod     (1000)    11340 2021-05-22 07:42:20.000000 pop-release-2.0.3/LICENSE
--rw-r--r--   0 akmod     (1000) akmod     (1000)     7495 2021-05-25 22:51:23.000000 pop-release-2.0.3/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)     5313 2021-05-22 17:11:32.000000 pop-release-2.0.3/README.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/acct/
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/acct/twine/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      580 2021-05-22 18:00:04.000000 pop-release-2.0.3/pop_release/acct/twine/settings.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1083 2021-05-22 17:59:31.000000 pop-release-2.0.3/pop_release/conf.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/exec/
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/exec/twine/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1558 2021-05-22 09:24:15.000000 pop-release-2.0.3/pop_release/exec/twine/command.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/exec/twine/contracts/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      276 2021-05-22 08:44:16.000000 pop-release-2.0.3/pop_release/exec/twine/contracts/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)       55 2021-05-21 17:55:19.000000 pop-release-2.0.3/pop_release/exec/twine/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      489 2021-05-22 08:46:57.000000 pop-release-2.0.3/pop_release/exec/twine/repository.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/pop_release/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      720 2021-05-25 22:50:35.000000 pop-release-2.0.3/pop_release/pop_release/dist.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      794 2021-05-22 09:24:15.000000 pop-release-2.0.3/pop_release/pop_release/gitpy.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2644 2021-05-22 18:05:44.000000 pop-release-2.0.3/pop_release/pop_release/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      438 2021-05-22 08:32:51.000000 pop-release-2.0.3/pop_release/pop_release/test.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      461 2021-05-22 09:18:08.000000 pop-release-2.0.3/pop_release/pop_release/twine.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1464 2021-05-22 08:32:51.000000 pop-release-2.0.3/pop_release/pop_release/version.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      178 2020-11-23 10:00:03.000000 pop-release-2.0.3/pop_release/scripts.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)       42 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release/version.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     7495 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)      695 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/SOURCES.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)        1 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/dependency_links.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       59 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/entry_points.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       55 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/requires.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       12 2021-05-25 22:51:23.000000 pop-release-2.0.3/pop_release.egg-info/top_level.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)      255 2020-11-23 10:00:03.000000 pop-release-2.0.3/pyproject.toml
--rw-r--r--   0 akmod     (1000) akmod     (1000)       38 2021-05-25 22:51:23.000000 pop-release-2.0.3/setup.cfg
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2198 2021-05-22 18:00:04.000000 pop-release-2.0.3/setup.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)    11340 2021-05-22 07:42:20.000000 pop-release-2.0.4/LICENSE
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     7495 2021-05-25 22:53:56.000000 pop-release-2.0.4/PKG-INFO
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     5313 2021-05-22 17:11:32.000000 pop-release-2.0.4/README.rst
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/acct/
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/acct/twine/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      580 2021-05-22 18:00:04.000000 pop-release-2.0.4/pop_release/acct/twine/settings.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1083 2021-05-22 17:59:31.000000 pop-release-2.0.4/pop_release/conf.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/exec/
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/exec/twine/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1558 2021-05-22 09:24:15.000000 pop-release-2.0.4/pop_release/exec/twine/command.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/exec/twine/contracts/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      276 2021-05-22 08:44:16.000000 pop-release-2.0.4/pop_release/exec/twine/contracts/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       55 2021-05-21 17:55:19.000000 pop-release-2.0.4/pop_release/exec/twine/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      489 2021-05-22 08:46:57.000000 pop-release-2.0.4/pop_release/exec/twine/repository.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release/pop_release/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      720 2021-05-25 22:50:35.000000 pop-release-2.0.4/pop_release/pop_release/dist.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      794 2021-05-22 09:24:15.000000 pop-release-2.0.4/pop_release/pop_release/gitpy.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     2644 2021-05-22 18:05:44.000000 pop-release-2.0.4/pop_release/pop_release/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      438 2021-05-22 08:32:51.000000 pop-release-2.0.4/pop_release/pop_release/test.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      461 2021-05-22 09:18:08.000000 pop-release-2.0.4/pop_release/pop_release/twine.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1464 2021-05-22 08:32:51.000000 pop-release-2.0.4/pop_release/pop_release/version.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      178 2020-11-23 10:00:03.000000 pop-release-2.0.4/pop_release/scripts.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       42 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release/version.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-05-25 22:53:56.000000 pop-release-2.0.4/pop_release.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     7495 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release.egg-info/PKG-INFO
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      695 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release.egg-info/SOURCES.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)        1 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release.egg-info/dependency_links.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       59 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release.egg-info/entry_points.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       59 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release.egg-info/requires.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       12 2021-05-25 22:53:55.000000 pop-release-2.0.4/pop_release.egg-info/top_level.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      255 2020-11-23 10:00:03.000000 pop-release-2.0.4/pyproject.toml
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       38 2021-05-25 22:53:56.000000 pop-release-2.0.4/setup.cfg
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     2198 2021-05-22 18:00:04.000000 pop-release-2.0.4/setup.py
```

### Comparing `pop-release-2.0.3/LICENSE` & `pop-release-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/PKG-INFO` & `pop-release-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-release
-Version: 2.0.3
+Version: 2.0.4
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-release
 Maintainer: Tyler Johnson
 Maintainer-email: tyjohnson@vmware.com
 License: UNKNOWN
 Description: ===========
         POP-RELEASE
```

### Comparing `pop-release-2.0.3/README.rst` & `pop-release-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/acct/twine/settings.py` & `pop-release-2.0.4/pop_release/acct/twine/settings.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/conf.py` & `pop-release-2.0.4/pop_release/conf.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/exec/twine/command.py` & `pop-release-2.0.4/pop_release/exec/twine/command.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/pop_release/dist.py` & `pop-release-2.0.4/pop_release/pop_release/dist.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/pop_release/gitpy.py` & `pop-release-2.0.4/pop_release/pop_release/gitpy.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/pop_release/init.py` & `pop-release-2.0.4/pop_release/pop_release/init.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release/pop_release/version.py` & `pop-release-2.0.4/pop_release/pop_release/version.py`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/pop_release.egg-info/PKG-INFO` & `pop-release-2.0.4/pop_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-release
-Version: 2.0.3
+Version: 2.0.4
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-release
 Maintainer: Tyler Johnson
 Maintainer-email: tyjohnson@vmware.com
 License: UNKNOWN
 Description: ===========
         POP-RELEASE
```

### Comparing `pop-release-2.0.3/pop_release.egg-info/SOURCES.txt` & `pop-release-2.0.4/pop_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-release-2.0.3/setup.py` & `pop-release-2.0.4/setup.py`

 * *Files identical despite different names*

