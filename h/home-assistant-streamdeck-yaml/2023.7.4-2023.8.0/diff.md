# Comparing `tmp/home_assistant_streamdeck_yaml-2023.7.4.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2023.7.4.tar", last modified: Fri Jul  7 07:20:36 2023, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2023.8.0.tar", last modified: Wed Aug  2 08:13:53 2023, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2023.7.4.tar` & `home_assistant_streamdeck_yaml-2023.8.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.668848 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 07:20:36.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    60076 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:36.672848 home_assistant_streamdeck_yaml-2023.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (123)    35366 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-07-07 07:20:18.000000 home_assistant_streamdeck_yaml-2023.7.4/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.999380 home_assistant_streamdeck_yaml-2023.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.991380 home_assistant_streamdeck_yaml-2023.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.991380 home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43640 2023-08-02 08:13:52.995380 home_assistant_streamdeck_yaml-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43166 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.995380 home_assistant_streamdeck_yaml-2023.8.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.995380 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43640 2023-08-02 08:13:52.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-02 08:13:52.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:13:52.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 08:13:52.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 08:13:52.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 08:13:52.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63007 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:13:52.999380 home_assistant_streamdeck_yaml-2023.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.995380 home_assistant_streamdeck_yaml-2023.8.0/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:13:52.995380 home_assistant_streamdeck_yaml-2023.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35462 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-08-02 08:13:30.000000 home_assistant_streamdeck_yaml-2023.8.0/tests/test_examples.py
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.github/release.py` & `home_assistant_streamdeck_yaml-2023.8.0/.github/release.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/release.yml` & `home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2023.8.0/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.gitignore` & `home_assistant_streamdeck_yaml-2023.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2023.8.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: mixed-line-ending
   - repo: "https://github.com/ambv/black"
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black-jupyter
         language_version: python3
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.276"
+    rev: "v0.0.281"
     hooks:
       - id: ruff
         args: ["--fix"]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.4.1"
     hooks:
       - id: mypy
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/Dockerfile` & `home_assistant_streamdeck_yaml-2023.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/LICENSE` & `home_assistant_streamdeck_yaml-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2023.7.4
+Version: 2023.8.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
@@ -297,32 +297,32 @@
 
 <!-- CODE:START -->
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
-| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
-|:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |           | `Optional[str]`                                                                                                 |
-| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
-| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
-| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
-| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
-| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
-| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
-| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
-| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                       |           | `Optional[str]`                                                                                                 |
-| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                                 |
-| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                           |
-| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
-| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                          |
-| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                        |           | `Union[float, str]`                                                                                             |
-| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed. |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
-| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used.                                                                 |           | `Optional[Any]`                                                                                                 |
+| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Default   | Type                                                                                                            |
+|:------------------------|:-----------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `Optional[str]`                                                                                                 |
+| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[str]`                                                                                                 |
+| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `str`                                                                                                           |
+| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |           | `Optional[str]`                                                                                                 |
+| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | `12`      | `int`                                                                                                           |
+| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `int`                                                                                                           |
+| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                                                                        |           | `Optional[str]`                                                                                                 |
+| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
+| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | `#000000` | `str`                                                                                                           |
+| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |           | `Optional[str]`                                                                                                 |
+| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |           | `bool`                                                                                                          |
+| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                                                                         |           | `Union[float, str]`                                                                                             |
+| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed.                                                  |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
+| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `color_temp_kelvin` key and a value a list of max (`n_keys_on_streamdeck - 5`) color temperatures in Kelvin. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used. |           | `Optional[Any]`                                                                                                 |
 
 <!-- OUTPUT:END -->
 
 # :bulb: More than 30 Button Configurations ideas
 
 Here are >30 interesting uses for the Stream Deck with Home Assistant (click on text to expand):
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/README.md` & `home_assistant_streamdeck_yaml-2023.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -284,32 +284,32 @@
 
 <!-- CODE:START -->
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
-| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
-|:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |           | `Optional[str]`                                                                                                 |
-| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
-| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
-| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
-| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
-| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
-| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
-| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
-| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                       |           | `Optional[str]`                                                                                                 |
-| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                                 |
-| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                           |
-| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
-| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                          |
-| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                        |           | `Union[float, str]`                                                                                             |
-| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed. |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
-| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used.                                                                 |           | `Optional[Any]`                                                                                                 |
+| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Default   | Type                                                                                                            |
+|:------------------------|:-----------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `Optional[str]`                                                                                                 |
+| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[str]`                                                                                                 |
+| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `str`                                                                                                           |
+| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |           | `Optional[str]`                                                                                                 |
+| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | `12`      | `int`                                                                                                           |
+| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `int`                                                                                                           |
+| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                                                                        |           | `Optional[str]`                                                                                                 |
+| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
+| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | `#000000` | `str`                                                                                                           |
+| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |           | `Optional[str]`                                                                                                 |
+| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |           | `bool`                                                                                                          |
+| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                                                                         |           | `Union[float, str]`                                                                                             |
+| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed.                                                  |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
+| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `color_temp_kelvin` key and a value a list of max (`n_keys_on_streamdeck - 5`) color temperatures in Kelvin. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used. |           | `Optional[Any]`                                                                                                 |
 
 <!-- OUTPUT:END -->
 
 # :bulb: More than 30 Button Configurations ideas
 
 Here are >30 interesting uses for the Stream Deck with Home Assistant (click on text to expand):
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2023.8.0/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/netflix.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/spotify.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/assets/xbox.png` & `home_assistant_streamdeck_yaml-2023.8.0/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/configuration.yaml` & `home_assistant_streamdeck_yaml-2023.8.0/configuration.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,25 @@
         service: light.toggle
         text: |
           Living room
           lights
         special_type: light-control
         special_type_data:
           colors:
