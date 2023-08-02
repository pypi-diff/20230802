# Comparing `tmp/napari-sam-0.4.8.tar.gz` & `tmp/napari-sam-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.8.tar", last modified: Tue May  9 13:02:31 2023, max compression
+gzip compressed data, was "napari-sam-0.4.9.tar", last modified: Tue May  9 14:32:11 2023, max compression
```

## Comparing `napari-sam-0.4.8.tar` & `napari-sam-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.727481 napari-sam-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 13:02:06.000000 napari-sam-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 13:02:06.000000 napari-sam-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-09 13:02:31.727481 napari-sam-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-09 13:02:06.000000 napari-sam-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-09 13:02:06.000000 napari-sam-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-09 13:02:31.727481 napari-sam-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.723480 napari-sam-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.727481 napari-sam-0.4.8/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66908 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-09 13:02:06.000000 napari-sam-0.4.8/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:02:31.727481 napari-sam-0.4.8/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 13:02:31.000000 napari-sam-0.4.8/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:11.096767 napari-sam-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 14:31:47.000000 napari-sam-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 14:31:47.000000 napari-sam-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-09 14:32:11.096767 napari-sam-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-09 14:31:47.000000 napari-sam-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-09 14:31:47.000000 napari-sam-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-09 14:32:11.100767 napari-sam-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:11.096767 napari-sam-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:11.096767 napari-sam-0.4.9/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-09 14:31:47.000000 napari-sam-0.4.9/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 14:31:47.000000 napari-sam-0.4.9/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66920 2023-05-09 14:31:47.000000 napari-sam-0.4.9/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 14:31:47.000000 napari-sam-0.4.9/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-09 14:31:47.000000 napari-sam-0.4.9/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-09 14:31:47.000000 napari-sam-0.4.9/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:11.096767 napari-sam-0.4.9/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-09 14:32:11.000000 napari-sam-0.4.9/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 14:32:11.000000 napari-sam-0.4.9/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:32:11.000000 napari-sam-0.4.9/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 14:32:11.000000 napari-sam-0.4.9/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 14:32:11.000000 napari-sam-0.4.9/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 14:32:11.000000 napari-sam-0.4.9/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.8/LICENSE` & `napari-sam-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.8/PKG-INFO` & `napari-sam-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.8
+Version: 0.4.9
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

### Comparing `napari-sam-0.4.8/README.md` & `napari-sam-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.8/setup.cfg` & `napari-sam-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.8/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.9/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.8/src/napari_sam/_widget.py` & `napari-sam-0.4.9/src/napari_sam/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,20 +610,20 @@
 
             if self.rb_click.isChecked():
                 self.annotator_mode = AnnotatorMode.CLICK
                 # self.rb_bbox.setEnabled(False)
                 self.rb_auto.setEnabled(False)
                 # self.rb_bbox.setStyleSheet("color: gray")
                 self.rb_auto.setStyleSheet("color: gray")
-            elif self.rb_bbox.isChecked():
-                self.annotator_mode = AnnotatorMode.BBOX
-                self.rb_click.setEnabled(False)
-                self.rb_auto.setEnabled(False)
-                self.rb_click.setStyleSheet("color: gray")
-                self.rb_auto.setStyleSheet("color: gray")
+            # elif self.rb_bbox.isChecked():
+            #     self.annotator_mode = AnnotatorMode.BBOX
+            #     self.rb_click.setEnabled(False)
+            #     self.rb_auto.setEnabled(False)
+            #     self.rb_click.setStyleSheet("color: gray")
+            #     self.rb_auto.setStyleSheet("color: gray")
             elif self.rb_auto.isChecked():
                 self.annotator_mode = AnnotatorMode.AUTO
                 self.rb_click.setEnabled(False)
                 # self.rb_bbox.setEnabled(False)
                 self.rb_click.setStyleSheet("color: gray")
                 # self.rb_bbox.setStyleSheet("color: gray")
             else:
```

### Comparing `napari-sam-0.4.8/src/napari_sam/slicer.py` & `napari-sam-0.4.9/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.8/src/napari_sam/utils.py` & `napari-sam-0.4.9/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.8/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.9/src/napari_sam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.8
+Version: 0.4.9
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

