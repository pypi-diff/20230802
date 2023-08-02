# Comparing `tmp/pyjt-0.1.0a2.tar.gz` & `tmp/pyjt-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.1.0a2.tar", last modified: Wed Aug  2 13:46:53 2023, max compression
+gzip compressed data, was "pyjt-0.1.0a8.tar", last modified: Wed Aug  2 14:20:00 2023, max compression
```

## Comparing `pyjt-0.1.0a2.tar` & `pyjt-0.1.0a8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 13:46:53.000000 pyjt-0.1.0a2/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:46:53.527205 pyjt-0.1.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 13:46:24.000000 pyjt-0.1.0a2/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.939617 pyjt-0.1.0a8/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/tests/test_textfield.py
```

### Comparing `pyjt-0.1.0a2/LICENSE` & `pyjt-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/PKG-INFO` & `pyjt-0.1.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.1.0a2
+Version: 0.1.0a8
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjt-0.1.0a2/README.md` & `pyjt-0.1.0a8/README.md`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/pyjt/ComponentFinder.py` & `pyjt-0.1.0a8/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/pyjt/Fixture.py` & `pyjt-0.1.0a8/pyjt/Fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,14 @@
             -   FillMode.PASTE
                 -   Fill the control by pasting the text from the clipboard
                 -   **Not implemented yet**
         """
         if mode == FillMode.TYPE:
             self.click()
             if clear:
-                self._control.selectAll()
+                self.robot.selectAll()
             self.robot.type(text)
         if mode == FillMode.SET:
             self._control.setText(text)
 
     def __getattr__(self, name):
         return getattr(self._control, name)
```

### Comparing `pyjt-0.1.0a2/pyjt/Frame.py` & `pyjt-0.1.0a8/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/pyjt/Inspector.py` & `pyjt-0.1.0a8/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/pyjt/Proxy.py` & `pyjt-0.1.0a8/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/pyjt/Robot.py` & `pyjt-0.1.0a8/pyjt/Robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import time
 import logging
 
+from pyjt import Proxy
+
 log = logging.getLogger(__name__)
 
 
 class Robot:
     """ Smart robot features for controlling the application. """
     _robot = None
 
@@ -16,17 +18,17 @@
                             create a own instance of the robot class.
 
         :param typespeed:   The speed to type text in number of keystrokes per second.
         """
         import java
         from java.awt.event import KeyEvent
 
-        self._robot = robot if robot else Robot._robot
+        self._robot = Proxy(robot) if robot else Robot._robot
         if not self._robot:
-            Robot._robot = java.awt.Robot()
+            Robot._robot = Proxy(java.awt.Robot())
             self._robot = Robot._robot
 
         self._typespeed = typespeed
 
         self._KeyCodes = {
                 'a': [KeyEvent.VK_A],
                 'b': [KeyEvent.VK_B],
@@ -129,26 +131,30 @@
 
     def move(self, control):
         """ Move the mouse pointer to the position of a **control**.
 
             :param control: The control to move the mouse pointer to.
         """
         position = control.getLocationOnScreen()
-        self._robot.mouseMove(position.x, position.y)
+        self._robot.mouseMove(position.x + 2, position.y + 2)
 
     def click(self):
         """ Execute a click of the left mouse. """
         import java
-        log.debug("mousedown")
+        log.debug("ymousedown")
         self._robot.mousePress(java.awt.event.MouseEvent.BUTTON1_DOWN_MASK)
-        log.debug("sleeping for {1 / self._typespeed}")
+        log.debug(f"sleeping for {1 / self._typespeed}")
         time.sleep(1 / self._typespeed)
         log.debug("mouseup")
         self._robot.mouseRelease(java.awt.event.MouseEvent.BUTTON1_DOWN_MASK)
 
+    def selectAll(self):
+        from java.awt.event import KeyEvent
+        self._typeVKs([KeyEvent.VK_CONTROL, KeyEvent.VK_A])
+
     def type(self, text):
         """ Emulate user typing the given text.
 
             :param text:    Text to type.
 
             Typing is emulated by generating VK_* events. The type speed
             (delay between each keystroke) is configured in the
```

### Comparing `pyjt-0.1.0a2/pyjt/__init__.py` & `pyjt-0.1.0a8/pyjt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a2/pyjt.egg-info/PKG-INFO` & `pyjt-0.1.0a8/pyjt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.1.0a2
+Version: 0.1.0a8
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjt-0.1.0a2/pyproject.toml` & `pyjt-0.1.0a8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.1.0a2"
+version = "0.1.0a8"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

