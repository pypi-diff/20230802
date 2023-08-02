# Comparing `tmp/hysteresis-2.0.0.tar.gz` & `tmp/hysteresis-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hysteresis-2.0.0.tar", last modified: Sat Jun  3 23:07:41 2023, max compression
+gzip compressed data, was "hysteresis-2.0.1.tar", last modified: Wed Aug  2 07:59:49 2023, max compression
```

## Comparing `hysteresis-2.0.0.tar` & `hysteresis-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.111264 hysteresis-2.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.077264 hysteresis-2.0.0/Hysteresis/
--rw-rw-rw-   0        0        0      393 2023-05-29 06:58:48.000000 hysteresis-2.0.0/Hysteresis/__init__.py
--rw-rw-rw-   0        0        0     5762 2023-05-29 06:59:11.000000 hysteresis-2.0.0/Hysteresis/baseFuncs.py
--rw-rw-rw-   0        0        0     4128 2023-05-29 06:57:38.000000 hysteresis-2.0.0/Hysteresis/climate.py
--rw-rw-rw-   0        0        0     2727 2023-05-29 06:57:27.000000 hysteresis-2.0.0/Hysteresis/compare.py
--rw-rw-rw-   0        0        0    42368 2023-06-03 22:27:08.000000 hysteresis-2.0.0/Hysteresis/curve.py
--rw-rw-rw-   0        0        0    13244 2023-05-29 05:23:43.000000 hysteresis-2.0.0/Hysteresis/data.py
--rw-rw-rw-   0        0        0     4542 2023-05-28 01:22:30.000000 hysteresis-2.0.0/Hysteresis/defaultDataFuncs.py
--rw-rw-rw-   0        0        0     4879 2023-05-29 05:00:45.000000 hysteresis-2.0.0/Hysteresis/defaultPlotFuncs.py
--rw-rw-rw-   0        0        0     1133 2023-05-25 07:01:28.000000 hysteresis-2.0.0/Hysteresis/env.py
--rw-rw-rw-   0        0        0    11795 2023-05-29 07:00:47.000000 hysteresis-2.0.0/Hysteresis/envelope.py
-drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.109262 hysteresis-2.0.0/Hysteresis/plotSpecial/
--rw-rw-rw-   0        0        0       75 2022-10-30 07:42:02.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/__init__.py
--rw-rw-rw-   0        0        0    12531 2023-06-03 21:17:34.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/animate.py
--rw-rw-rw-   0        0        0    14981 2023-05-29 07:14:01.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/core.py
--rw-rw-rw-   0        0        0     5584 2022-10-30 07:42:02.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/guiPlot.py
--rw-rw-rw-   0        0        0     7017 2023-05-29 07:00:30.000000 hysteresis-2.0.0/Hysteresis/protocol.py
--rw-rw-rw-   0        0        0    12094 2023-05-29 07:00:04.000000 hysteresis-2.0.0/Hysteresis/resample.py
-drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.083302 hysteresis-2.0.0/Hysteresis.egg-info/
--rw-rw-rw-   0        0        0     6075 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      943 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6075 2023-06-03 23:07:41.111264 hysteresis-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5609 2022-04-04 00:12:03.000000 hysteresis-2.0.0/README.md
--rw-rw-rw-   0        0        0     1096 2020-05-27 03:09:59.000000 hysteresis-2.0.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 23:07:41.111264 hysteresis-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-06-03 23:06:34.000000 hysteresis-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:59:49.444138 hysteresis-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:59:49.403165 hysteresis-2.0.1/Hysteresis/
+-rw-rw-rw-   0        0        0      393 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/__init__.py
+-rw-rw-rw-   0        0        0     5762 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/baseFuncs.py
+-rw-rw-rw-   0        0        0     4128 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/climate.py
+-rw-rw-rw-   0        0        0     2727 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/compare.py
+-rw-rw-rw-   0        0        0    41884 2023-07-09 04:16:44.000000 hysteresis-2.0.1/Hysteresis/curve.py
+-rw-rw-rw-   0        0        0    13244 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/data.py
+-rw-rw-rw-   0        0        0     4542 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/defaultDataFuncs.py
+-rw-rw-rw-   0        0        0     4879 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/defaultPlotFuncs.py
+-rw-rw-rw-   0        0        0     1133 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/env.py
+-rw-rw-rw-   0        0        0    12472 2023-07-23 21:42:22.000000 hysteresis-2.0.1/Hysteresis/envelope.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:59:49.442201 hysteresis-2.0.1/Hysteresis/plotSpecial/
+-rw-rw-rw-   0        0        0       75 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/plotSpecial/__init__.py
+-rw-rw-rw-   0        0        0    12531 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/plotSpecial/animate.py
+-rw-rw-rw-   0        0        0    14981 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/plotSpecial/core.py
+-rw-rw-rw-   0        0        0     5584 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/plotSpecial/guiPlot.py
+-rw-rw-rw-   0        0        0     7017 2023-06-03 23:08:56.000000 hysteresis-2.0.1/Hysteresis/protocol.py
+-rw-rw-rw-   0        0        0    12800 2023-07-09 04:44:59.000000 hysteresis-2.0.1/Hysteresis/resample.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:59:49.410165 hysteresis-2.0.1/Hysteresis.egg-info/
+-rw-rw-rw-   0        0        0     6075 2023-08-02 07:59:48.000000 hysteresis-2.0.1/Hysteresis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-08-02 07:59:49.000000 hysteresis-2.0.1/Hysteresis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:59:48.000000 hysteresis-2.0.1/Hysteresis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-02 07:59:48.000000 hysteresis-2.0.1/Hysteresis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 07:59:48.000000 hysteresis-2.0.1/Hysteresis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6075 2023-08-02 07:59:49.443138 hysteresis-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5609 2022-04-04 00:12:03.000000 hysteresis-2.0.1/README.md
+-rw-rw-rw-   0        0        0     1096 2020-05-27 03:09:59.000000 hysteresis-2.0.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:59:49.444642 hysteresis-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-08-02 07:58:55.000000 hysteresis-2.0.1/setup.py
```

### Comparing `hysteresis-2.0.0/Hysteresis/baseFuncs.py` & `hysteresis-2.0.1/Hysteresis/baseFuncs.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/climate.py` & `hysteresis-2.0.1/Hysteresis/climate.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/compare.py` & `hysteresis-2.0.1/Hysteresis/compare.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/curve.py` & `hysteresis-2.0.1/Hysteresis/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1048,25 +1048,14 @@
         xyMono = self.xy
         
         if not colorCycles:
             colorCycles = self.colorCycles
         
         self.showCycles(xyMono, showReversals, showPeaks, self.peakIndexes, 
                         self.reversalIndexes, None, subCyclesIndexes)
