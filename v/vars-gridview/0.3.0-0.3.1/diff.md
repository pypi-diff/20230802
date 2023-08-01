# Comparing `tmp/vars_gridview-0.3.0.tar.gz` & `tmp/vars_gridview-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.3.0.tar", max compression
+gzip compressed data, was "vars_gridview-0.3.1.tar", max compression
```

## Comparing `vars_gridview-0.3.0.tar` & `vars_gridview-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/LICENSE
--rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.3.0/README.md
--rw-r--r--   0        0        0      891 2023-06-16 00:39:48.645233 vars_gridview-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/vars_gridview/__init__.py
--rw-r--r--   0        0        0      865 2023-03-22 18:43:10.077134 vars_gridview-0.3.0/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    24010 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.3.0/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.3.0/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.3.0/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     3815 2023-06-12 16:29:02.472896 vars_gridview-0.3.0/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.3.0/vars_gridview/lib/util.py
--rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.3.0/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.0/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    24463 2023-06-16 00:39:48.645233 vars_gridview-0.3.0/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    16306 2023-03-22 18:43:10.077134 vars_gridview-0.3.0/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.0/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 vars_gridview-0.3.0/setup.py
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 vars_gridview-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.3.1/README.md
+-rw-r--r--   0        0        0      891 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      865 2023-08-01 22:13:37.845239 vars_gridview-0.3.1/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    13486 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.1/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.3.1/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.3.1/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.3.1/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     4518 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.3.1/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.3.1/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.1/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    25088 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.3.1/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    16306 2023-08-01 22:13:37.845239 vars_gridview-0.3.1/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0     3117 2023-08-01 22:15:53.857483 vars_gridview-0.3.1/vars_gridview/ui/SortDialog.py
+-rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.1/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 vars_gridview-0.3.1/setup.py
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 vars_gridview-0.3.1/PKG-INFO
```

### Comparing `vars_gridview-0.3.0/LICENSE` & `vars_gridview-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/README.md` & `vars_gridview-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/pyproject.toml` & `vars_gridview-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.3.0"
+version = "0.3.1"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
```

### Comparing `vars_gridview-0.3.0/vars_gridview/assets/base_query.sql` & `vars_gridview-0.3.1/vars_gridview/assets/base_query.sql`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.3.1/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/annotation.py` & `vars_gridview-0.3.1/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/boxes.py` & `vars_gridview-0.3.1/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/constants.py` & `vars_gridview-0.3.1/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.3.1/vars_gridview/lib/image_mosaic.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/log.py` & `vars_gridview-0.3.1/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.3.1/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.3.1/vars_gridview/lib/m3/clients.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.3.1/vars_gridview/lib/m3/operations.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/raziel.py` & `vars_gridview-0.3.1/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/settings.py` & `vars_gridview-0.3.1/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.3.1/vars_gridview/lib/sort_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
-from typing import Any, List
+from typing import Any, List, Tuple
 
 import numpy as np
 
 from vars_gridview.lib.widgets import RectWidget
 
 
 class SortMethod(ABC):
@@ -26,14 +26,40 @@
     def sort(cls, rect_widgets: List[RectWidget], **kwargs):
         """
         Sort a list of RectWidgets.
         """
         rect_widgets.sort(key=cls.key, **kwargs)
 
 
+class SortMethodGroup:
+    """
+    Composite method for sorting rect widgets by multiple sort methods. Methods are applied in the order they are specified.
+    """
+    
+    def __init__(self, *methods: SortMethod):
+        self.methods = methods
+
+    def key(self, rect: RectWidget) -> Tuple[Any]:
+        return tuple(method.key(rect) for method in self.methods)
+    
+    def sort(self, rect_widgets: List[RectWidget], **kwargs):
+        rect_widgets.sort(key=self.key, **kwargs)
+
+
+class NoopSort(SortMethod):
+    """
+    No-op sort method. Keeps the order of the rect widgets as-is.
+    """
+    NAME = "No-op"
+    
+    @staticmethod
+    def key(rect: RectWidget) -> None:
+        return None
+
+
 class RecordedTimestampSort(SortMethod):
     NAME = "Recorded timestamp"
     
     @staticmethod
     def key(rect: RectWidget) -> datetime:
         return rect.annotation_datetime() or datetime.min
```

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/sql.py` & `vars_gridview-0.3.1/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/util.py` & `vars_gridview-0.3.1/vars_gridview/lib/util.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/lib/widgets.py` & `vars_gridview-0.3.1/vars_gridview/lib/widgets.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/scripts/run.py` & `vars_gridview-0.3.1/vars_gridview/scripts/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     RegionMeanHueSort,
     WidthSort,
 )
 from vars_gridview.lib.util import parse_iso
 from vars_gridview.lib.widgets import RectWidget
 from vars_gridview.ui.LoginDialog import LoginDialog
 from vars_gridview.ui.QueryDialog import QueryDialog
