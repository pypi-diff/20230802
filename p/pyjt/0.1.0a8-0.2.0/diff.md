# Comparing `tmp/pyjt-0.1.0a8.tar.gz` & `tmp/pyjt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.1.0a8.tar", last modified: Wed Aug  2 14:20:00 2023, max compression
+gzip compressed data, was "pyjt-0.2.0.tar", last modified: Wed Aug  2 14:50:36 2023, max compression
```

## Comparing `pyjt-0.1.0a8.tar` & `pyjt-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.939617 pyjt-0.1.0a8/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 14:20:00.000000 pyjt-0.1.0a8/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:20:00.943617 pyjt-0.1.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 14:19:11.000000 pyjt-0.1.0a8/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.896167 pyjt-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 14:49:48.000000 pyjt-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 14:50:36.896167 pyjt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 14:49:48.000000 pyjt-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.892167 pyjt-0.2.0/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.896167 pyjt-0.2.0/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 14:50:36.000000 pyjt-0.2.0/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 14:49:48.000000 pyjt-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:50:36.896167 pyjt-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.896167 pyjt-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 14:49:48.000000 pyjt-0.2.0/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 14:49:48.000000 pyjt-0.2.0/tests/test_textfield.py
```

### Comparing `pyjt-0.1.0a8/LICENSE` & `pyjt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a8/PKG-INFO` & `pyjt-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.1.0a8
+Version: 0.2.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,17 +30,22 @@
 
     import pyjt
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
-    pyjt.start()
+    pyjt.start(classpath="myapp/")
     pyjt.run("HelloWorld")
 
     # find the frame window titled "Hello World"
     frame = pyjt.FrameFinder.find(title="Hello World")
 
     # Locate and click a button on the frame
     frame.locate(JButton, text="Ok").click()
 
+    # Locate and fill text to an text field
+    frame.locate(JTextField, name="textfield1").fill("John Smith")
+
+    # Close the frame (application)
+    frame.close()
```

### Comparing `pyjt-0.1.0a8/README.md` & `pyjt-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,22 @@
 
     import pyjt
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
-    pyjt.start()
+    pyjt.start(classpath="myapp/")
     pyjt.run("HelloWorld")
 
     # find the frame window titled "Hello World"
     frame = pyjt.FrameFinder.find(title="Hello World")
 
     # Locate and click a button on the frame
     frame.locate(JButton, text="Ok").click()
 
+    # Locate and fill text to an text field
+    frame.locate(JTextField, name="textfield1").fill("John Smith")
+
+    # Close the frame (application)
+    frame.close()
```

### Comparing `pyjt-0.1.0a8/pyjt/ComponentFinder.py` & `pyjt-0.2.0/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a8/pyjt/Fixture.py` & `pyjt-0.2.0/pyjt/Fixture.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a8/pyjt/Frame.py` & `pyjt-0.2.0/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a8/pyjt/Inspector.py` & `pyjt-0.2.0/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a8/pyjt/Proxy.py` & `pyjt-0.2.0/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.1.0a8/pyjt/Robot.py` & `pyjt-0.2.0/pyjt/Robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,21 @@
         """
         position = control.getLocationOnScreen()
         self._robot.mouseMove(position.x + 2, position.y + 2)
 
     def click(self):
         """ Execute a click of the left mouse. """
         import java
-        log.debug("ymousedown")
-        self._robot.mousePress(java.awt.event.MouseEvent.BUTTON1_DOWN_MASK)
+        log.debug("zmousedown")
+        btn = java.awt.event.InputEvent.getMaskForButton(1)
+        self._robot.mousePress(btn)
         log.debug(f"sleeping for {1 / self._typespeed}")
         time.sleep(1 / self._typespeed)
         log.debug("mouseup")
-        self._robot.mouseRelease(java.awt.event.MouseEvent.BUTTON1_DOWN_MASK)
+        self._robot.mouseRelease(btn)
 
     def selectAll(self):
         from java.awt.event import KeyEvent
         self._typeVKs([KeyEvent.VK_CONTROL, KeyEvent.VK_A])
 
     def type(self, text):
         """ Emulate user typing the given text.
```

### Comparing `pyjt-0.1.0a8/pyjt.egg-info/PKG-INFO` & `pyjt-0.2.0/pyjt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.1.0a8
+Version: 0.2.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,17 +30,22 @@
 
     import pyjt
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
     # a hello world application located in HelloWorld.java
-    pyjt.start()
+    pyjt.start(classpath="myapp/")
     pyjt.run("HelloWorld")
 
     # find the frame window titled "Hello World"
     frame = pyjt.FrameFinder.find(title="Hello World")
 
     # Locate and click a button on the frame
     frame.locate(JButton, text="Ok").click()
 
+    # Locate and fill text to an text field
+    frame.locate(JTextField, name="textfield1").fill("John Smith")
+
+    # Close the frame (application)
+    frame.close()
```

### Comparing `pyjt-0.1.0a8/pyproject.toml` & `pyjt-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.1.0a8"
+version = "0.2.0"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

