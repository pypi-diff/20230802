# Comparing `tmp/pydo-0.1.5.tar.gz` & `tmp/pydo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydo-0.1.5.tar", max compression
+gzip compressed data, was "pydo-0.1.6.tar", max compression
```

## Comparing `pydo-0.1.5.tar` & `pydo-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-06-13 14:11:48.852184 pydo-0.1.5/LICENSE
--rw-r--r--   0        0        0     7735 2023-06-13 14:11:48.852545 pydo-0.1.5/README.md
--rw-r--r--   0        0        0     1295 2023-06-13 14:11:48.857287 pydo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      779 2023-06-13 14:11:48.859264 pydo-0.1.5/src/pydo/__init__.py
--rw-r--r--   0        0        0    32652 2023-06-13 14:11:48.859745 pydo-0.1.5/src/pydo/_client.py
--rw-r--r--   0        0        0     2901 2023-06-13 14:11:48.860090 pydo-0.1.5/src/pydo/_configuration.py
--rw-r--r--   0        0        0     1875 2023-06-13 14:11:48.860424 pydo-0.1.5/src/pydo/_patch.py
--rw-r--r--   0        0        0    79579 2023-06-13 14:11:48.861092 pydo-0.1.5/src/pydo/_serialization.py
--rw-r--r--   0        0        0      770 2023-06-13 14:11:48.861534 pydo-0.1.5/src/pydo/_vendor.py
--rw-r--r--   0        0        0      383 2023-06-13 14:11:48.861794 pydo-0.1.5/src/pydo/_version.py
--rw-r--r--   0        0        0      726 2023-06-13 14:11:48.862202 pydo-0.1.5/src/pydo/aio/__init__.py
--rw-r--r--   0        0        0    32892 2023-06-13 14:11:48.862547 pydo-0.1.5/src/pydo/aio/_client.py
--rw-r--r--   0        0        0     2922 2023-06-13 14:11:48.862840 pydo-0.1.5/src/pydo/aio/_configuration.py
--rw-r--r--   0        0        0     2096 2023-06-13 14:11:48.863107 pydo-0.1.5/src/pydo/aio/_patch.py
--rw-r--r--   0        0        0     3055 2023-06-13 14:11:48.863504 pydo-0.1.5/src/pydo/aio/operations/__init__.py
--rw-r--r--   0        0        0  7214176 2023-06-13 14:11:48.948735 pydo-0.1.5/src/pydo/aio/operations/_operations.py
--rw-r--r--   0        0        0      800 2023-06-13 14:11:48.949861 pydo-0.1.5/src/pydo/aio/operations/_patch.py
--rw-r--r--   0        0        0      735 2023-06-13 14:11:48.950168 pydo-0.1.5/src/pydo/custom_policies.py
--rw-r--r--   0        0        0      233 2023-06-13 14:11:48.950458 pydo-0.1.5/src/pydo/exceptions.py
--rw-r--r--   0        0        0     3055 2023-06-13 14:11:48.950916 pydo-0.1.5/src/pydo/operations/__init__.py
--rw-r--r--   0        0        0  7421775 2023-06-13 14:11:48.986284 pydo-0.1.5/src/pydo/operations/_operations.py
--rw-r--r--   0        0        0      734 2023-06-13 14:11:48.987431 pydo-0.1.5/src/pydo/operations/_patch.py
--rw-r--r--   0        0        0       26 2023-06-13 14:11:48.987721 pydo-0.1.5/src/pydo/py.typed
--rw-r--r--   0        0        0     8965 2023-06-13 15:14:14.970620 pydo-0.1.5/setup.py
--rw-r--r--   0        0        0     8850 2023-06-13 15:14:14.971544 pydo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 21:02:20.822813 pydo-0.1.6/LICENSE
+-rw-r--r--   0        0        0     7735 2023-08-02 21:02:20.823303 pydo-0.1.6/README.md
+-rw-r--r--   0        0        0     1295 2023-08-02 21:02:20.828407 pydo-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      779 2023-08-02 21:02:20.830225 pydo-0.1.6/src/pydo/__init__.py
+-rw-r--r--   0        0        0    32652 2023-08-02 21:02:20.830765 pydo-0.1.6/src/pydo/_client.py
+-rw-r--r--   0        0        0     2901 2023-08-02 21:02:20.831111 pydo-0.1.6/src/pydo/_configuration.py
+-rw-r--r--   0        0        0     1875 2023-08-02 21:02:20.831460 pydo-0.1.6/src/pydo/_patch.py
+-rw-r--r--   0        0        0    79579 2023-08-02 21:02:20.832177 pydo-0.1.6/src/pydo/_serialization.py
+-rw-r--r--   0        0        0      770 2023-08-02 21:02:20.832487 pydo-0.1.6/src/pydo/_vendor.py
+-rw-r--r--   0        0        0      383 2023-08-02 21:02:20.832796 pydo-0.1.6/src/pydo/_version.py
+-rw-r--r--   0        0        0      726 2023-08-02 21:02:20.833162 pydo-0.1.6/src/pydo/aio/__init__.py
+-rw-r--r--   0        0        0    32892 2023-08-02 21:02:20.833505 pydo-0.1.6/src/pydo/aio/_client.py
+-rw-r--r--   0        0        0     2922 2023-08-02 21:02:20.833788 pydo-0.1.6/src/pydo/aio/_configuration.py
+-rw-r--r--   0        0        0     2096 2023-08-02 21:02:20.834066 pydo-0.1.6/src/pydo/aio/_patch.py
+-rw-r--r--   0        0        0     3055 2023-08-02 21:02:20.834685 pydo-0.1.6/src/pydo/aio/operations/__init__.py
+-rw-r--r--   0        0        0  7219149 2023-08-02 21:02:20.985373 pydo-0.1.6/src/pydo/aio/operations/_operations.py
+-rw-r--r--   0        0        0      800 2023-08-02 21:02:20.986182 pydo-0.1.6/src/pydo/aio/operations/_patch.py
+-rw-r--r--   0        0        0      735 2023-08-02 21:02:20.986475 pydo-0.1.6/src/pydo/custom_policies.py
+-rw-r--r--   0        0        0      233 2023-08-02 21:02:20.986732 pydo-0.1.6/src/pydo/exceptions.py
+-rw-r--r--   0        0        0     3055 2023-08-02 21:02:20.987099 pydo-0.1.6/src/pydo/operations/__init__.py
+-rw-r--r--   0        0        0  7426748 2023-08-02 21:02:21.005111 pydo-0.1.6/src/pydo/operations/_operations.py
+-rw-r--r--   0        0        0      734 2023-08-02 21:02:21.006600 pydo-0.1.6/src/pydo/operations/_patch.py
+-rw-r--r--   0        0        0       26 2023-08-02 21:02:21.006826 pydo-0.1.6/src/pydo/py.typed
+-rw-r--r--   0        0        0     8965 2023-08-02 21:02:50.302426 pydo-0.1.6/setup.py
+-rw-r--r--   0        0        0     8850 2023-08-02 21:02:50.303021 pydo-0.1.6/PKG-INFO
```

### Comparing `pydo-0.1.5/LICENSE` & `pydo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/README.md` & `pydo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/pyproject.toml` & `pydo-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydo"
-version = "0.1.5"
+version = "0.1.6"
 description = "The official client for interacting with the DigitalOcean API"
 authors = ["API Engineering <api-engineering@digitalocean.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/digitalocean/pydo"
 documentation = "https://pydo.readthedocs.io/"
 keywords = ["digitalocean", "api", "client"]
```

### Comparing `pydo-0.1.5/src/pydo/__init__.py` & `pydo-0.1.6/src/pydo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/_client.py` & `pydo-0.1.6/src/pydo/_client.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/_configuration.py` & `pydo-0.1.6/src/pydo/_configuration.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/_patch.py` & `pydo-0.1.6/src/pydo/_patch.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/_serialization.py` & `pydo-0.1.6/src/pydo/_serialization.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/_vendor.py` & `pydo-0.1.6/src/pydo/_vendor.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/aio/__init__.py` & `pydo-0.1.6/src/pydo/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/aio/_client.py` & `pydo-0.1.6/src/pydo/aio/_client.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/aio/_configuration.py` & `pydo-0.1.6/src/pydo/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/aio/_patch.py` & `pydo-0.1.6/src/pydo/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/aio/operations/__init__.py` & `pydo-0.1.6/src/pydo/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/aio/operations/_operations.py` & `pydo-0.1.6/src/pydo/aio/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,25 +281,25 @@
     build_ssh_keys_update_request,
     build_tags_assign_resources_request,
     build_tags_create_request,
     build_tags_delete_request,
     build_tags_get_request,
     build_tags_list_request,
     build_tags_unassign_resources_request,
-    build_uptime_alert_create_request,
-    build_uptime_alert_delete_request,
-    build_uptime_alert_get_request,
-    build_uptime_alert_update_request,
-    build_uptime_check_alerts_list_request,
-    build_uptime_check_create_request,
-    build_uptime_check_delete_request,
-    build_uptime_check_get_request,
-    build_uptime_check_state_get_request,
-    build_uptime_check_update_request,
-    build_uptime_checks_list_request,
+    build_uptime_create_alert_request,
+    build_uptime_create_check_request,
+    build_uptime_delete_alert_request,
+    build_uptime_delete_check_request,
+    build_uptime_get_alert_request,
+    build_uptime_get_check_request,
+    build_uptime_get_check_state_request,
+    build_uptime_list_alerts_request,
+    build_uptime_list_checks_request,
+    build_uptime_update_alert_request,
+    build_uptime_update_check_request,
     build_volume_actions_get_request,
     build_volume_actions_list_request,
     build_volume_actions_post_by_id_request,
     build_volume_actions_post_request,
     build_volume_snapshots_create_request,
     build_volume_snapshots_delete_by_id_request,
     build_volume_snapshots_get_by_id_request,
@@ -639,14 +639,15 @@
                           team may have active at one time. Required.
                         "email": "str",  # The email address used by the current user to
                           register for DigitalOcean. Required.
                         "email_verified": False,  # Default value is False. If true, the user
                           has verified their account via email. False otherwise. Required.
                         "floating_ip_limit": 0,  # The total number of Floating IPs the
                           current user or team may have. Required.
+                        "name": "str",  # Optional. The display name for the current user.
                         "status": "active",  # Default value is "active". This value is one
                           of "active", "warning" or "locked". Known values are: "active", "warning",
                           and "locked".
                         "status_message": "str",  # A human-readable message giving more
                           details about the status of the account. Required.
                         "team": {
                             "name": "str",  # Optional. The name for the current team.
@@ -73160,14 +73161,17 @@
                           creating a new user, the"ndefault for the version of MySQL in use will be
                           used. As of MySQL 8.0, the"ndefault is ``caching_sha2_password``. Required.
                           Known values are: "mysql_native_password" and "caching_sha2_password".
                     },
                     "name": "str",  # The name of a database user. Required.
                     "password": "str",  # Optional. A randomly generated password for the
                       database user.
+                    "readonly": bool,  # Optional. For MongoDB clusters, set to ``true`` to
+                      create a read-only user."nThis option is not currently supported for other
+                      database engines.
                     "role": "str"  # Optional. A string representing the database user's role.
                       The value will be either"n"primary" or "normal". Known values are: "primary" and
                       "normal".
                 }
 
                 # response body for status code(s): 201
                 response == {
@@ -89476,17 +89480,19 @@
                                     "auto_scale": bool,  # Optional. A boolean
                                       value indicating whether auto-scaling is enabled for this node
                                       pool.
                                     "count": 0,  # Optional. The number of
                                       Droplet instances in the node pool.
                                     "id": "str",  # Optional. A unique ID that
                                       can be used to identify and reference a specific node pool.
-                                    "labels": {},  # Optional. An object
-                                      containing a set of Kubernetes labels. The keys and are values
-                                      are both user-defined.
+                                    "labels": {},  # Optional. An object of
+                                      key/value mappings specifying labels to apply to all nodes in a
+                                      pool. Labels will automatically be applied to all existing nodes
+                                      and any subsequent nodes added to the pool. Note that when a
+                                      label is removed, it is not deleted from the nodes in the pool.
                                     "max_nodes": 0,  # Optional. The maximum
                                       number of nodes that this node pool can be auto-scaled to. The
                                       value will be ``0`` if ``auto_scale`` is set to ``false``.
                                     "min_nodes": 0,  # Optional. The minimum
                                       number of nodes that this node pool can be auto-scaled to. The
                                       value will be ``0`` if ``auto_scale`` is set to ``false``.
                                     "name": "str",  # Optional. A human-readable
@@ -89714,16 +89720,19 @@
                         {
                             "auto_scale": bool,  # Optional. A boolean value indicating
                               whether auto-scaling is enabled for this node pool.
                             "count": 0,  # Optional. The number of Droplet instances in
                               the node pool.
                             "id": "str",  # Optional. A unique ID that can be used to
                               identify and reference a specific node pool.
-                            "labels": {},  # Optional. An object containing a set of
-                              Kubernetes labels. The keys and are values are both user-defined.
+                            "labels": {},  # Optional. An object of key/value mappings
+                              specifying labels to apply to all nodes in a pool. Labels will
+                              automatically be applied to all existing nodes and any subsequent nodes
+                              added to the pool. Note that when a label is removed, it is not deleted
+                              from the nodes in the pool.
                             "max_nodes": 0,  # Optional. The maximum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "min_nodes": 0,  # Optional. The minimum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "name": "str",  # Optional. A human-readable name for the
@@ -89850,16 +89859,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -90021,16 +90033,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -90190,16 +90205,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -90415,16 +90433,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -90700,16 +90721,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -90883,16 +90907,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -91061,16 +91088,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -92443,16 +92473,19 @@
                         {
                             "auto_scale": bool,  # Optional. A boolean value indicating
                               whether auto-scaling is enabled for this node pool.
                             "count": 0,  # Optional. The number of Droplet instances in
                               the node pool.
                             "id": "str",  # Optional. A unique ID that can be used to
                               identify and reference a specific node pool.
-                            "labels": {},  # Optional. An object containing a set of
-                              Kubernetes labels. The keys and are values are both user-defined.
+                            "labels": {},  # Optional. An object of key/value mappings
+                              specifying labels to apply to all nodes in a pool. Labels will
+                              automatically be applied to all existing nodes and any subsequent nodes
+                              added to the pool. Note that when a label is removed, it is not deleted
+                              from the nodes in the pool.
                             "max_nodes": 0,  # Optional. The maximum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "min_nodes": 0,  # Optional. The minimum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "name": "str",  # Optional. A human-readable name for the
@@ -92622,16 +92655,18 @@
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "auto_scale": bool,  # Optional. A boolean value indicating whether
                       auto-scaling is enabled for this node pool.
                     "count": 0,  # Optional. The number of Droplet instances in the node pool.
                     "id": "str",  # Optional. A unique ID that can be used to identify and
                       reference a specific node pool.
-                    "labels": {},  # Optional. An object containing a set of Kubernetes labels.
-                      The keys and are values are both user-defined.
+                    "labels": {},  # Optional. An object of key/value mappings specifying labels
+                      to apply to all nodes in a pool. Labels will automatically be applied to all
+                      existing nodes and any subsequent nodes added to the pool. Note that when a label
+                      is removed, it is not deleted from the nodes in the pool.
                     "max_nodes": 0,  # Optional. The maximum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "min_nodes": 0,  # Optional. The minimum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "name": "str",  # Optional. A human-readable name for the node pool.
@@ -92688,16 +92723,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -92796,16 +92833,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -92899,16 +92938,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -93083,16 +93124,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -93265,16 +93308,18 @@
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "auto_scale": bool,  # Optional. A boolean value indicating whether
                       auto-scaling is enabled for this node pool.
                     "count": 0,  # Optional. The number of Droplet instances in the node pool.
                     "id": "str",  # Optional. A unique ID that can be used to identify and
                       reference a specific node pool.
-                    "labels": {},  # Optional. An object containing a set of Kubernetes labels.
-                      The keys and are values are both user-defined.
+                    "labels": {},  # Optional. An object of key/value mappings specifying labels
+                      to apply to all nodes in a pool. Labels will automatically be applied to all
+                      existing nodes and any subsequent nodes added to the pool. Note that when a label
+                      is removed, it is not deleted from the nodes in the pool.
                     "max_nodes": 0,  # Optional. The maximum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "min_nodes": 0,  # Optional. The minimum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "name": "str",  # Optional. A human-readable name for the node pool.
@@ -93329,16 +93374,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -93442,16 +93489,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -93549,16 +93598,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -113801,15 +113852,15 @@
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = (
             input_args.pop(0) if input_args else kwargs.pop("deserializer")
         )
 
     @distributed_trace_async
-    async def checks_list(
+    async def list_checks(
         self, *, per_page: int = 20, page: int = 1, **kwargs: Any
     ) -> JSON:
         """List All Checks.
 
         To list all of the Uptime checks on your account, send a GET request to ``/v2/uptime/checks``.
 
         :keyword per_page: Number of items returned per page. Default value is 20.
@@ -113871,15 +113922,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_checks_list_request(
+        request = build_uptime_list_checks_request(
             per_page=per_page,
             page=page,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
@@ -113930,15 +113981,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    async def check_create(
+    async def create_check(
         self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         """Create a New Check.
 
         To create an Uptime check, send a POST request to ``/v2/uptime/checks`` specifying the
         attributes
         in the table below in the JSON body.
@@ -113986,15 +114037,15 @@
                         "type": "str"  # Optional. The type of health check to perform. Known
                           values are: "ping", "http", and "https".
                     }
                 }
         """
 
     @overload
-    async def check_create(
+    async def create_check(
         self, body: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         """Create a New Check.
 
         To create an Uptime check, send a POST request to ``/v2/uptime/checks`` specifying the
         attributes
         in the table below in the JSON body.
@@ -114028,15 +114079,15 @@
                         "type": "str"  # Optional. The type of health check to perform. Known
                           values are: "ping", "http", and "https".
                     }
                 }
         """
 
     @distributed_trace_async
-    async def check_create(self, body: Union[JSON, IO], **kwargs: Any) -> JSON:
+    async def create_check(self, body: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Create a New Check.
 
         To create an Uptime check, send a POST request to ``/v2/uptime/checks`` specifying the
         attributes
         in the table below in the JSON body.
 
         :param body: Is either a model type or a IO type. Required.
@@ -114091,15 +114142,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_check_create_request(
+        request = build_uptime_create_check_request(
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
@@ -114134,15 +114185,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace_async
-    async def check_get(self, check_id: str, **kwargs: Any) -> JSON:
+    async def get_check(self, check_id: str, **kwargs: Any) -> JSON:
         """Retrieve an Existing Check.
 
         To show information about an existing check, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -114193,15 +114244,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_check_get_request(
+        request = build_uptime_get_check_request(
             check_id=check_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -114251,15 +114302,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    async def check_update(
+    async def update_check(
         self,
         check_id: str,
         body: JSON,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -114324,15 +114375,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @overload
-    async def check_update(
+    async def update_check(
         self,
         check_id: str,
         body: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -114383,15 +114434,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @distributed_trace_async
-    async def check_update(
+    async def update_check(
         self, check_id: str, body: Union[JSON, IO], **kwargs: Any
     ) -> JSON:
         """Update a Check.
 
         To update the settings of an Uptime check, send a PUT request to
         ``/v2/uptime/checks/$CHECK_ID``.
 
@@ -114460,15 +114511,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_check_update_request(
+        request = build_uptime_update_check_request(
             check_id=check_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -114521,15 +114572,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace_async
-    async def check_delete(self, check_id: str, **kwargs: Any) -> Optional[JSON]:
+    async def delete_check(self, check_id: str, **kwargs: Any) -> Optional[JSON]:
         """Delete a Check.
 
         To delete an Uptime check, send a DELETE request to ``/v2/uptime/checks/$CHECK_ID``. A 204
         status
         code with no body will be returned in response to a successful request.
 
         Deleting a check will also delete alerts associated with the check.
@@ -114565,15 +114616,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[JSON]]
 
-        request = build_uptime_check_delete_request(
+        request = build_uptime_delete_check_request(
             check_id=check_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -114619,15 +114670,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
     @distributed_trace_async
-    async def check_state_get(self, check_id: str, **kwargs: Any) -> JSON:
+    async def get_check_state(self, check_id: str, **kwargs: Any) -> JSON:
         """Retrieve Check State.
 
         To show information about an existing check's state, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID/state``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -114689,15 +114740,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_check_state_get_request(
+        request = build_uptime_get_check_state_request(
             check_id=check_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -114747,15 +114798,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace_async
-    async def check_alerts_list(
+    async def list_alerts(
         self, check_id: str, *, per_page: int = 20, page: int = 1, **kwargs: Any
     ) -> JSON:
         """List All Alerts.
 
         To list all of the alerts for an Uptime check, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID/alerts``.
 
@@ -114835,15 +114886,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_check_alerts_list_request(
+        request = build_uptime_list_alerts_request(
             check_id=check_id,
             per_page=per_page,
             page=page,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
@@ -114895,15 +114946,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    async def alert_create(
+    async def create_alert(
         self,
         check_id: str,
         body: JSON,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -115003,15 +115054,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @overload
-    async def alert_create(
+    async def create_alert(
         self,
         check_id: str,
         body: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -115083,15 +115134,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @distributed_trace_async
-    async def alert_create(
+    async def create_alert(
         self, check_id: str, body: Union[JSON, IO], **kwargs: Any
     ) -> JSON:
         """Create a New Alert.
 
         To create an Uptime alert, send a POST request to ``/v2/uptime/checks/$CHECK_ID/alerts``
         specifying the attributes
         in the table below in the JSON body.
@@ -115182,15 +115233,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_alert_create_request(
+        request = build_uptime_create_alert_request(
             check_id=check_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -115243,15 +115294,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace_async
-    async def alert_get(self, check_id: str, alert_id: str, **kwargs: Any) -> JSON:
+    async def get_alert(self, check_id: str, alert_id: str, **kwargs: Any) -> JSON:
         """Retrieve an Existing Alert.
 
         To show information about an existing alert, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID/alerts/$ALERT_ID``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -115317,15 +115368,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_alert_get_request(
+        request = build_uptime_get_alert_request(
             check_id=check_id,
             alert_id=alert_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
@@ -115376,15 +115427,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    async def alert_update(
+    async def update_alert(
         self,
         check_id: str,
         alert_id: str,
         body: JSON,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -115477,15 +115528,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @overload
-    async def alert_update(
+    async def update_alert(
         self,
         check_id: str,
         alert_id: str,
         body: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -115552,15 +115603,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @distributed_trace_async
-    async def alert_update(
+    async def update_alert(
         self, check_id: str, alert_id: str, body: Union[JSON, IO], **kwargs: Any
     ) -> JSON:
         """Update an Alert.
 
         To update the settings of an Uptime alert, send a PUT request to
         ``/v2/uptime/checks/$CHECK_ID/alerts/$ALERT_ID``.
 
@@ -115644,15 +115695,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_alert_update_request(
+        request = build_uptime_update_alert_request(
             check_id=check_id,
             alert_id=alert_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
@@ -115706,15 +115757,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace_async
-    async def alert_delete(
+    async def delete_alert(
         self, check_id: str, alert_id: str, **kwargs: Any
     ) -> Optional[JSON]:
         """Delete an Alert.
 
         To delete an Uptime alert, send a DELETE request to
         ``/v2/uptime/checks/$CHECK_ID/alerts/$ALERT_ID``. A 204 status
         code with no body will be returned in response to a successful request.
@@ -115752,15 +115803,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[JSON]]
 
-        request = build_uptime_alert_delete_request(
+        request = build_uptime_delete_alert_request(
             check_id=check_id,
             alert_id=alert_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
```

### Comparing `pydo-0.1.5/src/pydo/aio/operations/_patch.py` & `pydo-0.1.6/src/pydo/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/custom_policies.py` & `pydo-0.1.6/src/pydo/custom_policies.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/operations/__init__.py` & `pydo-0.1.6/src/pydo/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/src/pydo/operations/_operations.py` & `pydo-0.1.6/src/pydo/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -6727,15 +6727,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(
         method="GET", url=_url, params=_params, headers=_headers, **kwargs
     )
 
 
-def build_uptime_checks_list_request(
+def build_uptime_list_checks_request(
     *, per_page: int = 20, page: int = 1, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
@@ -6754,15 +6754,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(
         method="GET", url=_url, params=_params, headers=_headers, **kwargs
     )
 
 
-def build_uptime_check_create_request(**kwargs: Any) -> HttpRequest:
+def build_uptime_create_check_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
@@ -6775,15 +6775,15 @@
             "content_type", content_type, "str"
         )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_check_get_request(check_id: str, **kwargs: Any) -> HttpRequest:
+def build_uptime_get_check_request(check_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/uptime/checks/{check_id}"
     path_format_arguments = {
@@ -6794,15 +6794,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_check_update_request(check_id: str, **kwargs: Any) -> HttpRequest:
+def build_uptime_update_check_request(check_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
@@ -6820,15 +6820,15 @@
             "content_type", content_type, "str"
         )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_check_delete_request(check_id: str, **kwargs: Any) -> HttpRequest:
+def build_uptime_delete_check_request(check_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/uptime/checks/{check_id}"
     path_format_arguments = {
@@ -6839,15 +6839,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_check_state_get_request(check_id: str, **kwargs: Any) -> HttpRequest:
+def build_uptime_get_check_state_request(check_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/uptime/checks/{check_id}/state"
     path_format_arguments = {
@@ -6858,15 +6858,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_check_alerts_list_request(
+def build_uptime_list_alerts_request(
     check_id: str, *, per_page: int = 20, page: int = 1, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
@@ -6890,15 +6890,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(
         method="GET", url=_url, params=_params, headers=_headers, **kwargs
     )
 
 
-def build_uptime_alert_create_request(check_id: str, **kwargs: Any) -> HttpRequest:
+def build_uptime_create_alert_request(check_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )  # type: Optional[str]
     accept = _headers.pop("Accept", "application/json")
 
@@ -6916,15 +6916,15 @@
             "content_type", content_type, "str"
         )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_alert_get_request(
+def build_uptime_get_alert_request(
     check_id: str, alert_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -6938,15 +6938,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_alert_update_request(
+def build_uptime_update_alert_request(
     check_id: str, alert_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )  # type: Optional[str]
@@ -6967,15 +6967,15 @@
             "content_type", content_type, "str"
         )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
-def build_uptime_alert_delete_request(
+def build_uptime_delete_alert_request(
     check_id: str, alert_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -7303,14 +7303,15 @@
                           team may have active at one time. Required.
                         "email": "str",  # The email address used by the current user to
                           register for DigitalOcean. Required.
                         "email_verified": False,  # Default value is False. If true, the user
                           has verified their account via email. False otherwise. Required.
                         "floating_ip_limit": 0,  # The total number of Floating IPs the
                           current user or team may have. Required.
+                        "name": "str",  # Optional. The display name for the current user.
                         "status": "active",  # Default value is "active". This value is one
                           of "active", "warning" or "locked". Known values are: "active", "warning",
                           and "locked".
                         "status_message": "str",  # A human-readable message giving more
                           details about the status of the account. Required.
                         "team": {
                             "name": "str",  # Optional. The name for the current team.
@@ -79810,14 +79811,17 @@
                           creating a new user, the"ndefault for the version of MySQL in use will be
                           used. As of MySQL 8.0, the"ndefault is ``caching_sha2_password``. Required.
                           Known values are: "mysql_native_password" and "caching_sha2_password".
                     },
                     "name": "str",  # The name of a database user. Required.
                     "password": "str",  # Optional. A randomly generated password for the
                       database user.
+                    "readonly": bool,  # Optional. For MongoDB clusters, set to ``true`` to
+                      create a read-only user."nThis option is not currently supported for other
+                      database engines.
                     "role": "str"  # Optional. A string representing the database user's role.
                       The value will be either"n"primary" or "normal". Known values are: "primary" and
                       "normal".
                 }
 
                 # response body for status code(s): 201
                 response == {
@@ -96112,17 +96116,19 @@
                                     "auto_scale": bool,  # Optional. A boolean
                                       value indicating whether auto-scaling is enabled for this node
                                       pool.
                                     "count": 0,  # Optional. The number of
                                       Droplet instances in the node pool.
                                     "id": "str",  # Optional. A unique ID that
                                       can be used to identify and reference a specific node pool.
-                                    "labels": {},  # Optional. An object
-                                      containing a set of Kubernetes labels. The keys and are values
-                                      are both user-defined.
+                                    "labels": {},  # Optional. An object of
+                                      key/value mappings specifying labels to apply to all nodes in a
+                                      pool. Labels will automatically be applied to all existing nodes
+                                      and any subsequent nodes added to the pool. Note that when a
+                                      label is removed, it is not deleted from the nodes in the pool.
                                     "max_nodes": 0,  # Optional. The maximum
                                       number of nodes that this node pool can be auto-scaled to. The
                                       value will be ``0`` if ``auto_scale`` is set to ``false``.
                                     "min_nodes": 0,  # Optional. The minimum
                                       number of nodes that this node pool can be auto-scaled to. The
                                       value will be ``0`` if ``auto_scale`` is set to ``false``.
                                     "name": "str",  # Optional. A human-readable
@@ -96350,16 +96356,19 @@
                         {
                             "auto_scale": bool,  # Optional. A boolean value indicating
                               whether auto-scaling is enabled for this node pool.
                             "count": 0,  # Optional. The number of Droplet instances in
                               the node pool.
                             "id": "str",  # Optional. A unique ID that can be used to
                               identify and reference a specific node pool.
-                            "labels": {},  # Optional. An object containing a set of
-                              Kubernetes labels. The keys and are values are both user-defined.
+                            "labels": {},  # Optional. An object of key/value mappings
+                              specifying labels to apply to all nodes in a pool. Labels will
+                              automatically be applied to all existing nodes and any subsequent nodes
+                              added to the pool. Note that when a label is removed, it is not deleted
+                              from the nodes in the pool.
                             "max_nodes": 0,  # Optional. The maximum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "min_nodes": 0,  # Optional. The minimum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "name": "str",  # Optional. A human-readable name for the
@@ -96486,16 +96495,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -96657,16 +96669,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -96826,16 +96841,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -97051,16 +97069,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -97336,16 +97357,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -97519,16 +97543,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -97697,16 +97724,19 @@
                             {
                                 "auto_scale": bool,  # Optional. A boolean value
                                   indicating whether auto-scaling is enabled for this node pool.
                                 "count": 0,  # Optional. The number of Droplet
                                   instances in the node pool.
                                 "id": "str",  # Optional. A unique ID that can be
                                   used to identify and reference a specific node pool.
-                                "labels": {},  # Optional. An object containing a set
-                                  of Kubernetes labels. The keys and are values are both user-defined.
+                                "labels": {},  # Optional. An object of key/value
+                                  mappings specifying labels to apply to all nodes in a pool. Labels
+                                  will automatically be applied to all existing nodes and any
+                                  subsequent nodes added to the pool. Note that when a label is
+                                  removed, it is not deleted from the nodes in the pool.
                                 "max_nodes": 0,  # Optional. The maximum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "min_nodes": 0,  # Optional. The minimum number of
                                   nodes that this node pool can be auto-scaled to. The value will be
                                   ``0`` if ``auto_scale`` is set to ``false``.
                                 "name": "str",  # Optional. A human-readable name for
@@ -99079,16 +99109,19 @@
                         {
                             "auto_scale": bool,  # Optional. A boolean value indicating
                               whether auto-scaling is enabled for this node pool.
                             "count": 0,  # Optional. The number of Droplet instances in
                               the node pool.
                             "id": "str",  # Optional. A unique ID that can be used to
                               identify and reference a specific node pool.
-                            "labels": {},  # Optional. An object containing a set of
-                              Kubernetes labels. The keys and are values are both user-defined.
+                            "labels": {},  # Optional. An object of key/value mappings
+                              specifying labels to apply to all nodes in a pool. Labels will
+                              automatically be applied to all existing nodes and any subsequent nodes
+                              added to the pool. Note that when a label is removed, it is not deleted
+                              from the nodes in the pool.
                             "max_nodes": 0,  # Optional. The maximum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "min_nodes": 0,  # Optional. The minimum number of nodes that
                               this node pool can be auto-scaled to. The value will be ``0`` if
                               ``auto_scale`` is set to ``false``.
                             "name": "str",  # Optional. A human-readable name for the
@@ -99258,16 +99291,18 @@
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "auto_scale": bool,  # Optional. A boolean value indicating whether
                       auto-scaling is enabled for this node pool.
                     "count": 0,  # Optional. The number of Droplet instances in the node pool.
                     "id": "str",  # Optional. A unique ID that can be used to identify and
                       reference a specific node pool.
-                    "labels": {},  # Optional. An object containing a set of Kubernetes labels.
-                      The keys and are values are both user-defined.
+                    "labels": {},  # Optional. An object of key/value mappings specifying labels
+                      to apply to all nodes in a pool. Labels will automatically be applied to all
+                      existing nodes and any subsequent nodes added to the pool. Note that when a label
+                      is removed, it is not deleted from the nodes in the pool.
                     "max_nodes": 0,  # Optional. The maximum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "min_nodes": 0,  # Optional. The minimum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "name": "str",  # Optional. A human-readable name for the node pool.
@@ -99324,16 +99359,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -99432,16 +99469,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -99535,16 +99574,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -99717,16 +99758,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -99899,16 +99942,18 @@
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "auto_scale": bool,  # Optional. A boolean value indicating whether
                       auto-scaling is enabled for this node pool.
                     "count": 0,  # Optional. The number of Droplet instances in the node pool.
                     "id": "str",  # Optional. A unique ID that can be used to identify and
                       reference a specific node pool.
-                    "labels": {},  # Optional. An object containing a set of Kubernetes labels.
-                      The keys and are values are both user-defined.
+                    "labels": {},  # Optional. An object of key/value mappings specifying labels
+                      to apply to all nodes in a pool. Labels will automatically be applied to all
+                      existing nodes and any subsequent nodes added to the pool. Note that when a label
+                      is removed, it is not deleted from the nodes in the pool.
                     "max_nodes": 0,  # Optional. The maximum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "min_nodes": 0,  # Optional. The minimum number of nodes that this node pool
                       can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is set to
                       ``false``.
                     "name": "str",  # Optional. A human-readable name for the node pool.
@@ -99963,16 +100008,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -100076,16 +100123,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -100183,16 +100232,18 @@
                     "node_pool": {
                         "auto_scale": bool,  # Optional. A boolean value indicating whether
                           auto-scaling is enabled for this node pool.
                         "count": 0,  # Optional. The number of Droplet instances in the node
                           pool.
                         "id": "str",  # Optional. A unique ID that can be used to identify
                           and reference a specific node pool.
-                        "labels": {},  # Optional. An object containing a set of Kubernetes
-                          labels. The keys and are values are both user-defined.
+                        "labels": {},  # Optional. An object of key/value mappings specifying
+                          labels to apply to all nodes in a pool. Labels will automatically be applied
+                          to all existing nodes and any subsequent nodes added to the pool. Note that
+                          when a label is removed, it is not deleted from the nodes in the pool.
                         "max_nodes": 0,  # Optional. The maximum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "min_nodes": 0,  # Optional. The minimum number of nodes that this
                           node pool can be auto-scaled to. The value will be ``0`` if ``auto_scale`` is
                           set to ``false``.
                         "name": "str",  # Optional. A human-readable name for the node pool.
@@ -120423,15 +120474,15 @@
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = (
             input_args.pop(0) if input_args else kwargs.pop("deserializer")
         )
 
     @distributed_trace
-    def checks_list(self, *, per_page: int = 20, page: int = 1, **kwargs: Any) -> JSON:
+    def list_checks(self, *, per_page: int = 20, page: int = 1, **kwargs: Any) -> JSON:
         """List All Checks.
 
         To list all of the Uptime checks on your account, send a GET request to ``/v2/uptime/checks``.
 
         :keyword per_page: Number of items returned per page. Default value is 20.
         :paramtype per_page: int
         :keyword page: Which 'page' of paginated results to return. Default value is 1.
@@ -120491,15 +120542,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_checks_list_request(
+        request = build_uptime_list_checks_request(
             per_page=per_page,
             page=page,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
@@ -120550,15 +120601,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    def check_create(
+    def create_check(
         self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         """Create a New Check.
 
         To create an Uptime check, send a POST request to ``/v2/uptime/checks`` specifying the
         attributes
         in the table below in the JSON body.
@@ -120606,15 +120657,15 @@
                         "type": "str"  # Optional. The type of health check to perform. Known
                           values are: "ping", "http", and "https".
                     }
                 }
         """
 
     @overload
-    def check_create(
+    def create_check(
         self, body: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         """Create a New Check.
 
         To create an Uptime check, send a POST request to ``/v2/uptime/checks`` specifying the
         attributes
         in the table below in the JSON body.
@@ -120648,15 +120699,15 @@
                         "type": "str"  # Optional. The type of health check to perform. Known
                           values are: "ping", "http", and "https".
                     }
                 }
         """
 
     @distributed_trace
-    def check_create(self, body: Union[JSON, IO], **kwargs: Any) -> JSON:
+    def create_check(self, body: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Create a New Check.
 
         To create an Uptime check, send a POST request to ``/v2/uptime/checks`` specifying the
         attributes
         in the table below in the JSON body.
 
         :param body: Is either a model type or a IO type. Required.
@@ -120711,15 +120762,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_check_create_request(
+        request = build_uptime_create_check_request(
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
@@ -120754,15 +120805,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace
-    def check_get(self, check_id: str, **kwargs: Any) -> JSON:
+    def get_check(self, check_id: str, **kwargs: Any) -> JSON:
         """Retrieve an Existing Check.
 
         To show information about an existing check, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -120813,15 +120864,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_check_get_request(
+        request = build_uptime_get_check_request(
             check_id=check_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -120871,15 +120922,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    def check_update(
+    def update_check(
         self,
         check_id: str,
         body: JSON,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -120944,15 +120995,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @overload
-    def check_update(
+    def update_check(
         self,
         check_id: str,
         body: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -121003,15 +121054,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @distributed_trace
-    def check_update(self, check_id: str, body: Union[JSON, IO], **kwargs: Any) -> JSON:
+    def update_check(self, check_id: str, body: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update a Check.
 
         To update the settings of an Uptime check, send a PUT request to
         ``/v2/uptime/checks/$CHECK_ID``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -121078,15 +121129,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_check_update_request(
+        request = build_uptime_update_check_request(
             check_id=check_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -121139,15 +121190,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace
-    def check_delete(self, check_id: str, **kwargs: Any) -> Optional[JSON]:
+    def delete_check(self, check_id: str, **kwargs: Any) -> Optional[JSON]:
         """Delete a Check.
 
         To delete an Uptime check, send a DELETE request to ``/v2/uptime/checks/$CHECK_ID``. A 204
         status
         code with no body will be returned in response to a successful request.
 
         Deleting a check will also delete alerts associated with the check.
@@ -121183,15 +121234,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[JSON]]
 
-        request = build_uptime_check_delete_request(
+        request = build_uptime_delete_check_request(
             check_id=check_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -121237,15 +121288,15 @@
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
 
     @distributed_trace
-    def check_state_get(self, check_id: str, **kwargs: Any) -> JSON:
+    def get_check_state(self, check_id: str, **kwargs: Any) -> JSON:
         """Retrieve Check State.
 
         To show information about an existing check's state, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID/state``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -121307,15 +121358,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_check_state_get_request(
+        request = build_uptime_get_check_state_request(
             check_id=check_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
         pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -121365,15 +121416,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace
-    def check_alerts_list(
+    def list_alerts(
         self, check_id: str, *, per_page: int = 20, page: int = 1, **kwargs: Any
     ) -> JSON:
         """List All Alerts.
 
         To list all of the alerts for an Uptime check, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID/alerts``.
 
@@ -121453,15 +121504,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_check_alerts_list_request(
+        request = build_uptime_list_alerts_request(
             check_id=check_id,
             per_page=per_page,
             page=page,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
@@ -121513,15 +121564,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    def alert_create(
+    def create_alert(
         self,
         check_id: str,
         body: JSON,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -121621,15 +121672,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @overload
-    def alert_create(
+    def create_alert(
         self,
         check_id: str,
         body: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> JSON:
@@ -121701,15 +121752,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @distributed_trace
-    def alert_create(self, check_id: str, body: Union[JSON, IO], **kwargs: Any) -> JSON:
+    def create_alert(self, check_id: str, body: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Create a New Alert.
 
         To create an Uptime alert, send a POST request to ``/v2/uptime/checks/$CHECK_ID/alerts``
         specifying the attributes
         in the table below in the JSON body.
 
         :param check_id: A unique identifier for a check. Required.
@@ -121798,15 +121849,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_alert_create_request(
+        request = build_uptime_create_alert_request(
             check_id=check_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -121859,15 +121910,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace
-    def alert_get(self, check_id: str, alert_id: str, **kwargs: Any) -> JSON:
+    def get_alert(self, check_id: str, alert_id: str, **kwargs: Any) -> JSON:
         """Retrieve an Existing Alert.
 
         To show information about an existing alert, send a GET request to
         ``/v2/uptime/checks/$CHECK_ID/alerts/$ALERT_ID``.
 
         :param check_id: A unique identifier for a check. Required.
         :type check_id: str
@@ -121933,15 +121984,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[JSON]
 
-        request = build_uptime_alert_get_request(
+        request = build_uptime_get_alert_request(
             check_id=check_id,
             alert_id=alert_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
 
@@ -121992,15 +122043,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @overload
-    def alert_update(
+    def update_alert(
         self,
         check_id: str,
         alert_id: str,
         body: JSON,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -122093,15 +122144,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @overload
-    def alert_update(
+    def update_alert(
         self,
         check_id: str,
         alert_id: str,
         body: IO,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -122168,15 +122219,15 @@
                     "request_id": "str"  # Optional. Optionally, some endpoints may include a
                       request ID that should be  provided when reporting bugs or opening support
                       tickets to help  identify the issue.
                 }
         """
 
     @distributed_trace
-    def alert_update(
+    def update_alert(
         self, check_id: str, alert_id: str, body: Union[JSON, IO], **kwargs: Any
     ) -> JSON:
         """Update an Alert.
 
         To update the settings of an Uptime alert, send a PUT request to
         ``/v2/uptime/checks/$CHECK_ID/alerts/$ALERT_ID``.
 
@@ -122260,15 +122311,15 @@
         _json = None
         _content = None
         if isinstance(body, (IO, bytes)):
             _content = body
         else:
             _json = body
 
-        request = build_uptime_alert_update_request(
+        request = build_uptime_update_alert_request(
             check_id=check_id,
             alert_id=alert_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
@@ -122322,15 +122373,15 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), response_headers)
 
         return cast(JSON, deserialized)
 
     @distributed_trace
-    def alert_delete(
+    def delete_alert(
         self, check_id: str, alert_id: str, **kwargs: Any
     ) -> Optional[JSON]:
         """Delete an Alert.
 
         To delete an Uptime alert, send a DELETE request to
         ``/v2/uptime/checks/$CHECK_ID/alerts/$ALERT_ID``. A 204 status
         code with no body will be returned in response to a successful request.
@@ -122368,15 +122419,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls = kwargs.pop("cls", None)  # type: ClsType[Optional[JSON]]
 
-        request = build_uptime_alert_delete_request(
+        request = build_uptime_delete_alert_request(
             check_id=check_id,
             alert_id=alert_id,
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)  # type: ignore
```

### Comparing `pydo-0.1.5/src/pydo/operations/_patch.py` & `pydo-0.1.6/src/pydo/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `pydo-0.1.5/setup.py` & `pydo-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'typing-extensions>=3.7.4']
 
 extras_require = \
 {'aio': ['aiohttp>=3.0']}
 
 setup_kwargs = {
     'name': 'pydo',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'The official client for interacting with the DigitalOcean API',
     'long_description': '# **PyDo**\n\n`pydo` is the official Python client library that allows\nPython developers to interact with and manage their DigitalOcean\nresources through a Python abstraction layer on top of the raw\n[DigitalOcean API HTTP Interface](https://developers.digitalocean.com/documentation/v2/).\n\nA top priority of this project is to ensure the client abides by the API\ncontract. Therefore, the client itself wraps a generated client based\non the [DigitalOcean OpenAPI Specification](https://github.com/digitalocean/openapi) to support all of DigitalOcean\'s HTTP APIs.\n\n# **Getting Started With the Client**\n\n## Prerequisites\n\n- Python version: >= 3.7.2\n\n## Installation\n\nTo install from pip:\n\n```shell\n    pip install git+https://github.com/digitalocean/pydo.git\n```\n\nor, if repo is cloned locally:\n\n```shell\n    pip install /<PATH>/<TO>/pydo\n```\n\nTo install from source:\n\n```shell\nmake install\n```\n\n## **`pydo` Quickstart**\n\n> A quick guide to getting started with the client.\n\n`pydo` must be initialized with `pydo.Client()`. A DigitalOcean API Token is required. The token can be passed explicitly to `pydo.Client()`, as such:\n\n```python\nimport os\nfrom pydo import Client\n\nclient = Client(token=os.getenv("$DIGITALOCEAN_TOKEN"))\n```\n\n#### Example of Using `pydo` to Access DO Resources\n\nFind below a working example for GETting a ssh_key ([per this http request](https://docs.digitalocean.com/reference/api/api-reference/#operation/sshKeys_list)) and printing the ID associated with the ssh key. If you\'d like to try out this quick example, you can follow [these instructions](https://docs.digitalocean.com/products/droplets/how-to/add-ssh-keys/) to add ssh keys to your DO account.\n\n```python\nimport os\nfrom pydo import Client\n\nclient = Client(token=os.getenv("$DIGITALOCEAN_TOKEN"))\n\nssh_keys_resp = client.ssh_keys.list()\nfor k in ssh_keys_resp["ssh_keys"]:\n    print(f"ID: {k[\'id\']}, NAME: {k[\'name\']}, FINGERPRINT: {k[\'fingerprint\']}")\n```\n\nThe above code snippet should output the following:\n\n```shell\nID: 123456, NAME: my_test_ssh_key, FINGERPRINT: 5c:74:7e:60:28:69:34:ca:dd:74:67:c3:f3:00:7f:fe\nID: 123457, NAME: my_prod_ssh_key, FINGERPRINT: eb:76:c7:2a:d3:3e:80:5d:ef:2e:ca:86:d7:79:94:0d\n```\n\n**Consult the full list of supported DigitalOcean API endpoints in [PyDo\'s documentation](https://pydo.readthedocs.io/en/latest/).**\n\n**Note**: More working examples can be found [here](https://github.com/digitalocean/pydo/tree/main/examples).\n\n#### Pagination Example\n\nBelow is an example on handling pagination. One must parse the URL to find the\nnext page.\n\n```python\nresp = self.client.ssh_keys.list(per_page=50, page=page)\npages = resp.links.pages\nif \'next\' in pages.keys():\n    parsed_url = urlparse(pages[\'next\'])\n    page = parse_qs(parsed_url.query)[\'page\'][0]\nelse:\n    paginated = False\n```\n\n# **Contributing**\n\n>Visit our [Contribuing Guide](CONTRIBUTING.md) for more information on getting\ninvolved in developing this client.\n\n# **Tests**\n\n>The tests included in this repo are used to validate the generated client.\nWe use `pytest` to define and run the tests.\n\n**_Requirements_**\n\n- Python 3.7+\n  - Can be installed using something like\n    [pyenv](https://github.com/pyenv/pyenv)\n    - used to manage different installed versions of python.\n    - can also manage python virtual environments (with a plugin)\n  - [Poetry](https://python-poetry.org/docs/#installation).\n    - can also be configured to manage python virtual environments.\n\nThere are two types of test suites in the `tests/` directory.\n\n#### Mocked Tests: `tests/mocked/`\n\nTests in the `mocked` directory include:\n\n- tests that validate the generated client has all the expected classes and\n  methods for the respective API resources and operations.\n- tests that exercise individual operations against mocked responses.\n\nThese tests do not act against the real API so no real resources are created.\n\nTo run mocked tests, run:\n\n```shell\nmake test-mocked\n```\n\n#### Integration Tests: `tests/integration/`\n\nTests in the `integration` directory include tests that simulate specific\nscenarios a customer might use the client for to interact with the API.\n**_IMPORTANT:_** these tests require a valid API token and **_DO_** create real\nresources on the respective DigitalOcean account.\n\nTo run integration tests, run:\n\n```shell\nDIGITALOCEAN_TOKEN=... make test-integration\n```\n\n#### Test Customizations\n\nSome test values can be customized so integration tests can exercise different\nscenarios. For example, test use a default region to create resources. All the\ndefault values are managed in the\n[tests/integration/defaults.py](tests/integration/defaults.py) file. Any value\nthat has `environ.get()` can be overwritten by setting the respective environment\nvariable.\n\n#### Tests with Docker\n\nThe included Dockerfile is a developler convenience to test the package in\nisolation.\n\nTo use it, first build the image. Run:\n\n```shell\ndocker build -t pydo:dev .\n```\n\n##### Use the interactive python shell\n\nOpen the python shell:\n\n```shell\ndocker run -it --rm --name pydo pydo:dev python\n```\n\nThe above will launch an interactive python shell and display the following:\n\n```shell\nSkipping virtualenv creation, as specified in config file.\nPython 3.10.5 | packaged by conda-forge | (main, Jun 14 2022, 07:06:46) [GCC 10.3.0] on linux\nType "help", "copyright", "credits" or "license" for more information.\n>>>\n```\n\nFrom here you can use the client interactively:\n\n```shell\n>>> from pydo import Client\n>>> c = Client($DIGITALOCEAN_TOKEN)\n>>> c.droplets.get()\n```\n\nAlternatively, the tests can be run by attaching the tests as a volume and\nrunning pytest directly.\n\nRun:\n\n```shell\ndocker run -it --rm --name pydo -v $PWD/tests:/tests pydo:dev pytest tests/mocked\n```\n\n# **Known Issues**\n\n>This selection lists the known issues of the client generator.\n\n#### `kubernetes.get_kubeconfig` Does not serialize response content\n\nIn the generated python client, when calling client.kubernetes.get_kubeconfig(clust_id), the deserialization logic raises an error when the response content-type is applicaiton/yaml. We need to determine if the spec/schema can be configured such that the generator results in functions that properly handle the content. We will likely need to report the issue upstream to request support for the content-type.\n\n#### `invoices.get_pdf_by_uuid(invoice_uuid=invoice_uuid_param)` Does not return PDF\n\nIn the generated python client, when calling `invoices.get_pdf_by_uuid`, the response returns a Iterator[bytes] that does not format correctly into a PDF.\n\n#### Getting documentation via cli "help(<client function>)"\n\nCurrently, calling the "help(<client function>)" includes the API documentation for the respective operation which is substantial and can be confusing in the context of this client.\n\n# **Roadmap**\n\n>This section lists short-term and long-term goals for the project.\n**Note**: These are goals, not necessarily commitments. The sections are not intended to represent exclusive focus during these terms.\n\nShort term:\n\n> Usability, stability, and marketing.\n\nShort term, we are focused on improving usability and user productivity (part of this is getting the word out).\n\n- Documentation\n  - Support an automated process for creating comprehensive documentation that explains working of codes\n  - Support a clean cli `help(<client function>)` documentation solution\n- Release stability\n  - define release strategy\n  - pip release\n\nLong term:\n\n> Model support, expand on supporting functions\n\n- The client currently inputs and outputs JSON dictionaries. Adding models would unlock features such as typing and validation.\n- Add supporting functions to elevate customer experience (i.e. adding a funtion that surfaces IP address for a Droplet)\n',
     'author': 'API Engineering',
     'author_email': 'api-engineering@digitalocean.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/digitalocean/pydo',
```

### Comparing `pydo-0.1.5/PKG-INFO` & `pydo-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydo
-Version: 0.1.5
+Version: 0.1.6
 Summary: The official client for interacting with the DigitalOcean API
 Home-page: https://github.com/digitalocean/pydo
 License: Apache-2.0
 Keywords: digitalocean,api,client
 Author: API Engineering
 Author-email: api-engineering@digitalocean.com
 Requires-Python: >=3.7.2,<4.0.0
```

