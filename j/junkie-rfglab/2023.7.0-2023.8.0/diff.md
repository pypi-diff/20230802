# Comparing `tmp/junkie-rfglab-2023.7.0.tar.gz` & `tmp/junkie-rfglab-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junkie-rfglab-2023.7.0.tar", last modified: Tue Jul  4 21:39:06 2023, max compression
+gzip compressed data, was "junkie-rfglab-2023.8.0.tar", last modified: Wed Aug  2 16:38:43 2023, max compression
```

## Comparing `junkie-rfglab-2023.7.0.tar` & `junkie-rfglab-2023.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-04 21:39:06.943050 junkie-rfglab-2023.7.0/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.7.0/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     3807 2023-07-04 21:39:06.942928 junkie-rfglab-2023.7.0/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     3219 2023-06-25 21:38:24.000000 junkie-rfglab-2023.7.0/README.md
--rw-r--r--   0 rodrigo    (501) staff       (20)    12080 2023-07-03 21:16:59.000000 junkie-rfglab-2023.7.0/junkie.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-04 21:39:06.942783 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     3807 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-06-12 01:43:28.000000 junkie-rfglab-2023.7.0/pyproject.toml
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-07-04 21:39:06.943085 junkie-rfglab-2023.7.0/setup.cfg
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-02 16:38:43.120543 junkie-rfglab-2023.8.0/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.8.0/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4139 2023-08-02 16:38:43.120423 junkie-rfglab-2023.8.0/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3551 2023-08-02 16:06:24.000000 junkie-rfglab-2023.8.0/README.md
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12106 2023-08-02 16:07:57.000000 junkie-rfglab-2023.8.0/junkie.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-02 16:38:43.120279 junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4139 2023-08-02 16:38:43.000000 junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-08-02 16:38:43.000000 junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-08-02 16:38:43.000000 junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-08-02 16:38:43.000000 junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-08-02 16:38:43.000000 junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-08-02 16:25:55.000000 junkie-rfglab-2023.8.0/pyproject.toml
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-08-02 16:38:43.120575 junkie-rfglab-2023.8.0/setup.cfg
```

### Comparing `junkie-rfglab-2023.7.0/LICENSE` & `junkie-rfglab-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.7.0/PKG-INFO` & `junkie-rfglab-2023.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.7.0
+Version: 2023.8.0
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
 %matplotlib widgets
 
 from junkie import junkie
 ```
 
 ![Importing JuNkIE](./docs/import_junkie.gif)
 
-There are a couple of ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
+There are a few ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
 ![Opening an ndarray](./docs/open_ndarray.gif)
 
 - You can also specifiy the path to the image that you want to open:
 
@@ -69,14 +69,20 @@
 
 ![Figure size](./docs/figsize.gif)
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a new one with additional functionality:
 
 ![Toolbar](./docs/toolbar.gif)
 
+## [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) today
+
+As we develop and improve [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), there may be small changes to the user interface. This is how [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) looks as of today:
+
+![JuNkIE today](./docs/junkie_today.gif)
+
 ## Citing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 If you use [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), please cite this repository. We are working on the paper!
 
 ## Sponsors
 
 We are grateful for the generous support from the following agencies and institutions, which contribute to the
```

### Comparing `junkie-rfglab-2023.7.0/README.md` & `junkie-rfglab-2023.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 %matplotlib widgets
 
 from junkie import junkie
 ```
 
 ![Importing JuNkIE](./docs/import_junkie.gif)
 
-There are a couple of ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
+There are a few ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
 ![Opening an ndarray](./docs/open_ndarray.gif)
 
 - You can also specifiy the path to the image that you want to open:
 
@@ -55,14 +55,20 @@
 
 ![Figure size](./docs/figsize.gif)
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a new one with additional functionality:
 
 ![Toolbar](./docs/toolbar.gif)
 
+## [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) today
+
+As we develop and improve [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), there may be small changes to the user interface. This is how [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) looks as of today:
+
+![JuNkIE today](./docs/junkie_today.gif)
+
 ## Citing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 If you use [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), please cite this repository. We are working on the paper!
 
 ## Sponsors
 
 We are grateful for the generous support from the following agencies and institutions, which contribute to the
```

### Comparing `junkie-rfglab-2023.7.0/junkie.py` & `junkie-rfglab-2023.8.0/junkie.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import skimage
 import IPython.display as IPyd
 import ipywidgets as ipyw
 import matplotlib.pyplot as plt
 
-__version__: str = '2023.7.0'  # this must be here for pyproject.toml to find it.
+__version__: str = '2023.8.0'  # this must be here for pyproject.toml to find it.
 
 
 # You will need this line in your jupyter notebook: %matplotlib widget
 
 class junkie:
     """ 
     junkie: a JUpyter NotebooK Image Explorer
@@ -155,15 +155,15 @@
             description='maximum pixel value:', style={'description_width': 'auto'})
         self._vmax_slider.value = self.pix_val_min_max[1]
         self._vmax_slider.observe(self._vmax_slider_change, 'value')
 
         self._autocontrast_button = ipyw.Button(description='auto', layout=junkie.button_layout, style=junkie.button_style, tooltip='auto contrast')
         self._autocontrast_button.on_click(self._autocontrast_button_click)
 
-        self.new_toolbar = ipyw.VBox([self._channel_slider, self._t_slider, self._plane_selection, self._Z_slider, ipyw.HBox([self._vmin_slider, self._autocontrast_button, self._vmax_slider]), ipyw.HBox([self._axes_button, self._invert_button, self._continuousupdate_button])])
+        self.new_toolbar = ipyw.VBox([ipyw.HBox([ipyw.VBox([self._channel_slider, self._t_slider, self._Z_slider]), self._plane_selection, ipyw.VBox([self._vmin_slider, self._vmax_slider, self._autocontrast_button])]), ipyw.HBox([self._axes_button, self._invert_button, self._continuousupdate_button])])
 
         IPyd.display(self.new_toolbar)
 
     # Enables/disables UI components.
     def _setupUI(self):
         self._channel_slider.disabled = False if self.volume.shape[0] > 1 else True
         self._t_slider.disabled = False if self.volume.shape[1] > 1 else True
```

### Comparing `junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/PKG-INFO` & `junkie-rfglab-2023.8.0/junkie_rfglab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.7.0
+Version: 2023.8.0
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
 %matplotlib widgets
 
 from junkie import junkie
 ```
 
 ![Importing JuNkIE](./docs/import_junkie.gif)
 
-There are a couple of ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
+There are a few ways to open an image with [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/):
 
 - You can open an image with some other package (e.g. scikit-image, opencv, PIL, etc.) and invoke [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) with a [numpy ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) as the parameter:
 
 ![Opening an ndarray](./docs/open_ndarray.gif)
 
 - You can also specifiy the path to the image that you want to open:
 
@@ -69,14 +69,20 @@
 
 ![Figure size](./docs/figsize.gif)
 
 [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) provides access to the standard [matplotlib](https://matplotlib.org/) toolbar, and also includes a new one with additional functionality:
 
 ![Toolbar](./docs/toolbar.gif)
 
+## [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) today
+
+As we develop and improve [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), there may be small changes to the user interface. This is how [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) looks as of today:
+
+![JuNkIE today](./docs/junkie_today.gif)
+
 ## Citing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 If you use [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), please cite this repository. We are working on the paper!
 
 ## Sponsors
 
 We are grateful for the generous support from the following agencies and institutions, which contribute to the
```

### Comparing `junkie-rfglab-2023.7.0/pyproject.toml` & `junkie-rfglab-2023.8.0/pyproject.toml`

 * *Files identical despite different names*

