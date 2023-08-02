# Comparing `tmp/nso-oc-2.75.0.tar.gz` & `tmp/nso-oc-2.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.75.0.tar", last modified: Thu Jul 27 19:19:17 2023, max compression
+gzip compressed data, was "nso-oc-2.76.0.tar", last modified: Wed Aug  2 15:11:26 2023, max compression
```

## Comparing `nso-oc-2.75.0.tar` & `nso-oc-2.76.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:17.682756 nso-oc-2.75.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-27 19:18:37.000000 nso-oc-2.75.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 19:18:37.000000 nso-oc-2.75.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-27 19:19:17.682756 nso-oc-2.75.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-27 19:18:37.000000 nso-oc-2.75.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:17.674756 nso-oc-2.75.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-27 19:19:17.000000 nso-oc-2.75.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 19:19:17.000000 nso-oc-2.75.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:19:17.000000 nso-oc-2.75.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 19:19:17.000000 nso-oc-2.75.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 19:19:17.000000 nso-oc-2.75.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 19:19:17.000000 nso-oc-2.75.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:17.674756 nso-oc-2.75.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:17.678756 nso-oc-2.75.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33602 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:19:17.682756 nso-oc-2.75.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-27 19:18:37.000000 nso-oc-2.75.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 19:18:37.000000 nso-oc-2.75.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 19:19:17.682756 nso-oc-2.75.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-27 19:18:37.000000 nso-oc-2.75.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:11:26.362166 nso-oc-2.76.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-08-02 15:10:55.000000 nso-oc-2.76.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 15:10:55.000000 nso-oc-2.76.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-02 15:11:26.362166 nso-oc-2.76.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-02 15:10:55.000000 nso-oc-2.76.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:11:26.358166 nso-oc-2.76.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-02 15:11:26.000000 nso-oc-2.76.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-02 15:11:26.000000 nso-oc-2.76.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:11:26.000000 nso-oc-2.76.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 15:11:26.000000 nso-oc-2.76.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 15:11:26.000000 nso-oc-2.76.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 15:11:26.000000 nso-oc-2.76.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:11:26.358166 nso-oc-2.76.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:11:26.362166 nso-oc-2.76.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33602 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64005 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:11:26.362166 nso-oc-2.76.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-08-02 15:10:55.000000 nso-oc-2.76.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 15:10:55.000000 nso-oc-2.76.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 15:11:26.362166 nso-oc-2.76.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-02 15:10:55.000000 nso-oc-2.76.0/setup.py
```

### Comparing `nso-oc-2.75.0/LICENSE` & `nso-oc-2.76.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/PKG-INFO` & `nso-oc-2.76.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.75.0
+Version: 2.76.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.75.0/README.md` & `nso-oc-2.76.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.76.0/nso_oc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.75.0
+Version: 2.76.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.75.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.76.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/README.md` & `nso-oc-2.76.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/common.py` & `nso-oc-2.76.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/main.py` & `nso-oc-2.76.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 interface_dict[interface_type].update(temp)
                 nso_old_physical_interface_number = physical_interface_number
             oc_interface_index += 1
     return interface_dict
 
 
 def configure_switched_vlan(nso_before_interface: dict, nso_leftover_interface: dict,
-                            openconfig_interface: dict, interface_name: str) -> None:
+                            openconfig_interface: dict, interface_name: str, vlans_vlan_database: list) -> None:
     """Configure L2 interfaces: TRUNK and ACCESS"""
     openconfig_interface.update(
         {"openconfig-vlan:switched-vlan": {"openconfig-vlan:config": {}}})
     # Mode ACCESS
     if type(nso_before_interface["switchport"].get("mode", {}).get("access")) is dict:
         openconfig_interface["openconfig-vlan:switched-vlan"][
             "openconfig-vlan:config"]["openconfig-vlan:interface-mode"] = "ACCESS"
