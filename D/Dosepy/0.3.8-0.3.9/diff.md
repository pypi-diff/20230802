# Comparing `tmp/Dosepy-0.3.8.tar.gz` & `tmp/Dosepy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dosepy-0.3.8.tar", last modified: Fri May 12 19:34:21 2023, max compression
+gzip compressed data, was "Dosepy-0.3.9.tar", last modified: Tue Jul 11 17:45:40 2023, max compression
```

## Comparing `Dosepy-0.3.8.tar` & `Dosepy-0.3.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.388389 Dosepy-0.3.8/
--rw-rw-rw-   0        0        0     1282 2023-04-12 01:58:35.000000 Dosepy-0.3.8/LICENSE
--rw-rw-rw-   0        0        0       41 2023-04-12 01:58:35.000000 Dosepy-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0    20293 2023-05-12 19:34:21.383038 Dosepy-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    19326 2023-05-12 17:10:17.000000 Dosepy-0.3.8/README.md
--rw-rw-rw-   0        0        0     1351 2023-05-05 15:39:39.000000 Dosepy-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 19:34:21.388389 Dosepy-0.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.115375 Dosepy-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.179376 Dosepy-0.3.8/src/Dosepy/
--rw-rw-rw-   0        0        0    11421 2023-04-30 04:28:56.000000 Dosepy-0.3.8/src/Dosepy/GUI.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.265033 Dosepy-0.3.8/src/Dosepy/GUILayouts/
--rw-rw-rw-   0        0        0    14426 2023-04-30 04:28:56.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/Bloque_Imagenes.py
--rw-rw-rw-   0        0        0    11425 2023-04-30 04:28:56.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/Bloque_gamma.py
--rw-rw-rw-   0        0        0        0 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/__init__.py
--rw-rw-rw-   0        0        0     3093 2023-04-30 04:28:56.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/about_window.py
--rw-rw-rw-   0        0        0     3457 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/cross_hair_cursor.py
--rw-rw-rw-   0        0        0      447 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/cursor.py
--rw-rw-rw-   0        0        0    15880 2023-05-12 01:35:14.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/film_to_doseGUI.py
--rw-rw-rw-   0        0        0     4655 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/licencia_window.py
--rw-rw-rw-   0        0        0     4921 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/GUILayouts/to_do_rendering.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.285795 Dosepy-0.3.8/src/Dosepy/Icon/
--rw-rw-rw-   0        0        0   568371 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/Icon/Icon.png
--rw-rw-rw-   0        0        0    14061 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/Icon/Logo_Dosepy.png
--rw-rw-rw-   0        0        0    11084 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/Icon/folder.png
--rw-rw-rw-   0        0        0     5824 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/Icon/save.png
--rw-rw-rw-   0        0        0        0 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.325686 Dosepy-0.3.8/src/Dosepy/data/
--rw-rw-rw-   0        0        0   380730 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/data/D_FILM.csv
--rw-rw-rw-   0        0        0   380730 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/data/D_TPS.csv
--rw-rw-rw-   0        0        0    15468 2023-05-12 19:33:20.000000 Dosepy-0.3.8/src/Dosepy/dose.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.379032 Dosepy-0.3.8/src/Dosepy/tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 01:58:37.000000 Dosepy-0.3.8/src/Dosepy/tools/__init__.py
--rw-rw-rw-   0        0        0     4433 2023-05-12 18:24:06.000000 Dosepy-0.3.8/src/Dosepy/tools/film_to_dose.py
--rw-rw-rw-   0        0        0     4330 2023-05-06 01:38:19.000000 Dosepy-0.3.8/src/Dosepy/tools/resol.py
-drwxrwxrwx   0        0        0        0 2023-05-12 19:34:21.209263 Dosepy-0.3.8/src/Dosepy.egg-info/
--rw-rw-rw-   0        0        0    20293 2023-05-12 19:34:21.000000 Dosepy-0.3.8/src/Dosepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      872 2023-05-12 19:34:21.000000 Dosepy-0.3.8/src/Dosepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 19:34:21.000000 Dosepy-0.3.8/src/Dosepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-12 19:34:21.000000 Dosepy-0.3.8/src/Dosepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 19:34:21.000000 Dosepy-0.3.8/src/Dosepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.540393 Dosepy-0.3.9/
+-rw-rw-rw-   0        0        0     1108 2023-07-11 16:51:08.000000 Dosepy-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0       41 2022-11-01 02:03:00.000000 Dosepy-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    20387 2023-07-11 17:45:40.533392 Dosepy-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    19411 2023-07-11 16:51:08.000000 Dosepy-0.3.9/README.md
+-rw-rw-rw-   0        0        0     1392 2023-07-11 17:44:51.000000 Dosepy-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 17:45:40.541372 Dosepy-0.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.243015 Dosepy-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.271999 Dosepy-0.3.9/src/Dosepy/
+-rw-rw-rw-   0        0        0    13915 2023-07-11 17:41:58.000000 Dosepy-0.3.9/src/Dosepy/GUI.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.334963 Dosepy-0.3.9/src/Dosepy/GUILayouts/
+-rw-rw-rw-   0        0        0    14523 2023-07-11 17:43:28.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/Bloque_Imagenes.py
+-rw-rw-rw-   0        0        0    11479 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/Bloque_gamma.py
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/__init__.py
+-rw-rw-rw-   0        0        0     3149 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/about_window.py
+-rw-rw-rw-   0        0        0     3457 2022-11-12 15:41:30.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/cross_hair_cursor.py
+-rw-rw-rw-   0        0        0      447 2022-11-12 17:56:22.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/cursor.py
+-rw-rw-rw-   0        0        0    15957 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/film_to_doseGUI.py
+-rw-rw-rw-   0        0        0     4711 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/licencia_window.py
+-rw-rw-rw-   0        0        0     4921 2022-11-14 00:38:07.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/to_do_rendering.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.351953 Dosepy-0.3.9/src/Dosepy/Icon/
+-rw-rw-rw-   0        0        0   568371 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/Icon.png
+-rw-rw-rw-   0        0        0    14061 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/Logo_Dosepy.png
+-rw-rw-rw-   0        0        0    11084 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/folder.png
+-rw-rw-rw-   0        0        0     5824 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/save.png
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.441902 Dosepy-0.3.9/src/Dosepy/data/
+-rw-rw-rw-   0        0        0   380730 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/data/D_FILM.csv
+-rw-rw-rw-   0        0        0   380730 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/data/D_TPS.csv
+-rw-rw-rw-   0        0        0    15468 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/dose.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.524410 Dosepy-0.3.9/src/Dosepy/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/tools/__init__.py
+-rw-rw-rw-   0        0        0     4433 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/tools/film_to_dose.py
+-rw-rw-rw-   0        0        0     4330 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/tools/resol.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.292987 Dosepy-0.3.9/src/Dosepy.egg-info/
+-rw-rw-rw-   0        0        0    20387 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      872 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/top_level.txt
```

### Comparing `Dosepy-0.3.8/PKG-INFO` & `Dosepy-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Dosepy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Gamma analysis and film dosimetry for dose distributions in radiotherapy
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
-Project-URL: homepage, https://luisolivaresj.github.io/Dosepy/
+Project-URL: homepage, https://dosepy.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://pypi.org/project/Dosepy/
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/Dosepy
 Keywords: Radiotherapy,Dose distribution,gamma index,python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -17,14 +17,16 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *Dosepy*
 
