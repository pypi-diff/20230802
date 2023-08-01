# Comparing `tmp/panda_utils-1.4.4.tar.gz` & `tmp/panda_utils-1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.4.4.tar", last modified: Mon Jul 31 21:46:45 2023, max compression
+gzip compressed data, was "panda_utils-1.5b1.tar", last modified: Tue Aug  1 22:44:25 2023, max compression
```

## Comparing `panda_utils-1.4.4.tar` & `panda_utils-1.5b1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.646411 panda_utils-1.4.4/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.4/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-31 21:46:45.646411 panda_utils-1.4.4/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.4/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.4/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.4/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.4/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.4/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.4.4/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.4.4/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15470 2023-07-31 21:33:06.000000 panda_utils-1.4.4/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.4/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.4/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/blender/export_glb.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1797 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/blender/export_with_yabee.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.4/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.646411 panda_utils-1.4.4/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.4/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.4.4/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.646411 panda_utils-1.4.4/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.4/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.4/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.4/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.4/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.4/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.4/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.4/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-31 21:46:34.000000 panda_utils-1.4.4/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.4/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-31 21:46:45.646411 panda_utils-1.4.4/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.5b1/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-01 22:44:25.769596 panda_utils-1.5b1/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.5b1/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.5b1/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.766262 panda_utils-1.5b1/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b1/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.5b1/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.5b1/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.5b1/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.5b1/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.5b1/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    16004 2023-08-01 22:32:42.000000 panda_utils-1.5b1/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.5b1/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.5b1/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.5b1/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2025 2023-08-01 22:08:01.000000 panda_utils-1.5b1/panda_utils/blender/export_with_yabee.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.5b1/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.5b1/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.5b1/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-08-01 22:33:37.000000 panda_utils-1.5b1/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.5b1/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.769596 panda_utils-1.5b1/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b1/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.5b1/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.5b1/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.5b1/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.5b1/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.5b1/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.5b1/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-01 22:44:25.766262 panda_utils-1.5b1/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-08-01 22:44:25.000000 panda_utils-1.5b1/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-08-01 22:44:06.000000 panda_utils-1.5b1/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.5b1/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-08-01 22:44:25.769596 panda_utils-1.5b1/setup.cfg
```

### Comparing `panda_utils-1.4.4/LICENSE` & `panda_utils-1.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/PKG-INFO` & `panda_utils-1.5b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.4.4
+Version: 1.5b1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.4/README.md` & `panda_utils-1.5b1/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/__main__.py` & `panda_utils-1.5b1/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.5b1/panda_utils/assetpipeline/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/assetpipeline/misc.py` & `panda_utils-1.5b1/panda_utils/assetpipeline/misc.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/assetpipeline/models.py` & `panda_utils-1.5b1/panda_utils/assetpipeline/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from panda_utils.util import get_data_file_path
 
 preblend_regex = re.compile(r".*\.(fbx|obj)")
 image_regex = re.compile(r".*\.(png|jpg|rgb)")
 logger = logging.getLogger("panda_utils.pipeline.models")
 
 
-def run_blender(cwd, file, script, *inputs):
-    args = [util.choose_binary("blender"), "--background", "--python", get_data_file_path(script), "--", *inputs]
+def run_blender(cwd, file, script, *args):
+    args = [util.choose_binary("blender"), "--background", "--python", get_data_file_path(script), "--", *args]
     if file is not None:
         args.insert(1, file)
     stdout_pipe = subprocess.DEVNULL if not os.getenv("PANDA_UTILS_BLENDER_LOGGING") else None
     subprocess.run(args, stdout=stdout_pipe, cwd=cwd)
 
 
 def build_asset_mapper(assets, name):
@@ -138,20 +138,30 @@
 def action_bam2egg(ctx):
     for file in ctx.files:
         if file.endswith(".bam"):
             logger.info("%s: Converting %s from Bam to Egg", ctx.name, file)
             bam2egg(ctx.putil_ctx, file)
 
 
-def action_yabee(ctx):
+def action_yabee(ctx, **kwargs):
+    args_converted = [f"{target_name}::{blender_name}" for target_name, blender_name in kwargs.items()]
     for file in ctx.files:
         if file.endswith(".blend"):
             logger.info("%s: Exporting through YABEE: %s", ctx.name, file)
             full_path = pathlib.Path(ctx.cwd, file)
