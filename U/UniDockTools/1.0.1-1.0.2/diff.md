# Comparing `tmp/UniDockTools-1.0.1.tar.gz` & `tmp/UniDockTools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniDockTools-1.0.1.tar", last modified: Wed Aug  2 03:22:25 2023, max compression
+gzip compressed data, was "UniDockTools-1.0.2.tar", last modified: Wed Aug  2 07:39:54 2023, max compression
```

## Comparing `UniDockTools-1.0.1.tar` & `UniDockTools-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:25.036104 UniDockTools-1.0.1/
--rw-r--r--   0 4294967294 4294967294     1063 2023-08-02 02:58:30.000000 UniDockTools-1.0.1/LICENSE
--rw-r--r--   0 4294967294 4294967294      253 2023-08-02 03:22:25.028379 UniDockTools-1.0.1/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      880 2023-08-02 02:58:30.000000 UniDockTools-1.0.1/README.md
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:24.775335 UniDockTools-1.0.1/UniDockTools/
--rw-r--r--   0 4294967294 4294967294       28 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/__init__.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:25.003373 UniDockTools-1.0.1/UniDockTools/ligandPrepare/
--rw-r--r--   0 4294967294 4294967294       92 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/__init__.py
--rw-r--r--   0 4294967294 4294967294     2951 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/atom_type.py
--rw-r--r--   0 4294967294 4294967294      924 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/rotatable_bond.py
--rw-r--r--   0 4294967294 4294967294    19674 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/topology_builder.py
--rw-r--r--   0 4294967294 4294967294     4987 2023-08-02 02:58:31.000000 UniDockTools-1.0.1/UniDockTools/ligandPrepare/utils.py
--rw-r--r--   0 4294967294 4294967294    13477 2023-08-02 03:16:24.000000 UniDockTools-1.0.1/UniDockTools/unidock.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-08-02 03:22:24.900167 UniDockTools-1.0.1/UniDockTools.egg-info/
--rw-r--r--   0 4294967294 4294967294      253 2023-08-02 03:22:23.000000 UniDockTools-1.0.1/UniDockTools.egg-info/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      500 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/SOURCES.txt
--rw-r--r--   0 4294967294 4294967294        1 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/dependency_links.txt
--rw-r--r--   0 4294967294 4294967294       54 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/entry_points.txt
--rw-r--r--   0 4294967294 4294967294       15 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/requires.txt
--rw-r--r--   0 4294967294 4294967294       13 2023-08-02 03:22:24.000000 UniDockTools-1.0.1/UniDockTools.egg-info/top_level.txt
--rw-r--r--   0 4294967294 4294967294      565 2023-08-02 03:22:21.000000 UniDockTools-1.0.1/setpu.py
--rw-r--r--   0 4294967294 4294967294       38 2023-08-02 03:22:25.040091 UniDockTools-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.244777 UniDockTools-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      230 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      880 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/UniDock/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/UniDock/ligandPrepare/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/atom_type.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/rotatable_bond.py
+-rw-r--r--   0 root         (0) root         (0)    19659 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/topology_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/ligandPrepare/utils.py
+-rw-r--r--   0 root         (0) root         (0)    13395 2023-08-02 07:12:43.000000 UniDockTools-1.0.2/UniDock/unidock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:39:54.240777 UniDockTools-1.0.2/UniDockTools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      465 2023-08-02 07:39:54.000000 UniDockTools-1.0.2/UniDockTools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-02 07:39:53.000000 UniDockTools-1.0.2/UniDockTools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-02 07:39:54.000000 UniDockTools-1.0.2/UniDockTools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      570 2023-08-02 07:38:46.000000 UniDockTools-1.0.2/setpu.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:39:54.244777 UniDockTools-1.0.2/setup.cfg
```

### Comparing `UniDockTools-1.0.1/LICENSE` & `UniDockTools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.1/README.md` & `UniDockTools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.1/UniDockTools/ligandPrepare/atom_type.py` & `UniDockTools-1.0.2/UniDock/ligandPrepare/atom_type.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.1/UniDockTools/ligandPrepare/rotatable_bond.py` & `UniDockTools-1.0.2/UniDock/ligandPrepare/rotatable_bond.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.1/UniDockTools/ligandPrepare/topology_builder.py` & `UniDockTools-1.0.2/UniDock/ligandPrepare/topology_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from concurrent.futures import ThreadPoolExecutor
 
 from rdkit import Chem
 from rdkit.Chem import GetMolFrags, FragmentOnBonds
 from rdkit.Chem.rdPartialCharges import ComputeGasteigerCharges
 
