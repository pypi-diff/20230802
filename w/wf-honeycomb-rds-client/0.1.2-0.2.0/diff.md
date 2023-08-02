# Comparing `tmp/wf_honeycomb_rds_client-0.1.2.tar.gz` & `tmp/wf_honeycomb_rds_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_honeycomb_rds_client-0.1.2.tar", max compression
+gzip compressed data, was "wf_honeycomb_rds_client-0.2.0.tar", max compression
```

## Comparing `wf_honeycomb_rds_client-0.1.2.tar` & `wf_honeycomb_rds_client-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2023-06-26 20:37:02.570215 wf_honeycomb_rds_client-0.1.2/LICENSE
--rw-r--r--   0        0        0      560 2023-06-26 20:41:41.572706 wf_honeycomb_rds_client-0.1.2/README.md
--rw-r--r--   0        0        0      555 2023-06-26 23:15:19.471852 wf_honeycomb_rds_client-0.1.2/honeycomb_rds_client/__init__.py
--rw-r--r--   0        0        0     6995 2023-06-26 20:59:58.271561 wf_honeycomb_rds_client-0.1.2/honeycomb_rds_client/core.py
--rw-r--r--   0        0        0     1125 2023-07-30 22:29:57.675020 wf_honeycomb_rds_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.1.2/setup.py
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-26 20:37:02.570215 wf_honeycomb_rds_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0      560 2023-06-26 20:41:41.572706 wf_honeycomb_rds_client-0.2.0/README.md
+-rw-r--r--   0        0        0      555 2023-06-26 23:15:19.471852 wf_honeycomb_rds_client-0.2.0/honeycomb_rds_client/__init__.py
+-rw-r--r--   0        0        0     9832 2023-08-02 16:40:36.534263 wf_honeycomb_rds_client-0.2.0/honeycomb_rds_client/core.py
+-rw-r--r--   0        0        0     1125 2023-08-02 16:40:36.534263 wf_honeycomb_rds_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.2.0/setup.py
+-rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.2.0/PKG-INFO
```

### Comparing `wf_honeycomb_rds_client-0.1.2/LICENSE` & `wf_honeycomb_rds_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_honeycomb_rds_client-0.1.2/README.md` & `wf_honeycomb_rds_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wf_honeycomb_rds_client-0.1.2/honeycomb_rds_client/__init__.py` & `wf_honeycomb_rds_client-0.2.0/honeycomb_rds_client/__init__.py`

 * *Files identical despite different names*

### Comparing `wf_honeycomb_rds_client-0.1.2/honeycomb_rds_client/core.py` & `wf_honeycomb_rds_client-0.2.0/honeycomb_rds_client/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import postgres_client
 import honeycomb_io
 import pandas as pd
+import numpy as np
 import datetime
 import os
 
 class HoneycombRDSClient(postgres_client.PostgresClient):
     def __init__(
         self,
         dbname=None,
@@ -28,42 +29,47 @@
         device_ids=None,
         part_numbers=None,
         serial_numbers=None,
         tag_ids=None,
         names=None,
         environment_id=None,
         environment_name=None,
+        include_device_info=False,
+        include_entity_info=False,
+        include_material_info=False,
         connection=None,
         honeycomb_chunk_size=100,
         honeycomb_client=None,
         honeycomb_uri=None,
         honeycomb_token_uri=None,
         honeycomb_audience=None,
         honeycomb_client_id=None,
         honeycomb_client_secret=None
     ):
-        device_ids = honeycomb_io.fetch_device_ids(
+        device_info = honeycomb_io.fetch_devices(
             device_types=['UWBTAG'],
             device_ids=device_ids,
             part_numbers=part_numbers,
             serial_numbers=serial_numbers,
             tag_ids=tag_ids,
             names=names,
             environment_id=environment_id,
             environment_name=environment_name,
             start=start,
             end=end,
+            output_format='dataframe',
             chunk_size=honeycomb_chunk_size,
             client=honeycomb_client,
             uri=honeycomb_uri,
             token_uri=honeycomb_token_uri,
             audience=honeycomb_audience,
             client_id=honeycomb_client_id,
-            client_secret=honeycomb_client_secret
+            client_secret=honeycomb_client_secret,
         )
+        device_ids = device_info.index.unique().tolist()
         start_utc_naive = start.astimezone(datetime.timezone.utc).replace(tzinfo=None)
         end_utc_naive = end.astimezone(datetime.timezone.utc).replace(tzinfo=None)
         query_list = [
             {'fields': ['timestamp'], 'operator': 'gte', 'values': [start_utc_naive]},
             {'fields': ['timestamp'], 'operator': 'lt', 'values': [end_utc_naive]},
             {'fields': ['object'], 'operator': 'in', 'values': device_ids},
         ]
@@ -72,82 +78,118 @@
             schema='honeycomb',
             fields=None,
             query_list=query_list,
             connection=connection,
             convert_to_dataframe=True
         )
         position_data['timestamp'] = pd.to_datetime(position_data['timestamp']).dt.tz_localize('UTC')
