# Comparing `tmp/dheeobs-0.1.1.tar.gz` & `tmp/dheeobs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dheeobs-0.1.1.tar", last modified: Tue Jul 11 16:46:57 2023, max compression
+gzip compressed data, was "dheeobs-0.1.2.tar", last modified: Tue Aug  1 22:15:07 2023, max compression
```

## Comparing `dheeobs-0.1.1.tar` & `dheeobs-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:46:57.045670 dheeobs-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-11 16:46:57.045670 dheeobs-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-02 15:28:40.000000 dheeobs-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:46:57.044670 dheeobs-0.1.1/dheeobs/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-11 16:46:04.000000 dheeobs-0.1.1/dheeobs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-11 16:46:04.000000 dheeobs-0.1.1/dheeobs/dhee_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4129 2023-07-11 16:46:04.000000 dheeobs-0.1.1/dheeobs/dhee_loghandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:46:57.045670 dheeobs-0.1.1/dheeobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-11 16:46:56.000000 dheeobs-0.1.1/dheeobs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 16:46:57.045670 dheeobs-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-11 16:45:10.000000 dheeobs-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 22:15:07.092632 dheeobs-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-08-01 22:15:07.092632 dheeobs-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-02 15:28:40.000000 dheeobs-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 22:15:07.092632 dheeobs-0.1.2/dheeobs/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-08-01 22:14:28.000000 dheeobs-0.1.2/dheeobs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-08-01 22:14:28.000000 dheeobs-0.1.2/dheeobs/dhee_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     5152 2023-08-01 22:14:28.000000 dheeobs-0.1.2/dheeobs/dhee_loghandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 22:15:07.092632 dheeobs-0.1.2/dheeobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-08-01 22:15:07.000000 dheeobs-0.1.2/dheeobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-01 22:15:07.000000 dheeobs-0.1.2/dheeobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 22:15:07.000000 dheeobs-0.1.2/dheeobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-01 22:15:07.000000 dheeobs-0.1.2/dheeobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-01 22:15:07.000000 dheeobs-0.1.2/dheeobs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 22:15:07.092632 dheeobs-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-08-01 22:14:28.000000 dheeobs-0.1.2/setup.py
```

### Comparing `dheeobs-0.1.1/dheeobs/dhee_loghandler.py` & `dheeobs-0.1.2/dheeobs/dhee_loghandler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import json
 from datetime import datetime, timezone
 import logging
 import requests
 import os
 import sys
 
 
 class DheeLogHandler(logging.Handler):
 
     def __init__(self, **logparams) -> None:
         super().__init__()
         self.log_integration_list = logparams.get('log_integration_list')
         if logparams.get('glueContext') is not None:
             self.glueContext = logparams.get('glueContext')
+        self.run_parameters = {}
 
     def emit(self, record: logging.LogRecord) -> None:
         """
         Inherited Method invoked for all log levels
         :param record: logging record object
         :return:
         """
