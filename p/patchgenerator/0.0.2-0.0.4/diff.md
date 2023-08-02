# Comparing `tmp/patchgenerator-0.0.2.tar.gz` & `tmp/patchgenerator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchgenerator-0.0.2.tar", last modified: Sun Jul  2 10:13:05 2023, max compression
+gzip compressed data, was "patchgenerator-0.0.4.tar", last modified: Wed Aug  2 17:25:34 2023, max compression
```

## Comparing `patchgenerator-0.0.2.tar` & `patchgenerator-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 10:13:05.128637 patchgenerator-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:34:11.000000 patchgenerator-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1244 2023-07-02 10:13:05.128637 patchgenerator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-06-30 15:34:11.000000 patchgenerator-0.0.2/README.md
--rw-rw-rw-   0        0        0      733 2023-07-02 10:12:45.000000 patchgenerator-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      786 2023-07-02 10:13:05.130665 patchgenerator-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 10:13:05.111984 patchgenerator-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 10:13:05.116456 patchgenerator-0.0.2/src/patch_indices/
--rw-rw-rw-   0        0        0        0 2023-06-30 15:34:11.000000 patchgenerator-0.0.2/src/patch_indices/__init__.py
--rw-rw-rw-   0        0        0     3019 2023-07-02 07:50:09.000000 patchgenerator-0.0.2/src/patch_indices/patch_indices.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:13:05.120455 patchgenerator-0.0.2/src/patchgenerator.egg-info/
--rw-rw-rw-   0        0        0     1244 2023-07-02 10:13:05.000000 patchgenerator-0.0.2/src/patchgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-02 10:13:05.000000 patchgenerator-0.0.2/src/patchgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 10:13:05.000000 patchgenerator-0.0.2/src/patchgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-02 10:13:05.000000 patchgenerator-0.0.2/src/patchgenerator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 10:13:05.121456 patchgenerator-0.0.2/tests/
--rw-rw-rw-   0        0        0     1442 2023-07-02 07:49:50.000000 patchgenerator-0.0.2/tests/test_patch_indices.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:25:34.061093 patchgenerator-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:34:11.000000 patchgenerator-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1860 2023-08-02 17:25:34.061093 patchgenerator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1113 2023-07-22 12:15:44.000000 patchgenerator-0.0.4/README.md
+-rw-rw-rw-   0        0        0      733 2023-08-02 17:24:03.000000 patchgenerator-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      786 2023-08-02 17:25:34.065360 patchgenerator-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 17:25:34.035694 patchgenerator-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 17:25:34.048141 patchgenerator-0.0.4/src/patch_indices/
+-rw-rw-rw-   0        0        0        0 2023-07-22 12:03:23.000000 patchgenerator-0.0.4/src/patch_indices/__init__.py
+-rw-rw-rw-   0        0        0     4738 2023-08-02 17:22:23.000000 patchgenerator-0.0.4/src/patch_indices/patch_indices.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:25:34.056906 patchgenerator-0.0.4/src/patchgenerator.egg-info/
+-rw-rw-rw-   0        0        0     1860 2023-08-02 17:25:34.000000 patchgenerator-0.0.4/src/patchgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-08-02 17:25:34.000000 patchgenerator-0.0.4/src/patchgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 17:25:34.000000 patchgenerator-0.0.4/src/patchgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-02 17:25:34.000000 patchgenerator-0.0.4/src/patchgenerator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 17:25:34.058579 patchgenerator-0.0.4/tests/
+-rw-rw-rw-   0        0        0     2275 2023-08-02 17:17:50.000000 patchgenerator-0.0.4/tests/test_patch_indices.py
```

### Comparing `patchgenerator-0.0.2/LICENSE.txt` & `patchgenerator-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patchgenerator-0.0.2/PKG-INFO` & `patchgenerator-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchgenerator
-Version: 0.0.2
+Version: 0.0.4
 Summary: `Patchgenerator` is a simple tool to generate array indices, with or without overlap, to create numpy array patches. Only requires python.
 Home-page: https://github.com/earthobserved/patchgenerator
 Author: Earth Observed
 Author-email: EarthObserved <info@earthobserved.com>
 Project-URL: Homepage, https://github.com/earthobserved/patchgenerator
 Project-URL: Bug Tracker, https://github.com/earthobserved/patchgenerator/issues
 Classifier: Programming Language :: Python :: 3
