# Comparing `tmp/kubernetes_square-1.5.0.tar.gz` & `tmp/kubernetes_square-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes_square-1.5.0.tar", max compression
+gzip compressed data, was "kubernetes_square-1.5.1.tar", max compression
```

## Comparing `kubernetes_square-1.5.0.tar` & `kubernetes_square-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.5.0/LICENSE
--rw-r--r--   0        0        0      701 2023-07-29 08:50:02.005888 kubernetes_square-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3531 2023-07-22 06:18:28.743886 kubernetes_square-1.5.0/resources/defaultconfig.yaml
--rw-r--r--   0        0        0     1376 2023-07-29 08:50:02.005888 kubernetes_square-1.5.0/square/__init__.py
--rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.5.0/square/__main__.py
--rw-r--r--   0        0        0     4858 2023-07-23 05:29:00.549037 kubernetes_square-1.5.0/square/cfgfile.py
--rw-r--r--   0        0        0     2452 2023-07-22 06:08:22.385613 kubernetes_square-1.5.0/square/dotdict.py
--rw-r--r--   0        0        0     8427 2023-07-23 06:08:32.331674 kubernetes_square-1.5.0/square/dtypes.py
--rw-r--r--   0        0        0    31412 2023-07-23 06:08:32.331674 kubernetes_square-1.5.0/square/k8s.py
--rw-r--r--   0        0        0    14826 2023-07-23 05:29:00.549037 kubernetes_square-1.5.0/square/main.py
--rw-r--r--   0        0        0    38762 2023-07-29 08:50:06.777865 kubernetes_square-1.5.0/square/manio.py
--rw-r--r--   0        0        0    29780 2023-07-29 08:50:06.781865 kubernetes_square-1.5.0/square/square.py
--rw-r--r--   0        0        0     2068 2023-07-22 06:18:28.739886 kubernetes_square-1.5.0/square/yaml_io.py
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 kubernetes_square-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.5.1/LICENSE
+-rw-r--r--   0        0        0      701 2023-08-02 14:05:20.611855 kubernetes_square-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3531 2023-07-22 06:18:28.743886 kubernetes_square-1.5.1/resources/defaultconfig.yaml
+-rw-r--r--   0        0        0     1376 2023-08-02 14:05:20.611855 kubernetes_square-1.5.1/square/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.5.1/square/__main__.py
+-rw-r--r--   0        0        0     4858 2023-07-23 05:29:00.549037 kubernetes_square-1.5.1/square/cfgfile.py
+-rw-r--r--   0        0        0     2452 2023-07-22 06:08:22.385613 kubernetes_square-1.5.1/square/dotdict.py
+-rw-r--r--   0        0        0     8427 2023-07-23 06:08:32.331674 kubernetes_square-1.5.1/square/dtypes.py
+-rw-r--r--   0        0        0    31412 2023-08-02 13:21:10.395865 kubernetes_square-1.5.1/square/k8s.py
+-rw-r--r--   0        0        0    14826 2023-07-23 05:29:00.549037 kubernetes_square-1.5.1/square/main.py
+-rw-r--r--   0        0        0    39197 2023-08-02 09:50:04.774615 kubernetes_square-1.5.1/square/manio.py
+-rw-r--r--   0        0        0    32351 2023-07-30 13:48:32.562491 kubernetes_square-1.5.1/square/square.py
+-rw-r--r--   0        0        0     2068 2023-07-22 06:18:28.739886 kubernetes_square-1.5.1/square/yaml_io.py
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 kubernetes_square-1.5.1/PKG-INFO
```

### Comparing `kubernetes_square-1.5.0/LICENSE` & `kubernetes_square-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.5.0/pyproject.toml` & `kubernetes_square-1.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kubernetes-square"
-version = "1.5.0"
+version = "1.5.1"
 description = ""
 authors = ["Oliver Nagy <olitheolix@gmail.com>"]
 packages = [
     { include = "square" },
 ]
 include = ["resources/defaultconfig.yaml"]
```

### Comparing `kubernetes_square-1.5.0/resources/defaultconfig.yaml` & `kubernetes_square-1.5.1/resources/defaultconfig.yaml`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.5.0/square/__init__.py` & `kubernetes_square-1.5.1/square/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from pathlib import Path
 
 from . import square
 from .cfgfile import load
 
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 
 
 # ---------------------------------------------------------------------------
 # Global Runtime Constants
 # ---------------------------------------------------------------------------
 # Determine the base folder. This is usually the folder of this very file, but
 # will be different if we run inside a bundle produced by PyInstaller.
```