- 
-        # lines = []
-        # # If the list has content, get the cycles to plot, otherwise plot everything
-        # if subCyclesIndexes is not  None:
-        #     vectors = [self.subCycles[ii] for ii in subCyclesIndexes]
-        
-        # for ii, vector in enumerate(vectors):
-        #     c = colorCycles[int(ii % Ncolor)]
-        #     line, = plt.plot(vector.xy[:,0], vector.xy[:,1], c=c, **kwargs)
-        #     lines.append(line)        
-        # return lines
     
         return self._plot_curves(self.subCycles, subCyclesIndexes, colorCycles, **kwargs)
     
     
         
     def recalculatePeaks(self, peakDist = 2, peakWidth = None, peakProminence = None):
         """
```

### Comparing `hysteresis-2.0.0/Hysteresis/data.py` & `hysteresis-2.0.1/Hysteresis/data.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/defaultDataFuncs.py` & `hysteresis-2.0.1/Hysteresis/defaultDataFuncs.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/defaultPlotFuncs.py` & `hysteresis-2.0.1/Hysteresis/defaultPlotFuncs.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/env.py` & `hysteresis-2.0.1/Hysteresis/env.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/envelope.py` & `hysteresis-2.0.1/Hysteresis/envelope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import numpy as np
-from numpy import trapz
-# import matplotlib.pyplot as plt
-
 from scipy.interpolate import interp1d
 from hysteresis import data
-
 from .data import linearInterpolation
 from .curve import Hysteresis, SimpleCurve
-from .defaultDataFuncs import defaultAreaFunction, defaultSlopeFunction
-from .defaultPlotFuncs import initializeFig, defaultPlotFunction, defaultShowCycles
+from .baseFuncs import concatenate
 
 
 
  
 # =============================================================================
 # Find the backbone
 # =============================================================================
 
 def _LPparser(LPsteps):
     
     # InputParser - Decides what to do with the variable LoadProtcol
     # if you get an interger use that for all cycles
     
     if len(LPsteps) ==0:
-        Indexes =  []
+        Indexes = []
     
     # if type(LPsteps) == int:
     else:
         # shift = LPsteps[0] - 1
         shift = 1
         Indexes = np.concatenate([[0,1], np.cumsum(LPsteps,dtype=int) + shift])
         
     return Indexes
 
 
-def _getBackbonePeaks(hystersis, xyPosInd):
+def _getBackbonePeaks(hysteresis, xyPosInd):
     
     Ncycle = len(xyPosInd)
     
     CycleIndx = xyPosInd[1:] - 1
     
-    cycles = hystersis.getCycles(CycleIndx)
+    cycles = hysteresis.getCycles(CycleIndx)
     peaks = np.zeros([Ncycle,2])
     for ii in range(Ncycle - 1):
         # Set the peak, then find the local index of the maximum point
         cycles[ii].setPeaks()
         tempInd = cycles[ii].maxIndexes
         
         # Get the xy coords, the aliase over the peak indexes.
@@ -69,22 +64,28 @@
     return xyPosInd[startIndex:endIndex]
     
     
 """
 TODO:
     Allow for getting the peaks, end point, or both.
 """
-def getBackboneCurve(hysteresis, LPsteps = [], returnPeaks = False,  returnEnd = True, 
-                     skipStart = 0, skipEnd =0):
+def getBackboneCurve(hysteresis, LPsteps = None, returnPeaks = False,  returnEnd = True, 
+                     skipStart = 0, skipEnd =0, includeNegative = False):
     """
     Returns the positve backbone curve of a hysteresis.
         
     By default all reversal points on the backbone curve are returned.
