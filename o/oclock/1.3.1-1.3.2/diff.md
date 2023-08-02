# Comparing `tmp/oclock-1.3.1.tar.gz` & `tmp/oclock-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oclock-1.3.1.tar", last modified: Wed Aug  2 08:50:28 2023, max compression
+gzip compressed data, was "oclock-1.3.2.tar", last modified: Wed Aug  2 09:57:06 2023, max compression
```

## Comparing `oclock-1.3.1.tar` & `oclock-1.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.867336 oclock-1.3.1/
--rw-r--r--   0 olivier.vincent   (502) staff       (20)       69 2023-08-02 07:21:25.000000 oclock-1.3.1/.gitignore
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     4004 2023-08-02 07:21:25.000000 oclock-1.3.1/AccuracyTests.md
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    90676 2023-08-02 08:37:25.000000 oclock-1.3.1/Examples.ipynb
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    35149 2023-08-02 07:21:25.000000 oclock-1.3.1/LICENSE
--rw-r--r--   0 olivier.vincent   (502) staff       (20)       97 2023-08-02 07:21:25.000000 oclock-1.3.1/MANIFEST.in
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    16603 2023-08-02 08:50:28.867416 oclock-1.3.1/PKG-INFO
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    15691 2023-08-02 08:46:47.000000 oclock-1.3.1/README.md
--rw-r--r--   0 olivier.vincent   (502) staff       (20)      450 2023-08-02 07:21:25.000000 oclock-1.3.1/example.py
-drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.861307 oclock-1.3.1/media/
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    53154 2023-08-02 07:21:25.000000 oclock-1.3.1/media/countdown.gif
-drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.865136 oclock-1.3.1/media/img/
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    34866 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_1000ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    34131 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_100ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    35454 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_10ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    38781 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_1ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    36275 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_40ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    23765 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_1000ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    30214 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_100ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    30779 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_10ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    26842 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_1ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    32829 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_40ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    69846 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/ribosome.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    37413 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_interval_exceeded.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    36134 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_1000ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    36719 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_100ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    39398 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_10ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    57825 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_1ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    40345 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_40ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    33693 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_1000ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    51059 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_100ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    55678 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_10ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    33242 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_1ms.png
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    55281 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_40ms.png
-drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.866356 oclock-1.3.1/oclock/
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     1291 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/__init__.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     1394 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/__main__.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     4260 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/countdown.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     4974 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/event.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     3443 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/general.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     4480 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/loop.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     3992 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/performance.py
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     7288 2023-08-02 08:21:04.000000 oclock-1.3.1/oclock/timer.py
-drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.867106 oclock-1.3.1/oclock.egg-info/
--rw-r--r--   0 olivier.vincent   (502) staff       (20)    16603 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/PKG-INFO
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     1216 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/SOURCES.txt
--rw-r--r--   0 olivier.vincent   (502) staff       (20)        1 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/dependency_links.txt
--rw-r--r--   0 olivier.vincent   (502) staff       (20)       19 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/requires.txt
--rw-r--r--   0 olivier.vincent   (502) staff       (20)        7 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/top_level.txt
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     1039 2023-08-02 08:50:28.867722 oclock-1.3.1/setup.cfg
--rw-r--r--   0 olivier.vincent   (502) staff       (20)       89 2023-08-02 07:21:25.000000 oclock-1.3.1/setup.py
-drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.867241 oclock-1.3.1/tests/
--rw-r--r--   0 olivier.vincent   (502) staff       (20)     2512 2023-08-02 07:21:25.000000 oclock-1.3.1/tests/test_oclock.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 09:57:06.998694 oclock-1.3.2/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       69 2023-08-02 07:21:25.000000 oclock-1.3.2/.gitignore
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4004 2023-08-02 07:21:25.000000 oclock-1.3.2/AccuracyTests.md
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    90676 2023-08-02 08:37:25.000000 oclock-1.3.2/Examples.ipynb
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    35149 2023-08-02 07:21:25.000000 oclock-1.3.2/LICENSE
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       97 2023-08-02 07:21:25.000000 oclock-1.3.2/MANIFEST.in
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    16603 2023-08-02 09:57:06.998777 oclock-1.3.2/PKG-INFO
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    15691 2023-08-02 08:52:08.000000 oclock-1.3.2/README.md
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)      450 2023-08-02 07:21:25.000000 oclock-1.3.2/example.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 09:57:06.992317 oclock-1.3.2/media/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    53154 2023-08-02 07:21:25.000000 oclock-1.3.2/media/countdown.gif
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 09:57:06.996389 oclock-1.3.2/media/img/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    34866 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_macos_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    34131 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_macos_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    35454 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_macos_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    38781 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_macos_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    36275 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_macos_40ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    23765 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_windows_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    30214 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_windows_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    30779 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_windows_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    26842 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_windows_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    32829 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/precisetimer_windows_40ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    69846 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/ribosome.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    37413 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_interval_exceeded.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    36134 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_macos_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    36719 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_macos_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    39398 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_macos_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    57825 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_macos_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    40345 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_macos_40ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    33693 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_windows_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    51059 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_windows_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    55678 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_windows_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    33242 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_windows_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    55281 2023-08-02 07:21:25.000000 oclock-1.3.2/media/img/timer_windows_40ms.png
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 09:57:06.997627 oclock-1.3.2/oclock/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1291 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/__init__.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1394 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/__main__.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4260 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/countdown.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4974 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/event.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     3443 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/general.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4480 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/loop.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     3992 2023-08-02 07:21:25.000000 oclock-1.3.2/oclock/performance.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     7295 2023-08-02 09:50:20.000000 oclock-1.3.2/oclock/timer.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 09:57:06.998405 oclock-1.3.2/oclock.egg-info/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    16603 2023-08-02 09:57:06.000000 oclock-1.3.2/oclock.egg-info/PKG-INFO
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1216 2023-08-02 09:57:06.000000 oclock-1.3.2/oclock.egg-info/SOURCES.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)        1 2023-08-02 09:57:06.000000 oclock-1.3.2/oclock.egg-info/dependency_links.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       19 2023-08-02 09:57:06.000000 oclock-1.3.2/oclock.egg-info/requires.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)        7 2023-08-02 09:57:06.000000 oclock-1.3.2/oclock.egg-info/top_level.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1039 2023-08-02 09:57:06.999086 oclock-1.3.2/setup.cfg
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       89 2023-08-02 07:21:25.000000 oclock-1.3.2/setup.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 09:57:06.998567 oclock-1.3.2/tests/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     2512 2023-08-02 07:21:25.000000 oclock-1.3.2/tests/test_oclock.py
```

### Comparing `oclock-1.3.1/AccuracyTests.md` & `oclock-1.3.2/AccuracyTests.md`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/Examples.ipynb` & `oclock-1.3.2/Examples.ipynb`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/LICENSE` & `oclock-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/PKG-INFO` & `oclock-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oclock
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for timed, no-drift loops of constant duration, and other misc. timing tools (GUI countdown, context managers etc.)
 Home-page: https://github.com/ovinc/oclock
 Author: Olivier Vincent
 Author-email: ovinc.py@gmail.com
 License: GNU GPLv3
 Keywords: timing,loops,constant duration,cancellable,modifiable,countdown,context manager,gui
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oclock-1.3.1/README.md` & `oclock-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/countdown.gif` & `oclock-1.3.2/media/countdown.gif`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_macos_1000ms.png` & `oclock-1.3.2/media/img/precisetimer_macos_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_macos_100ms.png` & `oclock-1.3.2/media/img/precisetimer_macos_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_macos_10ms.png` & `oclock-1.3.2/media/img/precisetimer_macos_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_macos_1ms.png` & `oclock-1.3.2/media/img/precisetimer_macos_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_macos_40ms.png` & `oclock-1.3.2/media/img/precisetimer_macos_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_windows_1000ms.png` & `oclock-1.3.2/media/img/precisetimer_windows_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_windows_100ms.png` & `oclock-1.3.2/media/img/precisetimer_windows_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_windows_10ms.png` & `oclock-1.3.2/media/img/precisetimer_windows_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_windows_1ms.png` & `oclock-1.3.2/media/img/precisetimer_windows_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/precisetimer_windows_40ms.png` & `oclock-1.3.2/media/img/precisetimer_windows_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/ribosome.png` & `oclock-1.3.2/media/img/ribosome.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_interval_exceeded.png` & `oclock-1.3.2/media/img/timer_interval_exceeded.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_macos_1000ms.png` & `oclock-1.3.2/media/img/timer_macos_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_macos_100ms.png` & `oclock-1.3.2/media/img/timer_macos_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_macos_10ms.png` & `oclock-1.3.2/media/img/timer_macos_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_macos_1ms.png` & `oclock-1.3.2/media/img/timer_macos_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_macos_40ms.png` & `oclock-1.3.2/media/img/timer_macos_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_windows_1000ms.png` & `oclock-1.3.2/media/img/timer_windows_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_windows_100ms.png` & `oclock-1.3.2/media/img/timer_windows_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_windows_10ms.png` & `oclock-1.3.2/media/img/timer_windows_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_windows_1ms.png` & `oclock-1.3.2/media/img/timer_windows_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/media/img/timer_windows_40ms.png` & `oclock-1.3.2/media/img/timer_windows_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/__init__.py` & `oclock-1.3.2/oclock/__init__.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/__main__.py` & `oclock-1.3.2/oclock/__main__.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/countdown.py` & `oclock-1.3.2/oclock/countdown.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/event.py` & `oclock-1.3.2/oclock/event.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/general.py` & `oclock-1.3.2/oclock/general.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/loop.py` & `oclock-1.3.2/oclock/loop.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/performance.py` & `oclock-1.3.2/oclock/performance.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/oclock/timer.py` & `oclock-1.3.2/oclock/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     def interval(self):
         """Interval property: time interval of the Timer object."""
         return self._interval
 
     @interval.setter
     def interval(self, value):
         """Modify existing interval to a new value, effective immediately."""
-        self.set_interval(immediate=True)
+        self.set_interval(value, immediate=True)
 
     def set_interval(self, value, immediate=True):
         """Choose if interval change is effective immediately or at next checkpt"""
         if value < 0:
             raise ValueError('Timer interval must be positive')
         self._interval = value
         if immediate:
```

### Comparing `oclock-1.3.1/oclock.egg-info/PKG-INFO` & `oclock-1.3.2/oclock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oclock
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for timed, no-drift loops of constant duration, and other misc. timing tools (GUI countdown, context managers etc.)
 Home-page: https://github.com/ovinc/oclock
 Author: Olivier Vincent
 Author-email: ovinc.py@gmail.com
 License: GNU GPLv3
 Keywords: timing,loops,constant duration,cancellable,modifiable,countdown,context manager,gui
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oclock-1.3.1/oclock.egg-info/SOURCES.txt` & `oclock-1.3.2/oclock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/setup.cfg` & `oclock-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oclock-1.3.1/tests/test_oclock.py` & `oclock-1.3.2/tests/test_oclock.py`

 * *Files identical despite different names*

