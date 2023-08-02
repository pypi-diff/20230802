# Comparing `tmp/Dosepy-0.3.9.tar.gz` & `tmp/Dosepy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dosepy-0.3.9.tar", last modified: Tue Jul 11 17:45:40 2023, max compression
+gzip compressed data, was "Dosepy-0.4.0.tar", last modified: Wed Aug  2 19:24:47 2023, max compression
```

## Comparing `Dosepy-0.3.9.tar` & `Dosepy-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.540393 Dosepy-0.3.9/
--rw-rw-rw-   0        0        0     1108 2023-07-11 16:51:08.000000 Dosepy-0.3.9/LICENSE
--rw-rw-rw-   0        0        0       41 2022-11-01 02:03:00.000000 Dosepy-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0    20387 2023-07-11 17:45:40.533392 Dosepy-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    19411 2023-07-11 16:51:08.000000 Dosepy-0.3.9/README.md
--rw-rw-rw-   0        0        0     1392 2023-07-11 17:44:51.000000 Dosepy-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 17:45:40.541372 Dosepy-0.3.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.243015 Dosepy-0.3.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.271999 Dosepy-0.3.9/src/Dosepy/
--rw-rw-rw-   0        0        0    13915 2023-07-11 17:41:58.000000 Dosepy-0.3.9/src/Dosepy/GUI.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.334963 Dosepy-0.3.9/src/Dosepy/GUILayouts/
--rw-rw-rw-   0        0        0    14523 2023-07-11 17:43:28.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/Bloque_Imagenes.py
--rw-rw-rw-   0        0        0    11479 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/Bloque_gamma.py
--rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/__init__.py
--rw-rw-rw-   0        0        0     3149 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/about_window.py
--rw-rw-rw-   0        0        0     3457 2022-11-12 15:41:30.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/cross_hair_cursor.py
--rw-rw-rw-   0        0        0      447 2022-11-12 17:56:22.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/cursor.py
--rw-rw-rw-   0        0        0    15957 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/film_to_doseGUI.py
--rw-rw-rw-   0        0        0     4711 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/licencia_window.py
--rw-rw-rw-   0        0        0     4921 2022-11-14 00:38:07.000000 Dosepy-0.3.9/src/Dosepy/GUILayouts/to_do_rendering.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.351953 Dosepy-0.3.9/src/Dosepy/Icon/
--rw-rw-rw-   0        0        0   568371 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/Icon.png
--rw-rw-rw-   0        0        0    14061 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/Logo_Dosepy.png
--rw-rw-rw-   0        0        0    11084 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/folder.png
--rw-rw-rw-   0        0        0     5824 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/Icon/save.png
--rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.441902 Dosepy-0.3.9/src/Dosepy/data/
--rw-rw-rw-   0        0        0   380730 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/data/D_FILM.csv
--rw-rw-rw-   0        0        0   380730 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/data/D_TPS.csv
--rw-rw-rw-   0        0        0    15468 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/dose.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.524410 Dosepy-0.3.9/src/Dosepy/tools/
--rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.3.9/src/Dosepy/tools/__init__.py
--rw-rw-rw-   0        0        0     4433 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/tools/film_to_dose.py
--rw-rw-rw-   0        0        0     4330 2023-07-11 16:51:09.000000 Dosepy-0.3.9/src/Dosepy/tools/resol.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:45:40.292987 Dosepy-0.3.9/src/Dosepy.egg-info/
--rw-rw-rw-   0        0        0    20387 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      872 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 17:45:40.000000 Dosepy-0.3.9/src/Dosepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.928931 Dosepy-0.4.0/
+-rw-rw-rw-   0        0        0     1413 2023-08-02 17:21:30.000000 Dosepy-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       41 2022-11-01 02:03:00.000000 Dosepy-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11230 2023-08-02 19:24:47.928931 Dosepy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10254 2023-08-02 17:45:51.000000 Dosepy-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1392 2023-08-02 16:56:00.000000 Dosepy-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 19:24:47.928931 Dosepy-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.600828 Dosepy-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.632075 Dosepy-0.4.0/src/Dosepy/
+-rw-rw-rw-   0        0        0    19314 2023-08-02 19:17:34.000000 Dosepy-0.4.0/src/Dosepy/GUI.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.803940 Dosepy-0.4.0/src/Dosepy/GUILayouts/
+-rw-rw-rw-   0        0        0    13382 2023-08-02 16:12:38.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/Bloque_Imagenes.py
+-rw-rw-rw-   0        0        0     7766 2023-08-02 19:23:18.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/Bloque_gamma.py
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/__init__.py
+-rw-rw-rw-   0        0        0     3153 2023-07-11 20:16:10.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/about_window.py
+-rw-rw-rw-   0        0        0     3457 2022-11-12 15:41:30.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/cross_hair_cursor.py
+-rw-rw-rw-   0        0        0      447 2022-11-12 17:56:22.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/cursor.py
+-rw-rw-rw-   0        0        0    15957 2023-07-11 20:16:10.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/film_to_doseGUI.py
+-rw-rw-rw-   0        0        0     4712 2023-08-02 17:21:42.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/licencia_window.py
+-rw-rw-rw-   0        0        0     4921 2022-11-14 00:38:07.000000 Dosepy-0.4.0/src/Dosepy/GUILayouts/to_do_rendering.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.835189 Dosepy-0.4.0/src/Dosepy/Icon/
+-rw-rw-rw-   0        0        0   568371 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/Icon/Icon.png
+-rw-rw-rw-   0        0        0    14061 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/Icon/Logo_Dosepy.png
+-rw-rw-rw-   0        0        0    11084 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/Icon/folder.png
+-rw-rw-rw-   0        0        0     5824 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/Icon/save.png
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.882085 Dosepy-0.4.0/src/Dosepy/data/
+-rw-rw-rw-   0        0        0   380730 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/data/D_FILM.csv
+-rw-rw-rw-   0        0        0   380730 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/data/D_TPS.csv
+-rw-rw-rw-   0        0        0    15468 2023-07-11 19:51:55.000000 Dosepy-0.4.0/src/Dosepy/dose.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.928931 Dosepy-0.4.0/src/Dosepy/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-01 02:03:01.000000 Dosepy-0.4.0/src/Dosepy/tools/__init__.py
+-rw-rw-rw-   0        0        0     4433 2023-07-11 19:51:55.000000 Dosepy-0.4.0/src/Dosepy/tools/film_to_dose.py
+-rw-rw-rw-   0        0        0     4330 2023-07-11 19:51:55.000000 Dosepy-0.4.0/src/Dosepy/tools/resol.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:24:47.647699 Dosepy-0.4.0/src/Dosepy.egg-info/
+-rw-rw-rw-   0        0        0    11230 2023-08-02 19:24:47.000000 Dosepy-0.4.0/src/Dosepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      872 2023-08-02 19:24:47.000000 Dosepy-0.4.0/src/Dosepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 19:24:47.000000 Dosepy-0.4.0/src/Dosepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-08-02 19:24:47.000000 Dosepy-0.4.0/src/Dosepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 19:24:47.000000 Dosepy-0.4.0/src/Dosepy.egg-info/top_level.txt
```

### Comparing `Dosepy-0.3.9/README.md` & `Dosepy-0.4.0/src/Dosepy/dose.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,398 +1,342 @@
-# *Dosepy*
+# -*- coding: utf-8 -*-
+import numpy as np
+import pydicom
+import matplotlib.pyplot as plt
 
