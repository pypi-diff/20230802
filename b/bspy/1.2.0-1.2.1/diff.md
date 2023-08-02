# Comparing `tmp/bspy-1.2.0.tar.gz` & `tmp/bspy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bspy-1.2.0.tar", last modified: Mon Jul 31 05:12:22 2023, max compression
+gzip compressed data, was "bspy-1.2.1.tar", last modified: Wed Aug  2 15:07:21 2023, max compression
```

## Comparing `bspy-1.2.0.tar` & `bspy-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 05:12:22.442230 bspy-1.2.0/
--rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3684 2023-07-31 05:12:22.443232 bspy-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2569 2023-07-31 05:06:46.000000 bspy-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 05:12:22.385234 bspy-1.2.0/bspy/
--rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.2.0/bspy/__init__.py
--rw-rw-rw-   0        0        0    27826 2023-07-22 16:36:42.000000 bspy-1.2.0/bspy/_spline_domain.py
--rw-rw-rw-   0        0        0     6376 2023-07-30 05:37:58.000000 bspy-1.2.0/bspy/_spline_evaluation.py
--rw-rw-rw-   0        0        0    20552 2023-07-22 16:36:42.000000 bspy-1.2.0/bspy/_spline_fitting.py
--rw-rw-rw-   0        0        0    29293 2023-07-31 00:14:45.000000 bspy-1.2.0/bspy/_spline_intersection.py
--rw-rw-rw-   0        0        0    35722 2023-07-30 05:37:58.000000 bspy-1.2.0/bspy/_spline_operations.py
--rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.2.0/bspy/bspyApp.py
--rw-rw-rw-   0        0        0    17004 2023-07-22 16:36:42.000000 bspy-1.2.0/bspy/drawableSpline.py
--rw-rw-rw-   0        0        0    57454 2023-07-30 05:37:58.000000 bspy-1.2.0/bspy/spline.py
--rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.2.0/bspy/splineOpenGLFrame.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:12:22.432238 bspy-1.2.0/bspy.egg-info/
--rw-rw-rw-   0        0        0     3684 2023-07-31 05:12:22.000000 bspy-1.2.0/bspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-31 05:12:22.000000 bspy-1.2.0/bspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 05:12:22.000000 bspy-1.2.0/bspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-31 05:12:22.000000 bspy-1.2.0/bspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-31 05:12:22.000000 bspy-1.2.0/bspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-07-21 16:30:19.000000 bspy-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1169 2023-07-31 05:12:22.447235 bspy-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 05:12:22.437237 bspy-1.2.0/tests/
--rw-rw-rw-   0        0        0    72810 2023-07-31 00:17:29.000000 bspy-1.2.0/tests/test_bspy.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:07:21.483479 bspy-1.2.1/
+-rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3684 2023-08-02 15:07:21.484494 bspy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2569 2023-07-31 05:06:46.000000 bspy-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 15:07:21.424276 bspy-1.2.1/bspy/
+-rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.2.1/bspy/__init__.py
+-rw-rw-rw-   0        0        0    27826 2023-07-22 16:36:42.000000 bspy-1.2.1/bspy/_spline_domain.py
+-rw-rw-rw-   0        0        0     6376 2023-07-30 05:37:58.000000 bspy-1.2.1/bspy/_spline_evaluation.py
+-rw-rw-rw-   0        0        0    20552 2023-07-22 16:36:42.000000 bspy-1.2.1/bspy/_spline_fitting.py
+-rw-rw-rw-   0        0        0    30801 2023-08-02 14:57:12.000000 bspy-1.2.1/bspy/_spline_intersection.py
+-rw-rw-rw-   0        0        0    35722 2023-07-30 05:37:58.000000 bspy-1.2.1/bspy/_spline_operations.py
+-rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.2.1/bspy/bspyApp.py
+-rw-rw-rw-   0        0        0    17004 2023-07-22 16:36:42.000000 bspy-1.2.1/bspy/drawableSpline.py
+-rw-rw-rw-   0        0        0    57454 2023-07-30 05:37:58.000000 bspy-1.2.1/bspy/spline.py
+-rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.2.1/bspy/splineOpenGLFrame.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:07:21.476949 bspy-1.2.1/bspy.egg-info/
+-rw-rw-rw-   0        0        0     3684 2023-08-02 15:07:21.000000 bspy-1.2.1/bspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-08-02 15:07:21.000000 bspy-1.2.1/bspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:07:21.000000 bspy-1.2.1/bspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-02 15:07:21.000000 bspy-1.2.1/bspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-02 15:07:21.000000 bspy-1.2.1/bspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-07-21 16:30:19.000000 bspy-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1169 2023-08-02 15:07:21.487999 bspy-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 15:07:21.479472 bspy-1.2.1/tests/
+-rw-rw-rw-   0        0        0    73149 2023-08-02 15:02:56.000000 bspy-1.2.1/tests/test_bspy.py
```

### Comparing `bspy-1.2.0/LICENSE` & `bspy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/PKG-INFO` & `bspy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for manipulating and rendering non-uniform b-splines
 Home-page: http://github.com/ericbrec/bspy
 Author: Eric Brechner
 Author-email: ericbrec@msn.com
 License: MIT
 Project-URL: Bug Tracker, http://github.com/ericbrec/bspy/issues
 Keywords: opengl,bspline,b-spline,nub,tkinter
