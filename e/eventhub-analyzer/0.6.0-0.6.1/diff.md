# Comparing `tmp/eventhub_analyzer-0.6.0.tar.gz` & `tmp/eventhub_analyzer-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventhub_analyzer-0.6.0.tar", max compression
+gzip compressed data, was "eventhub_analyzer-0.6.1.tar", max compression
```

## Comparing `eventhub_analyzer-0.6.0.tar` & `eventhub_analyzer-0.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2160 2023-06-21 10:10:30.249503 eventhub_analyzer-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.6.0/eventhub_analyzer/__init__.py
--rw-r--r--   0        0        0    14180 2023-06-22 14:10:50.993043 eventhub_analyzer-0.6.0/eventhub_analyzer/main.py
--rw-r--r--   0        0        0      626 2023-08-02 10:05:36.479853 eventhub_analyzer-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 eventhub_analyzer-0.6.0/setup.py
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 eventhub_analyzer-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2160 2023-06-21 10:10:30.249503 eventhub_analyzer-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.6.1/eventhub_analyzer/__init__.py
+-rw-r--r--   0        0        0    14157 2023-08-02 10:11:08.543626 eventhub_analyzer-0.6.1/eventhub_analyzer/main.py
+-rw-r--r--   0        0        0      626 2023-08-02 10:11:59.255594 eventhub_analyzer-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 eventhub_analyzer-0.6.1/setup.py
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 eventhub_analyzer-0.6.1/PKG-INFO
```

### Comparing `eventhub_analyzer-0.6.0/README.md` & `eventhub_analyzer-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `eventhub_analyzer-0.6.0/eventhub_analyzer/main.py` & `eventhub_analyzer-0.6.1/eventhub_analyzer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,14 @@
 @container_name_option
 @cli.command(help="Clear checkpoints")
 def clear_checkpoints(connection_string, container_name, event_hub, consumer_group):
     clear_checkpoint_operation(connection_string, container_name, event_hub, consumer_group)
 
 
 @connection_string_option
-@consumer_group_option
 @event_hub_option
 @container_name_option
 @cli.command(help="Analyze owners of partitions")
 def owners(connection_string, container_name, event_hub):
     owner_analysis(connection_string, container_name)
```

### Comparing `eventhub_analyzer-0.6.0/pyproject.toml` & `eventhub_analyzer-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventhub-analyzer"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Stefan Hudelmaier <stefan.hudelmaier@device-insight.com>"]
 readme = "README.md"
 packages = [{include = "eventhub_analyzer"}]
 repository = "https://github.com/deviceinsight/eventhub-analyzer"
 
 [tool.poetry.dependencies]
```

### Comparing `eventhub_analyzer-0.6.0/setup.py` & `eventhub_analyzer-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'texttable>=1.6.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['eventhub-analyzer = eventhub_analyzer.main:cli']}
 
 setup_kwargs = {
     'name': 'eventhub-analyzer',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': '',
     'long_description': "# Event Hub Analyzer\n\nEvent Hub Analyzer is a small command line tool that can be used\nto analyze certain aspects of Event Hubs.\n\n## Installation\n\n```\npip install eventhub-analyzer\n```\n\n## Checkpoints per partition\n\nFor every event hub, consumer group, the number of \nevents/sequence numbers between two invocations is retrieved and\nthe throughput per partition is calculated. This can be used to \ndetermine if the load is correctly distributed among partitions.\n\nWhen there are some partition that get little to no throughput while\nothers have large throughput, it is a sign that the partition key\nis not chosen optimally and that you should try to choose a property\nwith a higher cardinality as the partition key.\n\n### Usage\n\n```bash\neventhub-analyzer checkpoints -n CONTAINER_NAME -c CONNECTION_STRING\n```\n\nYou can also specify the settings via environment variables:\n\n```bash\nexport STORAGE_ACCOUNT_CONNECTION_STRING='DefaultEndpointsProtocol=https;AccountName=x;AccountKey=y;EndpointSuffix=core.windows.net'\nexport CONTAINER_NAME='event-hub-offsets'\neventhub-analyzer checkpoints\n```\n\n### Example output\n\n```\nEvent Hub: telemetry, Consumer Group: my-consumer\nEvent Hub   Consumer Group   Partition   Events per second\ntelemetry   my-consumer              0             158.034\ntelemetry   my-consumer              1             203.257\ntelemetry   my-consumer              2             148.103\ntelemetry   my-consumer              3               0.000\ntelemetry   my-consumer              4             201.780\ntelemetry   my-consumer              5             106.081\ntelemetry   my-consumer              6              72.307\ntelemetry   my-consumer              7             160.783\ntelemetry   my-consumer              8             118.351\n```\n\nAs you can see, partition 3 is not getting any events and\nthe number of events is not well distributed overall. There\nmight be some gains possible by choosing a different partition key\n(or by partitioning manually on the client).\n\n### Clearing checkpoints\n\nExample:\n\n```bash\neventhub-analyzer clear-checkpoints --consumer-group redis-timeseries\n```\n\n## Publishing\n\n```\npoetry build\npoetry publish\n```\n",
     'author': 'Stefan Hudelmaier',
     'author_email': 'stefan.hudelmaier@device-insight.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/deviceinsight/eventhub-analyzer',
```

### Comparing `eventhub_analyzer-0.6.0/PKG-INFO` & `eventhub_analyzer-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhub-analyzer
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Home-page: https://github.com/deviceinsight/eventhub-analyzer
 Author: Stefan Hudelmaier
 Author-email: stefan.hudelmaier@device-insight.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