-            - "#FF0000"  # red
-            - "#00FF00"  # green
+            - "#81ADFF"  # from default HA options
+            - "#D797FF"  # from default HA options
+            - "#FF9FF2"  # from default HA options
+            - "#FF7056"  # from default HA options
             - "#0000FF"  # blue
-            - "#FFFF00"  # yellow
-            - "#FFC0CB"  # pink
-            - "#800080"  # purple
-            - "#FFA500"  # orange
-            - "#00FFFF"  # cyan
-            - "#FFD700"  # gold
-            - "#008000"  # dark green
+            - "#FF0000"  # red
+          color_temp_kelvin:
+            - 2000  # from default HA options
+            - 3521  # from default HA options
+            - 5025  # from default HA options
+            - 6535  # from default HA options
       - special_type: go-to-page
         special_type_data: all-lights
         text: |
           All
           lights
       - entity_id: light.dinner_area
         service: light.toggle
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/docker-compose.yaml` & `home_assistant_streamdeck_yaml-2023.8.0/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-streamdeck-yaml
-Version: 2023.7.4
+Version: 2023.8.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
@@ -297,32 +297,32 @@
 
 <!-- CODE:START -->
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
-| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
-|:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |           | `Optional[str]`                                                                                                 |
-| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
-| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
-| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
-| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
-| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
-| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
-| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
-| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                       |           | `Optional[str]`                                                                                                 |
-| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                                 |
-| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                           |
-| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
-| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                          |
-| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                        |           | `Union[float, str]`                                                                                             |
-| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed. |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
-| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used.                                                                 |           | `Optional[Any]`                                                                                                 |
+| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Default   | Type                                                                                                            |
+|:------------------------|:-----------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed. The button is re-rendered whenever the state of this entity changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `Optional[str]`                                                                                                 |
+| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[str]`                                                                                                 |
+| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `str`                                                                                                           |
+| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |           | `Optional[str]`                                                                                                 |
+| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | `12`      | `int`                                                                                                           |
+| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `int`                                                                                                           |
+| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                                                                        |           | `Optional[str]`                                                                                                 |
+| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
+| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | `#000000` | `str`                                                                                                           |
+| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |           | `Optional[str]`                                                                                                 |
+| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |           | `bool`                                                                                                          |
+| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                                                                         |           | `Union[float, str]`                                                                                             |
+| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed.                                                  |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
+| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `color_temp_kelvin` key and a value a list of max (`n_keys_on_streamdeck - 5`) color temperatures in Kelvin. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used. |           | `Optional[Any]`                                                                                                 |
 
 <!-- OUTPUT:END -->
 
 # :bulb: More than 30 Button Configurations ideas
 
 Here are >30 interesting uses for the Stream Deck with Home Assistant (click on text to expand):
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2023.8.0/home_assistant_streamdeck_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import asyncio
 import colorsys
 import functools as ft
 import hashlib
 import io
 import json
+import math
 import re
 import time
 import warnings
 from contextlib import asynccontextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Literal, TypeAlias
 
@@ -181,14 +182,15 @@
         default=None,
         allow_template=True,
         description="Data for the special type of button."
         " If `go-to-page`, the data should be an `int` or `str` (name of the page)."
         " If `light-control`, the data should optionally be a dictionary."
         " The dictionary can contain the following keys:"
         " The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors."