```

### Comparing `bspy-1.2.0/README.md` & `bspy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/__init__.py` & `bspy-1.2.1/bspy/__init__.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/_spline_domain.py` & `bspy-1.2.1/bspy/_spline_domain.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/_spline_evaluation.py` & `bspy-1.2.1/bspy/_spline_evaluation.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/_spline_fitting.py` & `bspy-1.2.1/bspy/_spline_fitting.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/_spline_intersection.py` & `bspy-1.2.1/bspy/_spline_intersection.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,86 +10,107 @@
     epsilon = np.finfo(self.coefs.dtype).eps
 
     # Set initial spline and domain
  
     spline = self
     (domain,) = spline.domain()
 
+    # Make sure this works for weird intervals of definition
+
+    if domain[0] != 0.0 or domain[1] != 1.0:
+        spline = spline.reparametrize([[0.0, 1.0]])
+        myZeros = spline.zeros()
+        fixedZeros = []
+        for thisZero in myZeros:
+            if type(thisZero) is type((1.0, 2.0),):
+                newLeft = (1.0 - thisZero[0]) * domain[0] + thisZero[0] * domain[1]
+                newRight = (1.0 - thisZero[1]) * domain[0] + thisZero[1] * domain[1]
+                fixedZeros += [(newLeft, newRight),]
+            else:
+                fixedZeros += [(1.0 - thisZero) * domain[0] + thisZero * domain[1]]
+        return fixedZeros
+
     # Perform an interval Newton step
 
-    def refine(spline, intervalSize, maxFunc):
-        (bbox,) = spline.range_bounds()
-        if bbox[0] * bbox[1] > epsilon:
+    def refine(spline, intervalSize, functionMax):
+        (boundingBox,) = spline.range_bounds()
+        if boundingBox[0] * boundingBox[1] > epsilon:
             return []
-        scalefactor = max(abs(bbox[0]), abs(bbox[1]))
-        scalespl = spline.scale(1.0 / scalefactor)
-        (mydomain,) = scalespl.domain()
-        intervalSize *= mydomain[1] - mydomain[0]
-        maxFunc *= scalefactor
-        myspline = scalespl.reparametrize([[0.0, 1.0]])
+        scaleFactor = max(abs(boundingBox[0]), abs(boundingBox[1]))
+        scaledSpline = spline.scale(1.0 / scaleFactor)
+        (myDomain,) = scaledSpline.domain()
+        intervalSize *= myDomain[1] - myDomain[0]
+        functionMax *= scaleFactor
+        mySpline = scaledSpline.reparametrize([[0.0, 1.0]])
         midPoint = 0.5