-[ReadTheDocs Documentation](https://dosepy.readthedocs.io/en/latest/intro.html)
+class Dose:
+    ''' Clase para la representación de una distribución de dosis absorbida.
 
-*Dosepy* es un paquete de código escrito en Python para la comparación mediante índice gamma de dos distribuciones de dosis, 2-dimensional. Adicionalmente, se cuenta con una herramienta para realizar dosimetría con película radiocrómica.<br/>
+    Regresa un objeto Dose que contiene la distribución de dosis y la resolución espacial.
 
-El formato de los archivos que contengan la distribución de dosis puede ser DICOM (.dmc) o CVS. Para la película se requiere un formato TIFF.<br/>
+    Parameters
+    ----------
+    array : numpy.ndarray
+        Arreglo o matriz de datos. Cada valor numérico representa la dosis absorbida en un punto en el espacio.
+
+    resolution : float
+        Resolución espacial dada como la distancia física (en milímetros) entre dos puntos consecutivos.
+
+    '''
+
+    def __init__(self, array, resolution):
+        '''
+        Inicialización del objeto Dose. Como primer argumento, array, se espera un objeto ndarray 2D (arreglo matricial de datos).
+        Como segundo argumento, resolution, se espera la distancia física (en mm) entre dos puntos consecutivos.
+        '''
+
+        self.array = array                  #   Valores numéricos de la distribución de dosis
+        self.columns = array.shape[1]       #   Número de columnas en la matriz.
+        self.rows = array.shape[0]          #   Número de filas en la matriz.
+        self.resolution = resolution;       #   Resolución espacial dada como la distancia entre dos puntos consecutivos [mm].
+
+    def gamma2D(self, D_reference, dose_t=3, dist_t=3, dose_tresh=10, dose_t_Gy=False, local_norm=False, mask_radius=10, max_as_percentile = True):
+        '''
+        Cálculo del índice gamma contra una distribución de referencia.
+        Se obtiene una matriz que representa los índices gamma en cada posición de la distribución de dosis,
+        así como el índice de aprobación definido como el porcentaje de valores gamma que son menor o igual a 1.
+        Se asume el registro de las distribuciones de dosis, es decir, que la coordenada espacial de un punto en la distribución de
+        referencia es igual a la coordenada del mismo punto en la distribución a evaluar.
+
+        Parameters
+        ----------
+
+        D_reference : Objeto Dose
+            Distribución de dosis de referencia contra la cual se realizará la comparación.
+            El número de filas y columnas debe de ser igual a la distribución a evaluar (self.array).
+            Lo anterior implica que las dimesiones espaciales de las distribuciones deben de ser iguales.
+
+        dose_t : float, default = 3
+            Tolerancia para la diferencia en dosis.
+            Este valor puede interpretarse de 3 formas diferentes según los parámetros dose_t_Gy,
+            local_norm y max_as_percentil, los cuales se describen más adelante.
+
+        dist_t : float, default = 3
+            Tolerancia para la distancia, en milímetros (criterio DTA [1]).
+
+        dose_tresh : float, default = 10
+            Umbral de dosis, en porcentaje (0 a 100) con respecto a la dosis máxima de la 
+            distribución de referencia (o al percentil 99 si max_as_percentile = TRUE). 
+            Todo punto en la distribución de dosis con un valor menor al umbral
+            de dosis, es excluido del análisis.
+            
+        dose_t_Gy : bool, default: False
+            Si el argumento es True, entonces "dose_t" (la dosis de tolerancia) se interpreta como un valor fijo y absoluto en Gray [Gy].
+            Si el argumento es False (default), "dose_t" se interpreta como un porcentaje.
+
+        local_norm : bool, default: False
+            Si el argumento es True (normalización local), el porcentaje de dosis de tolerancia "dose_t" se interpreta con respecto a la dosis local
+            en cada punto de la distribución de referencia.
+            Si el argumento es False (normalización global), el porcentaje de dosis de tolerancia "dose_t" se interpreta con respecto al
+            máximo de la distribución a evaluar.
+            Notas:
+            * Los argumentos dose_t_Gy y local_norm NO deben ser seleccionados como True de forma simultánea.
+            * Si se desea utilizar directamente el máximo de la distirbución, utilizar el parámetro max_as_percentile = False (ver explicación mas adelante).
+
+        mask_radius : float, default: 10
+            Distancia física en milímetros que se utiliza para acotar el cálculo con posiciones que estén dentro de una vecindad dada por mask_radius.
+
+            Para lo anterior, se genera un área de busqueda cuadrada o "máscara" aldrededor de cada punto o posición en la distribución de referencia.
+            El uso de esta máscara permite reducir el tiempo de cálculo debido al siguiente proceso:
+            
+                Por cada punto en la distribución de referencia, el cálculo de la función Gamma se realiza solamente
+                con aquellos puntos o posiciones de la distribución a evaluar que se encuentren a una distancia relativa
+                menor o igual a mask_radius, es decir, con los puntos que están dentro de la vecindad dada por mask_radius.
+                La longitud de uno de los lados de la máscara cuadrada es de 2*mask_radius + 1.
 
-> **Condiciones de uso.** Toda persona tiene acceso a la lectura y uso del código con fines académicos o de enseñanza. Sin embargo, para el uso clínico del programa se requiere contar con una licencia (disponible próximamente), conocida como “Acuerdo de licencia de usuario final” (EULA, por sus siglas en inglés), así como contratos que garanticen el cumplimiento de la legislación de cada país.<br/>  
+            Por otro lado, si se prefiere comparar con todos los puntos de la distribución a evaluar, es suficiente con ingresar
+            una distancia mayor a las dimensiones de la distribución de dosis (por ejemplo mask_radius = 1000).
 
-Para mayor información contactar al correo electrónico dosepy@gmail.com. 
+        max_as_percentile : bool, default: True
+        * Si el argumento es True, se utiliza el percentil 99 como una aproximación del valor máximo de la
+        distribución de dosis. Lo anterior permite excluir artefactos o errores en posiciones puntuales
+        (de utilidad por ejemplo cuando se utiliza película radiocrómica o etiquetas puntuales en la distribución).
+        * Si el argumento es False, se utiliza directamente el valor máximo de la distribución a evaluar.
 
-Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
+        Returns
+        -------
 
-## Métodos de comparación
+        ndarray :
+            Array, o matriz bidimensional con la distribución de índices gamma.
 
-### Comparación por índice gamma
-La comparación de dos distribuciones puede realizarse mediante la prueba del índice gamma 2-dimensional de acuerdo a la definición dada por [Low D. A.](https://doi.org/10.1118/1.598248) así como algunas recomendaciones del [TG-218]( https://doi.org/10.1002/mp.12810) de la AAPM:
+        float :
+            Índice de aprobación. Se calcula como el porcentaje de valores gamma <= 1, sin incluir las posiciones
+            en donde la dosis es menor al umbral de dosis.
 
-* El criterio de aceptación para la diferencia en dosis puede ser seleccionado en modo absoluto (en Gy) o en modo relativo (en %).
-  * En modo relativo, el porcentaje puede interpretarse con respecto al máximo de la distribución de dosis a evaluar (normalización global), o con respecto a la dosis local en la distribución de referencia (normalización local); según la selección del usuario.
-* El umbral de dosis puede ser ajustado por el usuario.
-* La distribución de referencia puede ser seleccionada por el usuario.
-* Se permite definir un radio de búsqueda como proceso de optimización para el cálculo.
-* Es posible utilizar el percentil 99.1 de la distribución de dosis como una aproximación del valor máximo. Esto permite evitar la posible inclusión de artefactos o errores en posiciones puntuales de la distribución (de utilidad por ejemplo cuando se utiliza película radiocrómica).
-* No se realiza interpolación entre puntos.
+        Notes
+        -----
 
-**Proceso de una primera validación del algoritmo gamma**<br/>
+        Es posible utilizar el percentil 99 de la distribución de dosis como una aproximación del valor máximo.
+        Esto permite evitar la posible inclusión de artefactos o errores en posiciones puntuales de la distribución
+        (de utilidad por ejemplo cuando se utiliza película radiocrómica o etiquetas puntuales en la distribución).
 
-[Resumen](https://github.com/LuisOlivaresJ/Dosepy/blob/2bf579e6c33c347ef8f0cdd6f4ee7534798f0d13/docs/assets/validation.pdf)<br/>
-La validación del algoritmo para la prueba del índice gamma se realizó mediante la comparación de resultados contra los softwares DoseLab 4.11 y VeriSoft 7.1.0.199. Dicho trabajo se presentó en el 7mo Congreso de la Federación Mexicana de Organizaiones de Física Médica en el año 2021 [(Video)](https://youtu.be/HM4qkYGzNFc).
+        Se asume que ambas distribuciones a evaluar representan exactamente las mismas dimensiones físicas, y las posiciones
+        espaciales para cada punto conciden entre ellas, es decir, las imagenes de cada distribución están registradas.
 
-**¡Consideraciones!**
+        No se realiza interpolación entre puntos.
 
-* Ambas distribuciones deben tener las mismas dimensiones físicas y resolución espacial (mismo número de filas y columnas).
-* Las distribuciones deben de  encontrarse registradas, es decir, la coordenada espacial de un punto en la distribución de referencia debe ser igual a la coordenada del mismo punto en la distribución a evaluar.<br/>
+        Referencias
+        
+        Para mayor información sobre los mecanismos de operación, efectividad y exactitud de la herramienta gamma consultar:
 
-En caso contrario, *Dosepy* dispone de algunas funciones para cumplir con lo anterior.
+        [1] M. Miften, A. Olch, et. al. "Tolerance Limits and Methodologies for IMRT Measurement-Based
+            Verification QA: Recommendations of AAPM Task Group No. 218" Medical Physics, vol. 45, nº 4, pp. e53-e83, 2018.
 
-## Instalación
-**En Linux**<br/>
-El método más sencillo para instalar Dosepy es escribiendo en una terminal:
-```bash
-pip install Dosepy
-```
-**En Windows**<br/>
-Previo a la instalación de Dosepy, es necesario contar con un administrador de paquetes. Para quienes no estén familiarizados con los paquetes Python, se recomienda utilizar la plataforma [ANACONDA](https://www.anaconda.com/products/individual).
-Una vez que se ha instalado ANACONDA, abrir el inicio de Windows y buscar *Anaconda Prompt*. Dentro de la terminal (ventana con fondo negro), seguir la indicación descrita para Linux (párrafo anterior).
+        [2] D. Low, W. Harms, S. Mutic y J. Purdy, «A technique for the quantitative evaluation of dose distributions,»
+            Medical Physics, vol. 25, nº 5, pp. 656-661, 1998.
 
-### Versión Beta
-Dosepy se encuentra en una versión beta, especificada por el formato 0.X.X. Lo anterior implica que en la práctica, un código que utiliza el paquete Dosepy en una versión, pudiera no ser ejecutado en una versión posterior.  La versión estable será publicada con el formato 1.X.X.<br/>
-Para mantener actualizado el paquete Dosepy, utilizar [pip](https://pip.pypa.io/en/stable/):
-```bash
-pip install --upgrade Dosepy
-```
+        [3] L. A. Olivares-Jimenez, "Distribución de dosis en radioterapia de intensidad modulada usando películas de tinte
+            radiocrómico : irradiación de cerebro completo con protección a hipocampo y columna con protección a médula"
+            (Tesis de Maestría) Posgrado en Ciencias Físicas, IF-UNAM, México, 2019
 
-### Ejemplos
- 
-**Ejemplo con interfaz gráfica**
+        Examples
+        --------
 
-Para utilizar *Dosepy* con una interfaz gráfica , abrimos una terminal (o Anaconda Prompt en el caso de Windows) y escribimos el comando **python**:
+        Archivo en formato CSV (comma separated values)
 
-```bash
-python
-```
-Posteriormente, escribimos:
+            import Dosepy.dose as dp
 
-```python
-import Dosepy.GUI
-```
+            #   Cargamos los archivos "D_TPS.csv" y "D_FILM.csv"
+            #   (Los archivos de ejemplo .csv se encuentran dentro del paquete Dosepy, en la carpeta src/Dosepy/data)
+            >>> D_eval = dp.from_csv("D_TPS.csv", 1)
+            >>> D_ref = dp.from_csv("D_FILM.csv", 1)
 
-**Uso de un Notebook**
+            #   Llamamos al método gamma2D, con criterio 3 %, 2 mm.
+            >>> g, pass_rate = D_eval.gamma2D(D_ref, 3, 2)
 
-Para aprender a utilizar todas las herramientas de *Dosepy* se recomienda el uso de un Notebook del entorno [Jupyter](https://jupyter.org/). [*Aquí*](Notebook.md) puedes consultar una guía para ello.
+            #   Imprimimos el resultado
+            >>> print(f'El índice de aprobación es: {pass_rate:.1f} %')
+            >>> plt.imshow(g, vmax = 1.4)
+            >>> plt.show()
 
-### Importación de archivo en formato csv
-La importación de la distribución de referencia puede realizarse sólo si el archivos se encuentra en formato .csv (valores separados por comas). Adicionalmente:
-* El archivo deberá contener sólo los valores de dosis.
-* Toda información adicional deberá estar precedida con el carácter "#". Ello indicará que todos los caracteres que se encuentren en la misma linea después de "#" debe de ser ignorados por Dosepy.
-* La unidad para la dosis deberá ser el Gray (Gy).
+            El índice de aprobación es: 98.9 %
 
-### Importación de archivo en formato dcm
-La distribución a evaluar puede importarse en un archivo con formato .csv o en formato .dcm (archivo DICOM). Si el formato es DICOM:
-* Deberá contener sólo un plano de dosis.
-* La resolución espacial debe ser igual en cada dimensión.
-* La unidad para la dosis deberá ser el Gray (Gy).
+        '''
 
-## Ejemplo utilizando una terminal
-En *Dosepy*, una distribución de dosis es representada como un objeto de la [clase](https://docs.python.org/es/3/tutorial/classes.html) **Dose** del paquete *Dosepy*. Para crear el objeto son necesarios dos argumentos: las dosis de la distribución en formato [ndarray](https://numpy.org/doc/stable/reference/index.html#module-numpy) y la resolución espacial dada por la distancia (en milímetros) entre dos puntos consecutivos.
-Para utilizar *Dosepy*, abrimos una terminal (o Anaconda Prompt en el caso de Windows) y escribimos el comando python:
+        #%%
 
-```bash
-python
-```
+        #   Verificar la ocurrencia de excepciones
+        if D_reference.array.shape != self.array.shape:
+            raise Exception("No es posible el cálculo con matrices de diferente tamaño.")
 
-Dentro de Python, escribimos el siguiente código de prueba:
+        if local_norm and dose_t_Gy:
+            raise Exception("No es posible la selección simultánea de dose_t_Gy y local_norm.")
 
-```python
-import numpy as np
-import Dosepy.dose as dp
+        if D_reference.resolution != self.resolution:
+            raise Exception("No es posible el cálculo con resoluciones diferentes para cada distribución.")
 
-a = np.zeros((10,10)) + 96   # Matrices de prueba
-b = np.zeros((10,10)) + 100  
+        #%%
 
-D_ref = dp.Dose(a, 1)   # Se crea la distribución de referencia
-D_eval = dp.Dose(b, 1)  # Se crea la distribución a evaluar
-```
-
-La comparación gamma entre dos distribuciones de dosis se realiza mediante el método *gamma2D*. Como argumentos se requiere:
-* La distribución de dosis de referencia
-* El porcentaje para la diferencia en dosis de tolerancia
-* La distancia de tolerancia o criterio DTA en mm.
-
-```python
-#   Llamamos al método gamma2D, con criterio 3 %, 1 mm.
-gamma_distribution, pass_rate = D_eval.gamma2D(D_ref, dose_t = 3, dist_t = 1)
-print(pass_rate)
-```
-
-## Datos en formato CSV, usando un umbral de dosis
-
-Es posible cargar archivos de datos en fromato CSV (comma separate values) mediante la función *from_csv* del paquete Dosepy.
-Para descartar filas dentro del archivo, utilizar el caracter # al inicio de cada fila (inicio de un comentario).
-```python
-import Dosepy.dose as dp
-import matplotlib.pyplot as plt
+        D_ref = D_reference.array
+        D_eval = self.array
 
-#   Cargamos los archivos "D_TPS.csv" y "D_FILM.csv", ambos con 1.0 milímetro de espacio entre un punto y otro.
-#   (Los archivos de ejemplo .csv se encuentran dentro del paquete Dosepy, en la carpeta src/Dosepy/data/)
-D_eval = dp.from_csv("D_TPS.csv", PixelSpacing = 1)
-D_ref = dp.from_csv("D_FILM.csv", PixelSpacing = 1)
-
-#   Llamamos al método gamma2D, con criterio 3 %, 2 mm, descartando puntos con dosis por debajo del 10 %.
-g, pass_rate = D_eval.gamma2D(D_ref, dose_t = 3, dist_t = 2, dose_tresh = 10)
-
-#   Imprimimos el resultado
-print(f'El índice de aprobación es: {pass_rate:.1f} %')
-plt.imshow(g, vmax = 1.4)
-plt.show()
-
-#El índice de aprobación es: 98.9 %
-
-```
-## Datos en formato DICOM y modo de dosis absoluto
-
-Importación de un archivo de dosis en formato DICOM
-
-*Consideraciones*
-
-* La distribución de dosis en el archivo DICOM debe contener solo dos dimensiones (2D).
-* El espacio entre dos puntos (pixeles) debe de ser igual en ambas dimensiones.
-* No se hace uso de las coordenadas dadas en el archivo DICOM. Ver primera consideración en el apartado Gamma index.
-
-```python
-import Dosepy.dose as dp
-
-#   Cargamos los archivos "RD_file.dcm" y "D_FILM_2mm.csv", ambos con 2 milímetro de espacio entre un punto y otro.
-D_eval = dp.from_dicom("RD_file.dcm")
-D_ref = dp.from_csv("D_FILM_2mm.csv", PixelSpacing = 2)
-
-#   Llamamos al método gamma2D, con criterio de 0.5 Gy para la diferencia en dosis y 3 mm para la diferencia en distancia.
-g, pass_rate = D_eval.gamma2D(D_ref, 0.5, 3, dose_t_Gy = True)
-
-#   Imprimimos el resultado
-print(pass_rate)
-
-```
-
-# Documentación
-```
-Dosepy.dose.Dose(data, resolution)
-  Clase para la representación de una distribución de dosis absorbida.
-  Regresa un objeto Dose que contiene la distribución de dosis y la resolución espacial.
-
-Parameters:
-           data : numpy.ndarray
-                Arreglo o matriz de datos. Cada valor numérico representa la dosis absorbida en un punto en el espacio.
-
-           resolution : float
-                Resolución espacial dada como la distancia física (en milímetros) entre dos puntos consecutivos.
-
-Dose methods
-
-Dose.gamma2D(
-  D_reference,
-  dose_t = 3,
-  dist_t = 3,
-  dose_tresh = 10,
-  dose_t_Gy = False,
-  local_norm = False,
-  mask_radius = 10,
-  max_as_percentile = True
-  )
-
-Cálculo del índice gamma contra una distribución de referencia.
-Se obtiene una matriz que representa los índices gamma en cada posición de la distribución de dosis, así como el índice de aprobación
-definido como el porcentaje de valores gamma que son menor o igual a 1.
-Consideraciones:
-Se asume el registro de las distribuciones de dosis, es decir, que la coordenada espacial de un punto en la distribución de referencia
-es igual a la coordenada del mismo punto en la distribución a evaluar.
-
-Parámetros
-----------
-D_reference : Objeto Dose
-    Distribución de dosis de referencia contra la cual se realizará la comparación.
-    El número de filas y columnas debe de ser igual a la distribución a evaluar (self.array).
-    Lo anterior implica que las dimesiones espaciales de las distribuciones deben de ser iguales.
-
-dose_t : float, default = 3
-    Tolerancia para la diferencia en dosis.
-    Este valor puede interpretarse de 3 formas diferentes según los parámetros dose_t_Gy,
-    local_norm y max_as_percentil, los cuales se describen más adelante.
-
-dist_t : float, default = 3
-    Tolerancia para la distancia, en milímetros (criterio DTA [1]).
-
-dose_tresh : float, default = 10
-    Umbral de dosis, en porcentaje (0 a 100) con respecto a la dosis máxima de la 
-    distribución de referencia (o al percentil 99 si max_as_percentile = TRUE). 
-    Todo punto en la distribución de dosis con un valor menor al umbral
-    de dosis, es excluido del análisis.
-    
-dose_t_Gy : bool, default: False
-    Si el argumento es True, entonces "dose_t" (la dosis de tolerancia) se interpreta como un valor fijo y absoluto en Gray [Gy].
-    Si el argumento es False (default), "dose_t" se interpreta como un porcentaje.
-
-local_norm : bool, default: False
-    Si el argumento es True (normalización local), el porcentaje de dosis de tolerancia "dose_t" se interpreta con respecto a la dosis local
-    en cada punto de la distribución de referencia.
-    Si el argumento es False (normalización global), el porcentaje de dosis de tolerancia "dose_t" se interpreta con respecto al máximo de la distribución a evaluar.
-    Notas:
-        1.- Los argumentos dose_t_Gy y local_norm NO deben ser seleccionados como True de forma simultánea.
-        2.- Si se desea utilizar directamente el máximo de la distirbución, utilizar el parámetro max_as_percentile = False (ver explicación mas adelante).
-
-mask_radius : float, default: 10
-    Distancia física en milímetros que se utiliza para acotar el cálculo con posiciones que estén dentro de una vecindad dada por mask_radius.
-
-    Para lo anterior, se genera un área de busqueda cuadrada o "máscara" aldrededor de cada punto o posición en la distribución de referencia.
-    El uso de esta máscara permite reducir el tiempo de cálculo debido al siguiente proceso:
-        Por cada punto en la distribución de referencia, el cálculo de la función Gamma se realiza solamente
-        con aquellos puntos o posiciones de la distribución a evaluar que se encuentren a una distancia relativa
-        menor o igual a mask_radius, es decir, con los puntos que están dentro de la vecindad dada por mask_radius.
-        La longitud de uno de los lados de la máscara cuadrada es de 2*mask_radius + 1.
-    Por otro lado, si se prefiere comparar con todos los puntos de la distribución a evaluar, es suficiente con ingresar
-    una distancia mayor a las dimensiones de la distribución de dosis (por ejemplo mask_radius = 1000).
+        if max_as_percentile:
+            maximum_dose = np.percentile(D_eval, 99)
+        else:
+            maximum_dose = np.amax(D_eval)
+        print(f'Dosis máxima: {maximum_dose:.1f}')
+        #  Umbral de dosis
+        Dose_threshold = (dose_tresh/100)*maximum_dose
+        print(f'Umbral de dosis: {Dose_threshold:.1f}')
 
-max_as_percentile : bool, default: True
-    -> Si el argumento es True, se utiliza el percentil 99 como una aproximación del valor máximo de la
-        distribución de dosis. Lo anterior permite excluir artefactos o errores en posiciones puntuales
-        (de utilidad por ejemplo cuando se utiliza película radiocrómica o etiquetas puntuales en la distribución).
-    -> Si el argumento es False, se utiliza directamente el valor máximo de la distribución a evaluar.
+        #   Dosis de tolerancia absoluta o relativa
+        if dose_t_Gy:
+            pass
+        elif local_norm:
+            pass
+        else:
+            dose_t = (dose_t/100) * maximum_dose
 
-Retorno
-----------
-ndarray :
-    Array, o matriz bidimensional con la distribución de índices gamma.
+        #   Número de pixeles que se usarán para definir una vecindad sobre la que se calculará el índice gamma.
+        neighborhood = round(mask_radius*1./self.resolution)
 
-float :
-    Índice de aprobación. Se calcula como el porcentaje de valores gamma <= 1, sin incluir las posiciones
-    en donde la dosis es menor al umbral de dosis.
+        #   Matriz que guardará el resultado del índice gamma.
+        gamma = np.zeros( (self.rows, self.columns) )
 
-Consideraciones
-----------
-      Es posible utilizar el percentil 99.1 de la distribución de dosis como una aproximación del valor máximo.
-      Esto permite evitar la posible inclusión de artefactos o errores en posiciones puntuales de la distribución
-      (de utilidad por ejemplo cuando se utiliza película radiocrómica o etiquetas puntuales en la distribución).
 
-      Se asume que ambas distribuciones a evaluar representan exactamente las mismas dimensiones físicas, y las posiciones
-      espaciales para cada punto conciden entre ellas, es decir, las imagenes de cada distribución están registradas.
 
-      No se realiza interpolación entre puntos.
 
+        #%%
+        for i in np.arange( D_ref.shape[0] ):
+            #   Código que permite incluir puntos cerca de la frontera de la distribución de dosis
+            mi = -(neighborhood - max(0, neighborhood - i))
+            mf = neighborhood - max(0, neighborhood - (D_eval.shape[0] - (i+1))) + 1
 
+            for j in np.arange( D_ref.shape[1] ):
+                ni = -(neighborhood - max(0, neighborhood - j))
+                nf = neighborhood - max(0, neighborhood - (D_eval.shape[1] - (j+1))) + 1
 
-```
+                #   Para almacenar temporalmente los valores de la función Gamma por cada punto en la distribución de referencia
+                Gamma = []
 
-Funciones
-```
+                for m in np.arange(mi , mf):
+                    for n in np.arange(ni, nf):
 
-Dosepy.dose.from_csv(file_name, PixelSpacing)
+                        # Distancia entre dos posiciones (en milímetros), por fila
+                        dm = m*self.resolution
+                        # Distancia entre dos posiciones (en milímetros), por columna
+                        dn = n*self.resolution
+                        # Distancia total entre dos puntos
+                        distance = np.sqrt(dm**2 + dn**2)
 
-    Importación de un archivo de dosis en formato CSV (Comma separated values).
-    Dentro del archivo .csv, utilizar el caracter # al inicio de una fila para
-    que sea descartada (inicio de un comentario).
+                        # Diferencia en dosis
+                        dose_dif = D_eval[i + m, j + n] - D_ref[i,j]
 
-    Parameters
-    -----------
-    file_name : str
-        Nombre del archivo en formato string
 
-    PixelSpacing : float
-        Distancia entre dos puntos consecutivos, en milímetros
+                        if local_norm:
+                            # La dosis de tolerancia se actualiza al porcentaje con respecto al valor
+                            # de dosis local en la distribución de referencia.
+                            dose_t_local = dose_t * D_ref[i,j] / 100
 
-    Return
-    --------
-    Dosepy.dose.Dose
-        Objeto Dose del paquete Dosepy que representa a la distribución de dosis.
+                            Gamma.append(
+                                np.sqrt(
+                                    (distance**2) / (dist_t**2)
+                                    + (dose_dif**2) / (dose_t_local**2))
+                                        )
+
+                        else :
+                            Gamma.append(
+                                np.sqrt(
+                                    (distance**2) / (dist_t**2)
+                                    + (dose_dif**2) / (dose_t**2))
+                                        )
 
+                gamma[i,j] = min(Gamma)
 
+                # Para la posición en cuestión, si la dosis es menor al umbral de dosis,
+                # entonces dicho punto no se toma en cuenta en el porcentaje de aprobación.
+                if D_eval[i,j] < Dose_threshold:
+                    gamma[i,j] = np.nan
 
-Dosepy.dose.from_dicom(file_name)
+        # Arroja las coordenadas en donde los valores gamma son menor o igual a 1
+        less_than_1_coordinate = np.where(gamma <= 1)
+        # Cuenta el número de coordenadas en donde se cumple que gamma <= 1
+        less_than_1 = np.shape(less_than_1_coordinate)[1]
+        # Número de valores gamma diferentes de np.nan
+        total_points = np.shape(gamma)[0]*np.shape(gamma)[1] - np.shape(np.where(np.isnan(gamma)))[1]
 
+        #   Índice de aprobación
+        gamma_percent = float(less_than_1)/total_points*100
+        return gamma, gamma_percent
+
+def from_dicom(file_name):
+    """
     Importación de un archivo de dosis en formato DICOM
 
     Parameters
-    -----------
+    ----------
     file_name : str
         Nombre del archivo en formato string
 
-    Return
-    --------
+    Returns
+    -------
+
     Dosepy.dose.Dose
         Objeto Dose del paquete Dosepy que representa a la distribución de dosis
 
-    Consideraciones
-    ----------------
-        La distribución de dosis en el archivo DICOM debe contener solo dos dimensiones.
-        La resolución espacial debe de ser igual en ambas dimensiones.
-        No se utilizan las coordenadas dadas en el archivo DICOM. Ver segunda consideración en la nota del método gamma2D de la clase Dose.
-
+    Notes
+    -----
 
+    La distribución de dosis en el archivo DICOM debe contener solo dos dimensiones.
+    La resolución espacial debe de ser igual en ambas dimensiones.
+    No se hace uso de las coordenadas dadas en el archivo DICOM. Ver segunda consideración en la nota del método gamma2D de la clase Dose.
 
-Dosepy.tools.resol.equalize(array, resol_array, resol_ref)
     """
-    Función que permite reducir el número de filas y columnas de una matriz (array) para igualar su resolución espacial (mm/punto) con respecto a una resolución de referencia.
-    Para lo anterior, se calcula un promedio de varios puntos y se asigna a un nuevo punto con una mayor dimensión espacial.
-
-    Parameters:
-    -----------
-    array: ndarray
-        Matriz a la que se le requiere reducir el tamaño.
-
-    resol_array: float
-        Resolución espacial de la matriz, en milímetros por punto.
+    DS = pydicom.dcmread(file_name)
+    array = DS.pixel_array
+    #image_orientation = DS.ImageOrientationPatient
+    if array.ndim != 2:
+        raise Exception("La distribución de dosis debe de ser en dos dimensiones")
+    dgs = DS.DoseGridScaling
+    D_array = array * dgs
+    resolution = DS.PixelSpacing
+    if resolution[0] != resolution[1]:
+        raise Exception("La resolución espacial debe ser igual en ambas dimensiones.")
 
-    resol_ref: float
-        Resolución espacial de referencia, en milímetros por punto.
+    Dose_DICOM = Dose(D_array, resolution[0])
+    return Dose_DICOM
 
-    Return:
-  	-------
-    array: ndarray
-  			Matriz reducida en su número de filas y columnas.
 
-    Ejemplo:
-    --------
-
-    Sean A y B dos matrices de tamaño (2362 x 2362) y (256 x 256), con
-    resolución espacial de 0.0847 mm/punto y 0.7812 mm/punto, respectivamente.
-
-    La dimensión espacial de la matriz A es de 200.06 mm
-    (2362 puntos * 0.0847 mm/punto = 200.06 mm)
-    La dimensión espacial de la matriz B es de 199.99 mm.
-    (256 puntos * 0.7812 mm/punto = 199.99 mm)
-
-    Para reducir el tamaño de la matriz A e igualarla al tamaño de la
-    matriz B, se utiliza la función equalize:
-
-        import Dosepy.tools.resol as resol
-        import numpy as np
+def from_csv(file_name, PixelSpacing):
+    """
+    Importación de un archivo de dosis en formato CSV (Comma separated values).
+    Dentro del archivo .csv, utilizar el caracter # al inicio de una fila para
+    que sea descartada (inicio de un comentario).
 
-        A = np.zeros( (2362, 2362) )
+    Parameters
+    -----------
+    file_name : str
+        Nombre del archivo en formato string
 
-        C = resol.equalize(A, 0.0847, 0.7812)
-        C.shape
-        # (256, 256)
+    PixelSpacing : float
+        Distancia en milímetros entre dos puntos consecutivos.
 
+    Returns
+    -------
+    Dosepy.dose.Dose
+        Objeto Dose del paquete Dosepy que representa a la distribución de dosis.
 
     """
-```
-
-**Presentación en eventos científicos**
-
-* (2021) 7mo Congreso de la Federación Mexicana de Organizaiones de Física Médica, "Desarrollo y validación de un software de código abierto para la comparación de distribuciones de dosis usadas en radioterapia" [(Video disponible)](https://youtu.be/HM4qkYGzNFc)
 
-# Advertencia
-El correcto funcionamiento del paquete se está evaluado y actualizado constantemente. Sin embargo, no se tiene garantía de que el código del paquete esté libre de errores o bugs. El usuario es el único responsable por utilizar *Dosepy*.
+    array = np.genfromtxt(file_name, delimiter = ",", comments = "#")
+    Dose_csv = Dose(array, PixelSpacing)
+    return Dose_csv
 
-# Licencia
 
-PROPRIETARY LICENSE
+#%%
+def main():
 
-Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
-03-2021-093012460400-01
+    "Bloque de código para realizar pruebas"
 
-CONDICIONES
+    D_eval = from_csv("D_TPS.csv", 1)
+    D_ref = from_csv("D_FILM.csv", 1)
 
-Toda persona tiene acceso al código solamente con fines académicos o de enseñanza. Cualquier otro uso del código DOSEPY
-requiere de una licencia para su uso particular, conocida como "Acuerdo de licencia de usuario final" (EULA, por sus siglas en inglés).
+    g, pass_percent = D_eval.gamma2D(D_ref, dose_t=3, dist_t=2)
 
-El código o software derivado, tales como arreglos, compendios, ampliaciones, traducciones, adaptaciones,
-paráfrasis, compilaciones, colecciones y transformaciones del software DOSEPY, podrán ser explotadas
-cuando hayan sido autorizadas por el titular del derecho patrimonial sobre la obra DOSEPY,
-previo consentimiento del titular del derecho moral, en los casos previstos en la Fracción III
-del Artículo 21 de la Ley Federal del Derecho de Autor.
+    print(f'El índice de aprobación es: {pass_percent:.1f} %')
+    plt.imshow(g, vmax = 1.4)
+    plt.show()
 
-GARANTÍA
+#%%
 
-El software Dosepy se ofrece sin ninguna garantía de cualquier tipo. Su uso es responsabilidad del usuario.
+if __name__ == "__main__":
+    main()
```

### Comparing `Dosepy-0.3.9/pyproject.toml` & `Dosepy-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Dosepy"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Gamma analysis and film dosimetry for dose distributions in radiotherapy"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
@@ -29,15 +29,15 @@
 dependencies = [
   "numpy >= 1.23.4",
   "pydicom >= 2.3.0",
   "matplotlib >= 3.6.1",
   "tifffile >= 2022.10.10",
   "scipy >= 1.9.3",
   "PyQt6 >= 6.5.1",
-  "relative_dose_1d >= 0.1.4"
+  "relative_dose_1d >= 0.1.7"
 ]
 [project.urls]
 homepage = "https://dosepy.readthedocs.io/en/latest/intro.html"
 repository = "https://pypi.org/project/Dosepy/"
 Bug-Tracker = "https://github.com/LuisOlivaresJ/Dosepy"
 
 [tool.setuptools.packages.find]
```

### Comparing `Dosepy-0.3.9/src/Dosepy/GUI.py` & `Dosepy-0.4.0/src/Dosepy/GUILayouts/Bloque_Imagenes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,349 +1,402 @@
-# -*- coding: utf-8 -*-
-"""
-@author:
-    Luis Alfonso Olivares Jimenez
-    Maestro en Ciencias (Física Médica)
-    Físico Médico, La Paz, Baja California Sur, México.
+#%%
+#   Para mostrar distribuciones de dosis y perfiles
 
-    Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
-"""
+
+#%%
 #---------------------------------------------
+
 #   Importaciones
 
+#---------------------------------------------
+
+from matplotlib import patches
+from PyQt6.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
 import sys
-from PyQt6.QtWidgets import QWidget, QVBoxLayout, QApplication, QHBoxLayout, QMessageBox, QMainWindow, QLabel, QLineEdit
-from PyQt6.QtGui import QIcon, QFont,  QAction
-from PyQt6.QtCore import Qt
-
-from PyQt6.QtWidgets import QFileDialog, QInputDialog
-from relative_dose_1d.tools import build_from_array_and_step, gamma_1D
-#from relative_dose_1d.GUI import Q_Graphic_Block
+import pkg_resources
+from matplotlib.figure import Figure
+from matplotlib.backends.backend_qtagg import FigureCanvas
+import matplotlib.colors as colors
+import numpy as np
+#from PyQt5.QtGui import QIcon
+import Dosepy.dose as dp
 
 
 
-import numpy as np
-from Dosepy.GUILayouts.Bloque_gamma import Bloque_gamma
-#from GUILayouts.Bloque_gamma import Bloque_gamma  # Se importa desde archivo en PC para testear
-from Dosepy.GUILayouts.Bloque_Imagenes import Bloque_Imagenes
-#from GUILayouts.Bloque_Imagenes import Bloque_Imagenes   # Se importa desde archivo en PC para testear
-import Dosepy.dose as dp
-import matplotlib as mpl
-import pkg_resources
+#%%
+#########################################################
+#---------------------------------------------
+
+#   Cuerpo de la app
 
-from Dosepy.GUILayouts.film_to_doseGUI import Film_to_Dose_Window
-#from GUILayouts.film_to_doseGUI import Film_to_Dose_Window
-from Dosepy.GUILayouts.about_window import About_Window
-#from GUILayouts.about_window import About_Window
-from Dosepy.GUILayouts.licencia_window import Licencia_Window
-#from GUILayouts.licencia_window import Licencia_Window
 #---------------------------------------------
 
+class Bloque_Imagenes(QWidget):
+    def __init__(self):
+        super().__init__()  #   Llamar al constructor de QWidget
+        self.iniciarUI()
 
-class VentanaPrincipal(QMainWindow):
-    """
-    Ventana principal
-    """
-    def __init__(self, Us):
-        super().__init__()
-        self.Us = Us
-        self.setStyleSheet("background-color: whitesmoke;")
-        #self.setStyleSheet("background-color: #1d1040;")
-        self.setWindowTitle('Dosepy')
-        file_name_icon = pkg_resources.resource_filename('Dosepy', 'Icon/Icon.png')
-        self.setWindowIcon(QIcon(file_name_icon))
-        self.setGeometry(150, 100, 1300, 800)
+    def iniciarUI(self):
+        self.IniciarWidgets()
+
+
+    def IniciarWidgets(self):
 
-        self.cuerpoUI()
-        self.menuUI()
+#%%
+        #   Widget para imagen de referencia
 
-        #Ventanas secundarias
-        self.film_to_dose_window = None
-        self.about_window = None
-        self.licencia_window_sec = None
+        file_name_FILM = pkg_resources.resource_filename('Dosepy', 'data/D_FILM.csv')
+        file_name_TPS = pkg_resources.resource_filename('Dosepy', 'data/D_TPS.csv')
 
-        self.show()
+        self.D_ref = dp.from_csv(file_name_FILM, 1)
+        self.D_eval = dp.from_csv(file_name_TPS, 1)
 
-    def cuerpoUI(self):
+        self.Mpl_Izq = Qt_Figure_Imagen()
+        self.Mpl_Der = Qt_Figure_Imagen()
 
-        cuerpo = QWidget()
-        self.Bloque_Imagen = Bloque_Imagenes()
+        self.Mpl_Izq.ax1.set_title('Referencia', fontsize = 10, loc = 'left')
+        self.Mpl_Der.ax1.set_title('A evaluar', fontsize = 10, loc = 'left')
 
+        self.Mpl_Izq.Img(self.D_ref)
+        self.Mpl_Der.Img(self.D_eval)
 
-        self.Bloque_Imagen.boton_recortar_Izq.clicked.connect(self.Cortar_Imagen)
-        self.Bloque_Imagen.compare_button.clicked.connect(self.Compare_profiles)
+        self.Mpl_Izq.Colores(self.D_ref.array)
+        self.Mpl_Der.Colores(self.D_eval.array)
 
-        self.Bloque_Gamma = Bloque_gamma(self.Us)
-        self.Bloque_Gamma.Eval_button.clicked.connect(self.mostrar_distribucion)
-        self.Bloque_Gamma.Calcular_Button.clicked.connect(self.Calculo_Gamma)
+        self.Mpl_Izq.hline.set_linestyle('-')
+        self.Mpl_Izq.vline.set_linestyle('-')
 
-        LayoutPrincipal = QVBoxLayout()
-        LayoutPrincipal.addWidget(self.Bloque_Gamma)
-        LayoutPrincipal.addWidget(self.Bloque_Imagen)
+        self.Mpl_Der.circ.set_visible(False)
 
-        #self.setLayout(LayoutPrincipal)
-        cuerpo.setLayout(LayoutPrincipal)
+        #self.Mpl_Izq.Cross_Hair_off()
+        #self.Mpl_Der.Cross_Hair_off()
 
-        self.setCentralWidget(cuerpo)
+        self.id_on_press_perfil = self.Mpl_Izq.Qt_fig.figure.canvas.mpl_connect('button_press_event', self.on_press_img_ref)            # Controlar si hay eventos y acciones
+        self.id_on_release_perfil = self.Mpl_Izq.Qt_fig.figure.canvas.mpl_connect('button_release_event', self.on_release_img_ref)
+        self.id_on_move_perfil = self.Mpl_Izq.Qt_fig.figure.canvas.mpl_connect('motion_notify_event', self.on_move_img_ref)
+        self.pressevent = None
 
-    def menuUI(self):
+        #   Widget para los perfiles
+        self.Mpl_perfiles = Qt_Figure_Perfiles()
+        self.Mpl_perfiles.set_data_and_plot(self.Mpl_Izq.npI, self.Mpl_Der.npI, self.Mpl_Izq.circ)
+
+        #   Widgets para los botones
+        self.boton_roi = QPushButton('ROI')
+        #self.boton_roi.resize(150,50)
+        self.boton_roi.setCheckable(True)
+        self.boton_roi.setChecked(False)
+        self.boton_roi.clicked.connect(self.clic_ROI)
+
+        #corte_icon = QIcon("../Icon/cut_icon.png")
+        #corte_name_folder = pkg_resources.resource_filename('Dosepy', 'Icon/cut_icon.png')
+        self.boton_recortar_Izq = QPushButton('Corte')
+        #self.boton_recortar_Izq.setIcon(corte_icon)
+        self.boton_recortar_Izq.setEnabled(False)
+
+        self.compare_button = QPushButton("H. Profile")
+
+        #self.boton_exportar_Izq = QPushButton('Exportar')
+        self.boton_exportar_Der = QPushButton('')
+        #self.boton_exportar_perfiles = QPushButton('Exportar')
+
+        #   Contenedores
         """
-        Crear un menú para la aplicación
+        layout_hijo_Izq = QHBoxLayout()
+        layout_hijo_Izq.addWidget(self.boton_roi)
+        layout_hijo_Izq.addWidget(self.boton_recortar_Izq)
+        #layout_hijo_Izq.addWidget(self.boton_exportar_Izq)
+        layout_hijo_Izq.addStretch()
+
+        layout_hijo_Der = QHBoxLayout()
+        layout_hijo_Der.addWidget(self.boton_exportar_Der)
+        layout_hijo_Der.addStretch()
+
+        layout_hijo_perfiles = QHBoxLayout()
+        #layout_hijo_perfiles.addWidget(self.boton_exportar_perfiles)
+        layout_hijo_perfiles.addStretch()
         """
-        # Crear acciones para el menú "Herramientas"
-        film_to_dose_action = QAction('Dosimetría con película', self)
-        film_to_dose_action.setShortcut('Ctrl+F')
-        film_to_dose_action.triggered.connect(self.film_to_dose)   #   Descomentar para desarrollo
-
-        about_action = QAction('Acerca de...', self)
-        about_action.triggered.connect(self.about_ventana)
-
-        licencia_action = QAction('Licencia', self)
-        licencia_action.triggered.connect(self.licencia_ventana)
-
-        # Crear barra del menu
-        barra_menu = self.menuBar()
-        barra_menu.setNativeMenuBar(False)
-
-        # Agregar menú herramientas y su acción a la barra del menú
-        herram_menu = barra_menu.addMenu('Herramientas')
-        herram_menu.addAction(film_to_dose_action)
-        about_menu = barra_menu.addMenu('Ayuda')
-        about_menu.addAction(about_action)
-        about_menu.addAction(licencia_action)
-        #licencia_action
-        #about_manu.AddAction(licencia_action)
-
-
-######################################################################
-#   Funciones para menu herramientas
-
-    def film_to_dose(self):
-        if self.film_to_dose_window == None:
-            self.film_to_dose_window = Film_to_Dose_Window()
-        self.film_to_dose_window.show()
-
-    def about_ventana(self):
-        if self.about_window == None:
-            self.about_window = About_Window()
-        self.about_window.show()
-
-    def licencia_ventana(self):
-        if self.licencia_window_sec == None:
-            self.licencia_window_sec = Licencia_Window()
-        self.licencia_window_sec.show()
-
-######################################################################
-#   Funciones para botones
-
-    def mostrar_distribucion(self):
-        if self.Bloque_Gamma.Formatos_ok == True:   # ¿Los archivos cumplen con las especificaciones?
-            self.Bloque_Imagen.Mpl_Izq.Img(self.Bloque_Gamma.Refer_npy)
-            self.Bloque_Imagen.Mpl_Izq.Colores(self.Bloque_Gamma.Eval_npy)
-
-            self.Bloque_Imagen.Mpl_Der.Img(self.Bloque_Gamma.Eval_npy)
-            self.Bloque_Imagen.Mpl_Der.Colores(self.Bloque_Gamma.Eval_npy)
+        layout_padre_botones = QVBoxLayout()
+        layout_padre_botones.addWidget(self.boton_roi)
+        layout_padre_botones.addWidget(self.boton_recortar_Izq)
+        layout_padre_botones.addWidget(self.compare_button)
+
+        layout_padre_botones.addStretch()
 
-            self.Bloque_Imagen.Mpl_perfiles.ax.clear()
-            self.Bloque_Imagen.Mpl_perfiles.set_data_and_plot(self.Bloque_Gamma.Refer_npy, self.Bloque_Gamma.Eval_npy, self.Bloque_Imagen.Mpl_Izq.circ)
+        layout_padre_Izq = QVBoxLayout()
+        #layout_padre_Izq.addLayout(layout_hijo_Izq)
+        layout_padre_Izq.addWidget(self.Mpl_Izq.Qt_fig)
 
-            self.Bloque_Imagen.Mpl_Izq.fig.canvas.draw()
-            self.Bloque_Imagen.Mpl_Der.fig.canvas.draw()
+        layout_padre_Der = QVBoxLayout()
+        #layout_padre_Der.addLayout(layout_hijo_Der)
+        layout_padre_Der.addWidget(self.Mpl_Der.Qt_fig)
+
+        layout_padre_perfiles = QVBoxLayout()
+        #layout_padre_perfiles.addLayout(layout_hijo_perfiles)
+        layout_padre_perfiles.addWidget(self.Mpl_perfiles.Qt_fig)
+
+        layout_abuelo = QHBoxLayout()
+        layout_abuelo.addLayout(layout_padre_botones)
+        layout_abuelo.addLayout(layout_padre_Izq)
+        layout_abuelo.addLayout(layout_padre_Der)
+        layout_abuelo.addLayout(layout_padre_perfiles)
+
+        self.setLayout(layout_abuelo)
+
+
+###############################################################################################
+#---------------------------------------------
+
+        #   Funciones de la app
+
+    def on_press_img_ref(self, event):
+
+        if self.boton_roi.isChecked():
+            if event.inaxes != self.Mpl_Izq.ax1:
+                return
+            #   Codigo para generar ROI rectangular
+            self.Mpl_Izq.ROI_Rect_set_up(event)
+            self.pressevent = event
 
-            self.Bloque_Imagen.Mpl_perfiles.fig.canvas.draw()
 
         else:
-            self.displayMessageBox()
+            if event.inaxes != self.Mpl_Izq.ax1:    #   ¿El axes donde se creó el evento es diferente que el axes de la imagen de referencia?
+                return
 
-    def Calculo_Gamma(self):
-        D_ref = dp.Dose(self.Bloque_Imagen.Mpl_Izq.npI, float(self.Bloque_Gamma.Resolution.text()))
-        D_eval = dp.Dose(self.Bloque_Imagen.Mpl_Der.npI, float(self.Bloque_Gamma.Resolution.text()))
-        g, p = D_eval.gamma2D(D_ref, float(self.Bloque_Gamma.Toler_dosis.text()), float(self.Bloque_Gamma.Toler_dist.text()), float(self.Bloque_Gamma.Umbral_dosis.text()))
-
-        self.Bloque_Gamma.Mpl_Histograma.Mostrar_Histograma(g)
-        self.Bloque_Gamma.Indice_gamma_porcentaje_Label.setText('Porcentaje de aprobación: ' + str(  round(p, 1)  ) + '%' )
-        self.Bloque_Gamma.Indice_gamma_promedio_Label.setText('Índice gamma promedio: ' + str(  round(np.mean(g[~np.isnan(g)]), 1)  ))
-        #self.Bloque_Gamma.Indice_gamma_maximo_Label.setText('Máximo: ' + str(  round(np.max(g[~np.isnan(g)]), 1)  ))
-        #self.Bloque_Gamma.Indice_gamma_mediana_Label.setText('Mediana: ' + str(  round(np.median(g[~np.isnan(g)]), 1)  ))
-
-        self.Bloque_Gamma.Mpl_Img_gamma.ax1.clear()
-        self.Bloque_Gamma.Mpl_Img_gamma.ax2.clear()
-        self.Bloque_Gamma.Mpl_Img_gamma.Img(g)
-        self.Bloque_Gamma.Mpl_Img_gamma.ax2.get_yaxis().set_visible(True)
-        self.Bloque_Gamma.Mpl_Img_gamma.ax1.set_title('Distribución gamma', fontsize = 11)
-        self.Bloque_Gamma.Mpl_Img_gamma.Colores(g[~np.isnan(g)])
-
-        viridis = mpl.cm.get_cmap('viridis',256)
-        hot = mpl.cm.get_cmap('hot',256)
-
-        bounds_gamma = np.linspace(0,1.5,16)
-        norm_gamma = mpl.colors.BoundaryNorm(boundaries = bounds_gamma, ncolors = 16)
-
-        new_viridis = viridis(np.linspace(0,1,10))
-        new_hot = np.flip(   hot(np.linspace(0,1,40)), 0   )
-        new_hot = new_hot[20:26, :]
-        new_color_gamma = np.vstack((new_viridis, new_hot))
-        new_cmp_gamma = mpl.colors.ListedColormap(new_color_gamma)
-        self.Bloque_Gamma.Mpl_Img_gamma.mplI.set_norm(norm_gamma)
-        self.Bloque_Gamma.Mpl_Img_gamma.mplI.set_cmap(new_cmp_gamma)
-
-       # I_g = self.Bloque_Gamma.Mpl_Img_gamma.ax1.pcolormesh(g, cmap = new_cmp_gamma, norm = norm_gamma)
-        #cbar_gamma = self.Bloque_Gamma.Mpl_Img_gamma.colorbar(I_g, orientation='vertical', shrink = 0.6, cax = self.Bloque_Gamma.Mpl_Img_gamma.axe2)
-        #cbar_gamma.ax.set_ylabel('Índice gamma', rotation=90, fontsize= 11)
-
-        #self.Bloque_Gamma.Mpl_Img_gamma.Mostrar_Imagen(g)
-        self.Bloque_Gamma.Mpl_Histograma.fig.canvas.draw()
-        self.Bloque_Gamma.Mpl_Img_gamma.fig.canvas.draw()
-
-
-
-    def Cortar_Imagen(self):
-
-        xi = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_x())
-        width = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_width())
-        yi = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_y())
-        height = int(self.Bloque_Imagen.Mpl_Izq.Rectangle.get_height())
-
-        npI_Izq = self.Bloque_Imagen.Mpl_Izq.npI[  yi : yi + height , xi : xi + width ]
-        npI_Der = self.Bloque_Imagen.Mpl_Der.npI[  yi : yi + height , xi : xi + width ]
-        self.Bloque_Imagen.D_ref = dp.Dose(npI_Izq, self.Bloque_Imagen.D_ref.resolution)
-        self.Bloque_Imagen.D_eval = dp.Dose(npI_Der, self.Bloque_Imagen.D_eval.resolution)
-
-        self.Bloque_Imagen.Mpl_Izq.Img(self.Bloque_Imagen.D_ref)
-        self.Bloque_Imagen.Mpl_Der.Img(self.Bloque_Imagen.D_eval)
-
-        self.Bloque_Imagen.Mpl_Izq.Colores(npI_Der)
-        self.Bloque_Imagen.Mpl_Der.Colores(npI_Der)
-
-        self.Bloque_Imagen.Mpl_Izq.Cross_Hair_on()
-        self.Bloque_Imagen.Mpl_Der.Cross_Hair_on()
-
-        self.Bloque_Imagen.Mpl_perfiles.set_data_and_plot(npI_Izq, npI_Der, self.Bloque_Imagen.Mpl_Izq.circ)
-
-        self.Bloque_Imagen.Mpl_Izq.ROI_Rect_off()
-        self.Bloque_Imagen.boton_recortar_Izq.setEnabled(False)
-        self.Bloque_Imagen.boton_roi.setChecked(False)
-
-    def Compare_profiles(self):
-
-        resolution = self.Bloque_Imagen.D_ref.resolution
-
-        D_profile_ref = build_from_array_and_step(
-            self.Bloque_Imagen.Mpl_perfiles.perfil_horizontal_ref,
-            resolution
-            )
-        D_profile_eval = build_from_array_and_step(
-            self.Bloque_Imagen.Mpl_perfiles.perfil_horizontal_eval,
-            resolution
-            )
-        
-        gamma, gamma_percent = gamma_1D(
-            D_profile_ref, 
-            D_profile_eval,
-            dose_t = 3, dist_t = 2, dose_tresh = 10, interpol = 1)
-        #print(gamma)
-        print(gamma_percent)
-
-        # TO_DO 
-        # gamma_1D requieres data to be normalized
-        # new fuction inside relative_dose_1d to whow a plot 
-        # plot_gamma_profiles() 
-
-
-######################################################################
-#   Ventanas para mensajes
-    def displayMessageBox(self):
-        """
-        Si la variable self.Bloque_Gamma.Formatos_ok es True, los archivos
-        para las distribuciones de dosis se cargaron correctamente.
-        En caso contrario se emite un mensaje de error.
-        """
-        QMessageBox().critical(self, "Error", "Error con la lectura de archivos.", QMessageBox.Ok, QMessageBox.Ok)
+            if not self.Mpl_Izq.circ.contains(event)[0]:    #   ¿El evento se creó fuera del patch?
+                return
 
