# Comparing `tmp/orbax-export-0.0.2.tar.gz` & `tmp/orbax_export-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-export-0.0.2.tar", last modified: Tue Apr  4 18:08:07 2023, max compression
+gzip compressed data, was "orbax_export-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax-export-0.0.2.tar` & `orbax_export-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-04-04 18:06:49.225037 orbax-export-0.0.2/LICENSE
--rw-r--r--   0        0        0      286 2023-04-04 18:06:49.225037 orbax-export-0.0.2/README.md
--rw-r--r--   0        0        0     1134 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/__init__.py
--rw-r--r--   0        0        0      740 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/conftest.py
--rw-r--r--   0        0        0     3334 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/dtensor_export_test.py
--rw-r--r--   0        0        0      949 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/dtensor_initialization_test.py
--rw-r--r--   0        0        0     6253 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/dtensor_utils.py
--rw-r--r--   0        0        0     4215 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/dtensor_utils_test.py
--rw-r--r--   0        0        0      583 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/examples/__init__.py
--rw-r--r--   0        0        0     3103 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/examples/flax_mnist_main.py
--rw-r--r--   0        0        0     1549 2023-04-04 18:06:49.225037 orbax-export-0.0.2/orbax/export/examples/flax_mnist_main_test.py
--rw-r--r--   0        0        0     5404 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/export_manager.py
--rw-r--r--   0        0        0      977 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/export_manager_base.py
--rw-r--r--   0        0        0     9127 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/export_manager_test.py
--rw-r--r--   0        0        0    10940 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/jax_module.py
--rw-r--r--   0        0        0     8639 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/jax_module_test.py
--rw-r--r--   0        0        0     5795 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/serving_config.py
--rw-r--r--   0        0        0      810 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/__init__.py
--rw-r--r--   0        0        0     3872 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_job.py
--rw-r--r--   0        0        0     3313 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_job_test.py
--rw-r--r--   0        0        0     7702 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_manager.py
--rw-r--r--   0        0        0    10273 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_manager_test.py
--rw-r--r--   0        0        0     8865 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_report.py
--rw-r--r--   0        0        0     5602 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_report_test.py
--rw-r--r--   0        0        0     2129 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_utils.py
--rw-r--r--   0        0        0     2282 2023-04-04 18:06:49.229037 orbax-export-0.0.2/orbax/export/validate/validation_utils_test.py
--rw-r--r--   0        0        0     1062 2023-04-04 18:06:49.229037 orbax-export-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 orbax-export-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 22:43:00.304403 orbax_export-0.0.3/LICENSE
+-rw-r--r--   0        0        0      655 2023-08-01 22:43:00.304403 orbax_export-0.0.3/README.md
+-rw-r--r--   0        0        0     1430 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/__init__.py
+-rw-r--r--   0        0        0      740 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/conftest.py
+-rw-r--r--   0        0        0     3454 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/dtensor_export_test.py
+-rw-r--r--   0        0        0     1389 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/dtensor_initialization_test.py
+-rw-r--r--   0        0        0     7331 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/dtensor_utils.py
+-rw-r--r--   0        0        0     6202 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/dtensor_utils_test.py
+-rw-r--r--   0        0        0      583 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/examples/__init__.py
+-rw-r--r--   0        0        0     3103 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/examples/flax_mnist_main.py
+-rw-r--r--   0        0        0     1549 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/examples/flax_mnist_main_test.py
+-rw-r--r--   0        0        0     5185 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/export_manager.py
+-rw-r--r--   0        0        0      977 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/export_manager_base.py
+-rw-r--r--   0        0        0    13265 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/export_manager_test.py
+-rw-r--r--   0        0        0    11096 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/jax_module.py
+-rw-r--r--   0        0        0     9205 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/jax_module_test.py
+-rw-r--r--   0        0        0     7632 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/serving_config.py
+-rw-r--r--   0        0        0     1434 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/serving_config_test.py
+-rw-r--r--   0        0        0    10840 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/utils.py
+-rw-r--r--   0        0        0     6437 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/utils_test.py
+-rw-r--r--   0        0        0      810 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/__init__.py
+-rw-r--r--   0        0        0     3872 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_job.py
+-rw-r--r--   0        0        0     3313 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_job_test.py
+-rw-r--r--   0        0        0     7702 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_manager.py
+-rw-r--r--   0        0        0    10435 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_manager_test.py
+-rw-r--r--   0        0        0     8865 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_report.py
+-rw-r--r--   0        0        0     5602 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_report_test.py
+-rw-r--r--   0        0        0     2129 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_utils.py
+-rw-r--r--   0        0        0     2282 2023-08-01 22:43:00.304403 orbax_export-0.0.3/orbax/export/validate/validation_utils_test.py
+-rw-r--r--   0        0        0     1084 2023-08-01 22:43:00.304403 orbax_export-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 orbax_export-0.0.3/PKG-INFO
```

### Comparing `orbax-export-0.0.2/LICENSE` & `orbax_export-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/conftest.py` & `orbax_export-0.0.3/orbax/export/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/dtensor_export_test.py` & `orbax_export-0.0.3/orbax/export/dtensor_export_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import tensorflow as tf
 
 
 def _create_sharded_jax_array(
     global_arr: np.ndarray, pspec: P, mesh: jax.sharding.Mesh
 ) -> jax.Array:
   with mesh:
-    return pjit.pjit(lambda x: x, out_axis_resources=pspec)(global_arr)
+    return pjit.pjit(lambda x: x, out_shardings=pspec)(global_arr)
 
 
 class DtensorExportTest(absltest.TestCase):
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
@@ -46,17 +46,14 @@
     self.assertTrue(dtensor_utils.dtensor_initialized())
     self._mesh_shape = (4, 2)
     devices = np.asarray(jax.devices()).reshape(*self._mesh_shape)
     self._mesh = jax.sharding.Mesh(devices, ('x', 'y'))
     self._export_dir = self.create_tempdir().full_path
 
   def test_jax_module_export(self):
-    if jax.config.jax2tf_default_native_serialization:
-      self.skipTest(
-          'TODO(b/274311054): Could not legalize op: tf.XlaCallModule')
     w = np.random.rand(16, 8).astype(np.float32)
     x = np.random.rand(2, 16).astype(np.float32)
     with self._mesh:
       pspec = P('x', 'y')
       params = {'w': _create_sharded_jax_array(w, pspec, self._mesh)}
       pspecs = {'w': pspec}
 