-from UniDockTools.ligandPrepare.atom_type import AtomType
-from UniDockTools.ligandPrepare.rotatable_bond import RotatableBond
-from UniDockTools.ligandPrepare import utils
+from UniDock.ligandPrepare.atom_type import AtomType
+from UniDock.ligandPrepare.rotatable_bond import RotatableBond
+from UniDock.ligandPrepare import utils
 
 class TopologyBuilder(object):
     def __init__(self,
                  ligand_sdf_file_name,
                  working_dir_name='.'):
 
         self.ligand_sdf_file_name = ligand_sdf_file_name
```

### Comparing `UniDockTools-1.0.1/UniDockTools/ligandPrepare/utils.py` & `UniDockTools-1.0.2/UniDock/ligandPrepare/utils.py`

 * *Files identical despite different names*

### Comparing `UniDockTools-1.0.1/UniDockTools/unidock.py` & `UniDockTools-1.0.2/UniDock/unidock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-from UniDockTools.ligandPrepare import prepare_ligands
+from UniDock.ligandPrepare import prepare_ligands
 import os, shutil
 import subprocess
 import glob
 import argparse
 
 from rdkit import Chem
 
 
 class UniDock():
-    def __init__(self, receptor:str, scoring:str='vina', output_dir:str='./docking_results'):
+    def __init__(self, receptor:str, scoring:str='vina', output_dir:str='./docking_results', processing_unit:str='gpu'):
         """
         Initialize the UniDock class with the given parameters.
 
         :param scoring: Docking scoring function. Options: 'vina', 'vinardo', 'gnina'. Default: 'vina'.
         :param output_dir: Directory where the docking results will be saved. Default: './docking_results'.
+        :param processing_unit: Processing unit to be used: 'gpu' or 'cpu'. Default: 'gpu'.
         """
         if scoring in ['vina', 'vinardo']:
             self.scoring = scoring
             self.rescoring = None
         elif scoring in ['gnina']:
             self.scoring = 'vina'
             self.rescoring = scoring
 
         self.receptor = receptor
         self.output_dir = output_dir
+        self.processing_unit = processing_unit
         self.ligand_input_method = ["ligand", "batch", "gpu_batch", "ligand_index"]
 
         self.command_scoring = '--scoring  %s'%self.scoring
         self.command_ligand = ''
 
         # delete output directory if it already exists
         if os.path.exists(self.output_dir) and os.path.isdir(self.output_dir):
             shutil.rmtree(self.output_dir)
-        os.makedirs(self.output_dir, exist_ok=True)
-
-        self.ligands_prepared_dir = "%s/ligands_prepared"%self.output_dir
-        os.makedirs(self.ligands_prepared_dir, exist_ok=True)
+        os.makedirs(output_dir, exist_ok=True)
 
     def set_receptor(self, receptor:str):
         """
         Set the receptor file for the docking.
 
         :param receptor: Path to the receptor file (PDBQT format).
         """
@@ -64,22 +63,22 @@
             if format == "sdf":
                 self.SDF.append(ligand)
             elif format == "pdbqt":
                 self.PDBQT.append(ligand)
 
         if len(self.SDF) > 0:
             print("Preparing ligand file...")
-            self.ligands = prepare_ligands(self.SDF, output_dir=self.ligands_prepared_dir) + self.PDBQT
+            self.ligands = prepare_ligands(self.SDF) + self.PDBQT
         else:
             self.ligands = self.PDBQT
         
         ligand_prepared_index_file = "%s/ligands.dat"%self.output_dir
         with open(ligand_prepared_index_file, 'w') as f:
             for ligand in self.ligands:
-                f.write("%s\n"%ligand)
+                f.write(ligand)
 
         self.command_ligand = '--ligand_index %s'%(ligand_prepared_index_file)
     
     def set_gpu_batch(self, ligands:list):
         """
         Set the ligands GPU batch for the docking.
 
@@ -94,15 +93,15 @@
             if format == "sdf":
                 self.SDF.append(ligand)
             elif format == "pdbqt":
                 self.PDBQT.append(ligand)
 
         if len(self.SDF) > 0:
             print("Preparing ligand file...")
-            self.ligands = prepare_ligands(self.SDF, output_dir=self.ligands_prepared_dir) + self.PDBQT
+            self.ligands = prepare_ligands(self.SDF) + self.PDBQT
         else:
             self.ligands = self.PDBQT
         
         self.command_ligand = '--gpu_batch %s'%(" ".join(self.ligands))
 
     def set_ligand(self, ligand:str):
         """
@@ -112,19 +111,19 @@
         :param need_prepare: Whether the ligands need to be prepared. Default: True.
         """
         self.PDBQT = []
         self.SDF = []
         basename =  os.path.basename(ligand)
         format = basename.split('.')[-1]
         if format == "sdf":
-            print("Preparing ligand file...")
-            self.ligands = prepare_ligands([ligand], output_dir=self.ligands_prepared_dir)
+            self.ligands = prepare_ligands([ligand])
         elif format == "pdbqt":
             self.ligands = [ligand]
         
+        self.processing_unit = 'cpu'
         self.command_ligand = '--ligand %s'%self.ligands[0]
             
     def set_batch(self, ligands:list):
         """
         Set the ligands batch for the docking.
 
         :param ligandv: Path to the ligand index file.
@@ -138,18 +137,19 @@
             if format == "sdf":
                 self.SDF.append(ligand)
             elif format == "pdbqt":
                 self.PDBQT.append(ligand)
 
         if len(self.SDF) > 0:
             print("Preparing ligand file...")
-            self.ligands = prepare_ligands(self.SDF, output_dir=self.ligands_prepared_dir) + self.PDBQT
+            self.ligands = prepare_ligands(self.SDF) + self.PDBQT
         else:
             self.ligands = self.PDBQT
 
+        self.processing_unit = 'cpu'
         self.command_ligand = '--batch %s'%(" ".join(self.ligands))
 
     def set_rescoring(self, rescoring:str):
         """
         Set the rescoring function for the docking.
 
         :param rescoring: Rescoring function. Options: 'gnina'. 
@@ -211,15 +211,15 @@
                     self.command_line += f"--{arg} {value} "
                 else:
                     raise ValueError(f"Unhandled value type for argument {arg}: {type(value)}")
         self.command_line = self.command_line.strip()
     
     def _check_args_and_return(self, args):
         assigned_properties = [prop for prop in self.ligand_input_method if getattr(args, prop, None) is not None]
-        #print([getattr(args, prop)for prop in self.ligand_input_method if getattr(args, prop, None) is not None])
+        print([getattr(args, prop)for prop in self.ligand_input_method if getattr(args, prop, None) is not None])
         
         if len(assigned_properties) != 1:
             raise ValueError("Exactly one argument must be assigned a value.")
         return assigned_properties[0]
 
     def _get_config(self, args):
         self._recreate_command_line(args)
@@ -277,14 +277,15 @@
     parser.add_argument("--search_mode", type=str, default="balance", help="search mode of vina (fast, balance, detail), using recommended settings of exhaustiveness and search steps; the higher the computational complexity, the higher the accuracy, but the larger the computational cost")
 
     args = parser.parse_args()
 
     unidock = UniDock(args.receptor, args.scoring, args.dir)
 
     ligand_input_method = unidock._check_args_and_return(args)
+    print(ligand_input_method)
     if ligand_input_method == "ligand":
         unidock.set_ligand(args.ligand)
     elif ligand_input_method == "batch":
         unidock.set_batch(args.batch)
     elif ligand_input_method == "gpu_batch":
         unidock.set_gpu_batch(args.gpu_batch)
     elif ligand_input_method == "ligand_index":
```