-class Ventana_Secundaria(QMainWindow):
-    'Clase para mantenimiento de Dosepy'
-    def __init__(self):
-        super().__init__()
+            self.pressevent = event
 
-        self.about_window_sec = None
-        self.licencia_window_sec = None
+    def on_release_img_ref(self, event):
+        self.pressevent = None
 
-        self.iniciarUI()
-        self.menu_ayuda()
-        #self.setCentralWidget(cuerpo_sec)
+        if self.boton_roi.isChecked():
+            return
 
-    def iniciarUI(self):
 
-        cuerpo = QWidget()
-        layout_principal = QVBoxLayout()
-        cuerpo.setLayout(layout_principal)
-        self.setCentralWidget(cuerpo)
-
-        self.setStyleSheet("background-color: whitesmoke;")
-        self.setWindowTitle('Dosepy')
-        file_name_icon = pkg_resources.resource_filename('Dosepy', 'Icon/Icon.png')    #   Obtenido desde paquete Dosepy
-        self.setWindowIcon(QIcon(file_name_icon))
-
-        label_usuario = QLabel(self)
-        label_usuario.setText('Ingrese clave de acceso:')
-        label_usuario.move(80, 20)
-        layout_principal.addWidget(label_usuario)
-        label_usuario.setFont(QFont('Arial', 14))
-
-        self.name_entry = QLineEdit(self)
-        self.name_entry.setFont(QFont('Arial', 18))
-        self.name_entry.setEchoMode(QLineEdit.Password)
-        self.name_entry.setAlignment(Qt.AlignmentFlag.AlignHCenter)
-
-        self.name_entry.returnPressed.connect(self.cerrar_UI)
-        self.name_entry.move(100, 70)
-        layout_principal.addWidget(self.name_entry)
-        layout_principal.setSpacing(10)
-        self.show()
-
-    def cerrar_UI(self):
-        if self.name_entry.text() == 'self':
-            #self.close()
-            self.Us = 'P'
-            self.window = VentanaPrincipal(self.Us)
         else:
-            self.Us = 'O'
-            self.window = VentanaPrincipal(self.Us)
+            self.Mpl_Izq.x0, self.Mpl_Izq.y0 = self.Mpl_Izq.circ.center
+            self.Mpl_Der.x0, self.Mpl_Der.y0 = self.Mpl_Der.circ.center
 
-    def menu_ayuda(self):
-        """
-        Crear un menú de ayuda
-        """
-        # Crear acciones para el menú "Herramientas"
 
-        about_action_secundaria = QAction('Acerca de', self)
-        about_action_secundaria.triggered.connect(self.about_ventana)
+    def on_move_img_ref(self, event):
+
+        if self.boton_roi.isChecked():
+            #   Código para generar ROI rectangular
+
+            if self.pressevent is None or event.inaxes != self.pressevent.inaxes:
+                return
+
+            dx = abs(event.xdata - self.pressevent.xdata)
+            dy = abs(event.ydata - self.pressevent.ydata)
+            x_i = min(event.xdata, self.pressevent.xdata)
+            y_i = min(event.ydata, self.pressevent.ydata)
+            self.Mpl_Izq.Rectangle.set_bounds(x_i, y_i, dx, dy)
+            self.boton_recortar_Izq.setEnabled(True)
+            #print(self.Mpl_Izq.Rectangle.properties())
+            self.Mpl_Izq.fig.canvas.draw()
+
+
+        else:
+            #   Código para generar cross hair y perfiles
+
+            if self.pressevent is None or event.inaxes != self.pressevent.inaxes:
+                return
+
+            dx = event.xdata - self.pressevent.xdata
+            dy = event.ydata - self.pressevent.ydata
+            self.Mpl_Izq.circ.center = self.Mpl_Izq.x0 + dx, self.Mpl_Izq.y0 + dy
+            self.Mpl_Der.circ.center = self.Mpl_Der.x0 + dx, self.Mpl_Der.y0 + dy
+
+            self.Mpl_Izq.Cross_Hair_set_up()
+            self.Mpl_Der.Cross_Hair_set_up()
 
