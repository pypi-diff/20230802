# Comparing `tmp/optionlab-0.1-py3-none-any.whl.zip` & `tmp/optionlab-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 16686 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx       97 b- defN 23-Jun-27 21:46 optionlab/__init__.py
--rwxrwxrwx  2.0 unx     7302 b- defN 23-May-25 21:16 optionlab/black_scholes.py
--rwxrwxrwx  2.0 unx    61299 b- defN 23-Jun-30 00:07 optionlab/strategy.py
--rwxrwxrwx  2.0 unx    16045 b- defN 23-Jun-28 13:24 optionlab/support.py
--rwxrwxrwx  2.0 unx     2485 b- defN 23-Jul-07 21:24 optionlab-0.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-07 21:24 optionlab-0.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-07 21:24 optionlab-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      614 b- defN 23-Jul-07 21:24 optionlab-0.1.dist-info/RECORD
-8 files, 87944 bytes uncompressed, 15624 bytes compressed:  82.2%
+Zip file size: 37333 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   121378 b- defN 23-Aug-01 19:26 optionlab/__holidays__.py
+-rw-rw-rw-  2.0 fat      127 b- defN 23-Aug-01 22:03 optionlab/__init__.py
+-rw-rw-rw-  2.0 fat     7302 b- defN 23-May-25 21:16 optionlab/black_scholes.py
+-rw-rw-rw-  2.0 fat    61299 b- defN 23-Jun-30 00:07 optionlab/strategy.py
+-rw-rw-rw-  2.0 fat    15809 b- defN 23-Aug-01 21:37 optionlab/support.py
+-rw-rw-rw-  2.0 fat     2487 b- defN 23-Aug-01 22:07 optionlab-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Aug-01 22:07 optionlab-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-01 22:07 optionlab-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      707 b- defN 23-Aug-01 22:07 optionlab-0.1.1.dist-info/RECORD
+9 files, 209216 bytes uncompressed, 36129 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
+Filename: optionlab/__holidays__.py
+Comment: 
+
 Filename: optionlab/__init__.py
 Comment: 
 
 Filename: optionlab/black_scholes.py
 Comment: 
 
 Filename: optionlab/strategy.py
 Comment: 
 
 Filename: optionlab/support.py
 Comment: 
 
-Filename: optionlab-0.1.dist-info/METADATA
+Filename: optionlab-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: optionlab-0.1.dist-info/WHEEL
+Filename: optionlab-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: optionlab-0.1.dist-info/top_level.txt
+Filename: optionlab-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: optionlab-0.1.dist-info/RECORD
+Filename: optionlab-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## optionlab/__init__.py

```diff
@@ -1,5 +1,6 @@
+from . import __holidays__
 from . import black_scholes
 from . import support
 from . import strategy
 
-__version__="0.1"
+__version__="0.1.1"
```

## optionlab/support.py

```diff
@@ -1,19 +1,14 @@
 from __future__ import division
 from scipy import stats
 from numpy import array,asarray,ndarray,exp,abs,round,diff,flatnonzero,arange,inf
 from numpy.random import normal,laplace
 from numpy.lib.scimath import log,sqrt
 from datetime import date,timedelta
-from sys import modules
-
-try:
-    import holidays
-except ModuleNotFoundError:
-    print("WARNING! Install the 'holidays' package to count holidays as non-business days!")
+from optionlab.__holidays__ import getholidays
 
 def getpayoff(optype,s,x):
     '''
     getpayoff(optype,s,x) -> returns the payoff of an option trade at expiration.
     
     Arguments:
     ----------    
@@ -194,23 +189,21 @@
     
     if enddate>startdate:
         ndays=(enddate-startdate).days
     else:
         raise ValueError("End date must be after start date!")
     
     nonbusinessdays=0
+    holidays=getholidays(country)
     
     for i in range(ndays):
         currdate=startdate+timedelta(days=i)
         
-        if currdate.weekday()>=5:
+        if currdate.weekday()>=5 or currdate.strftime("%Y-%m-%d") in holidays:
             nonbusinessdays+=1
-        elif "holidays" in modules:                      
-            if holidays.country_holidays(country).get(currdate.strftime("%Y-%m-%d")) is not None:
-                nonbusinessdays+=1
             
     return nonbusinessdays
 
 def createpriceseq(minprice,maxprice):
     '''
     createpriceseq(minprice,maxprice) -> generates a sequence of stock prices 
     from 'minprice' to 'maxprice' with increment $0.01.
```

## Comparing `optionlab-0.1.dist-info/METADATA` & `optionlab-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optionlab
-Version: 0.1
+Version: 0.1.1
 Summary: A Python library for evaluating option trading strategies.
 Home-page: https://github.com/rgaveiga/optionlab
 Author: Roberto Gomes de Aguiar Veiga
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `optionlab-0.1.dist-info/RECORD` & `optionlab-0.1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-optionlab/__init__.py,sha256=GIQJ_gEOtwA6d9ytZdPsVcxk56agny23KnLMAD1k7Rs,97
+optionlab/__holidays__.py,sha256=dbIE5VEpTBwbyM3lPCqFWp-bQAudrRiXqILMClBwkBc,121378
+optionlab/__init__.py,sha256=kDtk1ueeMJ20wPfI3U-fLtWDQQ1Q89uZoauUEv-9qeI,127
 optionlab/black_scholes.py,sha256=MvW5aAx192ghgstfWgsPAWZlp_NO-aa9ZPNIkOAWfkw,7302
 optionlab/strategy.py,sha256=E9fpsx_W4CpYYiDzq0HYAKE3_UglzvKhb34EG5J8_Go,61299
-optionlab/support.py,sha256=C-uIC6kDFaN6dc9oCPqm92yMNQg1isGCA65FrZBnGnA,16045
-optionlab-0.1.dist-info/METADATA,sha256=anxOgioi-4CKFJ4prKnfZwfZqrnZ2mWov76pakSJDgA,2485
-optionlab-0.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-optionlab-0.1.dist-info/top_level.txt,sha256=xORpnhGShXTTyokeOb01hHM4tqiVlu_6cR_jr85SJz8,10
-optionlab-0.1.dist-info/RECORD,,
+optionlab/support.py,sha256=Mrv6o573iYPCuKSfCARApgXzZGfII5EwgHVGQaK2VN8,15809
+optionlab-0.1.1.dist-info/METADATA,sha256=58P8MOz6aQFOXfKntPk6ZDDzm3sCsJK7-1DQfDysznc,2487
+optionlab-0.1.1.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+optionlab-0.1.1.dist-info/top_level.txt,sha256=xORpnhGShXTTyokeOb01hHM4tqiVlu_6cR_jr85SJz8,10
+optionlab-0.1.1.dist-info/RECORD,,
```