+from vars_gridview.ui.SortDialog import SortDialog
 from vars_gridview.ui.settings.SettingsDialog import SettingsDialog
 
 # Define main window class from template
 CWD = Path(__file__).parent
 ASSETS_DIR = CWD.parent / "assets"
 UI_FILE_PATH = ASSETS_DIR / "gridview.ui"
 WindowTemplate, TemplateBaseClass = pg.Qt.loadUiType(UI_FILE_PATH)
@@ -127,18 +128,19 @@
         self.sharktopoda_connected = False  # Whether the Sharktopoda client is connected
 
         # Connect signals to slots
         self.ui.discardButton.clicked.connect(self.delete)
         self.ui.clearSelections.clicked.connect(self.clear_selected)
         self.ui.labelSelectedButton.clicked.connect(self.update_labels)
         self.ui.zoomSpinBox.valueChanged.connect(self.update_zoom)
-        self.ui.sortMethod.currentTextChanged.connect(self.update_layout)
+        # self.ui.sortMethod.currentTextChanged.connect(self.update_layout)
         self.ui.hideLabeled.stateChanged.connect(self.update_layout)
         self.ui.styleComboBox.currentTextChanged.connect(self._style_gui)
         self.ui.openVideo.clicked.connect(self.open_video)
+        self.ui.sortButton.clicked.connect(self._sort_widgets)
 
         self.settings_dialog = SettingsDialog(self)
 
         self._launch()
 
     @property
     def loaded(self):
@@ -156,16 +158,16 @@
             LOGGER.error("Login failed")
             QtWidgets.QMessageBox.critical(self, "Login failed", "Login failed, exiting.")
             sys.exit(1)
 
         # Set up the label combo boxes
         self._setup_label_boxes()
 
-        # Set up the sort method combo box
-        self._setup_sort_methods()
+        # # Set up the sort method combo box
+        # self._setup_sort_methods()
 
         # Set up the menu bar
         self._setup_menu_bar()
         
         # Set up Sharktopoda client
         self._setup_sharktopoda_client()
 
@@ -291,14 +293,30 @@
     def _setup_from_settings(self):
         """
         Propagate the settings to the app.
         """
         m3.setup_from_settings()
         sql.connect_from_settings()
 
+    def _sort_widgets(self):
+        """
+        Open the sort dialog and apply a sort method to the rect widgets.
+        """
+        # Show a sort dialog
+        sort_dialog = SortDialog(parent=self)
+        ok = sort_dialog.exec()
+        if not ok:
+            return
+        method = sort_dialog.method
+        if method is None:
+            return
+        
+        self.image_mosaic.sort_rect_widgets(method)
+        self.image_mosaic.render_mosaic()
+
     def _do_query(self):
         """
         Perform a query based on the filter string.
         """
         # Show a query dialog
         constraint_dict = self.query()
         if constraint_dict is None:  # User cancelled, do nothing
@@ -329,16 +347,16 @@
         )
 
         self.image_mosaic.hide_discarded = False
         self.image_mosaic.hide_to_review = False
         self.image_mosaic._hide_labeled = self.ui.hideLabeled.isChecked()
 
         # Render
