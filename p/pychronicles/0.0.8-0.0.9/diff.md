# Comparing `tmp/pychronicles-0.0.8.tar.gz` & `tmp/pychronicles-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychronicles-0.0.8.tar", last modified: Fri Aug 12 16:35:04 2022, max compression
+gzip compressed data, was "pychronicles-0.0.9.tar", last modified: Tue Oct 18 15:29:36 2022, max compression
```

## Comparing `pychronicles-0.0.8.tar` & `pychronicles-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 tguyet    (1000) tguyet    (1000)        0 2022-08-12 16:35:04.894098 pychronicles-0.0.8/
--rw-r--r--   0 tguyet    (1000) tguyet    (1000)    35150 2020-07-08 15:09:08.000000 pychronicles-0.0.8/LICENCE
--rw-r--r--   0 tguyet    (1000) tguyet    (1000)       25 2020-07-15 08:32:37.000000 pychronicles-0.0.8/MANIFEST.in
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)     4604 2022-08-12 16:35:04.894098 pychronicles-0.0.8/PKG-INFO
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)     4138 2022-08-11 15:59:59.000000 pychronicles-0.0.8/README.md
-drwxrwxr-x   0 tguyet    (1000) tguyet    (1000)        0 2022-08-12 16:35:04.894098 pychronicles-0.0.8/pychronicles/
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)      185 2022-08-11 15:59:59.000000 pychronicles-0.0.8/pychronicles/__init__.py
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)     5696 2022-08-04 17:45:11.000000 pychronicles-0.0.8/pychronicles/chroaring.py
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)  1594276 2022-08-12 16:34:33.000000 pychronicles-0.0.8/pychronicles/chronicle.c
--rwxrwxr-x   0 tguyet    (1000) tguyet    (1000)  2474352 2022-08-12 16:34:42.000000 pychronicles-0.0.8/pychronicles/chronicle.cpython-310-x86_64-linux-gnu.so
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)    34525 2022-08-12 13:53:07.000000 pychronicles-0.0.8/pychronicles/chronicle.py
--rwxrwxr-x   0 tguyet    (1000) tguyet    (1000)    48132 2022-08-12 14:14:25.000000 pychronicles-0.0.8/pychronicles/chronicle.pyx
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)    37329 2022-08-04 17:44:44.000000 pychronicles-0.0.8/pychronicles/chronicle_multi.py
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)    50275 2022-08-12 14:16:50.000000 pychronicles-0.0.8/pychronicles/chronicle_python.py
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)     1050 2022-08-04 17:46:02.000000 pychronicles-0.0.8/pychronicles/test_cmp_chro.py
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)    48143 2022-08-12 12:35:09.000000 pychronicles-0.0.8/pychronicles/test_python.py
-drwxrwxr-x   0 tguyet    (1000) tguyet    (1000)        0 2022-08-12 16:35:04.894098 pychronicles-0.0.8/pychronicles.egg-info/
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)     4604 2022-08-12 16:35:04.000000 pychronicles-0.0.8/pychronicles.egg-info/PKG-INFO
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)      548 2022-08-12 16:35:04.000000 pychronicles-0.0.8/pychronicles.egg-info/SOURCES.txt
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)        1 2022-08-12 16:35:04.000000 pychronicles-0.0.8/pychronicles.egg-info/dependency_links.txt
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)       59 2022-08-12 16:35:04.000000 pychronicles-0.0.8/pychronicles.egg-info/requires.txt
--rwxrwxrwx   0 tguyet    (1000) tguyet    (1000)       13 2022-08-12 16:35:04.000000 pychronicles-0.0.8/pychronicles.egg-info/top_level.txt
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)       38 2022-08-12 16:35:04.894098 pychronicles-0.0.8/setup.cfg
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)     1206 2022-08-12 16:34:18.000000 pychronicles-0.0.8/setup.py
-drwxrwxr-x   0 tguyet    (1000) tguyet    (1000)        0 2022-08-12 16:35:04.894098 pychronicles-0.0.8/test/
--rw-rw-r--   0 tguyet    (1000) tguyet    (1000)     1878 2022-08-12 12:10:56.000000 pychronicles-0.0.8/test/test_ext_pandas.py
+drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       25 2022-10-18 10:07:43.000000 pychronicles-0.0.9/MANIFEST.in
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     5491 2022-10-18 15:29:36.044332 pychronicles-0.0.9/PKG-INFO
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     4239 2022-10-18 10:07:43.000000 pychronicles-0.0.9/README.md
+drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/pychronicles/
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)      325 2022-10-18 10:07:43.000000 pychronicles-0.0.9/pychronicles/__init__.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)   905848 2022-10-18 15:27:54.000000 pychronicles-0.0.9/pychronicles/chronicle.c
+-rwxrwxr-x   0 tguyet    (1001) tguyet    (1001)  7746896 2022-10-18 15:28:06.000000 pychronicles-0.0.9/pychronicles/chronicle.cpython-38-x86_64-linux-gnu.so
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)    25019 2022-10-18 15:23:49.000000 pychronicles-0.0.9/pychronicles/chronicle.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)    10490 2022-10-18 15:24:12.000000 pychronicles-0.0.9/pychronicles/fchronicle.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     6155 2022-10-18 14:16:22.000000 pychronicles-0.0.9/pychronicles/mtlformula.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     6276 2022-10-18 14:17:23.000000 pychronicles-0.0.9/pychronicles/pandas_tpatterns.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     4803 2022-10-18 10:07:43.000000 pychronicles-0.0.9/pychronicles/timedsequence.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     3346 2022-10-18 10:07:43.000000 pychronicles-0.0.9/pychronicles/utils.py
+drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/pychronicles.egg-info/
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     5491 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/PKG-INFO
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)      525 2022-10-18 15:29:36.000000 pychronicles-0.0.9/pychronicles.egg-info/SOURCES.txt
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)        1 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/dependency_links.txt
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       59 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/requires.txt
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       19 2022-10-18 15:29:35.000000 pychronicles-0.0.9/pychronicles.egg-info/top_level.txt
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)       38 2022-10-18 15:29:36.044332 pychronicles-0.0.9/setup.cfg
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     1205 2022-10-18 15:28:55.000000 pychronicles-0.0.9/setup.py
+drwxrwxr-x   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:29:36.044332 pychronicles-0.0.9/tests/
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)        0 2022-10-18 15:20:11.000000 pychronicles-0.0.9/tests/__init__.py
+-rw-rw-r--   0 tguyet    (1001) tguyet    (1001)     2536 2022-10-18 15:21:18.000000 pychronicles-0.0.9/tests/test_timedsequences.py
```

### Comparing `pychronicles-0.0.8/PKG-INFO` & `pychronicles-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-Metadata-Version: 2.1
-Name: pychronicles
-Version: 0.0.8
-Summary: A package for chronicle recognition
-Home-page: https://gitlab.inria.fr/tguyet/pychronicles
-Author: Thomas Guyet
-Author-email: thomas.guyet@inria.fr
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENCE
+[![PyPI version](https://badge.fury.io/py/pychronicles.svg)](https://badge.fury.io/py/pychronicles)
 
 # PyChronicle package
 
 A chronicle is a specification of the complex temporal behaviors as a graph of temporal constraints. More specifically, a chronicle is a multiset of events and a set of temporal constraints specifying that occurrences of pairs of events must occurs within a given temporal interval.
 It can be used to recognize complex behaviors in sequence the temporal events.
 
 This library proposes a Python class to define a chronicle, to read/save them in a standard CRS format. The main useful functionnality for chronicle is their efficient matching in a temporal sequence.
```

### Comparing `pychronicles-0.0.8/README.md` & `pychronicles-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,110 @@
-# PyChronicle package
-
-A chronicle is a specification of the complex temporal behaviors as a graph of temporal constraints. More specifically, a chronicle is a multiset of events and a set of temporal constraints specifying that occurrences of pairs of events must occurs within a given temporal interval.
-It can be used to recognize complex behaviors in sequence the temporal events.
-
-This library proposes a Python class to define a chronicle, to read/save them in a standard CRS format. The main useful functionnality for chronicle is their efficient matching in a temporal sequence.
-
-A temporal sequence may have three different format:
-* a simple list of items (str, int or None) with implicit timestamps : `['a', 'b', ..., None, 'c', None, 'd']`
-* a list of explicitly timestamped items (str or int) : `[ (1,'a'), (23,'b'), (30,'c'), (45, 'd')]`
-* a pandas dataframe indexed by timestamps and using the items in a columns (named `label`)
-
-The chronicles handles to model of timestamps (for the last two types of sequence models):
-* discrete timestamps using integers
-* continuous timestamps using `datetime` format. In this case the temporal constraints of a chronicle must be defined using `timedelta` values.
-
-The package implements efficient algorithms to recognize it. It benefits from pandas functionalities to increase their efficiency. There are three different ways to _recognize_ a chronicle in a sequence of a events:
-* the absence/presence recognition (`c.match(seq)`): its result is a boolean stating whether the chronicle occur at least once in the sequence, this is the most efficient algorithm
-* the occurrence enumeration (`c.recognize(seq)`): its result is a list of occurrence of the chronicle in a sequence. Contrary to the first implementation, it looks for all possible combinasion of events. Thus it is less efficient
-* the approximate occurrence enumeration (`c.cmp(seq, 0.7)`): its result is a list of occurrences that are similar of the chronicle with a similarity threshold of 0.7.
-
-In addition, when using a pandas dataframe which contains several sequences (indexed with an attribute), it is possible to request for matching a chronicle in all sequences (no specific optimisation).
-
-
-Please note that the author is not fully satisfied by the function name and that it appeals to change them in a short delay ...
-
-# Perspectives
-
-* extend the chronicle model for pandas dataframe by specifying event by a couple (attribute, value), that can be used to specify a wider range of complex behavior in multidimensional sequences
-* graphical interfaces to edit chronicle (for instance with dash)
-* better cythonize the recognition
-* optimized matching of several chronicles at the same time
-
-
-# Requirements
-
-Use `pip install -r requirements.txt` to install requirements.
-
-Naturally, the latter may require superuser rights (consider prefixing the commands by sudo).
-
-If you want to use Python 3 and your system defaults on Python 2.7, you may need to adjust the above commands, e.g., replace pip by pip3.
-
-The required libraries are the following
-* numpy
-* scipy
-* lazr.restfulclient
-* larz.uri
-* typing
-* pandas
-
-LAZR is used to instantiate chronicles from CRS files (with simple grammar).
-
-# Usage
-
-Example of usage:
-
-    from pychronicles import *
-    #define a sequence of events
-    seq = [3,4,'b','a','a',1,3,'coucou','b','coucou',5,'coucou',5]
-    
-    #define a chronicle
-    c=Chronicle()
-    c.add_event(0,'b')
-    c.add_event(1,1)
-    c.add_constraint(1,3, (3,45))
-    print(c)
-    
-    #recognize the chronicle in the sequence
-    occs=c.recognize(seq)
-    print("occurrences: "+str(occs))
-
-It is possible to specify chronicles using the CRS format. The following code illustrate the syntax for specifying a chronicle in this format.
-
-    chronicle C27_sub_0[]()
-    {
-	    event(Event_Type1[], t006)
-	    event(Event_Type1[], t004)
-	    event(Event_Type2[], t002)
-	    event(Event_Type3[], t001)
-
-	    t004-t006 in [17,25]
-	    t006-t002 in [-16,-10]
-	    t002-t001 in [14,29]
-	    t004-t001 in [27,35]
-    }
-
-
-# Authorship
-
-* **Author:** Thomas Guyet
-* **Institution:** Inria
-* **date:** 8/2022
-
+Metadata-Version: 2.1
+Name: pychronicles
+Version: 0.0.9
+Summary: A package for chronicle recognition
+Home-page: https://gitlab.inria.fr/tguyet/pychronicles
+Author: Thomas Guyet
+Author-email: thomas.guyet@inria.fr
+License: UNKNOWN
+Description: [![PyPI version](https://badge.fury.io/py/pychronicles.svg)](https://badge.fury.io/py/pychronicles)
+        
+        # PyChronicle package
+        
+        A chronicle is a specification of the complex temporal behaviors as a graph of temporal constraints. More specifically, a chronicle is a multiset of events and a set of temporal constraints specifying that occurrences of pairs of events must occurs within a given temporal interval.
+        It can be used to recognize complex behaviors in sequence the temporal events.
+        
+        This library proposes a Python class to define a chronicle, to read/save them in a standard CRS format. The main useful functionnality for chronicle is their efficient matching in a temporal sequence.
+        
+        A temporal sequence may have three different format:
+        * a simple list of items (str, int or None) with implicit timestamps : `['a', 'b', ..., None, 'c', None, 'd']`
+        * a list of explicitly timestamped items (str or int) : `[ (1,'a'), (23,'b'), (30,'c'), (45, 'd')]`
+        * a pandas dataframe indexed by timestamps and using the items in a columns (named `label`)
+        
+        The chronicles handles to model of timestamps (for the last two types of sequence models):
+        * discrete timestamps using integers
+        * continuous timestamps using `datetime` format. In this case the temporal constraints of a chronicle must be defined using `timedelta` values.
+        
+        The package implements efficient algorithms to recognize it. It benefits from pandas functionalities to increase their efficiency. There are three different ways to _recognize_ a chronicle in a sequence of a events:
+        * the absence/presence recognition (`c.match(seq)`): its result is a boolean stating whether the chronicle occur at least once in the sequence, this is the most efficient algorithm
+        * the occurrence enumeration (`c.recognize(seq)`): its result is a list of occurrence of the chronicle in a sequence. Contrary to the first implementation, it looks for all possible combinasion of events. Thus it is less efficient
+        * the approximate occurrence enumeration (`c.cmp(seq, 0.7)`): its result is a list of occurrences that are similar of the chronicle with a similarity threshold of 0.7.
+        
+        In addition, when using a pandas dataframe which contains several sequences (indexed with an attribute), it is possible to request for matching a chronicle in all sequences (no specific optimisation).
+        
+        
+        Please note that the author is not fully satisfied by the function name and that it appeals to change them in a short delay ...
+        
+        # Perspectives
+        
+        * extend the chronicle model for pandas dataframe by specifying event by a couple (attribute, value), that can be used to specify a wider range of complex behavior in multidimensional sequences
+        * graphical interfaces to edit chronicle (for instance with dash)
+        * better cythonize the recognition
+        * optimized matching of several chronicles at the same time
+        
+        
+        # Requirements
+        
+        Use `pip install -r requirements.txt` to install requirements.
+        
+        Naturally, the latter may require superuser rights (consider prefixing the commands by sudo).
+        
+        If you want to use Python 3 and your system defaults on Python 2.7, you may need to adjust the above commands, e.g., replace pip by pip3.
+        
+        The required libraries are the following
+        * numpy
+        * scipy
+        * lazr.restfulclient
+        * larz.uri
+        * typing
+        * pandas
+        
+        LAZR is used to instantiate chronicles from CRS files (with simple grammar).
+        
+        # Usage
+        
+        Example of usage:
+        
+            from pychronicles import *
+            #define a sequence of events
+            seq = [3,4,'b','a','a',1,3,'coucou','b','coucou',5,'coucou',5]
+            
+            #define a chronicle
+            c=Chronicle()
+            c.add_event(0,'b')
+            c.add_event(1,1)
+            c.add_constraint(1,3, (3,45))
+            print(c)
+            
+            #recognize the chronicle in the sequence
+            occs=c.recognize(seq)
+            print("occurrences: "+str(occs))
+        
+        It is possible to specify chronicles using the CRS format. The following code illustrate the syntax for specifying a chronicle in this format.
+        
+            chronicle C27_sub_0[]()
+            {
+        	    event(Event_Type1[], t006)
+        	    event(Event_Type1[], t004)
+        	    event(Event_Type2[], t002)
+        	    event(Event_Type3[], t001)
+        
+        	    t004-t006 in [17,25]
+        	    t006-t002 in [-16,-10]
+        	    t002-t001 in [14,29]
+        	    t004-t001 in [27,35]
+            }
+        
+        
+        # Authorship
+        
+        * **Author:** Thomas Guyet
+        * **Institution:** Inria
+        * **date:** 8/2022
+        
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `pychronicles-0.0.8/pychronicles.egg-info/PKG-INFO` & `pychronicles-0.0.9/pychronicles.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,110 @@
 Metadata-Version: 2.1
 Name: pychronicles
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for chronicle recognition
 Home-page: https://gitlab.inria.fr/tguyet/pychronicles
 Author: Thomas Guyet
 Author-email: thomas.guyet@inria.fr
+License: UNKNOWN
+Description: [![PyPI version](https://badge.fury.io/py/pychronicles.svg)](https://badge.fury.io/py/pychronicles)
+        
+        # PyChronicle package
+        
+        A chronicle is a specification of the complex temporal behaviors as a graph of temporal constraints. More specifically, a chronicle is a multiset of events and a set of temporal constraints specifying that occurrences of pairs of events must occurs within a given temporal interval.
+        It can be used to recognize complex behaviors in sequence the temporal events.
+        
+        This library proposes a Python class to define a chronicle, to read/save them in a standard CRS format. The main useful functionnality for chronicle is their efficient matching in a temporal sequence.
+        
+        A temporal sequence may have three different format:
+        * a simple list of items (str, int or None) with implicit timestamps : `['a', 'b', ..., None, 'c', None, 'd']`
+        * a list of explicitly timestamped items (str or int) : `[ (1,'a'), (23,'b'), (30,'c'), (45, 'd')]`
+        * a pandas dataframe indexed by timestamps and using the items in a columns (named `label`)
+        
+        The chronicles handles to model of timestamps (for the last two types of sequence models):
+        * discrete timestamps using integers
+        * continuous timestamps using `datetime` format. In this case the temporal constraints of a chronicle must be defined using `timedelta` values.
+        
+        The package implements efficient algorithms to recognize it. It benefits from pandas functionalities to increase their efficiency. There are three different ways to _recognize_ a chronicle in a sequence of a events:
+        * the absence/presence recognition (`c.match(seq)`): its result is a boolean stating whether the chronicle occur at least once in the sequence, this is the most efficient algorithm
+        * the occurrence enumeration (`c.recognize(seq)`): its result is a list of occurrence of the chronicle in a sequence. Contrary to the first implementation, it looks for all possible combinasion of events. Thus it is less efficient
+        * the approximate occurrence enumeration (`c.cmp(seq, 0.7)`): its result is a list of occurrences that are similar of the chronicle with a similarity threshold of 0.7.
+        
+        In addition, when using a pandas dataframe which contains several sequences (indexed with an attribute), it is possible to request for matching a chronicle in all sequences (no specific optimisation).
+        
+        
+        Please note that the author is not fully satisfied by the function name and that it appeals to change them in a short delay ...
+        
+        # Perspectives
+        
+        * extend the chronicle model for pandas dataframe by specifying event by a couple (attribute, value), that can be used to specify a wider range of complex behavior in multidimensional sequences
+        * graphical interfaces to edit chronicle (for instance with dash)
+        * better cythonize the recognition
+        * optimized matching of several chronicles at the same time
+        
+        
+        # Requirements
+        
+        Use `pip install -r requirements.txt` to install requirements.
+        
+        Naturally, the latter may require superuser rights (consider prefixing the commands by sudo).
+        
+        If you want to use Python 3 and your system defaults on Python 2.7, you may need to adjust the above commands, e.g., replace pip by pip3.
+        
+        The required libraries are the following
+        * numpy
+        * scipy
+        * lazr.restfulclient
+        * larz.uri
+        * typing
+        * pandas
+        
+        LAZR is used to instantiate chronicles from CRS files (with simple grammar).
+        
+        # Usage
+        
+        Example of usage:
+        
+            from pychronicles import *
+            #define a sequence of events
+            seq = [3,4,'b','a','a',1,3,'coucou','b','coucou',5,'coucou',5]
+            
+            #define a chronicle
+            c=Chronicle()
+            c.add_event(0,'b')
+            c.add_event(1,1)
+            c.add_constraint(1,3, (3,45))
+            print(c)
+            
+            #recognize the chronicle in the sequence
+            occs=c.recognize(seq)
+            print("occurrences: "+str(occs))
+        
+        It is possible to specify chronicles using the CRS format. The following code illustrate the syntax for specifying a chronicle in this format.
+        
+            chronicle C27_sub_0[]()
+            {
+        	    event(Event_Type1[], t006)
+        	    event(Event_Type1[], t004)
+        	    event(Event_Type2[], t002)
+        	    event(Event_Type3[], t001)
+        
+        	    t004-t006 in [17,25]
+        	    t006-t002 in [-16,-10]
+        	    t002-t001 in [14,29]
+        	    t004-t001 in [27,35]
+            }
+        
+        
+        # Authorship
+        
+        * **Author:** Thomas Guyet
+        * **Institution:** Inria
+        * **date:** 8/2022
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# PyChronicle package
-
-A chronicle is a specification of the complex temporal behaviors as a graph of temporal constraints. More specifically, a chronicle is a multiset of events and a set of temporal constraints specifying that occurrences of pairs of events must occurs within a given temporal interval.
-It can be used to recognize complex behaviors in sequence the temporal events.
-
-This library proposes a Python class to define a chronicle, to read/save them in a standard CRS format. The main useful functionnality for chronicle is their efficient matching in a temporal sequence.
-
-A temporal sequence may have three different format:
-* a simple list of items (str, int or None) with implicit timestamps : `['a', 'b', ..., None, 'c', None, 'd']`
-* a list of explicitly timestamped items (str or int) : `[ (1,'a'), (23,'b'), (30,'c'), (45, 'd')]`
-* a pandas dataframe indexed by timestamps and using the items in a columns (named `label`)
-
-The chronicles handles to model of timestamps (for the last two types of sequence models):
-* discrete timestamps using integers
-* continuous timestamps using `datetime` format. In this case the temporal constraints of a chronicle must be defined using `timedelta` values.
-
-The package implements efficient algorithms to recognize it. It benefits from pandas functionalities to increase their efficiency. There are three different ways to _recognize_ a chronicle in a sequence of a events:
-* the absence/presence recognition (`c.match(seq)`): its result is a boolean stating whether the chronicle occur at least once in the sequence, this is the most efficient algorithm
-* the occurrence enumeration (`c.recognize(seq)`): its result is a list of occurrence of the chronicle in a sequence. Contrary to the first implementation, it looks for all possible combinasion of events. Thus it is less efficient
-* the approximate occurrence enumeration (`c.cmp(seq, 0.7)`): its result is a list of occurrences that are similar of the chronicle with a similarity threshold of 0.7.
-
-In addition, when using a pandas dataframe which contains several sequences (indexed with an attribute), it is possible to request for matching a chronicle in all sequences (no specific optimisation).
-
-
-Please note that the author is not fully satisfied by the function name and that it appeals to change them in a short delay ...
-
-# Perspectives
-
-* extend the chronicle model for pandas dataframe by specifying event by a couple (attribute, value), that can be used to specify a wider range of complex behavior in multidimensional sequences
-* graphical interfaces to edit chronicle (for instance with dash)
-* better cythonize the recognition
-* optimized matching of several chronicles at the same time
-
-
-# Requirements
-
-Use `pip install -r requirements.txt` to install requirements.
-
-Naturally, the latter may require superuser rights (consider prefixing the commands by sudo).
-
-If you want to use Python 3 and your system defaults on Python 2.7, you may need to adjust the above commands, e.g., replace pip by pip3.
-
-The required libraries are the following
-* numpy
-* scipy
-* lazr.restfulclient
-* larz.uri
-* typing
-* pandas
-
-LAZR is used to instantiate chronicles from CRS files (with simple grammar).
-
-# Usage
-
-Example of usage:
-
-    from pychronicles import *
-    #define a sequence of events
-    seq = [3,4,'b','a','a',1,3,'coucou','b','coucou',5,'coucou',5]
-    
-    #define a chronicle
-    c=Chronicle()
-    c.add_event(0,'b')
-    c.add_event(1,1)
-    c.add_constraint(1,3, (3,45))
-    print(c)
-    
-    #recognize the chronicle in the sequence
-    occs=c.recognize(seq)
-    print("occurrences: "+str(occs))
-
-It is possible to specify chronicles using the CRS format. The following code illustrate the syntax for specifying a chronicle in this format.
-
-    chronicle C27_sub_0[]()
-    {
-	    event(Event_Type1[], t006)
-	    event(Event_Type1[], t004)
-	    event(Event_Type2[], t002)
-	    event(Event_Type3[], t001)
-
-	    t004-t006 in [17,25]
-	    t006-t002 in [-16,-10]
-	    t002-t001 in [14,29]
-	    t004-t001 in [27,35]
-    }
-
-
-# Authorship
-
-* **Author:** Thomas Guyet
-* **Institution:** Inria
-* **date:** 8/2022
-
```

### Comparing `pychronicles-0.0.8/setup.py` & `pychronicles-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extensions = [
     Extension(
         "pychronicles.chronicle",
-        ["pychronicles/chronicle.pyx"],
+        ["pychronicles/chronicle.py"],
         include_dirs=[], # not needed for fftw unless it is installed in an unusual place
         libraries=[],
         library_dirs=[], # not needed for fftw unless it is installed in an unusual place
     ),
 ]
 
 setuptools.setup(
     name="pychronicles",
-    version="0.0.8",
+    version="0.0.9",
     author="Thomas Guyet",
     author_email="thomas.guyet@inria.fr",
     description="A package for chronicle recognition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.inria.fr/tguyet/pychronicles",
     install_requires=['pandas','numpy','scipy','lazr.restfulclient','lazr.uri','lark-parser'],
```