+        " The `color_temp_kelvin` key and a value a list of max (`n_keys_on_streamdeck - 5`) color temperatures in Kelvin."
         " The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html)"
         " can be used. This requires the `matplotlib` package to be installed. If no"
         " list of `colors` or `colormap` is specified, 10 equally spaced colors are used.",
     )
 
     _timer: AsyncDelayedCallback | None = PrivateAttr(None)
 
@@ -376,15 +378,15 @@
             text=text,
             text_color=text_color if not key_pressed else "green",
             text_offset=self.text_offset,
         )
         return image
 
     @validator("special_type_data")
-    def _validate_special_type(
+    def _validate_special_type(  # noqa: PLR0912
         cls: type[Button],
         v: Any,
         values: dict[str, Any],
     ) -> Any:
         """Validate the special_type_data."""
         special_type = values["special_type"]
         if special_type == "go-to-page" and not isinstance(v, (int, str)):
@@ -404,15 +406,15 @@
             if not isinstance(v, dict):
                 msg = (
                     "With 'light-control', 'special_type_data' must"
                     f" be a dict, not '{v}'"
                 )
                 raise AssertionError(msg)
             # Can only have the following keys: colors and colormap
-            allowed_keys = {"colors", "colormap"}
+            allowed_keys = {"colors", "colormap", "color_temp_kelvin"}
             invalid_keys = v.keys() - allowed_keys
             if invalid_keys:
                 msg = (
                     f"Invalid keys in 'special_type_data', only {allowed_keys} allowed"
                 )
                 raise AssertionError(msg)
             # If colors is present, it must be a list of strings
@@ -422,14 +424,21 @@
                     raise AssertionError(msg)
                 for color in v["colors"]:
                     if not isinstance(color, str):
                         msg = "All colors must be strings"
                         raise AssertionError(msg)  # noqa: TRY004
                 # Cast colors to tuple (to make it hashable)
                 v["colors"] = tuple(v["colors"])
+            if "color_temp_kelvin" in v:
+                for kelvin in v["color_temp_kelvin"]:
+                    if not isinstance(kelvin, int):
+                        msg = "All color_temp_kelvin must be integers"
+                        raise AssertionError(msg)  # noqa: TRY004
+                # Cast color_temp_kelvin to tuple (to make it hashable)
+                v["color_temp_kelvin"] = tuple(v["color_temp_kelvin"])
         return v
 
     def maybe_start_or_cancel_timer(
         self,
         callback: Callable[[], None | Coroutine] | None = None,
     ) -> bool:
         """Start or cancel the timer."""
@@ -797,14 +806,77 @@
         raise ModuleNotFoundError(msg) from None
 
     cmap = plt.get_cmap(colormap)
     colors = cmap(np.linspace(0, 1, num_colors))
     return tuple(plt.matplotlib.colors.to_hex(color) for color in colors)
 
 
+def _color_temp_kelvin_to_rgb(  # noqa: PLR0912
+    colour_temperature: int,
+) -> tuple[int, int, int]:
+    """Converts from K to RGB.
+
+    Algorithm courtesy of
+    http://www.tannerhelland.com/4435/convert-temperature-rgb-algorithm-code/.
+    """
+    # range check
+    if colour_temperature < 1000:  # noqa: PLR2004
+        colour_temperature = 1000
+    elif colour_temperature > 40000:  # noqa: PLR2004
+        colour_temperature = 40000
+
+    tmp_internal = colour_temperature / 100.0
+
+    # red
+    if tmp_internal <= 66:  # noqa: PLR2004
+        red = 255
+    else:
+        tmp_red = 329.698727446 * math.pow(tmp_internal - 60, -0.1332047592)
+        if tmp_red < 0:
+            red = 0
+        elif tmp_red > 255:  # noqa: PLR2004
+            red = 255
+        else:
+            red = int(tmp_red)
+
+    # green
+    if tmp_internal <= 66:  # noqa: PLR2004
+        tmp_green = 99.4708025861 * math.log(tmp_internal) - 161.1195681661
+        if tmp_green < 0:
+            green = 0
+        elif tmp_green > 255:  # noqa: PLR2004
+            green = 255
+        else:
+            green = int(tmp_green)
+    else:
+        tmp_green = 288.1221695283 * math.pow(tmp_internal - 60, -0.0755148492)
+        if tmp_green < 0:
+            green = 0
+        elif tmp_green > 255:  # noqa: PLR2004
+            green = 255
+        else:
+            green = int(tmp_green)
+
+    # blue
+    if tmp_internal >= 66:  # noqa: PLR2004
+        blue = 255
+    elif tmp_internal <= 19:  # noqa: PLR2004
+        blue = 0
+    else:
+        tmp_blue = 138.5177312231 * math.log(tmp_internal - 10) - 305.0447927307
+        if tmp_blue < 0:
+            blue = 0
+        elif tmp_blue > 255:  # noqa: PLR2004
+            blue = 255
+        else:
+            blue = int(tmp_blue)
+
+    return red, green, blue
+
+
 def _generate_uniform_hex_colors(n_colors: int) -> tuple[str, ...]:
     """Generate a list of `n_colors` hex colors that are uniformly perceptually spaced.
 
     Parameters
     ----------
     n_colors
         The number of colors to generate.
@@ -861,14 +933,15 @@
 
 
 @ft.lru_cache(maxsize=16)
 def _light_page(
     entity_id: str,
     n_colors: int,
     colors: tuple[str, ...] | None,
+    color_temp_kelvin: tuple[int, ...] | None,
     colormap: str | None,
 ) -> Page:
     """Return a page of buttons for controlling lights."""
     if colormap is None and colors is None:
         colors = _generate_uniform_hex_colors(n_colors)
     elif colormap is not None:
         colors = _generate_colors_from_colormap(n_colors, colormap)
@@ -880,29 +953,43 @@
             service_data={
                 "entity_id": entity_id,
                 "rgb_color": _hex_to_rgb(color),
             },
         )
         for color in colors
     ]
+    buttons_color_temp_kelvin = [
+        Button(
+            icon_background_color=_rgb_to_hex(_color_temp_kelvin_to_rgb(kelvin)),
+            service="light.turn_on",
+            service_data={
+                "entity_id": entity_id,
+                "color_temp_kelvin": kelvin,
+            },
+        )
+        for kelvin in (color_temp_kelvin or ())
+    ]
     buttons_brightness = []
     for brightness in [0, 10, 30, 60, 100]:
         background_color = _scale_hex_color("#FFFFFF", brightness / 100)
         button = Button(
             icon_background_color=background_color,
             service="light.turn_on",
             text_color=_max_contrast_color(background_color),
             text=f"{brightness}%",
             service_data={
                 "entity_id": entity_id,
                 "brightness_pct": brightness,
             },
         )
         buttons_brightness.append(button)
-    return Page(name="Lights", buttons=buttons_colors + buttons_brightness)
+    return Page(
+        name="Lights",
+        buttons=buttons_colors + buttons_color_temp_kelvin + buttons_brightness,
+    )
 
 
 @asynccontextmanager
 async def setup_ws(
     host: str,
     token: str,
     protocol: Literal["wss", "ws"],
@@ -1437,14 +1524,15 @@
     elif button.special_type == "light-control":
         assert isinstance(button.special_type_data, dict)
         page = _light_page(
             entity_id=button.entity_id,
             n_colors=10,
             colormap=button.special_type_data.get("colormap", None),
             colors=button.special_type_data.get("colors", None),
+            color_temp_kelvin=button.special_type_data.get("color_temp_kelvin", None),
         )
         config._detached_page = page
         update_all()
         return  # to skip the _detached_page reset below
     elif button.special_type == "reload":
         config.reload()
         update_all()
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/pyproject.toml` & `home_assistant_streamdeck_yaml-2023.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2023.8.0/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/tests/state.json` & `home_assistant_streamdeck_yaml-2023.8.0/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/tests/test_app.py` & `home_assistant_streamdeck_yaml-2023.8.0/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,24 +419,26 @@
 def test_light_page() -> None:
     """Test light page."""
     page = _light_page(
         entity_id="light.bedroom",
         n_colors=10,
         colormap="hsv",
         colors=None,
+        color_temp_kelvin=None,
     )
     buttons = page.buttons
     assert len(buttons) == BUTTONS_PER_PAGE
     assert buttons[0].icon_background_color is not None
 
     page = _light_page(
         entity_id="light.bedroom",
         n_colors=10,
         colormap=None,
         colors=None,
+        color_temp_kelvin=None,
     )
     buttons = page.buttons
     assert len(buttons) == BUTTONS_PER_PAGE
     assert buttons[0].icon_background_color is not None
 
     hex_colors = (
         "#FF0000",  # red
@@ -452,14 +454,15 @@
     )
 
     page = _light_page(
         entity_id="light.bedroom",
         n_colors=10,
         colormap=None,
         colors=hex_colors,
+        color_temp_kelvin=None,
     )
     buttons = page.buttons
 
 
 def test_url_to_filename() -> None:
     """Test url_to_filename."""
     url = "https://www.example.com/path/to/file.html"
```

### Comparing `home_assistant_streamdeck_yaml-2023.7.4/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2023.8.0/tests/test_examples.py`

 * *Files identical despite different names*