@@ -205,32 +205,34 @@
         del nso_leftover_interface["switchport"]["mode"]
         if nso_before_interface["switchport"].get("trunk", {}).get("native", {}).get("vlan"):
             openconfig_interface["openconfig-vlan:switched-vlan"][
                 "openconfig-vlan:config"]["openconfig-vlan:native-vlan"] = \
                 nso_before_interface["switchport"]["trunk"].get("native", {}).get("vlan")
             del nso_leftover_interface["switchport"]["trunk"]["native"]
         if nso_before_interface["switchport"].get("trunk", {}).get("allowed", {}).get("vlan", {}).get("vlans"):
+            vlans_candidate = nso_before_interface["switchport"].get("trunk", {}).get("allowed", {}).get("vlan", {}).get("vlans")
+            vlans_allowed = [v for v in vlans_candidate if v in vlans_vlan_database]
             openconfig_interface["openconfig-vlan:switched-vlan"][
-                "openconfig-vlan:config"]["openconfig-vlan:trunk-vlans"] = \
-                nso_before_interface["switchport"].get("trunk", {}).get("allowed", {}).get("vlan", {}).get("vlans")
+                "openconfig-vlan:config"]["openconfig-vlan:trunk-vlans"] = vlans_allowed
             del nso_leftover_interface["switchport"]["trunk"]["allowed"]
     # Mode dynamic: desirable or dynamic: auto will be a converted to TRUNK in OC
     elif nso_before_interface["switchport"].get("mode", {}).get("dynamic"):
         openconfig_interface["openconfig-vlan:switched-vlan"][
             "openconfig-vlan:config"]["openconfig-vlan:interface-mode"] = "TRUNK"
         del nso_leftover_interface["switchport"]["mode"]
         if nso_before_interface["switchport"].get("trunk", {}).get("native", {}).get("vlan"):
             openconfig_interface["openconfig-vlan:switched-vlan"][
                 "openconfig-vlan:config"]["openconfig-vlan:native-vlan"] = \
                 nso_before_interface["switchport"]["trunk"].get("native", {}).get("vlan")
             del nso_leftover_interface["switchport"]["trunk"]["native"]
         if nso_before_interface["switchport"].get("trunk", {}).get("allowed", {}).get("vlan", {}).get("vlans"):
+            vlans_candidate = nso_before_interface["switchport"].get("trunk", {}).get("allowed", {}).get("vlan", {}).get("vlans")
+            vlans_allowed = [v for v in vlans_candidate if v in vlans_vlan_database]
             openconfig_interface["openconfig-vlan:switched-vlan"][
-                "openconfig-vlan:config"]["openconfig-vlan:trunk-vlans"] = \
-                nso_before_interface["switchport"].get("trunk", {}).get("allowed", {}).get("vlan", {}).get("vlans")
+                "openconfig-vlan:config"]["openconfig-vlan:trunk-vlans"] = vlans_allowed
             del nso_leftover_interface["switchport"]["trunk"]["allowed"]
         interfaces_notes_add(f"""
             Interface {interface_name} was set to trunking dynamic {nso_before_interface["switchport"].get("mode", {}).get("dynamic")}.
             OpenConfig configuration is now mode TRUNK. Review for issues.
         """)
 
 
@@ -509,14 +511,15 @@
                    interface_directory["oc_interface_index"], "openconfig-vlan:routed-vlan"]
         openconfig_interface = return_nested_dict(openconfig_interfaces, path_oc)
         xe_configure_ipv4_interface(nso_before_interface, nso_leftover_interface, openconfig_interface)
 
 
 def configure_port_channel(config_before: dict, config_leftover: dict, interface_data: dict) -> None:
     """Configure LACP port-channel"""
