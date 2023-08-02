# Comparing `tmp/idev-pycolor-1.0.3.tar.gz` & `tmp/idev-pycolor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idev-pycolor-1.0.3.tar", last modified: Mon Jul 31 06:35:56 2023, max compression
+gzip compressed data, was "idev-pycolor-1.0.4.tar", last modified: Wed Aug  2 05:09:07 2023, max compression
```

## Comparing `idev-pycolor-1.0.3.tar` & `idev-pycolor-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.657070 idev-pycolor-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     7998 2023-07-31 06:35:56.658073 idev-pycolor-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7252 2023-07-31 03:31:04.000000 idev-pycolor-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.623524 idev-pycolor-1.0.3/idev-pycolor/
-drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.635035 idev-pycolor-1.0.3/idev-pycolor/PyColor/
--rw-rw-rw-   0        0        0    37396 2023-07-31 06:29:08.000000 idev-pycolor-1.0.3/idev-pycolor/PyColor/Colors.py
--rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.3/idev-pycolor/PyColor/Palettes.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.3/idev-pycolor/PyColor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.656070 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/
--rw-rw-rw-   0        0        0     7998 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      740 2023-07-31 06:35:15.000000 idev-pycolor-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-07-31 06:35:56.665143 idev-pycolor-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-07-31 06:35:22.000000 idev-pycolor-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.288792 idev-pycolor-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     8387 2023-08-02 05:09:07.288792 idev-pycolor-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7641 2023-08-02 05:07:36.000000 idev-pycolor-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.228198 idev-pycolor-1.0.4/idev-pycolor/
+drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.267770 idev-pycolor-1.0.4/idev-pycolor/PyColor/
+-rw-rw-rw-   0        0        0    37388 2023-07-31 07:03:11.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/Colors.py
+-rw-rw-rw-   0        0        0     1587 2023-07-31 07:00:42.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/Functions.py
+-rw-rw-rw-   0        0        0     4292 2023-07-31 06:47:09.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/Palettes.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.287755 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/
+-rw-rw-rw-   0        0        0     8387 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      740 2023-08-02 05:07:44.000000 idev-pycolor-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-08-02 05:09:07.290755 idev-pycolor-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-08-02 05:08:07.000000 idev-pycolor-1.0.4/setup.py
```

### Comparing `idev-pycolor-1.0.3/LICENSE` & `idev-pycolor-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.3/PKG-INFO` & `idev-pycolor-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: idev-pycolor
-Version: 1.0.3
-Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
-Home-page: https://github.com/IrtsaDevelopment/PyColor
-Author: IrtsaDevelopment
-Author-email: Irtsa <irtsa.development@gmail.com>
-Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
-Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyColor
 A [**python**](https://www.python.org) collection of classes and functions to convert between **rgb**, **hsv**, **hsl**, **xyz**, **ycc**, **cmyk** and **hex** color formats and generate palettes from said colors.
 <br />
 - **RGB** (*red*, *green*, *blue*)
 - **HSV** (*hue*, *saturation*, *value*)
 - **HSL** (*hue*, *saturation*, *lightness*)
 - **XYZ** (*x*, *y*, *z*)
@@ -44,14 +28,15 @@
 <br />
 <br />
 
 ## Usage
 To import, simply put:
 ```py
 from PyColor.Colors import *
+from PyColor.Functions import *
 from PyColor.Palettes import GeneratePalette
 ```
 <br />
 
 Then, later on you may utilize:
 ```py
 rgb = RGB(100, 100, 100)
@@ -246,14 +231,20 @@
 # Will print off a string representation of the hexidecimal value
 ```
 <br />
 
 ```py
 GeneratePalette(RGB(100, 100, 100), 'triad')
 # Will generate a palette in the form of a list of colors in the same type of class given using the scheme provided.
+
+Interpolate([RGB(100, 100, 100), RGB(150, 150, 150)])
+# Will interpolate colors that should go in between the ones given and return as a list of RGB objects.
+
+InterpolateFormat([HSV(320, 50, 100), HSV(150, 100, 60)])
+# Will interpolate colors that should go in between the ones given and return a list of color objects similar to the provided ones.
 ```
 ​
 <br />
 <br />
 ### Code Examples
 ```py
 from PyColors.Colors import *
@@ -290,8 +281,8 @@
 The following are the currently supports schemes for the `GeneratePalette` function:
 - monochromatic
 - analogous
 - complimentary
 - splitcomplimentary
 - tetrad
 - triad
-- random
+- random
```

### Comparing `idev-pycolor-1.0.3/README.md` & `idev-pycolor-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: idev-pycolor
+Version: 1.0.4
+Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
+Home-page: https://github.com/IrtsaDevelopment/PyColor
+Author: IrtsaDevelopment
+Author-email: Irtsa <irtsa.development@gmail.com>
+Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
+Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyColor
 A [**python**](https://www.python.org) collection of classes and functions to convert between **rgb**, **hsv**, **hsl**, **xyz**, **ycc**, **cmyk** and **hex** color formats and generate palettes from said colors.
 <br />
 - **RGB** (*red*, *green*, *blue*)
 - **HSV** (*hue*, *saturation*, *value*)
 - **HSL** (*hue*, *saturation*, *lightness*)
 - **XYZ** (*x*, *y*, *z*)
@@ -28,14 +44,15 @@
 <br />
 <br />
 
 ## Usage
 To import, simply put:
 ```py
 from PyColor.Colors import *
+from PyColor.Functions import *
 from PyColor.Palettes import GeneratePalette
 ```
 <br />
 
 Then, later on you may utilize:
 ```py
 rgb = RGB(100, 100, 100)
@@ -230,14 +247,20 @@
 # Will print off a string representation of the hexidecimal value
 ```
 <br />
 
 ```py
 GeneratePalette(RGB(100, 100, 100), 'triad')
 # Will generate a palette in the form of a list of colors in the same type of class given using the scheme provided.
+
+Interpolate([RGB(100, 100, 100), RGB(150, 150, 150)])
+# Will interpolate colors that should go in between the ones given and return as a list of RGB objects.
+
+InterpolateFormat([HSV(320, 50, 100), HSV(150, 100, 60)])
+# Will interpolate colors that should go in between the ones given and return a list of color objects similar to the provided ones.
 ```
 ​
 <br />
 <br />
 ### Code Examples
 ```py
 from PyColors.Colors import *
@@ -274,8 +297,8 @@
 The following are the currently supports schemes for the `GeneratePalette` function:
 - monochromatic
 - analogous
 - complimentary
 - splitcomplimentary
 - tetrad
 - triad
-- random
+- random
```

### Comparing `idev-pycolor-1.0.3/idev-pycolor/PyColor/Colors.py` & `idev-pycolor-1.0.4/idev-pycolor/PyColor/Colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     @property
     def grayscale(self) -> tuple:
         if not self.__valid: return None
 
         gv = int(round((self.red + self.green + self.blue) / 3.0))
 
         return RGB(gv, gv, gv)
-    
+
 
     @property
     def greyscale(self) -> tuple: return self.grayscale
         
 
 
     def __repr__(self):
@@ -334,15 +334,14 @@
         if not self.__valid: return None
 
         y = round((16 + ((65.738 * self.rgb[0]) / 256) + ((129.057 * self.rgb[1]) / 256) + ((25.064 * self.rgb[2]) / 256)), 2)
         cb = round((128 - ((37.945 * self.rgb[0]) / 256) - ((74.494 * self.rgb[1]) / 256) + ((112.439 * self.rgb[2]) / 256)), 2)
         cr = round((128 + ((112.439 * self.rgb[0]) / 256) - ((94.154 * self.rgb[1]) / 256) - ((18.285 * self.rgb[2]) / 256)), 2)
 
         return (y, cb, cr)
-
       
 
     @property
     def cmyk(self):
         if not self.__valid: return None
 
         nr = self.rgb[0] / 255.0
@@ -355,15 +354,14 @@
         M = int(round(((1 - ng - K) / (1 - K) * 100)))
         Y = int(round(((1 - nb - K) / (1 - K) * 100)))
         K = int(round(K * 100))
 
         return (C, M, Y, K)
 
 
-
     @property
     def percentForm(self) -> float:
         Numbers = [int(i, 16) for i in self.hexicode[1:]][::-1]
         Numbers = [((16 ** i) * Numbers[i]) for i in range(len(Numbers))]
 
         number = sum(Numbers)
```

### Comparing `idev-pycolor-1.0.3/idev-pycolor/PyColor/Palettes.py` & `idev-pycolor-1.0.4/idev-pycolor/PyColor/Palettes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PyColor.Colors import *
 
 
 
 
 
 
-#Functions
+#Private Functions
 def __convertFormat(targetFormat: str, current: RGB | HEX | HSV | HSL | XYZ | YCC | CMYK):
     match targetFormat:
         case 'RGB': return RGB(*current.rgb)
         case 'HEX' : return HEX(*current.hexidecimal)
         case 'HSV' : return HSV(*current.hsv)
         case 'HSL' : return HSL(*current.hsl)
         case 'XYZ' : return XYZ(*current.xyz)
@@ -41,14 +41,16 @@
 def __capNumber(cap: int, number: int):
     if number < 0: return number + cap
     if number > cap: return number - cap
     return number
 
 
 
+
+#Public Functions
 def GeneratePalette(Color: RGB | HEX | HSV | HSL | XYZ | YCC | CMYK, scheme: str) -> list:
     """
     Function to generate a color pallete given a Color class object and a scheme.
 
     Attributes:
         Color (RGB | HEX | HSV | HSL | XYZ | YCC | CMYK): Color to generate pallete from.
         scheme (str): Scheme to use for the pallete, must be one of the supported schemes.
@@ -118,8 +120,8 @@
         
 
         case 'random':
             Hues = [__capNumber(360, Color.hsv[0] + randint(-360, 360)) for i in range(3)] + [Color.hsv[0]]
             saturation = Color.hsv[1]
             value = Color.hsv[2]
 
-            return [__convertFormat(__convertClassToString(Color), HSV(hue, saturation, value)) for hue in Hues]
+            return [__convertFormat(__convertClassToString(Color), HSV(hue, saturation, value)) for hue in Hues]
```

### Comparing `idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/PKG-INFO` & `idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
@@ -44,14 +44,15 @@
 <br />
 <br />
 
 ## Usage
 To import, simply put:
 ```py
 from PyColor.Colors import *
+from PyColor.Functions import *
 from PyColor.Palettes import GeneratePalette
 ```
 <br />
 
 Then, later on you may utilize:
 ```py
 rgb = RGB(100, 100, 100)
@@ -246,14 +247,20 @@
 # Will print off a string representation of the hexidecimal value
 ```
 <br />
 
 ```py
 GeneratePalette(RGB(100, 100, 100), 'triad')
 # Will generate a palette in the form of a list of colors in the same type of class given using the scheme provided.
+
+Interpolate([RGB(100, 100, 100), RGB(150, 150, 150)])
+# Will interpolate colors that should go in between the ones given and return as a list of RGB objects.
+
+InterpolateFormat([HSV(320, 50, 100), HSV(150, 100, 60)])
+# Will interpolate colors that should go in between the ones given and return a list of color objects similar to the provided ones.
 ```
 ​
 <br />
 <br />
 ### Code Examples
 ```py
 from PyColors.Colors import *
```

### Comparing `idev-pycolor-1.0.3/pyproject.toml` & `idev-pycolor-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "idev-pycolor"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `idev-pycolor-1.0.3/setup.cfg` & `idev-pycolor-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e33  .version = 1.0.3
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e34  .version = 1.0.4
 00000030: 0d0a 6175 7468 6f72 203d 2049 7274 7361  ..author = Irtsa
 00000040: 4465 7665 6c6f 706d 656e 740d 0a61 7574  Development..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6972 7473  hor_email = irts
 00000060: 612e 6465 7665 6c6f 706d 656e 7440 676d  a.development@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 636f 6c6c 6563 7469 6f6e 206f 6620 636c  collection of cl
```

### Comparing `idev-pycolor-1.0.3/setup.py` & `idev-pycolor-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "idev-pycolor",
-    version = "1.0.3",
+    version = "1.0.4",
     author = "IrtsaDevelopment",
     author_email = "irtsa.development@gmail.com",
     description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IrtsaDevelopment/PyColor",
     project_urls = {
```

