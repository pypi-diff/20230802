# Comparing `tmp/pysurfer-0.8.0.tar.gz` & `tmp/pysurfer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysurfer-0.8.0.tar", last modified: Tue Sep 26 19:23:03 2017, max compression
+gzip compressed data, was "dist/pysurfer-0.9.0.tar", last modified: Wed Oct  3 15:35:13 2018, max compression
```

## Comparing `pysurfer-0.8.0.tar` & `pysurfer-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2017-09-26 19:23:03.000000 pysurfer-0.8.0/
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     3356 2016-07-07 18:35:35.000000 pysurfer-0.8.0/setup.py
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)      990 2017-09-26 19:23:03.000000 pysurfer-0.8.0/PKG-INFO
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      188 2017-09-26 19:23:03.000000 pysurfer-0.8.0/setup.cfg
-drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2017-09-26 19:23:03.000000 pysurfer-0.8.0/pysurfer.egg-info/
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        1 2017-09-26 19:23:03.000000 pysurfer-0.8.0/pysurfer.egg-info/dependency_links.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        7 2017-09-26 19:23:03.000000 pysurfer-0.8.0/pysurfer.egg-info/top_level.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      990 2017-09-26 19:23:03.000000 pysurfer-0.8.0/pysurfer.egg-info/PKG-INFO
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        1 2013-01-18 00:14:09.000000 pysurfer-0.8.0/pysurfer.egg-info/not-zip-safe
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      416 2017-09-26 19:23:03.000000 pysurfer-0.8.0/pysurfer.egg-info/SOURCES.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)       44 2017-09-26 19:23:03.000000 pysurfer-0.8.0/pysurfer.egg-info/requires.txt
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)       16 2017-04-24 13:46:53.000000 pysurfer-0.8.0/MANIFEST.in
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     1514 2015-10-28 14:30:18.000000 pysurfer-0.8.0/LICENSE
-drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2017-09-26 19:23:03.000000 pysurfer-0.8.0/surfer/
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     3630 2016-09-14 15:47:24.000000 pysurfer-0.8.0/surfer/_commandline.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     8325 2017-07-20 19:21:03.000000 pysurfer-0.8.0/surfer/io.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)      266 2017-09-26 19:12:05.000000 pysurfer-0.8.0/surfer/__init__.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)    23519 2017-07-20 19:21:03.000000 pysurfer-0.8.0/surfer/utils.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)    44458 2017-07-20 19:21:03.000000 pysurfer-0.8.0/surfer/cm.py
-drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2017-09-26 19:23:03.000000 pysurfer-0.8.0/surfer/tests/
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        0 2015-10-28 14:30:18.000000 pysurfer-0.8.0/surfer/tests/__init__.py
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)    15469 2017-09-26 18:55:24.000000 pysurfer-0.8.0/surfer/tests/test_viz.py
--rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     3193 2017-07-20 19:21:03.000000 pysurfer-0.8.0/surfer/tests/test_utils.py
--rw-r--r--   0 larsoner  (1000) larsoner  (1000)   132226 2017-09-26 18:55:24.000000 pysurfer-0.8.0/surfer/viz.py
-drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2017-09-26 19:23:03.000000 pysurfer-0.8.0/bin/
--rwxrwxr-x   0 larsoner  (1000) larsoner  (1000)     3904 2016-09-14 15:47:24.000000 pysurfer-0.8.0/bin/pysurfer
+drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2018-10-03 15:35:13.000000 pysurfer-0.9.0/
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)       16 2018-10-02 15:08:32.000000 pysurfer-0.9.0/MANIFEST.in
+drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2018-10-03 15:35:13.000000 pysurfer-0.9.0/surfer/
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)   143648 2018-10-02 15:12:17.000000 pysurfer-0.9.0/surfer/viz.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)     3630 2018-10-02 15:03:30.000000 pysurfer-0.9.0/surfer/_commandline.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)    25277 2018-10-02 15:12:17.000000 pysurfer-0.9.0/surfer/utils.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)    44458 2018-10-02 15:08:32.000000 pysurfer-0.9.0/surfer/cm.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)     8325 2018-10-02 15:08:32.000000 pysurfer-0.9.0/surfer/io.py
+drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2018-10-03 15:35:13.000000 pysurfer-0.9.0/surfer/tests/
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)     3443 2018-10-02 15:12:17.000000 pysurfer-0.9.0/surfer/tests/test_utils.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)    16479 2018-10-02 15:12:17.000000 pysurfer-0.9.0/surfer/tests/test_viz.py
+-rw-rw-r--   0 larsoner  (1000) larsoner  (1000)        0 2015-10-28 14:30:18.000000 pysurfer-0.9.0/surfer/tests/__init__.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)      266 2018-10-03 15:18:23.000000 pysurfer-0.9.0/surfer/__init__.py
+drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2018-10-03 15:35:13.000000 pysurfer-0.9.0/bin/
+-rwxr-xr-x   0 larsoner  (1000) larsoner  (1000)     3904 2018-10-02 15:03:30.000000 pysurfer-0.9.0/bin/pysurfer
+drwxr-xr-x   0 larsoner  (1000) larsoner  (1000)        0 2018-10-03 15:35:13.000000 pysurfer-0.9.0/pysurfer.egg-info/
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)        1 2018-10-03 15:35:13.000000 pysurfer-0.9.0/pysurfer.egg-info/dependency_links.txt
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)      975 2018-10-03 15:35:13.000000 pysurfer-0.9.0/pysurfer.egg-info/PKG-INFO
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)       70 2018-10-03 15:35:13.000000 pysurfer-0.9.0/pysurfer.egg-info/requires.txt
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)        7 2018-10-03 15:35:13.000000 pysurfer-0.9.0/pysurfer.egg-info/top_level.txt
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)      426 2018-10-03 15:35:13.000000 pysurfer-0.9.0/pysurfer.egg-info/SOURCES.txt
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)        1 2018-10-03 15:35:01.000000 pysurfer-0.9.0/pysurfer.egg-info/not-zip-safe
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)      975 2018-10-03 15:35:13.000000 pysurfer-0.9.0/PKG-INFO
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)     2643 2018-10-02 15:12:17.000000 pysurfer-0.9.0/setup.py
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)      849 2018-10-03 15:35:13.000000 pysurfer-0.9.0/setup.cfg
+-rw-r--r--   0 larsoner  (1000) larsoner  (1000)     2039 2018-10-02 15:08:32.000000 pysurfer-0.9.0/README.md
+-rw-rw-r--   0 larsoner  (1000) larsoner  (1000)     1514 2015-10-28 14:30:18.000000 pysurfer-0.9.0/LICENSE
```

### Comparing `pysurfer-0.8.0/setup.py` & `pysurfer-0.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,67 +31,41 @@
 MAINTAINER_EMAIL = 'mwaskom@stanford.edu'
 URL = 'http://pysurfer.github.com'
 LICENSE = 'BSD (3-clause)'
 DOWNLOAD_URL = 'https://github.com/nipy/PySurfer'
 VERSION = version
 
 
-def check_dependencies():
-    needed_deps = ["numpy", "scipy", "matplotlib",
-                   "mayavi",
-                   ]
-    missing_deps = []
-    for dep in needed_deps:
-        try:
-            __import__(dep)
-        except ImportError:
-            missing_deps.append(dep)
-
-    if missing_deps:
-        missing = ", ".join(missing_deps)
-        raise ImportError("Missing dependencies: %s" % missing)
-
-
 if __name__ == "__main__":
     if os.path.exists('MANIFEST'):
         os.remove('MANIFEST')
-
-    import sys
-    if not (len(sys.argv) >= 2 and ('--help' in sys.argv[1:] or
-            sys.argv[1] in ('--help-commands',
-                            '--version',
-                            'egg_info',
-                            'clean'))):
-        check_dependencies()
-
     setup(name=DISTNAME,
           maintainer=MAINTAINER,
           include_package_data=True,
           maintainer_email=MAINTAINER_EMAIL,
           description=DESCRIPTION,
           license=LICENSE,
           url=URL,
           version=VERSION,
           download_url=DOWNLOAD_URL,
           long_description=LONG_DESCRIPTION,
           zip_safe=False,  # the package can run out of an .egg file
           classifiers=['Intended Audience :: Science/Research',
                        'Intended Audience :: Developers',
                        'Programming Language :: Python :: 2.7',
-                       'Programming Language :: Python :: 3.3',
-                       'Programming Language :: Python :: 3.4',
-                       'Programming Language :: Python :: 3.5',
+                       'Programming Language :: Python :: 3.6',
+                       'Programming Language :: Python :: 3.7',
                        'License :: OSI Approved',
                        'Programming Language :: Python',
                        'Topic :: Software Development',
                        'Topic :: Scientific/Engineering',
                        'Operating System :: Microsoft :: Windows',
                        'Operating System :: POSIX',
                        'Operating System :: Unix',
                        'Operating System :: MacOS'
                        ],
           platforms='any',
           packages=['surfer', 'surfer.tests'],
           scripts=['bin/pysurfer'],
-          install_requires=['nibabel >= 1.2'],
+          install_requires=['numpy', 'scipy', 'matplotlib', 'nibabel >= 1.2', 'mayavi'],
           extras_require={'save_movie': ['imageio >= 1.5']},
           )
```

### Comparing `pysurfer-0.8.0/PKG-INFO` & `pysurfer-0.9.0/pysurfer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pysurfer
-Version: 0.8.0
+Version: 0.9.0
 Summary: PySurfer: cortical surface visualization using Python.
 Home-page: http://pysurfer.github.com
-Author: Michael Waskom
-Author-email: mwaskom@stanford.edu
+Maintainer: Michael Waskom
+Maintainer-email: mwaskom@stanford.edu
 License: BSD (3-clause)
 Download-URL: https://github.com/nipy/PySurfer
 Description: PySurfer: cortical surface visualization using Python.
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Provides-Extra: save_movie
```

### Comparing `pysurfer-0.8.0/pysurfer.egg-info/PKG-INFO` & `pysurfer-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pysurfer
-Version: 0.8.0
+Version: 0.9.0
 Summary: PySurfer: cortical surface visualization using Python.
 Home-page: http://pysurfer.github.com
-Author: Michael Waskom
-Author-email: mwaskom@stanford.edu
+Maintainer: Michael Waskom
+Maintainer-email: mwaskom@stanford.edu
 License: BSD (3-clause)
 Download-URL: https://github.com/nipy/PySurfer
 Description: PySurfer: cortical surface visualization using Python.
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Provides-Extra: save_movie
```

### Comparing `pysurfer-0.8.0/LICENSE` & `pysurfer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysurfer-0.8.0/surfer/_commandline.py` & `pysurfer-0.9.0/surfer/_commandline.py`

 * *Files identical despite different names*

### Comparing `pysurfer-0.8.0/surfer/io.py` & `pysurfer-0.9.0/surfer/io.py`

 * *Files identical despite different names*

### Comparing `pysurfer-0.8.0/surfer/utils.py` & `pysurfer-0.9.0/surfer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from . import cm as surfer_cm
 
 logger = logging.getLogger('surfer')
 
 
 # Py3k compat
 if sys.version[0] == '2':
-    string_types = basestring  # noqa
+    string_types = basestring  # noqa, analysis:ignore
 else:
     string_types = str
 
 
 if LooseVersion(mayavi.__version__) == LooseVersion('4.5.0'):
     # Monkey-patch Mayavi 4.5:
     # In Mayavi 4.5, filters seem to be missing a .point_data attribute that
@@ -67,35 +67,26 @@
     ----------
     subject_id : string
         Name of subject
     hemi : {'lh', 'rh'}
         Which hemisphere to load
     surf : string
         Name of the surface to load (eg. inflated, orig ...)
-    data_path : string
-        Path where to look for data
-    x: 1d array
-        x coordinates of vertices
-    y: 1d array
-        y coordinates of vertices
-    z: 1d array
-        z coordinates of vertices
-    coords : 2d array of shape [n_vertices, 3]
-        The vertices coordinates
-    faces : 2d array
-        The faces ie. the triangles
-    nn : 2d array
-        Normalized surface normals for vertices.
     subjects_dir : str | None
         If not None, this directory will be used as the subjects directory
         instead of the value set using the SUBJECTS_DIR environment variable.
+    offset : float | None
+        If float, align inside edge of each hemisphere to center + offset.
+        If None, do not change coordinates (default).
+    units : str
+        Can be 'm' or 'mm' (default).
     """
 
     def __init__(self, subject_id, hemi, surf, subjects_dir=None,
-                 offset=None):
+                 offset=None, units='mm'):
         """Surface
 
         Parameters
         ----------
         subject_id : string
             Name of subject
         hemi : {'lh', 'rh'}
@@ -112,22 +103,25 @@
         self.subject_id = subject_id
         self.hemi = hemi
         self.surf = surf
         self.offset = offset
         self.coords = None
         self.faces = None
         self.nn = None
+        self.units = _check_units(units)
 
         subjects_dir = _get_subjects_dir(subjects_dir)
         self.data_path = op.join(subjects_dir, subject_id)
 
     def load_geometry(self):
         surf_path = op.join(self.data_path, "surf",
                             "%s.%s" % (self.hemi, self.surf))
         coords, faces = nib.freesurfer.read_geometry(surf_path)
