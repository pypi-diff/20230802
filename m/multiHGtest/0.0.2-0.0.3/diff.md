# Comparing `tmp/multiHGtest-0.0.2.tar.gz` & `tmp/multiHGtest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kipnisal/HGpvals_package/dist/.tmp-br_bn067/multiHGtest-0.0.2.tar", last modified: Wed Mar 22 13:13:09 2023, max compression
+gzip compressed data, was "multiHGtest-0.0.3.tar", last modified: Wed Aug  2 10:26:14 2023, max compression
```

## Comparing `multiHGtest-0.0.2.tar` & `multiHGtest-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-03-22 13:13:09.215044 multiHGtest-0.0.2/
--rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2022-02-20 07:18:17.000000 multiHGtest-0.0.2/LICENSE
--rw-r--r--   0 kipnisal   (503) staff       (20)      887 2023-03-22 13:13:09.215175 multiHGtest-0.0.2/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)      341 2023-03-15 07:50:36.000000 multiHGtest-0.0.2/README.md
--rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-03-15 07:51:05.000000 multiHGtest-0.0.2/pyproject.toml
--rw-r--r--   0 kipnisal   (503) staff       (20)      749 2023-03-22 13:13:09.215759 multiHGtest-0.0.2/setup.cfg
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-03-22 13:13:09.209549 multiHGtest-0.0.2/src/
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-03-22 13:13:09.210880 multiHGtest-0.0.2/src/multiHGtest/
--rw-r--r--   0 kipnisal   (503) staff       (20)       82 2023-03-22 12:05:06.000000 multiHGtest-0.0.2/src/multiHGtest/__init__.py
--rw-r--r--   0 kipnisal   (503) staff       (20)     5894 2023-03-22 13:09:17.000000 multiHGtest-0.0.2/src/multiHGtest/multiHGtest.py
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-03-22 13:13:09.211728 multiHGtest-0.0.2/src/multiHGtest.egg-info/
--rw-r--r--   0 kipnisal   (503) staff       (20)      887 2023-03-22 13:13:09.000000 multiHGtest-0.0.2/src/multiHGtest.egg-info/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)      321 2023-03-22 13:13:09.000000 multiHGtest-0.0.2/src/multiHGtest.egg-info/SOURCES.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)        1 2023-03-22 13:13:09.000000 multiHGtest-0.0.2/src/multiHGtest.egg-info/dependency_links.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       39 2023-03-22 13:13:09.000000 multiHGtest-0.0.2/src/multiHGtest.egg-info/requires.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       12 2023-03-22 13:13:09.000000 multiHGtest-0.0.2/src/multiHGtest.egg-info/top_level.txt
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-03-22 13:13:09.212850 multiHGtest-0.0.2/tests/
--rw-r--r--   0 kipnisal   (503) staff       (20)     3661 2023-03-22 12:40:10.000000 multiHGtest-0.0.2/tests/test_multiHGtest.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.124726 multiHGtest-0.0.3/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2022-02-20 07:18:17.000000 multiHGtest-0.0.3/LICENSE
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1134 2023-08-02 10:26:14.124782 multiHGtest-0.0.3/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)      588 2023-08-02 10:16:59.000000 multiHGtest-0.0.3/README.md
+-rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-03-15 07:51:05.000000 multiHGtest-0.0.3/pyproject.toml
+-rw-r--r--   0 kipnisal   (503) staff       (20)      749 2023-08-02 10:26:14.125042 multiHGtest-0.0.3/setup.cfg
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.122543 multiHGtest-0.0.3/src/
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.123739 multiHGtest-0.0.3/src/multiHGtest/
+-rw-r--r--   0 kipnisal   (503) staff       (20)       82 2023-03-22 12:05:06.000000 multiHGtest-0.0.3/src/multiHGtest/__init__.py
+-rw-r--r--   0 kipnisal   (503) staff       (20)     6087 2023-08-02 10:24:06.000000 multiHGtest-0.0.3/src/multiHGtest/multiHGtest.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.124409 multiHGtest-0.0.3/src/multiHGtest.egg-info/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1134 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)      321 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/SOURCES.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)        1 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/dependency_links.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       39 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/requires.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       12 2023-08-02 10:26:14.000000 multiHGtest-0.0.3/src/multiHGtest.egg-info/top_level.txt
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-08-02 10:26:14.124542 multiHGtest-0.0.3/tests/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     3661 2023-03-22 12:40:10.000000 multiHGtest-0.0.3/tests/test_multiHGtest.py
```

### Comparing `multiHGtest-0.0.2/LICENSE` & `multiHGtest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multiHGtest-0.0.2/PKG-INFO` & `multiHGtest-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: multiHGtest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Testing for differences in survival using hypergeometric P-values
 Home-page: https://github.com/alonkipnis/higher-criticism-test
 Download-URL: https://github.com/alonkipnis/higher-criticism-test
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# multiHGtest -- Testing for differences in survival using multiple hypergeometric P-values. Based on the tests described in 
+# multiHGtest -- Testing for differences in survival using multiple hypergeometric P-values. 
+
+This packages implements the test for survival data described in 
 [1] Galili, Kipnis and Yakini. Survival analysis with sensitivity to possible rare and weak differences. 2023. 
