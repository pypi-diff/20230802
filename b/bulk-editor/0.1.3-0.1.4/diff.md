# Comparing `tmp/bulk_editor-0.1.3.tar.gz` & `tmp/bulk_editor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bulk_editor-0.1.3.tar", last modified: Wed Aug  2 09:00:04 2023, max compression
+gzip compressed data, was "dist/bulk_editor-0.1.4.tar", last modified: Wed Aug  2 09:08:53 2023, max compression
```

## Comparing `bulk_editor-0.1.3.tar` & `bulk_editor-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2157 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/PKG-INFO
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulkeditor/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     3859 2023-08-01 11:42:15.000000 bulk_editor-0.1.3/bulkeditor/__init__.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)       10 2023-07-31 08:02:27.000000 bulk_editor-0.1.3/bulkeditor/Certificate.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)    20953 2023-07-31 08:02:27.000000 bulk_editor-0.1.3/bulkeditor/logo.png
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2558 2023-08-02 08:53:22.000000 bulk_editor-0.1.3/bulkeditor/img_to_pdf.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)   167336 2023-07-31 08:02:27.000000 bulk_editor-0.1.3/bulkeditor/Roboto-Bold.ttf
--rw-r--r--   0 harinikeshr   (501) admin       (80)     1070 2023-07-11 07:16:48.000000 bulk_editor-0.1.3/LICENSE
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulk_editor.egg-info/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2157 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulk_editor.egg-info/PKG-INFO
--rw-r--r--   0 harinikeshr   (501) admin       (80)      322 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulk_editor.egg-info/SOURCES.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulk_editor.egg-info/requires.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulk_editor.egg-info/top_level.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/bulk_editor.egg-info/dependency_links.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2336 2023-07-31 08:02:27.000000 bulk_editor-0.1.3/README.md
--rw-r--r--   0 harinikeshr   (501) admin       (80)     4810 2023-08-02 08:58:51.000000 bulk_editor-0.1.3/setup.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-08-02 09:00:04.000000 bulk_editor-0.1.3/setup.cfg
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2157 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/PKG-INFO
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulkeditor/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     6368 2023-08-02 09:08:03.000000 bulk_editor-0.1.4/bulkeditor/__init__.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       10 2023-07-31 08:02:27.000000 bulk_editor-0.1.4/bulkeditor/Certificate.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)    20953 2023-07-31 08:02:27.000000 bulk_editor-0.1.4/bulkeditor/logo.png
+-rw-r--r--   0 harinikeshr   (501) admin       (80)      109 2023-08-02 09:08:05.000000 bulk_editor-0.1.4/bulkeditor/img_to_pdf.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)   167336 2023-07-31 08:02:27.000000 bulk_editor-0.1.4/bulkeditor/Roboto-Bold.ttf
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     1070 2023-07-11 07:16:48.000000 bulk_editor-0.1.4/LICENSE
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulk_editor.egg-info/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2157 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulk_editor.egg-info/PKG-INFO
+-rw-r--r--   0 harinikeshr   (501) admin       (80)      322 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulk_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulk_editor.egg-info/requires.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulk_editor.egg-info/top_level.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/bulk_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2336 2023-07-31 08:02:27.000000 bulk_editor-0.1.4/README.md
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     4810 2023-08-02 09:08:25.000000 bulk_editor-0.1.4/setup.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-08-02 09:08:53.000000 bulk_editor-0.1.4/setup.cfg
```

### Comparing `bulk_editor-0.1.3/PKG-INFO` & `bulk_editor-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk_editor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.1.3/bulkeditor/logo.png` & `bulk_editor-0.1.4/bulkeditor/logo.png`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.1.3/bulkeditor/Roboto-Bold.ttf` & `bulk_editor-0.1.4/bulkeditor/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.1.3/LICENSE` & `bulk_editor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.1.3/bulk_editor.egg-info/PKG-INFO` & `bulk_editor-0.1.4/bulk_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-editor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.1.3/README.md` & `bulk_editor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.1.3/setup.py` & `bulk_editor-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     long_description = fh.read()
 
 # long_description = ""
 # with open("README.md", 'r') as f:
 #   long_description = f.read()
 #   print(long_description)
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.'
 LONG_DESCRIPTION = 'Batch Processing: Our Image Bulk Editor allows you to process multiple certificates or images simultaneously. No need to edit each file individually; simply upload your entire collection, and the tool will automatically apply your customizations to all the files. Custom Text Fields: Effortlessly insert names, dates, or any other custom text onto your certificates or images. Our editor provides intuitive text fields that can be easily filled with the desired information. You can choose from various fonts, sizes, and colors to match your preferences. Dynamic Variables: To further enhance personalization, we offer dynamic variables that automatically populate data across multiple files. For example, if you have a list of names, our tool can dynamically fill in each name in the designated areas, ensuring accuracy and consistency throughout the batch. Easy Alignment and Positioning: Achieve precise placement of text or custom elements on your certificates or images using our user-friendly alignment and positioning tools. You can adjust the position, rotation, and size of the elements to fit your design perfectly. Preview and Quality Control: Before finalizing your edits, our Image Bulk Editor enables you to preview each modified file. This allows you to ensure that the personalized text or customizations are accurately applied to every certificate or image. Additionally, you can compare the original and edited versions side by side to verify the changes. Export Options: Once you are satisfied with the edits, the Image Bulk Editor provides flexible export options. You can choose to save each edited file individually or merge them into a single document or image, making it convenient for distribution or archiving purposes. Time-Saving Efficiency: Image Bulk Editor is designed to streamline your workflow, significantly reducing the time and effort required for editing multiple certificates or images. Whether you are managing a large event, running an educational program, or organizing corporate achievements, our tool empowers you to process bulk customization quickly and accurately.'
 
 # Setting up
 setup(
     include_package_data=True,
     name="bulk_editor",
```

