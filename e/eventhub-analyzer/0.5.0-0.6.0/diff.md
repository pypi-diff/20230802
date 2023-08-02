# Comparing `tmp/eventhub_analyzer-0.5.0.tar.gz` & `tmp/eventhub_analyzer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventhub_analyzer-0.5.0.tar", max compression
+gzip compressed data, was "eventhub_analyzer-0.6.0.tar", max compression
```

## Comparing `eventhub_analyzer-0.5.0.tar` & `eventhub_analyzer-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2041 2023-04-26 09:25:09.524728 eventhub_analyzer-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.5.0/eventhub_analyzer/__init__.py
--rw-r--r--   0        0        0    12354 2023-02-22 15:59:56.060035 eventhub_analyzer-0.5.0/eventhub_analyzer/main.py
--rw-r--r--   0        0        0      626 2023-06-20 12:54:14.916880 eventhub_analyzer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 eventhub_analyzer-0.5.0/setup.py
--rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 eventhub_analyzer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2160 2023-06-21 10:10:30.249503 eventhub_analyzer-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.6.0/eventhub_analyzer/__init__.py
+-rw-r--r--   0        0        0    14180 2023-06-22 14:10:50.993043 eventhub_analyzer-0.6.0/eventhub_analyzer/main.py
+-rw-r--r--   0        0        0      626 2023-08-02 10:05:36.479853 eventhub_analyzer-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 eventhub_analyzer-0.6.0/setup.py
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 eventhub_analyzer-0.6.0/PKG-INFO
```

### Comparing `eventhub_analyzer-0.5.0/README.md` & `eventhub_analyzer-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -52,13 +52,21 @@
 ```
 
 As you can see, partition 3 is not getting any events and
 the number of events is not well distributed overall. There
 might be some gains possible by choosing a different partition key
 (or by partitioning manually on the client).
 
+### Clearing checkpoints
+
+Example:
+
+```bash
+eventhub-analyzer clear-checkpoints --consumer-group redis-timeseries
+```
+
 ## Publishing
 
 ```
 poetry build
 poetry publish
 ```
```

### Comparing `eventhub_analyzer-0.5.0/eventhub_analyzer/main.py` & `eventhub_analyzer-0.6.0/eventhub_analyzer/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import datetime
+import statistics
 
 import click
 import jsonpickle
 from azure.storage.blob import BlobServiceClient
 from azure.eventhub import EventHubConsumerClient
 import itertools
 from dotenv import load_dotenv
@@ -60,28 +61,36 @@
                                   't',
                                   'i',
                                   'i',
                                   'f'])
             table.set_cols_align(["l", "l", "r", "r", "r"])
             table.add_row(["Event Hub", "Consumer Group", "Partition", "Sequence number", "Events per second"])
             partition_ids = sorted(current_event_hubs[event_hub_name][consumer_group_name], key=lambda p: int(p))
+            events_per_seconds_stats = []
             for partition_id in partition_ids:
                 current_checkpoint = current_event_hubs[event_hub_name][consumer_group_name][partition_id]
                 try:
                     previous_checkpoint = previous_event_hubs[event_hub_name][consumer_group_name][partition_id]
                     sequence_delta = current_checkpoint.sequence_number - previous_checkpoint.sequence_number
                     events_per_second = sequence_delta / difference_in_seconds
+                    events_per_seconds_stats.append(events_per_second)
                 except KeyError:
                     events_per_second = -1
 
                 table.add_row([event_hub_name, consumer_group_name, partition_id, current_checkpoint.sequence_number,
                                events_per_second])
 
             click.echo(table.draw())
             click.echo()
+            click.echo("Events per second stats:")
+            click.echo(f"Min: {min(events_per_seconds_stats):.3f}")
+            click.echo(f"Max: {max(events_per_seconds_stats):.3f}")
+            click.echo(f"Avg: {sum(events_per_seconds_stats) / len(events_per_seconds_stats):.3f}")
+            click.echo(f"StdDev: {statistics.stdev(events_per_seconds_stats):.3f}")
+            click.echo()
 
 
 def checkpoint_analysis(connection_string, container_name, event_hub_filter, consumer_group_filter):
     previous_data = load_persisted_data()
 
     raw_checkpoints = get_data_from_container('checkpoint', connection_string, container_name)
 
@@ -92,14 +101,30 @@
         click.echo("No previous run found, cannot perform analysis. Wait a minute and run this command again.")
     else:
         previous_timestamp = datetime.datetime.fromisoformat(previous_data.timestamp)
         run_checkpoint_analysis(now(), event_hubs, previous_timestamp, previous_data.event_hubs, event_hub_filter,
                                 consumer_group_filter)
 
 
