# Comparing `tmp/surge_api-1.1.2-py3-none-any.whl.zip` & `tmp/surge_api-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 17563 bytes, number of entries: 16
--rw-r--r--  2.0 unx      186 b- defN 23-Jun-19 05:11 surge/__init__.py
--rw-r--r--  2.0 unx     2905 b- defN 23-Jun-21 06:40 surge/api_resource.py
--rw-r--r--  2.0 unx      734 b- defN 23-Jun-19 05:11 surge/carousel.py
--rw-r--r--  2.0 unx     1606 b- defN 23-Jun-19 05:11 surge/errors.py
--rw-r--r--  2.0 unx    12142 b- defN 23-Jun-21 06:22 surge/projects.py
--rw-r--r--  2.0 unx    26952 b- defN 23-Jun-19 05:11 surge/questions.py
--rw-r--r--  2.0 unx     5173 b- defN 23-Jun-19 05:11 surge/reports.py
--rw-r--r--  2.0 unx      939 b- defN 23-Jun-19 05:11 surge/responses.py
--rw-r--r--  2.0 unx     5799 b- defN 23-Jun-19 05:11 surge/tasks.py
--rw-r--r--  2.0 unx     4107 b- defN 23-Jun-19 05:11 surge/teams.py
--rw-r--r--  2.0 unx      442 b- defN 23-Jun-19 05:11 surge/utils.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3742 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 23-Jun-21 06:40 surge_api-1.1.2.dist-info/RECORD
-16 files, 67088 bytes uncompressed, 15625 bytes compressed:  76.7%
+Zip file size: 17862 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      186 b- defN 23-Aug-01 23:52 surge/__init__.py
+-rw-r--r--  2.0 unx     2905 b- defN 23-Aug-01 23:52 surge/api_resource.py
+-rw-r--r--  2.0 unx      734 b- defN 23-Aug-01 23:52 surge/carousel.py
+-rw-r--r--  2.0 unx     1606 b- defN 23-Aug-01 23:52 surge/errors.py
+-rw-r--r--  2.0 unx    12142 b- defN 23-Aug-01 23:52 surge/projects.py
+-rw-r--r--  2.0 unx    26952 b- defN 23-Aug-01 23:52 surge/questions.py
+-rw-r--r--  2.0 unx     5283 b- defN 23-Aug-02 00:31 surge/reports.py
+-rw-r--r--  2.0 unx      939 b- defN 23-Aug-01 23:52 surge/responses.py
+-rw-r--r--  2.0 unx     5799 b- defN 23-Aug-01 23:52 surge/tasks.py
+-rw-r--r--  2.0 unx     4107 b- defN 23-Aug-01 23:52 surge/teams.py
+-rw-r--r--  2.0 unx      442 b- defN 23-Aug-01 23:52 surge/utils.py
+-rw-r--r--  2.0 unx     1062 b- defN 23-Aug-02 00:31 surge_api-1.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4406 b- defN 23-Aug-02 00:31 surge_api-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 00:31 surge_api-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Aug-02 00:31 surge_api-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 23-Aug-02 00:31 surge_api-1.1.3.dist-info/RECORD
+16 files, 67862 bytes uncompressed, 15924 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: surge/teams.py
 Comment: 
 
 Filename: surge/utils.py
 Comment: 
 
-Filename: surge_api-1.1.2.dist-info/LICENSE
+Filename: surge_api-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: surge_api-1.1.2.dist-info/METADATA
+Filename: surge_api-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: surge_api-1.1.2.dist-info/WHEEL
+Filename: surge_api-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: surge_api-1.1.2.dist-info/top_level.txt
+Filename: surge_api-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: surge_api-1.1.2.dist-info/RECORD
+Filename: surge_api-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## surge/reports.py

```diff
@@ -1,10 +1,12 @@
 import gzip
 from time import sleep
 import urllib
+import tempfile
+import shutil
 
 from surge.errors import SurgeMissingIDError, SurgeMissingAttributeError
 from surge.api_resource import REPORTS_ENDPOINT, APIResource
 
 
 class Report(APIResource):
 
@@ -43,20 +45,21 @@
         for _ in range(poll_time // 2):
             response = cls.request(project_id=project_id, type=type)
             # Download zipped project results if ready
             if response.status == "READY":
                 file_ext = "csv" if "csv" in type else "json"
                 default_file_name = "project_{project_id}_results.{file_ext}.gzip".format(
                     project_id=project_id, file_ext=file_ext)
-                downloaded_file, http_message = urllib.request.urlretrieve(
-                    response.url, default_file_name)
-                # Unzip and save results
-                data = gzip.open(downloaded_file, "r").read()
-                open(filepath or default_file_name.rstrip('.gzip'),
-                     "wb").write(data)
+                with urllib.request.urlopen(response.url) as response:
+                  with tempfile.NamedTemporaryFile() as tmp_file:
+                    shutil.copyfileobj(response, tmp_file)
+                    # Unzip and save results
+                    data = gzip.open(tmp_file.name, "r").read()
+                    open(filepath or default_file_name.rstrip('.gzip'),
+                        "wb").write(data)
                 return None
 
             # Wait two seconds before polling again
             elif response.status == 'CREATING':
                 sleep(2)
                 continue
             else:
```

## Comparing `surge_api-1.1.2.dist-info/LICENSE` & `surge_api-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `surge_api-1.1.2.dist-info/METADATA` & `surge_api-1.1.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surge-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Surge Python SDK
 Home-page: https://github.com/surge-ai/surge-python
 Author: Surge
 Author-email: team@surgehq.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -59,16 +59,38 @@
 
 # Retrieve a specific Project
 project = surge.Project.retrieve("076d207b-c207-41ca-b73a-5822fe2248ab")
 
 # print the number of tasks in that Project
 print(project.num_tasks)
 ```
+If you have an existing project, you can use it as a template to get a new batch of data annotated.
+You can add new labeling tasks from a CSV or with a list of dictionaries.
 
-When creating a new Project, you can create a list of Questions and include them in the new Project.
+```python
+# Create a project from a template
+template_project_id = "076d207b-c207-41ca-b73a-5822fe2248ab"
+project = surge.Project.create("My Labeling Project (July 2023 Batch)", template_id=template_project_id)
+
+# Add data from a CSV file
+project.create_tasks_from_csv('my_data.csv')
+
+# Or add data directly
+tasks = project.create_tasks([{
+    "company": "Surge",
+    "city": "San Francisco",
+    "state": "CA"
+}])
+
+# Launch the project to send it to the Surge workforce
+project.launch()
+```
+
+
+Or you can create a new project from scratch by creating your own template and list of Question:
 
 ```python
 from surge.questions import FreeResponseQuestion, MultipleChoiceQuestion, CheckboxQuestion
 
 # Create a new Project
 free_response_q = FreeResponseQuestion(
     text="What is this company's website?")
```