-[2] Kipnis and Yakhini. Dominating the log-rank test with multiple exact hypergeometric tests. 2023. 
+
+
+## Methods
+``hypergeom_test``      Exact hypergeometric test
+``HCHGtest``            Use higher criticism of hypergeometric P-values to test the significant 
+``FisherHGtest``        Fisher combination test of hypergeometric P-values
+``testHG_dashboard``    Illustrates statistics associated with the HG P-values
```

### Comparing `multiHGtest-0.0.2/setup.cfg` & `multiHGtest-0.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multiHGtest
-version = 0.0.02
+version = 0.0.03
 author = Alon Kipnis
 author_email = alonkipnis@gmail.com
 description = Testing for differences in survival using hypergeometric P-values
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alonkipnis/higher-criticism-test
 download_url = https://github.com/alonkipnis/higher-criticism-test
```

### Comparing `multiHGtest-0.0.2/src/multiHGtest/multiHGtest.py` & `multiHGtest-0.0.3/src/multiHGtest/multiHGtest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from scipy.stats import hypergeom, uniform
 from multitest import MultiTest
+import pandas as pd
 
 
 def hypergeom_test(k, M, n, N, alternative='two-sided', randomize=False):
     """
     Exact hypergeometric test
 
     Args:
@@ -68,15 +69,15 @@
     alternative = kwargs.get('alternative', 'two-sided')
 
     pvals = hypergeom_test(Ot2, Nt2 + Nt1, Nt2, Ot1 + Ot2,
                            randomize=randomize, alternative=alternative)
     return MultiTest(pvals)
 
 
-def HCHGtest(Nt1: np.ndarray, Nt2: np.ndarray, Ot1=[], Ot2=[], **kwargs):
+def HCHGtest(Nt1: np.ndarray, Nt2: np.ndarray, Ot1=None, Ot2=None, **kwargs):
     """
     higher criticism test of hypergeometric P-values for comparing survival data as
     described in: [1] Galili, Kipnis, Yakhini. 2023. Survival Analysis with Sensitivity to Rare and Weak Temporal
     Differences.
 
     Args:
         Nt1:  number of at-risk subjects in group 1 per time
@@ -88,18 +89,18 @@
         **kwargs:
 
     Returns:
         HC test statistic
 
     """
 
-    if Ot1 == []:
+    if Ot1 is None:
         Ot1 = -Nt1.diff()
         Nt1 = Nt1[:-1]
-    if Ot2 == []:
+    if Ot2 is None:
         Ot2 = -Nt2.diff()
         Nt2 = Nt2[:-1]
 
     mtest = _MultiTest(Nt1, Nt2, Ot1, Ot2, **kwargs)
     gamma = kwargs.get('gamma', 0.2)
     return mtest.hc(gamma)[0]
 
@@ -147,15 +148,14 @@
         **kwargs:
 
     Returns:
         test statistic
         P-value of corresponding chi-squared test
 
     """
-    import pandas as pd
 
     if Ot1 == []:
         Ot1 = -Nt1.diff()
         Nt1 = Nt1[:-1]
     if Ot2 == []:
         Ot2 = -Nt2.diff()
         Nt2 = Nt2[:-1]
@@ -166,17 +166,22 @@
 
     df = pd.DataFrame()
     df['at-risk1'] = Nt1
     df['at-risk2'] = Nt2
     df['events1'] = Ot1
     df['events2'] = Ot2
 
+    df['at-risk1'] = df['at-risk1'].astype(int)
+    df['at-risk2'] = df['at-risk2'].astype(int)
+    df['events1'] = df['events1'].astype(int)
+    df['events2'] = df['events2'].astype(int)
+
     randomize = kwargs.get('randomize', False)
     alternative = kwargs.get('alternative', 'two-sided')
-    gamma = kwargs.get('gamma', 0.2)
+    gamma = kwargs.get('gamma', 0.4)
     pvals = hypergeom_test(Ot2, Nt2 + Nt1, Nt2, Ot1 + Ot2,
                            randomize=randomize, alternative=alternative)
     df['pvalue'] = pvals
 
     stbl = kwargs.get('stbl', True)
     mtest = MultiTest(pvals, stbl=stbl)
```

### Comparing `multiHGtest-0.0.2/src/multiHGtest.egg-info/PKG-INFO` & `multiHGtest-0.0.3/src/multiHGtest.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: multiHGtest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Testing for differences in survival using hypergeometric P-values
 Home-page: https://github.com/alonkipnis/higher-criticism-test
 Download-URL: https://github.com/alonkipnis/higher-criticism-test
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# multiHGtest -- Testing for differences in survival using multiple hypergeometric P-values. Based on the tests described in 
+# multiHGtest -- Testing for differences in survival using multiple hypergeometric P-values. 
+
+This packages implements the test for survival data described in 
 [1] Galili, Kipnis and Yakini. Survival analysis with sensitivity to possible rare and weak differences. 2023. 
-[2] Kipnis and Yakhini. Dominating the log-rank test with multiple exact hypergeometric tests. 2023. 
+
+
+## Methods
+``hypergeom_test``      Exact hypergeometric test
+``HCHGtest``            Use higher criticism of hypergeometric P-values to test the significant 
+``FisherHGtest``        Fisher combination test of hypergeometric P-values
+``testHG_dashboard``    Illustrates statistics associated with the HG P-values
```

### Comparing `multiHGtest-0.0.2/tests/test_multiHGtest.py` & `multiHGtest-0.0.3/tests/test_multiHGtest.py`

 * *Files identical despite different names*