@@ -76,14 +73,19 @@
                     [tf.TensorSpec((2, 16), tf.float32, name='x')],
                     tf_postprocessor=lambda y: {'y': y},
                 )
             ],
         )
         em.save(self._export_dir)
 
+      jax_result = pjit_model_fn(params, x)
+      tf_result = tf.saved_model.load(self._export_dir).signatures[
+          'serving_default'
+      ](x=x)['y']
+      np.testing.assert_allclose(jax_result, tf_result, atol=1e-5, rtol=1e-5)
 
   def test_dtensor_export_error(self):
     pspec = P('x', 'y')
     w = np.random.rand(16, 8).astype(np.float32)
     sharded_w = _create_sharded_jax_array(
         np.random.rand(16, 8).astype(np.float32), pspec, self._mesh
     )
@@ -94,8 +96,9 @@
     with self.assertRaisesRegex(
         ValueError, 'JaxModule is not created within a DTensor export context'
     ):
       JaxModule({'w': w}, lambda x: x, pspecs={'w': pspec})
 
 
 if __name__ == '__main__':
+  jax.config.parse_flags_with_absl()
   absltest.main()
```

### Comparing `orbax-export-0.0.2/orbax/export/dtensor_utils.py` & `orbax_export-0.0.3/orbax/export/dtensor_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,30 +26,37 @@
 
 DTensor = tf.Tensor
 
 
 _DTENSOR_INITIALIZED = False
 
 
-def initialize_dtensor():
+def initialize_dtensor(reset_context: bool = False):
   """Initialize a DTensor system for Orbax Export.
 
+  Args:
+    reset_context: Reset the tensorflow context along DTensor initialization.
+      Behaviors of existing TensorFlow objects (e.g. Tensors) are undefined. Set
+      this to True as an escape hatch, if there is no clear way to refactor your
+      code to call initialize_dtensor() before calling TensorFlow APIs that
+      initialize the context. See also `dtensor.initialize_accelerator_system`.
+
   Raises:
     RuntimeError: if the number of DTensor clients is not the same as that of
     JAX processes.
   """
   n_jax_devices = jax.device_count()
   n_jax_local_devices = jax.local_device_count()
   n_jax_processes = jax.process_count()
 
