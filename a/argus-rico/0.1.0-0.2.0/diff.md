# Comparing `tmp/argus_rico-0.1.0.tar.gz` & `tmp/argus_rico-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus_rico-0.1.0.tar", max compression
+gzip compressed data, was "argus_rico-0.2.0.tar", max compression
```

## Comparing `argus_rico-0.1.0.tar` & `argus_rico-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus_rico-0.1.0/LICENSE
--rw-r--r--   0        0        0     1345 2023-07-21 06:18:18.257825 argus_rico-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3619 2023-07-21 03:00:36.041304 argus_rico-0.1.0/src/argus_rico/__init__.py
--rw-r--r--   0        0        0       67 2023-07-19 01:08:54.295571 argus_rico-0.1.0/src/argus_rico/catalogs/__init__.py
--rw-r--r--   0        0        0     8750 2023-07-21 00:21:26.572087 argus_rico-0.1.0/src/argus_rico/catalogs/atlas.py
--rw-r--r--   0        0        0     1991 2023-07-21 00:31:24.283558 argus_rico-0.1.0/src/argus_rico/cli.py
--rw-r--r--   0        0        0     1162 2023-07-21 06:16:58.642013 argus_rico-0.1.0/src/argus_rico/consumer.py
--rw-r--r--   0        0        0      430 2023-07-21 03:00:53.645017 argus_rico-0.1.0/src/argus_rico/efte/__init__.py
--rw-r--r--   0        0        0     3735 2023-07-19 01:08:54.295934 argus_rico-0.1.0/src/argus_rico/efte/db.py
--rw-r--r--   0        0        0      878 2023-07-21 00:32:52.766382 argus_rico-0.1.0/src/argus_rico/efte/efte_runner.py
--rw-r--r--   0        0        0     1439 2023-07-21 00:31:06.618228 argus_rico-0.1.0/src/argus_rico/efte/processor.py
--rw-r--r--   0        0        0      659 2023-07-21 06:16:58.642198 argus_rico-0.1.0/src/argus_rico/efte/schemas/efte.alert.avsc
--rw-r--r--   0        0        0     3609 2023-07-21 06:16:58.642318 argus_rico-0.1.0/src/argus_rico/efte/schemas/efte.candidate.avsc
--rw-r--r--   0        0        0      895 2023-07-21 06:16:58.642438 argus_rico-0.1.0/src/argus_rico/efte/schemas/efte.xmatch.avsc
--rw-r--r--   0        0        0     3616 2023-07-21 06:16:58.642565 argus_rico-0.1.0/src/argus_rico/efte/schemas/raw_candidate.avsc
--rw-r--r--   0        0        0     9082 2023-07-21 06:16:58.642773 argus_rico-0.1.0/src/argus_rico/efte/stream.py
--rw-r--r--   0        0        0     4063 2023-07-21 00:33:38.742980 argus_rico-0.1.0/src/argus_rico/efte/vetnet.py
--rw-r--r--   0        0        0     1944 2023-07-21 00:33:55.798019 argus_rico-0.1.0/src/argus_rico/efte/watchdog.py
--rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus_rico-0.1.0/src/argus_rico/heartbeat.py
--rw-r--r--   0        0        0     5049 2023-07-19 01:08:54.296496 argus_rico-0.1.0/src/argus_rico/images.py
--rw-r--r--   0        0        0      262 2023-06-12 16:35:31.667792 argus_rico-0.1.0/src/argus_rico/models/__init__.py
--rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus_rico-0.1.0/src/argus_rico/models/evr_image.py
--rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus_rico-0.1.0/src/argus_rico/producer.py
--rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus_rico-0.1.0/src/argus_rico/py.typed
--rw-r--r--   0        0        0     2845 2023-07-19 23:57:27.800686 argus_rico-0.1.0/src/argus_rico/s3.py
--rw-r--r--   0        0        0     9084 2023-07-19 01:08:54.296760 argus_rico-0.1.0/src/argus_rico/slack.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 argus_rico-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus_rico-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1345 2023-08-02 03:41:31.806139 argus_rico-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3619 2023-08-01 15:17:21.804082 argus_rico-0.2.0/src/argus_rico/__init__.py
+-rw-r--r--   0        0        0       67 2023-07-19 01:08:54.295571 argus_rico-0.2.0/src/argus_rico/catalogs/__init__.py
+-rw-r--r--   0        0        0     8750 2023-07-21 00:21:26.572087 argus_rico-0.2.0/src/argus_rico/catalogs/atlas.py
+-rw-r--r--   0        0        0     2728 2023-08-02 03:34:16.263004 argus_rico-0.2.0/src/argus_rico/cli.py
+-rw-r--r--   0        0        0     1162 2023-08-01 16:33:55.909016 argus_rico-0.2.0/src/argus_rico/consumer.py
+-rw-r--r--   0        0        0      388 2023-08-02 03:34:16.263244 argus_rico-0.2.0/src/argus_rico/efte/__init__.py
+-rw-r--r--   0        0        0     3735 2023-07-19 01:08:54.295934 argus_rico-0.2.0/src/argus_rico/efte/db.py
+-rw-r--r--   0        0        0      878 2023-07-21 00:32:52.766382 argus_rico-0.2.0/src/argus_rico/efte/efte_runner.py
+-rw-r--r--   0        0        0     1848 2023-08-02 03:34:16.263454 argus_rico-0.2.0/src/argus_rico/efte/processor.py
+-rw-r--r--   0        0        0      659 2023-07-21 06:16:58.642198 argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.alert.avsc
+-rw-r--r--   0        0        0     3700 2023-08-02 03:34:16.263689 argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.candidate.avsc
+-rw-r--r--   0        0        0      895 2023-07-21 06:16:58.642438 argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.xmatch.avsc
+-rw-r--r--   0        0        0     3616 2023-07-21 06:16:58.642565 argus_rico-0.2.0/src/argus_rico/efte/schemas/raw_candidate.avsc
+-rw-r--r--   0        0        0     7282 2023-08-02 03:34:16.263896 argus_rico-0.2.0/src/argus_rico/efte/stream.py
+-rw-r--r--   0        0        0     4175 2023-08-01 16:38:21.655761 argus_rico-0.2.0/src/argus_rico/efte/vetnet.py
+-rw-r--r--   0        0        0     1978 2023-08-02 03:34:16.264112 argus_rico-0.2.0/src/argus_rico/efte/watchdog.py
+-rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus_rico-0.2.0/src/argus_rico/heartbeat.py
+-rw-r--r--   0        0        0     5049 2023-07-19 01:08:54.296496 argus_rico-0.2.0/src/argus_rico/images.py
+-rw-r--r--   0        0        0      379 2023-08-02 03:41:12.508808 argus_rico-0.2.0/src/argus_rico/models/__init__.py
+-rw-r--r--   0        0        0     1727 2023-08-02 03:34:16.264367 argus_rico-0.2.0/src/argus_rico/models/efte_alert.py
+-rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus_rico-0.2.0/src/argus_rico/models/evr_image.py
+-rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus_rico-0.2.0/src/argus_rico/producer.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus_rico-0.2.0/src/argus_rico/py.typed
+-rw-r--r--   0        0        0     2845 2023-07-19 23:57:27.800686 argus_rico-0.2.0/src/argus_rico/s3.py
+-rw-r--r--   0        0        0     9139 2023-07-25 22:16:36.634429 argus_rico-0.2.0/src/argus_rico/slack.py
+-rw-r--r--   0        0        0      828 2023-08-02 03:34:16.264530 argus_rico-0.2.0/src/argus_rico/utils.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 argus_rico-0.2.0/PKG-INFO
```

### Comparing `argus_rico-0.1.0/LICENSE` & `argus_rico-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/pyproject.toml` & `argus_rico-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "argus-rico"
-version = "0.1.0"
+version = "0.2.0"
 description = "Transient alert generation and database interaction for Argus and Evryscope"
 authors = ["Hank Corbett"]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 python-dotenv = "^0.19.0"
 fastavro = "^1.4.12"