-        [fval] = myspline([midPoint])
+        [functionValue] = mySpline([midPoint])
 
         # Root found
 
-        if intervalSize < epsilon: # or abs(fval) * maxFunc < epsilon:
-            return [0.5 * (mydomain[0] + mydomain[1])]
-    
+        if intervalSize < epsilon or abs(functionValue) * functionMax < epsilon:
+            if intervalSize < epsilon ** 0.25:
+                return [0.5 * (myDomain[0] + myDomain[1])]
+            else:
+                myZeros = refine(mySpline.trim(((0.0, midPoint - np.sqrt(epsilon)),)), intervalSize, functionMax)
+                myZeros += [0.5 * (myDomain[0] + myDomain[1])]
+                myZeros += refine(mySpline.trim(((midPoint + np.sqrt(epsilon), 1.0),)), intervalSize, functionMax)
+                return myZeros
+
         # Calculate Newton update
 
-        (fder,) = myspline.differentiate().range_bounds()
-        if fder[0] == 0.0:
-            fder[0] = epsilon
-        if fder[1] == 0.0:
-            fder[1] = -epsilon
-        xleft = midPoint - fval / fder[0]
-        xright = midPoint - fval / fder[1]
-        dleft = min(xleft, xright) - 0.5 * epsilon
-        dright = max(xleft, xright) + 0.5 * epsilon
-        if fder[0] * fder[1] >= 0.0:    # Refine interval
-           xnewleft = max(0.0, dleft)
-           xnewright = min(1.0, dright)
-           if xnewleft <= xnewright:
-               trimspl = myspline.trim(((xnewleft, xnewright),))
-               myzeros = refine(trimspl, intervalSize, maxFunc)
+        (derivativeBounds,) = mySpline.differentiate().range_bounds()
+        if derivativeBounds[0] == 0.0:
+            derivativeBounds[0] = epsilon
+        if derivativeBounds[1] == 0.0:
+            derivativeBounds[1] = -epsilon
+        leftNewtonStep = midPoint - functionValue / derivativeBounds[0]
+        rightNewtonStep = midPoint - functionValue / derivativeBounds[1]
+        adjustedLeftStep = min(leftNewtonStep, rightNewtonStep) - 0.5 * epsilon
+        adjustedRightStep = max(leftNewtonStep, rightNewtonStep) + 0.5 * epsilon
+        if derivativeBounds[0] * derivativeBounds[1] >= 0.0:    # Refine interval
+           projectedLeftStep = max(0.0, adjustedLeftStep)
+           projectedRightStep = min(1.0, adjustedRightStep)
+           if projectedLeftStep <= projectedRightStep:
+               trimmedSpline = mySpline.trim(((projectedLeftStep, projectedRightStep),))
+               myZeros = refine(trimmedSpline, intervalSize, functionMax)
            else:
                return []
         else:                           # . . . or split as needed
-            myzeros = []
-            if dleft > 0.0:
-                trimspl = myspline.trim(((0.0, dleft),))
-                myzeros += refine(trimspl, intervalSize, maxFunc)
-            if dright < 1.0:
-                trimspl = myspline.trim(((dright, 1.0),))
-                myzeros += refine(trimspl, intervalSize, maxFunc)
-        return [(1.0 - thiszero) * mydomain[0] + thiszero * mydomain[1] for thiszero in myzeros]
+            myZeros = []
+            if adjustedLeftStep > 0.0:
+                trimmedSpline = mySpline.trim(((0.0, adjustedLeftStep),))
+                myZeros += refine(trimmedSpline, intervalSize, functionMax)
+            if adjustedRightStep < 1.0:
+                trimmedSpline = mySpline.trim(((adjustedRightStep, 1.0),))
+                myZeros += refine(trimmedSpline, intervalSize, functionMax)
+        return [(1.0 - thisZero) * myDomain[0] + thisZero * myDomain[1] for thisZero in myZeros]
 
     # See if there are any zero intervals
 
