# Comparing `tmp/kube_ops-1.0.6-py3-none-any.whl.zip` & `tmp/kube_ops-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19960 bytes, number of entries: 12
+Zip file size: 20047 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1664 b- defN 23-Jul-27 04:35 kube/__init__.py
--rw-r--r--  2.0 unx    38722 b- defN 23-Jul-30 06:28 kube/api.py
+-rw-r--r--  2.0 unx    38581 b- defN 23-Aug-02 04:25 kube/api.py
 -rw-r--r--  2.0 unx     2611 b- defN 23-Jul-23 07:44 kube/common.py
--rw-r--r--  2.0 unx     5086 b- defN 23-Jul-28 06:22 kube/config.py
+-rw-r--r--  2.0 unx     5471 b- defN 23-Aug-02 04:29 kube/config.py
 -rw-r--r--  2.0 unx     1400 b- defN 23-Jul-27 02:32 kube/enums.py
 -rw-r--r--  2.0 unx    19385 b- defN 23-Jul-28 06:40 kube/manifests.py
 -rw-r--r--  2.0 unx    11913 b- defN 23-Jul-27 04:49 kube/templates.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3374 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 23-Jul-30 09:17 kube_ops-1.0.6.dist-info/RECORD
-12 files, 86215 bytes uncompressed, 18494 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Aug-02 04:34 kube_ops-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3369 b- defN 23-Aug-02 04:34 kube_ops-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 04:34 kube_ops-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-02 04:34 kube_ops-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-Aug-02 04:34 kube_ops-1.0.7.dist-info/RECORD
+12 files, 86454 bytes uncompressed, 18581 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kube/manifests.py
 Comment: 
 
 Filename: kube/templates.py
 Comment: 
 
-Filename: kube_ops-1.0.6.dist-info/LICENSE
+Filename: kube_ops-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: kube_ops-1.0.6.dist-info/METADATA
+Filename: kube_ops-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: kube_ops-1.0.6.dist-info/WHEEL
+Filename: kube_ops-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: kube_ops-1.0.6.dist-info/top_level.txt
+Filename: kube_ops-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: kube_ops-1.0.6.dist-info/RECORD
+Filename: kube_ops-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kube/api.py

```diff
@@ -175,15 +175,14 @@
 
         :return: The new instance of Kube
         """
 
         conf = client.Configuration().get_default_copy()
         conf.host = host
         conf.api_key['authorization'] = token
-        conf.api_key_prefix['authorization'] = 'Bearer'
         conf.ssl_ca_cert = ca_cert_data
         if not ca_cert_data:
             conf.verify_ssl = False
 
         return KubeApi(namespace, conf)
 
     @property
@@ -458,17 +457,16 @@
             if check_err:
                 raise
 
             logging.error(e)
 
     def _list(self, func, **kwargs):
         ns = kwargs.pop('namespace', self._ns)
-        namespaced = kwargs.pop('namespaced', True)
 
-        return func(ns, **kwargs) if namespaced else func(**kwargs)
+        return func(ns, **kwargs)
 
     def _scale(self, func, name: str, replicas: int, wait: bool, **kwargs):
         """
         Scale down wrapper.
         """
         kwargs['body'] = {"spec": {"replicas": replicas}}
         resp = self._get(func, name, check_err=True, **kwargs)
@@ -684,14 +682,15 @@
                            **kwargs):
         """
         List all Custom Object API in current namespace.
         """
 
         args = [obj.group, obj.version, obj.plural]
         func = self.custom_object_api.list_cluster_custom_object
+
         if namespaced:
             ns = kwargs.pop('namespace', self._ns)
             args.insert(2, ns)
             func = self.custom_object_api.list_namespaced_custom_object
 
         return func(*args, **kwargs)
```

## kube/config.py

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import base64
 import hashlib
 import os
+import tempfile
 from pathlib import Path
 from urllib.parse import urlparse
 
 import yaml
 from kubernetes import client
 from kubernetes.config.incluster_config import SERVICE_HOST_ENV_NAME, SERVICE_PORT_ENV_NAME, SERVICE_CERT_FILENAME
 from urllib3.exceptions import MaxRetryError
@@ -65,34 +66,44 @@
 
         parsed_url = urlparse(server)
         if not parsed_url.port:
             server = f'https://{parsed_url.netloc}:443'
             parsed_url = urlparse(server)
 
         namespace = kwargs.get('namespace', 'default')
+        ca_cert_data = None
 
-        ca_cert = None
         try:
-            cm = KubeApi.from_token(server, token, namespace).configmap_get('kube-root-ca.crt', check_err=False)
-            if cm:
-                ca_cert = cm.data.get('ca.crt')
-        except MaxRetryError as e:
-            raise ValueError(e.reason)
-        except client.exceptions.ApiException as e:
-            if e.status == 401:
-                raise ValueError("The token provided is invalid or expired")
-
-            raise
+            ca_cert = kwargs.get('ca_cert')
+            if ca_cert:
+                with tempfile.NamedTemporaryFile(mode='w', delete=False) as f:
+                    f.write(ca_cert)
+                    ca_cert_data = f.name
+
+            try:
+                cm = KubeApi.from_token(
+                    server, token, namespace, ca_cert_data=ca_cert_data).configmap_get('kube-root-ca.crt')
+                if cm and not ca_cert:
+                    ca_cert = cm.data.get('ca.crt')
+            except MaxRetryError as e:
+                raise ValueError(e.reason)
+            except client.exceptions.ApiException as e:
+                if e.status == 401:
+                    raise ValueError("The token provided is invalid or expired")
+
+                raise
+        finally:
+            if ca_cert_data:
+                os.remove(ca_cert_data)
 
         tok = base64.b64encode(hashlib.sha256(token.encode()).digest()).decode()[:12]
 
         cluster_name = kwargs.get('cluster_name', f'{parsed_url.netloc.replace(".", "-")}')
         ctx_name = kwargs.get('context_name', f'{namespace}/{cluster_name}/token-{tok}')
         user = kwargs.get('user', f'token-{tok}/{cluster_name}')
-        ca_cert = kwargs.get('ca_cert', ca_cert)
         insecure_skip_tls_verify = kwargs.get('skip_tls_verify', False)
 
         if not insecure_skip_tls_verify and not ca_cert:
             raise ValueError('Add CA data or set `skip_tls_verify=True`')
 
         cluster = {"server": server}
         if insecure_skip_tls_verify:
```

## Comparing `kube_ops-1.0.6.dist-info/LICENSE` & `kube_ops-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kube_ops-1.0.6.dist-info/METADATA` & `kube_ops-1.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-ops
-Version: 1.0.6
+Version: 1.0.7
 Summary: Kubernetes OOP
 Author-email: myback <54638513+myback@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 myback.space
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 ```python
 import kube
 
 # Make container
 container = kube.Container('nginx')
 container.set_image('nginx:alpine')
 
-# Add environment variables to from configmap
+# Add environment variables to configmap
 ## Make configmap
 cm = kube.ConfigMap('nginx')
 cm.set_data(NGINX_ENTRYPOINT_QUIET_LOGS='true')
 
 ## Make env from configmap
 env = kube.env_from_configmap(cm.name)
 container.add_env_from(env)
```

## Comparing `kube_ops-1.0.6.dist-info/RECORD` & `kube_ops-1.0.7.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 kube/__init__.py,sha256=Af0Oy_7_RNbsxihJ6BasxE6Cno70jrB8wuxkALgyUJw,1664
-kube/api.py,sha256=xPgKGTySYw7LycZ5y58Rc7j2dQ_bCflR0RPimq0Cs2E,38722
+kube/api.py,sha256=LrwdtTRNybi5aLxlbnF-greC2BjUl3VKF4pw2nxOU6U,38581
 kube/common.py,sha256=XRpVZJz700HSeErD7gFc1dWzT5GQlrhB1jEuxQ48N0Q,2611
-kube/config.py,sha256=aJhAQVvIUfZpBoF1pzQEb0ArY4LbbnnbjqqErVr43o0,5086
+kube/config.py,sha256=4I0swwzhhbNRepoexcSpBgVNIQ36BIJKi4TN1ymSdvc,5471
 kube/enums.py,sha256=a2UVx-KXe6GM_m3UTwEZHQNkFzMfgZLPG1S-CXTl-WU,1400
 kube/manifests.py,sha256=dE7qRvJ7Cz9TsMWcCgW_kh-0W0PKL60nt9GowyWr5Vk,19385
 kube/templates.py,sha256=dCNye1Ew8LSE_3cOu_dOT4A8ZBS7h_KkD0NzKf2VBZ8,11913
-kube_ops-1.0.6.dist-info/LICENSE,sha256=4UMudA3MzI411FVQKHbbLdnwm2GjFrbv5LBNk5ZTT8Y,1069
-kube_ops-1.0.6.dist-info/METADATA,sha256=FGZvILE4DoPbJT6ZDzYDEzL5kLNQp4PchBnR82AEuUw,3374
-kube_ops-1.0.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-kube_ops-1.0.6.dist-info/top_level.txt,sha256=VviGlBjAU4SlS_NC5yQCpy0uOZb8yzwuA9KQU4Tvrgc,5
-kube_ops-1.0.6.dist-info/RECORD,,
+kube_ops-1.0.7.dist-info/LICENSE,sha256=4UMudA3MzI411FVQKHbbLdnwm2GjFrbv5LBNk5ZTT8Y,1069
+kube_ops-1.0.7.dist-info/METADATA,sha256=J-vQM9yVI9mBuib_ouU6oBpbYh7BEHAk4hefi_Chwas,3369
+kube_ops-1.0.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+kube_ops-1.0.7.dist-info/top_level.txt,sha256=VviGlBjAU4SlS_NC5yQCpy0uOZb8yzwuA9KQU4Tvrgc,5
+kube_ops-1.0.7.dist-info/RECORD,,
```