-    This will not be appropriate for some types of hysteresis where the load
-    drops between cycles.
+    The reversal points will be the **end** points of each cycle, but for some 
+    hystereses we will need to include peak points to capture the full backbone
+    To capture theses peak value, we can set the "returnPeaks" flag to be true.
+    
+    The function will only include the positive backbone by default, however,
+    the negative values can be returned using the 
+    
+    
     The user can output only the first cycle of each load step by specifying 
     the number of loading cycles there are at each load step.
     By default the final point (the right most point) is returned for each
     cycle.
     The user can return the peak and final point by setting returnPeaks = True.
 
 
@@ -109,14 +110,18 @@
         the end points of each cycle.         
     skipStart : int, optional
         The number of cycles to skip from the start of the the backbone 
         curve. The default is 0 which skips no cycles.
     skipEnd : int, optional
         The number of cycles to skip from the end of the the backbone 
         curve. The default is 0 which skips no cycles.
+    includeNegative : bool, optional
+        A boolean that will make the function return a negative backbone as 
+        well once toggled true.
+        
     Returns
     -------
     backbone : SimpleCycle
         A simpleCycle object of the output backbone curve.
 
     """
     
@@ -125,25 +130,26 @@
     
     _checkBBinput(returnPeaks, returnEnd)    
     
     # Get a slice of the reversal indexes
     reversalIndexes = hysteresis.reversalIndexes
     xyPoints = hysteresis.xy[reversalIndexes]
     
+    # Seperate out positive cycles
     diff = np.diff(xyPoints[:,0])
     xyPosInd = np.where(0 <= diff)[0] + 1
     xyPosInd = np.concatenate([[0], xyPosInd])
 
     # If it doesn't start at zero for some reason, make it start at zero.
     # We should always include the first index!
     if xyPosInd[0] != 0:
         xyPosInd = np.hstack((0,xyPosInd))
         
     # get the indexes of the final cycle
-    if len(LPsteps) != 0:
+    if LPsteps != None: # If no value is provided
         Indexes = _LPparser(LPsteps)
         xyPosInd = xyPosInd[Indexes]
         
     Ncycle = len(xyPosInd)
        
     # skip the start/end cycles    
     xyPosInd = _skipCycles(xyPosInd, skipStart, skipEnd, Ncycle)
@@ -154,14 +160,21 @@
         xyPos = np.concatenate([xyPos, xyPosCycleEnd])
     
     # Get the postive indexes        
     if returnPeaks == True:
         xyPosPeak = _getBackbonePeaks(hysteresis, xyPosInd)
         xyPos = np.concatenate([xyPos, xyPosPeak])
     
+       
+    # Include the negative curve using some recursion magic
+    if includeNegative:
+        curve = getBackboneCurve(Hysteresis(-hysteresis.xy), LPsteps, returnPeaks,  
+                         returnEnd, skipStart, skipEnd, False)
+        xyNeg = -curve.xy[::-1]
+        xyPos = np.concatenate((xyNeg, xyPos)) 
         
     # Remove repeated points
     xPos = xyPos[:,0]
     _, indexes = np.unique(xPos,True)
     xyPos = xyPos[indexes]   
     
     return SimpleCurve(xyPos, True)
@@ -184,15 +197,15 @@
     
     xy = np.column_stack([x, yavg])
     backBoneAvg = SimpleCurve(xy, True)
     
     return backBoneAvg
 
 
-def getAvgBackbone(hystersis, LPsteps = [], returnPeaks = False,  returnEnd = False,
+def getAvgBackbone(hysteresis, LPsteps = [], returnPeaks = False, returnEnd = True,
                    skipStart = 0, skipEnd =0):
     
     """
     Returns the average, positve, and negative backbone curve of a hysteresis.
         
     By default all reversal points on the backbone curve are returned.
     This will not be appropriate for some types of hysteresis where the load