-        sort_method = self.ui.sortMethod.currentData()
-        self.image_mosaic.sort_rect_widgets(sort_method)
+        # sort_method = self.ui.sortMethod.currentData()
+        # self.image_mosaic.sort_rect_widgets(sort_method)  # TODO replace this logic
         self.image_mosaic.render_mosaic()
 
         # Show some stats about the images and annotations
         self.statusBar().showMessage(
             "Loaded "
             + str(self.image_mosaic.n_images)
             + " images and "
@@ -369,21 +387,21 @@
         self.ui.partComboBox.clear()
         parts = [""] + sorted([p for p in get_kb_parts() if p != ""])
         self.ui.partComboBox.addItems(parts)
         self.ui.partComboBox.completer().setCompletionMode(
             QtWidgets.QCompleter.CompletionMode.PopupCompletion
         )
 
-    def _setup_sort_methods(self):
-        """
-        Populate the sort method combo box
-        """
-        self.ui.sortMethod.clear()
-        for method in ENABLED_SORT_METHODS:
-            self.ui.sortMethod.addItem(method.NAME, userData=method)
+    # def _setup_sort_methods(self):
+    #     """
+    #     Populate the sort method combo box
+    #     """
+    #     self.ui.sortMethod.clear()
+    #     for method in ENABLED_SORT_METHODS:
+    #         self.ui.sortMethod.addItem(method.NAME, userData=method)
 
     def _restore_gui(self):
         """
         Restore window size and splitter states
         """
         finfo = QtCore.QFileInfo(GUI_SETTINGS.fileName())
         if finfo.exists() and finfo.isFile():
@@ -459,15 +477,15 @@
         self.image_mosaic.clear_selected()
 
     @QtCore.pyqtSlot()
     def update_layout(self):
         if not self.loaded:
             return
 
-        method = self.ui.sortMethod.currentData()
+        # method = self.ui.sortMethod.currentData()
         self.image_mosaic.hide_discarded = False
         self.image_mosaic.hide_to_review = False
         self.image_mosaic._hide_labeled = self.ui.hideLabeled.isChecked()
         self.image_mosaic.sort_rect_widgets(method)
         self.image_mosaic.render_mosaic()
 
     @QtCore.pyqtSlot(int)
```

### Comparing `vars_gridview-0.3.0/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.3.1/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.3.1/vars_gridview/ui/QueryDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.3.1/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.3.1/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.3.0/setup.py` & `vars_gridview-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'sharktopoda-client==0.4.0']
 
 entry_points = \
 {'console_scripts': ['vars-gridview = vars_gridview.scripts.run:main']}
 
 setup_kwargs = {
     'name': 'vars-gridview',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.',
     'long_description': '# vars-gridview\n\n**VARS GridView** is a tool for reviewing and correcting VARS localizations in bulk.\n\n[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/downloads/)\n\nAuthors: Kevin Barnard ([kbarnard@mbari.org](mailto:kbarnard@mbari.org)), Paul Roberts ([proberts@mbari.org](mailto:proberts@mbari.org))\n\n---\n\n## Install\n\n### From PyPI\n\nVARS GridView is available on PyPI as `vars-gridview`. To install, run:\n\n```bash\npip install vars-gridview\n```\n\n### From source\n\nThis project is built with [Poetry](https://python-poetry.org/). To install from source, run (in the project root):\n\n```bash\npoetry install\n```\n\n## Run\n\nOnce VARS GridView is installed, you can run it from the command line:\n\n```bash\nvars-gridview\n```\n\nYou will first be prompted to log in. Enter your VARS username and password. \n\n*Note: If you are not using MBARI production VARS, change the "Config server" field to point to your instance of Raziel. This setting is persisted.*\n\n---\n\nCopyright &copy; 2020&ndash;2023 [Monterey Bay Aquarium Research Institute](https://www.mbari.org)',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mbari-org/vars-gridview',
```

### Comparing `vars_gridview-0.3.0/PKG-INFO` & `vars_gridview-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.3.0
+Version: 0.3.1
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
```