+def clear_checkpoint_operation(connection_string, container_name, event_hub_filter, consumer_group_filter):
+    if consumer_group_filter is None:
+        print("You must specify a consumer group")
+        return
+    blob_service_client = BlobServiceClient.from_connection_string(connection_string)
+    container_client = blob_service_client.get_container_client(container=container_name)
+    blob_list = container_client.list_blobs(include='metadata')
+    for blob in blob_list:
+        name = blob.name
+        _, event_hub_name, consumer_group_name, entity, partition_id = name.split('/')
+        if consumer_group_name == consumer_group_filter and entity == 'checkpoint':
+            print(f"Deleting blob: {name}")
+            blob_client = blob_service_client.get_blob_client(container=container_name, blob=name)
+            blob_client.delete_blob()
+
+
 def group_raw_checkpoints(raw_checkpoints):
     """
     Groups the checkpoints in nested dicts: event_hub -> consumer_group -> partition_id
     :param raw_checkpoints:
     :return:
     """
     event_hubs = {}
@@ -144,14 +169,15 @@
                    "Consumer Group",
                    "Partition",
                    "Read/Committed Sequence number",
                    "Written/Enqueued Sequence Number",
                    "Lag",
                    ])
     for partition_id in event_hub_client.get_partition_ids():
+        print(f"Getting data for partition {partition_id}")
         partition_properties = event_hub_client.get_partition_properties(partition_id)
         read_sequence_number = relevant_checkpoints[partition_id].sequence_number
         written_sequence_number = partition_properties['last_enqueued_sequence_number']
         lag = written_sequence_number - read_sequence_number
 
         table.add_row([event_hub,
                        consumer_group,
@@ -170,16 +196,16 @@
     blob_list = container_client.list_blobs(include='metadata')
     result = []
     for blob in blob_list:
         name = blob.name
         _, event_hub_name, consumer_group_name, entity, partition_id = name.split('/')
 
         if entity_to_get == entity == 'checkpoint':
-            sequence_number = int(blob.metadata['sequencenumber'])
-            offset = int(blob.metadata['offset'])
+            sequence_number = int(blob.metadata['sequencenumber']) if blob.metadata is not None else 0
+            offset = int(blob.metadata['offset']) if blob.metadata is not None else 0
             checkpoint = RawCheckpoint(event_hub_name, consumer_group_name, partition_id, sequence_number, offset)
             result.append(checkpoint)
 
         if entity_to_get == entity == 'ownership':
             ownership = Ownership(event_hub_name, consumer_group_name, partition_id, blob.metadata['ownerid'])
             result.append(ownership)
     return result
@@ -279,14 +305,23 @@
     checkpoint_analysis(connection_string, container_name, event_hub, consumer_group)
 
 
 @connection_string_option
 @consumer_group_option
 @event_hub_option
 @container_name_option
+@cli.command(help="Clear checkpoints")
+def clear_checkpoints(connection_string, container_name, event_hub, consumer_group):
+    clear_checkpoint_operation(connection_string, container_name, event_hub, consumer_group)
+
+
+@connection_string_option
+@consumer_group_option
+@event_hub_option
+@container_name_option
 @cli.command(help="Analyze owners of partitions")
 def owners(connection_string, container_name, event_hub):
     owner_analysis(connection_string, container_name)
 
 
 @connection_string_option
 @container_name_option
```

### Comparing `eventhub_analyzer-0.5.0/pyproject.toml` & `eventhub_analyzer-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventhub-analyzer"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Stefan Hudelmaier <stefan.hudelmaier@device-insight.com>"]
 readme = "README.md"
 packages = [{include = "eventhub_analyzer"}]
 repository = "https://github.com/deviceinsight/eventhub-analyzer"
 
 [tool.poetry.dependencies]
```

### Comparing `eventhub_analyzer-0.5.0/setup.py` & `eventhub_analyzer-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'texttable>=1.6.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['eventhub-analyzer = eventhub_analyzer.main:cli']}
 
 setup_kwargs = {
     'name': 'eventhub-analyzer',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
-    'long_description': "# Event Hub Analyzer\n\nEvent Hub Analyzer is a small command line tool that can be used\nto analyze certain aspects of Event Hubs.\n\n## Installation\n\n```\npip install eventhub-analyzer\n```\n\n## Checkpoints per partition\n\nFor every event hub, consumer group, the number of \nevents/sequence numbers between two invocations is retrieved and\nthe throughput per partition is calculated. This can be used to \ndetermine if the load is correctly distributed among partitions.\n\nWhen there are some partition that get little to no throughput while\nothers have large throughput, it is a sign that the partition key\nis not chosen optimally and that you should try to choose a property\nwith a higher cardinality as the partition key.\n\n### Usage\n\n```bash\neventhub-analyzer checkpoints -n CONTAINER_NAME -c CONNECTION_STRING\n```\n\nYou can also specify the settings via environment variables:\n\n```bash\nexport STORAGE_ACCOUNT_CONNECTION_STRING='DefaultEndpointsProtocol=https;AccountName=x;AccountKey=y;EndpointSuffix=core.windows.net'\nexport CONTAINER_NAME='event-hub-offsets'\neventhub-analyzer checkpoints\n```\n\n### Example output\n\n```\nEvent Hub: telemetry, Consumer Group: my-consumer\nEvent Hub   Consumer Group   Partition   Events per second\ntelemetry   my-consumer              0             158.034\ntelemetry   my-consumer              1             203.257\ntelemetry   my-consumer              2             148.103\ntelemetry   my-consumer              3               0.000\ntelemetry   my-consumer              4             201.780\ntelemetry   my-consumer              5             106.081\ntelemetry   my-consumer              6              72.307\ntelemetry   my-consumer              7             160.783\ntelemetry   my-consumer              8             118.351\n```\n\nAs you can see, partition 3 is not getting any events and\nthe number of events is not well distributed overall. There\nmight be some gains possible by choosing a different partition key\n(or by partitioning manually on the client).\n\n## Publishing\n\n```\npoetry build\npoetry publish\n```\n",
+    'long_description': "# Event Hub Analyzer\n\nEvent Hub Analyzer is a small command line tool that can be used\nto analyze certain aspects of Event Hubs.\n\n## Installation\n\n```\npip install eventhub-analyzer\n```\n\n## Checkpoints per partition\n\nFor every event hub, consumer group, the number of \nevents/sequence numbers between two invocations is retrieved and\nthe throughput per partition is calculated. This can be used to \ndetermine if the load is correctly distributed among partitions.\n\nWhen there are some partition that get little to no throughput while\nothers have large throughput, it is a sign that the partition key\nis not chosen optimally and that you should try to choose a property\nwith a higher cardinality as the partition key.\n\n### Usage\n\n```bash\neventhub-analyzer checkpoints -n CONTAINER_NAME -c CONNECTION_STRING\n```\n\nYou can also specify the settings via environment variables:\n\n```bash\nexport STORAGE_ACCOUNT_CONNECTION_STRING='DefaultEndpointsProtocol=https;AccountName=x;AccountKey=y;EndpointSuffix=core.windows.net'\nexport CONTAINER_NAME='event-hub-offsets'\neventhub-analyzer checkpoints\n```\n\n### Example output\n\n```\nEvent Hub: telemetry, Consumer Group: my-consumer\nEvent Hub   Consumer Group   Partition   Events per second\ntelemetry   my-consumer              0             158.034\ntelemetry   my-consumer              1             203.257\ntelemetry   my-consumer              2             148.103\ntelemetry   my-consumer              3               0.000\ntelemetry   my-consumer              4             201.780\ntelemetry   my-consumer              5             106.081\ntelemetry   my-consumer              6              72.307\ntelemetry   my-consumer              7             160.783\ntelemetry   my-consumer              8             118.351\n```\n\nAs you can see, partition 3 is not getting any events and\nthe number of events is not well distributed overall. There\nmight be some gains possible by choosing a different partition key\n(or by partitioning manually on the client).\n\n### Clearing checkpoints\n\nExample:\n\n```bash\neventhub-analyzer clear-checkpoints --consumer-group redis-timeseries\n```\n\n## Publishing\n\n```\npoetry build\npoetry publish\n```\n",
     'author': 'Stefan Hudelmaier',
     'author_email': 'stefan.hudelmaier@device-insight.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/deviceinsight/eventhub-analyzer',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `eventhub_analyzer-0.5.0/PKG-INFO` & `eventhub_analyzer-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhub-analyzer
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Home-page: https://github.com/deviceinsight/eventhub-analyzer
 Author: Stefan Hudelmaier
 Author-email: stefan.hudelmaier@device-insight.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -72,14 +72,22 @@
 ```
 
 As you can see, partition 3 is not getting any events and
 the number of events is not well distributed overall. There
 might be some gains possible by choosing a different partition key
 (or by partitioning manually on the client).
 
+### Clearing checkpoints
+
+Example:
+
+```bash
+eventhub-analyzer clear-checkpoints --consumer-group redis-timeseries
+```
+
 ## Publishing
 
 ```
 poetry build
 poetry publish
 ```
```