@@ -230,17 +243,17 @@
     -------
     avg, pos, neg : SimpleCycle
         A simpleCycle object of the output backbone curve.
 
     """
     
     
-    hysNeg = Hysteresis(-hystersis.xy)
-    hysNeg.recalculateCycles_like(hystersis)
-    backBonePos = getBackboneCurve(hystersis, LPsteps, returnPeaks, returnEnd, skipStart, skipEnd)
+    hysNeg = Hysteresis(-hysteresis.xy)
+    hysNeg.recalculateCycles_like(hysteresis)
+    backBonePos = getBackboneCurve(hysteresis, LPsteps, returnPeaks, returnEnd, skipStart, skipEnd)
     backBoneNeg = getBackboneCurve(hysNeg, LPsteps, returnPeaks, returnEnd, skipStart, skipEnd)
     
     backBoneAvg = _averageBackbones(backBonePos, backBoneNeg)
 
     
     return backBoneAvg, backBonePos, backBoneNeg
```

### Comparing `hysteresis-2.0.0/Hysteresis/plotSpecial/animate.py` & `hysteresis-2.0.1/Hysteresis/plotSpecial/animate.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/plotSpecial/core.py` & `hysteresis-2.0.1/Hysteresis/plotSpecial/core.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/plotSpecial/guiPlot.py` & `hysteresis-2.0.1/Hysteresis/plotSpecial/guiPlot.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/protocol.py` & `hysteresis-2.0.1/Hysteresis/protocol.py`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/Hysteresis/resample.py` & `hysteresis-2.0.1/Hysteresis/resample.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,55 @@
 from .curve import Hysteresis, SimpleCurve, MonotonicCurve
 from .baseFuncs import (concatenateHys, concatenate, _linInterp, 
                         _linInterpSample, _getNsamples)
        
 # =============================================================================
 # concatenate and resample
 # =============================================================================
-           
+
+def _resampleSimpleCurve(curve, Nsamples):
+    x = curve.xy[:,0]
+    y = curve.xy[:,1]
+    
+    # If the simple cycle has subcycles, resample at the level of those.
+    if curve.subCycles:
+        outputSubcycles = [None]*curve.NsubCycles
+        for ii, subcycle in enumerate(curve.subCycles):
+            outputSubcycles[ii] = resample(subcycle, Nsamples)    
+            
+        tmpOut      = concatenate(outputSubcycles, outputClass = SimpleCurve)
+        tmpProps    = curve._getStatePropreties()
+        return SimpleCurve(tmpOut.xy, *tmpProps)
+                    
+    # Otherwise, resample the curve directly
+    else:
+        return SimpleCurve(_linInterp(x,y, Nsamples))  
+
+
+def _resampleHysteresis(curve, Nsamples):
+    outputCycles = [None]*curve.NCycles
+    for ii, cycle in enumerate(curve.cycles):
+        outputCycles[ii] = resample(cycle, Nsamples)      
+    
+    tmpOut = concatenateHys(outputCycles)    # If curve
+    tmpProps = curve._getStatePropreties()
+    return Hysteresis(tmpOut.xy,*tmpProps)      
+
+def _resampleMonotonicCurve(curve, Nsamples):
+    x = curve.xy[:,0]
+    y = curve.xy[:,1]
+    return MonotonicCurve(_linInterp(x,y, Nsamples))     
+
+def _resampleArray(curve, Nsamples):
+    x = curve[:,0]
+    y = curve[:,1]
+    return _linInterp(x,y, Nsamples)  
+
+
+
 def resample(curve, Nsamples, **kwargs):
     """
     Creates a new curve object that has a different number of sample points 
     between the start and end of each Cycle object.
     The curve resampled will be one level down, i.e. Hystereses will their
     simpleCycles resampled, and SimpleCycles will have their Monotonic Curves
     resampled
