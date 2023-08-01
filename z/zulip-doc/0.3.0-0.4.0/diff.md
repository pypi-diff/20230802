# Comparing `tmp/zulip_doc-0.3.0.tar.gz` & `tmp/zulip_doc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zulip_doc-0.3.0.tar", last modified: Tue Aug  1 22:12:27 2023, max compression
+gzip compressed data, was "zulip_doc-0.4.0.tar", last modified: Tue Aug  1 22:34:31 2023, max compression
```

## Comparing `zulip_doc-0.3.0.tar` & `zulip_doc-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-08-01 15:22:12.948824 zulip_doc-0.3.0/LICENSE
--rw-r--r--   0        0        0      783 2023-08-01 21:34:35.557954 zulip_doc-0.3.0/README.md
--rw-r--r--   0        0        0      725 2023-08-01 22:12:27.661685 zulip_doc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 18:53:34.217481 zulip_doc-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       22 2023-08-01 21:43:53.942038 zulip_doc-0.3.0/zdoc/__init__.py
--rwxr-xr-x   0        0        0     1911 2023-08-01 22:10:56.606943 zulip_doc-0.3.0/zdoc/main.py
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 zulip_doc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-01 15:22:12.948824 zulip_doc-0.4.0/LICENSE
+-rw-r--r--   0        0        0      949 2023-08-01 22:32:26.913713 zulip_doc-0.4.0/README.md
+-rw-r--r--   0        0        0      796 2023-08-01 22:34:31.280029 zulip_doc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 18:53:34.217481 zulip_doc-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-01 22:32:45.573460 zulip_doc-0.4.0/zdoc/__init__.py
+-rwxr-xr-x   0        0        0     1911 2023-08-01 22:10:56.606943 zulip_doc-0.4.0/zdoc/main.py
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 zulip_doc-0.4.0/PKG-INFO
```

### Comparing `zulip_doc-0.3.0/LICENSE` & `zulip_doc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zulip_doc-0.3.0/README.md` & `zulip_doc-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,7 +21,18 @@
                                   weekends]
   --config-file FILE              [env var: CONFIG_FILE; default:
                                   /home/{username}/.zuliprc]
   --help                          Show this message and exit.
 ```
 
 Example: `zdoc 12 22`
+
+
+## Cron Job Setup
+
+`crontab -e`
+
+Then add something like:
+
+`0 12 * * * /home/paul/.local/bin/zdoc --config-file /home/paul/.zuliprc 12 22`
+
+*runs everyday at noon*
```

### Comparing `zulip_doc-0.3.0/pyproject.toml` & `zulip_doc-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 dependencies = [
     "zulip>=0.8.2",
     "typer>=0.9.0",
     "humanize>=4.7.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.0"
+version = "0.4.0"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 zdoc = "zdoc.main:app"
 
+[project.urls]
+homepage = "https://github.com/pizzapanther/zulip-doc"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.version]
```

### Comparing `zulip_doc-0.3.0/zdoc/main.py` & `zulip_doc-0.4.0/zdoc/main.py`

 * *Files identical despite different names*

### Comparing `zulip_doc-0.3.0/PKG-INFO` & `zulip_doc-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: zulip-doc
-Version: 0.3.0
+Version: 0.4.0
 Summary: Zulip service that checks user presence for Duty of Care responsibilities for remote teams
+Home-page: https://github.com/pizzapanther/zulip-doc
 Author-Email: Paul Bailey <paul@neutron.studio>
 License: MIT
+Project-URL: Homepage, https://github.com/pizzapanther/zulip-doc
 Requires-Python: >=3.8
 Requires-Dist: zulip>=0.8.2
 Requires-Dist: typer>=0.9.0
 Requires-Dist: humanize>=4.7.0
 Description-Content-Type: text/markdown
 
 # Zulip Duty of Care Service
@@ -33,7 +35,18 @@
                                   weekends]
   --config-file FILE              [env var: CONFIG_FILE; default:
                                   /home/{username}/.zuliprc]
   --help                          Show this message and exit.
 ```
 
 Example: `zdoc 12 22`
+
+
+## Cron Job Setup
+
+`crontab -e`
+
+Then add something like:
+
+`0 12 * * * /home/paul/.local/bin/zdoc --config-file /home/paul/.zuliprc 12 22`
+
+*runs everyday at noon*
```

