# Comparing `tmp/edwh_files_plugin-0.1.0.tar.gz` & `tmp/edwh_files_plugin-0.1.1.tar.gz`

## Comparing `edwh_files_plugin-0.1.0.tar` & `edwh_files_plugin-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/src/edwh_files_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/src/edwh_files_plugin/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/src/edwh_files_plugin/files_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/src/edwh_files_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/src/edwh_files_plugin/__init__.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/src/edwh_files_plugin/files_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 edwh_files_plugin-0.1.1/PKG-INFO
```

### Comparing `edwh_files_plugin-0.1.0/src/edwh_files_plugin/files_plugin.py` & `edwh_files_plugin-0.1.1/src/edwh_files_plugin/files_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import io
+import json
+import sys
 
 import httpx
 from invoke import task
 from rich import print, progress
 
 DEFAULT_TRANSFERSH_SERVER = "https://files.edwh.nl"
 
 
 def require_protocol(url: str):
-    if not url.startswith("http"):
-        return f"https://{url}"
-    return url
+    return url if url.startswith(("http://", "https://")) else f"https://{url}"
 
 
-@task(aliases=("add",))
+@task(aliases=("add", "send"))
 def upload(_, filename, server=DEFAULT_TRANSFERSH_SERVER, max_downloads=None, max_days=None, encrypt=None):
     """
     Upload a file.
 
     Args:
         filename (str): path to the file to upload
         server (str): which transfer.sh server to use
@@ -37,29 +37,38 @@
     with httpx.Client() as session, open(filename, "rb") as f:
         file = {filename: f}
 
         url = require_protocol(server)
 
         response = session.post(url, files=file, headers=headers)
 
+        download_url = response.text.strip()
+        delete_url = response.headers.get('x-url-delete')
+
         print(
-            {
-                "status": response.status_code,
-                "url": response.text.strip(),
-                "delete": response.headers.get('x-url-delete'),
-            }
+            json.dumps(
+                {
+                    "status": response.status_code,
+                    "url": download_url,
+                    "delete": delete_url,
+                    "download_command": f"edwh file.download {download_url}",
+                    "delete_command": f"edwh file.delete {delete_url}",
+                },
+                indent=2,
+            ),
         )
 
 
-@task(aliases=("get",))
+@task(aliases=("get", "receive"))
 def download(_, download_url, output_file=None, decrypt=None):
     """
     Download a file.
 
     Args:
+        _ (Context)
         download_url (str): file to download
         output_file (str): path to store the file in
         decrypt (str): decryption token
     """
     if output_file is None:
         output_file = download_url.split("/")[-1]
 
@@ -67,15 +76,15 @@
 
     headers = {}
     if decrypt:
         headers["X-Decrypt-Password"] = decrypt
 
     with httpx.Client() as session, session.stream("GET", download_url, headers=headers) as response:
         if response.status_code >= 400:
-            print("[red] Something went wrong: [/red]", response.status_code, response.read().decode())
+            print("[red] Something went wrong: [/red]", response.status_code, response.read().decode(), file=sys.stderr)
             return
 
         total = int(response.headers["Content-Length"])
         with (
             open(output_file, "wb") as f,  # <- open file when we're sure the status code is successful!
             progress.Progress(
                 "[progress.percentage]{task.percentage:>3.0f}%",
@@ -92,14 +101,15 @@
 
 @task(aliases=("remove",))
 def delete(_, deletion_url):
     """
     Delete an uploaded file.
 
     Args:
+        _ (Context)
         deletion_url (str): File url + deletion token (from `x-url-delete`, shown in file.upload output)
     """
     deletion_url = require_protocol(deletion_url)
 
     with httpx.Client() as session:
         response = session.delete(deletion_url)
```

### Comparing `edwh_files_plugin-0.1.0/LICENSE.txt` & `edwh_files_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_files_plugin-0.1.0/README.md` & `edwh_files_plugin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_files_plugin-0.1.0/pyproject.toml` & `edwh_files_plugin-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_files_plugin-0.1.0/PKG-INFO` & `edwh_files_plugin-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-files-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: `edwh` plugin for files.edwh.nl
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-files-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-files-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-files-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

