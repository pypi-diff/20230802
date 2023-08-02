# Comparing `tmp/lightning_rod-0.5.0.tar.gz` & `tmp/lightning_rod-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.5.0.tar", max compression
+gzip compressed data, was "lightning_rod-0.5.1.tar", max compression
```

## Comparing `lightning_rod-0.5.0.tar` & `lightning_rod-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1061 2023-07-31 20:47:46.252010 lightning_rod-0.5.0/LICENSE
--rw-r--r--   0        0        0     1389 2023-07-31 20:47:46.252010 lightning_rod-0.5.0/README.md
--rw-r--r--   0        0        0      307 2023-07-31 20:48:54.808010 lightning_rod-0.5.0/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      664 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4562 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       38 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0       85 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/comment.bolt
--rw-r--r--   0        0        0      184 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     2579 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/damage.bolt
--rw-r--r--   0        0        0     1593 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      569 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     4604 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0     3596 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/offset_rotation.bolt
--rw-r--r--   0        0        0       35 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0       86 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1029 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2175 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/py.typed
--rw-r--r--   0        0        0     1242 2023-07-31 20:48:54.840012 lightning_rod-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-08-02 14:38:21.193668 lightning_rod-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1389 2023-08-02 14:38:21.193668 lightning_rod-0.5.1/README.md
+-rw-r--r--   0        0        0      307 2023-08-02 14:39:35.262308 lightning_rod-0.5.1/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      664 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4562 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       38 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      184 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     2579 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/damage.bolt
+-rw-r--r--   0        0        0     1593 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      569 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     4604 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0     3626 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/offset_rotation.bolt
+-rw-r--r--   0        0        0       35 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0       86 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1029 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2175 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-08-02 14:38:21.197668 lightning_rod-0.5.1/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1242 2023-08-02 14:39:35.298308 lightning_rod-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.5.1/PKG-INFO
```

### Comparing `lightning_rod-0.5.0/LICENSE` & `lightning_rod-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/README.md` & `lightning_rod-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/api.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/bossbar.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/damage.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/damage.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/effect.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/gamemode.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/gamemode.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/math.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/math.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/offset_rotation.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/offset_rotation.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 
     return output_rotation
 
 def offset_rotation_facing_caret(x: int | float | ExpressionNode,
                                  y: int | float | ExpressionNode,
                                  z: int | float | ExpressionNode):
 
-    if not isinstance(x, ExpressionNode) or not isinstance(y, ExpressionNode) or not isinstance(z, ExpressionNode):
-        at @s tp @s ~ ~ ~ facing ^x ^y ^z
-        return
-
-    vector_x = StaticVar(Int)
-    vector_y = StaticVar(Int)
-    vector_z = StaticVar(Int)
-
-    vector_x = x * 1000
-    vector_y = y * 1000
-    vector_z = z * 1000
-
-    copied_rotation = StaticVar(List)
-    copied_rotation = this.Rotation
-    matrix = _matrix_from_gimbal_3d(copied_rotation[0], copied_rotation[1])
-    t_vector_x, t_vector_y, t_vector_z = _transform_matrix_3d(matrix, vector_x, vector_y, vector_z)
-    new_rotation = _vector_to_gimbal_3d(t_vector_x, t_vector_y, t_vector_z)
-    this.Rotation = new_rotation
+    if isinstance(x, ExpressionNode) or isinstance(y, ExpressionNode) or isinstance(z, ExpressionNode):
+        vector_x = StaticVar(Int)
+        vector_y = StaticVar(Int)
+        vector_z = StaticVar(Int)
+
+        vector_x = x * 1000
+        vector_y = y * 1000
+        vector_z = z * 1000
+
+        copied_rotation = StaticVar(List)
+        copied_rotation = this.Rotation
+        matrix = _matrix_from_gimbal_3d(copied_rotation[0], copied_rotation[1])
+        t_vector_x, t_vector_y, t_vector_z = _transform_matrix_3d(matrix, vector_x, vector_y, vector_z)
+        new_rotation = _vector_to_gimbal_3d(t_vector_x, t_vector_y, t_vector_z)
+        this.Rotation = new_rotation
+
+    else:
+        at @s tp @s ~ ~ ~ facing ^x ^y ^z
```

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/time.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/time.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/lightning_rod/modules/xp.bolt` & `lightning_rod-0.5.1/lightning_rod/modules/xp.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.5.0/pyproject.toml` & `lightning_rod-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.5.0"
+version = "0.5.1"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
```

### Comparing `lightning_rod-0.5.0/PKG-INFO` & `lightning_rod-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-rod
-Version: 0.5.0
+Version: 0.5.1
 Summary: Function library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/lightning-rod
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