### Comparing `kubernetes_square-1.5.0/square/cfgfile.py` & `kubernetes_square-1.5.1/square/cfgfile.py`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.5.0/square/dotdict.py` & `kubernetes_square-1.5.1/square/dotdict.py`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.5.0/square/dtypes.py` & `kubernetes_square-1.5.1/square/dtypes.py`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.5.0/square/k8s.py` & `kubernetes_square-1.5.1/square/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,20 +686,20 @@
 
     def valid(_res):
         """Return `True` if `res` describes a Square compatible resource."""
         # Convenience.
         name = _res["name"]
         verbs = list(sorted(_res["verbs"]))
 
-        # Ignore resource like "services/status". We only care for "services".
+        # Ignore resources like "services/status". We only care for "services".
         if "/" in name:
             logit.debug(f"Ignore resource <{name}>: has a slash ('/') in its name")
             return False
 
-        # Square can only man age the resource if it can be read, modified and
+        # Square can only manage the resource if it can be read, modified and
         # deleted. Here we check if `res` has the respective verbs.
         minimal_verbs = {"create", "delete", "get", "list", "patch", "update"}
         if not minimal_verbs.issubset(set(verbs)):
             logit.debug(f"Ignore resource <{name}>: insufficient verbs: {verbs}")
             return False
 
         return True
