# Comparing `tmp/pytictoc-1.5.2.tar.gz` & `tmp/pytictoc-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictoc-1.5.2.tar", last modified: Fri Apr 23 17:14:06 2021, max compression
+gzip compressed data, was "pytictoc-1.5.3.tar", last modified: Wed Aug  2 20:07:50 2023, max compression
```

## Comparing `pytictoc-1.5.2.tar` & `pytictoc-1.5.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2021-04-23 17:14:06.303451 pytictoc-1.5.2/
--rw-rw-rw-   0        0        0     3482 2021-04-23 17:14:06.303084 pytictoc-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2260 2017-09-29 19:22:46.000000 pytictoc-1.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2021-04-23 17:14:06.301123 pytictoc-1.5.2/pytictoc.egg-info/
--rw-rw-rw-   0        0        0     3482 2021-04-23 17:14:06.000000 pytictoc-1.5.2/pytictoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2021-04-23 17:14:06.000000 pytictoc-1.5.2/pytictoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-23 17:14:06.000000 pytictoc-1.5.2/pytictoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-04-23 17:14:06.000000 pytictoc-1.5.2/pytictoc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2614 2021-04-23 16:46:46.000000 pytictoc-1.5.2/pytictoc.py
--rw-rw-rw-   0        0        0       42 2021-04-23 17:14:06.304082 pytictoc-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     3901 2021-04-23 17:05:30.000000 pytictoc-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:07:50.882022 pytictoc-1.5.3/
+-rw-rw-rw-   0        0        0     1487 2021-04-23 18:22:20.000000 pytictoc-1.5.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2891 2023-08-02 20:07:50.882022 pytictoc-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2260 2017-09-29 19:22:48.000000 pytictoc-1.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 20:07:50.877950 pytictoc-1.5.3/pytictoc.egg-info/
+-rw-rw-rw-   0        0        0     2891 2023-08-02 20:07:50.000000 pytictoc-1.5.3/pytictoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-08-02 20:07:50.000000 pytictoc-1.5.3/pytictoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:07:50.000000 pytictoc-1.5.3/pytictoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 20:07:50.000000 pytictoc-1.5.3/pytictoc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2614 2023-08-02 20:04:24.000000 pytictoc-1.5.3/pytictoc.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:07:50.882022 pytictoc-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     3907 2023-08-02 20:04:03.000000 pytictoc-1.5.3/setup.py
```

### Comparing `pytictoc-1.5.2/PKG-INFO` & `pytictoc-1.5.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,74 @@
-Metadata-Version: 1.1
-Name: pytictoc
-Version: 1.5.2
-Summary: Time code using syntax similar to tic and toc in MATLAB
-Home-page: https://github.com/ericcfields/pytictoc
-Author: Eric Fields
-Author-email: eric.fields@bc.edu
-License: BSD (three-clause)
-Description: pytictoc contains a class TicToc which replicates the functionality of MATLAB's tic and toc for easily timing sections of code. Under the hood, pytictoc uses the default_timer function from Python's timeit module.
-        
-        =============
-        INSTALLATION
-        =============
-        
-        pytictoc can be installed and updated via conda or pip.
-        
-        **pip** ::
-         
-          pip install pytictoc
-          pip install pytictoc --upgrade
-        
-        **conda** ::
-        
-          conda install pytictoc -c ecf
-          conda update pytictoc -c ecf
-        
-        
-        =============
-        USAGE
-        ============= 
-        
-        Basic usage: ::
-        
-          >> from pytictoc import TicToc
-          >> t = TicToc() #create instance of class
-        
-          >> t.tic() #Start timer
-          >> t.toc() #Time elapsed since t.tic()
-          Elapsed time is 2.612231 seconds.
-        
-        A string passed to the toc method changes the printed message. This can be useful to differentiate timing of different sections in the same script. ::
-        
-          >> t.toc('Section 1 took')
-          Section 1 took 16.494467 seconds.
-        
-        An optional keyword argument restarts the timer (equivalent to t.tic()) after reporting the time elapsed. ::
-        
-          >> t.toc(restart=True)
-          Elapsed time is 36.986837 seconds.
-          >>t.toc()
-          Elapsed time is 2.393425 seconds.
-        
-        If you want to return the time elapsed to a variable rather than printing it, use the tocvalue method. ::
-        
-          >>spam = t.tocvalue()
-          >>spam
-          20.156261717544602
-        
-        The TicToc class can be used within a context manager as an alternative way to time a section of code. The time taken to run the code inside the with statement will be reported on exit. ::
-         
-          >>with TicToc():
-          >>    spam = [x+1 for x in range(10000)]
-          Elapsed time is 0.002343 seconds.
-        
-        ------------------------------------
-        Determining and setting the timer
-        ------------------------------------
-        
-        pytictoc uses timeit.default_timer to time code. On Python 3.3 and later, this is an alias for time.perf_counter. On earlier versions of Python it is an alias for the most precise timer for a given system. 
-        
-        To see which function is being used: ::
-        
-          >>import pytictoc
-          >>pytictoc.default_timer
-          <function time.perf_counter>
-        
-        You can change the timer by simple assignment. ::
-          
-          >>import time
-          >>pytictoc.default_timer = time.clock
-          >>pytictoc.default_timer
-          <function time.clock>
-        
-Keywords: timing tic toc MATLAB
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
+pytictoc contains a class TicToc which replicates the functionality of MATLAB's tic and toc for easily timing sections of code. Under the hood, pytictoc uses the default_timer function from Python's timeit module.
+
+=============
+INSTALLATION
+=============
+
+pytictoc can be installed and updated via conda or pip.
+
+**pip** ::
+ 
+  pip install pytictoc
+  pip install pytictoc --upgrade
+
+**conda** ::
+
+  conda install pytictoc -c ecf
+  conda update pytictoc -c ecf
+
+
+=============
+USAGE
+============= 
+
+Basic usage: ::
+
+  >> from pytictoc import TicToc
+  >> t = TicToc() #create instance of class
+
+  >> t.tic() #Start timer
+  >> t.toc() #Time elapsed since t.tic()
+  Elapsed time is 2.612231 seconds.
+
+A string passed to the toc method changes the printed message. This can be useful to differentiate timing of different sections in the same script. ::
+
+  >> t.toc('Section 1 took')
+  Section 1 took 16.494467 seconds.
+
+An optional keyword argument restarts the timer (equivalent to t.tic()) after reporting the time elapsed. ::
+
+  >> t.toc(restart=True)
+  Elapsed time is 36.986837 seconds.
+  >>t.toc()
+  Elapsed time is 2.393425 seconds.
+
+If you want to return the time elapsed to a variable rather than printing it, use the tocvalue method. ::
+
+  >>spam = t.tocvalue()
+  >>spam
+  20.156261717544602
+
+The TicToc class can be used within a context manager as an alternative way to time a section of code. The time taken to run the code inside the with statement will be reported on exit. ::
+ 
+  >>with TicToc():
+  >>    spam = [x+1 for x in range(10000)]
+  Elapsed time is 0.002343 seconds.
+
+------------------------------------
+Determining and setting the timer
+------------------------------------
+
+pytictoc uses timeit.default_timer to time code. On Python 3.3 and later, this is an alias for time.perf_counter. On earlier versions of Python it is an alias for the most precise timer for a given system. 
+
+To see which function is being used: ::
+
+  >>import pytictoc
+  >>pytictoc.default_timer
+  <function time.perf_counter>
+
+You can change the timer by simple assignment. ::
+  
+  >>import time
+  >>pytictoc.default_timer = time.clock
+  >>pytictoc.default_timer
+  <function time.clock>
```

### Comparing `pytictoc-1.5.2/pytictoc.py` & `pytictoc-1.5.3/pytictoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 Module with class TicToc to replicate the functionality of MATLAB's tic and toc.
 
 Documentation: https://pypi.python.org/pypi/pytictoc
 """
 
 __author__       = 'Eric Fields'
-__version__      = '1.5.2'
-__version_date__ = '23 April 2021'
+__version__      = '1.5.3'
+__version_date__ = '2 August 2023'
 
 
 from timeit import default_timer
 
 class TicToc(object):
     
     """
```

### Comparing `pytictoc-1.5.2/setup.py` & `pytictoc-1.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #AUTHOR: Eric Fields
-#VERSION DATE: 23 April 2021
+#VERSION DATE: 2 August 2023
 
 """
 Setup file to add pytictoc to PyPi
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
@@ -20,25 +20,25 @@
 
 setup(
     name='pytictoc',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.5.2',
+    version='1.5.3',
 
     description='Time code using syntax similar to tic and toc in MATLAB',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/ericcfields/pytictoc',
 
     # Author details
     author='Eric Fields',
-    author_email='eric.fields@bc.edu',
+    author_email='fieldsec@westminster.edu',
 
     # Choose your license
     license='BSD (three-clause)',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
```

