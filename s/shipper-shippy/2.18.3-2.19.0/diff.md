# Comparing `tmp/shipper-shippy-2.18.3.tar.gz` & `tmp/shipper-shippy-2.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-2.18.3.tar", last modified: Wed Aug  2 00:05:42 2023, max compression
+gzip compressed data, was "shipper-shippy-2.19.0.tar", last modified: Wed Aug  2 04:59:27 2023, max compression
```

## Comparing `shipper-shippy-2.18.3.tar` & `shipper-shippy-2.19.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/shippy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/shippy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/version.py
```

### Comparing `shipper-shippy-2.18.3/PKG-INFO` & `shipper-shippy-2.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.18.3
+Version: 2.19.0
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.18.3/README.md` & `shipper-shippy-2.19.0/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.3/setup.py` & `shipper-shippy-2.19.0/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.3/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-2.19.0/shipper_shippy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.18.3
+Version: 2.19.0
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.18.3/shippy/__main__.py` & `shipper-shippy-2.19.0/shippy/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,41 +56,14 @@
 
 
 def lower_logger_level():
     logger.remove()
     logger.add(sys.stderr, level="INFO")
 
 
-def main():
-    # Get commandline arguments
-    args = init_argparse()
-
-    lower_logger_level()
-
-    if args.version:
-        print(__version__)
-        return
-
-    if args.debug:
-        print_warning("Debug mode has been turned on!")
-        logger.add(sink="shippy_{time}.log", level="DEBUG", enqueue=True)
-
-    print(f"Welcome to shippy (v.{__version__})!")
-
-    # Check for updates
-    check_shippy_update()
-
-    # Initialize client
-    client = build_client_from_config()
-    server_prechecks(client)
-
-    # Start uploads
-    search_and_upload_builds(client, args)
-
-
 def server_prechecks(client):
     check_server_compat(client)
     check_token_validity(client)
 
 
 def check_and_upload_build(client, args, build_path):
     # Check build file validity
@@ -98,18 +71,18 @@
         print_warning("Invalid build. Skipping...")
         return
 
     if is_upload_without_prompt_enabled(args) or input_yn(
         f"Uploading build {build_path}. Start?"
     ):
         try:
-            upload_id = client.upload(build_path=build_path)
+            uploaded_build_id = client.upload(build_path=build_path)
 
             if is_build_disabling_enabled():
-                client.disable_build(upload_id=upload_id)
+                client.disable_build(build_id=uploaded_build_id)
         except UploadException as exception:
             print_error(exception, newline=True, exit_after=False)
 
 
 def search_and_upload_builds(client, args):
     # Search current directory for files with regex pattern returned by server
     build_paths = get_builds_in_current_dir(client.get_regex_pattern())
@@ -396,9 +369,36 @@
 def is_build_disabling_enabled():
     try:
         return get_config_value("shippy", "DisableBuildOnUpload") == "true"
     except KeyError:
         return False
 
 
+def main():
+    # Get commandline arguments
+    args = init_argparse()
+
+    lower_logger_level()
+
+    if args.version:
+        print(__version__)
+        return
+
+    if args.debug:
+        print_warning("Debug mode has been turned on!")
+        logger.add(sink="shippy_{time}.log", level="DEBUG", enqueue=True)
+
+    print(f"Welcome to shippy (v.{__version__})!")
+
+    # Check for updates
+    check_shippy_update()
+
+    # Initialize client
+    client = build_client_from_config()
+    server_prechecks(client)
+
+    # Start uploads
+    search_and_upload_builds(client, args)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `shipper-shippy-2.18.3/shippy/client.py` & `shipper-shippy-2.19.0/shippy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,22 @@
         r_content = r.json()
     except ValueError:
         r_content = r.content
 
     logger.debug(f"Received response: {r_content}")
 
 
+def wait_rate_limit(seconds):
+    with console.status(RATE_LIMIT_WAIT_STATUS_MSG.format(seconds)) as status:
+        while seconds:
+            time.sleep(1)
+            seconds -= 1
+            status.update(status=RATE_LIMIT_WAIT_STATUS_MSG.format(seconds))
+
+
 class Client:
     def __init__(self, server_url, token=None):
         self.server_url = server_url
         self.token = token
 
     def is_url_secure(self):
         return self.server_url[0:5] == "https"
@@ -227,25 +235,25 @@
 
                 upload_exception_check(r, build_path)
         except UploadException as e:
             raise e
         except requests.exceptions.RequestException:
             raise UploadException(UNKNOWN_UPLOAD_ERROR_MSG)
 
-        return upload_id
+        return r.json()["build_id"]
 
-    def disable_build(self, upload_id):
+    def disable_build(self, build_id):
         r = self._post(
             "/api/v1/maintainers/build/enabled_status_modify/",
             headers=self._get_header(),
-            data={"build_id": upload_id, "enable": False},
+            data={"build_id": build_id, "enable": False},
         )
 
         if r.status_code == 200:
-            print(f"Build {upload_id} has been disabled.")
+            print(f"Build {build_id} has been disabled.")
         else:
             raise Exception("There was a problem disabling the build.")
 
     def _upload_chunk(self, build_path, chunk, current, total, upload_id):
         if upload_id:
             url = f"/api/v1/maintainers/chunked_upload/{upload_id}/"
         else:
@@ -307,29 +315,22 @@
             case _:
                 return
         log_debug_request_response(r)
 
         # Check for rate limit
         if r.status_code == 429:
             print(RATE_LIMIT_MSG)
-            self._wait_rate_limit(int(re.findall(r"\d+", r.json()["detail"])[0]))
+            wait_rate_limit(int(re.findall(r"\d+", r.json()["detail"])[0]))
 
             return self._request(
                 type=type, url=url, headers=headers, data=data, files=files
             )
 
         return r
 
-    def _wait_rate_limit(seconds):
-        with console.status(RATE_LIMIT_WAIT_STATUS_MSG.format(seconds)) as status:
-            while seconds:
-                time.sleep(1)
-                seconds -= 1
-                status.update(status=RATE_LIMIT_WAIT_STATUS_MSG.format(seconds))
-
     def _post(self, url, headers=None, data=None):
         return self._request("POST", url, headers, data)
 
     def _get(self, url, headers=None, data=None):
         return self._request("GET", url, headers, data)
 
     def _put(self, url, headers, data, files):
```

### Comparing `shipper-shippy-2.18.3/shippy/config.py` & `shipper-shippy-2.19.0/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.3/shippy/constants.py` & `shipper-shippy-2.19.0/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.3/shippy/helper.py` & `shipper-shippy-2.19.0/shippy/helper.py`

 * *Files identical despite different names*

