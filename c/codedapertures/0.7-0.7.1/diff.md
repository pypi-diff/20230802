# Comparing `tmp/codedapertures-0.7.tar.gz` & `tmp/codedapertures-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.7.tar", last modified: Sun Jul 30 03:45:31 2023, max compression
+gzip compressed data, was "codedapertures-0.7.1.tar", last modified: Wed Aug  2 01:31:18 2023, max compression
```

## Comparing `codedapertures-0.7.tar` & `codedapertures-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-30 03:45:31.652292 codedapertures-0.7/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.7/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-30 03:45:31.652187 codedapertures-0.7/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     2041 2023-07-29 01:49:47.000000 codedapertures-0.7/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-30 03:45:31.651286 codedapertures-0.7/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.7/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    31890 2023-07-30 03:30:23.000000 codedapertures-0.7/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-30 03:45:31.652033 codedapertures-0.7/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.7/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       40 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-30 03:45:31.652321 codedapertures-0.7/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      923 2023-07-30 03:44:00.000000 codedapertures-0.7/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-08-02 01:31:18.275516 codedapertures-0.7.1/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.7.1/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      722 2023-08-02 01:31:18.275410 codedapertures-0.7.1/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     2041 2023-07-29 01:49:47.000000 codedapertures-0.7.1/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-08-02 01:31:18.274504 codedapertures-0.7.1/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.7.1/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)    32071 2023-08-02 01:26:33.000000 codedapertures-0.7.1/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-08-02 01:31:18.275256 codedapertures-0.7.1/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      722 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.7.1/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       40 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-08-02 01:31:18.000000 codedapertures-0.7.1/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-08-02 01:31:18.275550 codedapertures-0.7.1/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      925 2023-08-02 01:29:51.000000 codedapertures-0.7.1/setup.py
```

### Comparing `codedapertures-0.7/LICENSE` & `codedapertures-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.7/PKG-INFO` & `codedapertures-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.7
+Version: 0.7.1
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.7/README.md` & `codedapertures-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `codedapertures-0.7/codedapertures/codedapertures.py` & `codedapertures-0.7.1/codedapertures/codedapertures.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,17 @@
 
         # determine labels
         self.rx = self.diam
         self.ry = self.diam
         self.l = np.zeros((self.rx,self.ry), dtype=np.int16)
         for i in range(self.rx):
             for j in range(self.ry):
-                self.l[i,j] = (i + r*j) % self.v
+                i_idx = i - self.radius
+                j_idx = j - self.radius
+                self.l[i,j] = (i_idx + self.r*j_idx) % self.v
 
         # calculate mask
         self.mask = np.zeros(self.l.shape, dtype=np.int16)
         for i in range(self.mask.shape[0]):
             for j in range(self.mask.shape[1]):
                 if self.l[i,j] in self.D:
                     self.mask[i,j] = 1
@@ -652,15 +654,17 @@
 
         # determine labels
         self.rx = self.diam
         self.ry = self.diam
         self.l = np.zeros((self.rx,self.ry), dtype=np.int16)
         for i in range(self.rx):
             for j in range(self.ry):
-                self.l[i,j] = (i + self.r*j) % self.v
+                i_idx = i - self.radius
+                j_idx = j - self.radius
+                self.l[i,j] = (i_idx + self.r*j_idx) % self.v
 
         # calculate mask
         self.mask = np.zeros(self.l.shape, dtype=np.int16)
         for i in range(self.mask.shape[0]):
             for j in range(self.mask.shape[1]):
                 if self.l[i,j] in self.D:
                     self.mask[i,j] = 1
```

### Comparing `codedapertures-0.7/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.7.1/codedapertures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.7
+Version: 0.7.1
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.7/setup.py` & `codedapertures-0.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.7',
+      version='0.7.1',
       description='a python package for generating coded apertures',
       long_description='CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
       url='https://github.com/bpops/codedapertures',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
                 'numpy',
```

