# Comparing `tmp/relative_dose_1d-0.1.6.tar.gz` & `tmp/relative_dose_1d-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.1.6.tar", last modified: Tue Jul 11 15:23:52 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.1.7.tar", last modified: Wed Aug  2 17:04:55 2023, max compression
```

## Comparing `relative_dose_1d-0.1.6.tar` & `relative_dose_1d-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/
--rw-rw-rw-   0        0        0     1108 2023-04-04 17:36:43.000000 relative_dose_1d-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     4831 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3743 2023-07-11 15:21:04.000000 relative_dose_1d-0.1.6/README.md
--rw-rw-rw-   0        0        0     1404 2023-07-11 15:20:51.000000 relative_dose_1d-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 15:23:52.759832 relative_dose_1d-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.666086 relative_dose_1d-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.712986 relative_dose_1d-0.1.6/src/relative_dose_1d/
--rw-rw-rw-   0        0        0     1410 2023-07-10 15:29:21.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0    13205 2023-07-11 15:18:58.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/GUI_tool.py
--rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/src/relative_dose_1d/test_data/
--rw-rw-rw-   0        0        0      341 2023-07-10 18:36:09.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/test_data/clean.py
--rw-rw-rw-   0        0        0    10639 2023-07-10 15:29:21.000000 relative_dose_1d-0.1.6/src/relative_dose_1d/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:23:52.744233 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     4831 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-11 15:23:52.000000 relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:55.018123 relative_dose_1d-0.1.7/
+-rw-rw-rw-   0        0        0     1108 2023-04-04 17:36:43.000000 relative_dose_1d-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4930 2023-08-02 17:04:55.018123 relative_dose_1d-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3842 2023-08-02 15:07:07.000000 relative_dose_1d-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1404 2023-08-02 15:05:27.000000 relative_dose_1d-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 17:04:55.018123 relative_dose_1d-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:54.924380 relative_dose_1d-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:54.971254 relative_dose_1d-0.1.7/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     1425 2023-08-02 17:01:16.000000 relative_dose_1d-0.1.7/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0    13554 2023-08-02 16:58:27.000000 relative_dose_1d-0.1.7/src/relative_dose_1d/GUI_tool.py
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 relative_dose_1d-0.1.7/src/relative_dose_1d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:55.002500 relative_dose_1d-0.1.7/src/relative_dose_1d/test_data/
+-rw-rw-rw-   0        0        0      341 2023-07-10 18:36:09.000000 relative_dose_1d-0.1.7/src/relative_dose_1d/test_data/clean.py
+-rw-rw-rw-   0        0        0    10639 2023-07-10 15:29:21.000000 relative_dose_1d-0.1.7/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:55.002500 relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     4930 2023-08-02 17:04:54.000000 relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-08-02 17:04:54.000000 relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 17:04:54.000000 relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-02 17:04:54.000000 relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 17:04:54.000000 relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.1.6/LICENSE` & `relative_dose_1d-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.6/PKG-INFO` & `relative_dose_1d-0.1.7/src/relative_dose_1d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: relative_dose_1d
-Version: 0.1.6
+Name: relative-dose-1d
+Version: 0.1.7
 Summary: Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
@@ -107,7 +107,10 @@
 
 Jul-2023 Version 0.1.4 - 0.1.6
 * Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
 * [New GUI_tool module](GUI_tool_module_label).
 * Now it is possible to change tolerance parameter for gamma evaluation.
 * Pass rate, total and evaluated points are now displayed on the GUI.
 * gamma_1d function returns the number of evaluated points.
+
+Aug-2023 Version 0.1.7
+* The plot function can be called outside relative_dose_1d application.
```

### Comparing `relative_dose_1d-0.1.6/README.md` & `relative_dose_1d-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -85,8 +85,11 @@
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
 
 Jul-2023 Version 0.1.4 - 0.1.6
 * Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
 * [New GUI_tool module](GUI_tool_module_label).
 * Now it is possible to change tolerance parameter for gamma evaluation.
 * Pass rate, total and evaluated points are now displayed on the GUI.
-* gamma_1d function returns the number of evaluated points.
+* gamma_1d function returns the number of evaluated points.
+
+Aug-2023 Version 0.1.7
+* The plot function can be called outside relative_dose_1d application.
```

### Comparing `relative_dose_1d-0.1.6/pyproject.toml` & `relative_dose_1d-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `relative_dose_1d-0.1.6/src/relative_dose_1d/GUI.py` & `relative_dose_1d-0.1.7/src/relative_dose_1d/GUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 import sys
 from PyQt6.QtWidgets import QApplication
 
 from relative_dose_1d.GUI_tool import GUI
       
 app = QApplication(sys.argv)
 window = GUI()
+window.show()
 sys.exit(app.exec())
```