@@ -38,62 +78,75 @@
 
     """  
         
     # We recursively resample by calling the function again for sub-cycle objects
     
     # if the curve is a SimpleCycle
     if isinstance(curve, SimpleCurve):
-        x = curve.xy[:,0]
-        y = curve.xy[:,1]
-        
-        # If the simple cycle has subcycles, resample at the level of those.
-        if curve.subCycles:
-            outputSubcycles = [None]*curve.NsubCycles
-            for ii, subcycle in enumerate(curve.subCycles):
-                outputSubcycles[ii] = resample(subcycle, Nsamples)    
-                
-            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
-            tmpProps    = curve._getStatePropreties()
-            Output      = SimpleCurve(tmpOut.xy, *tmpProps)
-                        
-        # Otherwise, resample the curve directly
-        else:
-            Output = SimpleCurve(_linInterp(x,y, Nsamples))    
+        output = _resampleSimpleCurve(curve, Nsamples)
        
     # if the curve is a hysteresis, we recursively create a series of Cycles
     elif isinstance(curve, Hysteresis):
-        outputCycles = [None]*curve.NCycles
-        for ii, cycle in enumerate(curve.cycles):
-            outputCycles[ii] = resample(cycle, Nsamples)
-        Output = concatenateHys(outputCycles)    # If curve
-        
-        
-        tmpOut = concatenateHys(outputCycles)    # If curve
-        tmpProps = curve._getStatePropreties()
-        Output = Hysteresis(tmpOut.xy,*tmpProps)
-                
+        output = _resampleHysteresis(curve, Nsamples)
         
     # if the curve is a Monotonic Cycle
     elif isinstance(curve, MonotonicCurve):
-        x = curve.xy[:,0]
-        y = curve.xy[:,1]
-        Output = MonotonicCurve(_linInterp(x,y, Nsamples))  
+        output = _resampleMonotonicCurve(curve, Nsamples)
     
     # if it is a np array
     elif isinstance(curve, np.ndarray):
-        x = curve[:,0]
-        y = curve[:,1]
-        Output = _linInterp(x,y, Nsamples)  
+        output = _resampleArray(curve, Nsamples)
         
     else:
-        Output = None
+        output = None
         
-    return Output
-   
-def resampleDx(curve, Targetdx):
+    return output
+
+
+
+
+def _resampledxSimpleCurve(curve, targetdx):
+    if curve.subCycles: # if subsycles are set, resample those
+        outputSubcycles = [None]*curve.NsubCycles
+        for ii, subcycle in enumerate(curve.subCycles):
+            outputSubcycles[ii] = resampleDx(subcycle, targetdx)        
+        tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
+        tmpProps    = curve._getStatePropreties()
+        return SimpleCurve(tmpOut.xy, *tmpProps)        
+    
+    else: # if subsycles aren't set, resample those
+        x = curve.xy[:,0]
+        dxNet = x[-1] - x[0]
+        Nsamples = _getNsamples(targetdx, dxNet)
+        return resample(curve, Nsamples)     
+
+
+def _resampledxHysteresis(curve, targetdx):
+    outputCycles = [None]*curve.NCycles
+    for ii, cycle in enumerate(curve.cycles):
+        outputCycles[ii] = resampleDx(cycle, targetdx)       
+    tmpOut = concatenateHys(outputCycles)    # If curve
+    tmpProps = curve._getStatePropreties()
+    return Hysteresis(tmpOut.xy,*tmpProps)         
+
+def _resampledxMonotonicCurve(curve, targetdx):
+    x = curve.xy[:,0]
+    dxNet = x[-1] - x[0]
+    Nsamples = _getNsamples(targetdx, dxNet)
+    return resample(curve, Nsamples)      
+
+def _resampledxArray(curve, targetdx):
+    x = curve[:,0]
+    dxNet = x[-1] - x[0]
+    Nsamples = _getNsamples(targetdx, dxNet)        
+    return resample(curve, Nsamples)
+
+
+
+def resampleDx(curve, targetdx):
     """
     Creates a new curve object where the distance between sample points
     is approximately dx. The number of samples betweent the start and 
     end point of each cycle is calculated so that the is as close to dx 
     as possible. Note that distance isn't precisely dx.
     
 
