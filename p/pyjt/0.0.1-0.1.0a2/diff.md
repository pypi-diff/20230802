# Comparing `tmp/pyjt-0.0.1.tar.gz` & `tmp/pyjt-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.0.1.tar", last modified: Wed Aug  2 10:53:13 2023, max compression
+gzip compressed data, was "pyjt-0.1.0a2.tar", last modified: Wed Aug  2 13:46:53 2023, max compression
```

## Comparing `pyjt-0.0.1.tar` & `pyjt-0.1.0a2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:53:13.558745 pyjt-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 10:52:41.000000 pyjt-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 10:53:13.558745 pyjt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-02 10:52:41.000000 pyjt-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:53:13.558745 pyjt-0.0.1/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:53:13.558745 pyjt-0.0.1/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 10:53:13.000000 pyjt-0.0.1/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-02 10:53:13.000000 pyjt-0.0.1/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:53:13.000000 pyjt-0.0.1/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 10:53:13.000000 pyjt-0.0.1/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 10:53:13.000000 pyjt-0.0.1/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 10:52:41.000000 pyjt-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 10:53:13.558745 pyjt-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:53:13.558745 pyjt-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-02 10:52:41.000000 pyjt-0.0.1/tests/test_framefinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/tests/test_textfield.py
```

### Comparing `pyjt-0.0.1/LICENSE` & `pyjt-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.0.1/PKG-INFO` & `pyjt-0.1.0a2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.0.1
+Version: 0.1.0a2
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,15 @@
 
     import pyjt
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
+    pyjt.start()
     pyjt.run("HelloWorld")
 
     # find the frame window titled "Hello World"
     frame = pyjt.FrameFinder.find(title="Hello World")
 
     # Locate and click a button on the frame
     frame.locate(JButton, text="Ok").click()
```

### Comparing `pyjt-0.0.1/README.md` & `pyjt-0.1.0a2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     import pyjt
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
+    pyjt.start()
     pyjt.run("HelloWorld")
 
     # find the frame window titled "Hello World"
     frame = pyjt.FrameFinder.find(title="Hello World")
 
     # Locate and click a button on the frame
     frame.locate(JButton, text="Ok").click()
```

### Comparing `pyjt-0.0.1/pyjt/ComponentFinder.py` & `pyjt-0.1.0a2/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.0.1/pyjt/Frame.py` & `pyjt-0.1.0a2/pyjt/Frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import logging
 
-from java.awt import Window
-from java.awt.event import WindowEvent
-
 from pyjt.Errors import ElementNotFoundError
 from pyjt.ComponentFinder import ComponentFinder, Locator
 from pyjt.Fixture import Fixture
 from pyjt.Inspector import Inspector
 from pyjt import Proxy
 
 log = logging.getLogger(__name__)
 
 
 class FrameFinder:
     @staticmethod
     def find(locator=None, **kwargs):
+        from java.awt import Window
         locator = locator if locator else Locator(**kwargs)
         wp = Proxy(Window)
         window = ComponentFinder.findIn(func=wp.getWindows, locator=locator)
         if not window:
             raise ElementNotFoundError(f"Window {kwargs} not found!")
         return Frame(window=window)
 
     @staticmethod
     def inspect():
+        from java.awt import Window
         wp = Proxy(Window)
         result = []
         for window in wp.getWindows():
             result.append(Inspector.inspect(window))
         return result
 
 
@@ -43,9 +42,13 @@
             raise ElementNotFoundError(f"Control({kwargs}) not found!")
         return Fixture(control)
 
     def locate(self, role, **kwargs):
         kwargs['role'] = role
         return self.find(**kwargs)
 
+    def dispose(self):
+        self._window.dispose()
+
     def close(self):
+        from java.awt.event import WindowEvent
         self._window.instance.dispatchEvent(WindowEvent(self._window.instance, WindowEvent.WINDOW_CLOSING))
```

### Comparing `pyjt-0.0.1/pyjt/Inspector.py` & `pyjt-0.1.0a2/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.0.1/pyjt.egg-info/PKG-INFO` & `pyjt-0.1.0a2/pyjt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.0.1
+Version: 0.1.0a2
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,15 @@
 
     import pyjt
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
+    pyjt.start()
     pyjt.run("HelloWorld")
 
     # find the frame window titled "Hello World"
     frame = pyjt.FrameFinder.find(title="Hello World")
 
     # Locate and click a button on the frame
     frame.locate(JButton, text="Ok").click()
```

### Comparing `pyjt-0.0.1/pyproject.toml` & `pyjt-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.0.1"
+version = "0.1.0a2"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

