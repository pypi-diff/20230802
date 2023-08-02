# Comparing `tmp/hamqtt_fs_publisher-0.1.2.tar.gz` & `tmp/hamqtt_fs_publisher-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamqtt_fs_publisher-0.1.2.tar", max compression
+gzip compressed data, was "hamqtt_fs_publisher-0.1.3.tar", max compression
```

## Comparing `hamqtt_fs_publisher-0.1.2.tar` & `hamqtt_fs_publisher-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/LICENSE
--rw-r--r--   0        0        0     2702 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/README.md
--rw-r--r--   0        0        0       54 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/__init__.py
--rw-r--r--   0        0        0     5361 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/__main__.py
--rw-r--r--   0        0        0     3505 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.py
--rw-r--r--   0        0        0     9263 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.schema.json
--rw-r--r--   0        0        0     1688 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 hamqtt_fs_publisher-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 21:45:35.549594 hamqtt_fs_publisher-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2702 2023-08-02 21:45:35.549594 hamqtt_fs_publisher-0.1.3/README.md
+-rw-r--r--   0        0        0       54 2023-08-02 21:45:35.549594 hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/__init__.py
+-rw-r--r--   0        0        0     5768 2023-08-02 21:45:35.549594 hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/__main__.py
+-rw-r--r--   0        0        0     3622 2023-08-02 21:45:35.549594 hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/configuration.py
+-rw-r--r--   0        0        0     9479 2023-08-02 21:45:35.553593 hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/configuration.schema.json
+-rw-r--r--   0        0        0     1919 2023-08-02 21:45:35.553593 hamqtt_fs_publisher-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 hamqtt_fs_publisher-0.1.3/PKG-INFO
```

### Comparing `hamqtt_fs_publisher-0.1.2/LICENSE` & `hamqtt_fs_publisher-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.2/README.md` & `hamqtt_fs_publisher-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/__main__.py` & `hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,22 @@
         )
 
     def publish_read(self):
         """Read a value from file and publish it to MQTT broker."""
         state = self._config.read_path.read_text("utf-8")
         if self._config.read_strip:
             state = state.strip()
+        if self._config.read_multiplier is not None:
+            try:
+                state = float(state) * self._config.read_multiplier
+            except ValueError:
+                logger.error(
+                    "{}: Failed to apply multiplication due to float conversion error.",
+                    self._log_name,
+                )
         logger.debug('{}: Publishing state "{}".', self._log_name, state)
         self._entity.publish_state(state)
         if not self._stop_event.is_set():
             self.start(False)
 
     def start(self, log: bool = True):
         """Start the periodic reading."""
@@ -84,14 +92,15 @@
     help="Configuration file (either YAML or JSON).",
 )
 def main(config: Path):
     """Run the HA MQTT filesystem publisher."""
     logger.info("Parsing configuration...")
     config_found = False
     config_default_dir = Path("hamqtt_fs_publisher")
+    # TODO: Search for both config.json and yaml if not defined.
     for prefix in (
         Path(),
         Path("/etc") / config_default_dir,
         Path.home() / ".config" / config_default_dir,
     ):
         tried_path = prefix / config
         if tried_path.exists() and not tried_path.is_dir():
```

### Comparing `hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.py` & `hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     """Filesystem read-only mixin."""
 
     read_path: Path = Field(description="Path to read the value from.")
     read_interval: float = Field(10.0, description="Read interval in seconds.")
     read_strip: bool = Field(
         True, description="Perform a strip operation on the read value."
     )
+    read_multiplier: Optional[float] = Field(
+        None, description="Multiply read value by given amount."
+    )
 
 
 class WriteMixin(BaseModel):  # pylint: disable=R0903
     """Filesystem write-only mixin."""
 
     write_path: Path = Field(description="Path to write the value to.")
```

### Comparing `hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.schema.json` & `hamqtt_fs_publisher-0.1.3/hamqtt_fs_publisher/configuration.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998842592592593%*

 * *Differences: {"'definitions'": "{'Sensor': {'properties': {'read_multiplier': OrderedDict([('title', 'Read "*

 * *                  "Multiplier'), ('description', 'Multiply read value by given amount.'), ('type', "*

 * *                  "'number')])}}}"}*

```diff
@@ -216,14 +216,19 @@
                 },
                 "read_interval": {
                     "default": 10.0,
                     "description": "Read interval in seconds.",
                     "title": "Read Interval",
                     "type": "number"
                 },
+                "read_multiplier": {
+                    "description": "Multiply read value by given amount.",
+                    "title": "Read Multiplier",
+                    "type": "number"
+                },
                 "read_path": {
                     "description": "Path to read the value from.",
                     "format": "path",
                     "title": "Read Path",
                     "type": "string"
                 },
                 "read_strip": {
```

### Comparing `hamqtt_fs_publisher-0.1.2/pyproject.toml` & `hamqtt_fs_publisher-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hamqtt-fs-publisher"
-version = "0.1.2"
+version = "0.1.3"
 description = "Publish file content as MQTT topic compatible with HomeAssistant."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
@@ -58,7 +58,10 @@
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.main]
 extension-pkg-whitelist = ["pydantic"]
 load-plugins = ["pylint_pydantic"]
+
+[tool.pylint."messages control"]
+disable = ["raw-checker-failed", "bad-inline-option", "locally-disabled", "file-ignored", "suppressed-message", "useless-suppression", "deprecated-pragma", "use-symbolic-message-instead", "fixme"]
```

### Comparing `hamqtt_fs_publisher-0.1.2/PKG-INFO` & `hamqtt_fs_publisher-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamqtt-fs-publisher
-Version: 0.1.2
+Version: 0.1.3
 Summary: Publish file content as MQTT topic compatible with HomeAssistant.
 Home-page: https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
```

