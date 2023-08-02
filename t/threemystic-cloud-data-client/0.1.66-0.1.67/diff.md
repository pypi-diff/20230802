# Comparing `tmp/threemystic_cloud_data_client-0.1.66.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.67.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.66.tar` & `threemystic_cloud_data_client-0.1.67.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    25671 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.66/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    19510 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    25671 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13576 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.67/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       *args, **kwargs)
   
   async def _process_account_data_region(self, account, region, resource_groups, loop, *args, **kwargs):
     pass
 
   def __init_costdata_month(self, data_dt, *args, **kwargs):
     return {
-      "currency": self.get_common().helper_type().string().set_case(self.get_cloud_data_client().get_default_currency(), case= "upper"),
+      "currency": self.get_common().helper_type().string().set_case(string_value= self.get_cloud_data_client().get_default_currency(), case= "upper"),
       "month": data_dt.month,
       "year": data_dt.year,
       "totals":{
         "total": Decimal(0),
         "fiscal_total": Decimal(0),
         "forcast_total": Decimal(0),
         "fiscal_forcast_total": Decimal(0),
@@ -37,15 +37,15 @@
         }
       },
       "days":{}
     }
   
   def __init_costdata_month_day(self, data_dt, currency, *args, **kwargs):
     return {
-      "currency": self.get_common().helper_type().string().set_case(self.get_cloud_data_client().get_default_currency(), case= "upper"),
+      "currency": self.get_common().helper_type().string().set_case(string_value= self.get_cloud_data_client().get_default_currency(), case= "upper"),
       "origional_currency": self.get_common().helper_type().string().set_case(string_value= currency, case= "upper"),
       "date": data_dt,
       "total": Decimal(0),
       "forcast_total": Decimal(0),
       "origional_currency_total": Decimal(0),
       "origional_currency_forcast_total": Decimal(0),
       "resource_group": {
@@ -58,25 +58,50 @@
         "total":{},
         "forcast_total":{},
         "origional_currency_total":{},
         "origional_currency_forcast_total":{},
       }
     }
   
+  def __convert_costmetric_forecast_metric(self, cost_metric, *args, **kwargs):
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "netunblendedcost":
+      return "NET_UNBLENDED_COST"
+    
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "blendedcost":
+      return "BLENDED_COST"
+    
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "unblendedcost":
+      return "UNBLENDED_COST"
+    
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "amortizedcost":
+      return "AMORTIZED_COST"
+    
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "netamortizedcost":
+      return "NET_AMORTIZED_COST"
+    
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "usagequantity":
+      return "USAGE_QUANTITY"
+    
+    if self.get_common().helper_type().string().set_case(string_value= cost_metric, case= "lower") == "normalizedusageamount":
+      return "NORMALIZED_USAGE_AMOUNT"
+    
+    return cost_metric
+
+
   async def __process_get_cost_data_process_forcast(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, cost_metrics, *args, **kwargs):
     
     for cost_metric in cost_metrics:
       results_by_time_forcast = self.get_cloud_client().general_boto_call_array(
         boto_call=lambda: client.get_cost_forecast(
           TimePeriod={
             'Start': start_date.strftime("%Y-%m-%d"),
             'End': end_date.strftime("%Y-%m-%d"),
           },
           Granularity='DAILY',
-          Metric=cost_metric,
+          Metric=self.__convert_costmetric_forecast_metric(cost_metric= cost_metric),
           Filter={
             "Dimensions":{
               "Key":"LINKED_ACCOUNT",
               "Values":[self.get_cloud_client().get_account_id(account= account)]
             }
           },
         ),
@@ -322,39 +347,39 @@
         dt_format= "%Y%m"
       )
       day_key = self.get_common().helper_type().datetime().datetime_as_string(
         dt= (self.get_data_start() - self.get_common().helper_type().datetime().time_delta(days= i)),
         dt_format= "%Y%m%d"
       )
 
-      if year_data[forcast_metric][month_key_last14]["days"].get(day_key) is None:
+      if year_data[cost_metric][month_key_last14]["days"].get(day_key) is None:
         continue
       
-      return_data["raw_last_14_days"][day_key] = year_data[forcast_metric][month_key_last14]["days"].get(day_key)
+      return_data["raw_last_14_days"][day_key] = year_data[cost_metric][month_key_last14]["days"].get(day_key)
 
       if day_count >= 7:
         continue
 
       day_count += 1
-      return_data["last_seven_days"] += year_data[forcast_metric][month_key_last14]["days"][day_key]["total"]
+      return_data["last_seven_days"] += year_data[cost_metric][month_key_last14]["days"][day_key]["total"]
       
-    for data in year_data[forcast_metric].values():
+    for data in year_data[cost_metric].values():
       return_data["fiscal_year_to_date"] += data["totals"].get("fiscal_total")
       return_data["fiscal_year_forecast"] += (data["totals"].get("fiscal_total") + data["totals"].get("fiscal_forcast_total"))
       if data["year"] == self.get_data_start().year:
         return_data["year_to_date"] += data["totals"].get("total")
         return_data["year_forecast"] += (data["totals"].get("total") + data["totals"].get("forcast_total"))
 
     
-    if year_data[forcast_metric].get(month_key) is not None:
-      return_data["month_to_date"] = year_data[forcast_metric][month_key]["totals"]["total"]
-      return_data["month_forecast"] = year_data[forcast_metric][month_key]["totals"]["total"] + year_data[forcast_metric][month_key]["totals"]["forcast_total"]
+    if year_data[cost_metric].get(month_key) is not None:
+      return_data["month_to_date"] = year_data[cost_metric][month_key]["totals"]["total"]
+      return_data["month_forecast"] = year_data[cost_metric][month_key]["totals"]["total"] + year_data[cost_metric][month_key]["totals"]["forcast_total"]
     
-    if year_data[forcast_metric].get(last_month_key) is not None:
-      return_data["last_month"] = year_data[forcast_metric][last_month_key]["totals"]["total"]
+    if year_data[cost_metric].get(last_month_key) is not None:
+      return_data["last_month"] = year_data[cost_metric][last_month_key]["totals"]["total"]
   
     return return_data
 
 
   async def _process_account_data(self, account, loop, *args, **kwargs):
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= kwargs.get("fiscal_year_start")):
       kwargs["fiscal_year_start"] = self.get_cloud_data_client().get_default_fiscal_year_start()
```

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.67/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/.gitignore` & `threemystic_cloud_data_client-0.1.67/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/LICENSE` & `threemystic_cloud_data_client-0.1.67/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/README.md` & `threemystic_cloud_data_client-0.1.67/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/hatch.toml` & `threemystic_cloud_data_client-0.1.67/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/pyproject.toml` & `threemystic_cloud_data_client-0.1.67/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.66/PKG-INFO` & `threemystic_cloud_data_client-0.1.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.66
+Version: 0.1.67
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