-  tf.config.set_logical_device_configuration(
-      tf.config.list_physical_devices('CPU')[0],
-      [tf.config.LogicalDeviceConfiguration()] * n_jax_local_devices,
+  dtensor.initialize_accelerator_system(
+      device_type='CPU',
+      num_logical_cpu_devices=n_jax_local_devices,
+      experimental_reset_context=reset_context,
   )
-  dtensor.initialize_accelerator_system('CPU')
   if dtensor.num_clients() != n_jax_processes:
     raise RuntimeError(
         f'The number of DTensor clients ({dtensor.num_clients()}) is not equal'
         f' to the number of JAX processes ({n_jax_processes}. Did you forget to'
         ' set ``DTENSOR_JOBS`` or other DTensor env variables for all the JAX'
         ' processes?'
     )
@@ -65,14 +72,22 @@
 
 
 def dtensor_initialized() -> bool:
   """Checks whether DTensor is intialized and matches the JAX device set."""
   return _DTENSOR_INITIALIZED
 
 
+def shutdown_dtensor() -> None:
+  if not dtensor_initialized():
+    raise RuntimeError('DTensor is not initialized.')
+  dtensor.shutdown_accelerator_system()
+  global _DTENSOR_INITIALIZED
+  _DTENSOR_INITIALIZED = False
+
+
 def jax_mesh_to_dtensor_mesh(mesh: jax.sharding.Mesh) -> dtensor.Mesh:
   """Creates a DTensor mesh from a JAX mesh.
 
   Args:
     mesh: a JAX global mesh for pjit.
 
   Returns:
@@ -82,15 +97,15 @@
   mesh_shape = mesh.devices.shape
   global_device_ids = np.arange(0, np.prod(mesh_shape)).reshape(mesh_shape)
   with mesh:
     # Shard the global device ids so that each process gets the local device ids
     # for the correponding DTensor mesh.
     sharded_device_ids = pjit.pjit(
         lambda x: x,
-        out_axis_resources=jax.sharding.PartitionSpec(*mesh.axis_names),
+        out_shardings=jax.sharding.PartitionSpec(*mesh.axis_names),
     )(global_device_ids)
 
   local_device_ids = [
       int(s.data) for s in sharded_device_ids.addressable_shards
   ]
   return dtensor.Mesh(
       list(mesh.shape.keys()),
@@ -129,22 +144,31 @@
         if not isinstance(mesh_axis_name, str):
           if not isinstance(mesh_axis_name, tuple):
             raise TypeError(
                 'An element in a PartitionSpec must be be a ``None``, a mesh'
                 ' axis or a tuple of mesh axes. Got {mesh_axis_name}.'
             )
           if len(mesh_axis_name) > 1:
-            raise ValueError(
-                f'Dimension {i} of the input array (shape={arr.shape}) is'
-                f' sharded across more than one axis ({mesh_axis_name}) of the'
-                ' mesh, but jax.Array to DTensor tranform does not support'
-                ' partitioning of an array dimension across multiple mesh axes.'
-            )
-          else:
-            mesh_axis_name = mesh_axis_name[0]
+            dim_sizes = tuple(dmesh.dim_size(name) for name in mesh_axis_name)
+            if dim_sizes.count(1) < len(mesh_axis_name) - 1:
+              raise ValueError(
+                  f'Dimension {i} of the input array (shape={arr.shape}) is'
+                  f' sharded across more than one axis ({mesh_axis_name}, sizes'
+                  f' = {dim_sizes}) of the mesh, but jax.Array to DTensor'
+                  ' tranform does not support partitioning of an array'
+                  ' dimension across multiple mesh axes, unless there is at'
+                  ' most one axis with size >= 1.'
+              )
+            else:
+              mesh_axis_name = tuple(
+                  filter(lambda x: dmesh.dim_size(x) != 1, mesh_axis_name)
+              ) or (mesh_axis_name[0],)
+
+          assert len(mesh_axis_name) == 1, mesh_axis_name
+          mesh_axis_name = mesh_axis_name[0]
         mesh_dim_size = dmesh.dim_size(mesh_axis_name)
         if arr.shape[i] % dmesh.dim_size(mesh_axis_name) != 0:
           raise ValueError(
               f'The size of the dim {i} (={arr.shape[i]}) of the input array'
               f' (shape={arr.shape}) must be a multiple of the size of'
               f' mesh axis "{mesh_axis_name}" (={mesh_dim_size}).)'
           )
```

### Comparing `orbax-export-0.0.2/orbax/export/dtensor_utils_test.py` & `orbax_export-0.0.3/orbax/export/dtensor_utils_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,39 +28,52 @@
 PartitionSpec = Optional[P]
 
 
 def _create_sharded_jax_array(
     global_arr: np.ndarray, pspec: PartitionSpec, mesh: jax.sharding.Mesh
 ) -> jax.Array:
   with mesh:
-    return pjit.pjit(lambda x: x, out_axis_resources=pspec)(global_arr)
+    return pjit.pjit(lambda x: x, out_shardings=pspec)(global_arr)
 
 
 def _get_dtensor_full_value(
     dt_arr: dtensor_utils.DTensor,
     dmesh: dtensor.Mesh,
 ) -> np.ndarray:
   return dtensor.relayout(
       dt_arr, dtensor.Layout([dtensor.UNSHARDED for _ in dt_arr.shape], dmesh)
   ).numpy()
 
 
+def _get_dtensor_shard_shape(dt_arr: dtensor_utils.DTensor) -> tuple[int, ...]:
+  layout = dtensor.fetch_layout(dt_arr)
+  return tuple(
+      size // layout.num_shards(i)
+      for i, size in enumerate(dt_arr.shape.as_list())
+  )
+
+
 class DtensorUtilsTest(parameterized.TestCase):
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
     dtensor_utils.initialize_dtensor()
 
   def setUp(self):
     super().setUp()
     self.assertTrue(dtensor_utils.dtensor_initialized())
     self._mesh_shape = (4, 2)
-    devices = np.asarray(jax.devices()).reshape(*self._mesh_shape)
-    self._mesh = jax.sharding.Mesh(devices, ('x', 'y'))
+    self._mesh = self._create_mesh(self._mesh_shape, ('x', 'y'))
+
+  def _create_mesh(
+      self, shape: tuple[int, ...], axis_names: tuple[str, ...]
+  ) -> jax.sharding.Mesh:
+    devices = np.asarray(jax.devices()).reshape(*shape)
+    return jax.sharding.Mesh(devices, axis_names)
 
   def test_jax_mesh_to_dtensor_mesh(self):
     dmesh = dtensor_utils.jax_mesh_to_dtensor_mesh(self._mesh)
     self.assertSequenceEqual(dmesh.shape(), self._mesh_shape)
     self.assertEqual(dmesh.dim_size('x'), 4)
     self.assertEqual(dmesh.dim_size('y'), 2)
 
@@ -75,14 +88,19 @@
   def test_jax_array_to_dtensor(
       self, shape: tuple[int, ...], pspec: PartitionSpec
   ):
     global_arr = np.arange(np.prod(shape)).reshape(shape)
     jax_arr = _create_sharded_jax_array(global_arr, pspec, self._mesh)
     dmesh = dtensor_utils.jax_mesh_to_dtensor_mesh(self._mesh)
     dt_arr = dtensor_utils.jax_array_to_dtensor(jax_arr, pspec, dmesh)
+
+    self.assertEqual(
+        _get_dtensor_shard_shape(dt_arr),
+        jax_arr.sharding.shard_shape(jax_arr.shape),
+    )
     np.testing.assert_equal(_get_dtensor_full_value(dt_arr, dmesh), global_arr)
 
   def test_sharding_across_multi_mesh_axes_unsupported(self):
     global_arr = np.arange(16).reshape((8, 2))
     pspec = P(('x', 'y'))
     jax_arr = _create_sharded_jax_array(global_arr, pspec, self._mesh)
     dmesh = dtensor_utils.jax_mesh_to_dtensor_mesh(self._mesh)
@@ -91,14 +109,47 @@
         (
             'not support partitioning of an array dimension across multiple'
             ' mesh axes'
         ),
     ):
       dtensor_utils.jax_array_to_dtensor(jax_arr, pspec, dmesh)
 
+  @parameterized.parameters(
+      ((1, 8), ('x', 'y'), P(None, ('x', 'y'))),
+      ((8, 1), ('x', 'y'), P(('x', 'y'), None)),
+      ((1, 2, 4), ('x', 'y', 'z'), P(None, 'y', ('x', 'z'))),
+      ((1, 2, 4), ('x', 'y', 'z'), P(None, 'y', ('z', 'x'))),
+      ((1, 2, 4), ('x', 'y', 'z'), P(None, None, ('y', 'x'))),
+      ((1, 1, 8), ('x', 'y', 'z'), P(None, None, ('x', 'y', 'z'))),
+      ((1, 8, 1), ('x', 'y', 'z'), P(None, ('x', 'y', 'z'), None)),
+      ((8, 1, 1), ('x', 'y', 'z'), P(('x', 'y', 'z'), None, None)),
+      ((1, 1, 8), ('x', 'y', 'z'), P(None, 'y', ('x', 'z'))),
+      ((1, 1, 8), ('x', 'y', 'z'), P('x', None, ('y', 'z'))),
+      ((1, 1, 8), ('x', 'y', 'z'), P('x', None, ('z', 'y'))),
+      ((1, 1, 8), ('x', 'y', 'z'), P(('x', 'y'), None, 'z')),
+  )
+  def test_sharding_across_multi_mesh_axes(
+      self,
+      mesh_shape: tuple[int, ...],
+      axis_names: tuple[str, ...],
+      pspec: P,
+  ):
+    arr_shape = np.asarray(mesh_shape) * 2
+    global_arr = np.arange(np.prod(arr_shape)).reshape(arr_shape)
+    mesh = self._create_mesh(mesh_shape, axis_names)
+    jax_arr = _create_sharded_jax_array(global_arr, pspec, mesh)
+    dmesh = dtensor_utils.jax_mesh_to_dtensor_mesh(mesh)
+    dt_arr = dtensor_utils.jax_array_to_dtensor(jax_arr, pspec, dmesh)
+
+    self.assertEqual(
+        _get_dtensor_shard_shape(dt_arr),
+        jax_arr.sharding.shard_shape(jax_arr.shape),
+    )
+    np.testing.assert_equal(_get_dtensor_full_value(dt_arr, dmesh), global_arr)
+
   def test_jax_dtensor_mesh_mismatch(self):
     global_arr = np.arange(16).reshape((8, 2))
     pspec = P('x', 'y')
     jax_arr = _create_sharded_jax_array(global_arr, pspec, self._mesh)
     dmesh = dtensor.create_mesh([('x', 2), ('y', 4)])
     with self.assertRaisesRegex(
         ValueError, 'must be a multiple of the size of mesh axis "y"'
```

### Comparing `orbax-export-0.0.2/orbax/export/examples/__init__.py` & `orbax_export-0.0.3/orbax/export/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/examples/flax_mnist_main.py` & `orbax_export-0.0.3/orbax/export/examples/flax_mnist_main.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/examples/flax_mnist_main_test.py` & `orbax_export-0.0.3/orbax/export/examples/flax_mnist_main_test.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/export_manager.py` & `orbax_export-0.0.3/orbax/export/export_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """Manage the exporting of a JAXModule."""
 
 from collections.abc import Mapping, Sequence
 from typing import Any, Callable, Optional
 
 from etils.epy.reraise_utils import maybe_reraise
+from orbax.export import utils
 from orbax.export.dtensor_utils import get_current_dtensor_mesh
 from orbax.export.export_manager_base import ExportManagerBase
 from orbax.export.jax_module import JaxModule
 from orbax.export.serving_config import ServingConfig
 import tensorflow as tf
 from tensorflow.experimental import dtensor
 
@@ -39,105 +40,101 @@
         cooresponding to a serving signature of the exported SavedModel.
     """
     # Creates a new tf.Module wrapping the JaxModule and extra trackable
     # resources.
     self._module = tf.Module()
     self._module.computation_module = module
     self._serving_signatures = {}
-    extra_trackables = []
+    tf_trackable_resources = []
 
     for sc in serving_configs:
       with maybe_reraise(f'Failed exporting signature_key={sc.signature_key} '):
         method = sc.get_infer_step(module.methods)
-        concrete_fn = make_concrete_inference_fn(method, sc)
+        inference_fn = make_e2e_inference_fn(method, sc)
         if isinstance(sc.signature_key, str):
           keys = [sc.signature_key]
         else:
           keys = sc.signature_key
         for key in keys:
           if key in self._serving_signatures:
             raise ValueError(
                 f'Duplicated key "{sc.signature_key}" in `serving_configs`.'
             )
-          self._serving_signatures[key] = concrete_fn
+          self._serving_signatures[key] = inference_fn
 
         if sc.extra_trackable_resources is not None:
-          extra_trackables.append(sc.extra_trackable_resources)
+          tf_trackable_resources.append(sc.extra_trackable_resources)
 
-    self._module.extra_trackables = extra_trackables
+      if len(serving_configs) == 1:
+        # Make this module callable. Once exported, it can be loaded back in
+        # python and the nested input structure will be preservered. In
+        # contrast, signatures will flatten the TensorSpecs of the to kwargs.
+        self.tf_module.__call__ = inference_fn
+
+    self._module.tf_trackable_resources = tf_trackable_resources
 
   @property
   def tf_module(self) -> tf.Module:
     """Returns the tf.module maintained by the export manager."""
     return self._module
 
   @property
   def serving_signatures(self) -> Mapping[str, Callable[..., Any]]:
     """Returns a map of signature keys to serving functions."""
     return self._serving_signatures
 
-  def save(self,
-           model_path: str,
-           save_options: Optional[tf.saved_model.SaveOptions] = None):
+  def save(
+      self,
+      model_path: str,
+      save_options: Optional[tf.saved_model.SaveOptions] = None,
+      signature_overrides: Optional[Mapping[str, Callable[..., Any]]] = None,
+  ):
     """Saves the JAX model to a Savemodel.
 
     Args:
       model_path: a directory in which to write the SavedModel.
       save_options: an optional tf.saved_model.SaveOptions for configuring save
         options.
+      signature_overrides: signatures to override the self-maintained ones, or
+        additional signatures to export.
     """
     save_options = save_options or tf.saved_model.SaveOptions()
     save_options.experimental_custom_gradients = (
         self._module.computation_module.with_gradient
     )
+
+    serving_signatures = dict(self.serving_signatures)
+    if signature_overrides:
+      serving_signatures.update(signature_overrides)
+
     tf.saved_model.save(
-        self.tf_module,
-        model_path,
-        self.serving_signatures,
-        options=save_options)
+        self.tf_module, model_path, serving_signatures, options=save_options
+    )
 
     if get_current_dtensor_mesh():
       # TODO(b/261191533): we can remove this once tf.saved_model.save is aware
       # of SPMD saving.
       dtensor.barrier(get_current_dtensor_mesh(), 'export done')
 
   def load(self, model_path: str, **kwargs: Any):
     loaded = tf.saved_model.load(model_path, **kwargs)
     return loaded
 
 