-        position_data['x'] = pd.to_numeric(position_data['data.coordinates'].apply(lambda x: x[0]))
-        position_data['y'] = pd.to_numeric(position_data['data.coordinates'].apply(lambda x: x[1]))
-        position_data['z'] = pd.to_numeric(position_data['data.coordinates'].apply(lambda x: x[2]))
+        position_data['position'] = position_data['data.coordinates'].apply(np.asarray)
         position_data['anchor_count'] = pd.to_numeric(position_data['anchor_count']).astype('Int64')
         position_data['socket_read_time'] = pd.to_datetime(position_data['socket_read_time']).dt.tz_localize('UTC')
         position_data['network_time'] = pd.to_numeric(position_data['network_time']).astype('Int64')
         position_data = (
             position_data
             .rename(columns={
                 'object': 'device_id',
                 'coordinate_space': 'coordinate_space_id',
             })
             .reindex(columns=[
                 'position_id',
                 'timestamp',
                 'device_id',
-                'x',
-                'y',
-                'z',
+                'position',
                 'quality',
                 'anchor_count',
                 'socket_read_time',
                 'network_time',
                 'coordinate_space_id',
             ])
             .set_index('position_id')
         )
+        if include_device_info:
+            position_data = (
+                position_data
+                .join(
+                    device_info,
+                    how='left',
+                    on='device_id'
+                )
+            )
+        if include_entity_info or include_material_info:
+            position_data = honeycomb_io.add_device_entity_assignment_info(
+                dataframe=position_data,
+                timestamp_column_name='timestamp',
+                device_id_column_name='device_id',
+                chunk_size=honeycomb_chunk_size,
+                client=honeycomb_client,
+                uri=honeycomb_uri,
+                token_uri=honeycomb_token_uri,
+                audience=honeycomb_audience,
+                client_id=honeycomb_client_id,
+                client_secret=honeycomb_client_secret,
+            )
+        if include_material_info:
+            position_data = honeycomb_io.add_tray_material_assignment_info(
+                dataframe=position_data,
+                timestamp_column_name='timestamp',
+                tray_id_column_name='tray_id',
+                chunk_size=honeycomb_chunk_size,
+                client=honeycomb_client,
+                uri=honeycomb_uri,
+                token_uri=honeycomb_token_uri,
+                audience=honeycomb_audience,
+                client_id=honeycomb_client_id,
+                client_secret=honeycomb_client_secret,
+            )
         return position_data
 
     def fetch_accelerometer_data(
         self,
         start,
         end,
         device_ids=None,
         part_numbers=None,
         serial_numbers=None,
         tag_ids=None,
         names=None,
         environment_id=None,
         environment_name=None,
+        include_device_info=False,
+        include_entity_info=False,
+        include_material_info=False,
         connection=None,
         honeycomb_chunk_size=100,
         honeycomb_client=None,
         honeycomb_uri=None,
         honeycomb_token_uri=None,
         honeycomb_audience=None,
         honeycomb_client_id=None,
         honeycomb_client_secret=None
     ):
-        device_ids = honeycomb_io.fetch_device_ids(
+        device_info = honeycomb_io.fetch_devices(
             device_types=['UWBTAG'],
             device_ids=device_ids,
             part_numbers=part_numbers,
             serial_numbers=serial_numbers,
             tag_ids=tag_ids,
             names=names,
             environment_id=environment_id,
             environment_name=environment_name,
             start=start,
             end=end,
+            output_format='dataframe',
             chunk_size=honeycomb_chunk_size,
             client=honeycomb_client,
             uri=honeycomb_uri,
             token_uri=honeycomb_token_uri,
             audience=honeycomb_audience,
             client_id=honeycomb_client_id,
-            client_secret=honeycomb_client_secret
+            client_secret=honeycomb_client_secret,
         )
+        device_ids = device_info.index.unique().tolist()
         start_utc_naive = start.astimezone(datetime.timezone.utc).replace(tzinfo=None)
         end_utc_naive = end.astimezone(datetime.timezone.utc).replace(tzinfo=None)
         query_list = [
             {'fields': ['timestamp'], 'operator': 'gte', 'values': [start_utc_naive]},
             {'fields': ['timestamp'], 'operator': 'lt', 'values': [end_utc_naive]},
             {'fields': ['device'], 'operator': 'in', 'values': device_ids},
         ]
@@ -156,31 +198,62 @@
             schema='honeycomb',
             fields=None,
             query_list=query_list,
             connection=connection,
             convert_to_dataframe=True
         )
         accelerometer_data['timestamp'] = pd.to_datetime(accelerometer_data['timestamp']).dt.tz_localize('UTC')