+    vlans_db = vlan_get_db(config_before)
     for interface_directory in interface_data.values():
         # Configure port-channel interface
         if interface_directory["nso_interface_type"] == "Port-channel":
             path_oc_physical = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                                 interface_directory["oc_interface_index"]]
             openconfig_interface_physical = return_nested_dict(openconfig_interfaces, path_oc_physical)
             interface_name = interface_directory["nso_interface_type"] + str(
@@ -531,15 +534,15 @@
             openconfig_interface_physical.update({"openconfig-if-aggregate:aggregation": {
                 "openconfig-if-aggregate:config": {"openconfig-if-aggregate:lag-type": "LACP"}}})
             path_oc_agg = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                            interface_directory["oc_interface_index"], "openconfig-if-aggregate:aggregation"]
             openconfig_interface_agg = return_nested_dict(openconfig_interfaces, path_oc_agg)
             if nso_before_interface.get("switchport"):
                 configure_switched_vlan(nso_before_interface, nso_leftover_interface, openconfig_interface_agg,
-                                        interface_name)
+                                        interface_name, vlans_db)
             xe_configure_ipv4_interface(nso_before_interface, nso_leftover_interface, openconfig_interface_agg)
         # Configure port-channel sub-interfaces
         if interface_directory["nso_interface_type"] == "Port-channel-subinterface":
             path_nso_subif = ["tailf-ned-cisco-ios:interface", "Port-channel-subinterface", "Port-channel",
                               interface_directory["nso_interface_index"]]
             nso_before_interface = return_nested_dict(config_before, path_nso_subif)
             nso_leftover_interface = return_nested_dict(config_leftover, path_nso_subif)
@@ -865,20 +868,25 @@
         # Keep object if it contains more properties
         if current_standby and len(current_standby) > 0:
             hsrp_leftover = current_standby
 
     return (service_hsrp, hsrp_leftover)
 
 
+def vlan_get_db(c):
+    return [v.get("id") for v in c.get("tailf-ned-cisco-ios:vlan", {}).get("vlan-list", [])]
+
+
 def configure_csmacd(config_before: dict, config_leftover: dict, interface_data: dict) -> None:
     """
     Iterate through interface_data
     Call up the config_before["tailf-ned-cisco-ios:interface"][v["nso_interface_type"]][v["nso_interface_index"]]
     Add need OC config to openconfig_interfaces["openconfig-interfaces:interfaces"]["openconfig-interfaces:interface"][v["oc_interface_index"]]
     """
+    vlans_db = vlan_get_db(config_before)
     for interface_directory in interface_data.values():
         path_oc = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                    interface_directory["oc_interface_index"], "openconfig-interfaces:subinterfaces",
                    "openconfig-interfaces:subinterface", interface_directory["oc_sub_interface_place_counter"]]
         openconfig_interface = return_nested_dict(openconfig_interfaces, path_oc)
         interface_name = interface_directory["nso_interface_type"] + str(
             config_before["tailf-ned-cisco-ios:interface"][interface_directory["nso_interface_type"]][
@@ -938,15 +946,15 @@
 
         # Is type really a l2vlan?
         if nso_before_interface.get("switchport"):
             openconfig_interface["openconfig-interfaces:config"]["openconfig-interfaces:type"] = "l2vlan"
             path_oc = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                        interface_directory["oc_interface_index"], "openconfig-if-ethernet:ethernet"]
             openconfig_interface = return_nested_dict(openconfig_interfaces, path_oc)
-            configure_switched_vlan(nso_before_interface, nso_leftover_interface, openconfig_interface, interface_name)
+            configure_switched_vlan(nso_before_interface, nso_leftover_interface, openconfig_interface, interface_name, vlans_db)
         else:
             path_oc = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                        interface_directory["oc_interface_index"], "openconfig-interfaces:subinterfaces",
                        "openconfig-interfaces:subinterface", interface_directory["oc_sub_interface_place_counter"]]
             openconfig_interface = return_nested_dict(openconfig_interfaces, path_oc)
             xe_configure_ipv4_interface(nso_before_interface, nso_leftover_interface, openconfig_interface)
```

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_mpls.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_mpls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.76.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.76.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.76.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.76.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.76.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.76.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.75.0/setup.py` & `nso-oc-2.76.0/setup.py`

 * *Files identical despite different names*