```

### Comparing `kubernetes_square-1.5.0/square/main.py` & `kubernetes_square-1.5.1/square/main.py`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.5.0/square/manio.py` & `kubernetes_square-1.5.1/square/manio.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,24 @@
         apiVersion=manifest['apiVersion'],
         kind=manifest['kind'],
         namespace=ns,
         name=manifest['metadata']['name']
     )
 
 
-def select(manifest: dict, selectors: Selectors) -> bool:
+def select(manifest: dict, selectors: Selectors,
+           match_labels: bool) -> bool:
     """Return `False` unless `manifest` satisfies _all_ `selectors`.
 
     Inputs:
         manifests: dict
-        selectors: Selectors,
+        selectors: Selectors
+        match_labels: bool
+            Skip label matching if `False`. This flag does not affect KIND or
+            Namespace matching.
 
     Returns:
         bool: `True` iff the resource matches all selectors.
 
     """
     # The "kinds" selector must be non-empty.
     if len(selectors.kinds) == 0:
@@ -107,45 +111,42 @@
 
     # Abort if this manifest does not have a KIND that matches the selector.
     if kind not in selectors._kinds_only:
         logit.debug(f"Kind {kind} does not match selector {selectors.kinds}")
         return False
 
     # The manifest must match all label selectors to be included.
-    if label_selectors:
+    if label_selectors and match_labels:
         # Convert the labels dictionary into a Set of (key, value) tuples. We can
         # then use set-logic to determine if the manifest has the necessary labels.
         labels = set(labels.items())
 
         if not label_selectors.issubset(labels):
             logit.debug(f"Labels {labels} do not match selector {selectors.labels}")
             return False
 
     # If we get to here then the resource matches all selectors.
     return True
 
 
-def unpack_k8s_resource_list(manifest_list: dict,
-                             selectors: Selectors) -> Tuple[SquareManifests, bool]:
-    """Return only those entries from `manifest_list` that match the `selectors`.
+def unpack_k8s_resource_list(manifest_list: dict) -> Tuple[SquareManifests, bool]:
+    """Convert the K8s `manifest_list` into a `SquareManifest` type.
 
-    The `manifest_list` must be a K8s List item, eg `DeploymentList` or
-    `NamespaceList`.
+    The `manifest_list` must be a K8s List, eg `DeploymentList` or `NamespaceList`.
 
     Input:
         manifest_list: dict
             K8s response from GET request for eg `deployments`.
-        selectors: Selectors
 
     Returns:
         SquareManifests
 
     """
-    # Ensure the server manifests have the essential fields. If not then
-    # something is seriously wrong.
+    # Ensure the server manifests have the essential fields. Something is
+    # seriously wrong if not.
     must_have = ("apiVersion", "kind", "items")
     missing = [key for key in must_have if key not in manifest_list]
     if len(missing) > 0:
         kind = manifest_list.get("kind", "UNKNOWN")
         logit.error(f"{kind} manifest is missing these keys: {missing}")
         return ({}, True)
     del must_have, missing
@@ -158,26 +159,24 @@
 
     # Strip off the "List" suffix from eg "DeploymentList".
     kind = kind[:-4]
 
     # Convenience.
     apiversion = manifest_list["apiVersion"]
 
-    # Compile the manifests into a {MetaManifest: Manifest} dictionary. Skip
-    # all the manifests that do not match the `selectors`.
+    # Compile the manifests into a {MetaManifest: Manifest} dictionary.
     manifests = {}
     for manifest in manifest_list["items"]:
         # The "kind" key is missing from the manifest when K8s returns them in
         # a list. Here we manually add it again because it is part of every
         # properly formatted stand-alone manifest.
         manifest = copy.deepcopy(manifest)
         manifest["kind"] = kind
         manifest['apiVersion'] = apiversion
-        if select(manifest, selectors):
-            manifests[make_meta(manifest)] = manifest
+        manifests[make_meta(manifest)] = manifest
     return (manifests, False)
 
 
 def _parse_worker(fname: Path,
                   yaml_str: str) -> Tuple[List[dict], bool]:
     logit.debug(f"Parsing <{fname}>")
 
@@ -227,16 +226,22 @@
             if err:
                 return ({}, err)
 
             # Remove all empty manifests. This typically happens when the YAML
             # file ends with a "---" string.
             manifests = [_ for _ in manifests if _ is not None]
 
-            # Retain only those manifests that satisfy the selectors.
-            manifests = [_ for _ in manifests if select(_, selectors)]
+            # Retain only those manifests with the correct KIND and namespace.
+            # The caller must match the labels themselves. This is necessary to
+            # line up resources that exist both locally and on the server but
+            # have incompatible labels. If we excluded them here then Square
+            # would think the resource does not exist and try to create it
+            # when, in fact, it should be patched.
+            # See `square.{make_plan, get_resources}` for details.
+            manifests = [_ for _ in manifests if select(_, selectors, False)]
 
             # Convert List[manifest] into List[(MetaManifest, manifest)].
             # Abort if `make_meta` throws a KeyError which happens if `file_yaml`
             # does not actually contain a Kubernetes manifest but some other
             # (valid) YAML.
             try:
                 out[fname] = [(make_meta(_), _) for _ in manifests]
@@ -317,25 +322,25 @@
     """
     # Avoid side effects.
     server_manifests = copy.deepcopy(server_manifests)
 
     # Only retain server manifests that match the selectors.
     server_manifests = {
         meta: manifest for meta, manifest in server_manifests.items()
-        if select(manifest, selectors)
+        if select(manifest, selectors, True)
     }
 
     # Add all local manifests that do not match the selectors to the server
     # manifests. This will *not* propagate to K8s in any way. However, it will
     # simplify the logic of this function because local and server manifests
     # that were not selected will be automatically in sync and not appear in
     # the diffs.
     for fname, manifests in local_manifests.items():
         for meta, manifest in manifests:
-            if select(manifest, selectors):
+            if select(manifest, selectors, True):
                 continue
             server_manifests[meta] = manifest
 
     # Create map for MetaManifest -> (File, doc-idx). The doc-idx denotes the
     # index of the manifest inside the YAML file which may contain multiple
     # manifests. We will need this index later to update the correct manifest
     # in the correct YAML file.
@@ -968,17 +973,17 @@
                 continue
 
             try:
                 # Download the resource manifests for the current `kind` from K8s.
                 manifest_list, err = square.k8s.get(k8sconfig.client, resource.url)
                 assert not err and manifest_list is not None
 
-                # Parse the K8s List (eg DeploymentList, NamespaceList, ...) into a
-                # Dict[MetaManifest, dict] dictionary.
-                manifests, err = unpack_k8s_resource_list(manifest_list, config.selectors)
+                # Parse the K8s List (eg `DeploymentList`, `NamespaceList`, ...) into a
+                # `SquareManifests` (ie `Dict[MetaManifest, dict]`) structure.
+                manifests, err = unpack_k8s_resource_list(manifest_list)
                 assert not err and manifests is not None
 
                 # Strip off the fields defined in `config.filters`.
                 ret = {k: strip(k8sconfig, man, config.filters)
                        for k, man in manifests.items()}
 
                 # Ensure `strip` worked for every manifest.
```

### Comparing `kubernetes_square-1.5.0/square/square.py` & `kubernetes_square-1.5.1/square/square.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     This function returns `server` verbatim if there is no overlap with
     `server` and `local`.
 
     Inputs:
         config: Square configuration.
         k8sconfig: K8sConfig
         local: SquareManifests
-            Should be output from `load_manifest` or `load`.
+            Should be output from `manio.load_manifests` or `manio.load`.
         server: SquareManifests
             Should be output from `manio.download`.
 
     Returns:
         `server` but possibly with some entries re-fetched from the same K8s
         endpoint that the equivalent resource in `local` specifies.
 
