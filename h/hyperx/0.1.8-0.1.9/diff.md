# Comparing `tmp/hyperx-0.1.8.tar.gz` & `tmp/hyperx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.1.8.tar", last modified: Thu Jul 27 13:51:06 2023, max compression
+gzip compressed data, was "hyperx-0.1.9.tar", last modified: Wed Aug  2 19:18:24 2023, max compression
```

## Comparing `hyperx-0.1.8.tar` & `hyperx-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.838381 hyperx-0.1.8/
--rw-rw-rw-   0        0        0      535 2023-07-27 13:51:06.836777 hyperx-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.785878 hyperx-0.1.8/hyperx/
--rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-0.1.8/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.808916 hyperx-0.1.8/hyperx/api/
--rw-rw-rw-   0        0        0   158176 2023-07-27 13:49:52.000000 hyperx-0.1.8/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.811916 hyperx-0.1.8/hyperx/api/types/
--rw-rw-rw-   0        0        0    23328 2023-07-27 13:49:25.000000 hyperx-0.1.8/hyperx/api/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.828777 hyperx-0.1.8/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.8/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.8/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.8/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.833778 hyperx-0.1.8/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.8/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.8/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 13:51:06.805529 hyperx-0.1.8/hyperx.egg-info/
--rw-rw-rw-   0        0        0      535 2023-07-27 13:51:06.000000 hyperx-0.1.8/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-07-27 13:51:06.000000 hyperx-0.1.8/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 13:51:06.000000 hyperx-0.1.8/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 13:51:06.000000 hyperx-0.1.8/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 13:51:06.000000 hyperx-0.1.8/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-07-27 13:50:48.000000 hyperx-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 13:51:06.839381 hyperx-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.777074 hyperx-0.1.9/
+-rw-rw-rw-   0        0        0      535 2023-08-02 19:18:24.776074 hyperx-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.742698 hyperx-0.1.9/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-0.1.9/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.760774 hyperx-0.1.9/hyperx/api/
+-rw-rw-rw-   0        0        0   161428 2023-08-02 19:09:25.000000 hyperx-0.1.9/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.762774 hyperx-0.1.9/hyperx/api/types/
+-rw-rw-rw-   0        0        0    23328 2023-08-02 18:26:00.000000 hyperx-0.1.9/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.770074 hyperx-0.1.9/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.774074 hyperx-0.1.9/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.9/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.758779 hyperx-0.1.9/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-08-02 19:18:07.000000 hyperx-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 19:18:24.777074 hyperx-0.1.9/setup.cfg
```

### Comparing `hyperx-0.1.8/PKG-INFO` & `hyperx-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.8
+Version: 0.1.9
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.8/hyperx/__init__.py` & `hyperx-0.1.9/hyperx/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.8/hyperx/api/__init__.py` & `hyperx-0.1.9/hyperx/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -637,26 +637,26 @@
 	@overload
 	def RemoveFailureMode(self, ids: tuple[int]) -> None: ...
 
 	def AddFailureMode(self, item1 = None) -> None:
 		if isinstance(item1, int):
 			return self._Entity.AddFailureMode(item1)
 
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			idsList = MakeCSharpIntList(item1)
 			idsEnumerable = IEnumerable(idsList)
 			return self._Entity.AddFailureMode(idsEnumerable)
 
 		return self._Entity.AddFailureMode(item1)
 
 	def RemoveFailureMode(self, item1 = None) -> None:
 		if isinstance(item1, int):
 			return self._Entity.RemoveFailureMode(item1)
 
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			idsList = MakeCSharpIntList(item1)
 			idsEnumerable = IEnumerable(idsList)
 			return self._Entity.RemoveFailureMode(idsEnumerable)
 
 		return self._Entity.RemoveFailureMode(item1)
 
 
@@ -1463,17 +1463,23 @@
 	@overload
 	def RemoveJoints(self, joints: JointCol) -> CollectionModificationStatus: ...
 
 	@overload
 	def AddZone(self, id: int) -> CollectionModificationStatus: ...
 
 	@overload