-    (bbox,) = spline.range_bounds()
-    scalefactor = max(abs(bbox[0]), abs(bbox[1]))
-    mysolution = []
+    (boundingBox,) = spline.range_bounds()
+    scaleFactor = max(abs(boundingBox[0]), abs(boundingBox[1]))
+    mySolution = []
     for interval in range(spline.nCoef[0] - spline.order[0] + 1):
-        maxFunc = max(np.abs(spline.coefs[0][interval:interval + spline.order[0]]))
-        if maxFunc < scalefactor * epsilon:     # Found an interval of zeros
-            intExtend = spline.nCoef[0] - spline.order[0] - interval
-            for ix in range(intExtend):         # Attempt to extend the interval to more than one polynomial piece
-                if abs(spline.coefs[0][interval + ix + spline.order[0]]) >= scalefactor * epsilon:
-                    intExtend = ix
+        functionMax = max(np.abs(spline.coefs[0][interval:interval + spline.order[0]]))
+        if functionMax < scaleFactor * epsilon: # Found an interval of zeros
+            intervalExtend = spline.nCoef[0] - spline.order[0] - interval
+            for ix in range(intervalExtend):    # Attempt to extend the interval to more than one polynomial piece
+                if abs(spline.coefs[0][interval + ix + spline.order[0]]) >= scaleFactor * epsilon:
+                    intervalExtend = ix
                     break
-            leftend = spline.knots[0][interval + spline.order[0] - 1]
-            rightend = spline.knots[0][interval + spline.order[0] + intExtend]
-            if domain[0] != leftend:            # Compute zeros from left of the interval
-                mysolution = refine(spline.trim(((domain[0], leftend - np.sqrt(epsilon)),)),
-                                    max (1.0, 1.0 / (leftend - domain[0])), 1.0)
-            mysolution += [(leftend, rightend)] # Add the interval of zeros
-            if rightend != domain[1]:           # Add the zeros from right of the interval
-                mysolution += spline.trim(((rightend + np.sqrt(epsilon), domain[1]),)).zeros()
-            return mysolution
-    return refine(spline, max (1.0, 1.0 / (domain[1] - domain[0])), 1.0)
+            leftEnd = spline.knots[0][interval + spline.order[0] - 1]
+            rightEnd = spline.knots[0][interval + spline.order[0] + intervalExtend]
+            if domain[0] != leftEnd:            # Compute zeros from left of the interval
+                mySolution = refine(spline.trim(((domain[0], leftEnd - np.sqrt(epsilon)),)),
+                                    max (1.0, 1.0 / (leftEnd - domain[0])), 1.0)
+            mySolution += [(leftEnd, rightEnd)] # Add the interval of zeros
+            if rightEnd != domain[1]:           # Add the zeros from right of the interval
+                mySolution += spline.trim(((rightEnd + np.sqrt(epsilon), domain[1]),)).zeros()
+            return mySolution
+    return refine(spline, 1.0, 1.0)
 
 def _convex_hull_2D(xData, yData, epsilon = 1.0e-8, evaluationEpsilon = 1.0e-4, xInterval = None):
     # Allow xData to be repeated for longer yData, but only if yData is a multiple.
     if not(len(yData) % len(xData) == 0): raise ValueError("Size of xData does not divide evenly in size of yData")
 
     # Assign p0 to the leftmost lowest point. Also compute xMin, xMax, and yMax.
     xMin = xMax = x0 = xData[0]
