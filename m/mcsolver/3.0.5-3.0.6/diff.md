# Comparing `tmp/mcsolver-3.0.5.tar.gz` & `tmp/mcsolver-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mcsolver-3.0.5.tar", last modified: Thu Jun 29 12:39:50 2023, max compression
+gzip compressed data, was "dist\mcsolver-3.0.6.tar", last modified: Wed Aug  2 03:28:20 2023, max compression
```

## Comparing `mcsolver-3.0.5.tar` & `mcsolver-3.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.270010 mcsolver-3.0.5/
--rw-rw-rw-   0        0        0    35823 2019-12-13 12:05:28.000000 mcsolver-3.0.5/LICENSE
--rw-rw-rw-   0        0        0       72 2021-05-31 04:17:53.000000 mcsolver-3.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8459 2023-06-29 12:39:50.269009 mcsolver-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6979 2023-05-24 09:15:09.000000 mcsolver-3.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.226011 mcsolver-3.0.5/mcsolver/
--rw-rw-rw-   0        0        0    14449 2023-05-23 15:54:54.000000 mcsolver-3.0.5/mcsolver/Lattice.py
--rw-rw-rw-   0        0        0    18263 2023-05-26 06:04:35.000000 mcsolver-3.0.5/mcsolver/WannierKit.py
--rw-rw-rw-   0        0        0      536 2023-05-23 16:29:59.000000 mcsolver-3.0.5/mcsolver/__init__.py
--rw-rw-rw-   0        0        0     8390 2023-05-22 11:26:05.000000 mcsolver-3.0.5/mcsolver/auxiliary.py
--rw-rw-rw-   0        0        0    13828 2023-05-23 14:42:07.000000 mcsolver-3.0.5/mcsolver/fileio.py
--rw-rw-rw-   0        0        0    18944 2023-05-26 06:02:12.000000 mcsolver-3.0.5/mcsolver/guiMain.py
--rw-rw-rw-   0        0        0    14059 2023-06-05 04:40:28.000000 mcsolver-3.0.5/mcsolver/guiPyQt5.py
--rw-rw-rw-   0        0        0     4020 2023-06-05 04:16:17.000000 mcsolver-3.0.5/mcsolver/guiPyQt5_toolbox.py
--rw-rw-rw-   0        0        0    40306 2023-06-29 11:28:12.000000 mcsolver-3.0.5/mcsolver/heisenbergLib.c
--rw-rw-rw-   0        0        0     1185 2023-06-24 17:02:47.000000 mcsolver-3.0.5/mcsolver/input.py
--rw-rw-rw-   0        0        0    11504 2021-01-21 13:51:41.000000 mcsolver-3.0.5/mcsolver/interface2swt.py
--rw-rw-rw-   0        0        0    25937 2023-06-29 12:13:05.000000 mcsolver-3.0.5/mcsolver/isingLib.c
--rw-rw-rw-   0        0        0    36491 2023-06-24 17:13:23.000000 mcsolver-3.0.5/mcsolver/mcMain.py
--rw-rw-rw-   0        0        0     3540 2019-12-14 04:31:12.000000 mcsolver-3.0.5/mcsolver/toolbox.py
--rw-rw-rw-   0        0        0     8720 2023-06-24 16:02:37.000000 mcsolver-3.0.5/mcsolver/win.py
--rw-rw-rw-   0        0        0    36085 2023-06-29 11:59:05.000000 mcsolver-3.0.5/mcsolver/xyLib.c
-drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.258013 mcsolver-3.0.5/mcsolver.egg-info/
--rw-rw-rw-   0        0        0     8459 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-06-29 12:39:50.000000 mcsolver-3.0.5/mcsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 12:39:49.000000 mcsolver-3.0.5/mcsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 12:39:50.270010 mcsolver-3.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1384 2023-06-29 12:22:19.000000 mcsolver-3.0.5/setup.py
--rw-rw-rw-   0        0        0      974 2023-06-29 12:37:50.000000 mcsolver-3.0.5/setup2.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:39:50.268007 mcsolver-3.0.5/test/
--rw-rw-rw-   0        0        0      283 2023-05-25 14:57:33.000000 mcsolver-3.0.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:28:20.376157 mcsolver-3.0.6/
+-rw-rw-rw-   0        0        0    35823 2019-12-13 12:05:28.000000 mcsolver-3.0.6/LICENSE
+-rw-rw-rw-   0        0        0       72 2021-05-31 04:17:53.000000 mcsolver-3.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     8459 2023-08-02 03:28:20.375159 mcsolver-3.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6979 2023-05-24 09:15:09.000000 mcsolver-3.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 03:28:20.335156 mcsolver-3.0.6/mcsolver/
+-rw-rw-rw-   0        0        0    14449 2023-05-23 15:54:54.000000 mcsolver-3.0.6/mcsolver/Lattice.py
+-rw-rw-rw-   0        0        0    18263 2023-05-26 06:04:35.000000 mcsolver-3.0.6/mcsolver/WannierKit.py
+-rw-rw-rw-   0        0        0      536 2023-05-23 16:29:59.000000 mcsolver-3.0.6/mcsolver/__init__.py
+-rw-rw-rw-   0        0        0     8390 2023-05-22 11:26:05.000000 mcsolver-3.0.6/mcsolver/auxiliary.py
+-rw-rw-rw-   0        0        0    13828 2023-05-23 14:42:07.000000 mcsolver-3.0.6/mcsolver/fileio.py
+-rw-rw-rw-   0        0        0    18944 2023-05-26 06:02:12.000000 mcsolver-3.0.6/mcsolver/guiMain.py
+-rw-rw-rw-   0        0        0    14059 2023-06-05 04:40:28.000000 mcsolver-3.0.6/mcsolver/guiPyQt5.py
+-rw-rw-rw-   0        0        0     4020 2023-06-05 04:16:17.000000 mcsolver-3.0.6/mcsolver/guiPyQt5_toolbox.py
+-rw-rw-rw-   0        0        0    40332 2023-08-02 03:03:51.000000 mcsolver-3.0.6/mcsolver/heisenbergLib.c
+-rw-rw-rw-   0        0        0     1185 2023-06-24 17:02:47.000000 mcsolver-3.0.6/mcsolver/input.py
+-rw-rw-rw-   0        0        0    11504 2021-01-21 13:51:41.000000 mcsolver-3.0.6/mcsolver/interface2swt.py
+-rw-rw-rw-   0        0        0    25989 2023-08-02 03:07:19.000000 mcsolver-3.0.6/mcsolver/isingLib.c
+-rw-rw-rw-   0        0        0    36491 2023-06-24 17:13:23.000000 mcsolver-3.0.6/mcsolver/mcMain.py
+-rw-rw-rw-   0        0        0     3540 2019-12-14 04:31:12.000000 mcsolver-3.0.6/mcsolver/toolbox.py
+-rw-rw-rw-   0        0        0     8720 2023-06-24 16:02:37.000000 mcsolver-3.0.6/mcsolver/win.py
+-rw-rw-rw-   0        0        0    36111 2023-08-02 03:06:32.000000 mcsolver-3.0.6/mcsolver/xyLib.c
+drwxrwxrwx   0        0        0        0 2023-08-02 03:28:20.365159 mcsolver-3.0.6/mcsolver.egg-info/
+-rw-rw-rw-   0        0        0     8459 2023-08-02 03:28:20.000000 mcsolver-3.0.6/mcsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-08-02 03:28:20.000000 mcsolver-3.0.6/mcsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 03:28:20.000000 mcsolver-3.0.6/mcsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 03:28:20.000000 mcsolver-3.0.6/mcsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 03:28:20.000000 mcsolver-3.0.6/mcsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 03:28:20.376157 mcsolver-3.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1384 2023-08-02 03:27:48.000000 mcsolver-3.0.6/setup.py
+-rw-rw-rw-   0        0        0      974 2023-08-02 03:27:41.000000 mcsolver-3.0.6/setup2.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:28:20.373152 mcsolver-3.0.6/test/
+-rw-rw-rw-   0        0        0      283 2023-05-25 14:57:33.000000 mcsolver-3.0.6/test/test.py
```

### Comparing `mcsolver-3.0.5/LICENSE` & `mcsolver-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/PKG-INFO` & `mcsolver-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mcsolver
-Version: 3.0.5
+Version: 3.0.6
 Summary: A user friendly program to do Monte Carlo sims for magnetic systems
 Home-page: https://github.com/golddoushi/mcsolver
 Author: Liang Liu
 Author-email: liangliu@main.sdu.edu.cn
 License: UNKNOWN
 Description: # mcsolver
         A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