```

### Comparing `argus_rico-0.1.0/src/argus_rico/__init__.py` & `argus_rico-0.2.0/src/argus_rico/__init__.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/catalogs/atlas.py` & `argus_rico-0.2.0/src/argus_rico/catalogs/atlas.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/consumer.py` & `argus_rico-0.2.0/src/argus_rico/consumer.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/db.py` & `argus_rico-0.2.0/src/argus_rico/efte/db.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/efte_runner.py` & `argus_rico-0.2.0/src/argus_rico/efte/efte_runner.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/processor.py` & `argus_rico-0.2.0/src/argus_rico/efte/processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 """Ray-parallelizable EFTE catalog reducer."""
+import os
+
 import astropy.table as tbl
 import ray
 
-from .. import catalogs
+from .. import catalogs, get_logger, utils
 from .stream import EFTEAlertStreamer
 from .vetnet import VetNet
 
 
 @ray.remote
 class EFTECatalogProcessor:
     def __init__(self):
         """Initialize the EFTECatalogProcessor class."""
         self.vetnet = VetNet()
         self.atlas = catalogs.ATLASRefcat2()
         self.producer = EFTEAlertStreamer()
 
+        self.log = get_logger(__name__)
+
     def process(self, filepath: str) -> None:
         """Perform vetting and crossmatching for the given FITS table.
 
         Args:
             filepath (str): The path to the FITS table.
 
         Returns:
             Table: Returns the FITS table with normalized stamps, scores.
         """
