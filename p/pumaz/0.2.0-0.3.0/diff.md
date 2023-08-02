# Comparing `tmp/pumaz-0.2.0.tar.gz` & `tmp/pumaz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pumaz-0.2.0.tar", last modified: Thu Jul 27 08:18:30 2023, max compression
+gzip compressed data, was "pumaz-0.3.0.tar", last modified: Wed Aug  2 14:18:03 2023, max compression
```

## Comparing `pumaz-0.2.0.tar` & `pumaz-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:18:30.452992 pumaz-0.2.0/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7084 2023-07-27 08:18:30.452992 pumaz-0.2.0/PKG-INFO
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     5833 2023-07-27 07:34:55.000000 pumaz-0.2.0/README.md
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:18:30.452992 pumaz-0.2.0/pumaz/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      305 2023-07-07 18:44:14.000000 pumaz-0.2.0/pumaz/__init__.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1924 2023-07-27 08:14:47.000000 pumaz-0.2.0/pumaz/constants.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     3526 2023-07-08 08:44:00.000000 pumaz-0.2.0/pumaz/display.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     4197 2023-07-07 20:08:58.000000 pumaz-0.2.0/pumaz/download.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     4281 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/file_utilities.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7661 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/image_conversion.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)    14300 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/image_processing.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     2306 2023-07-08 08:25:48.000000 pumaz-0.2.0/pumaz/input_validation.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     5275 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/pumaz.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1688 2023-07-04 19:36:14.000000 pumaz-0.2.0/pumaz/resources.py
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:18:30.452992 pumaz-0.2.0/pumaz.egg-info/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7084 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/PKG-INFO
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      402 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/SOURCES.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/dependency_links.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)       44 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/entry_points.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      235 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/requires.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)        6 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/top_level.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-07-27 08:18:30.452992 pumaz-0.2.0/setup.cfg
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1977 2023-07-27 08:17:33.000000 pumaz-0.2.0/setup.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2023-08-02 14:18:03.538448 pumaz-0.3.0/
+-rw-r--r--   0 x          (501) staff       (20)     7084 2023-08-02 14:18:03.538298 pumaz-0.3.0/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)     5833 2023-08-02 14:13:35.000000 pumaz-0.3.0/README.md
+drwxr-xr-x   0 x          (501) staff       (20)        0 2023-08-02 14:18:03.537282 pumaz-0.3.0/pumaz/
+-rw-r--r--   0 x          (501) staff       (20)      305 2023-07-07 10:51:04.000000 pumaz-0.3.0/pumaz/__init__.py
+-rw-r--r--   0 x          (501) staff       (20)     2146 2023-08-02 14:13:35.000000 pumaz-0.3.0/pumaz/constants.py
+-rw-r--r--   0 x          (501) staff       (20)     3526 2023-07-19 15:20:58.000000 pumaz-0.3.0/pumaz/display.py
+-rw-r--r--   0 x          (501) staff       (20)     4197 2023-07-19 15:20:58.000000 pumaz-0.3.0/pumaz/download.py
+-rw-r--r--   0 x          (501) staff       (20)     4281 2023-07-19 15:21:10.000000 pumaz-0.3.0/pumaz/file_utilities.py
+-rw-r--r--   0 x          (501) staff       (20)     7661 2023-07-19 15:21:11.000000 pumaz-0.3.0/pumaz/image_conversion.py
+-rw-r--r--   0 x          (501) staff       (20)    16076 2023-08-02 14:13:35.000000 pumaz-0.3.0/pumaz/image_processing.py
+-rw-r--r--   0 x          (501) staff       (20)     2306 2023-07-19 15:20:58.000000 pumaz-0.3.0/pumaz/input_validation.py
+-rw-r--r--   0 x          (501) staff       (20)     5295 2023-08-02 14:13:35.000000 pumaz-0.3.0/pumaz/pumaz.py
+-rw-r--r--   0 x          (501) staff       (20)     1688 2023-07-07 08:51:22.000000 pumaz-0.3.0/pumaz/resources.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2023-08-02 14:18:03.538042 pumaz-0.3.0/pumaz.egg-info/
+-rw-r--r--   0 x          (501) staff       (20)     7084 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      402 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/SOURCES.txt
+-rw-r--r--   0 x          (501) staff       (20)        1 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/dependency_links.txt
+-rw-r--r--   0 x          (501) staff       (20)       44 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/entry_points.txt
+-rw-r--r--   0 x          (501) staff       (20)      242 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/requires.txt
+-rw-r--r--   0 x          (501) staff       (20)        6 2023-08-02 14:18:03.000000 pumaz-0.3.0/pumaz.egg-info/top_level.txt
+-rw-r--r--   0 x          (501) staff       (20)       38 2023-08-02 14:18:03.538518 pumaz-0.3.0/setup.cfg
+-rw-r--r--   0 x          (501) staff       (20)     1996 2023-08-02 14:13:35.000000 pumaz-0.3.0/setup.py
```

### Comparing `pumaz-0.2.0/PKG-INFO` & `pumaz-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 0.2.0
+Version: 0.3.0
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
 Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Platform: UNKNOWN