```

### Comparing `mcsolver-3.0.5/README.md` & `mcsolver-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/Lattice.py` & `mcsolver-3.0.6/mcsolver/Lattice.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/WannierKit.py` & `mcsolver-3.0.6/mcsolver/WannierKit.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/__init__.py` & `mcsolver-3.0.6/mcsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/auxiliary.py` & `mcsolver-3.0.6/mcsolver/auxiliary.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/fileio.py` & `mcsolver-3.0.6/mcsolver/fileio.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/guiMain.py` & `mcsolver-3.0.6/mcsolver/guiMain.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/guiPyQt5.py` & `mcsolver-3.0.6/mcsolver/guiPyQt5.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/guiPyQt5_toolbox.py` & `mcsolver-3.0.6/mcsolver/guiPyQt5_toolbox.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/heisenbergLib.c` & `mcsolver-3.0.6/mcsolver/heisenbergLib.c`

 * *Files 1% similar despite different names*

```diff
@@ -590,15 +590,15 @@
     if (algorithm==1) p_mcUpdate=blockUpdate;
 
     // set diagonal dot version
     p_diagonalDot=diagonalDot;
     if (ignoreNonDiagonalJ>0) p_diagonalDot=diagonalDot_simple;
     
     // initialize lattice
-    Orb lattice[totOrbs];
+    Orb *lattice=(Orb*)malloc(totOrbs*sizeof(Orb));
     //printf("hello here is C lib\n");
     establishLattice(lattice, totOrbs, initSpin, initD, h, flunc, maxNLinking, nlink, linkStrength, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
     double energy=0;
     double *p_energy=&energy;
```

### Comparing `mcsolver-3.0.5/mcsolver/input.py` & `mcsolver-3.0.6/mcsolver/input.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/interface2swt.py` & `mcsolver-3.0.6/mcsolver/interface2swt.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/isingLib.c` & `mcsolver-3.0.6/mcsolver/isingLib.c`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
                    int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs*maxNLinking], int linkedOrb[totOrbs*maxNLinking],
                    int ninterval, int nLat, int corrOrbPair[nLat][2], double h,
                    int renormOn, int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking],
                    int spinFrame){
     //printf("hello block algorithm!\n");
     // initialize lattice including one ghost spin
     //totOrbs+=1;
-    Orb lattice[totOrbs];
+    Orb *lattice=(Orb*)malloc(totOrbs*sizeof(Orb));
     //establishLatticeWithGhost(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength, h, totOrb_rnorm, rOrb);
     //establishLinkingWithGhost(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
     establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
     double energy=0, totSpin=0, energy_rnorm=0;
@@ -365,15 +365,15 @@
 
 PyObject * localUpdateMC(int totOrbs, double initSpin[totOrbs], int nthermal, int nsweep, 
                    int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs*maxNLinking], int linkedOrb[totOrbs*maxNLinking],
                    int ninterval, int nLat, int corrOrbPair[nLat][2], double h,
                    int renormOn, int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm*nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm*maxNLinking],
                    int spinFrame){
     // initialize lattice 
-    Orb lattice[totOrbs];
+    Orb *lattice=(Orb*)malloc(totOrbs*sizeof(Orb));
     establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
     double energy=0, totSpin=0, energy_rnorm=0;;
     double *p_energy=&energy, *p_totSpin=&totSpin, *p_energy_rnorm=&energy_rnorm;
     for(int i=0;i<ninterval;i++) totSpin+=initSpin[i];
```

### Comparing `mcsolver-3.0.5/mcsolver/mcMain.py` & `mcsolver-3.0.6/mcsolver/mcMain.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/toolbox.py` & `mcsolver-3.0.6/mcsolver/toolbox.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/win.py` & `mcsolver-3.0.6/mcsolver/win.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/mcsolver/xyLib.c` & `mcsolver-3.0.6/mcsolver/xyLib.c`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
     if(algorithm==1) p_mcUpdate=blockUpdate;
 
     // set diagonal dot function
     p_diagonalDot=diagonalDot;
     if (ignoreNonDiagonalJ>0) p_diagonalDot=diagonalDot_simple;
 
     // initialize lattice add one ghost spin for mimicing external field
-    Orb lattice[totOrbs];
+    Orb *lattice=(Orb*)malloc(totOrbs*sizeof(Orb));
     //printf("hello here is C lib\n");
     establishLattice(lattice, totOrbs, initSpin, initD, flunc, maxNLinking, nlink, linkStrength, h, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
     double energy=0;
     double *p_energy=&energy;
```

### Comparing `mcsolver-3.0.5/mcsolver.egg-info/PKG-INFO` & `mcsolver-3.0.6/mcsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mcsolver
-Version: 3.0.5
+Version: 3.0.6
 Summary: A user friendly program to do Monte Carlo sims for magnetic systems
 Home-page: https://github.com/golddoushi/mcsolver
 Author: Liang Liu
 Author-email: liangliu@main.sdu.edu.cn
 License: UNKNOWN
 Description: # mcsolver
         A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
```

### Comparing `mcsolver-3.0.5/mcsolver.egg-info/SOURCES.txt` & `mcsolver-3.0.6/mcsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.5/setup.py` & `mcsolver-3.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 isingLib=Extension('isinglib',sources=['./mcsolver/isingLib.c'],language='c',extra_compile_args=['-std=c99','-fPIC','-O3'])
 xyLib=Extension('xylib',sources=['./mcsolver/xyLib.c'],language='c',extra_compile_args=['-std=c99','-fPIC','-O3'])
 heisenbergLib=Extension('heisenberglib',sources=['./mcsolver/heisenbergLib.c'],language='c',extra_compile_args=['-std=c99','-fPIC','-O3'])
 
 setup(
     name="mcsolver",
-    version="3.0.5",
+    version="3.0.6",
     author="Liang Liu",
     author_email="liangliu@main.sdu.edu.cn",
     description="A user friendly program to do Monte Carlo sims for magnetic systems",
     long_description=long_description,
     #long_description_content_type="text/markdown",
     url="https://github.com/golddoushi/mcsolver",
     packages=["mcsolver"],
```

### Comparing `mcsolver-3.0.5/setup2.py` & `mcsolver-3.0.6/setup2.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mcsolver",
-    version="3.0.5",
+    version="3.0.6",
     author="Liang Liu",
     author_email="liangliu@main.sdu.edu.cn",
     description="A user friendly program to do Monte Carlo sims for magnetic systems",
     long_description=long_description,
     python_requires='>=3.7',
     install_requires = ['matplotlib','numpy'],
     url="https://github.com/golddoushi/mcsolver",
```

