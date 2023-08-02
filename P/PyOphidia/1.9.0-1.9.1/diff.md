# Comparing `tmp/PyOphidia-1.9.0.tar.gz` & `tmp/PyOphidia-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyOphidia-1.9.0.tar", last modified: Thu Jul 22 11:13:17 2021, max compression
+gzip compressed data, was "dist/PyOphidia-1.9.1.tar", last modified: Tue Aug  3 09:09:39 2021, max compression
```

## Comparing `PyOphidia-1.9.0.tar` & `PyOphidia-1.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ophidia   (1000) ophidia   (1000)        0 2021-07-22 11:13:17.000000 PyOphidia-1.9.0/
-drwxrwxr-x   0 ophidia   (1000) ophidia   (1000)        0 2021-07-22 11:13:17.000000 PyOphidia-1.9.0/PyOphidia/
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)      772 2021-07-21 21:25:53.000000 PyOphidia-1.9.0/PyOphidia/__init__.py
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    51944 2021-07-21 21:25:53.000000 PyOphidia-1.9.0/PyOphidia/client.py
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)   238279 2021-07-21 21:25:53.000000 PyOphidia-1.9.0/PyOphidia/cube.py
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    11909 2021-07-22 10:49:42.000000 PyOphidia-1.9.0/PyOphidia/ophsubmit.py
-drwxrwxr-x   0 ophidia   (1000) ophidia   (1000)        0 2021-07-22 11:13:17.000000 PyOphidia-1.9.0/PyOphidia.egg-info/
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    12565 2021-07-22 11:13:16.000000 PyOphidia-1.9.0/PyOphidia.egg-info/PKG-INFO
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)      305 2021-07-22 11:13:16.000000 PyOphidia-1.9.0/PyOphidia.egg-info/SOURCES.txt
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)        1 2021-07-22 11:13:16.000000 PyOphidia-1.9.0/PyOphidia.egg-info/dependency_links.txt
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)       10 2021-07-22 11:13:16.000000 PyOphidia-1.9.0/PyOphidia.egg-info/top_level.txt
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)      343 2021-07-21 15:24:45.000000 PyOphidia-1.9.0/AUTHORS.rst
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     1467 2021-07-21 15:24:45.000000 PyOphidia-1.9.0/CONTRIBUTING.rst
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     6059 2021-07-21 21:25:53.000000 PyOphidia-1.9.0/HISTORY.rst
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    35141 2021-07-21 15:24:45.000000 PyOphidia-1.9.0/LICENSE
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)       22 2021-07-21 15:24:45.000000 PyOphidia-1.9.0/MANIFEST.in
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     9551 2021-07-21 21:25:53.000000 PyOphidia-1.9.0/README.rst
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)       82 2021-07-22 11:13:17.000000 PyOphidia-1.9.0/setup.cfg
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     2216 2021-07-21 21:25:53.000000 PyOphidia-1.9.0/setup.py
--rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    12565 2021-07-22 11:13:17.000000 PyOphidia-1.9.0/PKG-INFO
+drwxrwxr-x   0 ophidia   (1000) ophidia   (1000)        0 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/
+drwxrwxr-x   0 ophidia   (1000) ophidia   (1000)        0 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PyOphidia/
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)      772 2021-08-02 16:36:06.000000 PyOphidia-1.9.1/PyOphidia/__init__.py
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    51944 2021-08-02 16:37:28.000000 PyOphidia-1.9.1/PyOphidia/client.py
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)   248867 2021-08-03 08:46:49.000000 PyOphidia-1.9.1/PyOphidia/cube.py
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    11765 2021-08-03 09:09:31.000000 PyOphidia-1.9.1/PyOphidia/ophsubmit.py
+drwxrwxr-x   0 ophidia   (1000) ophidia   (1000)        0 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PyOphidia.egg-info/
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    12565 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PyOphidia.egg-info/PKG-INFO
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)      305 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PyOphidia.egg-info/SOURCES.txt
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)        1 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PyOphidia.egg-info/dependency_links.txt
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)       10 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PyOphidia.egg-info/top_level.txt
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)      343 2021-07-21 15:24:45.000000 PyOphidia-1.9.1/AUTHORS.rst
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     1467 2021-07-21 15:24:45.000000 PyOphidia-1.9.1/CONTRIBUTING.rst
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     6619 2021-08-03 08:46:49.000000 PyOphidia-1.9.1/HISTORY.rst
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    35141 2021-07-21 15:24:45.000000 PyOphidia-1.9.1/LICENSE
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)       22 2021-07-21 15:24:45.000000 PyOphidia-1.9.1/MANIFEST.in
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     9551 2021-08-03 08:46:49.000000 PyOphidia-1.9.1/README.rst
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)       82 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/setup.cfg
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)     2216 2021-08-03 08:46:49.000000 PyOphidia-1.9.1/setup.py
+-rw-rw-r--   0 ophidia   (1000) ophidia   (1000)    12565 2021-08-03 09:09:39.000000 PyOphidia-1.9.1/PKG-INFO
```

### Comparing `PyOphidia-1.9.0/PyOphidia/__init__.py` & `PyOphidia-1.9.1/PyOphidia/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOphidia-1.9.0/PyOphidia/client.py` & `PyOphidia-1.9.1/PyOphidia/client.py`

 * *Files identical despite different names*

### Comparing `PyOphidia-1.9.0/PyOphidia/cube.py` & `PyOphidia-1.9.1/PyOphidia/cube.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 
 def get_linenumber():
     cf = currentframe()
     return __file__, cf.f_back.f_lineno
 
 
 class Cube:
-    """Cube(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None, cdd=None, compressed='no',
-            exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='no', check_compliance='no', offset=0,
-            ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes'
-            subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
-            leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='-', policy='rr', description='-', schedule=0,
-            pid=None, check_grid='no', display=False) -> obj
+    """Cube(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None,
+            cdd=None, compressed='no', exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='no',
+            check_compliance='no', offset=0, ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none',
+            subset_filter='all', time_filter='yes', subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00',
+            calendar='standard', hierarchy='oph_base', leap_month=2, leap_year=0,
+            month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='-', policy='rr',
+            description='-', schedule=0, pid=None, check_grid='no', save='yes', display=False) -> obj
          or Cube(pid=None) -> obj
 
     Attributes:
         pid: cube PID
         creation_date: creation date of the cube
         measure: name of the variable imported into the cube
         measure_type: measure data type
@@ -60,180 +61,204 @@
         nelements: total number of elements
         dim_info: list of dict with information on each cube dimension
 
     Class Attributes:
         client: instance of class Client through which it is possible to submit all requests
 
     Methods:
-        aggregate(ncores=1, nthreads=1, exec_mode='sync', schedule=0, group_size='all', operation=None, missingvalue='NAN', grid='-', container='-',
-                  description='-', check_grid='no', display=False)
+        aggregate(ncores=1, nthreads=1, exec_mode='sync', schedule=0, group_size='all', operation=None, missingvalue='-',
+                  grid='-', container='-', description='-', check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_AGGREGATE
-        aggregate2(ncores=1, nthreads=1, exec_mode='sync', schedule=0, dim='-', concept_level='A', midnight='24', operation=None, grid='-', missingvalue='NAN',
-                   container='-', description='-', check_grid='no', display=False)
+        aggregate2(ncores=1, nthreads=1, exec_mode='sync', schedule=0, dim='-', concept_level='A', midnight='24', operation=None,
+                   grid='-', missingvalue='-', container='-', description='-', check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_AGGREGATE2
-        apply(ncores=1, nthreads=1, exec_mode='sync', query='measure', dim_query='null', measure='null', measure_type='manual', dim_type='manual', check_type='yes',
-              on_reduce='skip', compressed='auto', schedule=0,container='-', description='-', display=False)
+        apply(ncores=1, nthreads=1, exec_mode='sync', query='measure', dim_query='null', measure='null', measure_type='manual',
+              dim_type='manual', check_type='yes', on_reduce='skip', compressed='auto', schedule=0,container='-', description='-',
+              save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_APPLY
-        concatnc(src_path=None, cdd=None, grid='-', check_exp_dim='yes', dim_offset='-', dim_continue='no', offset=0, description='-', subset_dims='none',
-                          subset_filter='all', subset_type='index', time_filter='yes', ncores=1, exec_mode='sync', schedule=0, display=False)
-                  -> Cube or None : wrapper of the operator OPH_CONCATNC
-        concatnc2(src_path=None, cdd=None, grid='-', check_exp_dim='yes', dim_offset='-', dim_continue='no', offset=0, description='-', subset_dims='none',
-                          subset_filter='all', subset_type='index', time_filter='yes', ncores=1, nthreads=1, exec_mode='sync', schedule=0, display=False)
-                  -> Cube or None : wrapper of the operator OPH_CONCATNC2
-        cubeelements( schedule=0, algorithm='dim_product', ncores=1, exec_mode='sync', objkey_filter='all', display=True)
+        concatnc(src_path=None, cdd=None, grid='-', check_exp_dim='yes', dim_offset='-', dim_continue='no', offset=0,
+                 description='-', subset_dims='none', subset_filter='all', subset_type='index', time_filter='yes', ncores=1,
+                 exec_mode='sync', schedule=0, save='yes', display=False)
+          -> Cube or None : wrapper of the operator OPH_CONCATNC
+        concatnc2(src_path=None, cdd=None, grid='-', check_exp_dim='yes', dim_offset='-', dim_continue='no', offset=0,
+                  description='-', subset_dims='none', subset_filter='all', subset_type='index', time_filter='yes', ncores=1,
+                  nthreads=1, exec_mode='sync', schedule=0, save='yes', display=False)
+           -> Cube or None : wrapper of the operator OPH_CONCATNC2
+        cubeelements( schedule=0, algorithm='dim_product', ncores=1, exec_mode='sync', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_CUBEELEMENTS
-        cubeschema( objkey_filter='all', exec_mode='sync', level=0, dim=None, show_index='no', show_time='no', base64='no', 'action=read', concept_level='c',
-              dim_level=1, dim_array='yes', display=True)
+        cubeschema(objkey_filter='all', exec_mode='sync', level=0, dim=None, show_index='no', show_time='no', base64='no',
+                   action='read', concept_level='c', dim_level=1, dim_array='yes', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_CUBESCHEMA
-        cubesize( schedule=0, ncores=1, byte_unit='MB', algorithm='euristic', objkey_filter='all', exec_mode='sync', display=True)
+        cubesize(schedule=0, ncores=1, byte_unit='MB', algorithm='euristic', objkey_filter='all', exec_mode='sync',
+                 save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_CUBESIZE
-        delete(ncores=1, nthreads=1, exec_mode='sync', schedule=0, display=False)
+        delete(ncores=1, nthreads=1, exec_mode='sync', schedule=0, save='yes', display=False)
           -> None : wrapper of the operator OPH_DELETE
-        drilldown(ndim=1, container='-', ncores=1, exec_mode='sync', schedule=0, description='-', display=False)
+        drilldown(ndim=1, container='-', ncores=1, exec_mode='sync', schedule=0, description='-', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_DRILLDOWN
-        duplicate(container='-', ncores=1, nthreads=1, exec_mode='sync', description='-', display=False)
+        duplicate(container='-', ncores=1, nthreads=1, exec_mode='sync', description='-', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_DUPLICATE
-        explore(schedule=0, limit_filter=100, subset_dims=None, subset_filter='all', time_filter='yes', subset_type='index', show_index='no', show_id='no',
-                show_time='no', level=1, output_path='default', output_name='default', cdd=None, base64='no', ncores=1, exec_mode='sync', objkey_filter='all',
-                display=True)
+        explore(schedule=0, limit_filter=100, subset_dims=None, subset_filter='all', time_filter='yes', subset_type='index',
+                show_index='no', show_id='no', show_time='no', level=1, output_path='default', output_name='default', cdd=None,
+                base64='no', ncores=1, exec_mode='sync', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_EXPLORECUBE
-        exportnc(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0, exec_mode='sync', ncores=1,
-                 display=False)
+        exportnc(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0,
+                 exec_mode='sync', ncores=1, save='yes', display=False)
           -> None : wrapper of the operator OPH_EXPORTNC
-        exportnc2(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0, exec_mode='sync', ncores=1,
-                  display=False)
+        exportnc2(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0,
+                  exec_mode='sync', ncores=1, save='yes', display=False)
           -> None : wrapper of the operator OPH_EXPORTNC2
         export_array(show_id='no', show_time='no', subset_dims=None, subset_filter=None, time_filter='no')
-          -> dict or None : wrapper of the operator OPH_EXPLORECUBE
+          -> dict or None : return data from an Ophidia datacube into a Python structure
         info(display=True)
           -> None : call OPH_CUBESIZE and OPH_CUBESCHEMA to fill all Cube attributes
-        intercube(cube2=None, cubes=None, operation='sub', container='-', exec_mode='sync', ncores=1, description='-', display=False)
+        intercube(cube2=None, cubes=None, operation='sub', missingvalue="-", container='-', exec_mode='sync', ncores=1,
+                  description='-', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_INTERCUBE
-        merge(nmerge=0, schedule=0, description='-', container='-', exec_mode='sync', ncores=1, display=False)
+        merge(nmerge=0, schedule=0, description='-', container='-', exec_mode='sync', ncores=1, save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_MERGE
-        metadata(mode='read', metadata_id=0, metadata_key='all', variable='global', metadata_type='text', metadata_value=None, variable_filter=None,
-                 metadata_type_filter=None, metadata_value_filter=None, force='no', exec_mode='sync', objkey_filter='all', display=True)
+        metadata(mode='read', metadata_id=0, metadata_key='all', variable='global', metadata_type='text', metadata_value=None,
+                 variable_filter=None, metadata_type_filter=None, metadata_value_filter=None, force='no', exec_mode='sync',
+                 objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_METADATA
-        permute(dim_pos=None, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', display=False)
+        permute(dim_pos=None, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', save='yes',
+                display=False)
           -> Cube or None : wrapper of the operator OPH_PERMUTE
-        provenance(branch='all', exec_mode='sync', objkey_filter='all', display=True)
+        provenance(branch='all', exec_mode='sync', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_CUBEIO
-        publish( ncores=1, content='all', exec_mode='sync', show_id= 'no', show_index='no', schedule=0, show_time='no', display=True)
+        publish(ncores=1, content='all', exec_mode='sync', show_id= 'no', show_index='no', schedule=0, show_time='no',
+                save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_PUBLISH
-        reduce(operation=None, container=None, exec_mode='sync', grid='-', group_size='all', ncores=1, nthreads=1, schedule=0, order=2, description='-',
-               objkey_filter='all', check_grid='no', display=False)
+        reduce(operation=None, container=None, exec_mode='sync', missingvalue="-", grid='-', group_size='all', ncores=1,
+               nthreads=1, schedule=0, order=2, description='-', objkey_filter='all', check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_REDUCE
-        reduce2(dim=None, operation=None, concept_level='A', container='-', exec_mode='sync', grid='-', midnight='24', order=2, description='-',
-                schedule=0, ncores=1, nthreads=1, check_grid='no', display=False)
+        reduce2(dim=None, operation=None, concept_level='A', missingvalue="-", container='-', exec_mode='sync', grid='-',
+                midnight='24', order=2, description='-', schedule=0, ncores=1, nthreads=1, check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_REDUCE2
-        rollup(ndim=1, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', display=False)
+        rollup(ndim=1, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_ROLLUP
-        split(nsplit=2, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', display=False)
+        split(nsplit=2, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_SPLIT
         subset(subset_dims='none', subset_filter='all', container='-', exec_mode='sync', subset_type='index',
-               time_filter='yes', offset=0, grid='-', ncores=1, nthreads=1, schedule=0, description='-', check_grid='no', display=False)
+               time_filter='yes', offset=0, grid='-', ncores=1, nthreads=1, schedule=0, description='-', check_grid='no',
+               save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_SUBSET
-        subset2(subset_dims='none', subset_filter='all', grid='-', container='-', ncores=1, exec_mode='sync', schedule=0, time_filter='yes', offset=0,
-                description='-', check_grid='no', display=False)
-          -> Cube or None : wrapper of the operator OPH_SUBSET2. (Deprecated since Ophidia v1.1)
-        to_b2drop(cdd=None, auth_path='-', dst_path='-', ncores=1, export_metadata='yes')
-          -> None : method that integrates the features of OPH_EXPORTNC2 and OPH_B2DROP operators to upload a cube to B2DROP as a NetCDF file
-        unpublish( exec_mode='sync', display=False)
+        unpublish( exec_mode='sync', save='yes', display=False)
           -> None : wrapper of the operator OPH_UNPUBLISH
 
     Class Methods:
         setclient(username='', password='', server, port='11732', token='', read_env=False, api_mode=True, project=None)
           -> None : Instantiate the Client, common for all Cube objects, for submitting requests
-        b2drop(action='put', auth_path='-', src_path=None, dst_path='-', cdd=None, exec_mode='sync', display=False)
+        b2drop(action='put', auth_path='-', src_path=None, dst_path='-', cdd=None, exec_mode='sync', save='yes', display=False)
           -> None : wrapper of the operator OPH_B2DROP
         cancel(id=None, type='kill', objkey_filter='all', display=False)
           -> None : wrapper of the operator OPH_CANCEL
         cluster(action='info', nhost=1, host_partition='all', host_type='io', user_filter='all', exec_mode='sync', display=False)
           -> None : wrapper of the operator OPH_CLUSTER
-        containerschema(container=None, cwd=None, exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_CONTAINERSCHEMA
-        createcontainer(exec_mode='sync', container=None, cwd=None, dim=None, dim_type="double", hierarchy='oph_base', base_time='1900-01-01 00:00:00',
-                        units='d', calendar='standard', month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', leap_year=0, leap_month=2, vocabulary='CF',
-                        compressed='no', description='-', display=False)
+        containerschema(container=None, cwd=None, exec_mode='sync', objkey_filter='all', save='yes', display=True)
+          -> dict or None : wrapper of the operator OPH_CONTAINERSCHEMA
+        createcontainer(exec_mode='sync', container=None, cwd=None, dim=None, dim_type="double", hierarchy='oph_base',
+                        base_time='1900-01-01 00:00:00', units='d', calendar='standard',
+                        month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', leap_year=0, leap_month=2, vocabulary='CF',
+                        compressed='no', description='-', save='yes', display=False)
           -> None : wrapper of the operator OPH_CREATECONTAINER
-        deletecontainer(container=None, container_pid='-', force='no', cwd=None, nthreads=1, exec_mode='sync', objkey_filter='all', display=False)
+        deletecontainer(container=None, container_pid='-', force='no', cwd=None, nthreads=1, exec_mode='sync', objkey_filter='all',
+                        save='yes', display=False)
           -> None : wrapper of the operator OPH_DELETECONTAINER
-        explorenc(exec_mode='sync', schedule=0, measure='-', src_path=None, cdd=None, exp_dim='-', imp_dim='-', subset_dims='none', subset_type='index',
-                  subset_filter='all', limit_filter=100, show_index='no', show_id='no', show_time='no', show_stats='00000000000000', show_fit='no',
-                  level=0, imp_num_point=0, offset=50, operation='avg', wavelet='no', wavelet_ratio=0, wavelet_coeff='no', objkey_filter='all', display=True)
+        explorenc(exec_mode='sync', schedule=0, measure='-', src_path=None, cdd=None, exp_dim='-', imp_dim='-', subset_dims='none',
+                  subset_type='index', subset_filter='all', limit_filter=100, show_index='no', show_id='no', show_time='no',
+                  show_stats='00000000000000', show_fit='no', level=0, imp_num_point=0, offset=50, operation='avg', wavelet='no',
+                  wavelet_ratio=0, wavelet_coeff='no', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_EXPLORENC
-        folder(command=None, cwd=None, path=None, exec_mode='sync', display=False)
+        folder(command=None, cwd=None, path=None, exec_mode='sync', save='yes', display=False)
           -> None : wrapper of the operator OPH_FOLDER
-        fs(command='ls', dpath='-', file='-', cdd=None, recursive='no', depth=0, realpath='no', exec_mode='sync', display=False)
+        fs(command='ls', dpath='-', file='-', cdd=None, recursive='no', depth=0, realpath='no', exec_mode='sync', save='yes',
+           display=False)
           -> None : wrapper of the operator OPH_FS
         get_config(key='all', objkey_filter='all', display=True)
           -> dict or None : wrapper of the operator OPH_GET_CONFIG
-        hierarchy(hierarchy='all', hierarchy_version='latest', exec_mode='sync', objkey_filter='all', display=True)
+        hierarchy(hierarchy='all', hierarchy_version='latest', exec_mode='sync', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_HIERARCHY
-        importnc(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None, cdd=None, compressed='no',
-                 exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes', check_compliance='no', offset=0,
-                 ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes'
-                 subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
-                 leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-', policy='rr', schedule=0, check_grid='no')
+        importnc(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None,
+                 cdd=None, compressed='no', exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes',
+                 check_compliance='no', offset=0, ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none',
+                 subset_filter='all', time_filter='yes', subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00',
+                 calendar='standard', hierarchy='oph_base', leap_month=2, leap_year=0,
+                 month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-',
+                 policy='rr', schedule=0, check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_IMPORTNC
-        importnc2(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None, cdd=None, compressed='no',
-                 exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes', check_compliance='no', offset=0,
-                 ioserver='ophidiaio_memory', ncores=1, nthreads=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes'
-                 subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
-                 leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-', policy='rr', schedule=0, check_grid='no')
+        importnc2(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None,
+                  cdd=None, compressed='no', exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes',
+                  check_compliance='no', offset=0, ioserver='ophidiaio_memory', ncores=1, nthreads=1, nfrag=0, nhost=0,
+                  subset_dims='none', subset_filter='all', time_filter='yes', subset_type='index', exec_mode='sync',
+                  base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2, leap_year=0,
+                  month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-',
+                  policy='rr', schedule=0, check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_IMPORTNC2
         instances(action='read', level=1, host_filter='all', nhost=0, host_partition='all', ioserver_filter='all', host_status='all',
-                  exec_mode='sync', objkey_filter='all', display=True)
+                  exec_mode='sync', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_INSTANCES
         list(level=1, exec_mode='sync', path='-', cwd=None, container_filter='all', cube='all', host_filter='all', dbms_filter='all',
-             measure_filter='all', ntransform='all', src_filter='all', db_filter='all', recursive='no', objkey_filter='all', display=True)
+             measure_filter='all', ntransform='all', src_filter='all', db_filter='all', recursive='no', objkey_filter='all',
+             save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_LIST
         loggingbk(session_level=0, job_level=0, mask=000, session_filter='all', session_label_filter='all',
                   session_creation_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', workflowid_filter='all', markerid_filter='all',
                   parent_job_filter='all', job_creation_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', job_status_filter='all',
                   submission_string_filter='all', job_start_filter='1900-01-01 00:00:00,2100-01-01 00:00:00',
-                  job_end_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', nlines=100, objkey_filter='all', exec_mode='sync', display=True)
+                  job_end_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', nlines=100, objkey_filter='all', exec_mode='sync',
+                  save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_LOGGINGBK
-        log_info(log_type='server', container_id=0, ioserver='mysql', nlines=10, exec_mode='sync', objkey_filter='all', display=True)
+        log_info(log_type='server', container_id=0, ioserver='mysql', nlines=10, exec_mode='sync', objkey_filter='all',
+                 save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_LOG_INFO
-        man(function=None, function_type='operator', function_version='latest', exec_mode='sync', display=True)
+        man(function=None, function_type='operator', function_version='latest', exec_mode='sync', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_MAN
-        manage_session(action='list', session='this', key='user', value='null', objkey_filter='all', display=True)
+        manage_session(action='list', session='this', key='user', value='null', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_MANAGE_SESSION
-        mergecubes(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', mode='i', hold_values='no', number=1, order='none', description='-', display=False)
+        mergecubes(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', mode='i', hold_values='no', number=1,
+                   order='none', description='-', save='yes', display=False)
           -> Cube : wrapper of the operator OPH_MERGECUBES
-        mergecubes2(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', dim_type='long', number=1, order='none', description='-', dim='-', display=False)
+        mergecubes2(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', dim_type='long', number=1, order='none',
+                    description='-', dim='-', save='yes', display=False)
           -> Cube or None: wrapper of the operator OPH_MERGECUBES2
-        movecontainer(container=None, cwd=None, exec_mode='sync', display=False)
+        movecontainer(container=None, cwd=None, exec_mode='sync', save='yes', display=False)
           -> None : wrapper of the operator OPH_MOVECONTAINER
-        operators(operator_filter=None, limit_filter=0, exec_mode='sync', display=True)
+        operators(operator_filter=None, limit_filter=0, exec_mode='sync', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_OPERATORS_LIST
-        primitives(dbms_filter=None, level=1, limit_filter=0, primitive_filter=None, primitive_type=None, return_type=None, exec_mode='sync',
-                   objkey_filter='all', display=True)
+        primitives(dbms_filter=None, level=1, limit_filter=0, primitive_filter=None, primitive_type=None, return_type=None,
+                   exec_mode='sync', objkey_filter='all', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_PRIMITIVES_LIST
-        randcube(ncores=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='mysql_table', schedule=0, algorithm='default',
-                 policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None, exp_ndim=None, dim=None, concept_level='c',
-                 dim_size=None, compressed='no', grid='-', description='-', display=False)
+        randcube(ncores=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='mysql_table', schedule=0,
+                 algorithm='default', policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None,
+                 exp_ndim=None, dim=None, concept_level='c', dim_size=None, compressed='no', grid='-', description='-',
+                 save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_RANDCUBE
-        randcube2(ncores=1, nthreads=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='ophidiaio_memory', schedule=0, algorithm='default',
-                 policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None, exp_ndim=None, dim=None, concept_level='c',
-                 dim_size=None, compressed='no', grid='-', description='-', display=False)
+        randcube2(ncores=1, nthreads=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='ophidiaio_memory',
+                  schedule=0, algorithm='default', policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None,
+                  exp_ndim=None, dim=None, concept_level='c', dim_size=None, compressed='no', grid='-', description='-', save='yes',
+                  display=False)
           -> Cube or None : wrapper of the operator OPH_RANDCUBE2
-        resume( id=0, id_type='workflow', document_type='response', level=1, save='no', session='this', objkey_filter='all', user='', display=True)
+        resume(id=0, id_type='workflow', document_type='response', level=1, save='no', session='this', objkey_filter='all',
+               user='', display=True)
           -> dict or None : wrapper of the operator OPH_RESUME
-        script(script=':', args=' ', stdout='stdout', stderr='stderr', ncores=1, exec_mode='sync', list='no', space='no', python_code=False, display=False)
+        script(script=':', args=' ', stdout='stdout', stderr='stderr', ncores=1, exec_mode='sync', list='no', space='no',
+               python_code=False, save='yes', display=False)
           -> None : wrapper of the operator OPH_SCRIPT
-        search(path='-', metadata_value_filter='all', exec_mode='sync', metadata_key_filter='all', container_filter='all', objkey_filter='all',
-               cwd=None, recursive='no', display=True)
+        search(path='-', metadata_value_filter='all', exec_mode='sync', metadata_key_filter='all', container_filter='all',
+               objkey_filter='all', cwd=None, recursive='no', save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_SEARCH
-        service(status='', level=1, enable='all', disable='all', objkey_filter='all', display=False)
+        service(status='', level=1, enable='none', disable='none', objkey_filter='all', save='yes', display=False)
           -> dict or None : wrapper of the operator OPH_SERVICE
-        showgrid(container=None, grid='all', dim='all', show_index='no', cwd=None, exec_mode='sync', objkey_filter='all', display=True)
+        showgrid(container=None, grid='all', dim='all', show_index='no', cwd=None, exec_mode='sync', objkey_filter='all',
+                 save='yes', display=True)
           -> dict or None : wrapper of the operator OPH_SHOWGRID
-        tasks(cls, cube_filter='all', path='-', operator_filter='all', cwd=None, recursive='no', container='all', objkey_filter='all', exec_mode='sync', display=True)
-          -> dict or None : wrapper of the operator OPH_tasks
+        tasks(cls, cube_filter='all', path='-', operator_filter='all', cwd=None, recursive='no', container='all', objkey_filter='all',
+              exec_mode='sync', save='yes', display=True)
+          -> dict or None : wrapper of the operator OPH_TASKS
     """
 
     client = None
 
     @classmethod
     def setclient(cls, username="", password="", server="", port="11732", token="", read_env=False, api_mode=True, project=None):
         """setclient(username='', password='', server='', port='11732', token='', read_env=False, api_mode=True, project=None) -> None : Instantiate the Client, common for all Cube objects, for submitting requests
@@ -262,30 +287,32 @@
             cls.client = _client.Client(username, password, server, port, token, read_env, api_mode, project)
         except Exception as e:
             print(get_linenumber(), "Something went wrong in setting the client:", e)
         finally:
             pass
 
     @classmethod
-    def b2drop(cls, action="put", auth_path="-", src_path=None, dst_path="-", cdd=None, exec_mode="sync", display=False):
-        """b2drop(action='put', auth_path='-', src_path=None, dst_path='-', cdd=None, exec_mode='sync', display=False)
+    def b2drop(cls, action="put", auth_path="-", src_path=None, dst_path="-", cdd=None, exec_mode="sync", save="yes", display=False):
+        """b2drop(action='put', auth_path='-', src_path=None, dst_path='-', cdd=None, exec_mode='sync', save='yes', display=False)
           -> None : wrapper of the operator OPH_B2DROP
 
         :param action: put|get
         :type action: str
         :param auth_path: absolute path to the netrc file containing the B2DROP credentials
         :type auth_path: str
         :param src_path: path to the file to be uploaded/downloaded to/from B2DROP
         :type src_path: str
         :param dst_path: path where the file will be uploaded on B2DROP or downloaded on disk
         :type dst_path: str
         :param cdd: absolute path corresponding to the current directory on data repository
         :type cdd: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -303,14 +330,16 @@
                 query += "src_path=" + str(src_path) + ";"
             if dst_path is not None:
                 query += "dst_path=" + str(dst_path) + ";"
             if cdd is not None:
                 query += "cdd=" + str(cdd) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
@@ -361,26 +390,28 @@
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     @classmethod
-    def containerschema(cls, container=None, cwd=None, exec_mode="sync", objkey_filter="all", display=True):
-        """containerschema(container=None, cwd=None, exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_CONTAINERSCHEMA
+    def containerschema(cls, container=None, cwd=None, exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """containerschema(container=None, cwd=None, exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_CONTAINERSCHEMA
 
         :param container: container name
         :type container: str
         :param cwd: current working directory
         :type cwd: str
         :param exec_mode: async or sync
         :type exec_mode: str
         :param objkey_filter: filter on the output of the operator
         :type objkey_filter: str
-        :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
+        :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
         response = None
@@ -394,14 +425,16 @@
                 query += "container=" + str(container) + ";"
             if cwd is not None:
                 query += "cwd=" + str(cwd) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
@@ -424,19 +457,21 @@
         calendar="standard",
         month_lengths="31,28,31,30,31,30,31,31,30,31,30,31",
         leap_year=0,
         leap_month=2,
         vocabulary="CF",
         compressed="no",
         description="-",
+        save="yes",
         display=False,
     ):
         """createcontainer(exec_mode='sync', container=None, cwd=None, dim=None, dim_type="double", hierarchy='oph_base',
-                        base_time='1900-01-01 00:00:00', units='d', calendar='standard', month_lengths='31,28,31,30,31,30,31,31,30,31,30,31',
-                        leap_year=0, leap_month=2, vocabulary='CF', compressed='no', description='-', display=False) -> dict or None : wrapper of the operator OPH_CREATECONTAINER
+                           base_time='1900-01-01 00:00:00', units='d', calendar='standard',
+                           month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', leap_year=0, leap_month=2, vocabulary='CF',
+                           compressed='no', description='-', save='yes', display=False) -> dict or None : wrapper of the operator OPH_CREATECONTAINER
 
         :param exec_mode: async or sync
         :type exec_mode: str
         :param container: container name
         :type container: str
         :param cwd: current working directory
         :type cwd: str
@@ -460,14 +495,16 @@
         :type leap_month: int
         :param vocabulary: metadata vocabulary
         :type vocabulary: str
         :param compressed: yes or no
         :type compressed: str
         :param description: additional description to be associated with the output container
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -503,39 +540,43 @@
                 query += "leap_month=" + str(leap_month) + ";"
             if vocabulary is not None:
                 query += "vocabulary=" + str(vocabulary) + ";"
             if compressed is not None:
                 query += "compressed=" + str(compressed) + ";"
             if description is not None:
                 query += "description=" + str(description) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     @classmethod
-    def deletecontainer(cls, container=None, container_pid="-", force="no", cwd=None, nthreads=1, exec_mode="sync", objkey_filter="all", display=False):
-        """deletecontainer(container=None, container_pid='-', force='no', cwd=None, nthreads=1, exec_mode='sync', objkey_filter='all', display=False)
+    def deletecontainer(cls, container=None, container_pid="-", force="no", cwd=None, nthreads=1, exec_mode="sync", objkey_filter="all", save="yes", display=False):
+        """deletecontainer(container=None, container_pid='-', force='no', cwd=None, nthreads=1, exec_mode='sync', objkey_filter='all', save='yes', display=False)
              -> None : wrapper of the operator OPH_DELETECONTAINER
 
         :param container: container name
         :type container: str
         :param cwd: current working directory
         :type cwd: str
         :param container_pid: PID of the input container
         :type container_pid: str
         :param force: yes or no
         :type force: str
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -555,14 +596,16 @@
                 query += "cwd=" + str(cwd) + ";"
             if nthreads is not None:
                 query += "nthreads=" + str(nthreads) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
@@ -601,24 +644,24 @@
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     @classmethod
-    def service(cls, status="", level=1, enable="all", disable="all", objkey_filter="all", display=False):
-        """service(status='', level=1, enable='all', disable='all', objkey_filter='all', display=False) -> dict or None : wrapper of the operator OPH_SERVICE
+    def service(cls, status="", level=1, enable="none", disable="none", objkey_filter="all", display=False):
+        """service(status='', level=1, enable='none', disable='none', objkey_filter='all', display=False) -> dict or None : wrapper of the operator OPH_SERVICE
 
         :param status: up|down
         :type status: str
         :param level: 1|2
         :type level: int
-        :param enable: list of the users to be enabled
+        :param enable: list of the users to be enabled ('all' to enable all users)
         :type enable: str
-        :param disable: list of the users to be disabled
+        :param disable: list of the users to be disabled ('all' to disable all users)
         :type disable: str
         :param objkey_filter: filter the objkey
         :type objkey_filter: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
@@ -689,27 +732,29 @@
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def manage_session(cls, action="list", session="this", key="user", value="null", objkey_filter="all", display=True):
-        """manage_session(action='list', session='this', key='user', value='null', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_MANAGE_SESSION
+    def manage_session(cls, action="list", session="this", key="user", value="null", objkey_filter="all", save="yes", display=True):
+        """manage_session(action='list', session='this', key='user', value='null', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_MANAGE_SESSION
 
         :param action: disable|enable|env|grant|list|listusers|new|remove|revoke|setenv
         :type action: str
         :param session: link to intended session
         :type session: str
         :param key: active|autoremove|label|user
         :type key: str
         :param value:  value of the key
         :type value: str
         :param objkey_filter: filter the objkey
         :type objkey_filter: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -726,30 +771,34 @@
                 query += "session=" + str(session) + ";"
             if key is not None:
                 query += "key=" + str(key) + ";"
             if value is not None:
                 query += "value=" + str(value) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def instances(cls, action="read", level=1, host_filter="all", nhost=0, host_partition="all", ioserver_filter="all", host_status="all", exec_mode="sync", objkey_filter="all", display=True):
-        """instances(level=1, action='read', level=1, host_filter='all', nhost=0, host_partition='all', ioserver_filter='all', host_status='all',
-                     exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_INSTANCES
+    def instances(
+        cls, action="read", level=1, host_filter="all", nhost=0, host_partition="all", ioserver_filter="all", host_status="all", exec_mode="sync", objkey_filter="all", save="yes", display=True
+    ):
+        """instances(level=1, action='read', level=1, host_filter='all', nhost=0, host_partition='all', ioserver_filter='all',
+                     host_status='all', exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_INSTANCES
 
         :param action: read|add|remove
         :type action: str
         :param level: 1|2|3
         :type level: int
         :param host_filter: optional filter on host name
         :type host_filter: str
@@ -761,14 +810,16 @@
         :type ioserver_filter: str
         :param host_status: up|down|all
         :type host_status: str
         :param exec_mode: async or sync
         :type exec_mode: str
         :param objkey_filter: filter the objkey
         :type objkey_filter: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -793,42 +844,46 @@
                 query += "ioserver_filter=" + str(ioserver_filter) + ";"
             if host_status is not None:
                 query += "host_status=" + str(host_status) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def log_info(cls, log_type="server", container_id=0, ioserver="mysql", nlines=10, exec_mode="sync", objkey_filter="all", display=True):
-        """log_info(log_type='server', container_id=0, ioserver='mysql', nlines=10, exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_LOG_INFO
+    def log_info(cls, log_type="server", container_id=0, ioserver="mysql", nlines=10, exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """log_info(log_type='server', container_id=0, ioserver='mysql', nlines=10, exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_LOG_INFO
 
         :param log_type: server|container|ioserver
         :type log_type: str
         :param container_id: id of the container related to the requested log
         :type container_id: int
         :param ioserver: mysql|ophidiaio
         :type ioserver: str
         :param nlines: maximum number of lines to be displayed
         :type nlines: int
         :param objkey_filter: filter the objkey
         :type objkey_filter: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
         response = None
@@ -846,14 +901,16 @@
                 query += "ioserver=" + str(ioserver) + ";"
             if nlines is not None:
                 query += "nlines=" + str(nlines) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
@@ -878,21 +935,23 @@
         job_status_filter="all",
         submission_string_filter="all",
         job_start_filter="1900-01-01 00:00:00,2100-01-01 00:00:00",
         job_end_filter="1900-01-01 00:00:00,2100-01-01 00:00:00",
         nlines=100,
         objkey_filter="all",
         exec_mode="sync",
+        save="yes",
         display=True,
     ):
         """loggingbk(session_level=0, job_level=0, mask=000, session_filter='all', session_label_filter='all',
                      session_creation_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', workflowid_filter='all', markerid_filter='all',
                      parent_job_filter='all', job_creation_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', job_status_filter='all',
                      submission_string_filter='all', job_start_filter='1900-01-01 00:00:00,2100-01-01 00:00:00',
-                     job_end_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', nlines=100, objkey_filter='all', exec_mode='sync', display=True)
+                     job_end_filter='1900-01-01 00:00:00,2100-01-01 00:00:00', nlines=100, objkey_filter='all', exec_mode='sync',
+                     save='yes', display=True)
              -> dict or None : wrapper of the operator OPH_LOGGINGBK
 
         :param session_level: 0|1
         :type session_level: int
         :param job_level: 0|1|2
         :type job_level: int
         :param mask: 3-digit mask for job output
@@ -919,14 +978,16 @@
         :type job_start_filter: str
         :param job_end_filter: filter on job end date as with session_creation_filter
         :type job_end_filter: str
         :param nlines: maximum number of lines to be displayed
         :type nlines: int
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
         response = None
@@ -966,38 +1027,42 @@
                 query += "job_start_filter=" + str(job_start_filter) + ";"
             if job_end_filter is not None:
                 query += "job_end_filter=" + str(job_end_filter) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def folder(cls, command=None, path="-", cwd=None, exec_mode="sync", objkey_filter="all", display=False):
-        """folder(command=None, cwd=None, path=None, exec_mode='sync', display=False) -> None : wrapper of the operator OPH_FOLDER
+    def folder(cls, command=None, path="-", cwd=None, exec_mode="sync", objkey_filter="all", save="yes", display=False):
+        """folder(command=None, cwd=None, path=None, exec_mode='sync', save='yes', display=False) -> None : wrapper of the operator OPH_FOLDER
 
         :param command: cd|mkdir|mv|rm
         :type command: str
         :param cwd: current working directory
         :type cwd: str
         :param path: absolute or relative path
         :type path: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -1013,25 +1078,28 @@
                 query += "path=" + str(path) + ";"
             if cwd is not None:
                 query += "cwd=" + str(cwd) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     @classmethod
-    def fs(cls, command="ls", dpath="-", file="-", cdd=None, recursive="no", depth=0, realpath="no", exec_mode="sync", objkey_filter="all", display=False):
-        """fs(command='ls', dpath='-', file='-', cdd=None, recursive='no', depth=0, realpath='no', exec_mode='sync', objkey_filter='all', display=False) -> None : wrapper of the operator OPH_FS
+    def fs(cls, command="ls", dpath="-", file="-", cdd=None, recursive="no", depth=0, realpath="no", exec_mode="sync", objkey_filter="all", save="yes", display=False):
+        """fs(command='ls', dpath='-', file='-', cdd=None, recursive='no', depth=0, realpath='no', exec_mode='sync',
+              objkey_filter='all', save='yes', display=False) -> None : wrapper of the operator OPH_FS
 
         :param command: ls|cd|mkdir|rm|mv
         :type command: str
         :param dpath: paths needed by commands
         :type dpath: str
         :param file: file filter
         :type file: str
@@ -1041,14 +1109,16 @@
         :type recursive: str
         :param depth: maximum folder depth to be explored in case of recursion
         :type depth: int
         :param realpath: yes|no
         :type realpath: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -1072,25 +1142,28 @@
                 query += "depth=" + str(depth) + ";"
             if realpath is not None:
                 query += "realpath=" + str(realpath) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     @classmethod
-    def tasks(cls, cube_filter="all", operator_filter="all", path="-", cwd=None, recursive="no", container="all", exec_mode="sync", objkey_filter="all", display=True):
-        """tasks(cls, cube_filter='all', path='-', operator_filter='all', cwd=None, recursive='no',  container='all', objkey_filter='all', exec_mode='sync', display=True)
+    def tasks(cls, cube_filter="all", operator_filter="all", path="-", cwd=None, recursive="no", container="all", exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """tasks(cls, cube_filter='all', path='-', operator_filter='all', cwd=None, recursive='no', container='all',
+                 objkey_filter='all', exec_mode='sync', save='yes', display=True)
              -> dict or None : wrapper of the operator OPH_tasks
 
         :param cube_filter: optional filter on cube
         :type cube_filter: str
         :param operator_filter: optional filter on the name of the operators
         :type operator_filter: str
         :param path: optional filter on absolute or relative path
@@ -1099,14 +1172,16 @@
         :type cwd: str
         :param recursive: if the search is done recursively or not
         :type recursive: yes|no
         :param container: optional filter on container name
         :type container: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
         response = None
@@ -1128,42 +1203,47 @@
                 query += "recursive=" + str(recursive) + ";"
             if container is not None:
                 query += "container=" + str(container) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def showgrid(cls, container=None, grid="all", dim="all", show_index="no", cwd=None, exec_mode="sync", objkey_filter="all", display=True):
-        """showgrid(container=None, grid='all', dim='all', show_index='no', cwd=None, exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_SHOWGRID
+    def showgrid(cls, container=None, grid="all", dim="all", show_index="no", cwd=None, exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """showgrid(container=None, grid='all', dim='all', show_index='no', cwd=None, exec_mode='sync', objkey_filter='all',
+                    save='yes', display=True) -> dict or None : wrapper of the operator OPH_SHOWGRID
 
         :param container: name of the input container
         :type container: str
         :param grid: name of grid to show
         :type grid: str
         :param dim: name of dimension to show
         :type dim: str
         :param show_index: yes|no
         :type show_index: str
         :param cwd: current working directory
         :type cwd: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -1184,29 +1264,34 @@
                 query += "show_index=" + str(show_index) + ";"
             if cwd is not None:
                 query += "cwd=" + str(cwd) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def search(cls, container_filter="all", metadata_key_filter="all", metadata_value_filter="all", path="-", cwd=None, recursive="no", exec_mode="sync", objkey_filter="all", display=True):
-        """search(path='-', metadata_value_filter='all', exec_mode='sync', metadata_key_filter='all', container_filter='all', objkey_filter='all', cwd=None,  recursive='no', display=True)
+    def search(
+        cls, container_filter="all", metadata_key_filter="all", metadata_value_filter="all", path="-", cwd=None, recursive="no", exec_mode="sync", objkey_filter="all", save="yes", display=True
+    ):
+        """search(path='-', metadata_value_filter='all', exec_mode='sync', metadata_key_filter='all', container_filter='all',
+                 objkey_filter='all', cwd=None, recursive='no', save='yes', display=True)
              -> dict or None : wrapper of the operator OPH_SEARCH
 
         :param container_filter: filter on container name
         :type container_filter: str
         :param metadata_key_filter: name of the key (or the enumeration of keys) identifying requested metadata
         :type metadata_key_filter: str
         :param metadata_value_filter: value of the key (or the enumeration of keys) identifying requested metadata
@@ -1215,14 +1300,16 @@
         :type path: str
         :param cwd: current working directory
         :type cwd: str
         :param recursive: if the search is done recursively or not
         :type recursive: yes|no
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -1245,36 +1332,40 @@
                 query += "cwd=" + str(cwd) + ";"
             if recursive is not None:
                 query += "recursive=" + str(recursive) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def hierarchy(cls, hierarchy="all", hierarchy_version="latest", exec_mode="sync", objkey_filter="all", display=True):
-        """hierarchy(hierarchy='all', hierarchy_version='latest', exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_HIERARCHY
+    def hierarchy(cls, hierarchy="all", hierarchy_version="latest", exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """hierarchy(hierarchy='all', hierarchy_version='latest', exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_HIERARCHY
 
         :param hierarchy: name of the requested hierarchy
         :type hierarchy: str
         :param hierarchy_version: version of the requested hierarchy
         :type hierarchy_version: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -1289,14 +1380,16 @@
                 query += "hierarchy=" + str(hierarchy) + ";"
             if hierarchy_version is not None:
                 query += "hierarchy_version=" + str(hierarchy_version) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
@@ -1318,18 +1411,20 @@
         dbms_filter="all",
         measure_filter="all",
         ntransform="all",
         src_filter="all",
         db_filter="all",
         recursive="no",
         objkey_filter="all",
+        save="yes",
         display=True,
     ):
-        """list(level=1, exec_mode='sync', path='-', cwd=None, container_filter='all', cube='all', host_filter='all', dbms_filter='all', measure_filter='all',
-                ntransform='all', src_filter='all', db_filter='all', recursive='no', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_LIST
+        """list(level=1, exec_mode='sync', path='-', cwd=None, container_filter='all', cube='all', host_filter='all', dbms_filter='all',
+                measure_filter='all', ntransform='all', src_filter='all', db_filter='all', recursive='no', objkey_filter='all',
+                save='yes', display=True) -> dict or None : wrapper of the operator OPH_LIST
 
         :param level: 0|1|2|3|4|5|6|7|8
         :type level: int
         :param path: absolute or relative path
         :type path: str
         :param container_filter: filter on container name
         :type container_filter: str
@@ -1349,14 +1444,16 @@
         :type src_filter: str
         :param recursive: yes|no
         :type recursive: str
         :param cwd: current working directory
         :type cwd: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -1391,14 +1488,16 @@
                 query += "src_filter=" + str(src_filter) + ";"
             if db_filter is not None:
                 query += "db_filter=" + str(db_filter) + ";"
             if recursive is not None:
                 query += "recursive=" + str(recursive) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
@@ -1428,19 +1527,21 @@
         exp_ndim=None,
         dim=None,
         concept_level="c",
         dim_size=None,
         compressed="no",
         grid="-",
         description="-",
+        save="yes",
         display=False,
     ):
-        """randcube(ncores=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='mysql_table', schedule=0, algorithm='default',
-                 policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None, exp_ndim=None, dim=None, concept_level='c',
-                 dim_size=None, compressed='no', grid='-', description='-', display=False) -> Cube or None : wrapper of the operator OPH_RANDCUBE
+        """randcube(ncores=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='mysql_table', schedule=0,
+                    algorithm='default', policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None,
+                    exp_ndim=None, dim=None, concept_level='c', dim_size=None, compressed='no', grid='-', description='-',
+                    save='yes', display=False) -> Cube or None : wrapper of the operator OPH_RANDCUBE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param container: container name
         :type container: str
@@ -1478,14 +1579,16 @@
         :type dim_size: str
         :param compressed: yes|no
         :type compressed: str
         :param grid: optionally group dimensions in a grid
         :type grid: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: obj or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -1546,14 +1649,16 @@
             query += "dim_size=" + str(dim_size) + ";"
         if compressed is not None:
             query += "compressed=" + str(compressed) + ";"
         if grid is not None:
             query += "grid=" + str(grid) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
@@ -1586,19 +1691,21 @@
         exp_ndim=None,
         dim=None,
         concept_level="c",
         dim_size=None,
         compressed="no",
         grid="-",
         description="-",
+        save="yes",
         display=False,
     ):
-        """randcube2(ncores=1, nthreads=1, exec_mode='sync', container=None, cwd=None, host_partition='auto', ioserver='ophidiaio_memory', schedule=0, algorithm='default',
-                 policy='rr', nhost=0, run='yes', nfrag=1, ntuple=1, measure=None, measure_type=None, exp_ndim=None, dim=None, concept_level='c',
-                 dim_size=None, compressed='no', grid='-', description='-', display=False) -> Cube or None : wrapper of the operator OPH_RANDCUBE2
+        """randcube2(ncores=1, nthreads=1, exec_mode='sync', container=None, cwd=None, host_partition='auto',
+                    ioserver='ophidiaio_memory', schedule=0, algorithm='default', policy='rr', nhost=0, run='yes', nfrag=1,
+                    ntuple=1, measure=None, measure_type=None, exp_ndim=None, dim=None, concept_level='c', dim_size=None,
+                    compressed='no', grid='-', description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_RANDCUBE2
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
@@ -1638,14 +1745,16 @@
         :type dim_size: str
         :param compressed: yes|no
         :type compressed: str
         :param grid: optionally group dimensions in a grid
         :type grid: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: obj or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -1708,14 +1817,16 @@
             query += "dim_size=" + str(dim_size) + ";"
         if compressed is not None:
             query += "compressed=" + str(compressed) + ";"
         if grid is not None:
             query += "grid=" + str(grid) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
@@ -1749,19 +1860,21 @@
         imp_num_point=0,
         offset=50,
         operation="avg",
         wavelet="no",
         wavelet_ratio=0,
         wavelet_coeff="no",
         objkey_filter="all",
+        save="yes",
         display=True,
     ):
-        """explorenc(exec_mode='sync', schedule=0, measure='-', src_path=None, cdd=None, exp_dim='-', imp_dim='-', subset_dims='none', subset_type='index', subset_filter='all', limit_filter=100,
-                     show_index='no', show_id='no', show_time='no', show_stats='00000000000000', show_fit='no', level=0, imp_num_point=0, offset=50, operation='avg', wavelet='no', wavelet_ratio=0,
-                     wavelet_coeff='no', objkey_filter='all', display=True)
+        """explorenc(exec_mode='sync', schedule=0, measure='-', src_path=None, cdd=None, exp_dim='-', imp_dim='-', subset_dims='none',
+                     subset_type='index', subset_filter='all', limit_filter=100, show_index='no', show_id='no', show_time='no',
+                     show_stats='00000000000000', show_fit='no', level=0, imp_num_point=0, offset=50, operation='avg', wavelet='no',
+                     wavelet_ratio=0, wavelet_coeff='no', objkey_filter='all', save='yes', display=True)
              -> None : wrapper of the operator OPH_EXPLORENC
 
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param measure: name of the measure related to the NetCDF file
@@ -1802,14 +1915,16 @@
         :type operation: str
         :param wavelet: yes|no|only
         :type wavelet: str
         :param wavelet_ratio: fraction of wavelet transform coefficients that are cleared by the filter (percentage)
         :type wavelet_ratio: float
         :param wavelet_coeff: yes|no
         :type wavelet_coeff: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -1864,14 +1979,16 @@
                 query += "wavelet=" + str(wavelet) + ";"
             if wavelet_ratio is not None:
                 query += "wavelet_ratio=" + str(wavelet_ratio) + ";"
             if wavelet_coeff is not None:
                 query += "wavelet_coeff=" + str(wavelet_coeff) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
@@ -1916,22 +2033,24 @@
         run="yes",
         units="d",
         vocabulary="CF",
         description="-",
         policy="rr",
         schedule=0,
         check_grid="no",
+        save="yes",
         display=False,
     ):
-        """importnc(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None,  cdd=None, compressed='no',
-                    exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes', check_compliance='no', offset=0,
-                    ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes'
-                    subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
-                    leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-', policy='rr', schedule=0,
-                    check_grid='no')
+        """importnc(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None,
+                    cdd=None, compressed='no', exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes',
+                    check_compliance='no', offset=0, ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none',
+                    subset_filter='all', time_filter='yes', subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00',
+                    calendar='standard', hierarchy='oph_base', leap_month=2, leap_year=0,
+                    month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-',
+                    policy='rr', schedule=0, check_grid='no', save='yes', display=False)
              -> Cube or None : wrapper of the operator OPH_IMPORTNC
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
@@ -2000,14 +2119,16 @@
         :type vocabulary: str
         :param description: additional description to be associated with the output cube
         :type description: str
         :param policy: rule to select how data are distribuited over hosts (rr|port)
         :type policy: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: obj or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -2087,14 +2208,16 @@
             query += "leap_month=" + str(leap_month) + ";"
         if policy is not None:
             query += "policy=" + str(policy) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
@@ -2142,21 +2265,24 @@
         run="yes",
         units="d",
         vocabulary="CF",
         description="-",
         policy="rr",
         schedule=0,
         check_grid="no",
+        save="yes",
         display=False,
     ):
-        """importnc2(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None, cdd=None, compressed='no',
-                 exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes', check_compliance='no', offset=0,
-                 ioserver='ophidiaio_memory', ncores=1, nthreads=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes'
-                 subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
-                 leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF', description='-', policy='rr', schedule=0, check_grid='no')
+        """importnc2(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None,
+                     cdd=None, compressed='no', exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='yes',
+                     check_compliance='no', offset=0, ioserver='ophidiaio_memory', ncores=1, nthreads=1, nfrag=0, nhost=0,
+                     subset_dims='none', subset_filter='all', time_filter='yes', subset_type='index', exec_mode='sync',
+                     base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
+                     leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='CF',
+                     description='-', policy='rr', schedule=0, check_grid='no', save='yes', display=False)
           -> Cube or None : wrapper of the operator OPH_IMPORTNC2
 
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
@@ -2228,14 +2354,16 @@
         :type vocabulary: str
         :param policy: rule to select how data are distribuited over hosts (rr|port)
         :type policy: str
         :param description: additional description to be associated with the output cube
         :type description: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: obj or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -2317,14 +2445,16 @@
             query += "leap_month=" + str(leap_month) + ";"
         if policy is not None:
             query += "policy=" + str(policy) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
@@ -2332,25 +2462,27 @@
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
     @classmethod
-    def man(cls, function=None, function_version="latest", function_type="operator", exec_mode="sync", objkey_filter="all", display=True):
-        """man(function=None, function_type='operator', function_version='latest', exec_mode='sync', display=True) -> dict or None : wrapper of the operator OPH_MAN
+    def man(cls, function=None, function_version="latest", function_type="operator", exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """man(function=None, function_type='operator', function_version='latest', exec_mode='sync', save='yes', display=True) -> dict or None : wrapper of the operator OPH_MAN
 
         :param function: operator or primitive name
         :type function: str
         :param function_type: operator|primitive
         :type function_type: str
         :param function_version: operator or primitive version
         :type function_version: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -2367,36 +2499,40 @@
                 query += "function_version=" + str(function_version) + ";"
             if function_type is not None:
                 query += "function_type=" + str(function_type) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def movecontainer(cls, container=None, cwd=None, exec_mode="sync", display=False):
-        """movecontainer(container=None, cwd=None, exec_mode='sync', display=False) -> None : wrapper of the operator OPH_MOVECONTAINER
+    def movecontainer(cls, container=None, cwd=None, exec_mode="sync", save="yes", display=False):
+        """movecontainer(container=None, cwd=None, exec_mode='sync', save='yes', display=False) -> None : wrapper of the operator OPH_MOVECONTAINER
 
         :param container: container name
         :type container: str
         :param cwd: current working directory
         :type cwd: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -2408,32 +2544,36 @@
 
             if container is not None:
                 query += "container=" + str(container) + ";"
             if cwd is not None:
                 query += "cwd=" + str(cwd) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     @classmethod
-    def operators(cls, operator_filter=None, limit_filter=0, exec_mode="sync", objkey_filter="all", display=True):
-        """operators(operator_filter=None, limit_filter=0, exec_mode='sync', display=True) -> dict or None : wrapper of the operator OPH_OPERATORS_LIST
+    def operators(cls, operator_filter=None, limit_filter=0, exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """operators(operator_filter=None, limit_filter=0, exec_mode='sync', save='yes', display=True) -> dict or None : wrapper of the operator OPH_OPERATORS_LIST
 
         :param operator_filter: filter on operator name
         :type operator_filter: str
         :param limit_filter: max number of lines
         :type limit_filter: int
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -2448,29 +2588,31 @@
                 query += "operator_filter=" + str(operator_filter) + ";"
             if limit_filter is not None:
                 query += "limit_filter=" + str(limit_filter) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def primitives(cls, level=1, dbms_filter=None, return_type="all", primitive_type="all", primitive_filter="", limit_filter=0, exec_mode="sync", objkey_filter="all", display=True):
-        """primitives(dbms_filter=None, level=1, limit_filter=0, primitive_filter=None, primitive_type=None, return_type=None, exec_mode='sync', objkey_filter='all', display=True) ->
+    def primitives(cls, level=1, dbms_filter=None, return_type="all", primitive_type="all", primitive_filter="", limit_filter=0, exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """primitives(dbms_filter=None, level=1, limit_filter=0, primitive_filter=None, primitive_type=None, return_type=None, exec_mode='sync', objkey_filter='all', save='yes', display=True) ->
            dict or None : wrapper of the operator OPH_PRIMITIVES_LIST
 
         :param dbms_filter: filter on DBMS
         :type dbms_filter: str
         :param level: 1|2|3|4|5
         :type level: int
         :param limit_filter: max number of lines
@@ -2479,14 +2621,16 @@
         :type primitive_filter: str
         :param primitive_type: all|simple|aggregate
         :type primitive_type: str
         :param return_type: all|array|number
         :type return_type: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -2509,29 +2653,31 @@
                 query += "primitive_filter=" + str(primitive_filter) + ";"
             if limit_filter is not None:
                 query += "limit_filter=" + str(limit_filter) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def script(cls, script=":", args=" ", stdout="stdout", stderr="stderr", list="no", space="no", python_code=False, exec_mode="sync", ncores=1, display=False):
-        """script(script=':', args=' ', stdout='stdout', stderr='stderr', ncores=1, exec_mode='sync', list='no', space='no', python_code=False, display=False) -> None : wrapper of the operator OPH_SCRIPT
+    def script(cls, script=":", args=" ", stdout="stdout", stderr="stderr", list="no", space="no", python_code=False, exec_mode="sync", ncores=1, save="yes", display=False):
+        """script(script=':', args=' ', stdout='stdout', stderr='stderr', ncores=1, exec_mode='sync', list='no', space='no', python_code=False, save='yes', display=False) -> None : wrapper of the operator OPH_SCRIPT
 
         :param script: script/executable filename
         :type script: str
         :param args: pipe (|) separated list of arguments for the script
         :type args: str
         :param stdout: file/stream where stdout is redirected
         :type stdout: str
@@ -2543,14 +2689,16 @@
         :type space: str
         :param python_code: yes|no
         :type python_code: bool
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -2643,14 +2791,16 @@
                 query += "list=" + str(list) + ";"
             if space is not None:
                 query += "space=" + str(space) + ";"
             if exec_mode is not None:
                 query += "exec_mode=" + str(exec_mode) + ";"
             if ncores is not None:
                 query += "ncores=" + str(ncores) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 if script is not None and python_code:
                     os.remove(script_path)
 
                 raise RuntimeError()
 
@@ -2707,29 +2857,31 @@
                 query += "user=" + str(user) + ";"
             if status_filter is not None:
                 query += "status_filter=" + str(status_filter) + ";"
             if save is not None:
                 query += "save=" + str(save) + ";"
             if objkey_filter is not None:
                 query += "objkey_filter=" + str(objkey_filter) + ";"
+            if save is not None:
+                query += "save=" + str(save) + ";"
 
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None and display is False:
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
     @classmethod
-    def mergecubes(cls, ncores=1, exec_mode="sync", cubes=None, schedule=0, container="-", mode="i", hold_values="no", number=1, order="none", description="-", display=False):
-        """mergecubes(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', mode='i', hold_values='no', number=1, order='none', description='-', display=False) -> Cube : wrapper of the operator OPH_MERGECUBES
+    def mergecubes(cls, ncores=1, exec_mode="sync", cubes=None, schedule=0, container="-", mode="i", hold_values="no", number=1, order="none", description="-", save="yes", display=False):
+        """mergecubes(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', mode='i', hold_values='no', number=1, order='none', description='-', save='yes', display=False) -> Cube : wrapper of the operator OPH_MERGECUBES
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
@@ -2743,14 +2895,16 @@
         :type hold_values: str
         :param number: number of replies of the first cube
         :type number: int
         :param order: criteria on which input cubes are ordered before merging
         :type order: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -2776,14 +2930,16 @@
             query += "hold_values=" + str(hold_values) + ";"
         if number is not None:
             query += "number=" + str(number) + ";"
         if order is not None:
             query += "order=" + str(order) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
@@ -2791,16 +2947,16 @@
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
     @classmethod
-    def mergecubes2(cls, ncores=1, exec_mode="sync", cubes=None, schedule=0, container="-", dim_type="long", number=1, order="none", description="-", dim="-", display=False):
-        """mergecubes2(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', dim_type='long', number=1, order='none', description='-', dim='-', display=False) -> Cube or None: wrapper of the operator OPH_MERGECUBES2
+    def mergecubes2(cls, ncores=1, exec_mode="sync", cubes=None, schedule=0, container="-", dim_type="long", number=1, order="none", description="-", dim="-", save="yes", display=False):
+        """mergecubes2(ncores=1, exec_mode='sync', cubes=None, schedule=0, container='-', dim_type='long', number=1, order='none', description='-', dim='-', save='yes', display=False) -> Cube or None: wrapper of the operator OPH_MERGECUBES2
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
@@ -2814,14 +2970,16 @@
         :type number: int
         :param order: criteria on which input cubes are ordered before merging
         :type order: str
         :param description: additional description to be associated with the output cube
         :type description: str
         :param dim: name of the new dimension to be created
         :type dim: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -2847,14 +3005,16 @@
             query += "order=" + str(order) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if dim_type is not None:
             query += "dim_type=" + str(dim_type) + ";"
         if dim is not None:
             query += "dim=" + str(dim) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
@@ -2901,22 +3061,23 @@
         units="d",
         vocabulary="-",
         description="-",
         policy="rr",
         schedule=0,
         pid=None,
         check_grid="no",
+        save="yes",
         display=False,
     ):
-        """Cube(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None, cdd=None, compressed='no',
-                exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='no', check_compliance='no', offset=0,
-                ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes'
-                subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base', leap_month=2,
-                leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='-', description='-', policy='rr', schedule=0,
-                pid=None, check_grid='no', display=False) -> obj
+        """Cube(container='-', cwd=None, exp_dim='auto', host_partition='auto', imp_dim='auto', measure=None, src_path=None, cdd=None,
+                compressed='no', exp_concept_level='c', grid='-', imp_concept_level='c', import_metadata='no', check_compliance='no',
+                offset=0, ioserver='mysql_table', ncores=1, nfrag=0, nhost=0, subset_dims='none', subset_filter='all', time_filter='yes',
+                subset_type='index', exec_mode='sync', base_time='1900-01-01 00:00:00', calendar='standard', hierarchy='oph_base',
+                leap_month=2, leap_year=0, month_lengths='31,28,31,30,31,30,31,31,30,31,30,31', run='yes', units='d', vocabulary='-',
+                description='-', policy='rr', schedule=0, pid=None, check_grid='no', save='yes', display=False) -> obj
              or Cube(pid=None) -> obj
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
@@ -2987,14 +3148,16 @@
         :type description: str
         :param policy: rule to select how data are distribuited over hosts (rr|port)
         :type policy: str
         :param pid: PID of an existing cube (if used all other parameters are ignored)
         :type pid: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: obj or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3096,14 +3259,16 @@
                         query += "schedule=" + str(schedule) + ";"
                     if policy is not None:
                         query += "policy=" + str(policy) + ";"
                     if description is not None:
                         query += "description=" + str(description) + ";"
                     if check_grid is not None:
                         query += "check_grid=" + str(check_grid) + ";"
+                    if save is not None:
+                        query += "save=" + str(save) + ";"
 
                     try:
                         if Cube.client.submit(query, display) is None:
                             raise RuntimeError()
 
                         if Cube.client.last_response is not None:
                             if Cube.client.cube:
@@ -3179,16 +3344,16 @@
                         element["hierarchy"] = row_i[3]
                         element["concept_level"] = row_i[4]
                         element["array"] = row_i[5]
                         element["level"] = row_i[6]
                         element["lattice_name"] = row_i[7]
                         self.dim_info.append(element)
 
-    def exportnc(self, misc="no", output_path="default", output_name="default", cdd=None, force="no", export_metadata="yes", schedule=0, exec_mode="sync", ncores=1, display=False):
-        """exportnc(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0, exec_mode='sync', ncores=1, display=False)
+    def exportnc(self, misc="no", output_path="default", output_name="default", cdd=None, force="no", export_metadata="yes", schedule=0, exec_mode="sync", ncores=1, save="yes", display=False):
+        """exportnc(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0, exec_mode='sync', ncores=1, save='yes', display=False)
              -> None : wrapper of the operator OPH_EXPORTNC
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
@@ -3201,14 +3366,16 @@
         :type cdd: str
         :param force: yes|no
         :type force: str
         :param output_path: directory of the output file
         :type output_path: str
         :param output_name: name of the output file
         :type output_name: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -3231,26 +3398,28 @@
             query += "export_metadata=" + str(export_metadata) + ";"
         if schedule is not None:
             query += "schedule=" + str(schedule) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if ncores is not None:
             query += "ncores=" + str(ncores) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
-    def exportnc2(self, misc="no", output_path="default", output_name="default", cdd=None, force="no", export_metadata="yes", schedule=0, exec_mode="sync", ncores=1, display=False):
-        """exportnc2(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0, exec_mode='sync', ncores=1, display=False)
+    def exportnc2(self, misc="no", output_path="default", output_name="default", cdd=None, force="no", export_metadata="yes", schedule=0, exec_mode="sync", ncores=1, save="yes", display=False):
+        """exportnc2(misc='no', output_path='default', output_name='default', cdd=None, force='no', export_metadata='yes', schedule=0, exec_mode='sync', ncores=1, save='yes', display=False)
              -> None : wrapper of the operator OPH_EXPORTNC2
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
@@ -3263,14 +3432,16 @@
         :type cdd: str
         :param force: yes|no
         :type force: str
         :param output_path: directory of the output file
         :type output_path: str
         :param output_name: name of the output file
         :type output_name: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -3293,28 +3464,43 @@
             query += "export_metadata=" + str(export_metadata) + ";"
         if schedule is not None:
             query += "schedule=" + str(schedule) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if ncores is not None:
             query += "ncores=" + str(ncores) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     def aggregate(
-        self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, group_size="all", operation=None, missingvalue="NAN", grid="-", container="-", description="-", check_grid="no", display=False
+        self,
+        ncores=1,
+        nthreads=1,
+        exec_mode="sync",
+        schedule=0,
+        group_size="all",
+        operation=None,
+        missingvalue="-",
+        grid="-",
+        container="-",
+        description="-",
+        check_grid="no",
+        save="yes",
+        display=False,
     ):
-        """aggregate( ncores=1, nthreads=1, exec_mode='sync', schedule=0, group_size='all', operation=None, missingvalue='NAN', grid='-', container='-', description='-', check_grid='no', display=False)
+        """aggregate( ncores=1, nthreads=1, exec_mode='sync', schedule=0, group_size='all', operation=None, missingvalue='-', grid='-', container='-', description='-', check_grid='no', save='yes', display=False)
              -> Cube or None : wrapper of the operator OPH_AGGREGATE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
@@ -3325,20 +3511,22 @@
         :type operation: str
         :param container: optional container name
         :type container: str
         :param grid: optionally group dimensions in a grid
         :type grid: str
         :param group_size: number of tuples per group to consider in the aggregation function
         :type group_size: int or str
-        :param missingvalue: value to be considered as missing value; by default it is NAN (for float and double)
+        :param missingvalue: missing value; by default it is the value from the file if defined, NAN otherwise (for float and double)
         :type missingvalue: float
         :param description: additional description to be associated with the output cube
         :type description: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3366,14 +3554,16 @@
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -3393,22 +3583,23 @@
         exec_mode="sync",
         schedule=0,
         dim="-",
         concept_level="A",
         midnight="24",
         operation=None,
         grid="-",
-        missingvalue="NAN",
+        missingvalue="-",
         container="-",
         description="-",
         check_grid="no",
+        save="yes",
         display=False,
     ):
-        """aggregate2(ncores=1, nthreads=1, exec_mode='sync', schedule=0, dim='-', concept_level='A', midnight='24', operation=None, grid='-', missingvalue='NAN', container='-', description='-',
-                      check_grid='no', display=False)
+        """aggregate2(ncores=1, nthreads=1, exec_mode='sync', schedule=0, dim='-', concept_level='A', midnight='24', operation=None, grid='-', missingvalue='-', container='-', description='-',
+                      check_grid='no', save='yes', display=False)
              -> Cube or None : wrapper of the operator OPH_AGGREGATE2
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
@@ -3423,20 +3614,22 @@
         :type concept_level: str
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param grid: optional argument used to identify the grid of dimensions to be used or the one to be created
         :type grid: str
         :param midnight: 00|24
         :type midnight: str
-        :param missingvalue: value to be considered as missing value; by default it is NAN (for float and double)
+        :param missingvalue: missing value; by default it is the value from the file if defined, NAN otherwise (for float and double)
         :type missingvalue: float
         :param description: additional description to be associated with the output cube
         :type description: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3468,14 +3661,16 @@
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -3500,18 +3695,19 @@
         dim_type="manual",
         check_type="yes",
         on_reduce="skip",
         compressed="auto",
         schedule=0,
         container="-",
         description="-",
+        save="yes",
         display=False,
     ):
         """apply(ncores=1, nthreads=1, exec_mode='sync', query='measure', dim_query='null', measure='null', measure_type='manual', dim_type='manual', check_type='yes', on_reduce='skip', compressed='auto',
-                 schedule=0, container='-', description='-', display=False) -> Cube or None : wrapper of the operator OPH_APPLY
+                 schedule=0, container='-', description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_APPLY
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
@@ -3533,14 +3729,16 @@
         :type dim_type: str
         :param measure: name of the new measure resulting from the specified operation
         :type measure: str
         :param measure_type: auto|manual
         :type measure_type: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3574,14 +3772,16 @@
             internal_query += "schedule=" + str(schedule) + ";"
         if container is not None:
             internal_query += "container=" + str(container) + ";"
         if description is not None:
             internal_query += "description=" + str(description) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         internal_query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(internal_query, display) is None:
                 raise RuntimeError()
 
@@ -3607,18 +3807,19 @@
         subset_dims="none",
         subset_filter="all",
         subset_type="index",
         time_filter="yes",
         ncores=1,
         exec_mode="sync",
         schedule=0,
+        save="yes",
         display=False,
     ):
         """concatnc(src_path=None, cdd=None, grid='-', check_exp_dim='yes', dim_offset='-', dim_continue='no', offset=0, description='-', subset_dims='none',
-        subset_filter='all', subset_type='index', time_filter='yes', ncores=1, exec_mode='sync', schedule=0, display=False)
+        subset_filter='all', subset_type='index', time_filter='yes', ncores=1, exec_mode='sync', schedule=0, save='yes', display=False)
         -> Cube or None : wrapper of the operator OPH_CONCATNC
 
         :param src_path: path of file to be imported
         :type src_path: str
         :param cdd: absolute path corresponding to the current directory on data repository
         :type cdd: str
         :param grid: optionally group dimensions in a grid
@@ -3643,14 +3844,16 @@
         :type check_exp_dim: str
         :param dim_offset: offset to be added to dimension values of imported data
         :type dim_offset: float
         :param dim_continue: yes|no
         :type dim_continue: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3686,14 +3889,16 @@
             query += "description=" + str(description) + ";"
         if check_exp_dim is not None:
             query += "check_exp_dim=" + str(check_exp_dim) + ";"
         if dim_offset is not None:
             query += "dim_offset=" + str(dim_offset) + ";"
         if dim_continue is not None:
             query += "dim_continue=" + str(dim_continue) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -3720,18 +3925,19 @@
         subset_filter="all",
         subset_type="index",
         time_filter="yes",
         ncores=1,
         nthreads=1,
         exec_mode="sync",
         schedule=0,
+        save="yes",
         display=False,
     ):
         """concatnc(src_path=None, cdd=None, grid='-', check_exp_dim='yes', dim_offset='-', dim_continue='no', offset=0, description='-', subset_dims='none',
-        subset_filter='all', subset_type='index', time_filter='yes', ncores=1, nthreads=1, exec_mode='sync', schedule=0, display=False)
+        subset_filter='all', subset_type='index', time_filter='yes', ncores=1, nthreads=1, exec_mode='sync', schedule=0, save='yes', display=False)
         -> Cube or None : wrapper of the operator OPH_CONCATNC2
 
         :param src_path: path of file to be imported
         :type src_path: str
         :param cdd: absolute path corresponding to the current directory on data repository
         :type cdd: str
         :param grid: optionally group dimensions in a grid
@@ -3758,14 +3964,16 @@
         :type check_exp_dim: str
         :param dim_offset: offset to be added to dimension values of imported data
         :type dim_offset: float
         :param dim_continue: yes|no
         :type dim_continue: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3803,14 +4011,16 @@
             query += "description=" + str(description) + ";"
         if check_exp_dim is not None:
             query += "check_exp_dim=" + str(check_exp_dim) + ";"
         if dim_offset is not None:
             query += "dim_offset=" + str(dim_offset) + ";"
         if dim_continue is not None:
             query += "dim_continue=" + str(dim_continue) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -3819,21 +4029,23 @@
                     newcube = Cube(pid=Cube.client.cube)
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
-    def provenance(self, branch="all", exec_mode="sync", objkey_filter="all", display=True):
-        """provenance(branch='all', exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_CUBEIO
+    def provenance(self, branch="all", exec_mode="sync", objkey_filter="all", save="yes", display=True):
+        """provenance(branch='all', exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_CUBEIO
 
         :param branch: parent|children|all
         :type branch: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -3845,14 +4057,16 @@
 
         if branch is not None:
             query += "branch=" + str(branch) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if objkey_filter is not None:
             query += "objkey_filter=" + str(objkey_filter) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -3860,25 +4074,27 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def delete(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, display=False):
-        """delete(ncores=1, nthreads=1, exec_mode='sync', schedule=0, display=False) -> None : wrapper of the operator OPH_DELETE
+    def delete(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, save="yes", display=False):
+        """delete(ncores=1, nthreads=1, exec_mode='sync', schedule=0, save='yes', display=False) -> None : wrapper of the operator OPH_DELETE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
@@ -3891,39 +4107,43 @@
             query += "ncores=" + str(ncores) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if schedule is not None:
             query += "schedule=" + str(schedule) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
-    def drilldown(self, ncores=1, exec_mode="sync", schedule=0, ndim=1, container="-", description="-", display=False):
-        """drilldown(ndim=1, container='-', ncores=1, exec_mode='sync', schedule=0, description='-', display=False) -> Cube or None : wrapper of the operator OPH_DRILLDOWN
+    def drilldown(self, ncores=1, exec_mode="sync", schedule=0, ndim=1, container="-", description="-", save="yes", display=False):
+        """drilldown(ndim=1, container='-', ncores=1, exec_mode='sync', schedule=0, description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_DRILLDOWN
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param ndim: number of implicit dimensions that will be transformed in explicit dimensions
         :type ndim: int
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3941,14 +4161,16 @@
             query += "schedule=" + str(schedule) + ";"
         if ndim is not None:
             query += "ndim=" + str(ndim) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -3957,29 +4179,31 @@
                     newcube = Cube(pid=Cube.client.cube)
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
-    def duplicate(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, container="-", description="-", display=False):
-        """duplicate(container='-', ncores=1, nthreads=1, exec_mode='sync', description='-', display=False) -> Cube or None : wrapper of the operator OPH_DUPLICATE
+    def duplicate(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, container="-", description="-", save="yes", display=False):
+        """duplicate(container='-', ncores=1, nthreads=1, exec_mode='sync', description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_DUPLICATE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -3997,14 +4221,16 @@
             query += "schedule=" + str(schedule) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4032,18 +4258,19 @@
         output_path="default",
         output_name="default",
         cdd=None,
         base64="no",
         ncores=1,
         exec_mode="sync",
         objkey_filter="all",
+        save="yes",
         display=True,
     ):
         """explore(schedule=0, limit_filter=100, subset_dims=None, subset_filter='all', time_filter='yes', subset_type='index', show_index='no', show_id='no', show_time='no', level=1, output_path='default',
-                   output_name='default', cdd=None, base64='no', ncores=1, exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_EXPLORECUBE
+                   output_name='default', cdd=None, base64='no', ncores=1, exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_EXPLORECUBE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
@@ -4069,14 +4296,16 @@
         :type cdd: str
         :param base64: yes|no
         :type base64: str
         :param subset_dims: pipe (|) separated list of dimensions on which to apply the subsetting
         :type subset_dims: str
         :param subset_filter: pipe (|) separated list of filters, one per dimension, composed of comma-separated microfilters (e.g. 1,5,10:2:50)
         :type subset_filter: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -4116,14 +4345,16 @@
             query += "base64=" + str(base64) + ";"
         if ncores is not None:
             query += "ncores=" + str(ncores) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if objkey_filter is not None:
             query += "objkey_filter=" + str(objkey_filter) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4131,16 +4362,16 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def publish(self, content="all", schedule=0, show_index="no", show_id="no", show_time="no", ncores=1, exec_mode="sync", display=True):
-        """publish( ncores=1, content='all', exec_mode='sync', show_id= 'no', show_index='no', schedule=0, show_time='no', display=True) -> dict or None : wrapper of the operator OPH_PUBLISH
+    def publish(self, content="all", schedule=0, show_index="no", show_id="no", show_time="no", ncores=1, exec_mode="sync", save="yes", display=True):
+        """publish( ncores=1, content='all', exec_mode='sync', show_id= 'no', show_index='no', schedule=0, show_time='no', save='yes', display=True) -> dict or None : wrapper of the operator OPH_PUBLISH
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
@@ -4148,14 +4379,16 @@
         :type show_index: str
         :param show_id: yes|no
         :type show_id: str
         :param show_time: yes|no
         :type show_time: str
         :param content: all|data|metadata
         :type content: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -4175,14 +4408,16 @@
             query += "show_id=" + str(show_id) + ";"
         if show_time is not None:
             query += "show_time=" + str(show_time) + ";"
         if ncores is not None:
             query += "ncores=" + str(ncores) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4190,47 +4425,64 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def unpublish(self, exec_mode="sync", display=False):
-        """unpublish( exec_mode='sync', display=False) -> None : wrapper of the operator OPH_UNPUBLISH
+    def unpublish(self, exec_mode="sync", save="yes", display=False):
+        """unpublish( exec_mode='sync', save='yes', display=False) -> None : wrapper of the operator OPH_UNPUBLISH
 
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: None
         :rtype: None
         :raises: RuntimeError
         """
 
         if Cube.client is None or self.pid is None:
             raise RuntimeError("Cube.client or pid is None")
 
         query = "oph_unpublish ncores=1;"
 
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     def cubeschema(
-        self, level=0, dim="all", show_index="no", show_time="no", base64="no", action="read", concept_level="c", dim_level=1, dim_array="yes", exec_mode="sync", objkey_filter="all", display=True
+        self,
+        level=0,
+        dim="all",
+        show_index="no",
+        show_time="no",
+        base64="no",
+        action="read",
+        concept_level="c",
+        dim_level=1,
+        dim_array="yes",
+        exec_mode="sync",
+        objkey_filter="all",
+        save="yes",
+        display=True,
     ):
-        """cubeschema( objkey_filter='all', exec_mode='sync', level=0, dim=None, show_index='no', show_time='no', base64='no', action='read', concept_level='c', dim_level=1, dim_array='yes', display=True) -> dict or None : wrapper of the operator OPH_CUBESCHEMA
+        """cubeschema( objkey_filter='all', exec_mode='sync', level=0, dim=None, show_index='no', show_time='no', base64='no', action='read', concept_level='c', dim_level=1, dim_array='yes', save='yes', display=True) -> dict or None : wrapper of the operator OPH_CUBESCHEMA
 
         :param level: 0|1|2
         :type level: int
         :param dim: names of dimensions to show. Only valid with level bigger than 0
         :type dim: str
         :param show_index: yes|no
         :type show_index: str
@@ -4244,14 +4496,16 @@
         :type concept_level: str
         :param dim_level: level of a new dimension to be added, greater than 0 (default is 1)
         :type dim_level: int
         :param dim_array: yes|no
         :type dim_array: str
         :param exec_mode: async or sync
         :type exec_mode: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -4279,14 +4533,16 @@
             query += "dim_level=" + str(dim_level) + ";"
         if dim_array is not None:
             query += "dim_array=" + str(dim_array) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if objkey_filter is not None:
             query += "objkey_filter=" + str(objkey_filter) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4294,27 +4550,29 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def cubesize(self, schedule=0, exec_mode="sync", byte_unit="MB", algorithm="euristic", ncores=1, objkey_filter="all", display=True):
-        """cubesize( schedule=0, ncores=1, byte_unit='MB', algorithm='euristic', objkey_filter='all', exec_mode='sync', display=True) -> dict or None : wrapper of the operator OPH_CUBESIZE
+    def cubesize(self, schedule=0, exec_mode="sync", byte_unit="MB", algorithm="euristic", ncores=1, objkey_filter="all", save="yes", display=True):
+        """cubesize( schedule=0, ncores=1, byte_unit='MB', algorithm='euristic', objkey_filter='all', exec_mode='sync', save='yes', display=True) -> dict or None : wrapper of the operator OPH_CUBESIZE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param byte_unit: KB|MB|GB|TB|PB
         :type byte_unit: str
         :param algorithm: euristic|count
         :type algorithm: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -4332,14 +4590,16 @@
             query += "byte_unit=" + str(byte_unit) + ";"
         if algorithm is not None:
             algorithm += "algorithm=" + str(algorithm) + ";"
         if ncores is not None:
             query += "ncores=" + str(ncores) + ";"
         if objkey_filter is not None:
             query += "objkey_filter=" + str(objkey_filter) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4347,25 +4607,27 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def cubeelements(self, schedule=0, exec_mode="sync", algorithm="dim_product", ncores=1, objkey_filter="all", display=True):
-        """cubeelements( schedule=0, algorithm='dim_product', ncores=1, exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_CUBEELEMENTS
+    def cubeelements(self, schedule=0, exec_mode="sync", algorithm="dim_product", ncores=1, objkey_filter="all", save="yes", display=True):
+        """cubeelements( schedule=0, algorithm='dim_product', ncores=1, exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_CUBEELEMENTS
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param algorithm: dim_product|count
         :type algorithm: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
@@ -4381,14 +4643,16 @@
             query += "exec_mode=" + str(exec_mode) + ";"
         if algorithm is not None:
             query += "algorithm=" + str(algorithm) + ";"
         if ncores is not None:
             query += "ncores=" + str(ncores) + ";"
         if objkey_filter is not None:
             query += "objkey_filter=" + str(objkey_filter) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4396,37 +4660,39 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def intercube(self, ncores=1, exec_mode="sync", cube2=None, cubes=None, operation="sub", missingvalue="NAN", measure="null", schedule=0, container="-", description="-", display=False):
-        """intercube(cube2=None, cubes=None, operation='sub', container='-', exec_mode='sync', ncores=1, description='-', display=False) -> Cube or None : wrapper of the operator OPH_INTERCUBE
+    def intercube(self, ncores=1, exec_mode="sync", cube2=None, cubes=None, operation="sub", missingvalue="-", measure="null", schedule=0, container="-", description="-", save="yes", display=False):
+        """intercube(ncores=1, exec_mode='sync', cube2=None, cubes=None, operation='sub', missingvalue='-', measure='null', schedule=0, container='-', description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_INTERCUBE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param cube2: PID of the second cube
         :type cube2: str
         :param cubes: pipe (|) separated list of cubes
         :type cubes: str
         :param operation: sum|sub|mul|div|abs|arg|corr|mask|max|min|arg_max|arg_min
         :type operation: str
-        :param missingvalue: value to be considered as missing value; by default it is NAN (for float and double)
+        :param missingvalue: missing value; by default it is the value from the file if defined, NAN otherwise (for float and double)
         :type missingvalue: float
         :param measure: new measure name
         :type measure: str
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4455,43 +4721,47 @@
             query += "measure=" + str(measure) + ";"
         if schedule is not None:
             query += "schedule=" + str(schedule) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
             if Cube.client.last_response is not None:
                 if Cube.client.cube:
                     newcube = Cube(pid=Cube.client.cube)
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
-    def merge(self, ncores=1, exec_mode="sync", schedule=0, nmerge=0, container="-", description="-", display=False):
-        """merge(nmerge=0, schedule=0, description='-', container='-', exec_mode='sync', ncores=1, display=False) -> Cube or None : wrapper of the operator OPH_MERGE
+    def merge(self, ncores=1, exec_mode="sync", schedule=0, nmerge=0, container="-", description="-", save="yes", display=False):
+        """merge(nmerge=0, schedule=0, description='-', container='-', exec_mode='sync', ncores=1, save='yes', display=False) -> Cube or None : wrapper of the operator OPH_MERGE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param nmerge: number of input fragments to merge in an output fragment, 0 for all
         :type nmerge: int
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4509,14 +4779,16 @@
             query += "schedule=" + str(schedule) + ";"
         if nmerge is not None:
             query += "nmerge=" + str(nmerge) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4539,18 +4811,19 @@
         metadata_value="-",
         variable_filter="all",
         metadata_type_filter="all",
         metadata_value_filter="all",
         force="no",
         exec_mode="sync",
         objkey_filter="all",
+        save="yes",
         display=True,
     ):
         """metadata(mode='read', metadata_id=0, metadata_key='all', variable='global', metadata_type='text', metadata_value=None, variable_filter=None, metadata_type_filter=None,
-                    metadata_value_filter=None, force='no', exec_mode='sync', objkey_filter='all', display=True) -> dict or None : wrapper of the operator OPH_METADATA
+                    metadata_value_filter=None, force='no', exec_mode='sync', objkey_filter='all', save='yes', display=True) -> dict or None : wrapper of the operator OPH_METADATA
 
         :param mode: insert|read|update|delete
         :type mode: str
         :param metadata_id: id of the particular metadata instance to interact with
         :type metadata_id: int
         :param metadata_key: name of the key (or the enumeration of keys) identifying requested metadata
         :type metadata_key: str
@@ -4566,15 +4839,17 @@
         :type metadata_type_filter: str
         :param metadata_value_filter: filter on metadata value
         :type metadata_value_filter: str
         :param force: force update or deletion of functional metadata associated to a vocabulary, default is no
         :type force: str
         :param exec_mode: async or sync
         :type exec_mode: str
-        :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is Ture)
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
+        :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is True)
         :type display: bool
         :returns: response or None
         :rtype: dict or None
         :raises: RuntimeError
         """
 
         if Cube.client is None or self.pid is None:
@@ -4603,14 +4878,16 @@
             query += "metadata_value_filter=" + str(metadata_value_filter) + ";"
         if force is not None:
             query += "force=" + str(force) + ";"
         if exec_mode is not None:
             query += "exec_mode=" + str(exec_mode) + ";"
         if objkey_filter is not None:
             query += "objkey_filter=" + str(objkey_filter) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4618,16 +4895,16 @@
                 response = Cube.client.deserialize_response()["response"]
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return response
 
-    def permute(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, dim_pos=None, container="-", description="-", display=False):
-        """permute(dim_pos=None, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', display=False) -> Cube or None : wrapper of the operator OPH_PERMUTE
+    def permute(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, dim_pos=None, container="-", description="-", save="yes", display=False):
+        """permute(dim_pos=None, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_PERMUTE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
@@ -4635,14 +4912,16 @@
         :type schedule: int
         :param dim_pos: permutation of implicit dimensions as a comma-separated list of dimension levels
         :type dim_pos: str
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4662,14 +4941,16 @@
             query += "dim_pos=" + str(dim_pos) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4687,48 +4968,51 @@
         ncores=1,
         nthreads=1,
         exec_mode="sync",
         schedule=0,
         group_size="all",
         operation=None,
         order=2,
-        missingvalue="NAN",
+        missingvalue="-",
         grid="-",
         container="-",
         description="-",
         check_grid="no",
+        save="yes",
         display=False,
     ):
-        """reduce(operation=None, container=None, exec_mode='sync', grid='-', group_size='all', ncores=1, nthreads=1, schedule=0, order=2, description='-', objkey_filter='all', check_grid='no', display=False)
+        """reduce(operation=None, container=None, exec_mode='sync', missingvalue='-', grid='-', group_size='all', ncores=1, nthreads=1, schedule=0, order=2, description='-', objkey_filter='all', check_grid='no', save='yes', display=False)
              -> Cube or None : wrapper of the operator OPH_REDUCE
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
         :type schedule: int
         :param operation: count|max|min|avg|sum|std|var|cmoment|acmoment|rmoment|armoment|quantile|arg_max|arg_min
         :type operation: str
         :param order: order used in evaluation the moments or value of the quantile in range [0, 1]
         :type order: float
-        :param missingvalue: value to be considered as missing value; by default it is NAN (for float and double)
+        :param missingvalue: missing value; by default it is the value from the file if defined, NAN otherwise (for float and double)
         :type missingvalue: float
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param grid: optional argument used to identify the grid of dimensions to be used or the one to be created
         :type grid: str
         :param group_size: size of the aggregation set, all for the entire array
         :type group_size: int or str
         :param description: additional description to be associated with the output cube
         :type description: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4758,14 +5042,16 @@
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4784,23 +5070,24 @@
         exec_mode="sync",
         schedule=0,
         dim=None,
         concept_level="A",
         midnight="24",
         operation=None,
         order=2,
-        missingvalue="NAN",
+        missingvalue="-",
         grid="-",
         container="-",
         description="-",
         nthreads=1,
         check_grid="no",
+        save="yes",
         display=False,
     ):
-        """reduce2(dim=None, operation=None, concept_level='A', container='-', exec_mode='sync', grid='-', midnight='24', order=2, description='-', schedule=0, ncores=1, nthreads=1, check_grid='no', display=False)
+        """reduce2(dim=None, operation=None, concept_level='A', container='-', exec_mode='sync', grid='-', midnight='24', order=2, missingvalue="-", description='-', schedule=0, ncores=1, nthreads=1, check_grid='no', save='yes', display=False)
              -> Cube or None : wrapper of the operator OPH_REDUCE2
 
         :param ncores: number of cores to use
         :type ncores: int
         :param exec_mode: async or sync
         :type exec_mode: str
         :param schedule: 0
@@ -4815,22 +5102,24 @@
         :type container: str
         :param grid: optional argument used to identify the grid of dimensions to be used or the one to be created
         :type grid: str
         :param midnight: 00|24
         :type midnight: str
         :param order: order used in evaluation the moments or value of the quantile in range [0, 1]
         :type order: float
-        :param missingvalue: value to be considered as missing value; by default it is NAN (for float and double)
+        :param missingvalue: missing value; by default it is the value from the file if defined, NAN otherwise (for float and double)
         :type missingvalue: float
         :param description: additional description to be associated with the output cube
         :type description: str
         :param nthreads: number of threads to use
         :type nthreads: int
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4864,14 +5153,16 @@
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4880,16 +5171,16 @@
                     newcube = Cube(pid=Cube.client.cube)
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
-    def rollup(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, ndim=1, container="-", description="-", display=False):
-        """rollup(ndim=1, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', display=False) -> Cube or None : wrapper of the operator OPH_ROLLUP
+    def rollup(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, ndim=1, container="-", description="-", save="yes", display=False):
+        """rollup(ndim=1, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_ROLLUP
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
@@ -4897,14 +5188,16 @@
         :type schedule: int
         :param ndim: number of explicit dimensions that will be transformed in implicit dimensions
         :type ndim: int
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4924,14 +5217,16 @@
             query += "ndim=" + str(ndim) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -4940,16 +5235,16 @@
                     newcube = Cube(pid=Cube.client.cube)
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
         else:
             return newcube
 
-    def split(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, nsplit=2, container="-", description="-", display=False):
-        """split(nsplit=2, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', display=False) -> Cube or None : wrapper of the operator OPH_SPLIT
+    def split(self, ncores=1, nthreads=1, exec_mode="sync", schedule=0, nsplit=2, container="-", description="-", save="yes", display=False):
+        """split(nsplit=2, container='-', exec_mode='sync', ncores=1, nthreads=1, schedule=0, description='-', save='yes', display=False) -> Cube or None : wrapper of the operator OPH_SPLIT
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
         :type exec_mode: str
@@ -4957,14 +5252,16 @@
         :type schedule: int
         :param nsplit: number of output fragments per input fragment
         :type nsplit: int
         :param container: name of the container to be used to store the output cube, by default it is the input container
         :type container: str
         :param description: additional description to be associated with the output cube
         :type description: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -4984,14 +5281,16 @@
             query += "nsplit=" + str(nsplit) + ";"
         if container is not None:
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -5015,18 +5314,19 @@
         subset_type="index",
         time_filter="yes",
         offset=0,
         grid="-",
         container="-",
         description="-",
         check_grid="no",
+        save="yes",
         display=False,
     ):
         """subset(subset_dims='none', subset_filter='all', container='-', exec_mode='sync', subset_type='index', time_filter='yes', offset=0, grid='-', ncores=1, nthreads=1, schedule=0, description='-',
-                  check_grid='no', display=False)
+                  check_grid='no', save='yes', display=False)
              -> Cube or None : wrapper of the operator OPH_SUBSET
 
         :param ncores: number of cores to use
         :type ncores: int
         :param nthreads: number of threads to use
         :type nthreads: int
         :param exec_mode: async or sync
@@ -5047,14 +5347,16 @@
         :type offset: int
         :param grid: optional argument used to identify the grid of dimensions to be used or the one to be created
         :type grid: str
         :param description: additional description to be associated with the output cube
         :type description: str
         :param check_grid: yes|no
         :type check_grid: str
+        :param save: option to enable/disable JSON response saving on the server-side (default is yes)
+        :type save: str
         :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
         :type display: bool
         :returns: new cube or None
         :rtype: Cube or None
         :raises: RuntimeError
         """
 
@@ -5086,94 +5388,16 @@
             query += "container=" + str(container) + ";"
         if description is not None:
             query += "description=" + str(description) + ";"
         if check_grid is not None:
             query += "check_grid=" + str(check_grid) + ";"
         if nthreads is not None:
             query += "nthreads=" + str(nthreads) + ";"
-
-        query += "cube=" + str(self.pid) + ";"
-
-        try:
-            if Cube.client.submit(query, display) is None:
-                raise RuntimeError()
-
-            if Cube.client.last_response is not None:
-                if Cube.client.cube:
-                    newcube = Cube(pid=Cube.client.cube)
-        except Exception as e:
-            print(get_linenumber(), "Something went wrong:", e)
-            raise RuntimeError()
-        else:
-            return newcube
-
-    def subset2(
-        self, ncores=1, exec_mode="sync", schedule=0, subset_dims="none", subset_filter="all", time_filter="yes", offset=0, grid="-", container="-", description="-", check_grid="no", display=False
-    ):
-        """subset2(subset_dims='none', subset_filter='all', grid='-', container='-', ncores=1, exec_mode='sync', schedule=0, time_filter='yes', offset=0, description='-',
-                   check_grid='no', display=False)
-             -> Cube or None : wrapper of the operator OPH_SUBSET2 (Deprecated since Ophidia v1.1)
-
-        :param ncores: number of cores to use
-        :type ncores: int
-        :param exec_mode: async or sync
-        :type exec_mode: str
-        :param schedule: 0
-        :type schedule: int
-        :param subset_dims: pipe (|) separated list of dimensions on which to apply the subsetting
-        :type subset_dims: str
-        :param subset_filter: pipe (|) separated list of filters, one per dimension, composed of comma-separated microfilters on dimension values (e.g. 30,5,10:50)
-        :type subset_filter: str
-        :param time_filter: yes|no
-        :type time_filter: str
-        :param offset: added to the bounds of subset intervals
-        :type offset: int
-        :param grid: optional argument used to identify the grid of dimensions to be used or the one to be created
-        :type grid: str
-        :param container: name of the container to be used to store the output cube, by default it is the input container
-        :type container: str
-        :param description: additional description to be associated with the output cube
-        :type description: str
-        :param check_grid: yes|no
-        :type check_grid: str
-        :param display: option for displaying the response in a "pretty way" using the pretty_print function (default is False)
-        :type display: bool
-        :returns: new cube or None
-        :rtype: Cube or None
-        :raises: RuntimeError
-        """
-
-        if Cube.client is None or self.pid is None:
-            raise RuntimeError("Cube.client or pid is None")
-        newcube = None
-
-        query = "oph_subset2 "
-
-        if ncores is not None:
-            query += "ncores=" + str(ncores) + ";"
-        if exec_mode is not None:
-            query += "exec_mode=" + str(exec_mode) + ";"
-        if schedule is not None:
-            query += "schedule=" + str(schedule) + ";"
-        if subset_dims is not None:
-            query += "subset_dims=" + str(subset_dims) + ";"
-        if subset_filter is not None:
-            query += "subset_filter=" + str(subset_filter) + ";"
-        if time_filter is not None:
-            query += "time_filter=" + str(time_filter) + ";"
-        if offset is not None:
-            query += "offset=" + str(offset) + ";"
-        if grid is not None:
-            query += "grid=" + str(grid) + ";"
-        if container is not None:
-            query += "container=" + str(container) + ";"
-        if description is not None:
-            query += "description=" + str(description) + ";"
-        if check_grid is not None:
-            query += "check_grid=" + str(check_grid) + ";"
+        if save is not None:
+            query += "save=" + str(save) + ";"
 
         query += "cube=" + str(self.pid) + ";"
 
         try:
             if Cube.client.submit(query, display) is None:
                 raise RuntimeError()
 
@@ -5231,15 +5455,15 @@
             Cube.fs(command="rm", dpath=file_path, cdd="/", display=False)
 
         except Exception as e:
             print(get_linenumber(), "Something went wrong:", e)
             raise RuntimeError()
 
     def export_array(self, show_id="no", show_time="no", subset_dims=None, subset_filter=None, time_filter="no"):
-        """export_array(show_id='no', show_time='no', subset_dims=None, subset_filter=None, time_filter='no') -> dict or None : wrapper of the operator OPH_EXPLORECUBE
+        """export_array(show_id='no', show_time='no', subset_dims=None, subset_filter=None, time_filter='no') -> dict or None : return data from an Ophidia datacube into a Python structure
 
         :param show_id: yes|no
         :type show_id: str
         :param show_time: yes|no
         :type show_time: str
         :param subset_dims: pipe (|) separated list of dimensions on which to apply the subsetting
         :type subset_dims: str
@@ -5252,15 +5476,15 @@
         :raises: RuntimeError
         """
 
         if Cube.client is None or self.pid is None:
             raise RuntimeError("Cube.client or pid is None")
         response = None
 
-        query = "oph_explorecube ncore=1;base64=yes;level=2;show_index=yes;subset_type=coord;limit_filter=0;"
+        query = "oph_explorecube ncore=1;base64=yes;level=2;show_index=yes;subset_type=coord;limit_filter=0;save=no;"
 
         if time_filter is not None:
             query += "time_filter=" + str(time_filter) + ";"
         if show_id is not None:
             query += "show_id=" + str(show_id) + ";"
         if show_time is not None:
             query += "show_time=" + str(show_time) + ";"
```

### Comparing `PyOphidia-1.9.0/PyOphidia/ophsubmit.py` & `PyOphidia-1.9.1/PyOphidia/ophsubmit.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import sys
 import base64
 import re
-from xml.dom import minidom
+import xml.etree.ElementTree as ET
 from inspect import currentframe
 
 if sys.version_info < (3, 0):
     import httplib
 else:
     import http.client as httplib
 
@@ -189,23 +189,23 @@
             statuscode, statusmessage = _res.status, _res.reason
             reply = _res.read()
 
         if statuscode != 200:
             print(get_linenumber(), "Something went wrong in submitting the request:", statuscode, statusmessage)
             return (None, None, None, 1, statusmessage)
 
-        xmldoc = minidom.parseString(reply)
-        response = xmldoc.getElementsByTagName("oph:ophResponse")[0]
+        xmltree = ET.fromstring(reply)
+        response = xmltree.findall(".//oph:ophResponse", namespaces={"oph": "urn:oph"})[0]
         res_error, res_response, res_jobid = None, None, None
-        if len(response.getElementsByTagName("jobid")) > 0 and response.getElementsByTagName("jobid")[0].firstChild is not None:
-            res_jobid = response.getElementsByTagName("jobid")[0].firstChild.data
-        if len(response.getElementsByTagName("error")) > 0 and response.getElementsByTagName("error")[0].firstChild is not None:
-            res_error = int(response.getElementsByTagName("error")[0].firstChild.data)
-        if len(response.getElementsByTagName("response")) > 0 and response.getElementsByTagName("response")[0].firstChild is not None:
-            res_response = response.getElementsByTagName("response")[0].firstChild.data
+        if len(response.findall("jobid")) > 0 and response.findall("jobid")[0].text is not None:
+            res_jobid = response.findall("jobid")[0].text
+        if len(response.findall("error")) > 0 and response.findall("error")[0].text is not None:
+            res_error = int(response.findall("error")[0].text)
+        if len(response.findall("response")) > 0 and response.findall("response")[0].text is not None:
+            res_response = response.findall("response")[0].text
     except Exception as e:
         print(get_linenumber(), "Something went wrong in submitting the request:", e)
         return (None, None, None, 1, e)
     if res_error is None:
         return (None, None, None, 1, "Invalid response")
     if res_error == OPH_SERVER_OK:
         response, jobid, newsession, return_value, error = None, None, None, 0, None
```

### Comparing `PyOphidia-1.9.0/PyOphidia.egg-info/PKG-INFO` & `PyOphidia-1.9.1/PyOphidia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: PyOphidia
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python bindings for the Ophidia Data Analytics Platform
 Home-page: http://ophidia.cmcc.it
 Author: Ophidia Developers
 Author-email: ophidia-info@cmcc.it
 License: GPLv3+
 Description: PyOphidia: Python bindings for Ophidia
         ======================================
         
         *PyOphidia* is a GPLv3_-licensed Python package for interacting with the Ophidia_ framework.
         
         It is an alternative to Oph_Term, the Ophidia no-GUI interpreter component, and a convenient way to submit SOAP HTTPS requests to an Ophidia server or to develop your own application using Python. 
         
-        It runs on Python 2.7, 3.4, 3.5, 3.6, 3.7 and 3.8 has no Python dependencies and is pure-Python code. It requires a running Ophidia instance for client-server interactions. The latest PyOphidia version (v1.9) is compatible with Ophidia v1.6.
+        It runs on Python 2.7, 3.5, 3.6, 3.7, 3.8 and 3.9 has no Python dependencies and is pure-Python code. It requires a running Ophidia instance for client-server interactions. The latest PyOphidia version (v1.9) is compatible with Ophidia v1.6.
         
         It provides 2 main modules:
         
         - client.py: generic *low level* class to submit any type of requests (simple tasks and workflows), using SSL and SOAP with the client ophsubmit.py;
         - cube.py: *high level* cube-oriented class to interact directly with cubes, with several methods wrapping the operators.
         
         Installation
@@ -253,14 +253,14 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `PyOphidia-1.9.0/CONTRIBUTING.rst` & `PyOphidia-1.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyOphidia-1.9.0/HISTORY.rst` & `PyOphidia-1.9.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,34 @@
 
+v1.9.1 - 2021-08-03
+-------------------
+
+Added:
+~~~~~~
+
+- Argument 'save' for saving the JSON response in most cube methods
+
+Changed:
+~~~~~~~~
+
+- Default values of 'disable' and 'enable' argument in 'service' method in cube class
+- Default value of 'missingvalue' argument in cube class to '-'
+
+Fixed:
+~~~~~~
+
+- Slow parsing of large XML response documents in ophsubmit.py `#34 <https://github.com/OphidiaBigData/PyOphidia/issues/34>`_
+
+
+Removed:
+~~~~~~~~
+
+- Deprecated 'subset2' method from cube `#35 <https://github.com/OphidiaBigData/PyOphidia/pull/35>`_
+
+
 v1.9.0 - 2021-07-21
 -------------------
 
 Added:
 ~~~~~~
 
 - New attribute 'last_response_status' in client class
```

### Comparing `PyOphidia-1.9.0/LICENSE` & `PyOphidia-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOphidia-1.9.0/README.rst` & `PyOphidia-1.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 PyOphidia: Python bindings for Ophidia
 ======================================
 
 *PyOphidia* is a GPLv3_-licensed Python package for interacting with the Ophidia_ framework.
 
 It is an alternative to Oph_Term, the Ophidia no-GUI interpreter component, and a convenient way to submit SOAP HTTPS requests to an Ophidia server or to develop your own application using Python. 
 
-It runs on Python 2.7, 3.4, 3.5, 3.6, 3.7 and 3.8 has no Python dependencies and is pure-Python code. It requires a running Ophidia instance for client-server interactions. The latest PyOphidia version (v1.9) is compatible with Ophidia v1.6.
+It runs on Python 2.7, 3.5, 3.6, 3.7, 3.8 and 3.9 has no Python dependencies and is pure-Python code. It requires a running Ophidia instance for client-server interactions. The latest PyOphidia version (v1.9) is compatible with Ophidia v1.6.
 
 It provides 2 main modules:
 
 - client.py: generic *low level* class to submit any type of requests (simple tasks and workflows), using SSL and SOAP with the client ophsubmit.py;
 - cube.py: *high level* cube-oriented class to interact directly with cubes, with several methods wrapping the operators.
 
 Installation
```

### Comparing `PyOphidia-1.9.0/setup.py` & `PyOphidia-1.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """Build a file path from *paths* and return the contents."""
     with open(os.path.join(*paths), 'r') as f:
         return f.read()
 
 
 setup(
     name='PyOphidia',
-    version='1.9.0',
+    version='1.9.1',
     description='Python bindings for the Ophidia Data Analytics Platform',
     long_description=(read('README.rst') + '\n\n'),
     url='http://ophidia.cmcc.it',
     license='GPLv3+',
     author='Ophidia Developers',
     author_email='ophidia-info@cmcc.it',
     packages=['PyOphidia'],
@@ -44,17 +44,17 @@
         'Natural Language :: English',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Scientific/Engineering',
         #'Private :: Do Not Upload',
     ],
 )
```

### Comparing `PyOphidia-1.9.0/PKG-INFO` & `PyOphidia-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: PyOphidia
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python bindings for the Ophidia Data Analytics Platform
 Home-page: http://ophidia.cmcc.it
 Author: Ophidia Developers
 Author-email: ophidia-info@cmcc.it
 License: GPLv3+
 Description: PyOphidia: Python bindings for Ophidia
         ======================================
         
         *PyOphidia* is a GPLv3_-licensed Python package for interacting with the Ophidia_ framework.
         
         It is an alternative to Oph_Term, the Ophidia no-GUI interpreter component, and a convenient way to submit SOAP HTTPS requests to an Ophidia server or to develop your own application using Python. 
         
-        It runs on Python 2.7, 3.4, 3.5, 3.6, 3.7 and 3.8 has no Python dependencies and is pure-Python code. It requires a running Ophidia instance for client-server interactions. The latest PyOphidia version (v1.9) is compatible with Ophidia v1.6.
+        It runs on Python 2.7, 3.5, 3.6, 3.7, 3.8 and 3.9 has no Python dependencies and is pure-Python code. It requires a running Ophidia instance for client-server interactions. The latest PyOphidia version (v1.9) is compatible with Ophidia v1.6.
         
         It provides 2 main modules:
         
         - client.py: generic *low level* class to submit any type of requests (simple tasks and workflows), using SSL and SOAP with the client ophsubmit.py;
         - cube.py: *high level* cube-oriented class to interact directly with cubes, with several methods wrapping the operators.
         
         Installation
@@ -253,14 +253,14 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
```