@@ -238,15 +238,15 @@
     NOTE: modifies `local` and `server` inplace.
 
     Inputs:
         config: Square configuration.
         plan_patch: List[MetaManifest]
             The list of meta manifests that currently require a patch.
         local: SquareManifests
-            Should be output from `load_manifest` or `load`.
+            Should be output from `manio.load_manifests` or `manio.load`.
         server: SquareManifests
             Should be output from `manio.download`.
 
     """
     # Do nothing and return immediately if the user did not provide a callback.
     cb = config.patch_callback
     if not cb:
@@ -274,25 +274,25 @@
 
 
 def compile_plan(
         config: Config,
         k8sconfig: K8sConfig,
         local: SquareManifests,
         server: SquareManifests) -> Tuple[DeploymentPlan, bool]:
-    """Return the `DeploymentPlan` to transition K8s to the `local` state.
+    """Return the `DeploymentPlan` that would propagate the `local` state to K8s.
 
     The deployment plan is a named tuple. It specifies which resources to
     create, patch and delete to ensure that the state of K8s matches that
     specified in `local`.
 
     Inputs:
         config: Square configuration.
         k8sconfig: K8sConfig
         local: SquareManifests
-            Should be output from `load_manifest` or `load`.
+            Should be output from `manio.load_manifests` or `manio.load`.
         server: SquareManifests
             Should be output from `manio.download`.
 
     Returns:
         DeploymentPlan
 
     """
@@ -725,14 +725,60 @@
             logit.error(f"Could not patch {msg_res}")
             return True
 
     # All good.
     return False
 
 
+def pick_manifests_for_plan(
+        local: SquareManifests,
+        server: SquareManifests,
+        selectors: Selectors) -> Tuple[SquareManifests, SquareManifests]:
+    """Return the subset of `local` and `server` that satisfy the `selectors`."""
+
+    # Compile the server manifests that match the selectors.
+    sel_local = {
+        meta: man for meta, man in local.items()
+        if manio.select(man, selectors, True)
+    }
+
+    # Compile the local manifests that match the selectors.
+    sel_server = {
+        meta: man for meta, man in server.items()
+        if manio.select(man, selectors, True)
+    }
+
+    # Every selected resource which exists both locally and on the server
+    # *must* be included in both `sel_{local, server}`.
+    #
+    # This is a subtle point: if a resource exists both locally and on the
+    # server then Square will plan a PATCH, as expected. However, if the
+    # resource has different labels locally than on the server, and those
+    # labels are part of the `Selectors`, then it is possible that only the
+    # local or server side resource makes it into `sel_{local,server}`. If that
+    # happens, Square will produce a plan that either CREATEs or DELETEs the
+    # resource because it thinks the manifest is missing on the server or
+    # locally, respectively. This will produce an error when Square applies the
+    # plan and tries to create a resource that already exists (happy case), or
+    # delete that resource from the server (probably not a happy case).
+    #
+    # To avoid this scenario, we will ensure that the intersection of selected
+    # local manifests and server manifests is included in the selected server
+    # manifests. Similarly, the intersection of all selected server manifests
+    # with the full set of local manifests must be included in the set of
+    # selected local manifests.
+    missing_sel_server = {_ for _ in sel_local if _ in server and _ not in sel_server}
+    sel_server |= {_: server[_] for _ in missing_sel_server}
+
+    missing_sel_local = {_ for _ in sel_server if _ in local and _ not in sel_local}
+    sel_local |= {_: local[_] for _ in missing_sel_local}
+
+    return sel_local, sel_server
+
+
 def make_plan(cfg: Config) -> Tuple[DeploymentPlan, bool]:
     """Return the deployment plan.
 
     Returns:
         Deployment plan.
 
     """
@@ -753,14 +799,20 @@
         local, _, err = manio.load_manifests(cfg.folder, cfg.selectors)
         assert not err
 
         # Download manifests from K8s.
         server, err = manio.download(cfg, k8sconfig)
         assert not err
 
+        # Retain only those manifests that satisfy the selectors.
+        # NOTE: we can already be certain that `local` and `server`
+        # contain only the desired resource KINDs and namespaces, but the label
+        # selectors have not been applied yet.
+        local, server = pick_manifests_for_plan(local, server, cfg.selectors)
+
         # Align non-plannable fields, like the ServiceAccount tokens.
         local_meta, err = manio.align_serviceaccount(local, server)
         assert not err
 
         # Create deployment plan.
         plan, err = compile_plan(cfg, k8sconfig, local_meta, server)
         assert not err and plan
```

### Comparing `kubernetes_square-1.5.0/square/yaml_io.py` & `kubernetes_square-1.5.1/square/yaml_io.py`

 * *Files identical despite different names*