+        if self.units == 'm':
+            coords /= 1000.
         if self.offset is not None:
             if self.hemi == 'lh':
                 coords[:, 0] -= (np.max(coords[:, 0]) + self.offset)
             else:
                 coords[:, 0] -= (np.min(coords[:, 0]) + self.offset)
         nn = _compute_normals(coords, faces)
 
@@ -136,19 +130,14 @@
             self.faces = faces
             self.nn = nn
         else:
             self.coords[:] = coords
             self.faces[:] = faces
             self.nn[:] = nn
 
-    def save_geometry(self):
-        surf_path = op.join(self.data_path, "surf",
-                            "%s.%s" % (self.hemi, self.surf))
-        nib.freesurfer.write_geometry(surf_path, self.coords, self.faces)
-
     @property
     def x(self):
         return self.coords[:, 0]
 
     @property
     def y(self):
         return self.coords[:, 1]
@@ -339,14 +328,36 @@
         lh = logging.StreamHandler(WrapStdOut())
 
     lh.setFormatter(logging.Formatter(output_format))
     # actually add the stream handler
     logger.addHandler(lh)
 
 
+if hasattr(inspect, 'signature'):  # py35
+    def _get_args(function, varargs=False):
+        params = inspect.signature(function).parameters
+        args = [key for key, param in params.items()
+                if param.kind not in (param.VAR_POSITIONAL, param.VAR_KEYWORD)]
+        if varargs:
+            varargs = [param.name for param in params.values()
+                       if param.kind == param.VAR_POSITIONAL]
+            if len(varargs) == 0:
+                varargs = None
+            return args, varargs
+        else:
+            return args
+else:
+    def _get_args(function, varargs=False):
+        out = inspect.getargspec(function)  # args, varargs, keywords, defaults
+        if varargs:
+            return out[:2]
+        else:
+            return out[0]
+
+
 def verbose(function):
     """Decorator to allow functions to override default log level
 
     Do not call this function directly to set the global verbosity level,
     instead use set_log_level().
 
     Parameters (to decorated function)
@@ -355,15 +366,15 @@
         The level of messages to print. If a str, it can be either DEBUG,
         INFO, WARNING, ERROR, or CRITICAL. Note that these are for
         convenience and are equivalent to passing in logging.DEBUG, etc.
         For bool, True is the same as 'INFO', False is the same as 'WARNING'.
         None defaults to using the current log level [e.g., set using
         mne.set_log_level()].
     """
-    arg_names = inspect.getargspec(function).args
+    arg_names = _get_args(function)
     # this wrap allows decorated functions to be pickled (e.g., for parallel)
 
     @wraps(function)
     def dec(*args, **kwargs):
         # Check if the first arg is "self", if it has verbose, make it default
         if len(arg_names) > 0 and arg_names[0] == 'self':
             default_level = getattr(args[0], 'verbose', None)
@@ -371,15 +382,15 @@
             default_level = None
         verbose_level = kwargs.get('verbose', default_level)
         if verbose_level is not None:
             old_level = set_log_level(verbose_level, True)
             # set it back if we get an exception
             try:
                 ret = function(*args, **kwargs)
-            except:
+            except Exception:
                 set_log_level(old_level)
                 raise
             set_log_level(old_level)
             return ret
         else:
             return function(*args, **kwargs)
 
@@ -388,14 +399,20 @@
 
     return dec
 
 
 ###############################################################################
 # USEFUL FUNCTIONS
 
+def _check_units(units):
+    if units not in ('m', 'mm'):
+        raise ValueError('Units must be "m" or "mm", got %r' % (units,))
+    return units
+
+
 def find_closest_vertices(surface_coords, point_coords):
     """Return the vertices on a surface mesh closest to some given coordinates.
 
     The distance metric used is Euclidian distance.
 
     Parameters
     ----------
@@ -410,33 +427,37 @@
         Array of mesh vertex ids
 
     """
     point_coords = np.atleast_2d(point_coords)
     return np.argmin(cdist(surface_coords, point_coords), axis=0)
 
 
-def tal_to_mni(coords):
+def tal_to_mni(coords, units='mm'):
     """Convert Talairach coords to MNI using the Lancaster transform.
 
     Parameters
     ----------
     coords : n x 3 numpy array
         Array of Talairach coordinates
+    units : str
+        Can be 'm' or 'mm' (default).
 
     Returns
     -------
     mni_coords : n x 3 numpy array
-        Array of coordinates converted to MNI space
-
+        Array of coordinates converted to MNI space.
     """
     coords = np.atleast_2d(coords)
     xfm = np.array([[1.06860, -0.00396, 0.00826,  1.07816],
                     [0.00640,  1.05741, 0.08566,  1.16824],
                     [-0.01281, -0.08863, 1.10792, -4.17805],
                     [0.00000,  0.00000, 0.00000,  1.00000]])
+    units = _check_units(units)
+    if units == 'm':
+        xfm[:3, 3] /= 1000.
     mni_coords = np.dot(np.c_[coords, np.ones(coords.shape[0])], xfm.T)[:, :3]
     return mni_coords
 
 
 def mesh_edges(faces):
     """Returns sparse matrix with edges as an adjacency matrix
 
@@ -460,26 +481,33 @@
     edges = edges + sparse.coo_matrix((np.ones(nfaces), (c, a)),
                                       shape=(npoints, npoints))
     edges = edges + edges.T
     edges = edges.tocoo()
     return edges
 
 
-def create_color_lut(cmap, n_colors=256):
+def create_color_lut(cmap, n_colors=256, center=None):
     """Return a colormap suitable for setting as a Mayavi LUT.
 
     Parameters
     ----------
     cmap : string, list of colors, n x 3 or n x 4 array
         Input colormap definition. This can be the name of a matplotlib
         colormap, a list of valid matplotlib colors, or a suitable
         mayavi LUT (possibly missing the alpha channel).
+
+        if value is "auto", a default sequential or divergent colormap is
+        returned
     n_colors : int, optional
         Number of colors in the resulting LUT. This is ignored if cmap
         is a 2d array.
+    center : double, optional
+        indicates whether desired colormap should be for divergent values,
+        currently only used to select default colormap for cmap='auto'
+
     Returns
     -------
     lut : n_colors x 4 integer array
         Color LUT suitable for passing to mayavi
     """
     if isinstance(cmap, np.ndarray):
         if np.ndim(cmap) == 2:
@@ -489,14 +517,22 @@
             elif cmap.shape[1] == 3:
                 # This looks like a LUT, but it's missing the alpha channel
                 alpha = np.ones(len(cmap), np.int) * 255
                 lut = np.c_[cmap, alpha]
 
             return lut
 
+    # choose default colormaps (REMEMBER to change doc, e.g., in
+    # Brain.add_data, when changing these defaults)
+    if isinstance(cmap, string_types) and cmap == "auto":
+        if center is None:
+            cmap = "rocket"
+        else:
+            cmap = "icefire"
+
     surfer_cmaps = ["rocket", "mako", "icefire", "vlag"]
     surfer_cmaps += [name + "_r" for name in surfer_cmaps]
 
     if not isinstance(cmap, string_types) and isinstance(cmap, Sequence):
         colors = list(map(mpl.colors.colorConverter.to_rgba, cmap))
         cmap = mpl.colors.ListedColormap(colors)
     elif cmap in surfer_cmaps:
@@ -578,15 +614,16 @@
                                           len(vertices)))
 
     return smooth_mat
 
 
 @verbose
 def coord_to_label(subject_id, coord, label, hemi='lh', n_steps=30,
-                   map_surface='white', coord_as_vert=False, verbose=None):
+                   map_surface='white', coord_as_vert=False, units='mm',
+                   verbose=None):
     """Create label from MNI coordinate
 
     Parameters
     ----------
     subject_id : string
         Use if file is in register with subject's orig.mgz
     coord : numpy array of size 3 | int
@@ -597,40 +634,46 @@
         Hemisphere target
     n_steps : int
         Number of dilation iterations
     map_surface : str
         The surface name used to find the closest point
     coord_as_vert : bool
         whether the coords parameter should be interpreted as vertex ids
+    units : str
+        Can be 'm' or 'mm' (default).
     verbose : bool, str, int, or None
         If not None, override default verbose level (see surfer.verbose).
     """
-    geo = Surface(subject_id, hemi, map_surface)
+    geo = Surface(subject_id, hemi, map_surface, units=units)
     geo.load_geometry()
 
+    coords = geo.coords
+    # work in mm from here on
+    if geo.units == 'm':
+        coords = coords * 1000
     if coord_as_vert:
-        coord = geo.coords[coord]
+        coord = coords[coord]
 
-    n_vertices = len(geo.coords)
+    n_vertices = len(coords)
     adj_mat = mesh_edges(geo.faces)
-    foci_vtxs = find_closest_vertices(geo.coords, [coord])
+    foci_vtxs = find_closest_vertices(coords, [coord])
     data = np.zeros(n_vertices)
     data[foci_vtxs] = 1.
     smooth_mat = smoothing_matrix(np.arange(n_vertices), adj_mat, 1)
     for _ in range(n_steps):
         data = smooth_mat * data
     idx = np.where(data.ravel() > 0)[0]
     # Write label
     label_fname = label + '-' + hemi + '.label'
     logger.info("Saving label : %s" % label_fname)
     f = open(label_fname, 'w')
     f.write('#label at %s from subject %s\n' % (coord, subject_id))
     f.write('%d\n' % len(idx))
     for i in idx:
-        x, y, z = geo.coords[i]
+        x, y, z = coords[i]
         f.write('%d  %f  %f  %f 0.000000\n' % (i, x, y, z))
 
 
 def _get_subjects_dir(subjects_dir=None, raise_error=True):
     """Get the subjects directory from parameter or environment variable
 
     Parameters
@@ -675,22 +718,30 @@
             out = 'fsaverage not found in SUBJECTS_DIR: %s' % (fs_dir,)
         elif not op.isdir(surf_dir):
             out = 'fsaverage has no "surf" directory: %s' % (surf_dir,)
     out = (out == '', out) if return_why else (out == '')
     return out
 
 
-def has_imageio():
+def requires_fsaverage():
+    import pytest
+    has, why = has_fsaverage(raise_error=False, return_why=True)
+    return pytest.mark.skipif(
+        not has, reason='Requires fsaverage subject data (%s)' % why)
+
+
+def requires_imageio():
+    import pytest
     try:
-        import imageio  # NOQA
+        from imageio.plugins.ffmpeg import get_exe  # noqa, analysis:ignore
     except ImportError:
-        return False
+        has = False
     else:
-        return True
-
+        has = True
+    return pytest.mark.skipif(not has, reason="Requires imageio with ffmpeg")
 
-_has, _why = has_fsaverage(raise_error=False, return_why=True)
-requires_fsaverage = np.testing.dec.skipif(
-    not _has, 'Requires fsaverage subject data (%s)' % _why)
 
-requires_imageio = np.testing.dec.skipif(not has_imageio(),
-                                         "Requires imageio package")
+def requires_fs():
+    import pytest
+    has = ('FREESURFER_HOME' in os.environ)
+    return pytest.mark.skipif(
+        not has, reason='Requires FreeSurfer command line tools')
```

### Comparing `pysurfer-0.8.0/surfer/cm.py` & `pysurfer-0.9.0/surfer/cm.py`

 * *Files identical despite different names*

### Comparing `pysurfer-0.8.0/surfer/tests/test_viz.py` & `pysurfer-0.9.0/surfer/tests/test_viz.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,107 @@
 import os
 import os.path as op
 from os.path import join as pjoin
-import shutil
 import sys
-from tempfile import mkdtemp, mktemp
 import warnings
 
-from nose.tools import assert_equal, assert_in, assert_not_in
-from nose.plugins.skip import SkipTest
+import pytest
 from mayavi import mlab
 import nibabel as nib
 import numpy as np
-from numpy.testing import assert_raises, assert_array_equal
+from numpy.testing import assert_array_equal, assert_array_less
+
+from unittest import SkipTest
 
 from surfer import Brain, io, utils
-from surfer.utils import requires_fsaverage, requires_imageio
+from surfer.utils import requires_fsaverage, requires_imageio, requires_fs
 
 warnings.simplefilter('always')
 
 subject_id = 'fsaverage'
 std_args = [subject_id, 'lh', 'inflated']
 data_dir = pjoin(op.dirname(__file__), '..', '..', 'examples', 'example_data')
 
 overlay_fname = pjoin(data_dir, 'lh.sig.nii.gz')
 
 
-def has_freesurfer():
-    if 'FREESURFER_HOME' not in os.environ:
-        return False
-    else:
-        return True
-
-
-requires_fs = np.testing.dec.skipif(not has_freesurfer(),
-                                    'Requires FreeSurfer command line tools')
-
-
 def _set_backend(backend=None):
     """Use testing backend for Windows."""
+    only_test = (sys.platform == 'win32' or
+                 (os.getenv('TRAVIS', 'false') == 'true' and
+                  sys.platform == 'linux') and sys.version[0] == '3')
     if backend is None:
-        backend = 'test' if sys.platform == 'win32' else 'auto'
-    else:
-        if backend != 'test' and sys.platform == 'win32':
-            raise SkipTest('non-testing backend crashes on Windows')
+        backend = 'test' if only_test else 'auto'
+    if only_test and backend != 'test':
+        raise SkipTest('non-testing backend crashes on Windows and '
+                       'Travis Py3k')
     mlab.options.backend = backend
 
 