@@ -17,13 +17,29 @@
 # `patchgenerator`
 
 The `patchgenerator` is a simple tool to generate array indices, with or without overlap, to create numpy array patches. Only requires python.
 
 # Example usage:
 
 ```
-from patch_indices import PatchGenerator
+from patch_indices.patch_indices import PatchGenerator
+
 patch_generator = PatchGenerator(100, 80, 10, 20, y_overlap=2, x_overlap=3)
 for patch in patch_generator:
     row_start, cols_start, row_end, cols_end = patch
     print("row_start, cols_start, row_end, cols_end", row_start, cols_start, row_end, cols_end)
 ```
+```
+import numpy as np
+from patch_indices.patch_indices import PatchGenerator
+
+np_array = np.ones((100, 80, 3), dtype=np.uint8)
+y_size, x_size, z_size = np_array.shape
+patch_size_y = 10
+patch_size_x = 20
+
+patch_generator = PatchGenerator(y_size, x_size, patch_size_y, patch_size_x, y_overlap=2, x_overlap=3)
+for patch in patch_generator:
+    row_start, cols_start, row_end, cols_end = patch
+    print("row_start, cols_start, row_end, cols_end", row_start, cols_start, row_end, cols_end)
+    print(np_array[row_start:row_start + row_end, cols_start:cols_start + cols_end, :].shape)
+```
```

### Comparing `patchgenerator-0.0.2/pyproject.toml` & `patchgenerator-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=61']
 build-backend = 'setuptools.build_meta'
 [project]
 name = "patchgenerator"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="EarthObserved", email="info@earthobserved.com" },
 ]
 description = "`Patchgenerator` is a simple tool to generate array indices, with or without overlap, to create numpy array patches. Only requires python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `patchgenerator-0.0.2/setup.cfg` & `patchgenerator-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `patchgenerator-0.0.2/src/patchgenerator.egg-info/PKG-INFO` & `patchgenerator-0.0.4/src/patchgenerator.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchgenerator
-Version: 0.0.2
+Version: 0.0.4
 Summary: `Patchgenerator` is a simple tool to generate array indices, with or without overlap, to create numpy array patches. Only requires python.
 Home-page: https://github.com/earthobserved/patchgenerator
 Author: Earth Observed
 Author-email: EarthObserved <info@earthobserved.com>
 Project-URL: Homepage, https://github.com/earthobserved/patchgenerator
 Project-URL: Bug Tracker, https://github.com/earthobserved/patchgenerator/issues
 Classifier: Programming Language :: Python :: 3
@@ -17,13 +17,29 @@
 # `patchgenerator`
 
 The `patchgenerator` is a simple tool to generate array indices, with or without overlap, to create numpy array patches. Only requires python.
 
 # Example usage:
 
 ```
-from patch_indices import PatchGenerator
+from patch_indices.patch_indices import PatchGenerator
+
 patch_generator = PatchGenerator(100, 80, 10, 20, y_overlap=2, x_overlap=3)
 for patch in patch_generator:
     row_start, cols_start, row_end, cols_end = patch
     print("row_start, cols_start, row_end, cols_end", row_start, cols_start, row_end, cols_end)
 ```