### Comparing `relative_dose_1d-0.1.6/src/relative_dose_1d/GUI_tool.py` & `relative_dose_1d-0.1.7/src/relative_dose_1d/GUI_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qtagg import FigureCanvas
 from PyQt6.QtWidgets import (QApplication, QWidget, QLabel, QLineEdit, QHBoxLayout,
                              QPushButton, QMessageBox, QFileDialog, QVBoxLayout,
-                             QFormLayout, QInputDialog, QMainWindow)
-from PyQt6.QtCore import Qt
+                             QFormLayout, QInputDialog, QMainWindow, QDialog)
+from PyQt6.QtCore import Qt, QCoreApplication
 import numpy as np
 from relative_dose_1d.tools import identify_format, get_data, gamma_1D, build_from_array_and_step
 import sys
 import os
 import copy
 
-class GUI(QWidget):
+class GUI(QDialog):
 
-    def __init__(self, D_ref = None, D_eval = None):
+    def __init__(self, D_ref = None, D_eval = None, parent=None):
         """Constructor for a graphical user interface (GUI). Data has to be in 2 columns, 
         corresponding to positions and dose values, respectively.
 
         Parameters
         ----------
 
         D_ref : ndarray,
@@ -29,30 +29,29 @@
 
         Returns
         -------
 
         A PyQt widget to showing dose profiles, gamma analysis and dose difference.
 
         """
-        super().__init__()
+        super().__init__(parent=parent)
 
         self.D_ref = D_ref
         self.D_eval = D_eval
 
         self.initializeUI()
 
     def initializeUI(self):
         """Set up the apllication"""
         "x, y, width, height"
         self.setGeometry(200,100,1000,400)
         self.setWindowTitle("Relative dose 1D")
 
         self.set_up_window()
         self.set_up_data()
-        self.show()
 
     def set_up_window(self):
 
         "Layouts definition"
         self.main_box_layout = QHBoxLayout()
    
         self.v_box_layout = QVBoxLayout()
@@ -325,30 +324,37 @@
     -------
 
     A GUI showing dose profiles, gamma analysis and dose difference.
 
     Examples
     --------
 
-    >>> import relative_dose_1d.GUI_tool as rd
+    >>> from relative_dose_1d.GUI_tool import plot
+    >>> from relative_dose_1d.tools import build_from_array_and_step
+    >>> import numpy as np
 
     >>> a = np.array([0,1,2,3,4,5,6,7,8,9,10])
     >>> b = a + np.random.random_sample((11,))
 
     >>> A = build_from_array_and_step(a, 1)
     >>> B = build_from_array_and_step(b, 1)
     
-    >>> rd.plot(A,B)
+    >>> w = plot(A,B)
 
     """
-
-    app = QApplication(sys.argv)    
-    window = GUI(D_ref, D_eval)
-    sys.exit(app.exec())
-
+    
+    if not QCoreApplication.instance():
+        app = QApplication(sys.argv)
+        window = GUI(D_ref, D_eval)
+        window.show()
+        sys.exit(app.exec())
+    else:
+        """This condition is used when external applications call to plot function."""
+        return GUI(D_ref, D_eval)
+    
 def run_demo():
 
     a = np.array([0,1,2,3,4,5,6,7,8,9,10])
     b = a + np.random.random_sample((11,))
 
     A = build_from_array_and_step(a, 1)
     B = build_from_array_and_step(b, 1)
```

### Comparing `relative_dose_1d-0.1.6/src/relative_dose_1d/tools.py` & `relative_dose_1d-0.1.7/src/relative_dose_1d/tools.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.6/src/relative_dose_1d.egg-info/PKG-INFO` & `relative_dose_1d-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: relative-dose-1d
-Version: 0.1.6
+Name: relative_dose_1d
+Version: 0.1.7
 Summary: Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
@@ -107,7 +107,10 @@
 
 Jul-2023 Version 0.1.4 - 0.1.6
 * Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
 * [New GUI_tool module](GUI_tool_module_label).
 * Now it is possible to change tolerance parameter for gamma evaluation.
 * Pass rate, total and evaluated points are now displayed on the GUI.
 * gamma_1d function returns the number of evaluated points.
+
+Aug-2023 Version 0.1.7
+* The plot function can be called outside relative_dose_1d application.
```

