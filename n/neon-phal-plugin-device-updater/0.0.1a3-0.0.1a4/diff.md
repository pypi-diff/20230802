# Comparing `tmp/neon-phal-plugin-device-updater-0.0.1a3.tar.gz` & `tmp/neon-phal-plugin-device-updater-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a3.tar", last modified: Mon Jul 31 21:01:42 2023, max compression
+gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a4.tar", last modified: Wed Aug  2 20:45:04 2023, max compression
```

## Comparing `neon-phal-plugin-device-updater-0.0.1a3.tar` & `neon-phal-plugin-device-updater-0.0.1a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater/
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:45:04.148000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/setup.py
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a3/LICENSE.md` & `neon-phal-plugin-device-updater-0.0.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.0.1a3/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater/__init__.py` & `neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,33 @@
                 with open("/opt/neon/build_info.json") as f:
                     self._build_info = json.load(f)
             except Exception as e:
                 LOG.error(f"Failed to get build info: {e}")
                 self._build_info = dict()
         return self._build_info
 
+    def _check_initramfs_update_available(self):
+        """
+        Check if there is a newer initramfs version available by comparing MD5
+        """
+        if not self.initramfs_url:
+            raise RuntimeError("No initramfs_url configured")
+        md5_request = requests.get(f"{self.initramfs_url}.md5")
+        if not md5_request.ok:
+            LOG.warning("Unable to get md5; downloading latest initramfs")
+            return self._get_initramfs_latest()
+        new_hash = md5_request.text.split('\n')[0]
+        with open(self.initramfs_real_path, 'rb') as f:
+            old_hash = hashlib.md5(f.read()).hexdigest()
+        if new_hash == old_hash:
+            LOG.debug("initramfs not changed")
+            return False
+        LOG.info("initramfs update available")
+        return True
+
     def _get_initramfs_latest(self) -> bool:
         """
         Get the latest initramfs image and check if it is different from the
         current installed initramfs
         """
         if not self.initramfs_url:
             raise RuntimeError("No initramfs_url configured")
@@ -95,15 +114,15 @@
             initramfs_request = requests.get(self.initramfs_url)
             if not initramfs_request.ok:
                 raise ConnectionError(f"Unable to get updated initramfs from: "
                                       f"{self.initramfs_url}")
             new_hash = hashlib.md5(initramfs_request.content).hexdigest()
             with open(self.initramfs_update_path, 'wb+') as f:
                 f.write(initramfs_request.content)
-        with open("/boot/firmware/initramfs", 'rb') as f:
+        with open(self.initramfs_real_path, 'rb') as f:
             old_hash = hashlib.md5(f.read()).hexdigest()
         if new_hash == old_hash:
             LOG.debug("initramfs not changed")
             return False
         return True
 
     def _check_squashfs_update_available(self) -> Optional[Tuple[str, str]]:
@@ -118,14 +137,15 @@
         download_url = valid_links[0][1]
 
         # Check if the latest version matches the installed version
         installed_image_time = self.build_info.get("base_os", {}).get("time")
         if installed_image_time and installed_image_time in newest_version:
             LOG.info("Already updated")
             return None
+        LOG.info(f"New squashFS: {newest_version}")
         return newest_version, download_url
 
     def _get_squashfs_latest(self) -> Optional[str]:
         """
         Get the latest squashfs image if different from the installed version
         @returns: path to downloaded update if present, else None
         """
@@ -161,15 +181,15 @@
                 remove(temp_dl_path)
 
     def check_update_initramfs(self, message: Message):
         """
         Handle a request to check for initramfs updates
         @param message: `neon.check_update_initramfs` Message
         """
-        update_available = self._get_initramfs_latest()
+        update_available = self._check_initramfs_update_available()
         self.bus.emit(message.response({"update_available": update_available}))
 
     def check_update_squashfs(self, message: Message):
         """
         Handle a request to check for squash updates
         @param message: `neon.check_update_squashfs` Message
         """
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a3/setup.py` & `neon-phal-plugin-device-updater-0.0.1a4/setup.py`

 * *Files identical despite different names*