-@requires_fsaverage
+def get_view(brain):
+    """Setup for view persistence test"""
+    fig = brain._figures[0][0]
+    if mlab.options.backend == 'test':
+        return
+    fig.scene.camera.parallel_scale = 50
+    assert fig.scene.camera.parallel_scale == 50
+    view, roll = brain.show_view()
+    return fig.scene.camera.parallel_scale, view, roll
+
+
+def check_view(brain, view):
+    """Test view persistence"""
+    fig = brain._figures[0][0]
+    if mlab.options.backend == 'test':
+        return
+    parallel_scale, view, roll = view
+    assert fig.scene.camera.parallel_scale == parallel_scale
+    view_now, roll_now = brain.show_view()
+    assert view_now[:3] == view[:3]
+    assert_array_equal(view_now[3], view[3])
+    assert roll_now == roll
+
+
+@requires_fsaverage()
 def test_offscreen():
     """Test offscreen rendering."""
-    if sys.platform == 'darwin' and os.getenv('TRAVIS', 'false') == 'true':
-        raise SkipTest('Offscreen Travis tests fail on OSX')
     _set_backend()
     brain = Brain(*std_args, offscreen=True)
-    # Sometimes the first screenshot is rendered with a different
-    # resolution on OS X
-    brain.screenshot()
     shot = brain.screenshot()
-    assert_array_equal(shot.shape, (800, 800, 3))
+    assert_array_less((400, 400, 2), shot.shape)
+    assert_array_less(shot.shape, (801, 801, 4))
     brain.close()
 
 
-@requires_fsaverage
-def test_image():
+@requires_fsaverage()
+def test_image(tmpdir):
     """Test image saving."""
-    tmp_name = mktemp() + '.png'
+    tmp_name = tmpdir.join('temp.png')
+    tmp_name = str(tmp_name)  # coerce to str to avoid PIL error
 
     _set_backend()
     subject_id, _, surf = std_args
     brain = Brain(subject_id, 'both', surf=surf, size=100)
     brain.add_overlay(overlay_fname, hemi='lh', min=5, max=20, sign="pos")
     brain.save_imageset(tmp_name, ['med', 'lat'], 'jpg')
+    brain.close()
 
     brain = Brain(*std_args, size=100)
     brain.save_image(tmp_name)
     brain.save_image(tmp_name, 'rgba', True)
     brain.screenshot()
-    if not sys.platform.startswith('linux') or \
-            os.getenv('TRAVIS', 'false') != 'true':
+    if os.getenv('TRAVIS', '') != 'true':
         # for some reason these fail on Travis sometimes
         brain.save_montage(tmp_name, ['l', 'v', 'm'], orientation='v')
         brain.save_montage(tmp_name, ['l', 'v', 'm'], orientation='h')
         brain.save_montage(tmp_name, [['l', 'v'], ['m', 'f']])
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_brains():
     """Test plotting of Brain with different arguments."""
     # testing backend breaks when passing in a figure, so we use 'auto' here
     # (shouldn't affect usability, but it makes testing more annoying)
     _set_backend('auto')
     with warnings.catch_warnings(record=True):  # traits for mlab.figure()
         mlab.figure(101)
@@ -113,129 +125,161 @@
     alphas = [1.0, 0.5, 0.25, 0.7, 0.5, 0.25, 0.7]
     for surf, hemi, title, cort, s, bg, fg, fig, sd, alpha \
             in zip(surfs, hemis, titles, cortices, sizes,
                    backgrounds, foregrounds, figs, subj_dirs, alphas):
         brain = Brain(subject_id, hemi, surf, title=title, cortex=cort,
                       alpha=alpha, size=s, background=bg, foreground=fg,
                       figure=fig, subjects_dir=sd)
-        brain.set_distance()
+        with np.errstate(invalid='ignore'):  # encountered in double_scalars
+            brain.set_distance()
         brain.close()
     brain = Brain(subject_id, hemi, surf, subjects_dir=sd,
                   interaction='terrain')
     brain.close()