-        licencia_action_secundaria = QAction('Licencia', self)
-        licencia_action_secundaria.triggered.connect(self.licencia_ventana)
+            self.Mpl_perfiles.set_data_and_plot(self.Mpl_Izq.npI, self.Mpl_Der.npI, self.Mpl_Izq.circ)
 
-        # Crear barra del menu
-        barra_menu_sec = self.menuBar()
-        barra_menu_sec.setNativeMenuBar(False)
+            self.Mpl_Izq.fig.canvas.draw()
+            self.Mpl_Der.fig.canvas.draw()
 
-        # Agregar menú herramientas y su acción a la barra del menú
 
-        ayuda_menu_sec = barra_menu_sec.addMenu('Ayuda')
-        ayuda_menu_sec.addAction(about_action_secundaria)
-        ayuda_menu_sec.addAction(licencia_action_secundaria)
+ #%%
+
+    def clic_ROI(self):
+
+        if self.boton_roi.isChecked():
+            #   Código para el ROI
+            self.Mpl_Izq.Cross_Hair_off()
+            self.Mpl_Der.Cross_Hair_off()
+
+
+        else :
+            #   Código para el cross
+
+            self.Mpl_Izq.ROI_Rect_off()
+            self.Mpl_Izq.Cross_Hair_on()
+            self.Mpl_Der.Cross_Hair_on()
+
+            self.boton_recortar_Izq.setEnabled(False)
+
+
+#%%
+class Qt_Figure_Imagen:
+    """
+    Clase para contener la distribución de dosis
+    """
+
+    def __init__(self):
+        self.fig = Figure(figsize=(3.8,3), facecolor = 'whitesmoke')
+        self.Qt_fig = FigureCanvas(self.fig)
+
+        self.ax1 = self.fig.add_axes([0.08, 0.08, 0.75, 0.85])
+        self.ax2 = self.fig.add_axes([0.85, 0.15, 0.04, 0.72])
+
+        #   Definición y manipulación de patches
+        self.x0 = 0.5
+        self.y0 = 0.5
+        self.circ = patches.Circle((self.x0, self.y0), 5, alpha = 0.3, fc = 'yellow') #Parche para ciruclo del crosshair
+        #self.circ.set_fill(False)
+        self.circ.set_linestyle('--')
+        self.circ.set_linewidth(3)
+
+        self.hline = self.ax1.axhline(self.circ.center[1], color = 'cornflowerblue', lw = 1.5, ls = '--', alpha = 0.8)
+        self.vline = self.ax1.axvline(self.circ.center[0], color = 'orange', lw = 1.5, ls = '--', alpha = 0.8)
+
+        self.x0_rec = 0
+        self.y0_rec = 0
+        self.Rec_width = 0
+        self.Rec_height = 0
+        self.Rectangle = patches.Rectangle((self.x0, self.y0) , self.Rec_width, self.Rec_height)
+        self.Rectangle.set_fill(False)
+        self.Rectangle.set_linestyle('--')
+        self.Rectangle.set_linewidth(2)
+        self.ax1.add_patch(self.Rectangle)
+
+
+
+    def Img(self, D):
+        '''
+        Definir la imagen a partir de un objeto de la clase Dosepy.Dose.
+        '''
+
+        self.npI = D.array
+        self.mplI = self.ax1.imshow(self.npI)
+
+        self.x0 = int(self.npI.shape[1]/2)
+        self.y0 = int(self.npI.shape[0]/2)
+        self.circ.center  = self.x0, self.y0
+        self.circ.set_radius( 0.04 *  np.min(self.npI.shape))
+
+        self.hline.set_ydata( int(self.circ.center[1]) )
+        self.vline.set_xdata( int(self.circ.center[0]) )
+        self.ax1.add_patch(self.circ)
+
+        self.Cross_Hair_set_up()
+
+
+
+    def Colores(self, npI_color_ref):
+        '''
+        Definir el mapa de colores a utiliar. Como argumento se requiere de una imagen de referencia para elegui mapa.
+        Por lo general se utiliza la distribución calculada por el TPS.
+        '''
+        color_map = 'viridis'
+        bounds = np.linspace(0, round(1.15 * np.percentile(npI_color_ref, 98)), 256)
+        norm = colors.BoundaryNorm(boundaries = bounds, ncolors = 256)
+        self.mplI.set_norm(norm)
+        self.mplI.set_cmap(color_map)
+        self.cbar = self.fig.colorbar(self.mplI, cax = self.ax2, orientation = 'vertical', shrink = 0.6, format = '%.1f')
+
+
+    def ROI_Rect_set_up(self, event):
+        '''
+        Definición del ROI rectangular.
+        '''
+        self.x0_rec = event.xdata
+        self.y0_rec = event.ydata
+        self.Rectangle.set_visible(True)
+
+    def ROI_Rect_on(self):
+        self.Rectangle.set_visible(True)
+        self.fig.canvas.draw()
+
+    def ROI_Rect_off(self):
+        self.Rectangle.set_visible(False)
+        self.fig.canvas.draw()
+
+
+
+
+
+    def Cross_Hair_set_up(self):
+        '''
+        Definición del Cross Hair.
+        '''
+
+        self.hline.set_ydata( int(self.circ.center[1]) )
+        self.vline.set_xdata( int(self.circ.center[0]) )
+
+    def Cross_Hair_on(self):
+        '''
+        Enciende el Cross Hair.
+        '''
+        self.hline.set_visible(True)
+        self.vline.set_visible(True)
+        self.circ.set_visible(True)
+        self.fig.canvas.draw()
+
+    def Cross_Hair_off(self):
+        '''
+        Enciende el Cross Hair.
+        '''
+        self.hline.set_visible(False)
+        self.vline.set_visible(False)
+        self.circ.set_visible(False)
+        self.fig.canvas.draw()
+
+
+
+
+
+
+class Qt_Figure_Perfiles:
+    """
+    Clase para contener los perfiles de las distribuciones y graficarlos
+    """
+
+    def __init__(self):
+        self.fig = Figure(figsize=(4,3), tight_layout = True, facecolor = 'whitesmoke')
+        self.Qt_fig = FigureCanvas(self.fig)
 
