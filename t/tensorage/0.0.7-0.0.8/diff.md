# Comparing `tmp/tensorage-0.0.7.tar.gz` & `tmp/tensorage-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.7.tar", last modified: Mon Jul 31 09:54:07 2023, max compression
+gzip compressed data, was "tensorage-0.0.8.tar", last modified: Wed Aug  2 09:24:10 2023, max compression
```

## Comparing `tensorage-0.0.7.tar` & `tensorage-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:54:07.562017 tensorage-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-31 09:53:57.000000 tensorage-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 09:53:57.000000 tensorage-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 09:54:07.562017 tensorage-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 09:53:57.000000 tensorage-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-31 09:53:57.000000 tensorage-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 09:54:07.562017 tensorage-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-31 09:53:57.000000 tensorage-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:54:07.558017 tensorage-0.0.7/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/db_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:54:07.562017 tensorage-0.0.7/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 09:24:10.029866 tensorage-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-02 09:23:55.000000 tensorage-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-02 09:23:55.000000 tensorage-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-02 09:24:10.029866 tensorage-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-02 09:23:55.000000 tensorage-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-02 09:23:55.000000 tensorage-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 09:24:10.029866 tensorage-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-08-02 09:23:55.000000 tensorage-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 09:24:10.029866 tensorage-0.0.8/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9570 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-08-02 09:23:55.000000 tensorage-0.0.8/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 09:24:10.029866 tensorage-0.0.8/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-02 09:24:10.000000 tensorage-0.0.8/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.7/LICENSE` & `tensorage-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.7/setup.py` & `tensorage-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.7/tensorage/auth.py` & `tensorage-0.0.8/tensorage/auth.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.7/tensorage/db_init.py` & `tensorage-0.0.8/tensorage/db_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 SQL = """
 -- datasets table
 create table
 public.datasets (
     id bigint generated by default as identity not null,
     key character varying not null,
     ndim smallint not null,
-    shape array not null,
+    shape int[] not null,
     created_at timestamp with time zone null default now(),
     user_id uuid null,
+    is_public boolean not null default false,
     constraint datasets_pkey primary key (id),
     constraint datasets_key_user_id_key unique (key, user_id),
     constraint datasets_user_id_fkey foreign key (user_id) references users (id) on delete set null
 ) tablespace pg_default;
 
   -- RLS policy
 ALTER TABLE public.datasets ENABLE ROW LEVEL SECURITY;
 CREATE POLICY "Allow all actions to the record owner" ON "public"."datasets"
 AS PERMISSIVE FOR ALL
-TO public
-USING (auth.uid() = user_id)
-WITH CHECK (auth.uid() = user_id);
+TO authenticated
+USING (is_public OR (auth.uid() = user_id))
+WITH CHECK (is_public OR (auth.uid() = user_id));
 
 
 -- tensor_float4 table
 create table
 public.tensors_float4 (
     data_id bigint not null,
     index bigint not null,
-    tensor array not null,
+    tensor float4[] not null,
     user_id uuid not null,
+    is_public boolean not null default false,
     constraint tensors_float4_pkey primary key (data_id, index, user_id),
     constraint tensors_float4_data_id_fkey foreign key (data_id) references datasets (id) on delete cascade,
     constraint tensors_float4_user_id_fkey foreign key (user_id) references users (id) on delete set null
 ) tablespace pg_default;
 
 -- RLS policy
 ALTER TABLE public.tensors_float4 ENABLE ROW LEVEL SECURITY;
-CREATE POLICY "Allow all actions to the record owner" ON "public"."tensor_float4"
+CREATE POLICY "Allow all actions to the record owner" ON "public"."tensors_float4"
 AS PERMISSIVE FOR ALL
-TO public
-USING (auth.uid() = user_id)
-WITH CHECK (auth.uid() = user_id);
+TO authenticated
+USING (is_public OR (auth.uid() = user_id))
+WITH CHECK (is_public OR (auth.uid() = user_id));
 
 -- create the slicing database function
 CREATE OR REPLACE FUNCTION public.tensor_float4_slice(name character varying, index_low integer, index_up integer, slice_low integer[], slice_up integer[])
 RETURNS table(tensor float4[])
 AS
 $$
 DECLARE
@@ -60,8 +62,40 @@
                    WHERE datasets.key = ' || quote_literal(name) || '
                    AND tensors_float4.index >= ' || index_low || '
                    AND tensors_float4.index < ' || index_up ;
 
   RETURN QUERY EXECUTE query_string;
 END;
 $$ language plpgsql;
+
+-- add usage statistics views
+create view
+  public.user_usage_details as
+select
+  users.id,
+  users.email,
+  datasets.key as dataset,
+  sum(pg_column_size(tensors_float4.tensor)::real) / 1024.0::double precision / 1024.0::double precision / 1024.0::double precision as total_size_gb,
+  pg_size_pretty(sum(pg_column_size(tensors_float4.tensor))) as size
+from
+  tensors_float4
+  join users on tensors_float4.user_id = users.id
+  join datasets on datasets.id = tensors_float4.data_id
+group by
+  users.id,
+  users.email,
+  datasets.key;
+
+create view
+  public.user_usage_aggregate as
+select
+  users.id,
+  users.email,
+  sum(pg_column_size(tensors_float4.tensor)::real) / 1024.0::double precision / 1024.0::double precision / 1024.0::double precision as total_size_gb,
+  pg_size_pretty(sum(pg_column_size(tensors_float4.tensor))) as size
+from
+  tensors_float4
+  join users on tensors_float4.user_id = users.id
+group by
+  users.id,
+  users.email;
 """