-        accelerometer_data['x'] = pd.to_numeric(accelerometer_data['data.data'].apply(lambda x: x[0]))
-        accelerometer_data['y'] = pd.to_numeric(accelerometer_data['data.data'].apply(lambda x: x[1]))
-        accelerometer_data['z'] = pd.to_numeric(accelerometer_data['data.data'].apply(lambda x: x[2]))
+        accelerometer_data['acceleration'] = accelerometer_data['data.data'].apply(np.asarray)
         accelerometer_data['socket_read_time'] = pd.to_datetime(accelerometer_data['socket_read_time']).dt.tz_localize('UTC')
         accelerometer_data['network_time'] = pd.to_numeric(accelerometer_data['network_time']).astype('Int64')
         accelerometer_data = (
             accelerometer_data
             .rename(columns={
                 'device': 'device_id',
             })
             .reindex(columns=[
                 'accelerometer_data_id',
                 'timestamp',
                 'device_id',
-                'x',
-                'y',
-                'z',
+                'acceleration',
                 'socket_read_time',
                 'network_time',
             ])
             .set_index('accelerometer_data_id')
         )
+        if include_device_info:
+            accelerometer_data = (
+                accelerometer_data
+                .join(
+                    device_info,
+                    how='left',
+                    on='device_id'
+                )
+            )
+        if include_entity_info or include_material_info:
+            accelerometer_data = honeycomb_io.add_device_entity_assignment_info(
+                dataframe=accelerometer_data,
+                timestamp_column_name='timestamp',
+                device_id_column_name='device_id',
+                chunk_size=honeycomb_chunk_size,
+                client=honeycomb_client,
+                uri=honeycomb_uri,
+                token_uri=honeycomb_token_uri,
+                audience=honeycomb_audience,
+                client_id=honeycomb_client_id,
+                client_secret=honeycomb_client_secret,
+            )
+        if include_material_info:
+            accelerometer_data = honeycomb_io.add_tray_material_assignment_info(
+                dataframe=accelerometer_data,
+                timestamp_column_name='timestamp',
+                tray_id_column_name='tray_id',
+                chunk_size=honeycomb_chunk_size,
+                client=honeycomb_client,
+                uri=honeycomb_uri,
+                token_uri=honeycomb_token_uri,
+                audience=honeycomb_audience,
+                client_id=honeycomb_client_id,
+                client_secret=honeycomb_client_secret,
+            )
         return accelerometer_data
```

### Comparing `wf_honeycomb_rds_client-0.1.2/pyproject.toml` & `wf_honeycomb_rds_client-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-honeycomb-rds-client"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-honeycomb-rds-client"
-version = "0.1.2"
+version = "0.2.0"
 description = "A client for communicating with the RDS database underlying Honeycomb"
 authors = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 readme = "README.md"
 keywords = []
 repository = "https://github.com/WildflowerSchools/wf-honeycomb-rds-client"
 license = "MIT"
```

### Comparing `wf_honeycomb_rds_client-0.1.2/setup.py` & `wf_honeycomb_rds_client-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pandas>=1.5',
  'toml>=0.10.2,<0.11.0',
  'wf-honeycomb-io>=2.1',
  'wf-postgres-client>=0.1.0']
 
 setup_kwargs = {
     'name': 'wf-honeycomb-rds-client',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'A client for communicating with the RDS database underlying Honeycomb',
     'long_description': '# honeycomb_rds_client\n\nA client for communicating with the RDS database underlying Honeycomb\n\n## Installation\n\n`pip install wf-honeycomb-rds-client`\n\n## Development\n\n### Requirements\n\n* [Poetry](https://python-poetry.org/)\n* [just](https://github.com/casey/just)\n\n### Install\n\n`poetry install`\n\n\n#### Install w/ Python Version from PyEnv\n\n```\n# Specify pyenv python version\npyenv shell --unset\npyenv local <<VERSION>>\n\n# Set poetry python to pyenv version\npoetry env use $(pyenv which python)\npoetry cache clear . --all\npoetry install\n```\n\n## Task list\n* TBD\n',
     'author': 'Theodore Quinn',
     'author_email': 'ted.quinn@wildflowerschools.org',
     'maintainer': 'Theodore Quinn',
     'maintainer_email': 'ted.quinn@wildflowerschools.org',
     'url': 'https://github.com/WildflowerSchools/wf-honeycomb-rds-client',
```

### Comparing `wf_honeycomb_rds_client-0.1.2/PKG-INFO` & `wf_honeycomb_rds_client-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-honeycomb-rds-client
-Version: 0.1.2
+Version: 0.2.0
 Summary: A client for communicating with the RDS database underlying Honeycomb
 Home-page: https://github.com/WildflowerSchools/wf-honeycomb-rds-client
 License: MIT
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 Maintainer: Theodore Quinn
 Maintainer-email: ted.quinn@wildflowerschools.org
```