@@ -119,59 +172,31 @@
     Returns
     -------
     curve :
         An object of the input type, with points approximately at Targetdx.
 
     """  
 
-
     # the logic in these functions is getting a little nasty, in the future
     # consider pulling these out into class methods.
     if isinstance(curve, SimpleCurve):
-               
-        if curve.subCycles: # if subsycles are set, resample those
-            outputSubcycles = [None]*curve.NsubCycles
-            for ii, subcycle in enumerate(curve.subCycles):
-                outputSubcycles[ii] = resampleDx(subcycle, Targetdx)
-            # Output = concatenate(*outputSubcycles, outputClass = SimpleCurve)    # If curve        
-        
-            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
-            tmpProps    = curve._getStatePropreties()
-            Output      = SimpleCurve(tmpOut.xy, *tmpProps)        
-        
-        else: # if subsycles aren't set, resample those
-            x = curve.xy[:,0]
-            dxNet = x[-1] - x[0]
-            Nsamples = _getNsamples(Targetdx, dxNet)
-            Output = resample(curve, Nsamples)    
-        
-        
+        output = _resampledxSimpleCurve(curve, targetdx) 
+                
     elif isinstance(curve, Hysteresis):
-        outputCycles = [None]*curve.NCycles
-        for ii, cycle in enumerate(curve.cycles):
-            outputCycles[ii] = resampleDx(cycle, Targetdx)       
-        tmpOut = concatenateHys(outputCycles)    # If curve
-        tmpProps = curve._getStatePropreties()
-        Output = Hysteresis(tmpOut.xy,*tmpProps)       
+        output = _resampledxHysteresis(curve, targetdx) 
        
     # if the curve is a MonotonicCurve Cycle
     elif isinstance(curve, MonotonicCurve):
-        x = curve.xy[:,0]
-        dxNet = x[-1] - x[0]
-        Nsamples = _getNsamples(Targetdx, dxNet)
-        Output = resample(curve, Nsamples)  
+        output = _resampledxMonotonicCurve(curve, targetdx) 
     
     # if it is a np array
     elif isinstance(curve, np.ndarray):
-        x = curve[:,0]
-        dxNet = x[-1] - x[0]
-        Nsamples = _getNsamples(Targetdx, dxNet)        
-        Output = resample(curve, Nsamples)
+        output = _resampledxArray(curve, targetdx) 
         
-    return Output
+    return output
 
 
 
 
 def _parseRegions(regions):
     """
     Ensures each region either has only two items, and