+        clock = utils.Timer(log=self.log)
+        name = os.path.basename(filepath)
         table: tbl.Table = tbl.Table.read(filepath, format="fits")
+        clock.ping(f"Read {len(table)} candidates from {name}")
 
         stamps = table["stamp"].data
         mean_pred, _, _, confidence = self.vetnet.mc_predict(stamps, 10)
+        clock.ping(f"Vetted candidates from {name}")
 
-        table["vetnet"] = confidence[:, 0]
+        table["vetnet_score"] = confidence[:, 0]
         table = table[mean_pred[:, 0] > 0.5]
+        table = table[table["vetnet_score"] > 0.4]  # fairly arbitrary...
+
+        clock.ping(f"Reporting {len(table)} candidates in {name}")
 
-        table = table[table["vetnet"] > 0.4]  # fairly arbitrary...
         if len(table) == 0:
             return
-
         crossmatches = []
         for r in table:
             phot = self.atlas.radial(
                 r["ra"], r["dec"], 0.01, max_g=25, return_area=False
             )
             phot = phot.sort_values(by="separation")
             crossmatches.append(phot.to_dict(orient="records"))
 
+        clock.ping(f"Xmatched {name} with ATLAS Refcat")
+
         self.producer.push_alert(table, crossmatches)
```

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/schemas/efte.alert.avsc` & `argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.alert.avsc`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/schemas/efte.candidate.avsc` & `argus_rico-0.2.0/src/argus_rico/efte/schemas/raw_candidate.avsc`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'doc'": "'avro alert schema, evryscope/argus optical array, EFTE pipeline'",*

 * * "'name'": "'raw_candidate'",*

 * * "'namespace'": "'rico.efte'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "doc": "avro alert schema, evryscope/argus optical array, EFTE candidate.",
+    "doc": "avro alert schema, evryscope/argus optical array, EFTE pipeline",
     "fields": [
         {
             "name": "epoch",
             "type": "float"
         },
         {
             "name": "camera",
@@ -174,12 +174,12 @@
             "type": "float"
         },
         {
             "name": "stamp",
             "type": "bytes"
         }
     ],
-    "name": "candidate",
-    "namespace": "efte",
+    "name": "raw_candidate",
+    "namespace": "rico.efte",
     "type": "record",
     "version": "0.1"
 }
```

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/schemas/efte.xmatch.avsc` & `argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.xmatch.avsc`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/schemas/raw_candidate.avsc` & `argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.candidate.avsc`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7476851851851851%*

 * *Differences: {"'doc'": "'avro alert schema, evryscope/argus optical array, EFTE candidate.'",*

 * * "'fields'": "{44: {'name': 'stamp_bytes'}, insert: [(3, OrderedDict([('name', 'vetnet_score'), "*

 * *             "('type', 'float')]))]}",*

 * * "'name'": "'candidate'",*

 * * "'namespace'": "'efte'"}*

