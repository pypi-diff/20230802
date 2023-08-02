# Comparing `tmp/castor-orsay-2021.9.13.tar.gz` & `tmp/castor-orsay-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castor-orsay-2021.9.13.tar", last modified: Mon Sep 13 09:21:05 2021, max compression
+gzip compressed data, was "castor-orsay-2023.8.2.tar", last modified: Wed Aug  2 11:28:59 2023, max compression
```

## Comparing `castor-orsay-2021.9.13.tar` & `castor-orsay-2023.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 09:21:05.038454 castor-orsay-2021.9.13/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-09-13 09:21:05.034454 castor-orsay-2021.9.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      706 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 09:21:05.034454 castor-orsay-2021.9.13/castor/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 09:21:05.034454 castor-orsay-2021.9.13/castor/_console_scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1910 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/align.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2765 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/align_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22693 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/exoplanet_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7616 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/pointing_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2205 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/prepare.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3587 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/rotate_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2429 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/_console_scripts/wavelength_calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 09:21:05.034454 castor-orsay-2021.9.13/castor/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/data/instruments.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/files_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/mount_alignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/photometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/preparation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7512 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/castor/spectroscopy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 09:21:05.034454 castor-orsay-2021.9.13/castor_orsay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-09-13 09:21:04.000000 castor-orsay-2021.9.13/castor_orsay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      760 2021-09-13 09:21:04.000000 castor-orsay-2021.9.13/castor_orsay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-13 09:21:04.000000 castor-orsay-2021.9.13/castor_orsay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-09-13 09:21:04.000000 castor-orsay-2021.9.13/castor_orsay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-09-13 09:21:04.000000 castor-orsay-2021.9.13/castor_orsay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-13 09:21:04.000000 castor-orsay-2021.9.13/castor_orsay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-13 09:21:05.038454 castor-orsay-2021.9.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2021-09-13 09:20:56.000000 castor-orsay-2021.9.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.180082 castor-orsay-2023.8.2/castor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.180082 castor-orsay-2023.8.2/castor/_console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/align.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/align_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22987 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/exoplanet_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7616 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/pointing_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2205 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/prepare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3587 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/rotate_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2429 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/wavelength_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.180082 castor-orsay-2023.8.2/castor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/data/instruments.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/files_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/mount_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/spectroscopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/castor_orsay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/setup.py
```

### Comparing `castor-orsay-2021.9.13/LICENSE.txt` & `castor-orsay-2023.8.2/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020 Gabriel Pelouze
+Copyright (c) 2021 Gabriel Pelouze and Aurélien Stcherbinine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `castor-orsay-2021.9.13/PKG-INFO` & `castor-orsay-2023.8.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 Metadata-Version: 2.1
 Name: castor-orsay
-Version: 2021.9.13
+Version: 2023.8.2
 Summary: Codes pour l’ASTronomie à ORsay
 Home-page: https://github.com/coupole-orsay/castor
 Author: Gabriel Pelouze, Aurélien Stcherbinine
 Author-email: gabriel.pelouze@ias.u-psud.fr, aurelien.stcherbinine@ias.u-psud.fr
-License: UNKNOWN
-Description: # CASTOR: Codes pour l’ASTronomie à ORsay
-        
-        Outils pour l’analyse des données de la coupole d’Orsay.
-        
-        ## Documentation
-        
-        [Documentation pour les TP à la coupole (PDF)][doc-tp-pdf]
-        
-        [doc-tp-pdf]: https://github.com/coupole-orsay/castor/releases/latest/download/doc_TP_coupole.pdf
-        
-        ## Installation
-        
-        ### Option 1 : depuis PyPI (recommandé)
-        
-        Exécuter `pip3 install castor-orsay --user`.
-        
-        
-        ### Option 2 : depuis git (version de développement)
-        
-        Cloner (ou télécharger les sources) de ce dépôt, et l’installer avec pip :
-        
-        ~~~
-        git clone https://github.com/coupole-orsay/castor
-        cd castor
-        pip3 install . --user
-        ~~~
-        
-        ## Licence
-        
-        Ces outils sont mis à disposition sous licence MIT. Voir `LICENSE.txt`
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# CASTOR: Codes pour l’ASTronomie à ORsay
+
+Outils pour l’analyse des données de la coupole d’Orsay.
+
+## Documentation
+
+[Documentation pour les TP à la coupole (PDF)][doc-tp-pdf]
+
+[doc-tp-pdf]: https://github.com/coupole-orsay/castor/releases/latest/download/doc_TP_coupole.pdf
+
+## Installation
+
+### Version stable (depuis PyPI; recommandé)
+
+```bash
+mkdir castor && cd castor
+python3 -m venv venv
+source venv/bin/activate
+pip3 install castor-orsay
+```
+
+
+### Version de développement (depuis GitHub)
+
+```bash
+git clone https://github.com/coupole-orsay/castor
+cd castor
+python3 -m venv venv
+source venv/bin/activate
+pip3 install -e .
+```
+
+
+## Utilisation
+
+```bash
+cd castor
+source venv/bin/activate
+castor_<tab>
+```
+
+
+## Licence
+
+Ces outils sont mis à disposition sous licence MIT. Voir `LICENSE.txt`
```