@@ -218,15 +243,88 @@
     if  breakPoints[-1] < xmax:
         outsideRegions.append([breakPoints[-1], xmax])        
         isInside.append(False)
         
     return outsideRegions, isInside
 
 
-def resampleRegion(curve, Nsamples, regions = [[0, 0.1], [0.9, 1]]):
+
+
+def _resampleRegionSimpleCurve(curve, Nsamples, regions):
+    if curve.subCycles: # if subsycles are set, resample those
+        outputSubcycles = [None]*curve.NsubCycles
+        for ii, subcycle in enumerate(curve.subCycles):
+            outputSubcycles[ii] = resampleRegion(subcycle, Nsamples, regions)
+            
+        tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
+        tmpProps    = curve._getStatePropreties()
+        return SimpleCurve(tmpOut.xy, *tmpProps)        
+    
+    else: # if subsycles aren't set, resample at level of xy
+    
+        x = curve.xy[:,0]
+        y = curve.xy[:,1]
+        xy = np.column_stack([x, y])
+        return SimpleCurve(resampleRegion(xy, Nsamples, regions))    
+
+
+def _resampleRegionHysteresis(curve, Nsamples, regions):
+    outputCycles = [None]*curve.NCycles
+    for ii, cycle in enumerate(curve.cycles):
+        outputCycles[ii] = resampleRegion(cycle, Nsamples, regions)
+    tmpOut = concatenateHys(outputCycles)
+    tmpProps = curve._getStatePropreties()
+    return Hysteresis(tmpOut.xy,*tmpProps)        
+
+def _resampleRegionMonotonicCurve(curve, Nsamples, regions):
+    x = curve.xy[:,0]
+    y = curve.xy[:,1]
+    xy = np.column_stack([x, y])
+    return  MonotonicCurve(resampleRegion(xy, Nsamples, regions))        
+
+
+
+def _resampleRegionArray(curve, Nsamples, regions):
+    
+    allRegions, isInside = _getOutsideRegions(regions) # these get left alone  
+    x = curve[:,0]
+    y = curve[:,1] 
+
+    xSamples = []
+    ySamples = []
+    
+    allRegions = np.array(allRegions)*(x[-1] - x[0]) + x[0]
+    
+    if x[0] <= x[-1]:
+        isLeftRight = True
+    else:
+        isLeftRight = False
+    
+    for ii, region in enumerate(allRegions):
+        if isInside[ii]:
+            xtmp = np.linspace(region[0], region[1], Nsamples)
+            ytmp = _linInterpSample(x, y, xtmp)[:,1]
+    
+        else:
+            if isLeftRight:
+                inds = np.where((region[0] < x) *  (x < region[1]))
+            else:
+                inds = np.where((x < region[0]) *  (region[1] < x))
+
+            xtmp = x[inds]
+            ytmp = y[inds]
+        
+        xSamples.append(xtmp)
+        ySamples.append(ytmp)
+        
+    xSamples = np.concatenate(xSamples)
+    ySamples = np.concatenate(ySamples)
+    return np.column_stack([xSamples, ySamples])
+
+def resampleRegion(curve, Nsamples, regions = None):
     """
     Resamples only parts of an input a curve. The part of the
     curve that is resampled is defined using the regions variable.
     The regions is a list of lists, defining a start and end point
     of the curve in terms of a parameter varying between 0 and 1.
     
     Each region is resampled using Nsamples
@@ -251,83 +349,26 @@
         The number of sample to use for each region.
 
     Returns
     -------
     None.
 
     """
-    
+    if not regions:
+        regions = [[0, 0.1], [0.9, 1]]
     
     regions = _parseRegions(regions) # these get interpolated
-    allRegions, isInside = _getOutsideRegions(regions) # these get left alone  
-    
-    
+        
     if isinstance(curve, SimpleCurve):
