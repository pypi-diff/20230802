# Comparing `tmp/spyral_cli-1.1.0.tar.gz` & `tmp/spyral_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.1.0.tar", max compression
+gzip compressed data, was "spyral_cli-1.1.1.tar", max compression
```

## Comparing `spyral_cli-1.1.0.tar` & `spyral_cli-1.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-07 10:36:11.542344 spyral_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.1.0/src/spyral/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-07 10:35:10.675160 spyral_cli-1.1.0/src/spyral/cli.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 spyral_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-08-02 16:10:27.195166 spyral_cli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.1.1/src/spyral/__init__.py
+-rw-r--r--   0        0        0     7172 2023-08-02 16:10:19.670178 spyral_cli-1.1.1/src/spyral/cli.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 spyral_cli-1.1.1/PKG-INFO
```

### Comparing `spyral_cli-1.1.0/pyproject.toml` & `spyral_cli-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
```

### Comparing `spyral_cli-1.1.0/src/spyral/cli.py` & `spyral_cli-1.1.1/src/spyral/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,16 @@
         if platform.system() == "Darwin":
             plotext.plot(mon.time, [v / 1000 for v in mon.vms], label="vms * 10^3")
         else:
             plotext.plot(mon.time, mon.vms, label="vms")
 
         plotext.show()  # to finally plot
 
+    raise typer.Exit(code=p.returncode)
+
 
 class Format(StrEnum):
     pdf = "pdf"
     png = "png"
 
 
 @app.command()
```

### Comparing `spyral_cli-1.1.0/PKG-INFO` & `spyral_cli-1.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