-def make_concrete_inference_fn(
+def make_e2e_inference_fn(
     model_fn: Callable[..., Any],
     serving_config: ServingConfig) -> Callable[..., Any]:
   """Creates an concrete end-to-end inference tf.function.
 
   Args:
     model_fn: a callable in TF context for the numeric computation.
     serving_config: a ServingConfig that defines the input sigature,
       pre-processor and post-processor of the inference function.
 
   Returns:
-    A concrete tf.function for end-to-end inference.
+    A tf.function for end-to-end inference.
   """
-  input_signature = serving_config.input_signature
-  if input_signature is None:
-    if hasattr(serving_config.tf_preprocessor, 'input_signature'
-              ) and serving_config.tf_preprocessor.input_signature is not None:
-      input_signature = serving_config.tf_preprocessor.input_signature
-    else:
-      raise ValueError(
-          (
-              f'ServingConfig (key={serving_config.signature_key}) does not set'
-              ' `input_signature`, and it cannot be inferred from'
-              ' `tf_preprocessor.'
-          ),
-          ' Please set `input_signature` explictly.',
-      )
-
   infer_step_func_map = serving_config.bind(model_fn, require_numpy=False)
   signature_key = serving_config.get_signature_keys()[0]
-  inferece_tf_fn = tf.function(
-      infer_step_func_map[signature_key], autograph=False, jit_compile=False)
-  # TODO(b/239083475): tracing with an input signature is the most error-prone
-  # step in export. We can additionally trace the pre-processor, core module and
-  # the post-processor individually for better debuggability.
-  return inferece_tf_fn.get_concrete_function(*input_signature)
+  return utils.with_default_args(
+      infer_step_func_map[signature_key], serving_config.get_input_signature()
+  )
```

### Comparing `orbax-export-0.0.2/orbax/export/export_manager_base.py` & `orbax_export-0.0.3/orbax/export/export_manager_base.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/export_manager_test.py` & `orbax_export-0.0.3/orbax/export/export_manager_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 import functools
 import os
 
 from absl.testing import parameterized
 import jax
 import jax.numpy as jnp
 from orbax.export.export_manager import ExportManager
-from orbax.export.export_manager import make_concrete_inference_fn
+from orbax.export.export_manager import make_e2e_inference_fn
 from orbax.export.jax_module import JaxModule
 from orbax.export.serving_config import ServingConfig
+from orbax.export.utils import TensorSpecWithDefault
 import tensorflow as tf
 
 
 def _from_feature_dict(feature_dict):
   return feature_dict['feat']
 
 
@@ -52,65 +53,84 @@
   def setUp(self):
     super().setUp()
     self._output_dir = self.create_tempdir().full_path
 
   @parameterized.named_parameters(
       dict(
           testcase_name='normal',
-          input_signature=[{
-              'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')
-          }],
+          input_signature=[
+              {'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')}
+          ],
           preprocessor=_from_feature_dict,
           postprocessor=_add_output_name,
-          inputs={'feat': tf.constant(1)},
-          outputs={'outputs': tf.constant(2)}),
+          inputs=[{'feat': tf.constant(1)}],
+          outputs={'outputs': tf.constant(2)},
+      ),
       dict(
           testcase_name='embedded input signature',
-          preprocessor=tf.function(_from_feature_dict, [{
-              'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')
-          }]),
+          preprocessor=tf.function(
+              _from_feature_dict,
+              [{'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')}],
+          ),
           postprocessor=_add_output_name,