```

### Comparing `pumaz-0.2.0/README.md` & `pumaz-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz/constants.py` & `pumaz-0.3.0/pumaz/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,17 +47,30 @@
 MODALITIES_PREFIX = ['PT_ for PET', 'CT_ for CT']
 
 # FILE NAMES
 
 RESAMPLED_PREFIX = 'resampled_'
 ALIGNED_PREFIX = 'aligned_'
 
+# MOOSE PARAMETERS
+
+MOOSE_MODEL = "clin_ct_body"
+MOOSE_PREFIX = 'CT_Body_'
+MOOSE_LABEL_INDEX = {
+        1: "Legs",
+        2: "Body",
+        3: "Head",
+        4: "Arms"
+    }
+ACCELERATOR = 'cuda'
+
 # FOLDER NAMES
 
 PUMA_WORKING_FOLDER = 'PUMAZ-V01' + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 TRANSFORMS_FOLDER = 'transforms'
 ALIGNED_CT_FOLDER = 'aligned_CT'
 ALIGNED_PET_FOLDER = 'aligned_PT'
+MASK_FOLDER = 'masks'
 
 # HYPERPARAMETERS
 
 MULTI_RESOLUTION_SCHEME = '100x25x10'
```

### Comparing `pumaz-0.2.0/pumaz/display.py` & `pumaz-0.3.0/pumaz/display.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz/download.py` & `pumaz-0.3.0/pumaz/download.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz/file_utilities.py` & `pumaz-0.3.0/pumaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz/image_conversion.py` & `pumaz-0.3.0/pumaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz/image_processing.py` & `pumaz-0.3.0/pumaz/image_processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the pumaz to perform image conversion.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import SimpleITK as sitk
+import numpy as np
 import glob
 from pumaz import constants
 from pumaz.constants import GREEDY_PATH
 from mpire import WorkerPool
 import multiprocessing
 from rich.progress import Progress
 from pumaz import file_utilities
@@ -29,14 +30,16 @@
 import os
 import pathlib
 import subprocess
 import logging
 import sys
 import re
 from rich.progress import track