```

### Comparing `tensorage-0.0.7/tensorage/session.py` & `tensorage-0.0.8/tensorage/session.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.7/tensorage/store.py` & `tensorage-0.0.8/tensorage/store.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 from typing import TYPE_CHECKING, Tuple, Union, List
 from dataclasses import dataclass, field
+import warnings
 
+from tqdm import tqdm
 import numpy as np
+from postgrest.exceptions import APIError
 
 if TYPE_CHECKING:
     from tensorage.session import BackendSession
 from .types import Dataset
 
 
 @dataclass
 class TensorStore(object):
     _session: 'BackendSession' = field(repr=False)
+    quiet: bool = field(default=False)
+
+    # some stuff for upload
+    chunk_size: int = field(default=100000, repr=False)
+
+    def __post_init__(self):
+        # check if the schema is installed
+        with self._session as context:
+            if not context.check_schema_installed():
+                from tensorage.db_init import SQL
+                warnings.warn(f"The schema for the TensorStore is not installed. Please connect the database and run the following script:\n\n--------8<--------\n{SQL}\n\n--------8<--------\n")
 
     def __getitem__(self, key: Union[str, Tuple[Union[str, slice, int]]]):
         # first get key
         if isinstance(key, str):
             name = key
         elif isinstance(key[0], str):
             name = key[0]
@@ -77,21 +91,41 @@
         
         # get the shape
         shape = value.shape
 
         # get the dim
         dim = value.ndim
 
+        # check if this should be uplaoded chunk-wise
+        if value.size > self.chunk_size:
+            # figure out a good batch size
+            batch_size = self.chunk_size // np.multiply(*value.shape[1:])
+            if batch_size == 0:
+                batch_size = 1
+            
+            # create the index over the batch to determine the offset on upload
+            single_index = np.arange(0, value.shape[0], batch_size, dtype=int)
+            batch_index = list(zip(single_index, single_index[1:].tolist() + [value.shape[0]]))
+            
+            # build the 
+            batches = [(i * batch_size, value[up:low]) for i, (up, low) in enumerate(batch_index)]
+        else:
+            batches = [(0, value)]
+
         # connect
         with self._session as context:
             # insert the dataset
             dataset = context.insert_dataset(key, shape, dim)
 
+            # make the iterator
+            _iterator = tqdm(batches, desc=f'Uploading {key} [{len(batches)} batches of {batch_size}]') if not self.quiet else batches
+
             # insert the tensor
-            context.insert_tensor(dataset.id, [chunk for chunk in value])
+            for offset, batch in _iterator:
+                context.insert_tensor(dataset.id, [tensor for tensor in batch], offset=offset)
 
     def __delitem__(self, key: str):
         raise NotImplementedError
     
     def __contains__(self, key: str):
         # get the keys
         keys = self.keys()
@@ -128,14 +162,33 @@
         # set the JWT of the authenticated user as the new token
         self.backend.client.postgrest.auth(self.backend._session.access_token)
     
     def __restore_auth(self):
         # restore the original JWT
         self.backend.client.postgrest.auth(self._anon_key)
 
+    def check_schema_installed(self) -> bool:
+        # setup auth token
+        self.__setup_auth()
+
+        # check if the datasets and tensor_float4 tables exist
+        missing_table = False
+
+        for table in ('datasets', 'tensors_float4'):
+            try:
+                self.backend.client.table(table).select('*', count='exact').limit(1).execute()
+            except APIError as e:
+                if e.code == '42P01':
+                    missing_table = True
+                else:
+                    raise e
+        
+        # check if any of the needed tables was not found
+        return not missing_table
+
     @property
     def user_id(self) -> str:
         return self.backend._user.id
 
     def insert_dataset(self, key: str, shape: Tuple[int], dim: int) -> Dataset:
         # run the insert
         self.__setup_auth()
@@ -145,20 +198,20 @@
         # return an instance of Dataset
         data = response.data[0]
         return Dataset(id=data['id'], key=data['key'], shape=data['shape'], ndim=data['ndim'])
     
     def insert_tensor(self, data_id: int, data: List[np.ndarray], offset: int = 0) -> bool:
         # setup auth token
         self.__setup_auth()
-        
+
         # run the insert
         try:
-            response = self.backend.client.table('tensors_float4').insert([{'data_id': data_id, 'index': i + 1 + offset, 'user_id': self.user_id, 'tensor': chunk.tolist()} for i, chunk in enumerate(data)]).execute()
-        except Exception as e:
-            print(response.data)
+            self.backend.client.table('tensors_float4').insert([{'data_id': data_id, 'index': int(i + 1 + offset), 'user_id': self.user_id, 'tensor': chunk.tolist()} for i, chunk in enumerate(data)]).execute()
+        except APIError as e:
+            # TODO check if we expired here and refresh the token
             raise e
         
         # restore old token
         self.__restore_auth()
 
         # return 
         return True
```

