# Comparing `tmp/xmds2tools-1.0.0.tar.gz` & `tmp/xmds2tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmds2tools-1.0.0.tar", last modified: Wed Mar  1 14:47:03 2023, max compression
+gzip compressed data, was "xmds2tools-1.0.1.tar", last modified: Wed Aug  2 20:06:49 2023, max compression
```

## Comparing `xmds2tools-1.0.0.tar` & `xmds2tools-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 14:47:03.614177 xmds2tools-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-02-28 09:14:50.000000 xmds2tools-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       38 2023-02-28 11:27:05.000000 xmds2tools-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5209 2023-03-01 14:47:03.613180 xmds2tools-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3337 2023-03-01 14:42:43.000000 xmds2tools-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 14:47:03.589244 xmds2tools-1.0.0/examples/
--rw-rw-rw-   0        0        0     1558 2023-02-28 10:39:01.000000 xmds2tools-1.0.0/examples/bc_groundstate.py
--rw-rw-rw-   0        0        0     1482 2023-02-28 11:06:26.000000 xmds2tools-1.0.0/examples/bessel_integration.py
--rw-rw-rw-   0        0        0      970 2023-02-28 10:24:36.000000 xmds2tools-1.0.0/examples/groundstate_workedexamples.py
--rw-rw-rw-   0        0        0      864 2023-02-28 09:34:36.000000 xmds2tools-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 14:47:03.615175 xmds2tools-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-01 14:47:03.571292 xmds2tools-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 14:47:03.597224 xmds2tools-1.0.0/src/xmds2tools/
--rw-rw-rw-   0        0        0      182 2023-02-28 09:14:50.000000 xmds2tools-1.0.0/src/xmds2tools/__init__.py
--rw-rw-rw-   0        0        0     8992 2023-02-28 09:14:50.000000 xmds2tools-1.0.0/src/xmds2tools/bessel.py
--rw-rw-rw-   0        0        0     8980 2023-02-28 14:45:25.000000 xmds2tools-1.0.0/src/xmds2tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-03-01 14:47:03.611186 xmds2tools-1.0.0/src/xmds2tools.egg-info/
--rw-rw-rw-   0        0        0     5209 2023-03-01 14:47:03.000000 xmds2tools-1.0.0/src/xmds2tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-03-01 14:47:03.000000 xmds2tools-1.0.0/src/xmds2tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 14:47:03.000000 xmds2tools-1.0.0/src/xmds2tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-03-01 14:47:03.000000 xmds2tools-1.0.0/src/xmds2tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-01 14:47:03.000000 xmds2tools-1.0.0/src/xmds2tools.egg-info/top_level.txt
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-08-02 20:06:49.987621 xmds2tools-1.0.1/
+-rw-rw-r--   0 craig     (1000) craig     (1000)     1071 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/LICENSE
+-rw-rw-r--   0 craig     (1000) craig     (1000)       36 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/MANIFEST.in
+-rw-rw-r--   0 craig     (1000) craig     (1000)     5180 2023-08-02 20:06:49.987621 xmds2tools-1.0.1/PKG-INFO
+-rw-rw-r--   0 craig     (1000) craig     (1000)     3344 2023-08-02 19:58:49.000000 xmds2tools-1.0.1/README.md
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-08-02 20:06:49.983621 xmds2tools-1.0.1/examples/
+-rw-rw-r--   0 craig     (1000) craig     (1000)     1511 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/examples/bc_groundstate.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)     1437 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/examples/bessel_integration.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)      934 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/examples/groundstate_workedexamples.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)      835 2023-08-02 19:59:03.000000 xmds2tools-1.0.1/pyproject.toml
+-rw-rw-r--   0 craig     (1000) craig     (1000)       38 2023-08-02 20:06:49.987621 xmds2tools-1.0.1/setup.cfg
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-08-02 20:06:49.983621 xmds2tools-1.0.1/src/
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-08-02 20:06:49.983621 xmds2tools-1.0.1/src/xmds2tools/
+-rw-rw-r--   0 craig     (1000) craig     (1000)      172 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/src/xmds2tools/__init__.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)     8805 2023-07-09 20:22:28.000000 xmds2tools-1.0.1/src/xmds2tools/bessel.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)     8796 2023-08-02 19:57:47.000000 xmds2tools-1.0.1/src/xmds2tools/reader.py
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-08-02 20:06:49.987621 xmds2tools-1.0.1/src/xmds2tools.egg-info/
+-rw-rw-r--   0 craig     (1000) craig     (1000)     5180 2023-08-02 20:06:49.000000 xmds2tools-1.0.1/src/xmds2tools.egg-info/PKG-INFO
+-rw-rw-r--   0 craig     (1000) craig     (1000)      407 2023-08-02 20:06:49.000000 xmds2tools-1.0.1/src/xmds2tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)        1 2023-08-02 20:06:49.000000 xmds2tools-1.0.1/src/xmds2tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)       42 2023-08-02 20:06:49.000000 xmds2tools-1.0.1/src/xmds2tools.egg-info/requires.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)       11 2023-08-02 20:06:49.000000 xmds2tools-1.0.1/src/xmds2tools.egg-info/top_level.txt
```

### Comparing `xmds2tools-1.0.0/LICENSE` & `xmds2tools-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Craig Chisholm
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Craig Chisholm
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `xmds2tools-1.0.0/PKG-INFO` & `xmds2tools-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1
-Name: xmds2tools
-Version: 1.0.0
-Summary: Tools to read .hdf5 and .xsil files generated using XMDS2 and functions to implement Bessel transformations and Bessel quadrature integration
-Author-email: Craig Chisholm <craig.chisholm@protonmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Craig Chisholm
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/CSChisholm/xmds2-tools
-Keywords: XMDS2,HDF5,Bessel
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# xmds2-tools
-Tools to read .hdf5 and .xsil files generated using [XMDS2](http://xmds.org) and functions to implement Bessel transformations and Bessel quadrature integration
-
-These tools were built to work with the output files generated by XMDS2 but can be used for other purposes.
-
-The function `reader.ReadH5` reads any [HDF5 file](https://www.hdfgroup.org/solutions/hdf5/) and returns the contents as a Python dictionary. Likewise, `reader.WriteH5` takes a Python dictionary and saves the contents as an HDF5 file.
-
-XMDS2 simulations generate a text file with extension `.xsil` as well as the HDF5 data. The function 'reader.ParseXSIL' reads the XML data from the text file and returns a dictionary with simulation parameters including global variables, command line variables, and variables derived from global and command line variables. If the Bessel transform is used on an axis a variable called `"axis name"Outer` is added where `"axis name"` is the name of the axis defined in XMDS and the value of the variable is the outer radius of the interval defining the grid.
-
-The `bessel.py` module is based on [Numerical calculation of dipolar-quantum-droplet stationary states](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013283) and implements Bessel quadrature integration and numerical radial derivative in cylindrical coordinates.
-
-## Examples
-The `examples/` folder contains Python scripts demonstrating the use of the `reader` and `bessel` modules to analyse the output of some of the XMDS2 examples. The `bessel` module is also used for quadrature integration and compared to the trapezium method.
-
-None of the examples or any of the XMDS2 source code is reproduced here and the user is instead refered to the [XMDS2 website](http://xmds.org')
-
-* `examples/groundstate_workedexamples.py` corresponds to the continuous renormalisation groundstate example.
-* `examples/bc_groundstate.py` corresponds to the imaginary time evolution example using DCT and Bessel transform in the XMDS directory `examples/bessel_cosine_groundstate.xmds`
-* `examples/bessel_integration.py` compares convergence when integrating using the trapezium method and by Bessel quadrature
-
-## Installation
-
-### Install from PyPI
-
-* `python -m pip install xmds2tools`
-
-### Build from source
-* `python -m pip install --upgrade pip setuptools`
-* `python -m pip install build`
-* `git clone https://github.com/CSChisholm/xmds2-tools`
-* `cd xmds2-tools`
-* `python -m build`
-
-## Acknowledgements
-
-These functions were written and tested during the PhD project of C. S. Chisholm at [ICFO - The Institute of Photonic Sciences](https://www.icfo.eu/) under the supervision of Prof. Dr. Leticia Tarruell and with support from Dr. Ramón Ramos.
-
-Thanks to Prof. P. B. Blakie, Dr. M. Johnsson, and Prof. M. J. Davis for advice.
-
-## References
-
-1. G. R. Dennis, J. J. Hope, and M. T. Johnsson, [*XMDS2: Fast, scalable simulation of coupled stochastic partial differential equations*](https://doi.org/10.1016/j.cpc.2012.08.016). Compuer Physics Communications **184**(1), 201-208 (2013).
-2. A.-C. Lee, D. Baillie, and P. B. Blakie, [*Numerical calculation of dipolar-quantum-droplet stationary states*](https://doi.org/10.1103/PhysRevResearch.3.013283). Physical Review Research **3**, 013283 (2021).
+Metadata-Version: 2.1
+Name: xmds2tools
+Version: 1.0.1
+Summary: Tools to read .hdf5 and .xsil files generated using XMDS2 and functions to implement Bessel transformations and Bessel quadrature integration
+Author-email: Craig Chisholm <craig.chisholm@protonmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Craig Chisholm
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/CSChisholm/xmds2-tools
+Keywords: XMDS2,HDF5,Bessel
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# xmds2-tools
+Tools to read .hdf5 and .xsil files generated using [XMDS2](http://xmds.org) and functions to implement Bessel transformations and Bessel quadrature integration
+
+These tools were built to work with the output files generated by XMDS2 but can be used for other purposes.
+
+The function `reader.ReadH5` reads any [HDF5 file](https://www.hdfgroup.org/solutions/hdf5/) and returns the contents as a Python dictionary. Likewise, `reader.WriteH5` takes a Python dictionary and saves the contents as an HDF5 file.
+
+XMDS2 simulations generate a text file with extension `.xsil` as well as the HDF5 data. The function `reader.ParseXSIL` reads the XML data from the text file and returns a dictionary with simulation parameters including global variables, command line variables, and variables derived from global and command line variables. If the Bessel transform is used on an axis a variable called `"axis name"Outer` is added where `"axis name"` is the name of the axis defined in XMDS and the value of the variable is the outer radius of the interval defining the grid.
+
+The `bessel.py` module is based on [Numerical calculation of dipolar-quantum-droplet stationary states](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013283) and implements Bessel quadrature integration and numerical radial derivative in cylindrical coordinates.
+
+## Examples
+The `examples/` folder contains Python scripts demonstrating the use of the `reader` and `bessel` modules to analyse the output of some of the XMDS2 examples. The `bessel` module is also used for quadrature integration and compared to the trapezium method.
+
+None of the examples or any of the XMDS2 source code is reproduced here and the user is instead refered to the [XMDS2 website](http://xmds.org')
+
+* `examples/groundstate_workedexamples.py` corresponds to the continuous renormalisation groundstate example.
+* `examples/bc_groundstate.py` corresponds to the imaginary time evolution example using DCT and Bessel transform in the XMDS directory `examples/bessel_cosine_groundstate.xmds`
+* `examples/bessel_integration.py` compares convergence when integrating using the trapezium method and by Bessel quadrature
+
+## Installation
+
+### Install from [PyPI](https://pypi.org/project/xmds2tools/1.0.1/)
+
+* `python -m pip install xmds2tools`
+
+### Build from source
+* `python -m pip install --upgrade pip setuptools`
+* `python -m pip install build`
+* `git clone https://github.com/CSChisholm/xmds2-tools`
+* `cd xmds2-tools`
+* `python -m build`
+
+## Acknowledgements
+
+These functions were written and tested during the PhD project of C. S. Chisholm at [ICFO - The Institute of Photonic Sciences](https://www.icfo.eu/) under the supervision of Prof. Dr. Leticia Tarruell and with support from Dr. Ramón Ramos.
+
+Thanks to Prof. P. B. Blakie, Dr. M. T. Johnsson, and Prof. M. J. Davis for advice.
+
+## References
+
+1. G. R. Dennis, J. J. Hope, and M. T. Johnsson, [*XMDS2: Fast, scalable simulation of coupled stochastic partial differential equations*](https://doi.org/10.1016/j.cpc.2012.08.016). Computer Physics Communications **184**(1), 201-208 (2013).
+2. A.-C. Lee, D. Baillie, and P. B. Blakie, [*Numerical calculation of dipolar-quantum-droplet stationary states*](https://doi.org/10.1103/PhysRevResearch.3.013283). Physical Review Research **3**, 013283 (2021).
```

### Comparing `xmds2tools-1.0.0/README.md` & `xmds2tools-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# xmds2-tools
-Tools to read .hdf5 and .xsil files generated using [XMDS2](http://xmds.org) and functions to implement Bessel transformations and Bessel quadrature integration
-
-These tools were built to work with the output files generated by XMDS2 but can be used for other purposes.
-
-The function `reader.ReadH5` reads any [HDF5 file](https://www.hdfgroup.org/solutions/hdf5/) and returns the contents as a Python dictionary. Likewise, `reader.WriteH5` takes a Python dictionary and saves the contents as an HDF5 file.
-
-XMDS2 simulations generate a text file with extension `.xsil` as well as the HDF5 data. The function 'reader.ParseXSIL' reads the XML data from the text file and returns a dictionary with simulation parameters including global variables, command line variables, and variables derived from global and command line variables. If the Bessel transform is used on an axis a variable called `"axis name"Outer` is added where `"axis name"` is the name of the axis defined in XMDS and the value of the variable is the outer radius of the interval defining the grid.
-
-The `bessel.py` module is based on [Numerical calculation of dipolar-quantum-droplet stationary states](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013283) and implements Bessel quadrature integration and numerical radial derivative in cylindrical coordinates.
-
-## Examples
-The `examples/` folder contains Python scripts demonstrating the use of the `reader` and `bessel` modules to analyse the output of some of the XMDS2 examples. The `bessel` module is also used for quadrature integration and compared to the trapezium method.
-
-None of the examples or any of the XMDS2 source code is reproduced here and the user is instead refered to the [XMDS2 website](http://xmds.org')
-
-* `examples/groundstate_workedexamples.py` corresponds to the continuous renormalisation groundstate example.
-* `examples/bc_groundstate.py` corresponds to the imaginary time evolution example using DCT and Bessel transform in the XMDS directory `examples/bessel_cosine_groundstate.xmds`
-* `examples/bessel_integration.py` compares convergence when integrating using the trapezium method and by Bessel quadrature
-
-## Installation
-
-### Install from PyPI
-
-* `python -m pip install xmds2tools`
-
-### Build from source
-* `python -m pip install --upgrade pip setuptools`
-* `python -m pip install build`
-* `git clone https://github.com/CSChisholm/xmds2-tools`
-* `cd xmds2-tools`
-* `python -m build`
-
-## Acknowledgements
-
-These functions were written and tested during the PhD project of C. S. Chisholm at [ICFO - The Institute of Photonic Sciences](https://www.icfo.eu/) under the supervision of Prof. Dr. Leticia Tarruell and with support from Dr. Ramón Ramos.
-
-Thanks to Prof. P. B. Blakie, Dr. M. Johnsson, and Prof. M. J. Davis for advice.
-
-## References
-
-1. G. R. Dennis, J. J. Hope, and M. T. Johnsson, [*XMDS2: Fast, scalable simulation of coupled stochastic partial differential equations*](https://doi.org/10.1016/j.cpc.2012.08.016). Compuer Physics Communications **184**(1), 201-208 (2013).
-2. A.-C. Lee, D. Baillie, and P. B. Blakie, [*Numerical calculation of dipolar-quantum-droplet stationary states*](https://doi.org/10.1103/PhysRevResearch.3.013283). Physical Review Research **3**, 013283 (2021).
+# xmds2-tools
+Tools to read .hdf5 and .xsil files generated using [XMDS2](http://xmds.org) and functions to implement Bessel transformations and Bessel quadrature integration
+
+These tools were built to work with the output files generated by XMDS2 but can be used for other purposes.
+
+The function `reader.ReadH5` reads any [HDF5 file](https://www.hdfgroup.org/solutions/hdf5/) and returns the contents as a Python dictionary. Likewise, `reader.WriteH5` takes a Python dictionary and saves the contents as an HDF5 file.
+
+XMDS2 simulations generate a text file with extension `.xsil` as well as the HDF5 data. The function `reader.ParseXSIL` reads the XML data from the text file and returns a dictionary with simulation parameters including global variables, command line variables, and variables derived from global and command line variables. If the Bessel transform is used on an axis a variable called `"axis name"Outer` is added where `"axis name"` is the name of the axis defined in XMDS and the value of the variable is the outer radius of the interval defining the grid.
+
+The `bessel.py` module is based on [Numerical calculation of dipolar-quantum-droplet stationary states](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013283) and implements Bessel quadrature integration and numerical radial derivative in cylindrical coordinates.
+
+## Examples
+The `examples/` folder contains Python scripts demonstrating the use of the `reader` and `bessel` modules to analyse the output of some of the XMDS2 examples. The `bessel` module is also used for quadrature integration and compared to the trapezium method.
+
+None of the examples or any of the XMDS2 source code is reproduced here and the user is instead refered to the [XMDS2 website](http://xmds.org')
+
+* `examples/groundstate_workedexamples.py` corresponds to the continuous renormalisation groundstate example.
+* `examples/bc_groundstate.py` corresponds to the imaginary time evolution example using DCT and Bessel transform in the XMDS directory `examples/bessel_cosine_groundstate.xmds`
+* `examples/bessel_integration.py` compares convergence when integrating using the trapezium method and by Bessel quadrature
+
+## Installation
+
+### Install from [PyPI](https://pypi.org/project/xmds2tools/1.0.1/)
+
+* `python -m pip install xmds2tools`
+
+### Build from source
+* `python -m pip install --upgrade pip setuptools`
+* `python -m pip install build`
+* `git clone https://github.com/CSChisholm/xmds2-tools`
+* `cd xmds2-tools`
+* `python -m build`
+
+## Acknowledgements
+
+These functions were written and tested during the PhD project of C. S. Chisholm at [ICFO - The Institute of Photonic Sciences](https://www.icfo.eu/) under the supervision of Prof. Dr. Leticia Tarruell and with support from Dr. Ramón Ramos.
+
+Thanks to Prof. P. B. Blakie, Dr. M. T. Johnsson, and Prof. M. J. Davis for advice.
+
+## References
+
+1. G. R. Dennis, J. J. Hope, and M. T. Johnsson, [*XMDS2: Fast, scalable simulation of coupled stochastic partial differential equations*](https://doi.org/10.1016/j.cpc.2012.08.016). Computer Physics Communications **184**(1), 201-208 (2013).
+2. A.-C. Lee, D. Baillie, and P. B. Blakie, [*Numerical calculation of dipolar-quantum-droplet stationary states*](https://doi.org/10.1103/PhysRevResearch.3.013283). Physical Review Research **3**, 013283 (2021).
```

### Comparing `xmds2tools-1.0.0/examples/bc_groundstate.py` & `xmds2tools-1.0.1/examples/bc_groundstate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Feb 28 11:24:48 2023
-
-@author: CSChisholm
-"""
-
-#Using the reader module to load the .h5 file generate by the example in the
-# xmds installation directory examples/bessel_cosine_groundstate.xmds
-
-import numpy as np
-import matplotlib.pyplot as plt
-from xmds2tools import reader
-from xmds2tools import bessel
-
-plt.close('all')
-
-data = reader.ReadH5('bc_groundstate.h5')
-variables = reader.ParseXSIL('bc_groundstate.xsil')['Variables']
-
-#Plot imaginary time evolution by integrating out spatial axes
-plt.figure()
-plt.subplot(1,2,1)
-plt.pcolormesh(data['1']['z'],data['1']['t'],2*np.pi*bessel.BesselQuadratureN_array(data['1']['norm_dens'], variables['rOuter'], 1),shading='auto')
-plt.xlabel('z')
-plt.ylabel('t')
-plt.colorbar()
-plt.subplot(1,2,2)
-plt.pcolormesh(data['1']['r'],data['1']['t'],2*np.diff(data['1']['z'])[0]*np.sum(data['1']['norm_dens'],axis=-1),shading='auto')
-plt.xlabel('r')
-plt.ylabel('t')
-plt.colorbar()
-plt.tight_layout()
-
-#Plot last density
-plt.figure()
-plt.pcolormesh(data['1']['z'],data['1']['r'],data['1']['norm_dens'][-1],shading='auto')
-plt.xlabel('z')
-plt.ylabel('r')
-plt.colorbar()
-
-#Check normalisation, we get one here because the script normalises to Nparticles but the sampling group is divided by Ncalc
-norm = 4*np.pi*np.diff(data['1']['z'])[0]*np.sum(bessel.BesselQuadratureN_array(data['1']['norm_dens'], variables['rOuter'], 1),axis=-1)
-plt.figure()
-plt.plot(data['1']['t'],norm)
-plt.xlabel('t')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Feb 28 11:24:48 2023
+
+@author: CSChisholm
+"""
+
+#Using the reader module to load the .h5 file generate by the example in the
+# xmds installation directory examples/bessel_cosine_groundstate.xmds
+
+import numpy as np
+import matplotlib.pyplot as plt
+from xmds2tools import reader
+from xmds2tools import bessel
+
+plt.close('all')
+
+data = reader.ReadH5('bc_groundstate.h5')
+variables = reader.ParseXSIL('bc_groundstate.xsil')['Variables']
+
+#Plot imaginary time evolution by integrating out spatial axes
+plt.figure()
+plt.subplot(1,2,1)
+plt.pcolormesh(data['1']['z'],data['1']['t'],2*np.pi*bessel.BesselQuadratureN_array(data['1']['norm_dens'], variables['rOuter'], 1),shading='auto')
+plt.xlabel('z')
+plt.ylabel('t')
+plt.colorbar()
+plt.subplot(1,2,2)
+plt.pcolormesh(data['1']['r'],data['1']['t'],2*np.diff(data['1']['z'])[0]*np.sum(data['1']['norm_dens'],axis=-1),shading='auto')
+plt.xlabel('r')
+plt.ylabel('t')
+plt.colorbar()
+plt.tight_layout()
+
+#Plot last density
+plt.figure()
+plt.pcolormesh(data['1']['z'],data['1']['r'],data['1']['norm_dens'][-1],shading='auto')
+plt.xlabel('z')
+plt.ylabel('r')
+plt.colorbar()
+
+#Check normalisation, we get one here because the script normalises to Nparticles but the sampling group is divided by Ncalc
+norm = 4*np.pi*np.diff(data['1']['z'])[0]*np.sum(bessel.BesselQuadratureN_array(data['1']['norm_dens'], variables['rOuter'], 1),axis=-1)
+plt.figure()
+plt.plot(data['1']['t'],norm)
+plt.xlabel('t')
 plt.ylabel('norm')
```

### Comparing `xmds2tools-1.0.0/examples/bessel_integration.py` & `xmds2tools-1.0.1/examples/bessel_integration.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Feb 28 11:45:44 2023
-
-@author: CSChisholm
-"""
-
-#Using Bessel quadrature to integrate a Gaussian function
-
-import numpy as np
-import matplotlib.pyplot as plt
-from xmds2tools import bessel
-
-def Gauss(r,sigma):
-    return np.multiply(2/(sigma**2),np.exp(-np.divide(np.power(r,2),sigma**2)))
-
-plt.close('all')
-
-sigma = 1 #Width of Gaussian
-rOuter = 4*sigma #Set an upper integration bound four times the width of the Gaussian
-
-#Plot the Gaussian
-rr_Cart = np.linspace(0,rOuter,101)
-rr_Bessel = bessel.BesselParameters(rOuter, 16, 0)[0]
-
-plt.figure()
-plt.plot(rr_Cart,Gauss(rr_Cart,sigma),label='Cartesian')
-plt.scatter(rr_Bessel,Gauss(rr_Bessel,sigma),label='Bessel')
-plt.xlabel('r')
-plt.ylabel('G(r)')
-
-#Compare number of points needed to calculate \int G(r)*rdr with Bessel quadrature and trapezium method
-besselPoints = np.logspace(0,10,11,base=2,dtype=np.int64)
-besselInt = np.array([bessel.BesselQuadrature(Gauss, rOuter, Ngrid=NN, args=(sigma,)) for NN in besselPoints])
-
-trapzPoints = np.logspace(0,3,4,dtype=np.int64)
-trapzInt = np.array([np.trapz(Gauss(np.linspace(0,rOuter,NN),sigma)*np.linspace(0,rOuter,NN),x=np.linspace(0,rOuter,NN)) for NN in trapzPoints])
-
-plt.figure()
-plt.plot(trapzPoints,trapzInt,label='Trapezium')
-plt.plot(besselPoints,besselInt,label='Bessel')
-plt.xlabel('Number of points')
-plt.ylabel('$\int G(r)*r$d$r$')
-plt.legend()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Feb 28 11:45:44 2023
+
+@author: CSChisholm
+"""
+
+#Using Bessel quadrature to integrate a Gaussian function
+
+import numpy as np
+import matplotlib.pyplot as plt
+from xmds2tools import bessel
+
+def Gauss(r,sigma):
+    return np.multiply(2/(sigma**2),np.exp(-np.divide(np.power(r,2),sigma**2)))
+
+plt.close('all')
+
+sigma = 1 #Width of Gaussian
+rOuter = 4*sigma #Set an upper integration bound four times the width of the Gaussian
+
+#Plot the Gaussian
+rr_Cart = np.linspace(0,rOuter,101)
+rr_Bessel = bessel.BesselParameters(rOuter, 16, 0)[0]
+
+plt.figure()
+plt.plot(rr_Cart,Gauss(rr_Cart,sigma),label='Cartesian')
+plt.scatter(rr_Bessel,Gauss(rr_Bessel,sigma),label='Bessel')
+plt.xlabel('r')
+plt.ylabel('G(r)')
+
+#Compare number of points needed to calculate \int G(r)*rdr with Bessel quadrature and trapezium method
+besselPoints = np.logspace(0,10,11,base=2,dtype=np.int64)
+besselInt = np.array([bessel.BesselQuadrature(Gauss, rOuter, Ngrid=NN, args=(sigma,)) for NN in besselPoints])
+
+trapzPoints = np.logspace(0,3,4,dtype=np.int64)
+trapzInt = np.array([np.trapz(Gauss(np.linspace(0,rOuter,NN),sigma)*np.linspace(0,rOuter,NN),x=np.linspace(0,rOuter,NN)) for NN in trapzPoints])
+
+plt.figure()
+plt.plot(trapzPoints,trapzInt,label='Trapezium')
+plt.plot(besselPoints,besselInt,label='Bessel')
+plt.xlabel('Number of points')
+plt.ylabel('$\int G(r)*r$d$r$')
+plt.legend()
 plt.xscale('log')
```

### Comparing `xmds2tools-1.0.0/src/xmds2tools/reader.py` & `xmds2tools-1.0.1/src/xmds2tools/reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,196 +1,197 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Feb 27 22:36:21 2023
-
-@author: CSChisholm
-
-#These functions are primarily used for reading data generated by XMDS2
-# (http://xmds.org).
-#ParseXSIL is very specific to getting metadata out of the .xsil file generated
-# by XMDS2.
-#ReadH5 will load all of the outputs defined in XMDS2 into a Python dictionary
-# but will also read any other HDF5 file into a dictionary.
-#Likewise, WriteH5 will write any dictionary into an HDF5 file.
-"""
-
-import h5py
-import xml.etree.ElementTree as ET
-import numpy as np
-
-def ReadH5(filename: str) -> dict:
-    '''Opens hdf5 file and converts every group and subgroup into a dictionary
-    where the keys are the group keys and the items are the datasets
-    
-    return data'''
-    #Open file
-    with h5py.File(filename,'r') as f:
-        data = {}
-        _Group2Dict(f,data)
-    return data
-
-def WriteH5(filename: str, data: dict):
-    '''Takes dictionary and writes hdf5 file using keys as keys and items as
-    datasets if they are not dictionaries or groups if they are dictionaries'''
-    if not(isinstance(data,dict)):
-        raise TypeError(f'Data must be a dictionary. Got type: {type(data)}.')
-    with h5py.File(filename,'w') as f:
-        _Dict2Group(f,data)
-    return
-
-def ParseXSIL(xsilFile: str) -> dict:
-    ''''Parse most of the data from a .xsil file (XMDS2) into a dictionary. We don't need geometry or output because they are in the corresponding .h5 file.
-    
-    return data'''
-    data = {'Filename': xsilFile} #Construct dictionary
-    variables = {} #The variable definitions, will later be added to data
-    comments = {} #Store the C++ comments as strings
-    vectors = {} #Defined vectors (potential, initialisation etc.)
-    operators = {} #Operators for FFT in split-step
-    equations = {} #The differential equation(s) being solved
-    axes = {}
-    xmlData = ET.parse(xsilFile).getroot() #Load XML
-    children = [child.tag for child in xmlData]
-    data['Name'] = _SearchElement('name',xmlData,children).text #Get program name
-    data['Description'] = _SearchElement('description',xmlData,children).text
-    #We also want the file as a string so that we can access <![CDATA[ blocks
-    with open(xsilFile,'r') as f:
-        lines = f.readlines()
-    #Search for vectors
-    numVecs = len(np.where(np.array(children)=='vector')[0])
-    for II in range(numVecs):
-        vec = _SearchElement('vector',xmlData,children,index=II)
-        name = vec.attrib['name']
-        if not('kind' in vec[1].attrib.keys()):
-            vectors[name] = [line for line in vec[1].text.split('\n') if '=' in line][0]
-        else: #Initialised from hdf5 file
-            vectors[name] = vec[1][0].text #Just put the file name here
-    data['Vectors'] = vectors
-    #Look in the sequence for operators, differential equations, and breakpoint
-    sequence = _SearchElement('sequence',xmlData,children)
-    try:
-        data['Breakfile'] = _SearchElement('breakpoint',sequence).attrib['filename']
-    except IndexError:
-        data['Breakfile'] = None #no break file
-    integrate = _SearchElement('integrate',sequence)
-    data['Parameters'] = integrate.attrib
-    operatorsIndex = [II for II, line in enumerate(lines) if '<operator_names>' in line][0]
-    itr = operatorsIndex
-    while not(']]>' in lines[itr]):
-        if ('=' in lines[itr]):
-            linesplit = lines[itr].split(' = ')
-            operators[linesplit[0].split(' ')[-1]] = linesplit[1].split(';')[0]
-        itr+=1
-    data['Operators'] = operators
-    equationsIndex = [II for II, line in enumerate(lines) if '<integration_vectors>' in line][0]
-    itr = equationsIndex
-    while not(']]>' in lines[itr]):
-        if ('=' in lines[itr]):
-            linesplit = lines[itr].split(' = ')
-            equations[linesplit[0].split(' ')[-1]] = linesplit[1].split(';')[0]
-        itr+=1
-    data['Equations'] = equations
-    #Search for command line arguments and store them in dict: variables
-    info = _SearchElement('info',xmlData,children).text.split('\n')
-    clargs = [line for line in info if 'Command line argument' in line]
-    for clarg in clargs:
-        definition = clarg.split('Command line argument ')[1]
-        _GetVar(definition,variables)
-        comments[definition.split(' = ')[0]] = 'Command line argument'
-    #Get global variables
-    features = _SearchElement('features',xmlData,children)
-    globalvars = _SearchElement('globals',features).text.split('\n')
-    globaldefs = [globalvar for globalvar in globalvars if 'const real' in globalvar]
-    for globaldef in globaldefs:
-        definition = globaldef.split('real ')[1].split(';')[0]
-        _GetVar(definition,variables)
-        if ('//' in globaldef):
-            comments[definition.split(' = ')[0]] = globaldef.split('//')[1]
-    #Get variables derived from command line arguments and globals
-    subLines = [II for II, line in enumerate(lines) if '<arguments>' in line]
-    if (len(subLines)):
-        derivedIndex = subLines[0]
-        itr = derivedIndex
-        while not((']]>' in lines[itr]) or ('</features>' in lines[itr])):
-            if (('=' in lines[itr]) and not('default_value' in lines[itr])):
-                line = lines[itr].replace(' ','').replace('=',' = ')
-                _GetVar(line.split(';')[0],variables)
-                if ('//' in line):
-                    comments[line.split(' = ')[0]] = line.split('//')[1]
-            itr+=1
-    data['Variables'] = variables
-    data['Comments'] = comments
-    geometry = _SearchElement('geometry',xmlData,children)
-    transverseDimensions = _SearchElement('transverse_dimensions',geometry)
-    for dimension in transverseDimensions:
-        axes[dimension.attrib['name']] = {key: value for key, value in dimension.attrib.items() if not key=='name'}
-    data['Axes'] = axes
-    for key in data['Axes'].keys():
-        if (('transform', 'bessel') in data['Axes'][key].items()):
-            data['Variables'][f'{key}Outer'] = float(data['Axes'][key]['domain'].split(', ')[1].split(')')[0])
-    return data
-
-def _Group2Dict(h5Group,data):
-    '''Helper function for ReadH5'''
-    keys = [key for key in h5Group]
-    for key in keys:
-        if (isinstance(h5Group[key],h5py.Dataset)):
-            data[key] = h5Group[key][()]
-        else:
-            data[key] = {}
-            _Group2Dict(h5Group[key],data[key])
-    return
-
-def _Dict2Group(h5group,data):
-    '''Helper function for WriteH5'''
-    keys = data.keys()
-    for key in keys:
-        if (isinstance(data[key],dict)):
-            group = h5group.create_group(key)
-            _Dict2Group(group,data[key])
-        else:
-            h5group[key] = data[key]
-    return
-
-def _SearchElement(tag, root, tags=None,index=0):
-    '''Search for the index of an xml element with a given tag.
-    If the tag appears more than once in list(root) then the optional argument,
-    index, can be used to choose which one to take
-    Helper function for ParseXSIL
-    
-    return element'''
-    if (tags is None):
-        tags = [child.tag for child in root]
-    ind = np.where(np.array(tags)==tag)[0][index]
-    return root[ind]
-
-def _GetVar(definition, variables):
-    '''From a string, return a numeric definition of a variable,
-    using previously evaluated variables if necessary
-    Helper function for ParseXSIL'''
-    splitDef = definition.split(' = ')
-    varName = splitDef[0].replace(' ','')
-    try:
-        variables[varName] = float(splitDef[1])
-    except ValueError:
-        try:
-            #We need to evaluate an expression
-            expression = splitDef[1]
-            #Variables are defined sequentially so any variable used in the expression already exists
-            #Double pass on string replacement in case some variables contain other variables within their names
-            expSplit = re.split('\*|/|\+|\-|\)|\(',expression)
-            for part in expSplit:
-                if (part in variables.keys()):
-                    expression = expression.replace(part,str(variables[part]))
-            for key in variables.keys():
-                expression = expression.replace(key,str(variables[key]))
-            #We also know that M_PI should be replaced by np.pi
-            expression = expression.replace('M_PI',str(np.pi))
-            #The C++ expressions which can be used are sqrt and pow, the easiest solution is to replace them with np.sqrt and np.power
-            expression = expression.replace('sqrt','np.sqrt')
-            expression = expression.replace('pow','np.power')
-            #Now that variables are numeric we need to evaluate operators
-            variables[varName] = eval(expression) #Maybe eval is not the best choice here but the input should be sufficiently cleaned by now
-        except (NameError,SyntaxError):
-            pass
-    return
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Feb 27 22:36:21 2023
+
+@author: CSChisholm
+
+#These functions are primarily used for reading data generated by XMDS2
+# (http://xmds.org).
+#ParseXSIL is very specific to getting metadata out of the .xsil file generated
+# by XMDS2.
+#ReadH5 will load all of the outputs defined in XMDS2 into a Python dictionary
+# but will also read any other HDF5 file into a dictionary.
+#Likewise, WriteH5 will write any dictionary into an HDF5 file.
+"""
+
+import h5py
+import xml.etree.ElementTree as ET
+import numpy as np
+import re
+
+def ReadH5(filename: str) -> dict:
+    '''Opens hdf5 file and converts every group and subgroup into a dictionary
+    where the keys are the group keys and the items are the datasets
+    
+    return data'''
+    #Open file
+    with h5py.File(filename,'r') as f:
+        data = {}
+        _Group2Dict(f,data)
+    return data
+
+def WriteH5(filename: str, data: dict):
+    '''Takes dictionary and writes hdf5 file using keys as keys and items as
+    datasets if they are not dictionaries or groups if they are dictionaries'''
+    if not(isinstance(data,dict)):
+        raise TypeError(f'Data must be a dictionary. Got type: {type(data)}.')
+    with h5py.File(filename,'w') as f:
+        _Dict2Group(f,data)
+    return
+
+def ParseXSIL(xsilFile: str) -> dict:
+    ''''Parse most of the data from a .xsil file (XMDS2) into a dictionary. We don't need geometry or output because they are in the corresponding .h5 file.
+    
+    return data'''
+    data = {'Filename': xsilFile} #Construct dictionary
+    variables = {} #The variable definitions, will later be added to data
+    comments = {} #Store the C++ comments as strings
+    vectors = {} #Defined vectors (potential, initialisation etc.)
+    operators = {} #Operators for FFT in split-step
+    equations = {} #The differential equation(s) being solved
+    axes = {}
+    xmlData = ET.parse(xsilFile).getroot() #Load XML
+    children = [child.tag for child in xmlData]
+    data['Name'] = _SearchElement('name',xmlData,children).text #Get program name
+    data['Description'] = _SearchElement('description',xmlData,children).text
+    #We also want the file as a string so that we can access <![CDATA[ blocks
+    with open(xsilFile,'r') as f:
+        lines = f.readlines()
+    #Search for vectors
+    numVecs = len(np.where(np.array(children)=='vector')[0])
+    for II in range(numVecs):
+        vec = _SearchElement('vector',xmlData,children,index=II)
+        name = vec.attrib['name']
+        if not('kind' in vec[1].attrib.keys()):
+            vectors[name] = [line for line in vec[1].text.split('\n') if '=' in line][0]
+        else: #Initialised from hdf5 file
+            vectors[name] = vec[1][0].text #Just put the file name here
+    data['Vectors'] = vectors
+    #Look in the sequence for operators, differential equations, and breakpoint
+    sequence = _SearchElement('sequence',xmlData,children)
+    try:
+        data['Breakfile'] = _SearchElement('breakpoint',sequence).attrib['filename']
+    except IndexError:
+        data['Breakfile'] = None #no break file
+    integrate = _SearchElement('integrate',sequence)
+    data['Parameters'] = integrate.attrib
+    operatorsIndex = [II for II, line in enumerate(lines) if '<operator_names>' in line][0]
+    itr = operatorsIndex
+    while not(']]>' in lines[itr]):
+        if ('=' in lines[itr]):
+            linesplit = lines[itr].split(' = ')
+            operators[linesplit[0].split(' ')[-1]] = linesplit[1].split(';')[0]
+        itr+=1
+    data['Operators'] = operators
+    equationsIndex = [II for II, line in enumerate(lines) if '<integration_vectors>' in line][0]
+    itr = equationsIndex
+    while not(']]>' in lines[itr]):
+        if ('=' in lines[itr]):
+            linesplit = lines[itr].split(' = ')
+            equations[linesplit[0].split(' ')[-1]] = linesplit[1].split(';')[0]
+        itr+=1
+    data['Equations'] = equations
+    #Search for command line arguments and store them in dict: variables
+    info = _SearchElement('info',xmlData,children).text.split('\n')
+    clargs = [line for line in info if 'Command line argument' in line]
+    for clarg in clargs:
+        definition = clarg.split('Command line argument ')[1]
+        _GetVar(definition,variables)
+        comments[definition.split(' = ')[0]] = 'Command line argument'
+    #Get global variables
+    features = _SearchElement('features',xmlData,children)
+    globalvars = _SearchElement('globals',features).text.split('\n')
+    globaldefs = [globalvar for globalvar in globalvars if 'const real' in globalvar]
+    for globaldef in globaldefs:
+        definition = globaldef.split('real ')[1].split(';')[0]
+        _GetVar(definition,variables)
+        if ('//' in globaldef):
+            comments[definition.split(' = ')[0]] = globaldef.split('//')[1]
+    #Get variables derived from command line arguments and globals
+    subLines = [II for II, line in enumerate(lines) if '<arguments>' in line]
+    if (len(subLines)):
+        derivedIndex = subLines[0]
+        itr = derivedIndex
+        while not((']]>' in lines[itr]) or ('</features>' in lines[itr])):
+            if (('=' in lines[itr]) and not('default_value' in lines[itr])):
+                line = lines[itr].replace(' ','').replace('=',' = ')
+                _GetVar(line.split(';')[0],variables)
+                if ('//' in line):
+                    comments[line.split(' = ')[0]] = line.split('//')[1]
+            itr+=1
+    data['Variables'] = variables
+    data['Comments'] = comments
+    geometry = _SearchElement('geometry',xmlData,children)
+    transverseDimensions = _SearchElement('transverse_dimensions',geometry)
+    for dimension in transverseDimensions:
+        axes[dimension.attrib['name']] = {key: value for key, value in dimension.attrib.items() if not key=='name'}
+    data['Axes'] = axes
+    for key in data['Axes'].keys():
+        if (('transform', 'bessel') in data['Axes'][key].items()):
+            data['Variables'][f'{key}Outer'] = float(data['Axes'][key]['domain'].split(', ')[1].split(')')[0])
+    return data
+
+def _Group2Dict(h5Group,data):
+    '''Helper function for ReadH5'''
+    keys = [key for key in h5Group]
+    for key in keys:
+        if (isinstance(h5Group[key],h5py.Dataset)):
+            data[key] = h5Group[key][()]
+        else:
+            data[key] = {}
+            _Group2Dict(h5Group[key],data[key])
+    return
+
+def _Dict2Group(h5group,data):
+    '''Helper function for WriteH5'''
+    keys = data.keys()
+    for key in keys:
+        if (isinstance(data[key],dict)):
+            group = h5group.create_group(key)
+            _Dict2Group(group,data[key])
+        else:
+            h5group[key] = data[key]
+    return
+
+def _SearchElement(tag, root, tags=None,index=0):
+    '''Search for the index of an xml element with a given tag.
+    If the tag appears more than once in list(root) then the optional argument,
+    index, can be used to choose which one to take
+    Helper function for ParseXSIL
+    
+    return element'''
+    if (tags is None):
+        tags = [child.tag for child in root]
+    ind = np.where(np.array(tags)==tag)[0][index]
+    return root[ind]
+
+def _GetVar(definition, variables):
+    '''From a string, return a numeric definition of a variable,
+    using previously evaluated variables if necessary
+    Helper function for ParseXSIL'''
+    splitDef = definition.split(' = ')
+    varName = splitDef[0].replace(' ','')
+    try:
+        variables[varName] = float(splitDef[1])
+    except ValueError:
+        try:
+            #We need to evaluate an expression
+            expression = splitDef[1]
+            #Variables are defined sequentially so any variable used in the expression already exists
+            #Double pass on string replacement in case some variables contain other variables within their names
+            expSplit = re.split('\*|/|\+|\-|\)|\(',expression)
+            for part in expSplit:
+                if (part in variables.keys()):
+                    expression = expression.replace(part,str(variables[part]))
+            for key in variables.keys():
+                expression = expression.replace(key,str(variables[key]))
+            #We also know that M_PI should be replaced by np.pi
+            expression = expression.replace('M_PI',str(np.pi))
+            #The C++ expressions which can be used are sqrt and pow, the easiest solution is to replace them with np.sqrt and np.power
+            expression = expression.replace('sqrt','np.sqrt')
+            expression = expression.replace('pow','np.power')
+            #Now that variables are numeric we need to evaluate operators
+            variables[varName] = eval(expression) #Maybe eval is not the best choice here but the input should be sufficiently cleaned by now
+        except (NameError,SyntaxError):
+            pass
+    return
```

### Comparing `xmds2tools-1.0.0/src/xmds2tools.egg-info/PKG-INFO` & `xmds2tools-1.0.1/src/xmds2tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1
-Name: xmds2tools
-Version: 1.0.0
-Summary: Tools to read .hdf5 and .xsil files generated using XMDS2 and functions to implement Bessel transformations and Bessel quadrature integration
-Author-email: Craig Chisholm <craig.chisholm@protonmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Craig Chisholm
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/CSChisholm/xmds2-tools
-Keywords: XMDS2,HDF5,Bessel
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# xmds2-tools
-Tools to read .hdf5 and .xsil files generated using [XMDS2](http://xmds.org) and functions to implement Bessel transformations and Bessel quadrature integration
-
-These tools were built to work with the output files generated by XMDS2 but can be used for other purposes.
-
-The function `reader.ReadH5` reads any [HDF5 file](https://www.hdfgroup.org/solutions/hdf5/) and returns the contents as a Python dictionary. Likewise, `reader.WriteH5` takes a Python dictionary and saves the contents as an HDF5 file.
-
-XMDS2 simulations generate a text file with extension `.xsil` as well as the HDF5 data. The function 'reader.ParseXSIL' reads the XML data from the text file and returns a dictionary with simulation parameters including global variables, command line variables, and variables derived from global and command line variables. If the Bessel transform is used on an axis a variable called `"axis name"Outer` is added where `"axis name"` is the name of the axis defined in XMDS and the value of the variable is the outer radius of the interval defining the grid.
-
-The `bessel.py` module is based on [Numerical calculation of dipolar-quantum-droplet stationary states](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013283) and implements Bessel quadrature integration and numerical radial derivative in cylindrical coordinates.
-
-## Examples
-The `examples/` folder contains Python scripts demonstrating the use of the `reader` and `bessel` modules to analyse the output of some of the XMDS2 examples. The `bessel` module is also used for quadrature integration and compared to the trapezium method.
-
-None of the examples or any of the XMDS2 source code is reproduced here and the user is instead refered to the [XMDS2 website](http://xmds.org')
-
-* `examples/groundstate_workedexamples.py` corresponds to the continuous renormalisation groundstate example.
-* `examples/bc_groundstate.py` corresponds to the imaginary time evolution example using DCT and Bessel transform in the XMDS directory `examples/bessel_cosine_groundstate.xmds`
-* `examples/bessel_integration.py` compares convergence when integrating using the trapezium method and by Bessel quadrature
-
-## Installation
-
-### Install from PyPI
-
-* `python -m pip install xmds2tools`
-
-### Build from source
-* `python -m pip install --upgrade pip setuptools`
-* `python -m pip install build`
-* `git clone https://github.com/CSChisholm/xmds2-tools`
-* `cd xmds2-tools`
-* `python -m build`
-
-## Acknowledgements
-
-These functions were written and tested during the PhD project of C. S. Chisholm at [ICFO - The Institute of Photonic Sciences](https://www.icfo.eu/) under the supervision of Prof. Dr. Leticia Tarruell and with support from Dr. Ramón Ramos.
-
-Thanks to Prof. P. B. Blakie, Dr. M. Johnsson, and Prof. M. J. Davis for advice.
-
-## References
-
-1. G. R. Dennis, J. J. Hope, and M. T. Johnsson, [*XMDS2: Fast, scalable simulation of coupled stochastic partial differential equations*](https://doi.org/10.1016/j.cpc.2012.08.016). Compuer Physics Communications **184**(1), 201-208 (2013).
-2. A.-C. Lee, D. Baillie, and P. B. Blakie, [*Numerical calculation of dipolar-quantum-droplet stationary states*](https://doi.org/10.1103/PhysRevResearch.3.013283). Physical Review Research **3**, 013283 (2021).
+Metadata-Version: 2.1
+Name: xmds2tools
+Version: 1.0.1
+Summary: Tools to read .hdf5 and .xsil files generated using XMDS2 and functions to implement Bessel transformations and Bessel quadrature integration
+Author-email: Craig Chisholm <craig.chisholm@protonmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Craig Chisholm
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/CSChisholm/xmds2-tools
+Keywords: XMDS2,HDF5,Bessel
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# xmds2-tools
+Tools to read .hdf5 and .xsil files generated using [XMDS2](http://xmds.org) and functions to implement Bessel transformations and Bessel quadrature integration
+
+These tools were built to work with the output files generated by XMDS2 but can be used for other purposes.
+
+The function `reader.ReadH5` reads any [HDF5 file](https://www.hdfgroup.org/solutions/hdf5/) and returns the contents as a Python dictionary. Likewise, `reader.WriteH5` takes a Python dictionary and saves the contents as an HDF5 file.
+
+XMDS2 simulations generate a text file with extension `.xsil` as well as the HDF5 data. The function `reader.ParseXSIL` reads the XML data from the text file and returns a dictionary with simulation parameters including global variables, command line variables, and variables derived from global and command line variables. If the Bessel transform is used on an axis a variable called `"axis name"Outer` is added where `"axis name"` is the name of the axis defined in XMDS and the value of the variable is the outer radius of the interval defining the grid.
+
+The `bessel.py` module is based on [Numerical calculation of dipolar-quantum-droplet stationary states](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013283) and implements Bessel quadrature integration and numerical radial derivative in cylindrical coordinates.
+
+## Examples
+The `examples/` folder contains Python scripts demonstrating the use of the `reader` and `bessel` modules to analyse the output of some of the XMDS2 examples. The `bessel` module is also used for quadrature integration and compared to the trapezium method.
+
+None of the examples or any of the XMDS2 source code is reproduced here and the user is instead refered to the [XMDS2 website](http://xmds.org')
+
+* `examples/groundstate_workedexamples.py` corresponds to the continuous renormalisation groundstate example.
+* `examples/bc_groundstate.py` corresponds to the imaginary time evolution example using DCT and Bessel transform in the XMDS directory `examples/bessel_cosine_groundstate.xmds`
+* `examples/bessel_integration.py` compares convergence when integrating using the trapezium method and by Bessel quadrature
+
+## Installation
+
+### Install from [PyPI](https://pypi.org/project/xmds2tools/1.0.1/)
+
+* `python -m pip install xmds2tools`
+
+### Build from source
+* `python -m pip install --upgrade pip setuptools`
+* `python -m pip install build`
+* `git clone https://github.com/CSChisholm/xmds2-tools`
+* `cd xmds2-tools`
+* `python -m build`
+
+## Acknowledgements
+
+These functions were written and tested during the PhD project of C. S. Chisholm at [ICFO - The Institute of Photonic Sciences](https://www.icfo.eu/) under the supervision of Prof. Dr. Leticia Tarruell and with support from Dr. Ramón Ramos.
+
+Thanks to Prof. P. B. Blakie, Dr. M. T. Johnsson, and Prof. M. J. Davis for advice.
+
+## References
+
+1. G. R. Dennis, J. J. Hope, and M. T. Johnsson, [*XMDS2: Fast, scalable simulation of coupled stochastic partial differential equations*](https://doi.org/10.1016/j.cpc.2012.08.016). Computer Physics Communications **184**(1), 201-208 (2013).
+2. A.-C. Lee, D. Baillie, and P. B. Blakie, [*Numerical calculation of dipolar-quantum-droplet stationary states*](https://doi.org/10.1103/PhysRevResearch.3.013283). Physical Review Research **3**, 013283 (2021).
```