-          inputs={'feat': tf.constant(1)},
-          outputs={'outputs': tf.constant(2)}),
+          inputs=[{'feat': tf.constant(1)}],
+          outputs={'outputs': tf.constant(2)},
+      ),
       dict(
           testcase_name='no preprocessor',
           input_signature=[tf.TensorSpec((), tf.dtypes.int32, 'feat')],
           postprocessor=_add_output_name,
-          inputs=tf.constant(1),
-          outputs={'outputs': tf.constant(2)}),
+          inputs=[tf.constant(1)],
+          outputs={'outputs': tf.constant(2)},
+      ),
       dict(
           testcase_name='no postprocessor',
-          input_signature=[{
-              'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')
-          }],
+          input_signature=[
+              {'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')}
+          ],
           preprocessor=_from_feature_dict,
-          inputs={'feat': tf.constant(1)},
-          outputs=tf.constant(2)),
+          inputs=[{'feat': tf.constant(1)}],
+          outputs=tf.constant(2),
+      ),
       dict(
           testcase_name='core module only',
           input_signature=[tf.TensorSpec((), tf.dtypes.int32, 'feat')],
-          inputs=tf.constant(1),
-          outputs=tf.constant(2)),
+          inputs=[tf.constant(1)],
+          outputs=tf.constant(2),
+      ),
+      dict(
+          testcase_name='default value',
+          input_signature=[
+              TensorSpecWithDefault(
+                  tf.TensorSpec((), tf.dtypes.int32, 'feat'), 1
+              )
+          ],
+          inputs=[],
+          outputs=tf.constant(2),
+      ),
   )
-  def test_make_concrete_inference_fn(self,
-                                      inputs,
-                                      outputs,
-                                      input_signature=None,
-                                      preprocessor=None,
-                                      postprocessor=None):
+  def test_make_e2e_inference_fn(
+      self,
+      inputs,
+      outputs,
+      input_signature=None,
+      preprocessor=None,
+      postprocessor=None,
+  ):
     method = JaxModule(
         {
             'bias': jnp.array(1)
         },
         lambda p, x: x + p['bias'],
     ).methods[JaxModule.DEFAULT_METHOD_KEY]