```diff
@@ -1,23 +1,27 @@
 {
-    "doc": "avro alert schema, evryscope/argus optical array, EFTE pipeline",
+    "doc": "avro alert schema, evryscope/argus optical array, EFTE candidate.",
     "fields": [
         {
             "name": "epoch",
             "type": "float"
         },
         {
             "name": "camera",
             "type": "string"
         },
         {
             "name": "thresh",
             "type": "float"
         },
         {
+            "name": "vetnet_score",
+            "type": "float"
+        },
+        {
             "name": "npix",
             "type": "int"
         },
         {
             "name": "tnpix",
             "type": "int"
         },
@@ -170,16 +174,16 @@
             "type": "float"
         },
         {
             "name": "dec",
             "type": "float"
         },
         {
-            "name": "stamp",
+            "name": "stamp_bytes",
             "type": "bytes"
         }
     ],
-    "name": "raw_candidate",
-    "namespace": "rico.efte",
+    "name": "candidate",
+    "namespace": "efte",
     "type": "record",
     "version": "0.1"
 }
```

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/stream.py` & `argus_rico-0.2.0/src/argus_rico/efte/stream.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,29 @@
-__all__ = ["RawAlertStreamer"]
+__all__ = ["EFTEAlertReceiver", "EFTEAlertStreamer"]
 
+import base64
 import io
 import os
 from typing import Any, Dict, List, Optional, Tuple
 from uuid import uuid4
 
 import astropy.table as tbl
 import blosc
 import fastavro as fa
 import orjson
 import pandas as pd
 from confluent_kafka import KafkaException
 
-from .. import config
+from .. import config, get_logger
 from ..consumer import Consumer
 from ..producer import Producer
 
 PATH = os.path.realpath(os.path.dirname(__file__))
 
 
-class RawAlertStreamer(Producer):
-    def __init__(self) -> None:
-        """
-        Initialize the RawAlertStreamer instance.
-
-        It inherits from the Producer class and configures the Kafka connection parameters
-        using values from the config dictionary.
-
-        This class is used for streaming raw candidate detections from the
-        observatory to the Rico Kafka cluster.
-
-        The host, port, and topic are retrieved from the config dictionary
-        using the keys 'KAFKA_ADDR', 'KAFKA_PORT', and 'HBEAT_TOPIC' respectively.
-        """
-        super().__init__(
-            host=config.KAFKA_ADDR,
-            port=config.KAFKA_PORT,
-        )
-        self.topic_base = config.RAW_TOPIC_BASE
-
-    def _parse_raw_catalog(self, catalog_path: str) -> Tuple[bytes, Dict[str, Any]]:
-        """
-        Parses a raw catalog file and returns the serialized Avro data.
-
-        Args:
-            catalog_path (str): The path to the catalog file.
-
-        Returns:
-            bytes: The serialized Avro data.
-            dict: Catalog metadata.
-        """
-        tab = tbl.Table.read(catalog_path)
-
-        mjd = tab.meta["MJD"]
-        camera_id = tab.meta["CCDDETID"]
-
-        records = []
-        for r in tab:
-            stamp = blosc.compress(r["stamp"].tobytes())
-            record = dict(r)
-            record["stamp"] = stamp
-            record["epoch"] = mjd
-            record["camera"] = camera_id
-
-            records.append(record)
-
-        with open(f"{PATH}/schemas/raw_candidate.avsc", "rb") as f:
-            schema = orjson.loads(f.read())
-
-        parsed_schema = fa.parse_schema(schema)
-
-        fo = io.BytesIO()
-        fa.writer(fo, parsed_schema, records)
-        fo.seek(0)
-
-        return fo.read(), tab.meta
-
-    def push_from_catalog(self, catalog_path: str) -> None:
-        """
-        Pushes data from a catalog file to a camera-specific topic.
-
-        Args:
-            catalog_path (str): The path to the catalog file.
-
-        Returns:
-            None
-
-        """
-        avro_data, metadata = self._parse_raw_catalog(catalog_path)
-        topic = self.topic_base + f'.{metadata["CCDDETID"]}'
-
-        self.send_binary(avro_data, topic=topic)
-
-
 class EFTEAlertStreamer(Producer):
     def __init__(self) -> None:
         """
         Initialize the EFTEAlertStreamer instance.
 
         It inherits from the Producer class and configures the Kafka connection parameters
         using values from the config dictionary.
@@ -128,28 +55,34 @@
 
         Returns:
             bytes: The serialized Avro data.
             dict: Catalog metadata.
         """
         tab = catalog
 