-
-        if curve.subCycles: # if subsycles are set, resample those
-            outputSubcycles = [None]*curve.NsubCycles
-            for ii, subcycle in enumerate(curve.subCycles):
-                outputSubcycles[ii] = resampleRegion(subcycle, Nsamples, regions)
-                
-            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
-            tmpProps    = curve._getStatePropreties()
-            output      = SimpleCurve(tmpOut.xy, *tmpProps)        
-        
-        else: # if subsycles aren't set, resample at level of xy
-        
-            x = curve.xy[:,0]
-            y = curve.xy[:,1]
-            xy = np.column_stack([x, y])
-            output = SimpleCurve(resampleRegion(xy, Nsamples, regions))        
+        output = _resampleRegionSimpleCurve(curve, Nsamples,regions)
     
     elif isinstance(curve, Hysteresis):
-        outputCycles = [None]*curve.NCycles
-        for ii, cycle in enumerate(curve.cycles):
-            outputCycles[ii] = resampleRegion(cycle, Nsamples, regions)
-        tmpOut = concatenateHys(outputCycles)
-        tmpProps = curve._getStatePropreties()
-        output = Hysteresis(tmpOut.xy,*tmpProps)    
-    
+        output = _resampleRegionHysteresis(curve, Nsamples, regions)
     
     elif isinstance(curve, MonotonicCurve):
-        x = curve.xy[:,0]
-        y = curve.xy[:,1]
-        xy = np.column_stack([x, y])
-        output = MonotonicCurve(resampleRegion(xy, Nsamples, regions))  
+        output = _resampleRegionMonotonicCurve(curve, Nsamples, regions)
     
     # if it is a np array
     elif isinstance(curve, np.ndarray):
-        x = curve[:,0]
-        y = curve[:,1] 
-
-        xSamples = []
-        ySamples = []
-        
-        allRegions = np.array(allRegions)*(x[-1] - x[0]) + x[0]
-        
-        if x[0] <= x[-1]:
-            isLeftRight = True
-        else:
-            isLeftRight = False
-        
-        for ii, region in enumerate(allRegions):
-            if isInside[ii]:
-                xtmp = np.linspace(region[0], region[1], Nsamples)
-                ytmp = _linInterpSample(x, y, xtmp)[:,1]
-        
-            else:
-                if isLeftRight:
-                    inds = np.where((region[0] < x) *  (x < region[1]))
-                else:
-                    inds = np.where((x < region[0]) *  (region[1] < x))
-
-                xtmp = x[inds]
-                ytmp = y[inds]
-            
-            xSamples.append(xtmp)
-            ySamples.append(ytmp)
-            
-        xSamples = np.concatenate(xSamples)
-        ySamples = np.concatenate(ySamples)
-        output = np.column_stack([xSamples, ySamples])
+        output = _resampleRegionArray(curve, Nsamples, regions)
         
     return output
```

### Comparing `hysteresis-2.0.0/Hysteresis.egg-info/PKG-INFO` & `hysteresis-2.0.1/Hysteresis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysteresis
-Version: 2.0.0
+Version: 2.0.1
 Summary: Hysteresis data processing tools
 Home-page: https://github.com/cslotboom/Hysteresis
 Author: Christian Slotboom
 Author-email: christia.slotboom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hysteresis-2.0.0/Hysteresis.egg-info/SOURCES.txt` & `hysteresis-2.0.1/Hysteresis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/PKG-INFO` & `hysteresis-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysteresis
-Version: 2.0.0
+Version: 2.0.1
 Summary: Hysteresis data processing tools
 Home-page: https://github.com/cslotboom/Hysteresis
 Author: Christian Slotboom
 Author-email: christia.slotboom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hysteresis-2.0.0/README.md` & `hysteresis-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/license.txt` & `hysteresis-2.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `hysteresis-2.0.0/setup.py` & `hysteresis-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hysteresis",
-    version="2.0.0",
+    version="2.0.1",
     author="Christian Slotboom",
     author_email="christia.slotboom@gmail.com",
     description="Hysteresis data processing tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cslotboom/Hysteresis",
     packages=setuptools.find_packages(),
```