-    inference_fn = make_concrete_inference_fn(
+    inference_fn = make_e2e_inference_fn(
         method,
-        ServingConfig('key', input_signature, preprocessor, postprocessor))
-    self.assertAllEqual(inference_fn(inputs), outputs)
+        ServingConfig('key', input_signature, preprocessor, postprocessor),
+    )
+    self.assertAllEqual(inference_fn(*inputs), outputs)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='multiple signatures',
           serving_configs=[
               ServingConfig(
                   'with_processors',
@@ -153,14 +173,102 @@
         serving_configs,
     )
     em.save(self._output_dir)
     loaded = tf.saved_model.load(self._output_dir, ['serve'])
     self.assertCountEqual(expected_keys, em.serving_signatures.keys())
     self.assertCountEqual(expected_keys, loaded.signatures.keys())
 
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='all default',
+          serving_config=ServingConfig(
+              'serving_default',
+              input_signature=[
+                  TensorSpecWithDefault(tf.TensorSpec((), tf.int32, 'x'), 2),
+                  TensorSpecWithDefault(tf.TensorSpec((), tf.int32, 'y'), 3),
+              ],
+              tf_preprocessor=lambda x, y: x + y,
+          ),
+          serving_inputs={},
+          expected_outputs=6,
+      ),
+      dict(
+          testcase_name='some default',
+          serving_config=ServingConfig(
+              'serving_default',
+              input_signature=[
+                  tf.TensorSpec((), tf.int32, 'x'),
+                  TensorSpecWithDefault(tf.TensorSpec((), tf.int32, 'y'), 2),
+              ],
+              tf_preprocessor=lambda x, y: x + y,
+          ),
+          serving_inputs={'x': 3},
+          expected_outputs=6,
+      ),
+      dict(
+          testcase_name='override default',
+          serving_config=ServingConfig(
+              'serving_default',
+              input_signature=[
+                  tf.TensorSpec((), tf.int32, 'x'),
+                  TensorSpecWithDefault(tf.TensorSpec((), tf.int32, 'y'), 2),
+              ],
+              tf_preprocessor=lambda x, y: x + y,
+          ),
+          serving_inputs={'x': 1, 'y': 3},
+          expected_outputs=5,
+      ),
+      dict(
+          testcase_name='nested',
+          serving_config=ServingConfig(
+              'serving_default',
+              input_signature=[
+                  tf.TensorSpec((), tf.int32, 'x'),
+                  {
+                      'y': TensorSpecWithDefault(
+                          tf.TensorSpec((), tf.int32, 'y'), 2
+                      ),
+                      'z': TensorSpecWithDefault(
+                          tf.TensorSpec((), tf.int32, 'z'), 3
+                      ),
+                  },
+              ],
+              tf_preprocessor=lambda x, extra: x + extra['y'] + extra['z'],
+          ),
+          serving_inputs={'x': 1},
+          expected_outputs=7,
+      ),
+  )
+  def test_save_default_inputs(
+      self, serving_config, serving_inputs, expected_outputs
+  ):
+    em = ExportManager(
+        JaxModule(
+            {'bias': jnp.array(1, jnp.int32)}, lambda p, x: x + p['bias']
+        ),
+        [serving_config],
+    )
+    em.save(self._output_dir)
+    # TODO(b/277814477): use the TF2 API
+    # loaded.signature['serving_default'](**serving_inputs)
+    # once it supports default values.
+    with tf.compat.v1.Graph().as_default(), tf.compat.v1.Session() as sess:
+      meta_graph_def = tf.compat.v1.saved_model.loader.load(
+          sess, ['serve'], self._output_dir
+      )
+      signature_def = meta_graph_def.signature_def[serving_config.signature_key]
+      output_tensor_name = signature_def.outputs['output_0'].name
+      fetch = sess.graph.get_tensor_by_name(output_tensor_name)
+      feed_dict = {
+          sess.graph.get_tensor_by_name(signature_def.inputs[k].name): v
+          for k, v in serving_inputs.items()
+      }
+      outputs = sess.run(fetch, feed_dict=feed_dict)
+    self.assertAllEqual(outputs, expected_outputs)
+
   def test_save_multiple_model_functions(self):
     linear_mdl = JaxModule(
         params={
             'w': jnp.zeros((4, 2), jnp.int32),
             'b': jnp.ones((2,), jnp.int32),
         },
         apply_fn={
@@ -199,14 +307,39 @@
 
     x = jnp.zeros((1, 4), jnp.int32)
     self.assertAllEqual(loaded.signatures['serving_default'](x=x)['y'],
                         jnp.ones((1, 2)))
     self.assertAllEqual(loaded.signatures['no_bias'](x=x)['y'], jnp.zeros(
         (1, 2)))
 
+  def test_callable_module(self):
+    jax_module = JaxModule(
+        jnp.asarray(0.0),
+        lambda w, x: w + jnp.sum(x['a']['b']),
+    )
+    dummy_inputs = {'a': {'b': jnp.ones(3, jnp.float32)}}
+
+    input_signature = jax.tree_map(
+        lambda x: tf.TensorSpec(dtype=x.dtype, shape=x.shape), dummy_inputs
+    )
+    em = ExportManager(
+        jax_module,
+        [
+            ServingConfig(
+                'serving_default',
+                input_signature=[input_signature],
+                tf_postprocessor=lambda out: {'y': out},
+            )
+        ],
+    )
+    em.save(self._output_dir)
+    loaded = em.load(self._output_dir)
+    result = loaded(dummy_inputs)
+    self.assertAllClose(result['y'], jnp.asarray(3.0))
+
   def test_save_non_differentiable_fn(self):
 
     def non_differetiable_fn(_, x):
       _, x = jax.lax.while_loop(
           cond_fun=lambda state: state[0],
           body_fun=lambda state: (False, state[1] + 1),
           init_val=(False, x))
```

### Comparing `orbax-export-0.0.2/orbax/export/jax_module.py` & `orbax_export-0.0.3/orbax/export/jax_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,18 @@
     return self._jax_methods
 
 
 def _get_param_names(params: PyTree) -> PyTree:
   """Gets parameter names for PyTree elements."""
 
   def _param_name_from_keypath(keypath: Tuple[Any, ...]) -> str:
-    return '.'.join([str(ckpt_utils.get_key_name(k)) for k in keypath])
+    name = '.'.join([str(ckpt_utils.get_key_name(k)) for k in keypath])
+    # '~' is not allowed in variable names but are used by dm-haiku. See
+    # https://github.com/google/orbax/issues/420
+    return name.replace('~', '_')
 
   names = jax.tree_util.tree_map_with_path(
       lambda kp, _: _param_name_from_keypath(kp), params
   )
 
   if jax.tree_util.tree_structure(params) != jax.tree_util.tree_structure(
       names
```

### Comparing `orbax-export-0.0.2/orbax/export/jax_module_test.py` & `orbax_export-0.0.3/orbax/export/jax_module_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,36 @@
             'd.e:0': np.array(1),
             'd.f.0:0': np.array([5, 6]),
             'd.f.1:0': np.array([7, 8]),
         },
         variable_names_to_vals,
     )
 
+  def test_variable_names_contains_tilde(self):
+    """Test that variable containing ~ are escaped.
+
+    https://github.com/google/orbax/issues/420
+    """
+    params = {
+        'model/~/linear': {
+            'w': jnp.array(1),
+            'b': jnp.array(2),
+        }
+    }
+    variable_names_to_vals = {
+        v.name: v for v in JaxModule(params, lambda params, x: x).variables
+    }
+    self.assertEqual(
+        {
+            'model/_/linear.w:0': np.array(1),
+            'model/_/linear.b:0': np.array(2),
+        },
+        variable_names_to_vals,
+    )
+
   def test_variable_names_custom_node_not_registered(self):
     @_register_custom_dict_to_jax
     class MyDict(dict):
       pass
 
     params = MyDict(
         a=jnp.array(1),
```

### Comparing `orbax-export-0.0.2/orbax/export/serving_config.py` & `orbax_export-0.0.3/orbax/export/serving_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,36 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ServingConfig class."""
+
 import dataclasses
 from typing import Any, Callable, Mapping, Optional, Sequence, Text, Union
 
+from absl import logging
 import jax
 import tensorflow as tf
 
+
 PyTree = Any
 
 
 @dataclasses.dataclass
 class ServingConfig:
   """Configuration for constructing a serving signature for a JaxModule.
 
   A ServingConfig is to be bound with a JaxModule to form an end-to-end serving
   signature.
   """
+
   # The key of the serving signature or a sequence of keys mapping to the same
   # serving signature.
   signature_key: Union[str, Sequence[str]]
-  # The input signature. Will infer input_signature is specified from
-  # `tf_preprocessor` by default.
-  input_signature: Optional[Sequence[Any]] = None
+  # The input signature for `tf_preprocessor` (or the JaxModule method if there
+  # is no `tf_preprocessor`). If not specified, this will be infered from
+  # `tf_preprocessor`, in which case `tf_preprocessor` must be a tf.function
+  # with `input_signature` annotation. See
+  # https://www.tensorflow.org/api_docs/python/tf/function#input_signatures.
+  input_signature: Optional[Sequence[PyTree]] = None
   # Optional pre-precessing function written in TF.
   tf_preprocessor: Optional[Callable[..., Any]] = None
   # Optional post-processing function written in TF.
   tf_postprocessor: Optional[Callable[..., Any]] = None
   # A nested structure of tf.saved_model.experimental.TrackableResource that are
   # used in `tf_preprocessor` and/or `tf_postprocessor`. If a TrackableResource
   # an attritute of the `tf_preprocessor` (or `tf_postprocessor`), and the
@@ -52,17 +59,37 @@
 
   def get_signature_keys(self) -> Sequence[str]:
     if isinstance(self.signature_key, str):
       return [self.signature_key]
     else:
       return self.signature_key
 
+  def get_input_signature(self, required=True) -> Any:
+    """Gets the input signature from the explict one or tf_preprocessor."""
+    input_signature = self.input_signature
+    if input_signature is None:
+      if (
+          hasattr(self.tf_preprocessor, 'input_signature')
+          and self.tf_preprocessor.input_signature is not None
+      ):
+        input_signature = self.tf_preprocessor.input_signature
+
+    if required and input_signature is None:
+      raise ValueError(
+          f'Neithr the ServingConfig (key={self.signature_key}) nor its'
+          ' `tf_preprocessor` sets an `input_signature`, please set'
+          ' `input_signature` explicitly.',
+      )
+    return input_signature
+
   def get_infer_step(
-      self, infer_step_fns: Union[Callable[..., Any],
-                                  Mapping[str, Callable[..., Any]]]
+      self,
+      infer_step_fns: Union[
+          Callable[..., Any], Mapping[str, Callable[..., Any]]
+      ],
   ) -> Callable[..., Any]:
     """Finds the right inference fn to be bound with the ServingConfig.
 
     Args:
       infer_step_fns: the method_key/infer_step dict. Ususally the user can pass
         `JaxModule.methods` here.
 
@@ -75,72 +102,100 @@
     method_key = self.method_key
     if method_key is None:
       if len(infer_step_fns) != 1:
         raise ValueError(
             '`method_key` is not specified in ServingConfig '
             f'"{self.signature_key}" and the infer_step_fns has more than one '
             f' methods: {list(infer_step_fns)}. Please specify '
-            '`method_key` explictly.')
+            '`method_key` explicitly.'
+        )
       (method,) = infer_step_fns.values()  # this is a tuple-destructuring
       return method
     else:
       if method_key not in infer_step_fns:
         raise ValueError(
             f'Method key "{method_key}" is not found in the infer_step_fns. '
-            f'Available method keys: {list(infer_step_fns.keys())}.')
+            f'Available method keys: {list(infer_step_fns.keys())}.'
+        )
       return infer_step_fns[method_key]
 
   def bind(
       self,
-      infer_step_fns: Union[Callable[[PyTree], PyTree],
-                            Mapping[str, Callable[[PyTree], PyTree]]],
-      require_numpy=True) -> Mapping[str, Callable[..., Mapping[Text, Any]]]:
+      infer_step_fns: Union[
+          Callable[[PyTree], PyTree], Mapping[str, Callable[[PyTree], PyTree]]
+      ],
+      require_numpy: bool = True,
+  ) -> Mapping[str, Callable[..., Mapping[Text, Any]]]:
     """Returns an e2e inference function by binding a inference step function.
 
     Args:
       infer_step_fns:  An inference step function of a mapping of method key to
         inference step function. If it is a mapping, the function whose key
         matches the `method_key` of this ServingConfig will be used.  If Users
         only provide infer_step function, all `method_key`s use same infer_step
         function.
       require_numpy: Decide convert tf tensor to numpy after tf preprocess and
         tf postprocess. As a rule of thumb,  if infer_step is jax function, set
         it to True. if infer_step if tf function, set it to False.
+
     Return:
       func_map:  The mapping of serving signature to the inference function
         bound with the pre- and post-processors of this ServingConfig.
     """
 
     def make_inference_fn(infer_step):
       """Bind the preprocess, method and postproess together."""