```

### Comparing `bspy-1.2.0/bspy/_spline_operations.py` & `bspy-1.2.1/bspy/_spline_operations.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/bspyApp.py` & `bspy-1.2.1/bspy/bspyApp.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/drawableSpline.py` & `bspy-1.2.1/bspy/drawableSpline.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/spline.py` & `bspy-1.2.1/bspy/spline.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy/splineOpenGLFrame.py` & `bspy-1.2.1/bspy/splineOpenGLFrame.py`

 * *Files identical despite different names*

### Comparing `bspy-1.2.0/bspy.egg-info/PKG-INFO` & `bspy-1.2.1/bspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for manipulating and rendering non-uniform b-splines
 Home-page: http://github.com/ericbrec/bspy
 Author: Eric Brechner
 Author-email: ericbrec@msn.com
 License: MIT
 Project-URL: Bug Tracker, http://github.com/ericbrec/bspy/issues
 Keywords: opengl,bspline,b-spline,nub,tkinter
```

### Comparing `bspy-1.2.0/setup.cfg` & `bspy-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7370 790d 0a76 6572 7369 6f6e   = bspy..version
-00000020: 203d 2031 2e32 2e30 0d0a 6175 7468 6f72   = 1.2.0..author
+00000020: 203d 2031 2e32 2e31 0d0a 6175 7468 6f72   = 1.2.1..author
 00000030: 203d 2045 7269 6320 4272 6563 686e 6572   = Eric Brechner
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2065 7269 6362 7265 6340 6d73 6e2e 636f   ericbrec@msn.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 204c 6962 7261 7279 2066 6f72 206d 616e   Library for man
 00000080: 6970 756c 6174 696e 6720 616e 6420 7265  ipulating and re
 00000090: 6e64 6572 696e 6720 6e6f 6e2d 756e 6966  ndering non-unif
```

### Comparing `bspy-1.2.0/tests/test_bspy.py` & `bspy-1.2.1/tests/test_bspy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1088,15 +1088,15 @@
     expectedRoots = (0.19780681921299614, 0.959258605483323, 2.3682761525810267, 3.3362282254078597)
     roots = spline.zeros()
     check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (4,), ((0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0),), ((1.0, -13.0 / 9.0, 25.0 / 12.0, -3.0),))
     expectedRoots = (0.39999999558761995, 0.4285714285714262)
     roots = spline.zeros()
-    #check_1D_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (6,), ((0.0, 0.0, 0.0, 0.0, 0.3, 0.7, 1.0, 1.0, 1.0, 1.0),), ((1.3, 0, 0, 0, 0, -2.6),))
     expectedRoots = ((0.3, 0.7),)
     roots = spline.zeros()
     check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (6,), ((0.0, 0.0, 0.0, 0.0, 0.3, 0.7, 1.0, 1.0, 1.0, 1.0),), ((0, 0, 0, 0, 0, -2.6),))
@@ -1105,14 +1105,19 @@
     check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (11,), ((0.0, 0.0, 0.0, 0.0, 0.1, 0.2, 0.3, 0.5, 0.6, 0.7, 0.8, 1.0, 1.0, 1.0, 1.0),), ((4, 0, 0, 0, 0, -2.6, 0, 0, 0, 0, 0),))
     expectedRoots = ((0.1, 0.2), (0.7, 1.0))
     roots = spline.zeros()
     check_1D_roots(expectedRoots, roots, tolerance)
 
+    spline = bspy.Spline(1, 1, (4,), (7,), ((0.0, 0.0, 0.0, 0.0, 0.25, 0.5, 0.75, 1.0, 1.0, 1.0, 1.0),), ((1.0, -2.0, 2.0, 0.0, -2.0, 2.0, -1.0),))
+    expectedRoots = (0.03580961131802156, 0.1861089501087097, 0.5, 0.8138910498912902, 0.9641903886819785)
+    roots = spline.zeros()
+    check_1D_roots(expectedRoots, roots, tolerance)
+
     data = []
     for u in np.linspace(-2.0, 2.0, 3):
         for v in np.linspace(-2.0, 2.0, 7):
             data.append((u, v, 9 * u * u + v * v - 1.0, u - v))
     spline = bspy.Spline.least_squares(2, 2, (3,3), data)
     roots = spline.zeros(tolerance)
     check_roots(spline, 2, roots, tolerance)
```