+        #   Axes para la imagen
+        self.ax = self.fig.add_subplot(1, 1, 1)
+        self.ax.set_title('Perfiles')
+        self.ax.set_ylabel('Dosis [Gy]')
+        self.ax.grid(alpha = 0.3)
+
+
+    def set_data_and_plot(self, D_ref, D_eval, circ):
+        self.perfil_horizontal_ref = D_ref[int(circ.center[1]), :]
+        self.perfil_horizontal_eval = D_eval[int(circ.center[1]), :]
+        self.perfil_vertical_ref = D_ref[:, int(circ.center[0])]
+        self.perfil_vertical_eval = D_eval[:, int(circ.center[0])]
+        self.ax.clear()
+        self.ax.plot(self.perfil_horizontal_ref, color = 'cornflowerblue')
+        self.ax.plot(self.perfil_horizontal_eval, color = 'cornflowerblue', ls = '--')
+        self.ax.plot(self.perfil_vertical_ref, color = 'orange')
+        self.ax.plot(self.perfil_vertical_eval, color = 'orange', ls = '--')
+        self.ax.set_ylabel('Dosis [Gy]')
+        self.ax.set_xlabel('Píxel')
+        self.ax.grid(alpha = 0.3)
+
+        self.fig.canvas.draw()
 