-            run_blender(ctx.cwd, full_path, "blender/export_with_yabee.py", file[:-6] + ".egg")
+            egg_name = file[:-6] + ".egg"
+            run_blender(ctx.cwd, full_path, "blender/export_with_yabee.py", egg_name, *args_converted)
+
+            # NOTE: yabee does not care about the spaces in the file
+            # which means the file is hard to postprocess, so we have to do this thing below
+            # I think it only happens if any animations are exported - Wizz
+
+            if kwargs:
+                egg2bam(ctx.putil_ctx, egg_name)
+                bam2egg(ctx.putil_ctx, egg_name[:-4] + ".bam")
 
 
 def action_optimize(ctx, map_textures="true"):
     map_textures = map_textures.lower() not in ("", "0", "false")
 
     textures = set()
     ctx.cache_eggs()
```

### Comparing `panda_utils-1.4.4/panda_utils/assetpipeline/textures.py` & `panda_utils-1.5b1/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/blender/export_glb.py` & `panda_utils-1.5b1/panda_utils/blender/export_glb.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/blender/export_with_yabee.py` & `panda_utils-1.5b1/panda_utils/blender/export_with_yabee.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import bpy
 import addon_utils
 
 argv = sys.argv
 argv = argv[argv.index("--") + 1 :]  # get all arguments after "--"
 
-output_file = argv[0]
+output_file, *animations = argv
+animations = [x.split("::") for x in animations]
+animations = {blender_name: target_name for target_name, blender_name in animations}
 
 # we need to find the module that exports eggs
 modules = [
     mod
     for mod in addon_utils.modules()
     if mod.bl_info.get("description", "").lower().startswith("export to panda3d egg")
 ]
@@ -21,25 +23,26 @@
 yabee = addon_utils.enable(modules[0].__name__)
 BAKE_LAYERS = {layer: (512, 512, False) for layer in ["diffuse", "normal", "gloss", "glow", "AO", "shadow"]}
 bpy.ops.object.select_all(action="SELECT")
 
 errors = yabee.egg_writer.write_out(
     output_file,
     {},  # animations dictionary
-    False,  # "Export an animation for every action"
+    False,  # "Export an animation for every action" (obsoleted by actions dict)
     False,  # "Export UV map as texture"
     True,  # "Write an animation data into the separate files"
     False,  # "Write only animation data"
     False,  # "Copy texture files together with EGG" -> default True in blender but not needed here bc we postprocess
     ".",  # texture path to use -> we postprocess
     "NO",  # "Export all textures as MODULATE or bake texture layers" -> NO TBS GEN
     "BAKE",  # "Export all textures as MODULATE or bake texture layers" -> NO MODULATE
     BAKE_LAYERS,
     False,  # "Merge meshes, armatured by single Armature"
     True,  # "Apply modifiers on exported objects (except Armature)"
     False,  # "Run pview after exporting"
     False,  # "Use loop normals created by applying 'Normal Edit' Modifier as vertex normals."
     False,  # "Export Physically Based Properties, requires the BAM Exporter",
     False,  # "when False, writes only vertex color if polygon material is using it "
+    actions=animations,  # option specific to our YABEE
 )
 
 # right now status code of blender is ignored, so we're not checking the errors XD
```

### Comparing `panda_utils-1.4.4/panda_utils/blender/import_model.py` & `panda_utils-1.5b1/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/eggtree/eggparse.py` & `panda_utils-1.5b1/panda_utils/eggtree/eggparse.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/eggtree/operations.py` & `panda_utils-1.5b1/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/tools/animconvert.py` & `panda_utils-1.5b1/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/tools/convert.py` & `panda_utils-1.5b1/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/tools/downscale.py` & `panda_utils-1.5b1/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/tools/palettize.py` & `panda_utils-1.5b1/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/tools/toontown.py` & `panda_utils-1.5b1/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils/util.py` & `panda_utils-1.5b1/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.5b1/panda_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.4.4
+Version: 1.5b1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.4/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.5b1/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.4/pyproject.toml` & `panda_utils-1.5b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.4.4"
+version = "1.5b1"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