+```
+import numpy as np
+from patch_indices.patch_indices import PatchGenerator
+
+np_array = np.ones((100, 80, 3), dtype=np.uint8)
+y_size, x_size, z_size = np_array.shape
+patch_size_y = 10
+patch_size_x = 20
+
+patch_generator = PatchGenerator(y_size, x_size, patch_size_y, patch_size_x, y_overlap=2, x_overlap=3)
+for patch in patch_generator:
+    row_start, cols_start, row_end, cols_end = patch
+    print("row_start, cols_start, row_end, cols_end", row_start, cols_start, row_end, cols_end)
+    print(np_array[row_start:row_start + row_end, cols_start:cols_start + cols_end, :].shape)
+```
```

### Comparing `patchgenerator-0.0.2/tests/test_patch_indices.py` & `patchgenerator-0.0.4/tests/test_patch_indices.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,38 +6,72 @@
 """
 
 import unittest
 import sys # added!
 sys.path.append("..") # added!
 from src.patch_indices.patch_indices import PatchGenerator
 
-class PatchGeneratorTestCase(unittest.TestCase):
+    
+class TestArrayPatchGenerator(unittest.TestCase):
     def test_patch_generation(self):
-        patch_generator = PatchGenerator(100, 80, 10, 20, y_overlap=2, x_overlap=3)
+        ysize = 1024
+        xsize = 1024
+        y_block_size = 512
+        x_block_size = 512
+        y_overlap = 100
+        x_overlap = 100
 
+        generator = PatchGenerator(ysize, xsize, y_block_size, x_block_size, y_overlap, x_overlap)
+        
         expected_patches = [
-            (0, 0, 20, 10), # First block
-            (0, 7, 20, 10), # Second block with overlap
-            (0, 14, 20, 10), # Third block with overlap
-            (0, 21, 20, 10)  # Fourth block with overlap and adjusted size
+            (0, 0, 512, 512), # First block
+            (412, 0, 512, 512), # Second block with overlap
+            (824, 0, 200, 512), # Third block with overlap
+            (0, 412, 512, 512) # Fourth block with overlap
         ]
 
-        generated_patches = list(patch_generator)[:4]
+        patches = list(generator)[:4]
 
-        self.assertEqual(len(generated_patches), len(expected_patches))
+        self.assertEqual(patches, expected_patches)
 
-        for expected, generated in zip(expected_patches, generated_patches):
-            self.assertEqual(expected, generated)
-    
-            
-    def test_patch_size_exception(self):
-        # Test case where x_block_size is larger than xsize
+    def test_invalid_arguments(self):
+        # Test invalid block size and overlap
+        with self.assertRaises(ValueError):
+            PatchGenerator(10, 10, 0, 4)
+
+        with self.assertRaises(ValueError):
+            PatchGenerator(10, 10, 4, 0)
+
+        with self.assertRaises(ValueError):
+            PatchGenerator(10, 10, 4, 5, y_overlap=5)
+
+        with self.assertRaises(ValueError):
+            PatchGenerator(10, 10, 4, 5, x_overlap=6)
+
+        # Test block size larger than array size
         with self.assertRaises(ValueError):
-            generator1 = PatchGenerator(100, 80, 120, 20, y_overlap=2, x_overlap=3)
+            PatchGenerator(10, 10, 12, 5)
 
-        # Test case where y_block_size is larger than ysize
         with self.assertRaises(ValueError):
-            generator2 = PatchGenerator(100, 80, 10, 100, y_overlap=2, x_overlap=3)
+            PatchGenerator(10, 10, 5, 12)
 
+    def test_empty_array(self):
+        # Test empty array case
+        with self.assertRaises(ValueError):
+            PatchGenerator(0, 0, 3, 3)
+
+    def test_single_patch(self):
+        # Test case where the array size is equal to the block size
+        ysize = 4
+        xsize = 4
+        y_block_size = 4
+        x_block_size = 4
+
+        generator = PatchGenerator(ysize, xsize, y_block_size, x_block_size)
+        patches = list(generator)
+        expected_patches = [(0, 0, 4, 4)]
+        self.assertEqual(patches, expected_patches)
+
+        
+        
 if __name__ == '__main__':
     unittest.main()
-
```