-    def about_ventana(self):
-        if self.about_window_sec == None:
-            self.about_window = About_Window()
-        self.about_window.show()
 
-    def licencia_ventana(self):
-        if self.licencia_window_sec == None:
-            self.licencia_window_sec = Licencia_Window()
-        self.licencia_window_sec.show()
 
-app = QApplication(sys.argv)
-#windowA = Ventana_Secundaria() 
-windowA = VentanaPrincipal('P')
 
-sys.exit(app.exec())
+#%%
+
+if __name__ == '__main__':
+    app = QApplication(sys.argv)
+    ventana_raiz = Bloque_Imagenes()
+    ventana_raiz.setGeometry(100, 150, 1200, 300)
+    ventana_raiz.show()
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.3.9/src/Dosepy/GUILayouts/about_window.py` & `Dosepy-0.4.0/src/Dosepy/GUILayouts/about_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,18 @@
             "margin-left: 80px;" +
             "margin-right: 80px;"
         )
 
         layout_padre_V.addWidget(label_logo)
 
         label_version = QLabel(self)
-        label_version.setText('Versión 0.3.7')
+
+        label_version.setText('Versión 0.4.0')
         label_version.setAlignment(Qt.AlignmentFlag.AlignHCenter)
+
         label_version.setStyleSheet(
             "margin-top: 10px;" +
             "font-size: 22px;" +
             "margin-bottom: 5px;" +
             "color: 'whitesmoke';"
         )
