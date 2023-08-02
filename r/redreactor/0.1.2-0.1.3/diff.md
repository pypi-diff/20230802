# Comparing `tmp/redreactor-0.1.2.tar.gz` & `tmp/redreactor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redreactor-0.1.2.tar", max compression
+gzip compressed data, was "redreactor-0.1.3.tar", max compression
```

## Comparing `redreactor-0.1.2.tar` & `redreactor-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-07-25 19:51:52.729909 redreactor-0.1.2/LICENSE
--rw-r--r--   0        0        0     3409 2023-07-25 19:51:52.729909 redreactor-0.1.2/README.md
--rw-r--r--   0        0        0     3252 2023-07-25 19:52:08.442261 redreactor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       60 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/__init__.py
--rw-r--r--   0        0        0     3997 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/__main__.py
--rw-r--r--   0        0        0       97 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/commander/__init__.py
--rw-r--r--   0        0        0     6734 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/commander/commander.py
--rw-r--r--   0        0        0      121 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/__init__.py
--rw-r--r--   0        0        0      526 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/binary_sensor.py
--rw-r--r--   0        0        0      646 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/button.py
--rw-r--r--   0        0        0     4954 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/common.py
--rw-r--r--   0        0        0     7744 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/homeassistant.py
--rw-r--r--   0        0        0     1224 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/homeassistant/number.py
--rw-r--r--   0        0        0      707 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/homeassistant/sensor.py
--rw-r--r--   0        0        0       99 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/monitor/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/monitor/data.py
--rw-r--r--   0        0        0    12751 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/monitor/monitor.py
--rw-r--r--   0        0        0       84 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/mqtt/__init__.py
--rw-r--r--   0        0        0     6086 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/mqtt/mqtt.py
--rw-r--r--   0        0        0     8497 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/configuration.py
--rw-r--r--   0        0        0      794 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/const.py
--rw-r--r--   0        0        0       37 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/__init__.py
--rw-r--r--   0        0        0      902 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/emitter.py
--rw-r--r--   0        0        0     1116 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/repeater.py
--rw-r--r--   0        0        0      673 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/utils.py
--rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 redreactor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-02 06:54:43.456903 redreactor-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3597 2023-08-02 06:54:43.456903 redreactor-0.1.3/README.md
+-rw-r--r--   0        0        0     3252 2023-08-02 06:55:02.041141 redreactor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/__init__.py
+-rw-r--r--   0        0        0     3997 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/__main__.py
+-rw-r--r--   0        0        0       97 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/commander/__init__.py
+-rw-r--r--   0        0        0     6734 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/commander/commander.py
+-rw-r--r--   0        0        0      121 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/__init__.py
+-rw-r--r--   0        0        0      526 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/binary_sensor.py
+-rw-r--r--   0        0        0      646 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/button.py
+-rw-r--r--   0        0        0     4954 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/common.py
+-rw-r--r--   0        0        0     7714 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/homeassistant.py
+-rw-r--r--   0        0        0     1224 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/number.py
+-rw-r--r--   0        0        0      707 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/homeassistant/sensor.py
+-rw-r--r--   0        0        0       99 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/monitor/__init__.py
+-rw-r--r--   0        0        0     1601 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/monitor/data.py
+-rw-r--r--   0        0        0    12751 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/monitor/monitor.py
+-rw-r--r--   0        0        0       84 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/mqtt/__init__.py
+-rw-r--r--   0        0        0     6086 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/components/mqtt/mqtt.py
+-rw-r--r--   0        0        0     8497 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/configuration.py
+-rw-r--r--   0        0        0      794 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/const.py
+-rw-r--r--   0        0        0       37 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/helpers/__init__.py
+-rw-r--r--   0        0        0      902 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/helpers/emitter.py
+-rw-r--r--   0        0        0     1116 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/helpers/repeater.py
+-rw-r--r--   0        0        0      673 2023-08-02 06:54:43.456903 redreactor-0.1.3/src/redreactor/helpers/utils.py
+-rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 redreactor-0.1.3/PKG-INFO
```

### Comparing `redreactor-0.1.2/LICENSE` & `redreactor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/README.md` & `redreactor-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
   - Immediate Shutdown
   - Immediate Restart
   - Change the Battery Warning Threshold
   - Change the Battery Voltage Minimum and Maximum
   - Change the Report Interval
 - Provides `systemd` service example, so it can be started as a service on system boot
 