### Comparing `castor-orsay-2021.9.13/castor/__init__.py` & `castor-orsay-2023.8.2/castor/__init__.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/align.py` & `castor-orsay-2023.8.2/castor/_console_scripts/align.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/align_spectra.py` & `castor-orsay-2023.8.2/castor/_console_scripts/align_spectra.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/exoplanet_analysis.py` & `castor-orsay-2023.8.2/castor/_console_scripts/exoplanet_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,38 +155,47 @@
         self.parent = parent
         self.is_active = False
         self.radius = radius
         self.annulus_radii = annulus_radii
         self.color_active = color_active
         self.color_inactive = color_inactive
 
+        self._circles_are_plotted = False
+
         self.circ = plt.Circle(
-            (None, None), self.radius,
+            (0, 0), self.radius,
             fill=False, color=self.color_inactive)
-        self.parent.im_ax.add_patch(self.circ)
 
         if self.annulus_radii is not None:
             inner_radius, outer_radius = self.annulus_radii
             inner_circ = plt.Circle(
-                (None, None), inner_radius,
+                (0, 0), inner_radius,
                 fill=False, color=self.color_inactive)
             outer_circ = plt.Circle(
-                (None, None), outer_radius,
+                (0, 0), outer_radius,
                 fill=False, color=self.color_inactive)
-            self.parent.im_ax.add_patch(inner_circ)
-            self.parent.im_ax.add_patch(outer_circ)
             self.annulus_circs = (inner_circ, outer_circ)
         else:
             self.annulus_circs = None
 
+    def _plot_circles_if_needed(self):
+        if not self._circles_are_plotted:
+            self.parent.im_ax.add_patch(self.circ)
+            if self.annulus_circs is not None:
+                for circ in self.annulus_circs:
+                    self.parent.im_ax.add_patch(circ)
+                    self.parent.im_ax.add_patch(circ)
+            self._circles_are_plotted = True
+
     def set_coordinates(self, x, y):
         self.circ.center = x, y
         if self.annulus_circs is not None:
             for circ in self.annulus_circs:
                 circ.center = x, y
+        self._plot_circles_if_needed()
         self.parent.fig.canvas.draw()
 
     def get_coordinates(self):
         return self.circ.center
 
     def circ_contains(self, event):
         return self.circ.contains(event)[0]