```

### Comparing `Dosepy-0.3.9/src/Dosepy/GUILayouts/cross_hair_cursor.py` & `Dosepy-0.4.0/src/Dosepy/GUILayouts/cross_hair_cursor.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/GUILayouts/film_to_doseGUI.py` & `Dosepy-0.4.0/src/Dosepy/GUILayouts/film_to_doseGUI.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/GUILayouts/licencia_window.py` & `Dosepy-0.4.0/src/Dosepy/GUILayouts/licencia_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 Condiciones de uso 
 
 Toda persona tiene acceso a la lectura y uso del código con fines académicos o de enseñanza. 
 Sin embargo, para el uso clínico del programa se requiere contar con una licencia 
 (disponible próximamente), conocida como “Acuerdo de licencia de usuario final” 
 (EULA, por sus siglas en inglés), así como contratos que garanticen el cumplimiento 
-de la legislación de cada país.
+de la legislación de cada país. 
 
 El código o software derivado, tales como arreglos, compendios, ampliaciones, traducciones, adaptaciones,
 paráfrasis, compilaciones, colecciones y transformaciones del software DOSEPY, podrán ser explotadas
 cuando hayan sido autorizadas por el titular del derecho patrimonial sobre la obra DOSEPY,
 previo consentimiento del titular del derecho moral, en los casos previstos en la Fracción III
 del Artículo 21 de la Ley Federal del Derecho de Autor.
```

### Comparing `Dosepy-0.3.9/src/Dosepy/GUILayouts/to_do_rendering.py` & `Dosepy-0.4.0/src/Dosepy/GUILayouts/to_do_rendering.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/Icon/Icon.png` & `Dosepy-0.4.0/src/Dosepy/Icon/Icon.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/Icon/Logo_Dosepy.png` & `Dosepy-0.4.0/src/Dosepy/Icon/Logo_Dosepy.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/Icon/folder.png` & `Dosepy-0.4.0/src/Dosepy/Icon/folder.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/Icon/save.png` & `Dosepy-0.4.0/src/Dosepy/Icon/save.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/data/D_FILM.csv` & `Dosepy-0.4.0/src/Dosepy/data/D_FILM.csv`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/data/D_TPS.csv` & `Dosepy-0.4.0/src/Dosepy/data/D_TPS.csv`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/tools/film_to_dose.py` & `Dosepy-0.4.0/src/Dosepy/tools/film_to_dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy/tools/resol.py` & `Dosepy-0.4.0/src/Dosepy/tools/resol.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.3.9/src/Dosepy.egg-info/SOURCES.txt` & `Dosepy-0.4.0/src/Dosepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