+[ReadTheDocs Documentation](https://dosepy.readthedocs.io/en/latest/intro.html)
+
 *Dosepy* es un paquete de código escrito en Python para la comparación mediante índice gamma de dos distribuciones de dosis, 2-dimensional. Adicionalmente, se cuenta con una herramienta para realizar dosimetría con película radiocrómica.<br/>
 
 El formato de los archivos que contengan la distribución de dosis puede ser DICOM (.dmc) o CVS. Para la película se requiere un formato TIFF.<br/>
 
 > **Condiciones de uso.** Toda persona tiene acceso a la lectura y uso del código con fines académicos o de enseñanza. Sin embargo, para el uso clínico del programa se requiere contar con una licencia (disponible próximamente), conocida como “Acuerdo de licencia de usuario final” (EULA, por sus siglas en inglés), así como contratos que garanticen el cumplimiento de la legislación de cada país.<br/>  
 
 Para mayor información contactar al correo electrónico dosepy@gmail.com.
```

### Comparing `Dosepy-0.3.8/README.md` & `Dosepy-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # *Dosepy*
 
+[ReadTheDocs Documentation](https://dosepy.readthedocs.io/en/latest/intro.html)
+
 *Dosepy* es un paquete de código escrito en Python para la comparación mediante índice gamma de dos distribuciones de dosis, 2-dimensional. Adicionalmente, se cuenta con una herramienta para realizar dosimetría con película radiocrómica.<br/>
 
 El formato de los archivos que contengan la distribución de dosis puede ser DICOM (.dmc) o CVS. Para la película se requiere un formato TIFF.<br/>
 
 > **Condiciones de uso.** Toda persona tiene acceso a la lectura y uso del código con fines académicos o de enseñanza. Sin embargo, para el uso clínico del programa se requiere contar con una licencia (disponible próximamente), conocida como “Acuerdo de licencia de usuario final” (EULA, por sus siglas en inglés), así como contratos que garanticen el cumplimiento de la legislación de cada país.<br/>  
 
 Para mayor información contactar al correo electrónico dosepy@gmail.com. 
@@ -389,8 +391,8 @@
 paráfrasis, compilaciones, colecciones y transformaciones del software DOSEPY, podrán ser explotadas
 cuando hayan sido autorizadas por el titular del derecho patrimonial sobre la obra DOSEPY,
 previo consentimiento del titular del derecho moral, en los casos previstos en la Fracción III
 del Artículo 21 de la Ley Federal del Derecho de Autor.
 
 GARANTÍA
 
-El software Dosepy se ofrece sin ninguna garantía de cualquier tipo. Su uso es responsabilidad del usuario.
+El software Dosepy se ofrece sin ninguna garantía de cualquier tipo. Su uso es responsabilidad del usuario.
```

### Comparing `Dosepy-0.3.8/pyproject.toml` & `Dosepy-0.3.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Dosepy"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Gamma analysis and film dosimetry for dose distributions in radiotherapy"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
@@ -28,18 +28,19 @@
 keywords = ["Radiotherapy", "Dose distribution", "gamma index", "python"]
 dependencies = [
   "numpy >= 1.23.4",
   "pydicom >= 2.3.0",
   "matplotlib >= 3.6.1",
   "tifffile >= 2022.10.10",
   "scipy >= 1.9.3",
-  "PyQt5 >= 5.15.7",
+  "PyQt6 >= 6.5.1",
+  "relative_dose_1d >= 0.1.4"
 ]
 [project.urls]
-homepage = "https://luisolivaresj.github.io/Dosepy/"
+homepage = "https://dosepy.readthedocs.io/en/latest/intro.html"
 repository = "https://pypi.org/project/Dosepy/"
 Bug-Tracker = "https://github.com/LuisOlivaresJ/Dosepy"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUI.py` & `Dosepy-0.3.9/src/Dosepy/GUI.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 
     Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
 """
 #---------------------------------------------
 #   Importaciones
 
 import sys
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QApplication, QHBoxLayout, QMessageBox, QMainWindow, QAction, QLabel, QLineEdit
-from PyQt5.QtGui import QIcon, QFont
-from PyQt5.QtCore import Qt
+from PyQt6.QtWidgets import QWidget, QVBoxLayout, QApplication, QHBoxLayout, QMessageBox, QMainWindow, QLabel, QLineEdit
+from PyQt6.QtGui import QIcon, QFont,  QAction
+from PyQt6.QtCore import Qt
+
+from PyQt6.QtWidgets import QFileDialog, QInputDialog
+from relative_dose_1d.tools import build_from_array_and_step, gamma_1D
+#from relative_dose_1d.GUI import Q_Graphic_Block
+
+
 
 import numpy as np
 from Dosepy.GUILayouts.Bloque_gamma import Bloque_gamma
 #from GUILayouts.Bloque_gamma import Bloque_gamma  # Se importa desde archivo en PC para testear
 from Dosepy.GUILayouts.Bloque_Imagenes import Bloque_Imagenes
 #from GUILayouts.Bloque_Imagenes import Bloque_Imagenes   # Se importa desde archivo en PC para testear
 import Dosepy.dose as dp
@@ -57,14 +63,19 @@
 
         self.show()
 
     def cuerpoUI(self):
 
         cuerpo = QWidget()
         self.Bloque_Imagen = Bloque_Imagenes()
+
+
+        self.Bloque_Imagen.boton_recortar_Izq.clicked.connect(self.Cortar_Imagen)
+        self.Bloque_Imagen.compare_button.clicked.connect(self.Compare_profiles)
+
         self.Bloque_Gamma = Bloque_gamma(self.Us)
         self.Bloque_Gamma.Eval_button.clicked.connect(self.mostrar_distribucion)
         self.Bloque_Gamma.Calcular_Button.clicked.connect(self.Calculo_Gamma)
 
         LayoutPrincipal = QVBoxLayout()
         LayoutPrincipal.addWidget(self.Bloque_Gamma)
         LayoutPrincipal.addWidget(self.Bloque_Imagen)
@@ -180,14 +191,68 @@
         #cbar_gamma.ax.set_ylabel('Índice gamma', rotation=90, fontsize= 11)
 
         #self.Bloque_Gamma.Mpl_Img_gamma.Mostrar_Imagen(g)
         self.Bloque_Gamma.Mpl_Histograma.fig.canvas.draw()
         self.Bloque_Gamma.Mpl_Img_gamma.fig.canvas.draw()
 
 
+
+    def Cortar_Imagen(self):
+
+        xi = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_x())
+        width = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_width())
+        yi = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_y())
+        height = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_height())
+
+        npI_Izq = self.Bloque_Imagen.Mpl_Izq.npI[  yi : yi + height , xi : xi + width ]
+        npI_Der = self.Bloque_Imagen.Mpl_Der.npI[  yi : yi + height , xi : xi + width ]
+        self.Bloque_Imagen.D_ref = dp.Dose(npI_Izq, self.Bloque_Imagen.D_ref.resolution)
+        self.Bloque_Imagen.D_eval = dp.Dose(npI_Der, self.Bloque_Imagen.D_eval.resolution)
+
+        self.Bloque_Imagen.Mpl_Izq.Img(self.Bloque_Imagen.D_ref)
+        self.Bloque_Imagen.Mpl_Der.Img(self.Bloque_Imagen.D_eval)
+
+        self.Bloque_Imagen.Mpl_Izq.Colores(npI_Der)
+        self.Bloque_Imagen.Mpl_Der.Colores(npI_Der)
+
+        self.Bloque_Imagen.Mpl_Izq.Cross_Hair_on()
+        self.Bloque_Imagen.Mpl_Der.Cross_Hair_on()
+
+        self.Bloque_Imagen.Mpl_perfiles.set_data_and_plot(npI_Izq, npI_Der, self.Bloque_Imagen.Mpl_Izq.circ)
+
+        self.Bloque_Imagen.Mpl_Izq.ROI_Rect_off()
+        self.Bloque_Imagen.boton_recortar_Izq.setEnabled(False)
+        self.Bloque_Imagen.boton_roi.setChecked(False)
+
+    def Compare_profiles(self):
+
+        resolution = self.Bloque_Imagen.D_ref.resolution
+
+        D_profile_ref = build_from_array_and_step(
+            self.Bloque_Imagen.Mpl_perfiles.perfil_horizontal_ref,
+            resolution
+            )
+        D_profile_eval = build_from_array_and_step(
+            self.Bloque_Imagen.Mpl_perfiles.perfil_horizontal_eval,
+            resolution
+            )
+        
+        gamma, gamma_percent = gamma_1D(
+            D_profile_ref, 
+            D_profile_eval,
+            dose_t = 3, dist_t = 2, dose_tresh = 10, interpol = 1)
+        #print(gamma)
+        print(gamma_percent)
+
+        # TO_DO 
+        # gamma_1D requieres data to be normalized
+        # new fuction inside relative_dose_1d to whow a plot 
+        # plot_gamma_profiles() 
+
+
 ######################################################################
 #   Ventanas para mensajes
     def displayMessageBox(self):
         """
         Si la variable self.Bloque_Gamma.Formatos_ok es True, los archivos
         para las distribuciones de dosis se cargaron correctamente.
         En caso contrario se emite un mensaje de error.
@@ -223,15 +288,15 @@
         label_usuario.move(80, 20)
         layout_principal.addWidget(label_usuario)
         label_usuario.setFont(QFont('Arial', 14))
 
         self.name_entry = QLineEdit(self)
         self.name_entry.setFont(QFont('Arial', 18))
         self.name_entry.setEchoMode(QLineEdit.Password)
-        self.name_entry.setAlignment(Qt.AlignCenter)
+        self.name_entry.setAlignment(Qt.AlignmentFlag.AlignHCenter)
 
         self.name_entry.returnPressed.connect(self.cerrar_UI)
         self.name_entry.move(100, 70)
         layout_principal.addWidget(self.name_entry)
         layout_principal.setSpacing(10)
         self.show()
 
@@ -277,8 +342,8 @@
             self.licencia_window_sec = Licencia_Window()
         self.licencia_window_sec.show()
 
 app = QApplication(sys.argv)
 #windowA = Ventana_Secundaria() 
 windowA = VentanaPrincipal('P')
 
-sys.exit(app.exec_())
+sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/Bloque_Imagenes.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/Bloque_Imagenes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 #---------------------------------------------
 
 #   Importaciones
 
 #---------------------------------------------
 
 from matplotlib import patches
-from PyQt5.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
+from PyQt6.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
 import sys
 import pkg_resources
 from matplotlib.figure import Figure
-#from matplotlib.backends.backend_qt5agg import FigureCanvas
 from matplotlib.backends.backend_qtagg import FigureCanvas
 import matplotlib.colors as colors
 import numpy as np
 from PyQt5.QtGui import QIcon
 
 
 
@@ -92,14 +91,16 @@
         #corte_icon = QIcon("../Icon/cut_icon.png")
         #corte_name_folder = pkg_resources.resource_filename('Dosepy', 'Icon/cut_icon.png')
         self.boton_recortar_Izq = QPushButton('Corte')
         #self.boton_recortar_Izq.setIcon(corte_icon)
         self.boton_recortar_Izq.setEnabled(False)
         self.boton_recortar_Izq.clicked.connect(self.Cortar_Imagen)
 
+        self.compare_button = QPushButton("Compare")
+
         #self.boton_exportar_Izq = QPushButton('Exportar')
         self.boton_exportar_Der = QPushButton('')
         #self.boton_exportar_perfiles = QPushButton('Exportar')
 
         #   Contenedores
         """
         layout_hijo_Izq = QHBoxLayout()
@@ -115,14 +116,16 @@
         layout_hijo_perfiles = QHBoxLayout()
         #layout_hijo_perfiles.addWidget(self.boton_exportar_perfiles)
         layout_hijo_perfiles.addStretch()
         """
         layout_padre_botones = QVBoxLayout()
         layout_padre_botones.addWidget(self.boton_roi)
         layout_padre_botones.addWidget(self.boton_recortar_Izq)
+        layout_padre_botones.addWidget(self.compare_button)
+        layout_padre_botones.addStretch()
 
         layout_padre_Izq = QVBoxLayout()
         #layout_padre_Izq.addLayout(layout_hijo_Izq)
         layout_padre_Izq.addWidget(self.Mpl_Izq.Qt_fig)
 
         layout_padre_Der = QVBoxLayout()
         #layout_padre_Der.addLayout(layout_hijo_Der)
@@ -432,8 +435,8 @@
 #%%
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     ventana_raiz = Bloque_Imagenes()
     ventana_raiz.setGeometry(100, 150, 1200, 300)
     ventana_raiz.show()
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/Bloque_gamma.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/Bloque_gamma.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
-from matplotlib.backends.backend_qt5agg import FigureCanvas
-from PyQt5.QtWidgets import QApplication, QWidget, QLabel, QPushButton, QFormLayout, QLineEdit, QHBoxLayout, QVBoxLayout, QMessageBox
-from PyQt5.QtWidgets import QFileDialog
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QIcon
+from matplotlib.backends.backend_qtagg import FigureCanvas
+from PyQt6.QtWidgets import QApplication, QWidget, QLabel, QPushButton, QFormLayout, QLineEdit, QHBoxLayout, QVBoxLayout, QMessageBox
+from PyQt6.QtWidgets import QFileDialog
+from PyQt6.QtCore import Qt
+from PyQt6.QtGui import QIcon
 from matplotlib.figure import Figure
 import numpy as np
 from Dosepy.GUILayouts.Bloque_Imagenes import Qt_Figure_Imagen
 #from GUILayouts.Bloque_Imagenes import Qt_Figure_Imagen
 import pkg_resources
 import os
 import Dosepy.dose as dp
@@ -57,35 +57,35 @@
             "background : #90EE90;"
             "}")
 
         # Crear LineEdit para parámetros gamma
         self.Toler_dosis = QLineEdit()
         self.Toler_dosis.setFixedWidth(40)
         self.Toler_dosis.setText("3.0")
-        self.Toler_dosis.setAlignment(Qt.AlignRight)
+        self.Toler_dosis.setAlignment(Qt.AlignmentFlag.AlignRight)
         self.Toler_dosis.textChanged.connect(self.revisar_si_es_flotante)
         self.Toler_dosis.setStyleSheet("QLineEdit"
             "{"
             "background : #90EE90;"
             "}")
 
         self.Toler_dist = QLineEdit()
         self.Toler_dist.setFixedWidth(40)
         self.Toler_dist.setText("3.0")
-        self.Toler_dist.setAlignment(Qt.AlignRight)
+        self.Toler_dist.setAlignment(Qt.AlignmentFlag.AlignRight)
         self.Toler_dist.textChanged.connect(self.revisar_si_es_flotante)
         self.Toler_dist.setStyleSheet("QLineEdit"
             "{"
             "background : #90EE90;"
             "}")
         
         self.Umbral_dosis = QLineEdit()
         self.Umbral_dosis.setFixedWidth(40)
         self.Umbral_dosis.setText("10")
-        self.Umbral_dosis.setAlignment(Qt.AlignRight)
+        self.Umbral_dosis.setAlignment(Qt.AlignmentFlag.AlignRight)
         self.Umbral_dosis.textChanged.connect(self.revisar_si_es_flotante)
         self.Umbral_dosis.setStyleSheet("QLineEdit"
             "{"
             "background : #90EE90;"
             "}")
 
         # Crear LineEdit para parámetros gamma
@@ -133,15 +133,15 @@
         Resolution_Form = QFormLayout()
         Resolution_Form.addRow('Distancia entre puntos [mm]', self.Resolution)
 
         if self.Us == 'P':
             #   Crear FormLayout
             Parametros_gamma_Layout = QFormLayout()
             #Parametros_gamma_Layout.setLabelAlignment(Qt.AlignLeft)
-            Parametros_gamma_Layout.setFormAlignment(Qt.AlignRight)
+            Parametros_gamma_Layout.setFormAlignment(Qt.AlignmentFlag.AlignRight)
             Parametros_gamma_Layout.addRow('Toler. en dosis [%]', self.Toler_dosis)
             Parametros_gamma_Layout.addRow('Toler. en distancia [mm]', self.Toler_dist)
             Parametros_gamma_Layout.addRow('Umbral de dosis [%]', self.Umbral_dosis)
 
         #   Crear vertical Layout
 
         Padre_Info_V_Layout = QVBoxLayout()
@@ -289,8 +289,8 @@
 
         self.fig.canvas.draw()
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     window = Bloque_gamma('P')
     window.show()
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/about_window.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/about_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
 
 """
 
 import sys
 import pkg_resources
 
-from PyQt5.QtWidgets import QWidget, QLabel, QVBoxLayout, QHBoxLayout, QApplication
-from PyQt5.QtGui import QIcon, QPixmap, QFont
-from PyQt5.QtCore import Qt
+from PyQt6.QtWidgets import QWidget, QLabel, QVBoxLayout, QHBoxLayout, QApplication
+from PyQt6.QtGui import QPixmap
+from PyQt6.QtCore import Qt
 
 
 class About_Window(QWidget):
     """
     Ventana para mostrar información del programa.
     """
     def __init__(self):
@@ -35,54 +35,54 @@
 
         layout_padre_V = QVBoxLayout()
 
         file_name_logo = pkg_resources.resource_filename('Dosepy', 'Icon/Logo_Dosepy.png')
         logo = QPixmap(file_name_logo)
         #logo.scaled(0.5, 0.5) #Qt.KeepAspectRatio)
         label_logo = QLabel(self)
-        label_logo.setAlignment(Qt.AlignCenter)
+        label_logo.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_logo.setPixmap(logo)
         label_logo.setStyleSheet(
             "border-radius: 15px;" +
             "margin-top: 15px;" +
             "margin-bottom: 15px;" +
             "margin-left: 80px;" +
             "margin-right: 80px;"
         )
 
         layout_padre_V.addWidget(label_logo)
 
         label_version = QLabel(self)
         label_version.setText('Versión 0.3.7')
-        label_version.setAlignment(Qt.AlignCenter)
+        label_version.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_version.setStyleSheet(
             "margin-top: 10px;" +
             "font-size: 22px;" +
             "margin-bottom: 5px;" +
             "color: 'whitesmoke';"
         )
 
         label_derechos = QLabel(self)
         label_derechos.setText('Derechos Reservados (c) \n Luis Alfonso Olivares Jiménez 2021')
-        label_derechos.setAlignment(Qt.AlignCenter)
+        label_derechos.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_derechos.setStyleSheet(
             "margin-top: 5px;" +
             "font-size: 17px;" +
             "margin-bottom: 20px;" +
             "color: 'whitesmoke';"
         )
 
         link_label = QLabel(self)
         link_label.setText(
-            "<a href=\"https://luisolivaresj.github.io/Dosepy//\">Documentación</a>"
+            "<a href=\"https://dosepy.readthedocs.io/en/latest/intro.html\">Documentación</a>"
         )
-        link_label.setTextFormat(Qt.RichText)
+        #link_label.setTextFormat(Qt.RichText)
         #link_label.setTextInteractionFlags(Qt.TextBrowserInteraction)
         link_label.setOpenExternalLinks(True)
-        link_label.setAlignment(Qt.AlignCenter)
+        link_label.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         link_label.setStyleSheet(
             "font-size: 17px;" +
             "margin-bottom: 15px;" +
             "color: 'whitesmoke';"
         )
 
         layout_padre_V.addWidget(label_version)
@@ -93,15 +93,15 @@
         self.setLayout(layout_padre_V)
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     window = About_Window()
     window.show()
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/cross_hair_cursor.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/cross_hair_cursor.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/film_to_doseGUI.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/film_to_doseGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 
 """
 
 #---------------------------------------------
 #   Importaciones
 from Dosepy.tools.film_to_dose import calibracion, cubico
 from Dosepy.tools.resol import match_resolution
+#from ..tools.resol import match_resolution
 
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QApplication, QHBoxLayout, QMessageBox, QMainWindow, QAction, QLabel, QPushButton, QFileDialog, QLayout, QCheckBox, QLineEdit, QFormLayout
-from PyQt5.QtGui import QIcon, QPixmap
-from PyQt5.QtCore import Qt
+from PyQt6.QtWidgets import QWidget, QVBoxLayout, QApplication, QHBoxLayout, QMessageBox, QMainWindow, QLabel, QPushButton, QFileDialog, QLayout, QCheckBox, QLineEdit, QFormLayout
+from PyQt6.QtGui import QIcon, QPixmap
+from PyQt6.QtCore import Qt
 
 from matplotlib.figure import Figure
-from matplotlib.backends.backend_qt5agg import FigureCanvas
+from matplotlib.backends.backend_qtagg import FigureCanvas
 import matplotlib.colors as colors
 import tifffile as tiff
 import numpy as np
 import pkg_resources
 import sys
 import os
 
@@ -72,27 +73,27 @@
         layout_padre_botones.addSpacing(50)
         layout_padre_botones.addWidget(self.button_leer_tiff_pre)
         layout_padre_botones.addWidget(self.label_a0)
         layout_padre_botones.addWidget(self.label_a1)
         layout_padre_botones.addWidget(self.label_a2)
         layout_padre_botones.addWidget(self.label_a3)
         layout_padre_botones.addSpacing(70)
-        layout_padre_botones.setAlignment(Qt.AlignTop)
+        layout_padre_botones.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         #   Widget para los perfiles
         self.Qt_Mpl_curva_calib = Qt_Figure_CurvaCalibracion()
 
         layout_abuelo.addWidget(self.Qt_Mpl_curva_calib.Qt_fig)
         layout_abuelo.addLayout(layout_padre_botones)
 
         file_name_image_logo = pkg_resources.resource_filename('Dosepy', 'Icon/Logo_Dosepy.png')
         #file_name_image_logo = 'Logo_Dosepy.png'
         pixmap_logo = QPixmap(file_name_image_logo)
         self.label_logo = QLabel(self)
-        self.label_logo.setAlignment(Qt.AlignCenter)
+        self.label_logo.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         self.label_logo.setPixmap(pixmap_logo)
         self.Qt_Mpl_distribucion = Qt_Figure_Imagen()
 
         self.button_distr_pre = QPushButton('Dist.')
         self.button_distr_pre.setEnabled(False)
         self.button_distr_pre.clicked.connect(self.leer_tiff_pre_distr)
         self.button_distr_pre.setIcon(folder_icon)
@@ -135,15 +136,15 @@
         layout_padre_botones_2inf.addWidget(self.check_button_tif)
         layout_padre_botones_2inf.addWidget(self.check_button_csv)
 
         layout_padre_botones_2inf.addSpacing(40)
         #layout_padre_botones_2inf.addWidget(self.QLabel_Reducir_resolucion)
         layout_padre_botones_2inf.addLayout(Qform_layout_resol)
         layout_padre_botones_2inf.addWidget(self.button_reducir)
-        layout_padre_botones_2inf.setAlignment(Qt.AlignTop)
+        layout_padre_botones_2inf.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         layout_abuelo_2inf.addWidget(self.Qt_Mpl_distribucion.Qt_fig)
         layout_abuelo_2inf.addLayout(layout_padre_botones_2inf)
 
         layout_bisabuelo.addWidget(self.label_logo)
         layout_bisabuelo.addLayout(layout_abuelo)
         layout_bisabuelo.addSpacing(40)
@@ -371,8 +372,8 @@
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     window = Film_to_Dose_Window()
     window.show()
 
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/licencia_window.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/licencia_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
 
 """
 
 import sys
 import pkg_resources
 
-from PyQt5.QtWidgets import QWidget, QLabel, QVBoxLayout, QHBoxLayout, QApplication, QPlainTextEdit
-from PyQt5.QtGui import QIcon, QPixmap, QFont
-from PyQt5.QtCore import Qt
+from PyQt6.QtWidgets import QWidget, QLabel, QVBoxLayout, QHBoxLayout, QApplication, QPlainTextEdit
+from PyQt6.QtGui import QPixmap
+from PyQt6.QtCore import Qt
 
 
 class Licencia_Window(QWidget):
     """
     Ventana para mostrar licencia.
     """
     def __init__(self):
@@ -39,29 +39,29 @@
 
         layout_padre_V = QVBoxLayout()
 
         file_name_logo = pkg_resources.resource_filename('Dosepy', 'Icon/Logo_Dosepy.png')
         logo = QPixmap(file_name_logo)
         #logo.scaled(0.5, 0.5) #Qt.KeepAspectRatio)
         label_logo = QLabel(self)
-        label_logo.setAlignment(Qt.AlignCenter)
+        label_logo.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_logo.setPixmap(logo)
         label_logo.setStyleSheet(
             "border-radius: 15px;" +
             "margin-top: 15px;" +
             "margin-bottom: 15px;" +
             "margin-left: 80px;" +
             "margin-right: 80px;"
         )
 
         layout_padre_V.addWidget(label_logo)
 
         label_version = QLabel(self)
         label_version.setText('PROPRIETARY LICENSE')
-        label_version.setAlignment(Qt.AlignCenter)
+        label_version.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_version.setStyleSheet(
             "margin-top: 10px;" +
             "font-size: 22px;" +
             "margin-bottom: 5px;" +
             "color: 'whitesmoke';"
         )
 
@@ -95,30 +95,30 @@
 
 El software Dosepy se ofrece sin ninguna garantía de cualquier tipo. Su uso es responsabilidad del usuario.
 
 Para mayor información contactar al correo electrónico dosepy@gmail.com. 
 
 ''')
         label_info_licencia.setReadOnly(True)
-        #label_info_licencia.setAlignment(Qt.AlignCenter)
+        #label_info_licencia.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_info_licencia.setStyleSheet(
             "margin-top: 5px;" +
             "font-size: 17px;" +
             "margin-bottom: 20px;" +
             "color: 'whitesmoke';"
         )
 
         link_label = QLabel(self)
         link_label.setText(
-            "<a href=\"https://luisolivaresj.github.io/Dosepy//\">Home page</a>"
+            "<a href=\"https://dosepy.readthedocs.io/en/latest/intro.html\">Home page</a>"
         )
-        link_label.setTextFormat(Qt.RichText)
+        #link_label.setTextFormat(Qt.RichText)
         #link_label.setTextInteractionFlags(Qt.TextBrowserInteraction)
         link_label.setOpenExternalLinks(True)
-        #link_label.setAlignment(Qt.AlignCenter)
+        #link_label.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         link_label.setStyleSheet(
             "font-size: 17px;" +
             "margin-bottom: 15px;" +
             "color: 'whitesmoke';"
         )
 
         layout_padre_V.addWidget(label_version)
@@ -129,8 +129,8 @@
         self.setLayout(layout_padre_V)
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     window = Licencia_Window()
     window.show()
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.8/src/Dosepy/GUILayouts/to_do_rendering.py` & `Dosepy-0.3.9/src/Dosepy/GUILayouts/to_do_rendering.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/Icon/Icon.png` & `Dosepy-0.3.9/src/Dosepy/Icon/Icon.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/Icon/Logo_Dosepy.png` & `Dosepy-0.3.9/src/Dosepy/Icon/Logo_Dosepy.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/Icon/folder.png` & `Dosepy-0.3.9/src/Dosepy/Icon/folder.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/Icon/save.png` & `Dosepy-0.3.9/src/Dosepy/Icon/save.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/data/D_FILM.csv` & `Dosepy-0.3.9/src/Dosepy/data/D_FILM.csv`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/data/D_TPS.csv` & `Dosepy-0.3.9/src/Dosepy/data/D_TPS.csv`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/dose.py` & `Dosepy-0.3.9/src/Dosepy/dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/tools/film_to_dose.py` & `Dosepy-0.3.9/src/Dosepy/tools/film_to_dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy/tools/resol.py` & `Dosepy-0.3.9/src/Dosepy/tools/resol.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.8/src/Dosepy.egg-info/PKG-INFO` & `Dosepy-0.3.9/src/Dosepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Dosepy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Gamma analysis and film dosimetry for dose distributions in radiotherapy
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
-Project-URL: homepage, https://luisolivaresj.github.io/Dosepy/
+Project-URL: homepage, https://dosepy.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://pypi.org/project/Dosepy/
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/Dosepy
 Keywords: Radiotherapy,Dose distribution,gamma index,python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -17,14 +17,16 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *Dosepy*
 
+[ReadTheDocs Documentation](https://dosepy.readthedocs.io/en/latest/intro.html)
+
 *Dosepy* es un paquete de código escrito en Python para la comparación mediante índice gamma de dos distribuciones de dosis, 2-dimensional. Adicionalmente, se cuenta con una herramienta para realizar dosimetría con película radiocrómica.<br/>
 
 El formato de los archivos que contengan la distribución de dosis puede ser DICOM (.dmc) o CVS. Para la película se requiere un formato TIFF.<br/>
 
 > **Condiciones de uso.** Toda persona tiene acceso a la lectura y uso del código con fines académicos o de enseñanza. Sin embargo, para el uso clínico del programa se requiere contar con una licencia (disponible próximamente), conocida como “Acuerdo de licencia de usuario final” (EULA, por sus siglas en inglés), así como contratos que garanticen el cumplimiento de la legislación de cada país.<br/>  
 
 Para mayor información contactar al correo electrónico dosepy@gmail.com.
```

### Comparing `Dosepy-0.3.8/src/Dosepy.egg-info/SOURCES.txt` & `Dosepy-0.3.9/src/Dosepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