+        if "MJD" not in tab.meta:
+            tab.meta["MJD"] = 60000.1
+        if "CCDDETID" not in tab.meta:
+            tab.meta["CCDDETID"] = "ML3103817"
+
         mjd = tab.meta["MJD"]
         camera_id = tab.meta["CCDDETID"]
 
         records = []
         for i, r in enumerate(tab):
             alert_data = {
                 "schemavsn": self.parsed_alert_schema["version"],
                 "publisher": "rico.efte_generator",
                 "objectId": str(uuid4()),
             }
 
-            stamp = blosc.compress(r["stamp"].tobytes())
+            stamp = blosc.compress(r["stamp"].data.tobytes())
+
             candidate = dict(r)
-            candidate["stamp"] = stamp
+            candidate["stamp_bytes"] = stamp
             candidate["epoch"] = mjd
             candidate["camera"] = camera_id
 
             alert_data["candidate"] = candidate
             alert_data["xmatch"] = xmatches[i]
 
             records.append(alert_data)
@@ -197,14 +130,15 @@
         )
 
         self.parsed_alert_schema = fa.schema.load_schema(
             f"{PATH}/schemas/efte.alert.avsc"
         )
         self.filter_path = filter_path
         self.output_path = output_path
+        self.log = get_logger(__name__)
 
     def poll_and_record(self) -> None:
         """Start polling for Kafka messages and process the candidates based on filter conditions."""
         c = self.get_consumer()
 
         c.subscribe(
             [
@@ -215,16 +149,16 @@
             while True:
                 event = c.poll(1.0)
                 if event is None:
                     continue
                 if event.error():
                     raise KafkaException(event.error())
                 else:
-                    candidates = self._decode(event.value())
-                    self._filter_candidates(candidates)
+                    alerts = self._decode(event.value())
+                    self._filter_to_disk(alerts)
 
         except KeyboardInterrupt:
             print("Canceled by user.")
         finally:
             c.close()
 
     def _decode(self, message: bytes) -> List[Dict[str, Any]]:
@@ -240,26 +174,30 @@
         stringio.seek(0)
 
         records = []
         for record in fa.reader(stringio):
             records.append(record)
         return records
 
-    def _write_candidate(self, candidate: Dict[str, Any]) -> None:
+    def _write_candidate(self, alert: Dict[str, Any]) -> None:
         """Write the candidate data to a JSON file.
 
         Args:
             candidate (Dict[str, Any]): The candidate dictionary to be written to the JSON file.
         """
+        alert["candidate"]["stamp_bytes"] = base64.b64encode(
+            alert["candidate"]["stamp_bytes"]
+        ).decode("utf-8")
         with open(
-            os.path.join(self.output_path, f"{candidate['objectId']}.json"), "w"
+            os.path.join(self.output_path, f"{alert['objectId']}.json"), "wb"
         ) as f:
-            f.write(orjson.dumps(candidate))
+            f.write(orjson.dumps(alert))
+        self.log.info(f'New candidate: {alert["objectId"]}.json')
 
-    def _filter_candidates(self, candidates: List[Dict[str, Any]]) -> None:
+    def _filter_to_disk(self, alerts: List[Dict[str, Any]]) -> None:
         """Filter the candidates based on the specified filter conditions.
 
         Args:
             candidates (List[Dict[str, Any]]): The list of candidate dictionaries to be filtered.
 
         Note:
             If the 'filter_path' is provided, the candidates will be filtered based on the conditions
@@ -267,17 +205,17 @@
             all candidates will be written to the output.
         """
         if self.filter_path is not None:
             with open(self.filter_path, "r") as file:
                 filter_conditions = file.read().splitlines()
             filter_conditions = [f for f in filter_conditions if len(f) > 3]
 
-        for candidate in candidates:
-            if len(candidate["xmatch"]) > 0 and self.filter_path is not None:
-                xmatch = pd.DataFrame.from_records(candidate["xmatch"])
+        for alert in alerts:
+            if len(alert["xmatch"]) > 0 and self.filter_path is not None:
+                xmatch = pd.DataFrame.from_records(alert["xmatch"])
                 for condition in filter_conditions:
                     column_name, operator, value = condition.split()
                     xmatch = xmatch.query(f"{column_name} {operator} {value}")
                 if len(xmatch) > 0:
-                    self._write_candidate(candidate)
+                    self._write_candidate(alert)
             else:
-                self._write_candidate(candidate)
+                self._write_candidate(alert)
```

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/vetnet.py` & `argus_rico-0.2.0/src/argus_rico/efte/vetnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 __all__ = ["VetNet"]
 """Wrapper for the MC EFTE Vetnet model."""
 import os
 from typing import Tuple
 
-import astropy.visualization as viz
-import numpy as np
-import tensorflow as tf
-import tensorflow.keras.models as models
+os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
 
-from .. import s3
+import astropy.visualization as viz  # noqa: E402
+import numpy as np  # noqa: E402
+import tensorflow as tf  # noqa: E402
+import tensorflow.keras.models as models  # noqa: E402
+
+from .. import s3  # noqa: E402
 
 
 class VetNet:
     def __init__(self) -> None:
         """Initialize the Vetnet class.
 
         Loads the pretrained model and sets class variables.
```

### Comparing `argus_rico-0.1.0/src/argus_rico/efte/watchdog.py` & `argus_rico-0.2.0/src/argus_rico/efte/watchdog.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import ray
 from watchdog.events import FileSystemEvent, FileSystemEventHandler
 from watchdog.observers.polling import PollingObserver
 
 from .. import get_logger
 from .processor import EFTECatalogProcessor
 
-log = get_logger(__name__)
-
 
 class EFTEWatcher:
     def __init__(self, watch_path: str) -> None:
         """Initialize the EFTEWatcher class.
 
         Args:
             watch_path (str): The path to the directory to watch for catalog files.
@@ -41,25 +39,27 @@
         observer.join()
 
 
 class EFTECatalogHandler(FileSystemEventHandler):
     def __init__(self):
         """Initialize the EFTECatalogHandler class."""
         self.efte_processors = defaultdict(EFTECatalogProcessor.remote)
+        self.log = get_logger(__name__)
 
     def on_created(self, event: FileSystemEvent) -> None:
         """Process the newly created catalog file.
 
         Args:
             event (FileSystemEvent): The event object representing the file creation.
 
         Returns:
             None: This method does not return any value; it processes the catalog file.
         """
         filepath = event.src_path
-        print("found: ", event.src_path)
 
         if filepath[-4:] != ".cat":
             return
         camera_id = os.path.basename(filepath)[:9]
 
+        self.log.info(f"New cat for {camera_id}: {filepath}")
+
         self.efte_processors[camera_id].process.remote(filepath)
```

### Comparing `argus_rico-0.1.0/src/argus_rico/heartbeat.py` & `argus_rico-0.2.0/src/argus_rico/heartbeat.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/images.py` & `argus_rico-0.2.0/src/argus_rico/images.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/models/evr_image.py` & `argus_rico-0.2.0/src/argus_rico/models/evr_image.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/producer.py` & `argus_rico-0.2.0/src/argus_rico/producer.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/s3.py` & `argus_rico-0.2.0/src/argus_rico/s3.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.1.0/src/argus_rico/slack.py` & `argus_rico-0.2.0/src/argus_rico/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from slack_bolt import App
 
 from . import config, efte_runner, get_logger
 from . import images as rimages
 
 log = get_logger("slack_bot")
 
-slack_app = App(
-    token=config.SLACK_BOT_TOKEN,
-    signing_secret=config.SLACK_SIGNING_SECRET,
-)
+if config.SLACK_BOT_TOKEN is not None:
+    slack_app = App(
+        token=config.SLACK_BOT_TOKEN,
+        signing_secret=config.SLACK_SIGNING_SECRET,
+    )
 
 
 @slack_app.event("message")
 def handle_message_events(body: Dict[str, Any]) -> None:
     """Handle message events in the Slack app.
 
     Args:
```

### Comparing `argus_rico-0.1.0/PKG-INFO` & `argus_rico-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argus-rico
-Version: 0.1.0
+Version: 0.2.0
 Summary: Transient alert generation and database interaction for Argus and Evryscope
 Author: Hank Corbett
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: astropy (>=5.3,<6.0)
```