```

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/pointing_analysis.py` & `castor-orsay-2023.8.2/castor/_console_scripts/pointing_analysis.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/prepare.py` & `castor-orsay-2023.8.2/castor/_console_scripts/prepare.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/rotate_spectra.py` & `castor-orsay-2023.8.2/castor/_console_scripts/rotate_spectra.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/_console_scripts/wavelength_calibration.py` & `castor-orsay-2023.8.2/castor/_console_scripts/wavelength_calibration.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/alignment.py` & `castor-orsay-2023.8.2/castor/alignment.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/data/instruments.yml` & `castor-orsay-2023.8.2/castor/data/instruments.yml`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/files_handling.py` & `castor-orsay-2023.8.2/castor/files_handling.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/mount_alignment.py` & `castor-orsay-2023.8.2/castor/mount_alignment.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/photometry.py` & `castor-orsay-2023.8.2/castor/photometry.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/preparation.py` & `castor-orsay-2023.8.2/castor/preparation.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor/spectroscopy.py` & `castor-orsay-2023.8.2/castor/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/castor_orsay.egg-info/PKG-INFO` & `castor-orsay-2023.8.2/castor_orsay.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 Metadata-Version: 2.1
 Name: castor-orsay
-Version: 2021.9.13
+Version: 2023.8.2
 Summary: Codes pour l’ASTronomie à ORsay
 Home-page: https://github.com/coupole-orsay/castor
 Author: Gabriel Pelouze, Aurélien Stcherbinine
 Author-email: gabriel.pelouze@ias.u-psud.fr, aurelien.stcherbinine@ias.u-psud.fr
-License: UNKNOWN
-Description: # CASTOR: Codes pour l’ASTronomie à ORsay
-        
-        Outils pour l’analyse des données de la coupole d’Orsay.
-        
-        ## Documentation
-        
-        [Documentation pour les TP à la coupole (PDF)][doc-tp-pdf]
-        
-        [doc-tp-pdf]: https://github.com/coupole-orsay/castor/releases/latest/download/doc_TP_coupole.pdf
-        
-        ## Installation
-        
-        ### Option 1 : depuis PyPI (recommandé)
-        
-        Exécuter `pip3 install castor-orsay --user`.
-        
-        
-        ### Option 2 : depuis git (version de développement)
-        
-        Cloner (ou télécharger les sources) de ce dépôt, et l’installer avec pip :
-        
-        ~~~
-        git clone https://github.com/coupole-orsay/castor
-        cd castor
-        pip3 install . --user
-        ~~~
-        
-        ## Licence
-        
-        Ces outils sont mis à disposition sous licence MIT. Voir `LICENSE.txt`
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# CASTOR: Codes pour l’ASTronomie à ORsay
+
+Outils pour l’analyse des données de la coupole d’Orsay.
+
+## Documentation
+
+[Documentation pour les TP à la coupole (PDF)][doc-tp-pdf]
+
+[doc-tp-pdf]: https://github.com/coupole-orsay/castor/releases/latest/download/doc_TP_coupole.pdf
+
+## Installation
+
+### Version stable (depuis PyPI; recommandé)
+
+```bash
+mkdir castor && cd castor
+python3 -m venv venv
+source venv/bin/activate
+pip3 install castor-orsay
+```
+
+
+### Version de développement (depuis GitHub)
+
+```bash
+git clone https://github.com/coupole-orsay/castor
+cd castor
+python3 -m venv venv
+source venv/bin/activate
+pip3 install -e .
+```
+
+
+## Utilisation
+
+```bash
+cd castor
+source venv/bin/activate
+castor_<tab>
+```
+
+
+## Licence
+
+Ces outils sont mis à disposition sous licence MIT. Voir `LICENSE.txt`
```

### Comparing `castor-orsay-2021.9.13/castor_orsay.egg-info/SOURCES.txt` & `castor-orsay-2023.8.2/castor_orsay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `castor-orsay-2021.9.13/setup.py` & `castor-orsay-2023.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 package_data = {
     '': ['data/*'],
     }
 
 setuptools.setup(
     name='castor-orsay',
-    version='2021.9.13',
+    version='2023.8.2',
     author='Gabriel Pelouze, Aurélien Stcherbinine',
     author_email='gabriel.pelouze@ias.u-psud.fr, aurelien.stcherbinine@ias.u-psud.fr',
     description='Codes pour l’ASTronomie à ORsay',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/coupole-orsay/castor',
     packages=setuptools.find_packages(),
```