+from moosez import moose
+import nibabel as nib
 
 
 def reslice_identity(reference_image: sitk.Image, moving_image: sitk.Image,
                      output_image_path: str = None, is_label_image: bool = False) -> sitk.Image:
     """
     Reslice an image to the same space as another image
     :param reference_image: The reference image
@@ -78,14 +81,34 @@
 
 def copy_and_rename_file(src, dst, subdir):
     file_utilities.copy_file(src, dst)
     new_file = os.path.join(dst, os.path.basename(subdir) + '_' + os.path.basename(src))
     os.rename(os.path.join(dst, os.path.basename(src)), new_file)
 
 
+def change_mask_labels(mask_file: str, label_map: dict, excluded_labels: list):
+    # Load the image
+    img = nib.load(mask_file)
+
+    # Get the image data (returns a numpy array)
+    data = img.get_fdata()
+
+    # Prepare labels for modification
+    excluded_indices = [idx for idx, lbl in label_map.items() if lbl in excluded_labels]
+    other_indices = [idx for idx, lbl in label_map.items() if lbl not in excluded_labels]
+
+    # Set the labels
+    data[np.isin(data, excluded_indices)] = 0
+    data[np.isin(data, other_indices)] = 1
+
+    # Save the modified image
+    new_img = nib.Nifti1Image(data, img.affine, img.header)
+    nib.save(new_img, mask_file)
+
+
 def preprocess(puma_compliant_subjects: list, num_workers: int = None):
     """
     Preprocesses the images in the subject directory
     :param puma_compliant_subjects: The puma compliant subjects
     :param num_workers: The number of worker processes for parallel processing
     """
     if num_workers is None:
@@ -105,14 +128,15 @@
     parent_dir = os.path.dirname(puma_compliant_subjects[0])
     puma_working_dir = os.path.join(parent_dir, constants.PUMA_WORKING_FOLDER)
     file_utilities.create_directory(puma_working_dir)
 
     # create CT and PET folders
     ct_dir = os.path.join(puma_working_dir, constants.MODALITIES[1])
     pt_dir = os.path.join(puma_working_dir, constants.MODALITIES[0])
+    mask_dir = os.path.join(puma_working_dir, constants.MASK_FOLDER)
     file_utilities.create_directory(ct_dir)
     file_utilities.create_directory(pt_dir)
 
     index = 0
     # Move and rename files in parallel
     with ThreadPoolExecutor(max_workers=num_workers) as executor:
         for subdir in puma_compliant_subjects:
@@ -126,20 +150,32 @@
             new_pt_file = re.sub(r'PET_', f'PET_{index}_', pt_file[0])
             # rename the actual file
             os.rename(pt_file[0], new_pt_file)
 
             index += 1
             executor.submit(copy_and_rename_file, new_pt_file, pt_dir, subdir)
 
-    return puma_working_dir, ct_dir, pt_dir
+    # Run moosez to get the masks
+
+    moose(constants.MOOSE_MODEL, ct_dir, mask_dir, constants.ACCELERATOR)
+
+    # remove the prefix from the mask files
+
+    for mask_file in glob.glob(os.path.join(mask_dir, constants.MOOSE_PREFIX + '*')):
+        new_mask_file = re.sub(rf'{constants.MOOSE_PREFIX}', '', mask_file)
+        os.rename(mask_file, new_mask_file)
+        change_mask_labels(new_mask_file, constants.MOOSE_LABEL_INDEX, ["Arms"])
+
+    return puma_working_dir, ct_dir, pt_dir, mask_dir
 
 
 class ImageRegistration:
-    def __init__(self, fixed_img: str, multi_resolution_iterations: str):
+    def __init__(self, fixed_img: str, multi_resolution_iterations: str, fixed_mask: str = None):
         self.fixed_img = fixed_img
+        self.fixed_mask = fixed_mask
         self.multi_resolution_iterations = multi_resolution_iterations
         self.moving_img = None
         self.transform_files = None
 
     def set_moving_image(self, moving_img: str, update_transforms: bool = True):
         self.moving_img = moving_img
         if update_transforms:
@@ -149,38 +185,41 @@
                 'rigid': os.path.join(out_dir, f"{moving_img_filename}_rigid.mat"),
                 'affine': os.path.join(out_dir, f"{moving_img_filename}_affine.mat"),
                 'warp': os.path.join(out_dir, f"{moving_img_filename}_warp.nii.gz"),
                 'inverse_warp': os.path.join(out_dir, f"{moving_img_filename}_inverse_warp.nii.gz")
             }
 
     def rigid(self) -> str:
-        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} -ia-image" \
-                     f"-centers -dof 6 -o {re.escape(self.transform_files['rigid'])} -n {self.multi_resolution_iterations} -m " \
-                     f"SSD"
+        mask_cmd = f"-gm {re.escape(self.fixed_mask)}" if self.fixed_mask else ""
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} " \
+                     f"{mask_cmd} -ia-image-centers -dof 6 -o {re.escape(self.transform_files['rigid'])} " \
+                     f"-n {self.multi_resolution_iterations} -m SSD"
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
         logging.info(
             f"Rigid alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} | Aligned image: "
             f"moco-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['rigid']).name}")
         return self.transform_files['rigid']
 
     def affine(self) -> str:
-        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} -ia-image" \
-                     f"-centers -dof 12 -o {re.escape(self.transform_files['affine'])} -n {self.multi_resolution_iterations} " \
-                     f"-m SSD"
+        mask_cmd = f"-gm {re.escape(self.fixed_mask)}" if self.fixed_mask else ""
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} " \
+                     f"{mask_cmd} -ia-image-centers -dof 12 -o {re.escape(self.transform_files['affine'])} " \
+                     f"-n {self.multi_resolution_iterations} -m SSD"
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
         logging.info(
             f"Affine alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} |"
-            f" Aligned image: mock-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['affine']).name}")
+            f" Aligned image: moco-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['affine']).name}")
         return self.transform_files['affine']
 
     def deformable(self) -> tuple:
         self.rigid()
+        mask_cmd = f"-gm {re.escape(self.fixed_mask)}" if self.fixed_mask else ""
         cmd_to_run = f"{GREEDY_PATH} -d 3 -m SSD -i {re.escape(self.fixed_img)} {re.escape(self.moving_img)} " \
-                     f"-it {re.escape(self.transform_files['rigid'])} -o {re.escape(self.transform_files['warp'])} -oinv" \
-                     f" {re.escape(self.transform_files['inverse_warp'])} -sv -n {self.multi_resolution_iterations}"
+                     f"{mask_cmd} -it {re.escape(self.transform_files['rigid'])} -o {re.escape(self.transform_files['warp'])} " \
+                     f"-oinv {re.escape(self.transform_files['inverse_warp'])} -sv -n {self.multi_resolution_iterations}"
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
         logging.info(
             f"Deformable alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} | "
             f"Aligned image: moco-{pathlib.Path(self.moving_img).name} | "
             f"Initial alignment:{pathlib.Path(self.transform_files['rigid']).name}"
             f" | warp file: {pathlib.Path(self.transform_files['warp']).name}")
         return self.transform_files['rigid'], self.transform_files['warp'], self.transform_files['inverse_warp']
@@ -214,25 +253,29 @@
         if segmentation and resampled_seg:
             cmd += f" -ri LABEL 0.2vox -rm {re.escape(segmentation)} {re.escape(resampled_seg)}"
         for transform_file in transform_files:
             cmd += f" -r {re.escape(transform_file)}"
         return cmd
 
 
-def align(puma_working_dir: str, ct_dir: str, pt_dir: str):
+def align(puma_working_dir: str, ct_dir: str, pt_dir: str, mask_dir: str):
+
     ct_files = sorted(glob.glob(os.path.join(ct_dir, '*.nii*')))
+
     reference_image = ct_files[0]
+    fixed_mask = glob.glob(os.path.join(mask_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0]
     moving_images = ct_files[1:]
 
     with Progress() as progress:
         task = progress.add_task("[cyan] Aligning CT and PT images to a common frame ", total=len(moving_images))
 
         for moving_image in moving_images:
             aligner = ImageRegistration(fixed_img=reference_image,
-                                        multi_resolution_iterations=constants.MULTI_RESOLUTION_SCHEME)
+                                        multi_resolution_iterations=constants.MULTI_RESOLUTION_SCHEME,
+                                        fixed_mask=fixed_mask)
             aligner.set_moving_image(moving_image)
             aligner.registration('deformable')
             aligner.resample(resampled_moving_img=os.path.join(puma_working_dir, constants.ALIGNED_PREFIX +
                                                                os.path.basename(moving_image)),
                              registration_type='deformable')
             progress.update(task, advance=1)
             pet_image = glob.glob(os.path.join(pt_dir, os.path.basename(moving_image).split('_')[0] + '*.nii*'))[0]
@@ -260,24 +303,25 @@
         aligned_ct_files = sorted(glob.glob(os.path.join(puma_working_dir, constants.ALIGNED_PREFIX + '*CT*.nii*')))
         for aligned_ct_file in aligned_ct_files:
             file_utilities.move_file(aligned_ct_file, aligned_ct_dir)
         # copy the reference ct file to the aligned_ct_dir and add an aligned prefix to the copied file
         file_utilities.copy_file(reference_image, os.path.join(aligned_ct_dir, constants.ALIGNED_PREFIX +
                                                                os.path.basename(reference_image)))
 
-
         # move the aligned PET files to a new folder called aligned_PET, this is stored in the puma_working_dir
         aligned_pet_dir = os.path.join(puma_working_dir, constants.ALIGNED_PET_FOLDER)
         file_utilities.create_directory(aligned_pet_dir)
         # get aligned pet files using glob by looking for keyword 'aligned'
         aligned_pet_files = sorted(
             glob.glob(os.path.join(puma_working_dir, constants.ALIGNED_PREFIX + '*PET*.nii*')))
         for aligned_pet_file in aligned_pet_files:
             file_utilities.move_file(aligned_pet_file, aligned_pet_dir)
         # copy the pet file corresponding to the reference ct file to the aligned_pet_dir and add an aligned prefix
         # to the copied file
-        file_utilities.copy_file(glob.glob(os.path.join(pt_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0],
-                                    os.path.join(aligned_pet_dir, constants.ALIGNED_PREFIX +
-                                                    os.path.basename(glob.glob(os.path.join(pt_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0])))
+        file_utilities.copy_file(
+            glob.glob(os.path.join(pt_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0],
+            os.path.join(aligned_pet_dir, constants.ALIGNED_PREFIX +
+                         os.path.basename(glob.glob(
+                             os.path.join(pt_dir, os.path.basename(reference_image).split('_')[0] + '*.nii*'))[0])))
```

### Comparing `pumaz-0.2.0/pumaz/input_validation.py` & `pumaz-0.3.0/pumaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz/pumaz.py` & `pumaz-0.3.0/pumaz/pumaz.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     start_time = time.time()
     print('')
     print(f'{constants.ANSI_VIOLET} {emoji.emojize(":rocket:")} RUNNING PREPROCESSING AND REGISTRATION PIPELINE:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
     logging.info(' RUNNING PREPROCESSING AND REGISTRATION PIPELINE:')
     logging.info(' ')
-    puma_dir, ct_dir, pt_dir = image_processing.preprocess(puma_compliant_subjects)
-    image_processing.align(puma_dir, ct_dir, pt_dir)
+    puma_dir, ct_dir, pt_dir, mask_dir = image_processing.preprocess(puma_compliant_subjects)
+    image_processing.align(puma_dir, ct_dir, pt_dir, mask_dir)
     end_time = time.time()
     elapsed_time = end_time - start_time
     # show elapsed time in minutes and round it to 2 decimal places
     elapsed_time = round(elapsed_time / 60, 2)
     print(f'{constants.ANSI_GREEN} {emoji.emojize(":hourglass_done:")} Preprocessing and registration complete. Elapsed time: {elapsed_time} minutes!')
```

### Comparing `pumaz-0.2.0/pumaz/resources.py` & `pumaz-0.3.0/pumaz/resources.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.2.0/pumaz.egg-info/PKG-INFO` & `pumaz-0.3.0/pumaz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 0.2.0
+Version: 0.3.0
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
 Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Platform: UNKNOWN
```

### Comparing `pumaz-0.2.0/setup.py` & `pumaz-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pumaz',
-    version='0.2.0',
+    version='0.3.0',
     author='Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar',
     author_email='Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at',
     description='PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.',
     python_requires='>=3.9',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/QIMP-Team/PUMA',
@@ -39,15 +39,16 @@
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
         'rich',
         'pandas',
         'dicom2nifti~=2.4.8',
-        'requests'
+        'requests',
+        'moosez'
     ],
     entry_points={
         'console_scripts': [
             'pumaz=pumaz.pumaz:main',
         ],
     },
-)
+)
```

