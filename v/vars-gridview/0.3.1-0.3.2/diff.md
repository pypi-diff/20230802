# Comparing `tmp/vars_gridview-0.3.1.tar.gz` & `tmp/vars_gridview-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.3.1.tar", max compression
+gzip compressed data, was "vars_gridview-0.3.2.tar", max compression
```

## Comparing `vars_gridview-0.3.1.tar` & `vars_gridview-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/LICENSE
--rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.3.1/README.md
--rw-r--r--   0        0        0      891 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/vars_gridview/__init__.py
--rw-r--r--   0        0        0      865 2023-08-01 22:13:37.845239 vars_gridview-0.3.1/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    13486 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.3.1/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.3.1/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.3.1/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     4518 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.3.1/vars_gridview/lib/util.py
--rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.3.1/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.1/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    25088 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    16306 2023-08-01 22:13:37.845239 vars_gridview-0.3.1/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0     3117 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/ui/SortDialog.py
--rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.1/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 vars_gridview-0.3.1/setup.py
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 vars_gridview-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.3.2/README.md
+-rw-r--r--   0        0        0      891 2023-08-01 22:30:20.091219 vars_gridview-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.2/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      935 2023-08-01 22:30:14.871236 vars_gridview-0.3.2/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    13486 2023-08-01 22:18:53.027493 vars_gridview-0.3.2/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.3.2/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.2/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.3.2/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.3.2/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.3.2/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     4518 2023-08-01 22:18:53.027493 vars_gridview-0.3.2/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.3.2/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.3.2/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.2/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    25088 2023-08-01 22:18:53.027493 vars_gridview-0.3.2/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.3.2/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    18666 2023-08-01 22:30:14.871236 vars_gridview-0.3.2/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0     3117 2023-08-01 22:18:53.027493 vars_gridview-0.3.2/vars_gridview/ui/SortDialog.py
+-rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.3.2/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.3.2/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.2/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 vars_gridview-0.3.2/setup.py
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 vars_gridview-0.3.2/PKG-INFO
```

### Comparing `vars_gridview-0.3.1/LICENSE` & `vars_gridview-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/README.md` & `vars_gridview-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/pyproject.toml` & `vars_gridview-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.3.1"
+version = "0.3.2"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
```

### Comparing `vars_gridview-0.3.1/vars_gridview/assets/base_query.sql` & `vars_gridview-0.3.2/vars_gridview/assets/base_query.sql`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-SELECT DISTINCT
+SELECT
     imaged_moment_uuid,
     image_reference_uuid,
     anno.observation_uuid AS observation_uuid,
     video_reference_uuid,
     anno.index_elapsed_time_millis,
     anno.index_recorded_timestamp,
     anno.index_timecode,
@@ -26,8 +26,10 @@
     pressure_dbar,
     salinity,
     temperature_celsius,
     light_transmission
 FROM
     annotations anno INNER JOIN associations assoc ON anno.observation_uuid = assoc.observation_uuid
 WHERE
+    assoc.link_name = 'bounding box' AND
+    assoc.link_value LIKE '{{%}}' AND
     {filters}
```

### Comparing `vars_gridview-0.3.1/vars_gridview/assets/gridview.ui` & `vars_gridview-0.3.2/vars_gridview/assets/gridview.ui`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.3.2/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/annotation.py` & `vars_gridview-0.3.2/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/boxes.py` & `vars_gridview-0.3.2/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/constants.py` & `vars_gridview-0.3.2/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.3.2/vars_gridview/lib/image_mosaic.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/log.py` & `vars_gridview-0.3.2/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.3.2/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.3.2/vars_gridview/lib/m3/clients.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.3.2/vars_gridview/lib/m3/operations.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/raziel.py` & `vars_gridview-0.3.2/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/settings.py` & `vars_gridview-0.3.2/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.3.2/vars_gridview/lib/sort_methods.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/sql.py` & `vars_gridview-0.3.2/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/util.py` & `vars_gridview-0.3.2/vars_gridview/lib/util.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/lib/widgets.py` & `vars_gridview-0.3.2/vars_gridview/lib/widgets.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/scripts/run.py` & `vars_gridview-0.3.2/vars_gridview/scripts/run.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.3.2/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.3.2/vars_gridview/ui/QueryDialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 class PlatformFilter(Filter):
     class Result(Filter.Result):
         def __init__(self, platform: str):
             self.platform = platform
 
         @property
         def constraints(self) -> Iterable[Constraint]:
-            yield Constraint("platform", self.platform)
+            yield Constraint("camera_platform", self.platform)
 
         def __str__(self) -> str:
             return "Platform: {}".format(self.platform)
 
     def __call__(self) -> Optional[Result]:
         platform, ok = QInputDialog.getText(
             self.parent, "Platform", "Platform", QLineEdit.EchoMode.Normal, ""
@@ -344,14 +344,86 @@
                 UUID(video_reference_uuid)
             except ValueError:
                 QMessageBox.warning(self.parent, "Invalid UUID", "The UUID is invalid.")
                 return None
             return VideoReferenceUUIDFilter.Result(video_reference_uuid.lower())
 
 
+class ActivityFilter(Filter):
+    class Result(Filter.Result):
+        def __init__(self, activity: str):
+            self.activity = activity
+        
+        @property
+        def constraints(self) -> Iterable[Constraint]:
+            yield Constraint("activity", self.activity)
+        
+        def __str__(self) -> str:
+            return "Activity: {}".format(self.activity)
+    
+    def __call__(self) -> Optional[Result]:
+        activity, ok = QInputDialog.getText(
+            self.parent,
+            "Activity",
+            "Activity",
+            QLineEdit.EchoMode.Normal,
+            "",
+        )
+        if ok:
+            return ActivityFilter.Result(activity)
+
+
+class ObservationGroupFilter(Filter):
+    class Result(Filter.Result):
+        def __init__(self, observation_group: str):
+            self.observation_group = observation_group
+        
+        @property
+        def constraints(self) -> Iterable[Constraint]:
+            yield Constraint("observation_group", self.observation_group)
+        
+        def __str__(self) -> str:
+            return "Observation group: {}".format(self.observation_group)
+    
+    def __call__(self) -> Optional[Result]:
+        observation_group, ok = QInputDialog.getText(
+            self.parent,
+            "Observation group",
+            "Observation group",
+            QLineEdit.EchoMode.Normal,
+            "",
+        )
+        if ok:
+            return ObservationGroupFilter.Result(observation_group)
+
+
+class GeneratorFilter(Filter):
+    class Result(Filter.Result):
+        def __init__(self, generator: str):
+            self.generator = generator
+        
+        @property
+        def constraints(self) -> Iterable[Constraint]:
+            yield Constraint("JSON_VALUE(assoc.link_value, '$.generator')", self.generator)
+
+        def __str__(self) -> str:
+            return "Generator: {}".format(self.generator)
+    
+    def __call__(self) -> Optional[Result]:
+        generator, ok = QInputDialog.getText(
+            self.parent,
+            "Generator",
+            "Generator",
+            QLineEdit.EchoMode.Normal,
+            "",
+        )
+        if ok:
+            return GeneratorFilter.Result(generator)
+
+
 class ResultListModel(QAbstractListModel):
     def __init__(self, parent: QObject = None, results: List[Filter.Result] = None):
         super().__init__(parent=parent)
 
         self.results = results or []
 
     def rowCount(self, parent: QModelIndex = None) -> int:
@@ -399,24 +471,27 @@
         self.setWindowTitle("Query")
         self.setLayout(QVBoxLayout())
 
         # Create filters
         self.filters = [
             ConceptFilter(self, "Concept"),
             ConceptDescFilter(self, "Concept (+ descendants)"),
-            DiveNumberFilter(self, "Dive number"),
+            # DiveNumberFilter(self, "Dive number"),
             VideoSequenceNameFilter(self, "Video sequence name"),
             ChiefScientistFilter(self, "Chief scientist"),
             PlatformFilter(self, "Platform"),
             ObserverFilter(self, "Observer"),
             ImagedMomentUUIDFilter(self, "Imaged moment UUID"),
             ObservationUUIDFilter(self, "Observation UUID"),
             AssociationUUIDFilter(self, "Association UUID"),
             ImageReferenceUUIDFilter(self, "Image reference UUID"),
             VideoReferenceUUIDFilter(self, "Video reference UUID"),
+            ActivityFilter(self, "Activity"),
+            ObservationGroupFilter(self, "Observation group"),
+            GeneratorFilter(self, "Generator"),
         ]
 
         # Create button bar (add, remove, clear constraints)
         self.button_bar = QWidget()
         self.button_bar.setLayout(QHBoxLayout())
         self.add_constraint_button = QPushButton("Add Constraint")
         self.add_constraint_button.setIcon(
```

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/SortDialog.py` & `vars_gridview-0.3.2/vars_gridview/ui/SortDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.3.2/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.3.2/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.1/setup.py` & `vars_gridview-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'sharktopoda-client==0.4.0']
 
 entry_points = \
 {'console_scripts': ['vars-gridview = vars_gridview.scripts.run:main']}
 
 setup_kwargs = {
     'name': 'vars-gridview',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.',
     'long_description': '# vars-gridview\n\n**VARS GridView** is a tool for reviewing and correcting VARS localizations in bulk.\n\n[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/downloads/)\n\nAuthors: Kevin Barnard ([kbarnard@mbari.org](mailto:kbarnard@mbari.org)), Paul Roberts ([proberts@mbari.org](mailto:proberts@mbari.org))\n\n---\n\n## Install\n\n### From PyPI\n\nVARS GridView is available on PyPI as `vars-gridview`. To install, run:\n\n```bash\npip install vars-gridview\n```\n\n### From source\n\nThis project is built with [Poetry](https://python-poetry.org/). To install from source, run (in the project root):\n\n```bash\npoetry install\n```\n\n## Run\n\nOnce VARS GridView is installed, you can run it from the command line:\n\n```bash\nvars-gridview\n```\n\nYou will first be prompted to log in. Enter your VARS username and password. \n\n*Note: If you are not using MBARI production VARS, change the "Config server" field to point to your instance of Raziel. This setting is persisted.*\n\n---\n\nCopyright &copy; 2020&ndash;2023 [Monterey Bay Aquarium Research Institute](https://www.mbari.org)',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mbari-org/vars-gridview',
```

### Comparing `vars_gridview-0.3.1/PKG-INFO` & `vars_gridview-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.3.1
+Version: 0.3.2
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
```