@@ -38,39 +40,51 @@
         :return:
         """
         message = self.format(record)
         level = record.levelname
         log_location = record.filename + "::" + record.funcName + "::" + str(
             record.lineno)  # Eg., dhee_loghandler.py::post_logs_to_influxdb::45
 
-        if hasattr(self, 'glueContext') and self.glueContext is not None:
-            args = self.get_commandline_args()
-        else:
-            args = {'INFLUXDB_URL': os.getenv('INFLUXDB_URL'), 'INFLUXDB_ORG': os.getenv('INFLUXDB_ORG'),
-                    'INFLUXDB_BUCKET': os.getenv('INFLUXDB_BUCKET'), 'INFLUXDB_TOKEN': os.getenv('INFLUXDB_TOKEN'),
-                    'MEASUREMENT_NAME': os.getenv('MEASUREMENT_NAME'), 'PIPELINE_ID': os.getenv('PIPELINE_ID'),
-                    'JOB_RUN_ID': os.getenv('JOB_RUN_ID')}
-
-        timestamp = int(datetime.now(timezone.utc).timestamp() * 1000000000)
-        url = args['INFLUXDB_URL'] + "/api/v2/write?org=" + args['INFLUXDB_ORG'] + "&bucket=" + args[
-            'INFLUXDB_BUCKET'] + "&precision=ns"
+        url = f'{self.run_parameters.get("DHEE_URL")}/log'
         headers = {
-            'Authorization': 'Token ' + args['INFLUXDB_TOKEN'],
-            'Content-Type': 'text/plain; charset=utf-8'
+            'Authorization': 'Bearer '+self.run_parameters.get("DHEE_TOKEN"),
+            'Content-Type': 'application/json'
         }
 
-        if 'PIPELINE_ID' not in args:
-            payload = args['MEASUREMENT_NAME'] + ",level=" + level + " message=\"" + message + "\",location=\"" + log_location +"\" " + str(timestamp)
+
+        if 'CONNECTION_FILE' not in self.run_parameters:
+            payload = {
+                "measurement": self.run_parameters.get("POD_ID"),
+                "bucket": self.run_parameters.get("INFLUXDB_BUCKET"),
+                "tags": [
+                    {"key": "level", "value": level},
+                ],
+                "fields": [
+                    {"key": "message", "value": message},
+                    {"key": "location", "value": log_location},
+                ]
+            }
         else:
             content = message.split("#")
-            payload = args['MEASUREMENT_NAME'] + ",pipelineId=" + args['PIPELINE_ID'] + ",job_run_id=\"" + args[
-                      'JOB_RUN_ID'] + "\",expectation_type=\"" + content[
-                      0] + "\",column_name=\"" + content[1] + "\",validation_status=\"" + content[2] + "\" values=\"" + content[
-                      3] + "\" " + str(timestamp)
-        response = requests.request("POST", url, headers=headers, data=payload)
+            payload = {
+                "measurement": self.run_parameters.get("POD_ID"),
+                "bucket": self.run_parameters.get("INFLUXDB_BUCKET"),
+                "tags": [
+                    {"key": "pipelineId", "value": self.run_parameters.get("PIPELINE_ID")},
+                    {"key": "job_run_id", "value": self.run_parameters.get("JOB_RUN_ID")},
+                    {"key": "expectation_type", "value": content[0]},
+                    {"key": "column_name", "value": content[1]},
+                    {"key": "validation_status", "value": content[2]},
+                ],
+                "fields":[
+                    {"key": "values", "value": content[3]}
+                ]
+            }
+        print(payload)
+        response = requests.request("POST", url, headers=headers, json=payload)
         response.raise_for_status()
 
     def post_logs_to_cloudwatch(self, record: logging.LogRecord):
         """
         Post Logs to Cloudwatch from AWS Glue Job
         :param record: logging record object
         :return:
@@ -93,7 +107,32 @@
         :return:
         """
         arguments_dict = {}
         for index, argument in enumerate(sys.argv):
             if argument.startswith("--"):
                 arguments_dict[argument[2:]] = sys.argv[index + 1]
         return arguments_dict
+
+    def get_run_parameters(self):
+        if hasattr(self, 'glueContext') and self.glueContext is not None:
+            args = self.get_commandline_args()
+        else:
+            args = {'DHEE_URL': os.getenv('DHEE_URL'), 'DHEE_TOKEN': os.getenv('DHEE_TOKEN'), 'POD_ID': os.getenv('POD_ID'),
+                    'JOB_RUN_ID': os.getenv('JOB_RUN_ID')}
+
+        dhee_url = args['DHEE_URL']
+        podId = args['POD_ID']
+        dhee_token = args['DHEE_TOKEN']
+
+        url = f'{dhee_url}/pod/{podId}/runparameters'
+        headers = {
+            'Authorization': 'Bearer ' + dhee_token,
+            'Content-Type': 'application/json'
+        }
+        response = requests.request('GET', url, headers=headers)
+        if response is not None:
+            paramJSON = json.loads(json.dumps(response.json()))
+            for param in paramJSON:
+                self.run_parameters.update({param: paramJSON[param]})
+
+        self.run_parameters.update(args)
+        return self.run_parameters
```