+      preprocessor = tf.function(self.tf_preprocessor or (lambda *a: a))
+      postprocessor = tf.function(self.tf_postprocessor or (lambda *a: a))
 
-      def inference_fn(*preprocessed_inputs):
+      def inference_fn(*inputs):
         if self.tf_preprocessor:
-          inputs = tf.function(self.tf_preprocessor)(*preprocessed_inputs)
+          preprocessed_inputs = preprocessor(*inputs)
           if require_numpy:
-            inputs = jax.tree_util.tree_map(lambda x: x.numpy(), inputs)
+            preprocessed_inputs = jax.tree_util.tree_map(
+                lambda x: x.numpy(), preprocessed_inputs
+            )
         else:
-          inputs = preprocessed_inputs
+          preprocessed_inputs = inputs
 
           if len(preprocessed_inputs) != 1:
-            raise ValueError('Currently does not accept multiple args, '
-                             f'got len(inputs)={len(inputs)}.')
+            raise ValueError(
+                'JaxModule only takes single arg as the input, but got'
+                f' len(inputs)={len(inputs)} from the preprocessor or input'
+                ' signature. Please pack all inputs into one PyTree by'
+                ' modifying the `input_signature` (if no `tf_preprocessor`) or'
+                ' the ServingConfig.tf_preprocessor.'
+            )
 
-          inputs = preprocessed_inputs[0]
+          preprocessed_inputs = preprocessed_inputs[0]
 
         # Currently Jax Module only takes 1 input
-        outputs = infer_step(inputs)
+        outputs = infer_step(preprocessed_inputs)
+        if logging.vlog_is_on(3) and require_numpy:
+          if hasattr(infer_step, 'lower'):
+            lower = infer_step.lower
+          else:
+            lower = jax.jit(infer_step).lower
+
+          mlir_module_text = lower(
+              preprocessed_inputs,
+          ).as_text()
+          logging.info(
+              'Jax function infer_step mlir module: = %s', mlir_module_text
+          )
+
         if self.tf_postprocessor:
-          outputs = tf.function(self.tf_postprocessor)(outputs)
+          outputs = postprocessor(outputs)
           if require_numpy:
             outputs = jax.tree_util.tree_map(lambda x: x.numpy(), outputs)
         return outputs
 
       return inference_fn
 
     func_map = {}
     infer_fn_with_processors = make_inference_fn(
-        self.get_infer_step(infer_step_fns))
+        self.get_infer_step(infer_step_fns)
+    )
     for key in self.get_signature_keys():
       func_map[key] = infer_fn_with_processors
 
     return func_map
```

### Comparing `orbax-export-0.0.2/orbax/export/validate/__init__.py` & `orbax_export-0.0.3/orbax/export/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_job.py` & `orbax_export-0.0.3/orbax/export/validate/validation_job.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_job_test.py` & `orbax_export-0.0.3/orbax/export/validate/validation_job_test.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_manager.py` & `orbax_export-0.0.3/orbax/export/validate/validation_manager.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_manager_test.py` & `orbax_export-0.0.3/orbax/export/validate/validation_manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,29 +144,33 @@
     self.assertAllValidationReportsPass(validation_reports)
 
   def test_basic(self):
 
     serving_configs = [
         ServingConfig(
             'without_processors',
-            input_signature=[{
-                'feature1': tf.TensorSpec((), tf.dtypes.int32, 'feature1')
-            }],
+            input_signature=[
+                {
+                    'feature1': tf.TensorSpec(
+                        (None,), tf.dtypes.int32, 'feature1'
+                    )
+                }
+            ],
         ),
     ]
     params = {'bias': jnp.array(0)}
 
     def apply_fn(p, x):
       y = x['feature1'] + p['bias']
       results = {}
       for i in range(9):
         results[str(i)] = y + i
       return results
 
-    jax_module = JaxModule(params, apply_fn)
+    jax_module = JaxModule(params, apply_fn, input_polymorphic_shape='b, ...')
     batch_input = list(np.arange(16).reshape((16, 1)).astype(np.int32))
     batch_input = [{'feature1': i} for i in batch_input]
     em = ExportManager(
         jax_module,
         serving_configs,
     )
     em.save(self._output_dir)
@@ -179,27 +183,27 @@
   @parameterized.named_parameters([
       dict(
           testcase_name='without_xprof',
           serving_configs=[
               ServingConfig(
                   'with_processors',
                   input_signature=[
-                      {'feat': tf.TensorSpec((), tf.dtypes.int32, 'feat')}
+                      {'feat': tf.TensorSpec((None,), tf.dtypes.int32, 'feat')}
                   ],
                   tf_preprocessor=_from_feature_dict,
                   tf_postprocessor=_add_output_name,
               ),
           ],
           with_xprof=False,
       ),
   ])
   def test_perf(self, serving_configs, with_xprof):
     params = {'bias': jnp.array(1)}
     apply_fn = lambda p, x: x + p['bias']
-    jax_module = JaxModule(params, apply_fn)
+    jax_module = JaxModule(params, apply_fn, input_polymorphic_shape='b, ...')
     batch_input = list(np.arange(128).reshape((16, 8)).astype(np.int32))
     batch_input = [{'feat': i} for i in batch_input]
     em = ExportManager(
         jax_module,
         serving_configs,
     )
     em.save(self._output_dir)
```

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_report.py` & `orbax_export-0.0.3/orbax/export/validate/validation_report.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_report_test.py` & `orbax_export-0.0.3/orbax/export/validate/validation_report_test.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_utils.py` & `orbax_export-0.0.3/orbax/export/validate/validation_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/orbax/export/validate/validation_utils_test.py` & `orbax_export-0.0.3/orbax/export/validate/validation_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-export-0.0.2/pyproject.toml` & `orbax_export-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,32 @@
 
 keywords = ["JAX machine learning", "serialization", "export"]
 
 dependencies = [
     'absl-py',
     'etils',
     'orbax-checkpoint',
-    'jax >= 0.4.8',
+    'jax',
     'jaxlib',
     'numpy',
     'dataclasses-json',
-    'tensorflow',
 ]
 
 dynamic = ['version']
 
 [tool.flit.module]
 name = "orbax.export"
 
 [project.urls]
 homepage = 'http://github.com/google/orbax'
 repository = 'http://github.com/google/orbax'
 
 [project.optional-dependencies]
-dev = [
+all = [
+  'tensorflow',
+]
+
+testing = [
     'pytest',
-    'pytest-xdist'
+    'pytest-xdist',
+    'tf-nightly'
 ]
```

### Comparing `orbax-export-0.0.2/PKG-INFO` & `orbax_export-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 Metadata-Version: 2.1
 Name: orbax-export
-Version: 0.0.2
+Version: 0.0.3
 Summary: Orbax Export
 Keywords: JAX machine learning,serialization,export
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: absl-py
 Requires-Dist: etils
 Requires-Dist: orbax-checkpoint
-Requires-Dist: jax >= 0.4.8
+Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: numpy
 Requires-Dist: dataclasses-json
-Requires-Dist: tensorflow
-Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: pytest-xdist ; extra == "dev"
+Requires-Dist: tensorflow ; extra == "all"
+Requires-Dist: pytest ; extra == "testing"
+Requires-Dist: pytest-xdist ; extra == "testing"
+Requires-Dist: tf-nightly ; extra == "testing"
 Project-URL: homepage, http://github.com/google/orbax
 Project-URL: repository, http://github.com/google/orbax
-Provides-Extra: dev
+Provides-Extra: all
+Provides-Extra: testing
 
-`pip install orbax-export`
+# Orbax Export
+
+`pip install orbax-export` (latest PyPi release) OR
+
+`pip install 'git+https://github.com/google/orbax/#subdirectory=export'` (from this repository, at HEAD)
 
 `import orbax.export`
 
-Orbax includes a serialization library for JAX users, enabling the exporting of
-JAX models to the TensorFlow SavedModel format. 
+Orbax includes a serialization library for JAX users, enabling the exporting of JAX models to the TensorFlow SavedModel format.
+
+Note that `orbax-export` requires TensorFlow, but does not include it by default to allow for flexibility in version choice. If you wish to install with standard TensorFlow, please use `pip install orbax-export[all]`.
 
-To get started, check out our [documentation](https://github.com/google/orbax/blob/main/docs/export.md).
+To get started, check out our [documentation](https://orbax.readthedocs.io/en/latest/orbax_export_101.html).
```

