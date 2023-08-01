# Comparing `tmp/zulip_doc-0.2.0.tar.gz` & `tmp/zulip_doc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zulip_doc-0.2.0.tar", last modified: Tue Aug  1 21:40:48 2023, max compression
+gzip compressed data, was "zulip_doc-0.3.0.tar", last modified: Tue Aug  1 22:12:27 2023, max compression
```

## Comparing `zulip_doc-0.2.0.tar` & `zulip_doc-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-08-01 15:22:12.948824 zulip_doc-0.2.0/LICENSE
--rw-r--r--   0        0        0      783 2023-08-01 21:34:35.557954 zulip_doc-0.2.0/README.md
--rw-r--r--   0        0        0      697 2023-08-01 21:40:48.472943 zulip_doc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 18:53:34.217481 zulip_doc-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 21:15:31.360705 zulip_doc-0.2.0/zdoc/__init__.py
--rwxr-xr-x   0        0        0     1835 2023-08-01 21:07:05.610539 zulip_doc-0.2.0/zdoc/main.py
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 zulip_doc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-01 15:22:12.948824 zulip_doc-0.3.0/LICENSE
+-rw-r--r--   0        0        0      783 2023-08-01 21:34:35.557954 zulip_doc-0.3.0/README.md
+-rw-r--r--   0        0        0      725 2023-08-01 22:12:27.661685 zulip_doc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 18:53:34.217481 zulip_doc-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-01 21:43:53.942038 zulip_doc-0.3.0/zdoc/__init__.py
+-rwxr-xr-x   0        0        0     1911 2023-08-01 22:10:56.606943 zulip_doc-0.3.0/zdoc/main.py
+-rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 zulip_doc-0.3.0/PKG-INFO
```

### Comparing `zulip_doc-0.2.0/LICENSE` & `zulip_doc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zulip_doc-0.2.0/README.md` & `zulip_doc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zulip_doc-0.2.0/pyproject.toml` & `zulip_doc-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [project]
 name = "zulip-doc"
-version = "0.2.0"
+dynamic = []
 description = "Zulip service that checks user presence for Duty of Care responsibilities for remote teams"
 authors = [
     { name = "Paul Bailey", email = "paul@neutron.studio" },
 ]
 dependencies = [
     "zulip>=0.8.2",
     "typer>=0.9.0",
     "humanize>=4.7.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
+version = "0.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 zdoc = "zdoc.main:app"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.version]
-from = "nsync/__init__.py"
+source = "file"
+path = "zdoc/__init__.py"
 
 [tool.pdm.scripts]
 publish = "pdm publish --username __token__ --password $PDM_PUBLISH_PASSWORD"
 
 [tool.pdm.scripts._]
 env_file = ".env"
```

### Comparing `zulip_doc-0.2.0/zdoc/main.py` & `zulip_doc-0.3.0/zdoc/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,21 @@
   writable=False,
   readable=True,
   resolve_path=True,
   envvar="CONFIG_FILE",
 )
 
 MAX_IDLE_OPTION = typer.Option(default= 24 * 60 * 60, envvar="MAX_IDLE")
-IGNORE_WEEKENDS_OPTION = typer.Option(True, envvar="IGNORE_WEEKENDS")
-
+IGNORE_WEEKENDS_OPTION = typer.Option(default=True, envvar="IGNORE_WEEKENDS")
 
 def main(
     send_to: List[int] = typer.Argument(None),
     max_idle: int = MAX_IDLE_OPTION,
     ignore_weekends: bool = IGNORE_WEEKENDS_OPTION,
-    config_file: Path = CONFIG_OPTION
+    config_file: Path = CONFIG_OPTION,
   ):
   client = zulip.Client(config_file=config_file)
 
   now = time.time()
   today = datetime.date.today()
   idle_users = []
 
@@ -55,21 +54,24 @@
       old = now - presence['timestamp']
       if old > max_idle:
         idle_users.append(user)
 
   if idle_users:
     timeframe = humanize.naturaldelta(datetime.timedelta(seconds=max_idle))
     users = ", ".join(idle_users)
-    request = {
-      "type": "private",
-      "to": send_to,
-      "content": f"**The following user have been offline for more than {timeframe}:**\n{users}",
-    }
-    print(f"Sending Idle Users: {len(idle_users)}")
-    result = client.send_message(request)
+    msg = f"**The following user have been offline for more than {timeframe}:**\n{users}"
+    print(msg + "\n\n")
+    if send_to:
+      request = {
+        "type": "private",
+        "to": send_to,
+        "content": msg,
+      }
+      print(f"Sending Idle Users: {len(idle_users)}")
+      result = client.send_message(request)
 
   else:
     print("No Idle Users")
 
 def app():
   typer.run(main)
```

### Comparing `zulip_doc-0.2.0/PKG-INFO` & `zulip_doc-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zulip-doc
-Version: 0.2.0
+Version: 0.3.0
 Summary: Zulip service that checks user presence for Duty of Care responsibilities for remote teams
 Author-Email: Paul Bailey <paul@neutron.studio>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: zulip>=0.8.2
 Requires-Dist: typer>=0.9.0
 Requires-Dist: humanize>=4.7.0
```

