# Comparing `tmp/tum_esm_em27_metadata-2.0.0rc3.tar.gz` & `tmp/tum_esm_em27_metadata-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc3.tar", max compression
+gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc4.tar", max compression
```

## Comparing `tum_esm_em27_metadata-2.0.0rc3.tar` & `tum_esm_em27_metadata-2.0.0rc4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     2826 2023-04-23 11:30:01.572048 tum_esm_em27_metadata-2.0.0rc3/README.md
--rw-r--r--   0        0        0     1061 2023-04-24 18:57:54.884363 tum_esm_em27_metadata-2.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/__init__.py
--rw-r--r--   0        0        0     6459 2023-04-24 18:57:22.893799 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/interfaces.py
--rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/loader.py
--rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/py.typed
--rw-r--r--   0        0        0     4033 2023-04-24 18:50:37.062912 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/types.py
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc3/setup.py
--rw-r--r--   0        0        0     3500 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     3990 2023-08-02 12:33:06.624704 tum_esm_em27_metadata-2.0.0rc4/README.md
+-rw-r--r--   0        0        0     1137 2023-08-02 12:25:22.653875 tum_esm_em27_metadata-2.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/__init__.py
+-rw-r--r--   0        0        0    13975 2023-08-02 12:25:22.654638 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/interfaces.py
+-rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/loader.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/py.typed
+-rw-r--r--   0        0        0     5517 2023-08-02 12:25:22.654845 tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/types.py
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc4/PKG-INFO
```

### Comparing `tum_esm_em27_metadata-2.0.0rc3/README.md` & `tum_esm_em27_metadata-2.0.0rc4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ```bash
 poetry add tum-esm-em27-metadata
 # or
 pip install tum-esm-em27-metadata
 ```
 
 ```python
+import pendulum
 import tum_esm_em27_metadata
 
 em27_metadata = tum_esm_em27_metadata.load_from_github(
     github_repository="org-name/repo-name",
     access_token="your-github-access-token",
 )
 
@@ -40,44 +41,57 @@
 em27_metadata = tum_esm_em27_metadata.load_from_local_files(
     locations_path="location-data/locations.json",
     sensors_path="location-data/sensors.json",
     campaigns_path="location-data/campaigns.json",
 )
 
 metadata = em27_metadata.get(
-    sensor_id = "ma", date = "20220601"
+    sensor_id = "ma",
+    from_datetime = pendulum.DateTime(
+        year=2022, month=6, day=1, hour=0, minute=0, second=0
+    ),
+    to_datetime = pendulum.DateTime(
+        year=2022, month=6, day=1, hour=23, minute=59, second=59
+    ),
 )
 
-print(metadata.dict())
+print(metadata)
+
 ```
 
 Prints out:
 
 ```json
-{
-    "sensor_id": "ma",
-    "serial_number": 61,
-    "utc_offset": 0,
-    "pressure_data_source": "ma",
-    "pressure_calibration_factor": 1,
-    "output_calibration_factor": 1,
-    "date": "20220601",
-    "location": {
-        "location_id": "TUM_I",
-        "details": "TUM Dach Innenstadt",
-        "lon": 11.569,
-        "lat": 48.151,
-        "alt": 539
+[
+    {
+        "sensor_id": "ma",
+        "serial_number": 61,
+        "from_datetime": "2022-06-01T00:00:00+00:00",
+        "to_datetime": "2022-06-01T23:59:59+00:00",
+        "location": {
+            "location_id": "TUM_I",
+            "details": "TUM Dach Innenstadt",
+            "lon": 11.569,
+            "lat": 48.151,
+            "alt": 539
+        },
+        "utc_offset": 0,
+        "pressure_data_source": "ma",
+        "pressure_calibration_factor": 1,
+        "output_calibration_factors_xco2": 1,
+        "output_calibration_factors_xch4": 1,
+        "output_calibration_factors_xco": 1,
+        "output_calibration_scheme": null
     }
-}
+]
 ```
 
-The object returned by `em27_metadata.get()` is of type `tum_esm_em27_metadata.types.SensorDataContext`. It is a Pydantic model (https://docs.pydantic.dev/) but can be converted to a dictionary using `metadata.dict()`.
+The object returned by `em27_metadata.get()` is of type `lis[tum_esm_em27_metadata.types.SensorDataContext]`. It is a Pydantic model (https://docs.pydantic.dev/) but can be converted to a dictionary using `metadata.model_dump()`.
 
-You can find dummy data in the `data/` folder.
+The list will contain one item per time period where the metadata properties are continuous (same location, etc.). You can find dummy data in the `data/` folder.
 
 <br/>
 
 ## Set up an EM27 Metadata Storage Directory
 
 You can use the repository https://github.com/tum-esm/em27-metadata-storage-template to create your own repository for storing the metadata. It contains a GitHub Actions workflow that automatically validates the metadata on every commit in any branch.
 
@@ -100,7 +114,13 @@
 
 Publish the Package to PyPI:
 
 ```bash
 poetry build
 poetry publish
 ```
+
+In order to test the "get metadata for a time period" function, the following example is used:
+
+![](./data/example.png)
+
+The test `tests/test_data_integrity.py` requests the time period `00:00` to `23:59`. The UTC offsets are specified (to be non-zero) from `02:00` to `15:59`, where it has one non-zero value, and from `16:00` to `21:59`, where it has another non-zero value. Each property has two (non-default) values over the day. There should be eight resulting chunks of metadata. All properties of each chunk are validated in the test.
```

### Comparing `tum_esm_em27_metadata-2.0.0rc3/pyproject.toml` & `tum_esm_em27_metadata-2.0.0rc4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "tum_esm_em27_metadata"
-version = "2.0.0-rc.3"
+version = "2.0.0-rc.4"
 description = "Single source of truth for ESM's EM27 measurement logistics"
 readme = "README.md"
 authors = [
     "Moritz Makowski <moritz.makowski@tum.de>",
     "Marlon Mueller <marlon.mueller@tum.de>"
 ]
 packages = [
     {include = "tum_esm_em27_metadata"},
     {include = "tum_esm_em27_metadata/py.typed"},
 ]
 repository = "https://github.com/tum-esm/em27-metadata"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10.7"
 tum-esm-utils = "^1.4.0"
+pendulum = "^2.1.2"
+pydantic = "^2.1.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^22.12.0"
@@ -35,13 +36,18 @@
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 no_warn_unused_ignores = true
 plugins = ["pydantic.mypy"]
 
+
+[[tool.mypy.overrides]]
+module = ["pendulum"]
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 markers = [
-    "ci: can be run in GitHub CI",
-    "action: can be run when using this repo as a GitHub Action",
-    "local: can be run locally"
+    "ci: run in GitHub CI",
+    "action: run when using this repo as a GitHub Action",
+    "local: run locally"
 ]
```

### Comparing `tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/loader.py` & `tum_esm_em27_metadata-2.0.0rc4/tum_esm_em27_metadata/loader.py`

 * *Files identical despite different names*