+	def AddZones(self, ids: tuple[int]) -> CollectionModificationStatus: ...
+
+	@overload
 	def AddZone(self, zone: Zone) -> CollectionModificationStatus: ...
 
 	@overload
+	def AddZones(self, zones: tuple[Zone]) -> CollectionModificationStatus: ...
+
+	@overload
 	def RemoveZone(self, id: int) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveZone(self, zone: Zone) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveZones(self, zoneIds: tuple[int]) -> CollectionModificationStatus: ...
@@ -1514,52 +1520,69 @@
 
 		if isinstance(item1, Joint):
 			return CollectionModificationStatus[self._Entity.RemoveJoint(item1._Entity).ToString()]
 
 		return self._Entity.RemoveJoint(item1)
 
 	def RemoveJoints(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			jointIdsList = MakeCSharpIntList(item1)
 			jointIdsEnumerable = IEnumerable(jointIdsList)
 			return CollectionModificationStatus[self._Entity.RemoveJoints(jointIdsEnumerable).ToString()]
 
 		if isinstance(item1, JointCol):
 			return CollectionModificationStatus[self._Entity.RemoveJoints(item1._Entity).ToString()]
 
-		return self._Entity.RemoveJoints(jointIdsEnumerable)
+		return self._Entity.RemoveJoints(item1)
 
 	def AddZone(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus[self._Entity.AddZone(item1).ToString()]
 
 		if isinstance(item1, Zone):
 			return CollectionModificationStatus[self._Entity.AddZone(item1._Entity).ToString()]
 
 		return self._Entity.AddZone(item1)
 
+	def AddZones(self, item1 = None) -> CollectionModificationStatus:
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
+			idsList = MakeCSharpIntList(item1)
+			idsEnumerable = IEnumerable(idsList)
+			return CollectionModificationStatus[self._Entity.AddZones(idsEnumerable).ToString()]
+
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], Zone):
+			zonesList = List[_api.Zone]()
+			if item1 is not None:
+				for thing in item1:
+					if thing is not None:
+						zonesList.Add(thing._Entity)
+			zonesEnumerable = IEnumerable(zonesList)
+			return CollectionModificationStatus[self._Entity.AddZones(zonesEnumerable).ToString()]
+
+		return self._Entity.AddZones(item1)
+
 	def RemoveZone(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus[self._Entity.RemoveZone(item1).ToString()]
 
 		if isinstance(item1, Zone):
 			return CollectionModificationStatus[self._Entity.RemoveZone(item1._Entity).ToString()]
 
 		return self._Entity.RemoveZone(item1)
 
 	def RemoveZones(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			zoneIdsEnumerable = IEnumerable(zoneIdsList)
 			return CollectionModificationStatus[self._Entity.RemoveZones(zoneIdsEnumerable).ToString()]
 
 		if isinstance(item1, ZoneCol):
 			return CollectionModificationStatus[self._Entity.RemoveZones(item1._Entity).ToString()]
 
-		return self._Entity.RemoveZones(zoneIdsEnumerable)
+		return self._Entity.RemoveZones(item1)
 
 	def AddPanelSegment(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus[self._Entity.AddPanelSegment(item1).ToString()]
 
 		if isinstance(item1, PanelSegment):
 			return CollectionModificationStatus[self._Entity.AddPanelSegment(item1._Entity).ToString()]
@@ -1572,23 +1595,23 @@
 
 		if isinstance(item1, PanelSegment):
 			return CollectionModificationStatus[self._Entity.RemovePanelSegment(item1._Entity).ToString()]
 
 		return self._Entity.RemovePanelSegment(item1)
 
 	def RemovePanelSegments(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			segmentIdsList = MakeCSharpIntList(item1)
 			segmentIdsEnumerable = IEnumerable(segmentIdsList)
 			return CollectionModificationStatus[self._Entity.RemovePanelSegments(segmentIdsEnumerable).ToString()]
 
 		if isinstance(item1, PanelSegmentCol):
 			return CollectionModificationStatus[self._Entity.RemovePanelSegments(item1._Entity).ToString()]
 
-		return self._Entity.RemovePanelSegments(segmentIdsEnumerable)
+		return self._Entity.RemovePanelSegments(item1)
 
 
 class FoamTemperature:
 	'''
 	Foam material temperature dependent properties.
 	'''
 	def __init__(self, foamTemperature: _api.FoamTemperature):
@@ -3915,15 +3938,15 @@
 	@overload
 	def AddJoint(self, joint: Joint) -> CollectionModificationStatus: ...
 
 	@overload
 	def AddPanelSegment(self, segment: PanelSegment) -> CollectionModificationStatus: ...
 
 	@overload
-	def AddZone(self, zone: Zone) -> CollectionModificationStatus: ...
+	def AddZones(self, zones: tuple[Zone]) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveJoints(self, jointIds: tuple[int]) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemovePanelSegments(self, segmentIds: tuple[int]) -> CollectionModificationStatus: ...
 
@@ -3942,14 +3965,20 @@
 	@overload
 	def RemoveJoints(self, joints: JointCol) -> CollectionModificationStatus: ...
 
 	@overload
 	def AddZone(self, id: int) -> CollectionModificationStatus: ...
 
 	@overload
+	def AddZones(self, ids: tuple[int]) -> CollectionModificationStatus: ...
+
+	@overload
+	def AddZone(self, zone: Zone) -> CollectionModificationStatus: ...
+
+	@overload
 	def RemoveZone(self, id: int) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveZone(self, zone: Zone) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveZones(self, zones: ZoneCol) -> CollectionModificationStatus: ...
@@ -3980,65 +4009,80 @@
 			return CollectionModificationStatus[self._Entity.AddPanelSegment(item1._Entity).ToString()]
 
 		if isinstance(item1, int):
 			return CollectionModificationStatus(super().AddPanelSegment(item1))
 
 		return self._Entity.AddPanelSegment(item1._Entity)
 
-	def AddZone(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, Zone):
-			return CollectionModificationStatus[self._Entity.AddZone(item1._Entity).ToString()]
+	def AddZones(self, item1 = None) -> CollectionModificationStatus:
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], Zone):
+			zonesList = List[_api.Zone]()
+			if item1 is not None:
+				for thing in item1:
+					if thing is not None:
+						zonesList.Add(thing._Entity)
+			zonesEnumerable = IEnumerable(zonesList)
+			return CollectionModificationStatus[self._Entity.AddZones(zonesEnumerable).ToString()]
 
-		if isinstance(item1, int):
-			return CollectionModificationStatus(super().AddZone(item1))
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
+			return CollectionModificationStatus(super().AddZones(item1))
 
-		return self._Entity.AddZone(item1._Entity)
+		return self._Entity.AddZones(item1)
 
 	def RemoveJoints(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			jointIdsList = MakeCSharpIntList(item1)
 			jointIdsEnumerable = IEnumerable(jointIdsList)
 			return CollectionModificationStatus[self._Entity.RemoveJoints(jointIdsEnumerable).ToString()]
 
 		if isinstance(item1, JointCol):
 			return CollectionModificationStatus(super().RemoveJoints(item1))
 
-		return self._Entity.RemoveJoints(jointIdsEnumerable)
+		return self._Entity.RemoveJoints(item1)
 
 	def RemovePanelSegments(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			segmentIdsList = MakeCSharpIntList(item1)
 			segmentIdsEnumerable = IEnumerable(segmentIdsList)
 			return CollectionModificationStatus[self._Entity.RemovePanelSegments(segmentIdsEnumerable).ToString()]
 
 		if isinstance(item1, PanelSegmentCol):
 			return CollectionModificationStatus(super().RemovePanelSegments(item1))
 
-		return self._Entity.RemovePanelSegments(segmentIdsEnumerable)
+		return self._Entity.RemovePanelSegments(item1)
 
 	def RemoveZones(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			zoneIdsEnumerable = IEnumerable(zoneIdsList)
 			return CollectionModificationStatus[self._Entity.RemoveZones(zoneIdsEnumerable).ToString()]
 
 		if isinstance(item1, ZoneCol):
 			return CollectionModificationStatus(super().RemoveZones(item1))
 
-		return self._Entity.RemoveZones(zoneIdsEnumerable)
+		return self._Entity.RemoveZones(item1)
 
 	def RemoveJoint(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus(super().RemoveJoint(item1))
 
 		if isinstance(item1, Joint):
 			return CollectionModificationStatus(super().RemoveJoint(item1))
 
 		return self._Entity.RemoveJoint(item1)
 
+	def AddZone(self, item1 = None) -> CollectionModificationStatus:
+		if isinstance(item1, int):
+			return CollectionModificationStatus(super().AddZone(item1))
+
+		if isinstance(item1, Zone):
+			return CollectionModificationStatus(super().AddZone(item1))
+
+		return self._Entity.AddZone(item1)
+
 	def RemoveZone(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus(super().RemoveZone(item1))
 
 		if isinstance(item1, Zone):
 			return CollectionModificationStatus(super().RemoveZone(item1))
 
@@ -4139,15 +4183,15 @@
 
 	def AddPfemProperties(self, pfemPropertyIds: tuple[int]) -> CollectionModificationStatus:
 		pfemPropertyIdsList = MakeCSharpIntList(pfemPropertyIds)
 		pfemPropertyIdsEnumerable = IEnumerable(pfemPropertyIdsList)
 		return CollectionModificationStatus[self._Entity.AddPfemProperties(pfemPropertyIdsEnumerable).ToString()]
 
 	@overload
-	def AddZone(self, zone: Zone) -> CollectionModificationStatus: ...
+	def AddZones(self, zones: tuple[Zone]) -> CollectionModificationStatus: ...
 
 	def CreateZone(self, elementIds: tuple[int], name: str = None) -> None:
 		elementIdsList = MakeCSharpIntList(elementIds)
 		elementIdsEnumerable = IEnumerable(elementIdsList)
 		return self._Entity.CreateZone(elementIdsEnumerable, name)
 
 	def CreatePanelSegment(self, discreteTechnique: types.DiscreteTechnique, discreteElementLkp: dict[types.DiscreteDefinitionType, list[int]], name: str = None) -> int:
@@ -4183,14 +4227,20 @@
 	@overload
 	def RemoveJoints(self, joints: JointCol) -> CollectionModificationStatus: ...
 
 	@overload
 	def AddZone(self, id: int) -> CollectionModificationStatus: ...
 
 	@overload
+	def AddZones(self, ids: tuple[int]) -> CollectionModificationStatus: ...
+
+	@overload
+	def AddZone(self, zone: Zone) -> CollectionModificationStatus: ...
+
+	@overload
 	def RemoveZone(self, id: int) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveZone(self, zone: Zone) -> CollectionModificationStatus: ...
 
 	@overload
 	def RemoveZones(self, zones: ZoneCol) -> CollectionModificationStatus: ...
@@ -4221,84 +4271,99 @@
 			return CollectionModificationStatus[self._Entity.AddPanelSegment(item1._Entity).ToString()]
 
 		if isinstance(item1, int):
 			return CollectionModificationStatus(super().AddPanelSegment(item1))
 
 		return self._Entity.AddPanelSegment(item1._Entity)
 
-	def AddZone(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, Zone):
-			return CollectionModificationStatus[self._Entity.AddZone(item1._Entity).ToString()]
+	def AddZones(self, item1 = None) -> CollectionModificationStatus:
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], Zone):
+			zonesList = List[_api.Zone]()
+			if item1 is not None:
+				for thing in item1:
+					if thing is not None:
+						zonesList.Add(thing._Entity)
+			zonesEnumerable = IEnumerable(zonesList)
+			return CollectionModificationStatus[self._Entity.AddZones(zonesEnumerable).ToString()]
 
-		if isinstance(item1, int):
-			return CollectionModificationStatus(super().AddZone(item1))
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
+			return CollectionModificationStatus(super().AddZones(item1))
 
-		return self._Entity.AddZone(item1._Entity)
+		return self._Entity.AddZones(item1)
 
 	def Remove(self, item1 = None, item2 = None, item3 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple) and isinstance(item2, tuple) and isinstance(item3, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int) and isinstance(item2, tuple) and len(item2) > 0 and isinstance(item2[0], int) and isinstance(item3, tuple) and len(item3) > 0 and isinstance(item3[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			zoneIdsEnumerable = IEnumerable(zoneIdsList)
 			jointIdsList = MakeCSharpIntList(item2)
 			jointIdsEnumerable = IEnumerable(jointIdsList)
 			panelSegmentIdsList = MakeCSharpIntList(item3)
 			panelSegmentIdsEnumerable = IEnumerable(panelSegmentIdsList)
 			return CollectionModificationStatus[self._Entity.Remove(zoneIdsEnumerable, jointIdsEnumerable, panelSegmentIdsEnumerable).ToString()]
 
-		if isinstance(item1, tuple) and isinstance(item2, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int) and isinstance(item2, tuple) and len(item2) > 0 and isinstance(item2[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			zoneIdsEnumerable = IEnumerable(zoneIdsList)
 			jointIdsList = MakeCSharpIntList(item2)
 			jointIdsEnumerable = IEnumerable(jointIdsList)
 			return CollectionModificationStatus[self._Entity.Remove(zoneIdsEnumerable, jointIdsEnumerable).ToString()]
 
-		return self._Entity.Remove(zoneIdsEnumerable, jointIdsEnumerable, panelSegmentIdsEnumerable)
+		return self._Entity.Remove(item1, item2, item3)
 
 	def RemoveJoints(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			jointIdsList = MakeCSharpIntList(item1)
 			jointIdsEnumerable = IEnumerable(jointIdsList)
 			return CollectionModificationStatus[self._Entity.RemoveJoints(jointIdsEnumerable).ToString()]
 
 		if isinstance(item1, JointCol):
 			return CollectionModificationStatus(super().RemoveJoints(item1))
 
-		return self._Entity.RemoveJoints(jointIdsEnumerable)
+		return self._Entity.RemoveJoints(item1)
 
 	def RemovePanelSegments(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			segmentIdsList = MakeCSharpIntList(item1)
 			segmentIdsEnumerable = IEnumerable(segmentIdsList)
 			return CollectionModificationStatus[self._Entity.RemovePanelSegments(segmentIdsEnumerable).ToString()]
 
 		if isinstance(item1, PanelSegmentCol):
 			return CollectionModificationStatus(super().RemovePanelSegments(item1))
 
-		return self._Entity.RemovePanelSegments(segmentIdsEnumerable)
+		return self._Entity.RemovePanelSegments(item1)
 
 	def RemoveZones(self, item1 = None) -> CollectionModificationStatus:
-		if isinstance(item1, tuple):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			zoneIdsEnumerable = IEnumerable(zoneIdsList)
 			return CollectionModificationStatus[self._Entity.RemoveZones(zoneIdsEnumerable).ToString()]
 
 		if isinstance(item1, ZoneCol):
 			return CollectionModificationStatus(super().RemoveZones(item1))
 
-		return self._Entity.RemoveZones(zoneIdsEnumerable)
+		return self._Entity.RemoveZones(item1)
 
 	def RemoveJoint(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus(super().RemoveJoint(item1))
 
 		if isinstance(item1, Joint):
 			return CollectionModificationStatus(super().RemoveJoint(item1))
 
 		return self._Entity.RemoveJoint(item1)
 
+	def AddZone(self, item1 = None) -> CollectionModificationStatus:
+		if isinstance(item1, int):
+			return CollectionModificationStatus(super().AddZone(item1))
+
+		if isinstance(item1, Zone):
+			return CollectionModificationStatus(super().AddZone(item1))
+
+		return self._Entity.AddZone(item1)
+
 	def RemoveZone(self, item1 = None) -> CollectionModificationStatus:
 		if isinstance(item1, int):
 			return CollectionModificationStatus(super().RemoveZone(item1))
 
 		if isinstance(item1, Zone):
 			return CollectionModificationStatus(super().RemoveZone(item1))
 
@@ -4872,57 +4937,57 @@
 	@overload
 	def ExportCad(self, filePath: str) -> None: ...
 
 	@overload
 	def ExportCad(self, cadIds: tuple[int], filePath: str) -> None: ...
 
 	def AnalyzeZones(self, item1 = None) -> tuple[bool, str]:
-		if isinstance(item1, list):
+		if isinstance(item1, list) and len(item1) > 0 and isinstance(item1[0], Zone):
 			zonesList = List[_api.Zone]()
 			if item1 is not None:
 				for thing in item1:
 					if thing is not None:
 						zonesList.Add(thing._Entity)
 			result = self._Entity.AnalyzeZones(item1 if item1 is None else zonesList)
 			return tuple([result.Item1, result.Item2])
 
-		if isinstance(item1, list):
+		if isinstance(item1, list) and len(item1) > 0 and isinstance(item1[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			result = self._Entity.AnalyzeZones(zoneIdsList)
 			return tuple([result.Item1, result.Item2])
 
-		return self._Entity.AnalyzeZones(item1 if item1 is None else zonesList)
+		return self._Entity.AnalyzeZones(item1)
 
 	def SizeZones(self, item1 = None) -> tuple[bool, str]:
-		if isinstance(item1, list):
+		if isinstance(item1, list) and len(item1) > 0 and isinstance(item1[0], Zone):
 			zonesList = List[_api.Zone]()
 			if item1 is not None:
 				for thing in item1:
 					if thing is not None:
 						zonesList.Add(thing._Entity)
 			result = self._Entity.SizeZones(item1 if item1 is None else zonesList)
 			return tuple([result.Item1, result.Item2])
 
-		if isinstance(item1, list):
+		if isinstance(item1, list) and len(item1) > 0 and isinstance(item1[0], int):
 			zoneIdsList = MakeCSharpIntList(item1)
 			result = self._Entity.SizeZones(zoneIdsList)
 			return tuple([result.Item1, result.Item2])
 
-		return self._Entity.SizeZones(item1 if item1 is None else zonesList)
+		return self._Entity.SizeZones(item1)
 
 	def ExportCad(self, item1 = None, item2 = None) -> None:
-		if isinstance(item1, tuple) and isinstance(item2, str):
+		if isinstance(item1, tuple) and len(item1) > 0 and isinstance(item1[0], int) and isinstance(item2, str):
 			cadIdsList = MakeCSharpIntList(item1)
 			cadIdsEnumerable = IEnumerable(cadIdsList)
 			return self._Entity.ExportCad(cadIdsEnumerable, item2)
 
 		if isinstance(item1, str):
 			return self._Entity.ExportCad(item1)
 
-		return self._Entity.ExportCad(cadIdsEnumerable, item2)
+		return self._Entity.ExportCad(item1, item2)
 
 
 class ProjectInfo(IdNameEntityRenameable):
 	def __init__(self, projectInfo: _api.ProjectInfo):
 		self._Entity = projectInfo
```

### Comparing `hyperx-0.1.8/hyperx/api/types/__init__.py` & `hyperx-0.1.9/hyperx/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.8/hyperx/library/find.py` & `hyperx-0.1.9/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.8/hyperx/library/library.py` & `hyperx-0.1.9/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.8/hyperx/utils/utils.py` & `hyperx-0.1.9/hyperx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.8/hyperx.egg-info/PKG-INFO` & `hyperx-0.1.9/hyperx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.8
+Version: 0.1.9
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.8/pyproject.toml` & `hyperx-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyperx"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Kelly Ann Smith", email="kellyann.smith@collieraerospace.com" },
   { name="Noah Prezant", email="noah.prezant@collieraerospace.com" },
 ]
 description = "HyperX scripting for Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