+If you haven't already got yourself a Red Reactor (An uninterruptible battery powered backup for your Raspberry Pi), one can be purchased from there [website](https://theredreactor.com).
+
 ## Home Assistant
 
 Connecting your Home Assistant instance to the same MQTT Broker as your Red Reactor will allow your Red Reactor to be auto discovered by your Home Assistant instance. It will give you access to all the readings available from the Red Reactor sensors, and allows full configuration of the Red Reactor on the fly - it even adds the ability to reboot and shutdown your device at the push of a button.
 
 There is also a [Home Assistant Add-on](https://github.com/mreditor97/homeassistant-addons) available for Supervisor users.
 
 ## MQTT
```

### Comparing `redreactor-0.1.2/pyproject.toml` & `redreactor-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redreactor"
-version = "0.1.2"
+version = "0.1.3"
 description = "Red Reactor Battery Monitoring service with MQTT, and Home Assistant support"
 documentation = "https://github.com/mreditor97/redreactor"
 repository = "https://github.com/mreditor97/redreactor"
 homepage = "https://github.com/mreditor97/redreactor"
 authors = ["MrEditor97 <dev@mreditor97.co.uk>"]
 license = "MIT"
 readme = "README.md"
@@ -28,19 +28,19 @@
 blacken-docs = "1.15.0"
 codespell = "2.2.5"
 covdefaults = "2.3.0"
 coverage = {version = "7.2.7", extras = ["toml"]}
 mypy = "1.4.1"
 pre-commit = "3.3.3"
 pre-commit-hooks = "4.4.0"
-pylint = "2.17.4"
+pylint = "2.17.5"
 pytest = "7.4.0"
 pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
-ruff = "0.0.280"
+ruff = "0.0.282"
 safety = "2.4.0b1"
 types-cachetools = "^5.3.0"
 yamllint = "1.32.0"
 types-pyyaml = "^6.0.12.10"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
```

### Comparing `redreactor-0.1.2/src/redreactor/__main__.py` & `redreactor-0.1.3/src/redreactor/__main__.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/commander/commander.py` & `redreactor-0.1.3/src/redreactor/components/commander/commander.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/homeassistant/binary_sensor.py` & `redreactor-0.1.3/src/redreactor/components/homeassistant/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/homeassistant/button.py` & `redreactor-0.1.3/src/redreactor/components/homeassistant/button.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/homeassistant/common.py` & `redreactor-0.1.3/src/redreactor/components/homeassistant/common.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/homeassistant/homeassistant.py` & `redreactor-0.1.3/src/redreactor/components/homeassistant/homeassistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             sw_version="1.0.0",
         )
 
         for field in static_configuration["fields"]:
             field = static_configuration["fields"][field]  # noqa: PLW2901
 
             configuring: Base = Base(
-                name=f"{configuration_defaults.name} {field.get('pretty')}",
+                name=f"{field.get('pretty')}",
                 device_class=field.get("device_class", None),
                 state_class="measurement",
                 expire_after=int(static_configuration["homeassistant"]["expire_after"]),
                 entity_category=field.get("entity_category", None),
                 icon=field.get("icon", None),
                 object_id=field.get("object_id", None),
                 unique_id=f"{configuration_defaults.identifiers}_{field['name']}",
```

### Comparing `redreactor-0.1.2/src/redreactor/components/homeassistant/number.py` & `redreactor-0.1.3/src/redreactor/components/homeassistant/number.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/homeassistant/sensor.py` & `redreactor-0.1.3/src/redreactor/components/homeassistant/sensor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/monitor/data.py` & `redreactor-0.1.3/src/redreactor/components/monitor/data.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/monitor/monitor.py` & `redreactor-0.1.3/src/redreactor/components/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/components/mqtt/mqtt.py` & `redreactor-0.1.3/src/redreactor/components/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/configuration.py` & `redreactor-0.1.3/src/redreactor/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,80 +132,80 @@
                     "type": "sensor",
                     "unit": "mA",
                     "device_class": "current",
                     "suggested_display_precision": 2,
                 },
                 "battery_level": {
                     "name": "battery_level",
-                    "pretty": "Battery Level",
+                    "pretty": "Battery level",
                     "type": "sensor",
                     "unit": "%",
                     "device_class": "battery",
                 },
                 "external_power": {
                     "name": "external_power",
-                    "pretty": "External Power",
+                    "pretty": "External power",
                     "type": "binary_sensor",
                     "device_class": "plug",
                     "entity_category": "diagnostic",
                 },
                 "cpu_temperature": {
                     "name": "cpu_temperature",
-                    "pretty": "CPU Temperature",
+                    "pretty": "CPU temperature",
                     "type": "sensor",
                     "unit": "°C",
                     "device_class": "temperature",
                     "entity_category": "diagnostic",
                     "suggested_display_precision": 2,
                 },
                 "cpu_stat": {
                     "name": "cpu_stat",
-                    "pretty": "CPU Stat",
+                    "pretty": "CPU stat",
                     "type": "sensor",
                     "entity_category": "diagnostic",
                 },
                 "battery_warning_threshold": {
                     "name": "battery_warning_threshold",
-                    "pretty": "Battery Warning",
+                    "pretty": "Battery warning",
                     "type": "number",
                     "unit": "%",
                     "device_class": "battery",
                     "entity_category": "diagnostic",
                     "min": 0,
                     "max": 100,
                     "mode": "box",
                     "step": 1,
                 },
                 "battery_voltage_minimum": {
                     "name": "battery_voltage_minimum",
-                    "pretty": "Battery Voltage Minimum",
+                    "pretty": "Battery voltage minimum",
                     "type": "number",
                     "unit": "V",
                     "device_class": "voltage",
                     "entity_category": "diagnostic",
                     "min": 2.5,
                     "max": 4.5,
                     "mode": "box",
                     "step": 0.1,
                 },
                 "battery_voltage_maximum": {
                     "name": "battery_voltage_maximum",
-                    "pretty": "Battery Voltage Maximum",
+                    "pretty": "Battery voltage maximum",
                     "type": "number",
                     "unit": "V",
                     "device_class": "voltage",
                     "entity_category": "diagnostic",
                     "min": 2.5,
                     "max": 4.5,
                     "mode": "box",
                     "step": 0.1,
                 },
                 "report_interval": {
                     "name": "report_interval",
-                    "pretty": "Report Interval",
+                    "pretty": "Report interval",
                     "type": "number",
                     "unit": "s",
                     "entity_category": "diagnostic",
                     "min": 5,
                     "max": 300,
                     "mode": "box",
                     "step": 5,
```

### Comparing `redreactor-0.1.2/src/redreactor/const.py` & `redreactor-0.1.3/src/redreactor/const.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/helpers/emitter.py` & `redreactor-0.1.3/src/redreactor/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/helpers/repeater.py` & `redreactor-0.1.3/src/redreactor/helpers/repeater.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/src/redreactor/helpers/utils.py` & `redreactor-0.1.3/src/redreactor/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.2/PKG-INFO` & `redreactor-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redreactor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Red Reactor Battery Monitoring service with MQTT, and Home Assistant support
 Home-page: https://github.com/mreditor97/redreactor
 License: MIT
 Author: MrEditor97
 Author-email: dev@mreditor97.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,16 @@
   - Immediate Shutdown
   - Immediate Restart
   - Change the Battery Warning Threshold
   - Change the Battery Voltage Minimum and Maximum
   - Change the Report Interval
 - Provides `systemd` service example, so it can be started as a service on system boot
 
+If you haven't already got yourself a Red Reactor (An uninterruptible battery powered backup for your Raspberry Pi), one can be purchased from there [website](https://theredreactor.com).
+
 ## Home Assistant
 
 Connecting your Home Assistant instance to the same MQTT Broker as your Red Reactor will allow your Red Reactor to be auto discovered by your Home Assistant instance. It will give you access to all the readings available from the Red Reactor sensors, and allows full configuration of the Red Reactor on the fly - it even adds the ability to reboot and shutdown your device at the push of a button.
 
 There is also a [Home Assistant Add-on](https://github.com/mreditor97/homeassistant-addons) available for Supervisor users.
 
 ## MQTT
```