-    assert_raises(ValueError, Brain, subject_id, 'lh', 'inflated',
+    pytest.raises(ValueError, Brain, subject_id, 'lh', 'inflated',
                   subjects_dir='')
-    assert_raises(ValueError, Brain, subject_id, 'lh', 'inflated',
+    pytest.raises(ValueError, Brain, subject_id, 'lh', 'inflated',
                   interaction='foo', subjects_dir=sd)
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_annot():
     """Test plotting of annot."""
     _set_backend()
     annots = ['aparc', 'aparc.a2005s']
     borders = [True, False, 2]
     alphas = [1, 0.5]
     brain = Brain(*std_args)
+    view = get_view(brain)
+
     for a, b, p in zip(annots, borders, alphas):
         brain.add_annotation(a, b, p)
+    check_view(brain, view)
+
     brain.set_surf('white')
-    assert_raises(ValueError, brain.add_annotation, 'aparc', borders=-1)
+    with pytest.raises(ValueError):
+        brain.add_annotation('aparc', borders=-1)
 
     subj_dir = utils._get_subjects_dir()
     annot_path = pjoin(subj_dir, subject_id, 'label', 'lh.aparc.a2009s.annot')
     labels, ctab, names = nib.freesurfer.read_annot(annot_path)
     brain.add_annotation((labels, ctab))
 
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_contour():
     """Test plotting of contour overlay."""
     _set_backend()
     brain = Brain(*std_args)
+    view = get_view(brain)
+
     overlay_file = pjoin(data_dir, "lh.sig.nii.gz")
     brain.add_contour_overlay(overlay_file)
     brain.add_contour_overlay(overlay_file, max=20, n_contours=9,
                               line_width=2)
     brain.contour['surface'].actor.property.line_width = 1
     brain.contour['surface'].contour.number_of_contours = 10
+
+    check_view(brain, view)
     brain.close()
 
 
-@requires_fsaverage
-@requires_fs
+@requires_fsaverage()
+@requires_fs()
 def test_data():
     """Test plotting of data."""
     _set_backend()
     brain = Brain(*std_args)
     mri_file = pjoin(data_dir, 'resting_corr.nii.gz')
     reg_file = pjoin(data_dir, 'register.dat')
     surf_data = io.project_volume_data(mri_file, "lh", reg_file)
     brain.add_data(surf_data, -.7, .7, colormap="jet", alpha=.7)
     brain.set_surf('white')
     brain.add_data([], vertices=np.array([], int))
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
+def test_data_limits():
+    """Test handling of data limits."""
+    _set_backend()
+    brain = Brain(*std_args)
+    surf_data = np.zeros(163842)
+    pytest.raises(ValueError, brain.add_data, surf_data, 0, 0)
+    brain.add_data(surf_data, 0, 1)
+    brain.close()
+
+
+@requires_fsaverage()
 def test_foci():
     """Test plotting of foci."""
     _set_backend('test')
     brain = Brain(*std_args)
     coords = [[-36, 18, -3],
               [-43, 25, 24],
               [-48, 26, -2]]
-    brain.add_foci(coords, map_surface="white", color="gold")
+    brain.add_foci(coords, map_surface="white", color="gold", name='test1')
 
     subj_dir = utils._get_subjects_dir()
     annot_path = pjoin(subj_dir, subject_id, 'label', 'lh.aparc.a2009s.annot')
     ids, ctab, names = nib.freesurfer.read_annot(annot_path)
     verts = np.arange(0, len(ids))
     coords = np.random.permutation(verts[ids == 74])[:10]
     scale_factor = 0.7
-    brain.add_foci(coords, coords_as_verts=True,
-                   scale_factor=scale_factor, color="#A52A2A")
+    brain.add_foci(coords, coords_as_verts=True, scale_factor=scale_factor,
+                   color="#A52A2A", name='test2')
+    with pytest.raises(ValueError):
+        brain.remove_foci(['test4'])
+    brain.remove_foci('test1')
+    brain.remove_foci()
+    assert len(brain.foci_dict) == 0
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_label():
     """Test plotting of label."""
     _set_backend()
     subject_id = "fsaverage"
     hemi = "lh"
     surf = "inflated"
     brain = Brain(subject_id, hemi, surf)
+    view = get_view(brain)
+
     brain.add_label("BA1")
+    check_view(brain, view)
     brain.add_label("BA1", color="blue", scalar_thresh=.5)
     subj_dir = utils._get_subjects_dir()
     label_file = pjoin(subj_dir, subject_id,
                        "label", "%s.MT.label" % hemi)
     brain.add_label(label_file)
     brain.add_label("BA44", borders=True)
     brain.add_label("BA6", alpha=.7)
     brain.show_view("medial")
     brain.add_label("V1", color="steelblue", alpha=.6)
     brain.add_label("V2", color="#FF6347", alpha=.6)
     brain.add_label("entorhinal", color=(.2, 1, .5), alpha=.6)
     brain.set_surf('white')
+    brain.show_view(dict(elevation=40, distance=430), distance=430)
+    with pytest.raises(ValueError, match='!='):
+        brain.show_view(dict(elevation=40, distance=430), distance=431)
 
     # remove labels
     brain.remove_labels('V1')
-    assert_in('V2', brain.labels_dict)
-    assert_not_in('V1', brain.labels_dict)
+    assert 'V2' in brain.labels_dict
+    assert 'V1' not in brain.labels_dict
     brain.remove_labels()
-    assert_not_in('V2', brain.labels_dict)
+    assert 'V2' not in brain.labels_dict
 
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_meg_inverse():
     """Test plotting of MEG inverse solution."""
     _set_backend()
     brain = Brain(*std_args)
     stc_fname = os.path.join(data_dir, 'meg_source_estimate-lh.stc')
     stc = io.read_stc(stc_fname)
     vertices = stc['vertices']
@@ -250,68 +294,68 @@
         return 'time=%0.2f ms' % (1e3 * t)
 
     for use_data in (data, data_full):
         brain.add_data(use_data, colormap=colormap, vertices=vertices,
                        smoothing_steps=1, time=time, time_label=time_label)
 
     brain.scale_data_colormap(fmin=13, fmid=18, fmax=22, transparent=True)
-    assert_equal(brain.data_dict['lh']['time_idx'], 0)
+    assert brain.data_dict['lh']['time_idx'] == 0
 
     brain.set_time(.1)
-    assert_equal(brain.data_dict['lh']['time_idx'], 2)
+    assert brain.data_dict['lh']['time_idx'] == 2
     # viewer = TimeViewer(brain)
 
     # multiple data layers
-    assert_raises(ValueError, brain.add_data, data, vertices=vertices,
+    pytest.raises(ValueError, brain.add_data, data, vertices=vertices,
                   time=time[:-1])
     brain.add_data(data, colormap=colormap, vertices=vertices,
                    smoothing_steps=1, time=time, time_label=time_label,
                    initial_time=.09)
-    assert_equal(brain.data_dict['lh']['time_idx'], 1)
+    assert brain.data_dict['lh']['time_idx'] == 1
     data_dicts = brain._data_dicts['lh']
-    assert_equal(len(data_dicts), 3)
-    assert_equal(data_dicts[0]['time_idx'], 1)
-    assert_equal(data_dicts[1]['time_idx'], 1)
+    assert len(data_dicts) == 3
+    assert data_dicts[0]['time_idx'] == 1
+    assert data_dicts[1]['time_idx'] == 1
 
     # shift time in both layers
     brain.set_data_time_index(0)
-    assert_equal(data_dicts[0]['time_idx'], 0)
-    assert_equal(data_dicts[1]['time_idx'], 0)
+    assert data_dicts[0]['time_idx'] == 0
+    assert data_dicts[1]['time_idx'] == 0
     brain.set_data_smoothing_steps(2)
 
     # add second data-layer without time axis
     brain.add_data(data[:, 1], colormap=colormap, vertices=vertices,
                    smoothing_steps=2)
     brain.set_data_time_index(2)
-    assert_equal(len(data_dicts), 4)
+    assert len(data_dicts) == 4
 
     # change surface
     brain.set_surf('white')
 
     # remove all layers
     brain.remove_data()
-    assert_equal(brain._data_dicts['lh'], [])
+    assert brain._data_dicts['lh'] == []
 
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_morphometry():
     """Test plotting of morphometry."""
     _set_backend()
     brain = Brain(*std_args)
     brain.add_morphometry("curv")
     brain.add_morphometry("sulc", grayscale=True)
     brain.add_morphometry("thickness")
     brain.close()
 
 
-@requires_imageio
-@requires_fsaverage
-def test_movie():
+@requires_imageio()
+@requires_fsaverage()
+def test_movie(tmpdir):
     """Test saving a movie of an MEG inverse solution."""
     import imageio
 
     # create and setup the Brain instance
     _set_backend()
     brain = Brain(*std_args)
     stc_fname = os.path.join(data_dir, 'meg_source_estimate-lh.stc')
@@ -319,36 +363,29 @@
     data = stc['data']
     time = np.arange(data.shape[1]) * stc['tstep'] + stc['tmin']
     brain.add_data(data, colormap='hot', vertices=stc['vertices'],
                    smoothing_steps=10, time=time, time_label='time=%0.2f ms')
     brain.scale_data_colormap(fmin=13, fmid=18, fmax=22, transparent=True)
 
     # save movies with different options
-    tempdir = mkdtemp()
-    try:
-        dst = os.path.join(tempdir, 'test.mov')
-        # test the number of frames in the movie
-        brain.save_movie(dst)
-        frames = imageio.mimread(dst)
-        assert_equal(len(frames), 2)
-        brain.save_movie(dst, time_dilation=10)
-        frames = imageio.mimread(dst)
-        assert_equal(len(frames), 7)
-        brain.save_movie(dst, tmin=0.081, tmax=0.102)
-        frames = imageio.mimread(dst)
-        assert_equal(len(frames), 2)
-    finally:
-        # clean up
-        if not (sys.platform == 'win32' and
-                os.getenv('APPVEYOR', 'False') == 'True'):  # cleanup problems
-            shutil.rmtree(tempdir)
+    dst = str(tmpdir.join('test.mov'))
+    # test the number of frames in the movie
+    brain.save_movie(dst)
+    frames = imageio.mimread(dst)
+    assert len(frames) == 2
+    brain.save_movie(dst, time_dilation=10)
+    frames = imageio.mimread(dst)
+    assert len(frames) == 7
+    brain.save_movie(dst, tmin=0.081, tmax=0.102)
+    frames = imageio.mimread(dst)
+    assert len(frames) == 2
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_overlay():
     """Test plotting of overlay."""
     _set_backend()
     # basic overlay support
     overlay_file = pjoin(data_dir, "lh.sig.nii.gz")
     brain = Brain(*std_args)
     brain.add_overlay(overlay_file)
@@ -358,16 +395,16 @@
     sig2 = io.read_scalar_data(pjoin(data_dir, "lh.alt_sig.nii.gz"))
 
     # two-sided overlay
     brain.add_overlay(sig1, 4, 30, name="two-sided")
     overlay = brain.overlays_dict.pop('two-sided')[0]
     assert_array_equal(overlay.pos_bar.data_range, [4, 30])
     assert_array_equal(overlay.neg_bar.data_range, [-30, -4])
-    assert_equal(overlay.pos_bar.reverse_lut, True)
-    assert_equal(overlay.neg_bar.reverse_lut, False)
+    assert overlay.pos_bar.reverse_lut
+    assert not overlay.neg_bar.reverse_lut
     overlay.remove()
 
     thresh = 4
     sig1[sig1 < thresh] = 0
     sig2[sig2 < thresh] = 0
 
     conjunct = np.min(np.vstack((sig1, sig2)), axis=0)
@@ -384,15 +421,15 @@
     brain.overlays["conjunct"].pos_bar.visible = False
 
     brain.set_surf('white')
 
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_probabilistic_labels():
     """Test plotting of probabilistic labels."""
     _set_backend()
     brain = Brain("fsaverage", "lh", "inflated",
                   cortex="low_contrast")
 
     brain.add_label("BA1", color="darkblue")
@@ -411,38 +448,38 @@
 
     with warnings.catch_warnings(record=True):
         brain.data["colorbar"].number_of_colors = 10
         brain.data["colorbar"].number_of_labels = 11
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_text():
     """Test plotting of text."""
     _set_backend('test')
     brain = Brain(*std_args)
     brain.add_text(0.1, 0.1, 'Hello', 'blah')
     brain.close()
 
 
-@requires_fsaverage
-def test_animate():
+@requires_fsaverage()
+def test_animate(tmpdir):
     """Test animation."""
     _set_backend('auto')
     brain = Brain(*std_args, size=100)
     brain.add_morphometry('curv')
-    tmp_name = mktemp() + '.avi'
+    tmp_name = str(tmpdir.join('test.avi'))
     brain.animate(["m"] * 3, n_steps=2)
     brain.animate(['l', 'l'], n_steps=2, fname=tmp_name)
     # can't rotate in axial plane
-    assert_raises(ValueError, brain.animate, ['l', 'd'])
+    pytest.raises(ValueError, brain.animate, ['l', 'd'])
     brain.close()
 
 
-@requires_fsaverage
+@requires_fsaverage()
 def test_views():
     """Test showing different views."""
     _set_backend('test')
     brain = Brain(*std_args)
     brain.show_view('lateral')
     brain.show_view('m')
     brain.show_view('rostral')
```

### Comparing `pysurfer-0.8.0/surfer/viz.py` & `pysurfer-0.9.0/surfer/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from copy import deepcopy
+import logging
 from math import floor
 import os
 from os.path import join as pjoin
 import warnings
 from warnings import warn
 
 import numpy as np
@@ -13,21 +15,22 @@
 from mayavi.core import lut_manager
 from mayavi.core.scene import Scene
 from mayavi.core.ui.api import SceneEditor
 from mayavi.core.ui.mayavi_scene import MayaviScene
 from traits.api import (HasTraits, Range, Int, Float,
                         Bool, Enum, on_trait_change, Instance)
 from tvtk.api import tvtk
+from pyface.api import GUI
+from traitsui.api import View, Item, Group, VGroup, HGroup, VSplit, HSplit
 
 from . import utils, io
 from .utils import (Surface, verbose, create_color_lut, _get_subjects_dir,
-                    string_types, threshold_filter)
+                    string_types, threshold_filter, _check_units)
 
 
-import logging
 logger = logging.getLogger('surfer')
 
 
 lh_viewdict = {'lateral': {'v': (180., 90.), 'r': 90.},
                'medial': {'v': (0., 90.), 'r': -90.},
                'rostral': {'v': (90., 90.), 'r': -180.},
                'caudal': {'v': (270., 90.), 'r': 0.},
@@ -166,51 +169,53 @@
     data = data.copy()
     data = data.astype(np.float64)
     if data.dtype.byteorder == '>':
         data.byteswap(True)
     return data
 
 
-def _force_render(figures, backend):
+def _force_render(figures):
     """Ensure plots are updated before properties are used"""
     if not isinstance(figures, list):
         figures = [[figures]]
+    _gui = GUI()
+    orig_val = _gui.busy
+    _gui.set_busy(busy=True)
+    _gui.process_events()
     for ff in figures:
         for f in ff:
             f.render()
             mlab.draw(figure=f)
-    if backend == 'TraitsUI':
-        from pyface.api import GUI
-        _gui = GUI()
-        orig_val = _gui.busy
-        _gui.set_busy(busy=True)
-        _gui.process_events()
-        _gui.set_busy(busy=orig_val)
-        _gui.process_events()
+    _gui.set_busy(busy=orig_val)
+    _gui.process_events()
 
 
 def _make_viewer(figure, n_row, n_col, title, scene_size, offscreen,
                  interaction='trackball'):
     """Triage viewer creation
 
     If n_row == n_col == 1, then we can use a Mayavi figure, which
     generally guarantees that things will be drawn before control
     is returned to the command line. With the multi-view, TraitsUI
     unfortunately has no such support, so we only use it if needed.
     """
     if figure is None:
         # spawn scenes
         h, w = scene_size
-        if offscreen is True:
+        if offscreen == 'auto':
+            offscreen = mlab.options.offscreen
+        if offscreen:
             orig_val = mlab.options.offscreen
-            mlab.options.offscreen = True
-            with warnings.catch_warnings(record=True):  # traits
-                figures = [[mlab.figure(size=(h / n_row, w / n_col))
-                            for _ in range(n_col)] for __ in range(n_row)]
-            mlab.options.offscreen = orig_val
+            try:
+                mlab.options.offscreen = True
+                with warnings.catch_warnings(record=True):  # traits
+                    figures = [[mlab.figure(size=(h / n_row, w / n_col))
+                                for _ in range(n_col)] for __ in range(n_row)]
+            finally:
+                mlab.options.offscreen = orig_val
             _v = None
         else:
             # Triage: don't make TraitsUI if we don't have to
             if n_row == 1 and n_col == 1:
                 with warnings.catch_warnings(record=True):  # traits
                     figure = mlab.figure(title, size=(w, h))
                 mlab.clf(figure)
@@ -241,15 +246,14 @@
         figures = [figure[slice(ri * n_col, (ri + 1) * n_col)]
                    for ri in range(n_row)]
     return figures, _v
 
 
 class _MlabGenerator(HasTraits):
     """TraitsUI mlab figure generator"""
-    from traitsui.api import View
     view = Instance(View)
 
     def __init__(self, n_row, n_col, width, height, title, **traits):
         HasTraits.__init__(self, **traits)
         self.mlab_names = []
         self.n_row = n_row
         self.n_col = n_col
@@ -272,15 +276,14 @@
                 x = getattr(self, self.mlab_names[ind])
                 rfigs.append(x.mayavi_scene)
                 ind += 1
             figures.append(rfigs)
         return figures, self._v
 
     def _get_gen_view(self):
-        from traitsui.api import (View, Item, VGroup, HGroup)
         ind = 0
         va = []
         for ri in range(self.n_row):
             ha = []
             for ci in range(self.n_col):
                 ha += [Item(name=self.mlab_names[ind], style='custom',
                             resizable=True, show_label=False,
@@ -331,16 +334,20 @@
             6. A dict of keyword arguments that is passed on to the
                call to surface.
     alpha : float in [0, 1]
         Alpha level to control opacity of the cortical surface.
     size : float or pair of floats
         the size of the window, in pixels. can be one number to specify
         a square window, or the (width, height) of a rectangular window.
-    background, foreground : matplotlib colors
-        color of the background and foreground of the display window
+    background : matplotlib color
+        Color of the background.
+    foreground : matplotlib color
+        Color of the foreground (will be used for colorbars and text).
+        None (default) will use black or white depending on the value
+        of ``background``.
     figure : list of mayavi.core.scene.Scene | None | int
         If None (default), a new window will be created with the appropriate
         views. For single view plots, the figure can be specified as int to
         retrieve the corresponding Mayavi window.
     subjects_dir : str | None
         If not None, this directory will be used as the subjects directory
         instead of the value set using the SUBJECTS_DIR environment
@@ -348,21 +355,24 @@
     views : list | str
         views to use
     offset : bool
         If True, aligs origin with medial wall. Useful for viewing inflated
         surface where hemispheres typically overlap (Default: True)
     show_toolbar : bool
         If True, toolbars will be shown for each view.
-    offscreen : bool
+    offscreen : bool | str
         If True, rendering will be done offscreen (not shown). Useful
         mostly for generating images or screenshots, but can be buggy.
-        Use at your own risk.
+        Use at your own risk. Can be "auto" (default) to use
+        ``mlab.options.offscreen``.
     interaction : str
         Can be "trackball" (default) or "terrain", i.e. a turntable-style
         camera.
+    units : str
+        Can be 'm' or 'mm' (default).
 
     Attributes
     ----------
     annot : list
         List of annotations.
     brains : list
         List of the underlying brain instances.
@@ -375,51 +385,23 @@
     overlays : dict
         The overlays.
     texts : dict
         The text objects.
     """
     def __init__(self, subject_id, hemi, surf, title=None,
                  cortex="classic", alpha=1.0, size=800, background="black",
-                 foreground="white", figure=None, subjects_dir=None,
+                 foreground=None, figure=None, subjects_dir=None,
                  views=['lat'], offset=True, show_toolbar=False,
-                 offscreen=False, interaction='trackball',
-                 config_opts=None, curv=None):
-
-        # Keep backwards compatability
-        if config_opts is not None:
-            msg = ("The `config_opts` dict has been deprecated and will "
-                   "be removed in future versions. You should update your "
-                   "code and pass these options directly to the `Brain` "
-                   "constructor.")
-            warn(msg, DeprecationWarning)
-            cortex = config_opts.get("cortex", cortex)
-            background = config_opts.get("background", background)
-            foreground = config_opts.get("foreground", foreground)
-
-            size = config_opts.get("size", size)
-            width = config_opts.get("width", size)
-            height = config_opts.get("height", size)
-            size = (width, height)
-        # Keep backwards compatability
-        if curv is not None:
-            msg = ("The `curv` keyword has been deprecated and will "
-                   "be removed in future versions. You should update your "
-                   "code and use the `cortex` keyword to specify how the "
-                   "brain surface is rendered. Setting `cortex` to `None` "
-                   "will reproduce the previous behavior when `curv` was "
-                   "set to `False`. To emulate the previous behavior for "
-                   "cases where `curv` was set to `True`, simply omit it.")
-            warn(msg, DeprecationWarning)
-            if not curv:
-                cortex = None
+                 offscreen='auto', interaction='trackball', units='mm'):
 
         if not isinstance(interaction, string_types) or \
                 interaction not in ('trackball', 'terrain'):
             raise ValueError('interaction must be "trackball" or "terrain", '
                              'got "%s"' % (interaction,))
+        self._units = _check_units(units)
         col_dict = dict(lh=1, rh=1, both=1, split=2)
         n_col = col_dict[hemi]
         if hemi not in col_dict.keys():
             raise ValueError('hemi must be one of [%s], not %s'
                              % (', '.join(col_dict.keys()), hemi))
         # Get the subjects directory from parameter or env. var
         subjects_dir = _get_subjects_dir(subjects_dir=subjects_dir)
@@ -443,45 +425,47 @@
         elif hemi == 'rh':
             geo_hemis = ['rh']
         else:
             raise ValueError('bad hemi value')
         geo_kwargs, geo_reverse, geo_curv = self._get_geo_params(cortex, alpha)
         for h in geo_hemis:
             # Initialize a Surface object as the geometry
-            geo = Surface(subject_id, h, surf, subjects_dir, offset)
+            geo = Surface(subject_id, h, surf, subjects_dir, offset,
+                          units=self._units)
             # Load in the geometry and (maybe) curvature
             geo.load_geometry()
             if geo_curv:
                 geo.load_curvature()
             self.geo[h] = geo
 
         # deal with making figures
         self._set_window_properties(size, background, foreground)
+        del background, foreground
         figures, _v = _make_viewer(figure, n_row, n_col, title,
                                    self._scene_size, offscreen,
                                    interaction)
         self._figures = figures
         self._v = _v
         self._window_backend = 'Mayavi' if self._v is None else 'TraitsUI'
         for ff in self._figures:
             for f in ff:
                 if f.scene is not None:
                     f.scene.background = self._bg_color
                     f.scene.foreground = self._fg_color
 
         # force rendering so scene.lights exists
-        _force_render(self._figures, self._window_backend)
+        _force_render(self._figures)
         self.toggle_toolbars(show_toolbar)
-        _force_render(self._figures, self._window_backend)
+        _force_render(self._figures)
         self._toggle_render(False)
 
         # fill figures with brains
         kwargs = dict(geo_curv=geo_curv, geo_kwargs=geo_kwargs,
                       geo_reverse=geo_reverse, subjects_dir=subjects_dir,
-                      bg_color=self._bg_color)
+                      bg_color=self._bg_color, fg_color=self._fg_color)
         brains = []
         brain_matrix = []
         for ri, view in enumerate(views):
             brain_row = []
             for hi, h in enumerate(['lh', 'rh']):
                 if not (hemi in ['lh', 'rh'] and h != hemi):
                     ci = hi if hemi == 'split' else 0
@@ -539,44 +523,44 @@
             views = [None] * len(figs)
         for vi, (_f, view) in enumerate(zip(figs, views)):
             # Testing backend doesn't have these options
             if mlab.options.backend == 'test':
                 continue
 
             if state is False and view is None:
-                views[vi] = (mlab.view(figure=_f),
-                             _f.scene.camera.parallel_scale)
+                views[vi] = (mlab.view(figure=_f), mlab.roll(figure=_f),
+                             _f.scene.camera.parallel_scale
+                             if _f.scene is not None else False)
 
-            _f.scene.disable_render = not state
+            if _f.scene is not None:
+                _f.scene.disable_render = not state
 
-            if state is True and view is not None:
+            if state is True and view is not None and _f.scene is not None:
                 mlab.draw(figure=_f)
                 with warnings.catch_warnings(record=True):  # traits focalpoint
                     mlab.view(*view[0], figure=_f)
-                _f.scene.camera.parallel_scale = view[1]
+                    mlab.roll(view[1], figure=_f)
         # let's do the ugly force draw
         if state is True:
-            _force_render(self._figures, self._window_backend)
+            _force_render(self._figures)
         return views
 
     def _set_window_properties(self, size, background, foreground):
         """Set window properties that are used elsewhere."""
         # old option "size" sets both width and height
         from matplotlib.colors import colorConverter
         try:
             width, height = size
         except (TypeError, ValueError):
             width, height = size, size
         self._scene_size = height, width
-
-        bg_color_rgb = colorConverter.to_rgb(background)
-        self._bg_color = bg_color_rgb
-
-        fg_color_rgb = colorConverter.to_rgb(foreground)
-        self._fg_color = fg_color_rgb
+        self._bg_color = colorConverter.to_rgb(background)
+        if foreground is None:
+            foreground = 'w' if sum(self._bg_color) < 2 else 'k'
+        self._fg_color = colorConverter.to_rgb(foreground)
 
     def _get_geo_params(self, cortex, alpha=1.0):
         """Return keyword arguments and other parameters for surface
         rendering.
 
         Parameters
         ----------
@@ -685,15 +669,15 @@
             props["transparent"] : lower part of colormap transparent?
             props["time"] : time points
             props["time_idx"] : current time index
             props["smoothing_steps"] : number of smoothing steps
         """
         props = dict()
         keys = ['fmin', 'fmid', 'fmax', 'transparent', 'time', 'time_idx',
-                'smoothing_steps']
+                'smoothing_steps', 'center']
         try:
             if self.data_dict['lh'] is not None:
                 hemi = 'lh'
             else:
                 hemi = 'rh'
             for key in keys:
                 props[key] = self.data_dict[hemi][key]
@@ -958,20 +942,20 @@
         if name in self.overlays_dict:
             name = "%s%d" % (name, len(self.overlays_dict) + 1)
         self.overlays_dict[name] = ol
         self._toggle_render(True, views)
 
     @verbose
     def add_data(self, array, min=None, max=None, thresh=None,
-                 colormap="RdBu_r", alpha=1,
+                 colormap="auto", alpha=1,
                  vertices=None, smoothing_steps=20, time=None,
                  time_label="time index=%d", colorbar=True,
                  hemi=None, remove_existing=False, time_label_size=14,
                  initial_time=None, scale_factor=None, vector_alpha=None,
-                 verbose=None):
+                 mid=None, center=None, transparent=False, verbose=None):
         """Display data from a numpy array on the surface.
 
         This provides a similar interface to
         :meth:`surfer.Brain.add_overlay`, but it displays
         it with a single colormap. It offers more flexibility over the
         colormap, and provides a way to display four-dimensional data
         (i.e., a timecourse) or five-dimensional data (i.e., a
@@ -988,22 +972,33 @@
             (3 values per vertex corresponding to X/Y/Z surface RAS),
             then ``array`` must be have all 3 dimensions.
             If vectors with no time dimension are desired, consider using a
             singleton (e.g., ``np.newaxis``) to create a "time" dimension
             and pass ``time_label=None``.
         min : float
             min value in colormap (uses real min if None)
+        mid : float
+            intermediate value in colormap (middle between min and max if None)
         max : float
             max value in colormap (uses real max if None)
         thresh : None or float
             if not None, values below thresh will not be visible
+        center : float or None
+            if not None, center of a divergent colormap, changes the meaning of
+            min, max and mid, see :meth:`scale_data_colormap` for further info.
+        transparent : bool
+            if True: use a linear transparency between fmin and fmid and make
+            values below fmin fully transparent (symmetrically for divergent
+            colormaps)
         colormap : string, list of colors, or array
             name of matplotlib colormap to use, a list of matplotlib colors,
             or a custom look up table (an n x 4 array coded with RBGA values
-            between 0 and 255).
+            between 0 and 255), the default "auto" chooses a default divergent
+            colormap, if "center" is given (currently "icefire"), otherwise a
+            default sequential colormap (currently "rocket").
         alpha : float in [0, 1]
             alpha level to control opacity of the overlay.
         vertices : numpy array
             vertices for which the data is defined (needed if len(data) < nvtx)
         smoothing_steps : int or None
             number of smoothing steps (smoothing is used if len(data) < nvtx)
             Default : 20
@@ -1046,24 +1041,34 @@
 
         Due to a Mayavi (or VTK) alpha rendering bug, ``vector_alpha`` is
         clamped to be strictly < 1.
         """
         hemi = self._check_hemi(hemi)
         array = np.asarray(array)
 
-        if min is None:
-            min = array.min() if array.size > 0 else 0
-        if max is None:
-            max = array.max() if array.size > 0 else 0
-        mid = (min + max) / 2.
+        if center is None:
+            if min is None:
+                min = array.min() if array.size > 0 else 0
+            if max is None:
+                max = array.max() if array.size > 0 else 1
+        else:
+            if min is None:
+                min = 0
+            if max is None:
+                max = np.abs(center - array).max() if array.size > 0 else 1
+        if mid is None:
+            mid = (min + max) / 2.
+        _check_limits(min, mid, max, extra='')
 
         # Create smoothing matrix if necessary
         if len(array) < self.geo[hemi].x.shape[0]:
             if vertices is None:
-                raise ValueError("len(data) < nvtx: need vertices")
+                raise ValueError("len(data) < nvtx (%s < %s): the vertices "
+                                 "parameter must not be None"
+                                 % (len(array), self.geo[hemi].x.shape[0]))
             adj_mat = utils.mesh_edges(self.geo[hemi].faces)
             smooth_mat = utils.smoothing_matrix(vertices, adj_mat,
                                                 smoothing_steps)
         else:
             smooth_mat = None
 
         magnitude = None
@@ -1077,32 +1082,35 @@
                 distance = np.sum([array[:, dim, :].ptp(axis=0).max() ** 2
                                    for dim in range(3)])
                 if distance == 0:
                     scale_factor = 1
                 else:
                     scale_factor = (0.4 * distance /
                                     (4 * array.shape[0] ** (0.33)))
+            if self._units == 'm':
+                scale_factor = scale_factor / 1000.
             magnitude_max = magnitude.max()
         elif array.ndim not in (1, 2):
             raise ValueError('array has must have 1, 2, or 3 dimensions, '
                              'got (%s)' % (array.ndim,))
 
         # Process colormap argument into a lut
-        lut = create_color_lut(colormap)
+        lut = create_color_lut(colormap, center=center)
         colormap = "Greys"
 
         # determine unique data layer ID
         data_dicts = self._data_dicts['lh'] + self._data_dicts['rh']
         if data_dicts:
             layer_id = np.max([data['layer_id'] for data in data_dicts]) + 1
         else:
             layer_id = 0
 
         data = dict(array=array, smoothing_steps=smoothing_steps,
-                    fmin=min, fmid=mid, fmax=max, scale_factor=scale_factor,
+                    fmin=min, fmid=mid, fmax=max, center=center,
+                    scale_factor=scale_factor,
                     transparent=False, time=0, time_idx=0,
                     vertices=vertices, smooth_mat=smooth_mat,
                     layer_id=layer_id, magnitude=magnitude)
 
         # clean up existing data
         if remove_existing:
             self.remove_data(hemi)
@@ -1170,14 +1178,16 @@
         data['surfaces'] = surfs
         data['colorbars'] = bars
         data['orig_ctable'] = ct
         data['glyphs'] = glyphs
 
         self._data_dicts[hemi].append(data)
 
+        self.scale_data_colormap(min, mid, max, transparent, center, alpha)
+
         if initial_time_index is not None:
             self.set_data_time_index(initial_time_index)
         self._toggle_render(True, views)
 
     def add_annotation(self, annot, borders=True, alpha=1, hemi=None,
                        remove_existing=True):
         """Add an annotation file.
@@ -1253,24 +1263,26 @@
 
         for hemi, (labels, cmap) in zip(hemis, annots):
 
             # Maybe zero-out the non-border vertices
             self._to_borders(labels, hemi, borders)
 
             # Handle null labels properly
-            # (tksurfer doesn't use the alpha channel, so sometimes this
-            # is set weirdly. For our purposes, it should always be 0.
-            # Unless this sometimes causes problems?
-            cmap[np.where(cmap[:, 4] == 0), 3] = 0
-            if np.any(labels == 0) and not np.any(cmap[:, -1] == 0):
-                cmap = np.vstack((cmap, np.zeros(5, int)))
+            cmap[:, 3] = 255
+            bgcolor = self._brain_color
+            bgcolor[-1] = 0
+            cmap[cmap[:, 4] < 0, 4] += 2 ** 24  # wrap to positive
+            cmap[cmap[:, 4] <= 0, :4] = bgcolor
+            if np.any(labels == 0) and not np.any(cmap[:, -1] <= 0):
+                cmap = np.vstack((cmap, np.concatenate([bgcolor, [0]])))
 
             # Set label ids sensibly
-            ord = np.argsort(cmap[:, -1])
-            ids = ord[np.searchsorted(cmap[ord, -1], labels)]
+            order = np.argsort(cmap[:, -1])
+            cmap = cmap[order]
+            ids = np.searchsorted(cmap[:, -1], labels)
             cmap = cmap[:, :4]
 
             #  Set the alpha level
             alpha_vec = cmap[:, 3]
             alpha_vec[alpha_vec > 0] = alpha * 255
 
             for brain in self._brain_list:
@@ -1438,14 +1450,42 @@
                         brain.remove_data(data['layer_id'])
             self._data_dicts[hemi] = []
 
         # if no data is left, reset time properties
         if all(len(brain.data) == 0 for brain in self.brains):
             self.n_times = self._times = None
 
+    def remove_foci(self, name=None):
+        """Remove foci added with ``Brain.add_foci()``.
+
+        Parameters
+        ----------
+        name : str | list of str | None
+            Names of the foci to remove (if None, remove all).
+
+        Notes
+        -----
+        Only foci added with a unique names can be removed.
+        """
+        if name is None:
+            keys = tuple(self.foci_dict)
+        else:
+            if isinstance(name, str):
+                keys = (name,)
+            else:
+                keys = name
+            if not all(key in self.foci_dict for key in keys):
+                missing = ', '.join(key for key in keys if key not in
+                                    self.foci_dict)
+                raise ValueError("foci=%r: no foci named %s" % (name, missing))
+
+        for key in keys:
+            for points in self.foci_dict.pop(key):
+                points.remove()
+
     def remove_labels(self, labels=None, hemi=None):
         """Remove one or more previously added labels from the image.
 
         Parameters
         ----------
         labels : None | str | list of str
             Labels to remove. Can be a string naming a single label, or None to
@@ -1455,15 +1495,16 @@
             Deprecated parameter, do not use.
         """
         if hemi is not None:
             warn("The `hemi` parameter to Brain.remove_labels() has no effect "
                  "and will be removed in PySurfer 0.9", DeprecationWarning)
 
         if labels is None:
-            labels_ = self._label_dicts.keys()
+            # make list before iterating (Py3k)
+            labels_ = list(self._label_dicts.keys())
         else:
             labels_ = [labels] if isinstance(labels, str) else labels
             missing = [key for key in labels_ if key not in self._label_dicts]
             if missing:
                 raise ValueError("labels=%r contains unknown labels: %s" %
                                  (labels, ', '.join(map(repr, missing))))
 
@@ -1570,21 +1611,22 @@
         from a volume-based analysis in MNI space can be displayed on an
         inflated average surface by finding the closest vertex on the
         white surface and mapping to that vertex on the inflated mesh.
 
         Parameters
         ----------
         coords : numpy array
-            x, y, z coordinates in stereotaxic space or array of vertex ids
+            x, y, z coordinates in stereotaxic space (default) or array of
+            vertex ids (with ``coord_as_verts=True``)
         coords_as_verts : bool
             whether the coords parameter should be interpreted as vertex ids
         map_surface : Freesurfer surf or None
             surface to map coordinates through, or None to use raw coords
-        scale_factor : int
-            controls the size of the foci spheres
+        scale_factor : float
+            Controls the size of the foci spheres (relative to 1cm).
         color : matplotlib color code
             HTML name, RBG tuple, or hex code
         alpha : float in [0, 1]
             opacity of focus gylphs
         name : str
             internal name to use
         hemi : str | None
@@ -1601,29 +1643,32 @@
             map_surface = None
 
         # Possibly map the foci coords through a surface
         if map_surface is None:
             foci_coords = np.atleast_2d(coords)
         else:
             foci_surf = Surface(self.subject_id, hemi, map_surface,
-                                subjects_dir=self.subjects_dir)
+                                subjects_dir=self.subjects_dir,
+                                units=self._units)
             foci_surf.load_geometry()
             foci_vtxs = utils.find_closest_vertices(foci_surf.coords, coords)
             foci_coords = self.geo[hemi].coords[foci_vtxs]
 
         # Get a unique name (maybe should take this approach elsewhere)
         if name is None:
             name = "foci_%d" % (len(self.foci_dict) + 1)
 
         # Convert the color code
         if not isinstance(color, tuple):
             color = colorConverter.to_rgb(color)
 
         views = self._toggle_render(False)
         fl = []
+        if self._units == 'm':
+            scale_factor = scale_factor / 1000.
         for brain in self._brain_list:
             if brain['hemi'] == hemi:
                 fl.append(brain['brain'].add_foci(foci_coords, scale_factor,
                                                   color, alpha, name))
         self.foci_dict[name] = fl
         self._toggle_render(True, views)
 
@@ -1700,15 +1745,17 @@
         y : Float
             y coordinate
         text : str
             Text to add
         name : str
             Name of the text (text label can be updated using update_text())
         color : Tuple
-            Color of the text. Default: (1, 1, 1)
+            Color of the text. Default is the foreground color set during
+            initialization (default is black or white depending on the
+            background color).
         opacity : Float
             Opacity of the text. Default: 1.0
         row : int
             Row index of which brain to use
         col : int
             Column index of which brain to use
         """
@@ -1750,27 +1797,29 @@
 
         Parameters
         ----------
         view : str | dict
             brain surface to view (one of 'lateral', 'medial', 'rostral',
             'caudal', 'dorsal', 'ventral', 'frontal', 'parietal') or kwargs to
             pass to :func:`mayavi.mlab.view()`.
-
-        Returns
-        -------
-        view : tuple
-            tuple returned from mlab.view
         roll : float
             camera roll
         distance : float | 'auto' | None
             distance from the origin
         row : int
             Row index of which brain to use
         col : int
             Column index of which brain to use
+
+        Returns
+        -------
+        view : tuple
+            tuple returned from mlab.view
+        roll : float
+            camera roll returned from mlab.roll
         """
         return self.brain_matrix[row][col].show_view(view, roll, distance)
 
     def set_distance(self, distance=None):
         """Set view distances for all brain plots to the same value
 
         Parameters
@@ -1823,68 +1872,139 @@
             except IOError:  # surface file does not exist
                 geo.surf = self.surf
                 self._toggle_render(True)
                 raise
 
         # update mesh objects (they use a reference to geo.coords)
         for brain in self.brains:
+            brain._geo_mesh.data.points = self.geo[brain.hemi].coords
             brain.update_surf()
 
         self.surf = surf
         self._toggle_render(True, views)
 
         for brain in self.brains:
             if brain._f.scene is not None:
                 brain._f.scene.reset_zoom()
 
+    @property
+    def _brain_color(self):
+        geo_actor = self._brain_list[0]['brain']._geo_surf.actor
+        if self._brain_list[0]['brain']._using_lut:
+            bgcolor = np.mean(
+                self._brain_list[0]['brain']._geo_surf.module_manager
+                .scalar_lut_manager.lut.table.to_array(), axis=0)
+        else:
+            bgcolor = geo_actor.property.color
+            if len(bgcolor) == 3:
+                bgcolor = bgcolor + (1,)
+            bgcolor = 255 * np.array(bgcolor)
+        bgcolor[-1] *= geo_actor.property.opacity
+        return bgcolor
+
     @verbose
-    def scale_data_colormap(self, fmin, fmid, fmax, transparent, verbose=None):
+    def scale_data_colormap(self, fmin, fmid, fmax, transparent,
+                            center=None, alpha=1.0, verbose=None):
         """Scale the data colormap.
 
+        The colormap may be sequential or divergent. When the colormap is
+        divergent indicate this by providing a value for 'center'. The
+        meanings of fmin, fmid and fmax are different for sequential and
+        divergent colormaps. For sequential colormaps the colormap is
+        characterised by::
+
+            [fmin, fmid, fmax]
+
+        where fmin and fmax define the edges of the colormap and fmid will be
+        the value mapped to the center of the originally chosen colormap. For
+        divergent colormaps the colormap is characterised by::
+
+            [center-fmax, center-fmid, center-fmin, center,
+             center+fmin, center+fmid, center+fmax]
+
+        i.e., values between center-fmin and center+fmin will not be shown
+        while center-fmid will map to the middle of the first half of the
+        original colormap and center-fmid to the middle of the second half.
+
         Parameters
         ----------
         fmin : float
-            minimum value of colormap
+            minimum value for colormap
         fmid : float
             value corresponding to color midpoint
         fmax : float
             maximum value for colormap
         transparent : boolean
-            if True: use a linear transparency between fmin and fmid
+            if True: use a linear transparency between fmin and fmid and make
+            values below fmin fully transparent (symmetrically for divergent
+            colormaps)
+        center : float
+            if not None, gives the data value that should be mapped to the
+            center of the (divergent) colormap
+        alpha : float
+            sets the overall opacity of colors, maintains transparent regions
         verbose : bool, str, int, or None
             If not None, override default verbose level (see surfer.verbose).
         """
+        divergent = center is not None
+
         # Get the original colormap
         for h in ['lh', 'rh']:
             data = self.data_dict[h]
             if data is not None:
                 table = data["orig_ctable"].copy()
                 break
 
-        lut = _scale_mayavi_lut(table, fmin, fmid, fmax, transparent)
+        lut = _scale_mayavi_lut(table, fmin, fmid, fmax, transparent,
+                                center, alpha)
+
+        # Get the effective background color as 255-based 4-element array
+        bgcolor = self._brain_color
 
         views = self._toggle_render(False)
         # Use the new colormap
         for hemi in ['lh', 'rh']:
             data = self.data_dict[hemi]
             if data is not None:
                 for surf in data['surfaces']:
                     cmap = surf.module_manager.scalar_lut_manager
                     cmap.load_lut_from_list(lut / 255.)
-                    cmap.data_range = np.array([fmin, fmax])
+                    if divergent:
+                        cmap.data_range = np.array([center-fmax, center+fmax])
+                    else:
+                        cmap.data_range = np.array([fmin, fmax])
+
+                    # if there is any transparent color in the lut
+                    if np.any(lut[:, -1] < 255):
+                        # Update the colorbar to deal with transparency
+                        cbar_lut = tvtk.LookupTable()
+                        cbar_lut.deep_copy(surf.module_manager
+                                           .scalar_lut_manager.lut)
+                        alphas = lut[:, -1][:, np.newaxis] / 255.
+                        use_lut = lut.copy()
+                        use_lut[:, -1] = 255.
+                        vals = (use_lut * alphas) + bgcolor * (1 - alphas)
+                        cbar_lut.table.from_array(vals)
+                        cmap.scalar_bar.lookup_table = cbar_lut
+                        cmap.scalar_bar.use_opacity = 1
 
                 # Update the data properties
-                data.update(fmin=fmin, fmid=fmid, fmax=fmax,
+                data.update(fmin=fmin, fmid=fmid, fmax=fmax, center=center,
                             transparent=transparent)
                 # And the hemisphere properties to match
                 for glyph in data['glyphs']:
                     if glyph is not None:
                         l_m = glyph.parent.vector_lut_manager
                         l_m.load_lut_from_list(lut / 255.)
-                        l_m.data_range = np.array([fmin, fmax])
+                        if divergent:
+                            l_m.data_range = np.array(
+                                    [center-fmax, center+fmax])
+                        else:
+                            l_m.data_range = np.array([fmin, fmax])
+
         self._toggle_render(True, views)
 
     def set_data_time_index(self, time_idx, interpolation='quadratic'):
         """Set the data time index to show
 
         Parameters
         ----------
@@ -2114,14 +2234,15 @@
     def close(self):
         """Close all figures and cleanup data structure."""
         for ri, ff in enumerate(self._figures):
             for ci, f in enumerate(ff):
                 if f is not None:
                     mlab.close(f)
                     self._figures[ri][ci] = None
+        _force_render([])
 
         # should we tear down other variables?
         if self._v is not None:
             self._v.dispose()
             self._v = None
 
     def __del__(self):
@@ -2160,14 +2281,24 @@
         if ftype not in good_ftypes:
             raise ValueError("Supported image types are %s"
                              % " ".join(good_ftypes))
         mlab.draw(brain._f)
         if mlab.options.backend != 'test':
             mlab.savefig(filename, figure=brain._f)
 
+    def _screenshot_figure(self, mode='rgb', antialiased=False):
+        """Create a matplolib figure from the current screenshot."""
+        # adapted from matplotlib.image.imsave
+        from matplotlib.backends.backend_agg import FigureCanvasAgg
+        from matplotlib.figure import Figure
+        fig = Figure(frameon=False)
+        FigureCanvasAgg(fig)
+        fig.figimage(self.screenshot(mode, antialiased), resize=True)
+        return fig
+
     def save_image(self, filename, mode='rgb', antialiased=False):
         """Save view from all panels to disk
 
         Only mayavi image types are supported:
         (png jpg bmp tiff ps eps pdf rib  oogl iv  vrml obj
 
         Parameters
@@ -2186,16 +2317,15 @@
         Due to limitations in TraitsUI, if multiple views or hemi='split'
         is used, there is no guarantee painting of the windows will
         complete before control is returned to the command line. Thus
         we strongly recommend using only one figure window (which uses
         a Mayavi figure to plot instead of TraitsUI) if you intend to
         script plotting commands.
         """
-        from scipy import misc
-        misc.imsave(filename, self.screenshot(mode, antialiased))
+        self._screenshot_figure(mode, antialiased).savefig(filename)
 
     def screenshot(self, mode='rgb', antialiased=False):
         """Generate a screenshot of current view.
 
         Wraps to :func:`mayavi.mlab.screenshot` for ease of use.
 
         Parameters
@@ -2543,15 +2673,15 @@
         # find indexes at which to create frames
         if tmax is None:
             tmax = self._times[-1]
         elif tmax > self._times[-1]:
             raise ValueError("tmax=%r is greater than the latest time point "
                              "(%r)" % (tmax, self._times[-1]))
         n_frames = floor((tmax - tmin) * time_dilation * framerate)
-        times = np.arange(n_frames)
+        times = np.arange(n_frames, dtype=float)
         times /= framerate * time_dilation
         times += tmin
         interp_func = interp1d(self._times, np.arange(self.n_times))
         time_idx = interp_func(times)
 
         n_times = len(time_idx)
         if n_times == 0:
@@ -2608,15 +2738,15 @@
                 dr /= np.array((n_steps))
                 brain.show_view(beg)
                 for i in range(int(n_steps)):
                     brain._f.scene.camera.orthogonalize_view_up()
                     brain._f.scene.camera.azimuth(dv[0])
                     brain._f.scene.camera.elevation(dv[1])
                     brain._f.scene.renderer.reset_camera_clipping_range()
-                    _force_render([[brain._f]], self._window_backend)
+                    _force_render([[brain._f]])
                     if fname is not None:
                         if not (os.path.isfile(tmp_fname % i) and use_cache):
                             self.save_single_image(tmp_fname % i, row, col)
             except IndexError:
                 pass
         if fname is not None:
             fps = 10
@@ -2631,98 +2761,219 @@
                                 "-noskip",
                                 "-o %s" % fname])
             ret = os.system(enc_cmd)
             if ret:
                 print("\n\nError occured when exporting movie\n\n")
 
 
+def _scale_sequential_lut(lut_table, fmin, fmid, fmax):
+    """Scale a sequential colormap."""
+
+    lut_table_new = lut_table.copy()
+    n_colors = lut_table.shape[0]
+    n_colors2 = n_colors // 2
+
+    # Index of fmid in new colorbar (which position along the N colors would
+    # fmid take, if fmin is first and fmax is last?)
+    fmid_idx = int(np.round(n_colors * ((fmid - fmin) /
+                                        (fmax - fmin))) - 1)
+
+    # morph each color channel so that fmid gets assigned the middle color of
+    # the original table and the number of colors to the left and right are
+    # stretched or squeezed such that they correspond to the distance of fmid
+    # to fmin and fmax, respectively
+    for i in range(4):
+        part1 = np.interp(np.linspace(0, n_colors2 - 1, fmid_idx + 1),
+                          np.arange(n_colors),
+                          lut_table[:, i])
+        lut_table_new[:fmid_idx + 1, i] = part1
+        part2 = np.interp(np.linspace(n_colors2, n_colors - 1,
+                                      n_colors - fmid_idx - 1),
+                          np.arange(n_colors),
+                          lut_table[:, i])
+        lut_table_new[fmid_idx + 1:, i] = part2
+
+    return lut_table_new
+
+
+def _check_limits(fmin, fmid, fmax, extra='f'):
+    """Check for monotonicity."""
+    if fmin >= fmid:
+        raise ValueError('%smin must be < %smid, got %0.4g >= %0.4g'
+                         % (extra, extra, fmin, fmid))
+    if fmid >= fmax:
+        raise ValueError('%smid must be < %smax, got %0.4g >= %0.4g'
+                         % (extra, extra, fmid, fmax))
+
+
+def _get_fill_colors(cols, n_fill):
+    """Get the fill colors for the middle of divergent colormaps.
+
+    Tries to figure out whether there is a smooth transition in the center of
+    the original colormap. If yes, it chooses the color in the center as the
+    only fill color, else it chooses the two colors between which there is
+    a large step in color space to fill up the middle of the new colormap.
+    """
+    steps = np.linalg.norm(np.diff(cols[:, :3].astype(float), axis=0), axis=1)
+
+    # if there is a jump in the middle of the colors
+    # (define a jump as a step in 3D colorspace whose size is 3-times larger
+    # than the mean step size between the first and last steps of the given
+    # colors - I verified that no such jumps exist in the divergent colormaps
+    # of matplotlib 2.0 which all have a smooth transition in the middle)
+    ind = np.flatnonzero(steps[1:-1] > steps[[0, -1]].mean() * 3)
+    if ind.size > 0:
+        # choose the two colors between which there is the large step
+        ind = ind[0] + 1
+        fillcols = np.r_[np.tile(cols[ind, :], (n_fill / 2, 1)),
+                         np.tile(cols[ind + 1, :], (n_fill - n_fill / 2, 1))]
+    else:
+        # choose a color from the middle of the colormap
+        fillcols = np.tile(cols[int(cols.shape[0] / 2), :], (n_fill, 1))
+
+    return fillcols
+
+
 @verbose
 def _scale_mayavi_lut(lut_table, fmin, fmid, fmax, transparent,
-                      verbose=None):
+                      center=None, alpha=1.0, verbose=None):
     """Scale a mayavi colormap LUT to a given fmin, fmid and fmax.
 
     This function operates on a Mayavi LUTManager. This manager can be obtained
     through the traits interface of mayavi. For example:
     ``x.module_manager.vector_lut_manager``.
 
+    Divergent colormaps are respected, if ``center`` is given, see
+    ``Brain.scale_data_colormap`` for more info.
+
     Parameters
     ----------
     lut_orig : array
         The original LUT.
     fmin : float
         minimum value of colormap.
     fmid : float
         value corresponding to color midpoint.
     fmax : float
         maximum value for colormap.
     transparent : boolean
-        if True: use a linear transparency between fmin and fmid.
+        if True: use a linear transparency between fmin and fmid and make
+        values below fmin fully transparent (symmetrically for divergent
+        colormaps)
+    center : float
+        gives the data value that should be mapped to the center of the
+        (divergent) colormap
+    alpha : float
+        sets the overall opacity of colors, maintains transparent regions
     verbose : bool, str, int, or None
         If not None, override default verbose level (see mne.verbose).
 
     Returns
     -------
     lut_table_new : 2D array (n_colors, 4)
         The re-scaled color lookup table
     """
     if not (fmin < fmid) and (fmid < fmax):
         raise ValueError("Invalid colormap, we need fmin<fmid<fmax")
+    if not 0 <= alpha <= 1:
+        raise ValueError("Invalid alpha: it needs to be within [0, 1]")
 
     # Cast inputs to float to prevent integer division
     fmin = float(fmin)
     fmid = float(fmid)
     fmax = float(fmax)
+    _check_limits(fmin, fmid, fmax)
+
+    divergent = center is not None
 
-    logger.info("colormap: fmin=%0.2e fmid=%0.2e fmax=%0.2e "
-                "transparent=%d" % (fmin, fmid, fmax, transparent))
+    trstr = ['(opaque)', '(transparent)']
+    if divergent:
+        logger.info(
+            "colormap divergent: center=%0.2e, [%0.2e, %0.2e, %0.2e] %s"
+            % (center, fmin, fmid, fmax, trstr[transparent]))
+    else:
+        logger.info("colormap sequential: [%0.2e, %0.2e, %0.2e] %s"
+                    % (fmin, fmid, fmax, trstr[transparent]))
+
+    n_colors = lut_table.shape[0]
 
     # Add transparency if needed
     if transparent:
-        n_colors = lut_table.shape[0]
+        if divergent:
+            N4 = np.full(4, n_colors / 4, dtype=int)
+            N4[:np.mod(n_colors, 4)] += 1
+            assert N4.sum() == n_colors
+            lut_table[:, -1] = np.r_[255 * np.ones(N4[0]),
+                                     np.linspace(255, 0, N4[2]),
+                                     np.linspace(0, 255, N4[3]),
+                                     255 * np.ones(N4[1])]
+        else:
+            n_colors2 = int(n_colors / 2)
+            lut_table[:n_colors2, -1] = np.linspace(0, 255, n_colors2)
+            lut_table[n_colors2:, -1] = 255 * np.ones(n_colors - n_colors2)
+
+    alpha = float(alpha)
+    if alpha < 1.0:
+        lut_table[:, -1] = lut_table[:, -1] * alpha
+
+    if divergent:
+        # the colormap should consist of 3 parts: a left part for the negative
+        # data, a right part for the positive data and a middle, fill part
+        # representing the values in [center-fmin, center+fmin], we
+        # introduce this middle part by extending the number of 'colors' of the
+        # original colormap because the Mayavi lut manager scales linearly
+        # between colors and we don't want to reduce the color resolution in
+        # the interesting regions of data space
         n_colors2 = int(n_colors / 2)
-        lut_table[:n_colors2, -1] = np.linspace(0, 255, n_colors2)
-        lut_table[n_colors2:, -1] = 255 * np.ones(n_colors - n_colors2)
+        n_fill = int(round(fmin * n_colors2 / (fmax-fmin))) * 2
+        lut_table = np.r_[
+                _scale_sequential_lut(lut_table[:n_colors2, :],
+                                      center-fmax, center-fmid, center-fmin),
+                _get_fill_colors(
+                    lut_table[n_colors2 - 3:n_colors2 + 3, :], n_fill),
+                _scale_sequential_lut(lut_table[n_colors2:, :],
+                                      center+fmin, center+fmid, center+fmax)]
+    else:
+        lut_table = _scale_sequential_lut(lut_table, fmin, fmid, fmax)
 
-    # Scale the colormap
-    lut_table_new = lut_table.copy()
+    # rescale to 256 colors; this is necessary, because Mayavi/VTK does not
+    # handle a change in the number of colors well: when you change from a long
+    # table to a short table, values beyond the table value range get somehow
+    # not mapped to the colors defined by the table edges; it may be that this
+    # is due to improper setting of the number of table values / colors in the
+    # underlying VTK lookup table, or mapper, but I couldn't figure out where
+    # exactly the fault lies, so simply stick with the constant table size
     n_colors = lut_table.shape[0]
-    n_colors2 = n_colors // 2
-
-    # Index of fmid in new colorbar
-    fmid_idx = int(np.round(n_colors * ((fmid - fmin) /
-                                        (fmax - fmin))) - 1)
-
-    # Go through channels
-    for i in range(4):
-        part1 = np.interp(np.linspace(0, n_colors2 - 1, fmid_idx + 1),
-                          np.arange(n_colors),
-                          lut_table[:, i])
-        lut_table_new[:fmid_idx + 1, i] = part1
-        part2 = np.interp(np.linspace(n_colors2, n_colors - 1,
-                                      n_colors - fmid_idx - 1),
-                          np.arange(n_colors),
-                          lut_table[:, i])
-        lut_table_new[fmid_idx + 1:, i] = part2
+    if n_colors != 256:
+        lut = np.zeros((256, 4))
+        x = np.linspace(1, n_colors, 256)
+        for chan in range(4):
+            lut[:, chan] = np.interp(x,
+                                     np.arange(1, n_colors+1),
+                                     lut_table[:, chan])
+        lut_table = lut
 
-    return lut_table_new
+    return lut_table
 
 
 class _Hemisphere(object):
     """Object for visualizing one hemisphere with mlab"""
     def __init__(self, subject_id, hemi, figure, geo, geo_curv,
-                 geo_kwargs, geo_reverse, subjects_dir, bg_color, backend):
+                 geo_kwargs, geo_reverse, subjects_dir, bg_color, backend,
+                 fg_color):
         if hemi not in ['lh', 'rh']:
             raise ValueError('hemi must be either "lh" or "rh"')
         # Set the identifying info
         self.subject_id = subject_id
         self.hemi = hemi
         self.subjects_dir = subjects_dir
         self.viewdict = viewdicts[hemi]
         self._f = figure
         self._bg_color = bg_color
+        self._fg_color = fg_color
         self._backend = backend
         self.data = {}
         self._mesh_clones = {}  # surface mesh data-sources
 
         # mlab pipeline mesh and surface for geomtery
         meshargs = dict(scalars=geo.bin_curv) if geo_curv else dict()
         with warnings.catch_warnings(record=True):  # traits
@@ -2737,14 +2988,15 @@
             self._geo_mesh.update()
         if 'lut' in geo_kwargs:
             # create a new copy we can modify:
             geo_kwargs = dict(geo_kwargs)
             lut = geo_kwargs.pop('lut')
         else:
             lut = None
+        self._using_lut = bool(geo_curv)
         with warnings.catch_warnings(record=True):  # traits warnings
             self._geo_surf = mlab.pipeline.surface(
                self._geo_mesh, figure=self._f, reset_zoom=True, **geo_kwargs)
         self._geo_surf.actor.property.backface_culling = True
         if lut is not None:
             lut_manager = self._geo_surf.module_manager.scalar_lut_manager
             lut_manager.load_lut_from_list(lut / 255.)
@@ -2760,25 +3012,31 @@
                 vd = self._xfm_view(view, 'd')
                 view = dict(azimuth=vd['v'][0], elevation=vd['v'][1])
                 roll = vd['r']
             except ValueError as v:
                 print(v)
                 raise
 
-        _force_render(self._f, self._backend)
+        _force_render(self._f)
         if view is not None:
+            view = deepcopy(view)
             view['reset_roll'] = True
             view['figure'] = self._f
-            view['distance'] = distance
+            if 'distance' not in view:
+                view['distance'] = distance
+            elif distance is not None and distance != view['distance']:
+                raise ValueError('view parameters view["distance"] != '
+                                 'distance (%s != %s)' % (view['distance'],
+                                                          distance))
             # DO NOT set focal point, can screw up non-centered brains
             # view['focalpoint'] = (0.0, 0.0, 0.0)
             mlab.view(**view)
         if roll is not None:
             mlab.roll(roll=roll, figure=self._f)
-        _force_render(self._f, self._backend)
+        _force_render(self._f)
 
         view = mlab.view(figure=self._f)
         roll = mlab.roll(figure=self._f)
 
         return view, roll
 
     def _xfm_view(self, view, out='s'):
@@ -2845,18 +3103,14 @@
                 else:
                     dv.append(diff)
             dr = np.array(end_d['r']) - np.array(beg_d['r'])
         return (np.array(dv), dr)
 
     def _add_scalar_data(self, data):
         """Add scalar values to dataset"""
-        if mlab.options.backend == 'test':
-            # required SetActiveAttribute filter attributes are not set under
-            # the testing backend
-            return 0, self._geo_mesh
         array_id = self._mesh_dataset.point_data.add_array(data)
         self._mesh_dataset.point_data.get_array(array_id).name = array_id
         self._mesh_dataset.point_data.update()
 
         # build visualization pipeline
         with warnings.catch_warnings(record=True):
             pipe = mlab.pipeline.set_active_attribute(
@@ -2866,18 +3120,14 @@
             if pipe.parent not in self._f.children:
                 self._f.add_child(pipe.parent)
         self._mesh_clones[array_id] = pipe.parent
         return array_id, pipe
 
     def _remove_scalar_data(self, array_id):
         """Removes scalar data"""
-        if mlab.options.backend == 'test':
-            # required SetActiveAttribute filter attributes are not set under
-            # the testing backend
-            return
         self._mesh_clones.pop(array_id).remove()
         self._mesh_dataset.point_data.remove_array(array_id)
 
     def _add_vector_data(self, vectors, vector_values, fmin, fmid, fmax,
                          scale_factor_norm, vertices, vector_alpha, lut):
         vertices = slice(None) if vertices is None else vertices
         x, y, z = np.array(self._geo_mesh.data.points.data)[vertices].T
@@ -2886,16 +3136,15 @@
             quiver = mlab.quiver3d(
                 x, y, z, vectors[:, 0], vectors[:, 1], vectors[:, 2],
                 scalars=vector_values, colormap='hot', vmin=fmin,
                 vmax=fmax, figure=self._f, opacity=vector_alpha)
 
         # Enable backface culling
         quiver.actor.property.backface_culling = False
-        if mlab.options.backend != 'test':
-            quiver.mlab_source.update()
+        quiver.mlab_source.update()
 
         # Compute scaling for the glyphs
         quiver.glyph.glyph.scale_factor = (scale_factor_norm *
                                            vector_values.max())
 
         # Scale colormap used for the glyphs
         l_m = quiver.parent.vector_lut_manager
@@ -2912,35 +3161,37 @@
         array_id, mesh = self._add_scalar_data(old.mlab_data)
 
         if old.pos_lims is not None:
             with warnings.catch_warnings(record=True):
                 pos_thresh = threshold_filter(mesh, low=old.pos_lims[0])
                 pos = mlab.pipeline.surface(
                     pos_thresh, colormap="YlOrRd", figure=self._f,
-                    vmin=old.pos_lims[1], vmax=old.pos_lims[2])
+                    vmin=old.pos_lims[1], vmax=old.pos_lims[2],
+                    reset_zoom=False)
                 pos.actor.property.backface_culling = False
                 pos_bar = mlab.scalarbar(pos, nb_labels=5)
             pos_bar.reverse_lut = True
             pos_bar.scalar_bar_representation.position = (0.53, 0.01)
             pos_bar.scalar_bar_representation.position2 = (0.42, 0.09)
-            self._format_cbar_text(pos_bar)
+            pos_bar.label_text_property.color = self._fg_color
         else:
             pos = pos_bar = None
 
         if old.neg_lims is not None:
             with warnings.catch_warnings(record=True):
                 neg_thresh = threshold_filter(mesh, up=old.neg_lims[0])
                 neg = mlab.pipeline.surface(
                     neg_thresh, colormap="PuBu", figure=self._f,
-                    vmin=old.neg_lims[1], vmax=old.neg_lims[2])
+                    vmin=old.neg_lims[1], vmax=old.neg_lims[2],
+                    reset_zoom=False)
                 neg.actor.property.backface_culling = False
                 neg_bar = mlab.scalarbar(neg, nb_labels=5)
             neg_bar.scalar_bar_representation.position = (0.05, 0.01)
             neg_bar.scalar_bar_representation.position2 = (0.42, 0.09)
-            self._format_cbar_text(neg_bar)
+            neg_bar.label_text_property.color = self._fg_color
         else:
             neg = neg_bar = None
 
         return OverlayDisplay(self, array_id, pos, pos_bar, neg, neg_bar)
 
     @verbose
     def add_data(self, array, fmin, fmid, fmax, thresh, lut, colormap, alpha,
@@ -2983,45 +3234,46 @@
                 warn("Data min is greater than threshold.")
             else:
                 with warnings.catch_warnings(record=True):
                     pipe = threshold_filter(pipe, low=thresh, figure=self._f)
         with warnings.catch_warnings(record=True):
             surf = mlab.pipeline.surface(
                 pipe, colormap=colormap, vmin=fmin, vmax=fmax,
-                opacity=float(alpha), figure=self._f)
+                opacity=float(alpha), figure=self._f, reset_zoom=False)
             surf.actor.property.backface_culling = False
 
         # apply look up table if given
         if lut is not None:
             l_m = surf.module_manager.scalar_lut_manager
             l_m.load_lut_from_list(lut / 255.)
 
         # Get the original colormap table
         orig_ctable = \
             surf.module_manager.scalar_lut_manager.lut.table.to_array().copy()
 
         # Get the colorbar
         if colorbar:
             bar = mlab.scalarbar(surf)
-            self._format_cbar_text(bar)
+            bar.label_text_property.color = self._fg_color
             bar.scalar_bar_representation.position2 = .8, 0.09
         else:
             bar = None
 
         self.data[layer_id] = dict(
             array_id=array_id, mesh=mesh, glyphs=glyphs,
             scale_factor_norm=scale_factor_norm)
         return surf, orig_ctable, bar, glyphs
 
     def add_annotation(self, annot, ids, cmap):
         """Add an annotation file"""
         # Add scalar values to dataset
         array_id, pipe = self._add_scalar_data(ids)
         with warnings.catch_warnings(record=True):
-            surf = mlab.pipeline.surface(pipe, name=annot, figure=self._f)
+            surf = mlab.pipeline.surface(pipe, name=annot, figure=self._f,
+                                         reset_zoom=False)
             surf.actor.property.backface_culling = False
 
         # Set the color table
         l_m = surf.module_manager.scalar_lut_manager
         l_m.load_lut_from_list(cmap / 255.)
 
         # Set the brain attributes
@@ -3029,35 +3281,39 @@
                     array_id=array_id)
 
     def add_label(self, label, label_name, color, alpha):
         """Add an ROI label to the image"""
         from matplotlib.colors import colorConverter
         array_id, pipe = self._add_scalar_data(label)
         with warnings.catch_warnings(record=True):
-            surf = mlab.pipeline.surface(pipe, name=label_name, figure=self._f)
+            surf = mlab.pipeline.surface(pipe, name=label_name, figure=self._f,
+                                         reset_zoom=False)
             surf.actor.property.backface_culling = False
         color = colorConverter.to_rgba(color, alpha)
         cmap = np.array([(0, 0, 0, 0,), color])
         l_m = surf.module_manager.scalar_lut_manager
-        l_m.load_lut_from_list(cmap)
+        # for some reason (traits?) using `load_lut_from_list` here does
+        # not work (.data_range needs to be tweaked in this case),
+        # but setting the table directly does:
+        l_m.lut.table = np.round(cmap * 255).astype(np.uint8)
         return array_id, surf
 
     def add_morphometry(self, morph_data, colormap, measure,
                         min, max, colorbar):
         """Add a morphometry overlay to the image"""
         array_id, pipe = self._add_scalar_data(morph_data)
         with warnings.catch_warnings(record=True):
-            surf = mlab.pipeline.surface(pipe, colormap=colormap,
-                                         vmin=min, vmax=max,
-                                         name=measure, figure=self._f)
+            surf = mlab.pipeline.surface(
+                pipe, colormap=colormap, vmin=min, vmax=max, name=measure,
+                figure=self._f, reset_zoom=False)
 
         # Get the colorbar
         if colorbar:
             bar = mlab.scalarbar(surf)
-            self._format_cbar_text(bar)
+            bar.label_text_property.color = self._fg_color
             bar.scalar_bar_representation.position2 = .8, 0.09
         else:
             bar = None
 
         # Fil in the morphometry dict
         return dict(surface=surf, colorbar=bar, measure=measure, brain=self,
                     array_id=array_id)
@@ -3075,35 +3331,37 @@
     def add_contour_overlay(self, scalar_data, min=None, max=None,
                             n_contours=7, line_width=1.5, lut=None,
                             colorbar=True):
         """Add a topographic contour overlay of the positive data"""
         array_id, pipe = self._add_scalar_data(scalar_data)
         with warnings.catch_warnings(record=True):
             thresh = threshold_filter(pipe, low=min)
-            surf = mlab.pipeline.contour_surface(thresh, contours=n_contours,
-                                                 line_width=line_width)
+            surf = mlab.pipeline.contour_surface(
+                thresh, contours=n_contours, line_width=line_width,
+                reset_zoom=False)
         if lut is not None:
             l_m = surf.module_manager.scalar_lut_manager
             l_m.load_lut_from_list(lut / 255.)
 
         # Set the colorbar and range correctly
         with warnings.catch_warnings(record=True):  # traits
             bar = mlab.scalarbar(surf, nb_colors=n_contours,
                                  nb_labels=n_contours + 1)
         bar.data_range = min, max
-        self._format_cbar_text(bar)
+        bar.label_text_property.color = self._fg_color
         bar.scalar_bar_representation.position2 = .8, 0.09
         if not colorbar:
             bar.visible = False
 
         # Set up a dict attribute with pointers at important things
         return dict(surface=surf, colorbar=bar, brain=self, array_id=array_id)
 
     def add_text(self, x, y, text, name, color=None, opacity=1.0):
         """ Add a text to the visualization"""
+        color = self._fg_color if color is None else color
         with warnings.catch_warnings(record=True):
             text = mlab.text(x, y, text, name=name, color=color,
                              opacity=opacity, figure=self._f)
             return text
 
     def remove_data(self, layer_id):
         """Remove data shown with .add_data()"""
@@ -3113,29 +3371,27 @@
 
     def set_data(self, layer_id, values, vectors=None, vector_values=None):
         """Set displayed data values and vectors."""
         data = self.data[layer_id]
         self._mesh_dataset.point_data.get_array(
             data['array_id']).from_array(values)
         # avoid "AttributeError: 'Scene' object has no attribute 'update'"
-        if mlab.options.backend != 'test':
-            data['mesh'].update()
+        data['mesh'].update()
         if vectors is not None:
             q = data['glyphs']
 
             # extract params that will change after calling .update()
             l_m = q.parent.vector_lut_manager
             data_range = np.array(l_m.data_range)
             lut = l_m.lut.table.to_array().copy()
 
             # Update glyphs
             q.mlab_source.vectors = vectors
             q.mlab_source.scalars = vector_values
-            if mlab.options.backend != 'test':
-                q.mlab_source.update()
+            q.mlab_source.update()
 
             # Update changed parameters, and glyph scaling
             q.glyph.glyph.scale_factor = (data['scale_factor_norm'] *
                                           values.max())
             l_m.load_lut_from_list(lut / 255.)
             l_m.data_range = data_range
 
@@ -3143,27 +3399,20 @@
         """Set lights to come from same direction relative to brain."""
         if self.hemi == "rh":
             if self._f.scene is not None and \
                     self._f.scene.light_manager is not None:
                 for light in self._f.scene.light_manager.lights:
                     light.azimuth *= -1
 
-    def _format_cbar_text(self, cbar):
-        bg_color = self._bg_color
-        if bg_color is None or sum(bg_color) < 2:
-            text_color = (1., 1., 1.)
-        else:
-            text_color = (0., 0., 0.)
-        cbar.label_text_property.color = text_color
-
     def update_surf(self):
-        "Update surface mesh after mesh coordinates change"
-        self._geo_mesh.update()
-        for mesh in self._mesh_clones.values():
-            mesh.update()
+        """Update surface mesh after mesh coordinates change."""
+        with warnings.catch_warnings(record=True):  # traits
+            self._geo_mesh.update()
+            for mesh in self._mesh_clones.values():
+                mesh.update()
 
 
 class OverlayData(object):
     """Encapsulation of statistical neuroimaging overlay viz data"""
 
     def __init__(self, scalar_data, min, max, sign):
         if scalar_data.min() >= 0:
@@ -3224,15 +3473,14 @@
 
     Parameters
     ----------
     brain : Brain (or list of Brain)
         brain(s) to control
     """
     # Nested import of traisui for setup.py without X server
-    from traitsui.api import (View, Item, VSplit, HSplit, Group)
     min_time = Int(0)
     max_time = Int(1E9)
     current_time = Range(low="min_time", high="max_time", value=0)
     # colormap: only update when user presses Enter
     fmax = Float(enter_set=True, auto_set=False)
     fmid = Float(enter_set=True, auto_set=False)
     fmin = Float(enter_set=True, auto_set=False)
@@ -3271,14 +3519,15 @@
         self._disable_updates = True
         self.max_time = len(props["time"]) - 1
         self.current_time = props["time_idx"]
         self.fmin = props["fmin"]
         self.fmid = props["fmid"]
         self.fmax = props["fmax"]
         self.transparent = props["transparent"]
+        self.center = props["center"]
         if props["smoothing_steps"] is None:
             self.smoothing_steps = -1
         else:
             self.smoothing_steps = props["smoothing_steps"]
         self._disable_updates = False
 
         # Make sure all brains have the same time points
@@ -3288,50 +3537,50 @@
                 raise ValueError("all brains must have the same time"
                                  "points")
 
         # Show GUI
         self.configure_traits()
 
     @on_trait_change("smoothing_steps")
-    def set_smoothing_steps(self):
+    def _set_smoothing_steps(self):
         """ Change number of smooting steps
         """
         if self._disable_updates:
             return
 
         smoothing_steps = self.smoothing_steps
         if smoothing_steps < 0:
             smoothing_steps = None
 
         for brain in self.brains:
             brain.set_data_smoothing_steps(self.smoothing_steps)
 
     @on_trait_change("orientation")
-    def set_orientation(self):
+    def _set_orientation(self):
         """ Set the orientation
         """
         if self._disable_updates:
             return
 
         for brain in self.brains:
             brain.show_view(view=self.orientation)
 
     @on_trait_change("current_time")
-    def set_time_point(self):
+    def _set_time_point(self):
         """ Set the time point shown
         """
         if self._disable_updates:
             return
 
         for brain in self.brains:
             brain.set_data_time_index(self.current_time)
 
     @on_trait_change("fmin, fmid, fmax, transparent")
-    def scale_colormap(self):
+    def _scale_colormap(self):
         """ Scale the colormap
         """
         if self._disable_updates:
             return
 
         for brain in self.brains:
             brain.scale_data_colormap(self.fmin, self.fmid, self.fmax,
-                                      self.transparent)
+                                      self.transparent, self.center)
```

### Comparing `pysurfer-0.8.0/bin/pysurfer` & `pysurfer-0.9.0/bin/pysurfer`

 * *Files identical despite different names*

