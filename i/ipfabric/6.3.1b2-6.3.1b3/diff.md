# Comparing `tmp/ipfabric-6.3.1b2.tar.gz` & `tmp/ipfabric-6.3.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.3.1b2.tar", max compression
+gzip compressed data, was "ipfabric-6.3.1b3.tar", max compression
```

## Comparing `ipfabric-6.3.1b2.tar` & `ipfabric-6.3.1b3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1498 2023-07-17 15:20:24.288289 ipfabric-6.3.1b2/ipfabric/__init__.py
--rw-r--r--   0        0        0    17287 2023-07-17 15:20:24.293213 ipfabric-6.3.1b2/ipfabric/api.py
--rw-r--r--   0        0        0    11597 2023-07-14 16:09:22.706505 ipfabric-6.3.1b2/ipfabric/client.py
--rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.3.1b2/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    14821 2023-07-13 12:33:49.973872 ipfabric-6.3.1b2/ipfabric/models/device.py
--rw-r--r--   0        0        0     5842 2023-06-01 16:01:19.099648 ipfabric-6.3.1b2/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-04-24 14:44:33.818272 ipfabric-6.3.1b2/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2219 2023-07-17 12:44:51.298382 ipfabric-6.3.1b2/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     6964 2023-07-13 12:33:49.979894 ipfabric-6.3.1b2/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    12421 2023-07-13 12:33:49.985397 ipfabric-6.3.1b2/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    25472 2023-07-17 15:20:24.297305 ipfabric-6.3.1b2/ipfabric/models/table.py
--rw-r--r--   0        0        0     2988 2023-07-17 15:01:32.974051 ipfabric-6.3.1b2/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-04-24 14:44:33.821325 ipfabric-6.3.1b2/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-04-24 14:44:33.822322 ipfabric-6.3.1b2/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-04-24 14:44:33.822322 ipfabric-6.3.1b2/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-04-24 14:44:33.822322 ipfabric-6.3.1b2/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-04-24 14:44:33.823320 ipfabric-6.3.1b2/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-04-24 14:44:33.823320 ipfabric-6.3.1b2/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-04-24 14:44:33.823320 ipfabric-6.3.1b2/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-04-24 14:44:33.824322 ipfabric-6.3.1b2/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-04-24 14:44:33.824322 ipfabric-6.3.1b2/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-04-24 14:44:33.825321 ipfabric-6.3.1b2/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-04-24 14:44:33.825321 ipfabric-6.3.1b2/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-04-24 14:44:33.826320 ipfabric-6.3.1b2/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1076 2023-07-17 12:44:51.298382 ipfabric-6.3.1b2/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     5549 2023-07-17 12:44:51.299382 ipfabric-6.3.1b2/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2158 2023-07-17 12:44:51.299382 ipfabric-6.3.1b2/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-04-24 14:44:33.827321 ipfabric-6.3.1b2/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-04-24 14:44:33.828325 ipfabric-6.3.1b2/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2094 2023-07-17 12:44:51.300385 ipfabric-6.3.1b2/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-04-24 14:44:33.829324 ipfabric-6.3.1b2/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-04-24 14:44:33.829324 ipfabric-6.3.1b2/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.3.1b2/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3342 2023-07-13 12:33:49.997188 ipfabric-6.3.1b2/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.3.1b2/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.3.1b2/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.3.1b2/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.3.1b2/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.3.1b2/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     5137 2023-07-13 12:33:50.002187 ipfabric-6.3.1b2/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.3.1b2/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-04-24 14:44:33.870769 ipfabric-6.3.1b2/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.3.1b2/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-04-24 14:44:33.876769 ipfabric-6.3.1b2/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.3.1b2/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125000 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125000 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/dashboard.json
--rw-r--r--   0        0        0     5852 2023-07-14 17:28:19.475539 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/groups.json
--rw-r--r--   0        0        0   122055 2023-07-14 17:21:35.755499 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-24 14:44:33.881459 ipfabric-6.3.1b2/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     6141 2023-07-14 16:43:51.555959 ipfabric-6.3.1b2/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-04-24 14:44:33.891098 ipfabric-6.3.1b2/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-04-24 14:44:33.895102 ipfabric-6.3.1b2/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-04-24 14:44:33.902766 ipfabric-6.3.1b2/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.3.1b2/LICENSE
--rw-r--r--   0        0        0     2020 2023-07-17 15:20:49.946414 ipfabric-6.3.1b2/pyproject.toml
--rw-r--r--   0        0        0     3951 2023-07-17 15:20:24.284079 ipfabric-6.3.1b2/README.md
--rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 ipfabric-6.3.1b2/setup.py
--rw-r--r--   0        0        0     5423 1970-01-01 00:00:00.000000 ipfabric-6.3.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-31 14:49:28.256233 ipfabric-6.3.1b3/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17790 2023-08-02 15:14:42.097610 ipfabric-6.3.1b3/ipfabric/api.py
+-rw-r--r--   0        0        0    19570 2023-08-02 18:27:43.591322 ipfabric-6.3.1b3/ipfabric/client.py
+-rw-r--r--   0        0        0      434 2023-06-01 16:01:19.090676 ipfabric-6.3.1b3/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    15519 2023-08-02 18:51:49.825841 ipfabric-6.3.1b3/ipfabric/models/device.py
+-rw-r--r--   0        0        0     6287 2023-07-31 14:49:28.274772 ipfabric-6.3.1b3/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.3.1b3/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2226 2023-07-31 14:49:28.277738 ipfabric-6.3.1b3/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     6971 2023-07-31 14:49:28.278744 ipfabric-6.3.1b3/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12577 2023-07-31 14:59:33.102173 ipfabric-6.3.1b3/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    33123 2023-08-02 18:27:43.646232 ipfabric-6.3.1b3/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2993 2023-07-31 14:49:28.305092 ipfabric-6.3.1b3/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-31 14:49:28.307092 ipfabric-6.3.1b3/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      495 2023-07-31 14:49:28.308090 ipfabric-6.3.1b3/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2180 2023-07-31 14:49:28.309091 ipfabric-6.3.1b3/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1009 2023-07-31 14:49:28.310091 ipfabric-6.3.1b3/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7025 2023-07-31 14:49:28.312091 ipfabric-6.3.1b3/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      331 2023-07-31 14:49:28.313091 ipfabric-6.3.1b3/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      850 2023-07-31 14:49:28.314101 ipfabric-6.3.1b3/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      477 2023-07-31 14:49:28.315096 ipfabric-6.3.1b3/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5651 2023-07-31 14:49:28.317095 ipfabric-6.3.1b3/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2052 2023-07-31 14:49:28.318098 ipfabric-6.3.1b3/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2790 2023-07-31 14:49:28.319105 ipfabric-6.3.1b3/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      766 2023-07-31 14:49:28.320102 ipfabric-6.3.1b3/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      640 2023-07-31 14:49:28.321101 ipfabric-6.3.1b3/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3536 2023-07-31 14:49:28.322108 ipfabric-6.3.1b3/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1238 2023-07-31 14:49:28.323103 ipfabric-6.3.1b3/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1083 2023-07-31 14:49:28.325090 ipfabric-6.3.1b3/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     5556 2023-07-31 14:49:28.326098 ipfabric-6.3.1b3/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2165 2023-07-31 14:49:28.327090 ipfabric-6.3.1b3/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      438 2023-07-31 14:49:28.328091 ipfabric-6.3.1b3/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2069 2023-07-31 14:49:28.329423 ipfabric-6.3.1b3/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2101 2023-07-31 14:49:28.330448 ipfabric-6.3.1b3/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      863 2023-07-31 14:49:28.331452 ipfabric-6.3.1b3/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      874 2023-07-31 14:49:28.332447 ipfabric-6.3.1b3/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.3.1b3/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-31 14:49:28.333893 ipfabric-6.3.1b3/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-04-24 14:44:33.840110 ipfabric-6.3.1b3/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8814 2023-07-31 14:49:28.334917 ipfabric-6.3.1b3/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.3.1b3/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.3.1b3/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-04-24 14:44:33.844128 ipfabric-6.3.1b3/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5171 2023-07-31 14:59:33.103174 ipfabric-6.3.1b3/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-04-24 14:44:33.866077 ipfabric-6.3.1b3/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6335 2023-07-31 14:49:28.347932 ipfabric-6.3.1b3/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      459 2023-07-31 14:49:28.349931 ipfabric-6.3.1b3/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7900 2023-07-31 14:49:28.350933 ipfabric-6.3.1b3/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.3.1b3/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2023-07-31 14:05:50.920368 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/__init__.py
+-rw-r--r--   0        0        0     3152 2023-07-31 14:05:50.920368 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/dashboard.json
+-rw-r--r--   0        0        0     5852 2023-07-31 14:05:50.920368 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/groups.json
+-rw-r--r--   0        0        0   122055 2023-07-31 14:05:50.922363 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4509 2023-07-31 14:49:28.352932 ipfabric-6.3.1b3/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     6141 2023-07-31 14:05:50.934362 ipfabric-6.3.1b3/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0    21216 2023-07-31 14:49:28.354943 ipfabric-6.3.1b3/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2431 2023-07-31 14:49:28.355937 ipfabric-6.3.1b3/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2594 2023-07-31 14:49:28.356942 ipfabric-6.3.1b3/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.3.1b3/LICENSE
+-rw-r--r--   0        0        0     2182 2023-08-02 19:25:53.642742 ipfabric-6.3.1b3/pyproject.toml
+-rw-r--r--   0        0        0     6515 2023-08-02 15:08:15.750226 ipfabric-6.3.1b3/README.md
+-rw-r--r--   0        0        0     8380 1970-01-01 00:00:00.000000 ipfabric-6.3.1b3/setup.py
+-rw-r--r--   0        0        0     8126 1970-01-01 00:00:00.000000 ipfabric-6.3.1b3/PKG-INFO
```

### Comparing `ipfabric-6.3.1b2/ipfabric/__init__.py` & `ipfabric-6.3.1b3/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/api.py` & `ipfabric-6.3.1b3/ipfabric/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import Optional, Union, Dict, List, Generator, Any
 from urllib.parse import urljoin
 from uuid import UUID
 
 import dotenv
 import httpx
 from httpx import Client, URL
-from pydantic import BaseSettings, validator
+from pydantic import field_validator
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from ipfabric.models import Snapshot, SNAPSHOT_COLUMNS
 from ipfabric.settings.user_mgmt import User
 
 logger = logging.getLogger("ipfabric")
 
 LAST_ID, PREV_ID, LASTLOCKED_ID = "$last", "$prev", "$lastLocked"
@@ -35,47 +36,44 @@
                 resp.raise_for_status()  # Response updates accessToken in shared CookieJar
                 request.headers["Cookie"] = "accessToken=" + self.client.cookies["accessToken"]  # Update request
                 yield request
         return response
 
 
 class Settings(BaseSettings):
-    ipf_url: Optional[str]
-    ipf_version: Optional[Union[int, float, str]]
-    ipf_token: Optional[str]
-    ipf_username: Optional[str]
-    ipf_password: Optional[str]
-    ipf_snapshot: Optional[str]
-    ipf_verify: Union[bool, str] = True
-    ipf_timeout: Optional[float] = None
-
-    @validator("ipf_version")
-    def _valid_version(cls, v):
-        if v is None:
-            return v
+    model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8", env_prefix="ipf_")
+    url: Optional[str] = None
+    version: Optional[Union[int, float, str]] = None
+    token: Optional[str] = None
+    username: Optional[str] = None
+    password: Optional[str] = None
+    snapshot: Optional[str] = None
+    verify: Union[bool, str] = True
+    timeout: Optional[float] = None
+
+    @field_validator("version")
+    @classmethod
+    def _valid_version(cls, v: Union[None, int, float, str]) -> Union[None, str]:
         if v and isinstance(v, (int, float)):
             v = "v" + str(v)
-        if re.match(r"v\d(\.\d)?", v) or not v:
+        if not v or re.match(r"v\d(\.\d)?", v):
             return v
         else:
             raise ValueError(f"IPF_VERSION ({v}) is not valid, must be like `v#` or `v#.#`.")
 
-    @validator("ipf_snapshot")
-    def _valid_snapshot(cls, v):
+    @field_validator("snapshot")
+    @classmethod
+    def _valid_snapshot(cls, v: Union[None, str]) -> Union[None, str]:
         if v is None or v in VALID_REFS:
             return v
         elif re.match(r"^[\da-f]{8}-([\da-f]{4}-){3}[\da-f]{12}$", v.lower()):
             return v.lower()
         else:
             raise ValueError(f"IPF_SNAPSHOT ({v}) is not valid, must be a UUID or one of {VALID_REFS}.")
 
-    class Config:
-        env_file = ".env"
-        env_file_encoding = "utf-8"
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Needed for context"""
         pass
 
@@ -96,43 +94,44 @@
             base_url: IP Fabric instance provided in 'base_url' parameter, or the 'IPF_URL' environment variable
             api_version: [Optional] Version of IP Fabric API
             auth: API token, tuple (username, password), or custom Auth to pass to httpx
             snapshot_id: IP Fabric snapshot ID to use by default for database actions - defaults to '$last'
             unloaded: True to load metadata from unloaded snapshots
             **kwargs: Keyword args to pass to httpx
         """
-        if {kwargs.get(i, None) for i in ["token", "username", "password"]} != {None}:
+        if {kwargs.get(i, None) for i in ["token", "username", "password"]} != {None}:  # TODO: Remove v7.0
             logger.warning(
                 "Use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` authentication will be deprecated "
                 "in v7.0.X, please use `auth='<TOKEN>'` or `auth=('<USER>','<PASS>')` instead.\n"
                 "This does not apply to .env file or environment variables (IPF_TOKEN, IPF_USERNAME, IPF_PASSWORD).\n"
                 "This is to support custom authentication methods that will be passed directly to HTTPX."
             )
         self.unloaded = unloaded
         # find env file
         dotenv.load_dotenv(dotenv.find_dotenv())
         with Settings() as settings:
             cookie_jar = CookieJar()
             super().__init__(
                 cookies=cookie_jar,
-                **self._httpx_kwargs(kwargs, kwargs.get("verify", settings.ipf_verify), settings.ipf_timeout),
+                headers={"User-Agent": f'python-ipfabric-sdk/{metadata.version("ipfabric")}'},
+                **self._httpx_kwargs(kwargs, kwargs.get("verify", settings.verify), settings.timeout),
             )
-            base_url = base_url or settings.ipf_url
+            base_url = base_url or settings.url
             if not base_url:
                 raise RuntimeError("IP Fabric base_url not provided or IPF_URL not set")
 
-            self.api_version, self.os_version = self.check_version(api_version or settings.ipf_version, base_url)
+            self.api_version, self.os_version = self.check_version(api_version or settings.version, base_url)
             self.base_url = urljoin(base_url, f"api/{self.api_version}/")
-            snapshot_id = snapshot_id or settings.ipf_snapshot
+            snapshot_id = snapshot_id or settings.snapshot
             if auth:
                 token, username, password = None, None, None
             else:
-                token = kwargs.get("token", settings.ipf_token)  # TODO: Update this in v7.0
-                username = kwargs.get("username", settings.ipf_username)
-                password = kwargs.get("password", settings.ipf_password)
+                token = kwargs.get("token", settings.token)  # TODO: Update this in v7.0
+                username = kwargs.get("username", settings.username)
+                password = kwargs.get("password", settings.password)
 
         if token:
             self._login(token)
         elif username and password:
             self._login((username, password), base_url=base_url, cookie_jar=cookie_jar)
         else:
             self._login(auth, base_url=base_url, cookie_jar=cookie_jar)  # TODO: Keep only this in v7.0
@@ -309,15 +308,17 @@
         else:
             self._snapshot_id = self.snapshots[snapshot_id].snapshot_id
 
     def get_snapshot(self, snapshot_id: str):
         if snapshot_id in self.snapshots:
             return self.snapshots[snapshot_id]
         else:
-            payload = {"columns": SNAPSHOT_COLUMNS, "filters": {"id": ["eq", snapshot_id]}}
+            if self.api_version < "v6.3":  # TODO: Remove v7.0
+                SNAPSHOT_COLUMNS.discard("creatorUsername")
+            payload = {"columns": list(SNAPSHOT_COLUMNS), "filters": {"id": ["eq", snapshot_id]}}
             results = self._ipf_pager("tables/management/snapshots", payload)
             if not results:
                 logger.error(f"Snapshot {snapshot_id} not found.")
                 return None
             get_results = self._get_snapshots()
             snapshot = self._create_snapshot_model(results[0], get_results)
             if snapshot.loaded:
@@ -367,20 +368,22 @@
         initialVersion
         """
         res = self.get("/snapshots")
         res.raise_for_status()
         return {s["id"]: s for s in res.json()}
 
     def get_snapshots(self) -> Dict[str, Snapshot]:
-        """Gets all snapshots from IP Fabric and returns a dictionary of {ID:   Snapshot_info}
+        """Gets all snapshots from IP Fabric and returns a dictionary of {ID: Snapshot_info}
 
         Returns:
             Dictionary with ID as key and dictionary with info as the value
         """
-        payload = {"columns": SNAPSHOT_COLUMNS, "sort": {"order": "desc", "column": "tsEnd"}}
+        if self.api_version < "v6.3":  # TODO: Remove v7.0
+            SNAPSHOT_COLUMNS.discard("creatorUsername")
+        payload = {"columns": list(SNAPSHOT_COLUMNS), "sort": {"order": "desc", "column": "tsEnd"}}
         if not self.unloaded:
             logger.warning("Retrieving only loaded snapshots. To load all snapshots set `unloaded` to True.")
             payload["filters"] = {"and": [{"status": ["eq", "done"]}, {"finishStatus": ["eq", "done"]}]}
         results = self._ipf_pager("tables/management/snapshots", payload)
         get_results = self._get_snapshots()
 
         snap_dict = OrderedDict()
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/device.py` & `ipfabric-6.3.1b3/ipfabric/models/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,65 +17,70 @@
 
 
 logger = logging.getLogger("ipfabric")
 
 
 class DeviceConfig(BaseModel):
     status: str
-    current: Optional[str] = Field(alias="currentConfig")
-    start: Optional[str] = Field(alias="startupConfig")
+    current: Optional[str] = Field(None, alias="currentConfig")
+    start: Optional[str] = Field(None, alias="startupConfig")
 
 
 class Device(BaseModel):
-    attributes: dict
-    domain: Optional[str]
-    family: Optional[str]
-    fqdn: Optional[str]
+    attributes: Optional[dict] = None
+    global_attributes: Optional[dict] = None
+    domain: Optional[str] = None
+    family: Optional[str] = None
+    fqdn: Optional[str] = None
     hostname: str
-    image: Optional[str]
-    model: Optional[str]
-    platform: Optional[str]
-    processor: Optional[str]
-    reload: Optional[str]
+    image: Optional[str] = None
+    model: Optional[str] = None
+    platform: Optional[str] = None
+    processor: Optional[str] = None
+    reload: Optional[str] = None
     sn: str
-    uptime: Optional[timedelta]
+    uptime: Optional[timedelta] = None
     vendor: str
     version: str
-    blob_key: Optional[str] = Field(alias="blobKey")
-    config_reg: Optional[str] = Field(alias="configReg")
-    dev_type: str = Field(alias="devType")
-    hostname_original: Optional[str] = Field(alias="hostnameOriginal")
-    hostname_processed: Optional[str] = Field(alias="hostnameProcessed")
-    login_ip: Optional[IPv4Interface] = Field(alias="loginIp")
-    login_type: str = Field(alias="loginType")
-    mem_total_bytes: Optional[float] = Field(alias="memoryTotalBytes")
-    mem_used_bytes: Optional[float] = Field(alias="memoryUsedBytes")
-    mem_utilization: Optional[float] = Field(alias="memoryUtilization")
-    object_id: Optional[str] = Field(alias="objectId")
-    routing_domain: Optional[int] = Field(alias="rd")
-    site: str = Field(alias="siteName")
-    sn_hw: str = Field(alias="snHw")
-    stp_domain: Optional[int] = Field(alias="stpDomain")
-    task_key: Optional[str] = Field(alias="taskKey")
+    blob_key: Optional[str] = Field(None, alias="blobKey")
+    config_reg: Optional[str] = Field(None, alias="configReg")
+    dev_type: str = Field(None, alias="devType")
+    hostname_original: Optional[str] = Field(None, alias="hostnameOriginal")
+    hostname_processed: Optional[str] = Field(None, alias="hostnameProcessed")
+    login_ip: Optional[IPv4Interface] = Field(None, alias="loginIp")
+    login_type: str = Field(None, alias="loginType")
+    mem_total_bytes: Optional[float] = Field(None, alias="memoryTotalBytes")
+    mem_used_bytes: Optional[float] = Field(None, alias="memoryUsedBytes")
+    mem_utilization: Optional[float] = Field(None, alias="memoryUtilization")
+    object_id: Optional[str] = Field(None, alias="objectId")
+    routing_domain: Optional[int] = Field(None, alias="rd")
+    site: str = Field(None, alias="siteName")
+    sn_hw: str = Field(None, alias="snHw")
+    stp_domain: Optional[int] = Field(None, alias="stpDomain")
+    task_key: Optional[str] = Field(None, alias="taskKey")
 
     def __repr__(self):
         return self.hostname
 
     def __str__(self):
         return self.hostname
 
     def __eq__(self, other):
         return self.sn == other.sn if isinstance(other, Device) else str(other)
 
     def __hash__(self):
         return hash(self.sn)
 
+    @property
+    def local_attributes(self):
+        return self.attributes
+
     @classmethod
     def check_attribute(cls, attribute) -> True:
-        if attribute not in cls.__fields__:
+        if attribute not in cls.model_fields:
             raise AttributeError(f"Attribute {attribute} not in Device class.")
         return True
 
     def get_log_file(self, client: IPFClient) -> str:
         res = client.get("/os/logs/task/" + self.task_key)
         res.raise_for_status()
         return res.text
@@ -217,24 +222,37 @@
         Device.check_attribute(attribute)
         return Devices.group_dev_by_attr(self._flatten_devs(), attribute).regex(pattern, *flags)
 
 
 class Devices(BaseModel):
     snapshot_id: str
     _attrs: Optional[DefaultDict[str, Set[str]]] = PrivateAttr()
+    _global_attrs: Optional[DefaultDict[str, Set[str]]] = PrivateAttr()
     _all: List[Device] = PrivateAttr()
 
     def __init__(
-        self, snapshot_id: str, devices: List[dict], attributes: List[dict] = None, blob_keys: List[dict] = None
+        self,
+        snapshot_id: str,
+        devices: List[dict],
+        attributes: List[dict] = None,
+        global_attributes: List[dict] = None,
+        blob_keys: List[dict] = None,
     ):
         super().__init__(snapshot_id=snapshot_id)
-        self._attrs, dev_attr = self._parse_attrs(attributes)
+        self._attrs, lcl_attr = self._parse_attrs(attributes)
+        self._global_attrs, glb_attr = self._parse_attrs(global_attributes)
         blob_keys = {b["sn"]: b["blobKey"] for b in blob_keys} if blob_keys else dict()
         self._all = [
-            Device(**d, attributes=dev_attr.get(d["sn"], dict()), blobKey=blob_keys.get(d["sn"], None)) for d in devices
+            Device(
+                **d,
+                attributes=lcl_attr.get(d["sn"], dict()),
+                global_attributes=glb_attr.get(d["sn"], dict()),
+                blobKey=blob_keys.get(d["sn"], None),
+            )
+            for d in devices
         ]
 
     @staticmethod
     def _parse_attrs(attributes: List[dict] = None):
         if not attributes:
             return None, dict()
         cls_attr, dev_attr = defaultdict(set), defaultdict(dict)
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/intent.py` & `ipfabric-6.3.1b3/ipfabric/models/intent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from collections import defaultdict
 from typing import Any, Union, List
 
 from httpx import HTTPStatusError
 
 from .intent_check import Group, IntentCheck
 
 logger = logging.getLogger("ipfabric")
@@ -78,14 +79,26 @@
         return {c.intent_id: c for c in self.intent_checks}
 
     @property
     def intent_by_name(self):
         return {c.name: c for c in self.intent_checks}
 
     @property
+    def intent_ids_by_web_endpoint(self):
+        reports = defaultdict(list)
+        [reports[c.web_endpoint].append(c.intent_id) for c in self.intent_checks]
+        return reports
+
+    @property
+    def intent_ids_by_api_endpoint(self):
+        reports = defaultdict(list)
+        [reports[c.api_endpoint].append(c.intent_id) for c in self.intent_checks]
+        return reports
+
+    @property
     def group_by_id(self):
         return {g.group_id: g for g in self.groups}
 
     @property
     def group_by_name(self):
         return {g.name: g for g in self.groups}
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/intent_check.py` & `ipfabric-6.3.1b3/ipfabric/models/intent_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 from pydantic import BaseModel, Field
 
 
 class Checks(BaseModel):
     """model for intent checks"""
 
-    green: Union[int, str, dict] = Field(alias="0", default=None)
-    blue: Union[int, str, dict] = Field(alias="10", default=None)
-    amber: Union[int, str, dict] = Field(alias="20", default=None)
-    red: Union[int, str, dict] = Field(alias="30", default=None)
+    green: Union[int, str, dict] = Field(None, alias="0")
+    blue: Union[int, str, dict] = Field(None, alias="10")
+    amber: Union[int, str, dict] = Field(None, alias="20")
+    red: Union[int, str, dict] = Field(None, alias="30")
 
 
 class CheckResults(Checks):
     """model for intent check results"""
 
-    nan: Union[int, str, dict] = Field(alias="-1", default=None)
+    nan: Union[int, str, dict] = Field(None, alias="-1")
 
 
 class Description(BaseModel):
     """model for description of intent check"""
 
-    general: Union[None, str]
+    general: Union[None, str] = None
     checks: Checks = Field(default_factory=Checks)
 
 
 class Result(BaseModel):
     """model for results of intent check"""
 
-    count: Union[int, None]
+    count: Union[int, None] = None
     checks: Checks = Field(default_factory=Checks)
 
     def compare(self, other: "Result") -> dict:
         """
 
         Args:
             other: intent check
@@ -63,35 +63,35 @@
         return int((getattr(data, value) if data else 0) or 0)
 
 
 class Child(BaseModel):
     """model for child of intent check"""
 
     weight: int
-    intent_id: str = Field(alias="id")
+    intent_id: str = Field(None, alias="id")
 
 
 class Group(BaseModel):
     """model of a group of intent checks"""
 
     custom: bool
     name: str
-    group_id: str = Field(alias="id")
+    group_id: str = Field(None, alias="id")
     children: List[Child] = Field(default_factory=list)
 
 
 class IntentCheck(BaseModel):
     """model for intent checks"""
 
     groups: List[Group]
     checks: Checks
     column: str
     custom: bool
     descriptions: Description
     name: str
     status: int
     result: Result
-    api_endpoint: str = Field(alias="apiEndpoint")
-    default_color: Union[None, int] = Field(alias="defaultColor")
-    web_endpoint: str = Field(alias="webEndpoint")
-    intent_id: str = Field(alias="id")
+    api_endpoint: str = Field(None, alias="apiEndpoint")
+    default_color: Union[None, int] = Field(None, alias="defaultColor")
+    web_endpoint: str = Field(None, alias="webEndpoint")
+    intent_id: str = Field(None, alias="id")
     result_data: Optional[CheckResults] = Field(default_factory=CheckResults)
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/inventory.py` & `ipfabric-6.3.1b3/ipfabric/models/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 IGNORE_COLUMNS = {"id"}
 
 
 class Inventory(BaseModel):
     """model for inventories"""
 
-    client: Any
+    client: Any = None
 
     @property
     def sites(self):
         return Table(client=self.client, endpoint="tables/inventory/sites")
 
     @property
     def vendors(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/jobs.py` & `ipfabric-6.3.1b3/ipfabric/models/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .table import BaseTable
 
 logger = logging.getLogger("ipfabric")
 
 
 class Jobs(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def all_jobs(self):
         return BaseTable(client=self.client, endpoint="tables/jobs")
 
     @property
     def columns(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/snapshot.py` & `ipfabric-6.3.1b3/ipfabric/models/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pathlib import Path
 
 from pydantic import BaseModel, Field
 from .jobs import Jobs
 
 logger = logging.getLogger("ipfabric")
 
-SNAPSHOT_COLUMNS = [
+SNAPSHOT_COLUMNS = {
     "id",
     "creatorUsername",
     "status",
     "finishStatus",
     "loadedSize",
     "unloadedSize",
     "name",
@@ -37,63 +37,63 @@
     "interfaceEdgeCount",
     "totalDevCount",
     "isLastSnapshot",
     "tsChange",
     "tsEnd",
     "tsStart",
     "userCount",
-]
+}
 
 
 def snapshot_upload(ipf: IPFClient, filename: str):
     data = {"file": (Path(filename).name, open(filename, "rb"), "application/x-tar")}
     resp = ipf.post("snapshots/upload", files=data)
     if resp.status_code == 400:
         if resp.json()["code"] == "API_SNAPSHOT_CONFLICT":
             logger.warning(f"SNAPSHOT ID {resp.json()['data']['snapshot']} already uploaded")
             return
     resp.raise_for_status()
     return resp.json()
 
 
 class Error(BaseModel):
-    error_type: str = Field(alias="errorType")
+    error_type: str = Field(None, alias="errorType")
     count: int
 
 
 class Snapshot(BaseModel):
-    snapshot_id: str = Field(alias="id")
-    name: Optional[str]
-    note: Optional[str]
-    creator_username: Optional[str] = Field(alias="creatorUsername")
-    total_dev_count: int = Field(alias="totalDevCount")
-    licensed_dev_count: Optional[int] = Field(alias="licensedDevCount")
-    user_count: int = Field(alias="userCount")
-    interface_active_count: int = Field(alias="interfaceActiveCount")
-    interface_count: int = Field(alias="interfaceCount")
-    interface_edge_count: int = Field(alias="interfaceEdgeCount")
-    device_added_count: int = Field(alias="deviceAddedCount")
-    device_removed_count: int = Field(alias="deviceRemovedCount")
+    snapshot_id: str = Field(None, alias="id")
+    name: Optional[str] = None
+    note: Optional[str] = None
+    creator_username: Optional[str] = Field(None, alias="creatorUsername")
+    total_dev_count: int = Field(None, alias="totalDevCount")
+    licensed_dev_count: Optional[int] = Field(None, alias="licensedDevCount")
+    user_count: int = Field(None, alias="userCount")
+    interface_active_count: int = Field(None, alias="interfaceActiveCount")
+    interface_count: int = Field(None, alias="interfaceCount")
+    interface_edge_count: int = Field(None, alias="interfaceEdgeCount")
+    device_added_count: int = Field(None, alias="deviceAddedCount")
+    device_removed_count: int = Field(None, alias="deviceRemovedCount")
     status: str
-    finish_status: str = Field(alias="finishStatus")
+    finish_status: str = Field(None, alias="finishStatus")
     loading: bool
     locked: bool
-    from_archive: bool = Field(alias="fromArchive")
-    start: datetime = Field(alias="tsStart")
-    end: Optional[datetime] = Field(alias="tsEnd")
-    change: Optional[datetime] = Field(alias="tsChange")
+    from_archive: bool = Field(None, alias="fromArchive")
+    start: datetime = Field(None, alias="tsStart")
+    end: Optional[datetime] = Field(None, alias="tsEnd")
+    change: Optional[datetime] = Field(None, alias="tsChange")
     version: Optional[str] = None
-    initial_version: Optional[str] = Field(alias="initialVersion")
+    initial_version: Optional[str] = Field(None, alias="initialVersion")
     sites: List[str]
-    errors: Optional[List[Error]]
-    loaded_size: int = Field(alias="loadedSize")
-    unloaded_size: int = Field(alias="unloadedSize")
-    disabled_graph_cache: Optional[bool]
-    disabled_historical_data: Optional[bool]
-    disabled_intent_verification: Optional[bool]
+    errors: Optional[List[Error]] = None
+    loaded_size: int = Field(None, alias="loadedSize")
+    unloaded_size: int = Field(None, alias="unloadedSize")
+    disabled_graph_cache: Optional[bool] = None
+    disabled_historical_data: Optional[bool] = None
+    disabled_intent_verification: Optional[bool] = None
 
     def lock(self, ipf: IPFClient):
         if not self.locked and self.loaded:
             res = ipf.post(f"snapshots/{self.snapshot_id}/lock")
             res.raise_for_status()
             self.locked = True
         elif not self.loaded:
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/table.py` & `ipfabric-6.3.1b3/ipfabric/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,645 +1,463 @@
 import logging
-from typing import Optional, Dict, List, Any, Union
-
-import deepdiff
-from httpx import HTTPStatusError
-from pydantic import BaseModel
-
-from ipfabric.models import Devices
-from ipfabric.settings import Attributes
+import re
+from json import loads, dumps
+from typing import Optional, Union, Dict, List, Any, overload, Literal
+from urllib.parse import urlparse, urljoin, quote
+
+from httpx import HTTPStatusError, InvalidURL
+
+from ipfabric.api import IPFabricAPI
+from ipfabric.models import Technology, Inventory, Jobs, Intent, Devices
+from ipfabric.tools import TIMEZONES
+
+try:
+    from pandas import DataFrame
+except ImportError:
+    DataFrame = None
 
 logger = logging.getLogger("ipfabric")
 
-IGNORE_COLUMNS = {"id"}
+RE_PATH = re.compile(r"^/?(api/)?v\d(\.\d)?/")
+RE_TABLE = re.compile(r"^tables/")
+EXPORT_FORMAT = Literal["json", "csv", "df"]
 
 
-class BaseTable(BaseModel):
-    """model for table data"""
+class IPFClient(IPFabricAPI):
+    def __init__(
+        self,
+        base_url: Optional[str] = None,
+        api_version: Optional[str] = None,
+        snapshot_id: Optional[str] = None,
+        auth: Optional[Any] = None,
+        unloaded: bool = False,
+        streaming: bool = False,  # TODO: Default True in 6.4/7.0
+        **kwargs,
+    ):
+        """Initializes the IP Fabric Client
 
-    endpoint: str
-    client: Any
+        Args:
+            base_url: IP Fabric instance provided in 'base_url' parameter, or the 'IPF_URL' environment variable
+            api_version: [Optional] Version of IP Fabric API
+            auth: API token, tuple (username, password), or custom Auth to pass to httpx
+            snapshot_id: IP Fabric snapshot ID to use by default for database actions - defaults to '$last'
+            streaming: Stream table requests instead of paging results, see documentation for important information.
+            **kwargs: Keyword args to pass to httpx
+        """
+        super().__init__(
+            base_url=base_url,
+            api_version=api_version,
+            auth=auth,
+            snapshot_id=snapshot_id,
+            unloaded=unloaded,
+            **kwargs,
+        )
+        self.streaming = streaming
+        if self.streaming and self.os_version.split("+")[0] < "6.3.1":
+            logger.warning(
+                f"Setting `streaming=True` is not recommended until 6.3.1 due to RBAC issues: "  # TODO: Remove in v7.0
+                f"IP Fabric OS Version is {self.os_version}."
+            )
+        self.technology = Technology(client=self)
+        self.jobs = Jobs(client=self)
+        self._devices = list()
 
     @property
-    def name(self):
-        return self.endpoint.split("/")[-1]
+    def snapshot_id(self) -> str:
+        """get snapshot Id"""
+        return self._snapshot_id
+
+    @snapshot_id.setter
+    def snapshot_id(self, snapshot_id):
+        super(self.__class__, self.__class__).snapshot_id.fset(self, snapshot_id)
+        self.intent = Intent(client=self)
+        self.api_to_web = {intent.api_endpoint: intent.web_endpoint for intent in self.intent.intent_checks}
+        self.inventory = Inventory(client=self)
 
     @property
-    def abs_endpoint(self):
-        return self.endpoint if self.endpoint[0] == "/" else "/" + self.endpoint
+    def devices(self) -> Devices:
+        """get devices"""
+        if not self._devices:
+            logger.info("Devices not loaded, loading devices.")
+            self._devices = self.load_devices()
+        return self._devices
+
+    @devices.setter
+    def devices(self, devices):
+        self._devices = devices
+
+    def load_devices(self, device_filters: dict = None, device_attr_filters: dict = None):
+        if self._no_loaded_snapshots:
+            logger.warning("No loaded snapshots, cannot load devices.")
+        else:
+            if not device_attr_filters and self.attribute_filters:
+                logger.warning(
+                    f"Global `attribute_filters` is set; only pulling devices matching:\n{self.attribute_filters}."
+                )
+            try:
+                self.devices = self.inventory.devices.all(
+                    export="object", filters=device_filters, attr_filters=device_attr_filters
+                )
+                return self.devices
+            except HTTPStatusError:
+                logger.warning(self._api_insuf_rights + 'on POST "/tables/inventory/devices". Will not load Devices.')
+        return list()
 
-    def fetch(
+    @staticmethod
+    def _check_url(url):
+        path = urlparse(url).path
+        r = RE_PATH.search(path)
+        url = path[r.end():] if r else path  # fmt: skip
+        url = url[1:] if url[0] == "/" else url
+        return url
+
+    def _create_payload(self, url, snapshot_id, filters, sort, attr_filters):
+        payload = dict()
+        if self.api_version >= "v6.3":  # TODO: No check in v7.0
+            payload = {"format": {"dataType": "json"}}
+        if filters and isinstance(filters, str):
+            payload["filters"] = loads(filters)
+        elif filters and isinstance(filters, dict):
+            payload["filters"] = filters
+        if snapshot_id:
+            payload["snapshot"] = snapshot_id
+        if sort:
+            payload["sort"] = sort
+        if RE_TABLE.match(url) and (attr_filters or self.attribute_filters):
+            payload["attributeFilters"] = attr_filters or self.attribute_filters
+        return payload
+
+    def _check_url_payload(self, url, snapshot_id, filters, reports, sort, attr_filters, export, csv_tz):
+        url = self._check_url(url)
+        payload = self._create_payload(url, snapshot_id, filters, sort, attr_filters)
+
+        if export != "csv":
+            if isinstance(reports, (str, list)):
+                payload["reports"] = reports
+            elif reports is True and "/" + url in self.api_to_web:
+                payload["reports"] = self.api_to_web["/" + url]
+            elif reports is True and "/" + url not in self.api_to_web:
+                logger.warning(
+                    f"Could not automatically discover Web Endpoint for Intent Data for table '/{url}'.\n"
+                    f"Table may not have any Intent Checks, please manually verify and enter to reports.\n"
+                    f"Returning results without Intent Rules."
+                )
+        else:
+            if reports:
+                logger.warning("CSV export does not return reports, parameter has been excluded.")
+            payload["format"] = {"exportToFile": True, "dataType": "csv"}
+            if csv_tz and csv_tz.lower() not in TIMEZONES:
+                raise ValueError(
+                    f"CSV timezone '{csv_tz}' not in available timezones; see `ipfabric.tools.shared.TIMEZONES`"
+                )
+            elif csv_tz:
+                payload["format"]["options"] = {"timezone": TIMEZONES[csv_tz.lower()]}
+        return url, payload
+
+    def _reports_stream_bug(self, payload):  # TODO: Remove in v7 and NIM-11915
+        """Bug NIM-11915"""
+        if getattr(self, "intent", None) and "reports" in payload and isinstance(payload["reports"], str):
+            reports = self.intent.intent_ids_by_web_endpoint[payload["reports"]]
+            if not reports:
+                logger.warning(
+                    f"Could not find Intent Report IDs for web endpoint '{payload['reports']}' or none defined."
+                )
+                del payload["reports"]
+            else:
+                payload["reports"] = reports
+        return payload
+
+    def _get_payload(self, url, payload):
+        snapshot_id = payload.pop("snapshot", None)
+        p = "&".join([f"{k}={quote(dumps(v, separators=(',', ':')))}" for k, v in payload.items()])
+        if snapshot_id:
+            p += f"&snapshot={snapshot_id}"
+        url = urljoin(str(self.base_url), url + f"?{p}")
+        if len(url) > 4096:
+            return False
+        return url
+
+    def _stream(self, url, payload, export):
+        if export != "csv":  # Bug NIM-11915
+            payload = self._reports_stream_bug(payload)
+        if export == "csv" and self.api_version <= "v6.3":
+            raise NotImplementedError(f"CSV export is implemented in v6.3.0; IPF version: {self.os_version}.")
+        get_url = self._get_payload(url, payload)
+        if get_url is False and export == "csv":
+            raise InvalidURL("URL exceeds max character limit of 4096 cannot export to CSV.")
+        elif get_url is False:
+            logger.warning("URL exceeds max character limit of 4096 switching to pagination.")
+            return False
+        with self.stream("GET", get_url) as stream_resp:
+            stream_resp.raise_for_status()
+            data = stream_resp.read()
+        return data if export == "csv" else loads(data)["data"]
+
+    def query(self, url: str, payload: Union[str, dict], get_all: bool = True) -> Union[List[dict], bytes]:
+        """Submits a query, does no formatting on the parameters.  Use for copy/pasting from the webpage.
+
+        Args:
+            url: Example: https://demo1.ipfabric.io/api/v1/tables/vlan/device-summary or tables/vlan/device-summary
+            payload: Dictionary to submit in POST or can be JSON string (i.e. read from file).
+            get_all: Default use pager to get all results and ignore pagination information in the payload
+
+        Returns:
+            list or bytes: List of Dictionary objects or bytes if csv.
+        """
+        url = self._check_url(url)
+        if isinstance(payload, str):
+            payload = loads(payload)
+        export = payload.get("format", {}).get("dataType", "json")
+        data = False
+        if (export == "csv" or self.streaming) and get_all:
+            data = self._stream(url, payload, export)
+        elif get_all and data is False:
+            data = self._ipf_pager(url, payload)
+        elif data is False:
+            res = self.post(url, json=payload)
+            res.raise_for_status()
+            data = res.json()["data"]
+        return data
+
+    def _get_columns(self, url: str):  # TODO: Remove in v7
+        logger.warning("""Use of _get_columns will be deprecated in a future release, please use get_columns""")
+        return self.get_columns(url=url)
+
+    def get_columns(self, url: str, snapshot: bool = True) -> List[str]:
+        """Submits malformed payload and extracts column names from it
+
+        Args:
+            url: API url to post
+            snapshot: Set to False for some tables like management endpoints.
+
+        Returns:
+            list: List of column names
+        """
+        snapshot_id = self.snapshot_id if snapshot else None
+        url, payload = self._check_url_payload(url, snapshot_id, None, None, None, None, None, None)
+        payload["columns"] = ["*"]
+        r = self.post(url, json=payload)
+        if r.status_code == 422:
+            msg = r.json()["errors"][0]["message"]
+            return [x.strip() for x in re.match(r"\".*\".*\[(.*)]$", msg).group(1).split(",")]
+        else:
+            r.raise_for_status()
+
+    def get_count(
         self,
-        columns: list = None,
-        filters: Optional[dict] = None,
+        url: str,
+        filters: Optional[Union[dict, str]] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
-        sort: Optional[dict] = None,
-        limit: Optional[int] = 1000,
-        start: Optional[int] = 0,
-        csv: bool = False,
-    ) -> Union[List[dict], bytes]:
-        """Gets all data from corresponding endpoint
-
-        Args:
-            columns: Optional columns to return, default is all
-            filters: Optional filters'
-            attr_filters: dict: Optional dictionary of Attribute filters
-            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
-            limit: Default to 1,000 rows
-            start: Starts at 0
-            csv: bool: Default False, returns bytes if True.
-        Returns:
-            Union[List[dict], str]: List of Dictionaries or bytes if CSV
-        """
-        return self.client.fetch(
-            self.endpoint,
-            columns=columns,
-            filters=filters,
-            attr_filters=attr_filters,
-            sort=sort,
-            limit=limit,
-            start=start,
-            snapshot=False,
-            csv=csv,
-        )
+        snapshot_id: Optional[str] = None,
+        snapshot: bool = True,
+    ) -> int:
+        """Get a total number of rows
+        Args:
+            url: API URL to post to
+            filters: Optional dictionary of filters
+            attr_filters: Optional dictionary of attribute filters
+            snapshot_id: Optional snapshot_id to override default
+            snapshot: Set to False for some tables like management endpoints.
+        Returns:
+            int: a count of rows
+        """
+        snapshot_id = snapshot_id or self.snapshot_id if snapshot else None
+        url, payload = self._check_url_payload(url, snapshot_id, filters, None, None, attr_filters, None, None)
+        payload.update({"columns": ["id"], "pagination": {"limit": 1, "start": 0}})
+        res = self.post(url, json=payload)
+        res.raise_for_status()
+        return res.json()["_meta"]["count"]
+
+    def _fetch_setup(self, url, export, columns, snapshot_id, filters, reports, sort, attr_filters, csv_tz, snapshot):
+        if export == "df" and DataFrame is None:
+            raise ImportError("pandas not installed. Run `pip install ipfabric[pd]`.")
+        snapshot_id = snapshot_id or self.snapshot_id if snapshot else None
+        url, payload = self._check_url_payload(url, snapshot_id, filters, reports, sort, attr_filters, export, csv_tz)
+        payload["columns"] = columns or self.get_columns(url, snapshot=snapshot)
+        return url, payload
 
-    def all(
+    @overload
+    def fetch(
         self,
-        columns: list = None,
-        filters: Optional[dict] = None,
-        attr_filters: Optional[Dict[str, List[str]]] = None,
+        url,
+        export: Literal["json"] = ...,
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
+        limit: Optional[int] = 1000,
+        start: Optional[int] = 0,
+        snapshot_id: Optional[str] = None,
+        reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
-        csv: bool = False,
-    ) -> Union[List[dict], bytes]:
-        """Gets all data from corresponding endpoint
-
-        Args:
-            columns: Optional columns to return, default is all
-            filters: Optional filters
-            attr_filters: dict: Optional dictionary of Attribute filters
-            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
-            csv: bool: Default False, returns bytes if True.
-        Returns:
-            Union[List[dict], bytes]: List of Dictionaries or bytes if CSV
-        """
-        return self.client.fetch_all(
-            self.endpoint,
-            columns=columns,
-            filters=filters,
-            attr_filters=attr_filters,
-            sort=sort,
-            snapshot=False,
-            csv=csv,
-        )
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot: bool = True,
+    ) -> List[dict]:
+        ...
 
-    def count(
+    @overload
+    def fetch(
         self,
-        filters: Optional[dict] = None,
+        url,
+        export: Literal["csv"],
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
+        limit: Optional[int] = 1000,
+        start: Optional[int] = 0,
+        snapshot_id: Optional[str] = None,
+        sort: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
-    ):
-        """
-        Gets count of table
-        :param filters: dict: Optional filters
-        :param attr_filters: dict: Optional dictionary of Attribute filters
-        :return: int: Count
-        """
-        return self.client.get_count(self.endpoint, filters=filters, attr_filters=attr_filters, snapshot=False)
-
-
-class Table(BaseTable, BaseModel):
-    """model for table data"""
+        snapshot: bool = True,
+        csv_tz: Optional[str] = None,
+    ) -> bytes:
+        ...
 
+    @overload
     def fetch(
         self,
-        columns: list = None,
-        filters: Optional[dict] = None,
-        attr_filters: Optional[Dict[str, List[str]]] = None,
+        url,
+        export: Literal["df"] = ...,
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
+        limit: Optional[int] = 1000,
+        start: Optional[int] = 0,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot: bool = True,
+    ) -> DataFrame:
+        ...
+
+    def fetch(
+        self,
+        url,
+        export: EXPORT_FORMAT = "json",
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
         limit: Optional[int] = 1000,
         start: Optional[int] = 0,
-        csv: bool = False,
-    ) -> Union[List[dict], bytes]:
-        """Gets all data from corresponding endpoint
+        snapshot_id: Optional[str] = None,
+        reports: Optional[Union[bool, list, str]] = False,
+        sort: Optional[dict] = None,
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot: bool = True,
+        csv_tz: Optional[str] = None,
+    ):
+        """Gets data from IP Fabric for specified endpoint
 
         Args:
-            columns: Optional columns to return, default is all
-            filters: Optional filters'
-            attr_filters: dict: Optional dictionary of Attribute filters
-            snapshot_id: Optional snapshot ID to override class
-            reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
-            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            url: Example tables/vlan/device-summary
+            export: str: Export format to return [json, csv]; default is json.
+            columns: Optional list of columns to return, None will return all
+            filters: Optional dictionary of filters
             limit: Default to 1,000 rows
             start: Starts at 0
-            csv: bool: Default False, returns bytes if True.
+            snapshot_id: Optional snapshot_id to override default
+            reports: String of frontend URL where the reports are displayed or a list of report IDs
+            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            attr_filters: Optional dictionary to apply an Attribute filter
+            snapshot: Set to False for some tables like management endpoints.
+            csv_tz: str: Default None, set a timezone to return human-readable dates when using CSV;
+                         see `ipfabric.tools.shared.TIMEZONES`
         Returns:
-            Union[List[dict], str]: List of Dictionaries or bytes if CSV
+            Union[List[dict], bytes, pandas.DataFrame]: List of dict if json, bytes string if CSV, DataFrame is df
         """
-        return self.client.fetch(
-            self.endpoint,
-            columns=columns,
-            filters=filters,
-            attr_filters=attr_filters,
-            snapshot_id=snapshot_id,
-            reports=reports,
-            sort=sort,
-            limit=limit,
-            start=start,
-            csv=csv,
+        url, payload = self._fetch_setup(
+            url, export, columns, snapshot_id, filters, reports, sort, attr_filters, csv_tz, snapshot
         )
+        payload["pagination"] = dict(start=start, limit=limit)
+        data = False
+        if export == "csv" or self.streaming:
+            data = self._stream(url, payload, export)
+        if data is False:
+            res = self.post(url, json=payload)
+            res.raise_for_status()
+            data = res.json()["data"]
+        if export == "df":
+            data = DataFrame.from_records(data) if export == "df" else data
+        return data
 
-    def all(
+    @overload
+    def fetch_all(
         self,
-        columns: list = None,
-        filters: Optional[dict] = None,
-        attr_filters: Optional[Dict[str, List[str]]] = None,
+        url: str,
+        export: Literal["json"] = ...,
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
-        csv: bool = False,
-    ) -> Union[List[dict], bytes]:
-        """Gets all data from corresponding endpoint
-
-        Args:
-            columns: Optional columns to return, default is all
-            filters: Optional filters
-            attr_filters: dict: Optional dictionary of Attribute filters
-            snapshot_id: Optional snapshot ID to override class
-            reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
-            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
-            csv: bool: Default False, returns bytes if True.
-        Returns:
-            Union[List[dict], bytes]: List of Dictionaries or bytes if CSV
-        """
-        return self.client.fetch_all(
-            self.endpoint,
-            columns=columns,
-            filters=filters,
-            attr_filters=attr_filters,
-            snapshot_id=snapshot_id,
-            reports=reports,
-            sort=sort,
-            csv=csv,
-        )
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot: bool = True,
+    ) -> List[dict]:
+        ...
 
-    def count(
+    @overload
+    def fetch_all(
         self,
-        filters: Optional[dict] = None,
+        url: str,
+        export: Literal["csv"],
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
         snapshot_id: Optional[str] = None,
+        sort: Optional[dict] = None,
         attr_filters: Optional[Dict[str, List[str]]] = None,
-    ):
-        """
-        Gets count of table
-        Args:
-            filters: dict: Optional filters
-            snapshot_id: str: Optional snapshot ID to override class
-            attr_filters: dict: Optional dictionary of Attribute filters
+        snapshot: bool = True,
+        csv_tz: Optional[str] = None,
+    ) -> bytes:
+        ...
 
-        Returns:
-            int: Count of rows
-        """
-        return self.client.get_count(self.endpoint, filters=filters, attr_filters=attr_filters, snapshot_id=snapshot_id)
-
-    @staticmethod
-    def _ignore_columns(columns: set, columns_ignore: set):
-        """
-        Determines which columns to use in the query.
-        Args:
-            columns: set : Set of columns to use
-            columns_ignore: set : Set of columns to ignore
-
-        Returns:
-            list[str]: List of columns to use
-        """
-        cols_for_return = set()
-        for col in columns:
-            if col in columns_ignore and col != "id":
-                logger.debug(f"Column {col} in columns_ignore, ignoring")
-                continue
-            cols_for_return.add(col)
-        return cols_for_return
-
-    def _compare_determine_columns(self, columns: set, columns_ignore: set, unique_keys: set, nested_keys: set):
-        """
-        Determines which columns to use in the query, and which columns to use
-        Only supports a single nested column
-        Args:
-            columns: set : Set of columns to use
-            columns_ignore: set : Set of columns to ignore
-            unique_keys: set : Set of columns for unique keys
-            nested_keys: set: Set of nested columns that belongs to a column in columns, columns_ignore, or unique_keys
-
-        Returns:
-            tuple[list, list]: List of columns to use in query, List of columns to use when sorting data
-        """
-        # get all columns for the table
-        table_columns = set(self.client.get_columns(self.endpoint))
-
-        # get any nested columns
-        nested_cols_for_return = None
-        # if the user passed nested_column_returns
-        if nested_keys:
-            # get a row of data
-            one_row_of_data = self.fetch(limit=1)
-            # loop over each column in the table columns
-            for col in table_columns:
-                # check if the data returned has nested columns
-                if isinstance(one_row_of_data[0][col], list):
-                    logger.debug(f"Column: {col}, one row of data: {one_row_of_data}")
-                    check_len_of_data = len(one_row_of_data[0][col])
-                    if check_len_of_data >= 0:
-                        logger.warning(
-                            "Nested Column was Detected, but no data was present to determine if there are any nested columns, skipping"
-                        )
-                        continue
-                    # get all the nested column names
-                    nested_cols = set(one_row_of_data[0][col][0].keys())
-                    # create a set of nested column names requested by the user
-                    nested_cols_for_return = {col for col in nested_cols if col in nested_keys}
-
-        # Must always ignore some columns
-        columns_ignore.update(IGNORE_COLUMNS)
-
-        cols_for_return = set()
-        # user passes unique_keys
-        if unique_keys:
-            if not table_columns.issuperset(unique_keys):
-                raise ValueError(f"Unique Key(s) {unique_keys - table_columns} not in table {self.name}")
-            for u in unique_keys:
-                cols_for_return.add(u)
-            return list(cols_for_return), nested_cols_for_return
-        # user passes columns
-        if columns:
-            if not table_columns.issuperset(columns):
-                raise ValueError(f"Column(s) {columns - table_columns} not in table {self.name}")
-            cols_for_return.update(self._ignore_columns(columns, columns_ignore))
-            return list(cols_for_return), nested_cols_for_return
-        # user does not pass columns
-        # or only passed columns_ignore
-        else:
-            cols_for_return.update(self._ignore_columns(table_columns, columns_ignore))
-            return list(cols_for_return), nested_cols_for_return
-
-    @staticmethod
-    def _remove_keys_from_dict(dict_object, keys_to_remove):
-        if not keys_to_remove:
-            return dict_object
-
-        for v in dict_object.values():
-            if not isinstance(v, list):
-                continue
-
-            for item in v:
-                for key in keys_to_remove:
-                    if key in item:
-                        item.pop(key)
-
-        return dict_object
-
-    def _hash_data(self, json_data, unique_keys=None, nested_columns_ignore=None):
-        """
-        Hashes data. Turns any data into a string and hashes it, then returns the hash as a key for the data
-        Args:
-            json_data: list[dict] : List of dictionaries to hash
-            unique_keys: list[str] : List of keys to use for hashing
-            nested_columns_ignore: list[str]: List of nested column keys to filter data
-
-        Returns:
-            dict[str]: dictionary with hash as key and values as the original data
-        """
-        # loop over each obj, turn the obj into a string, and hash it
-        return_json = dict()
-        # user passes unique_keys
-        if unique_keys:
-            # loop over each response
-            for dict_obj in json_data:
-                dict_for_hash = self._remove_keys_from_dict(dict_object=dict_obj, keys_to_remove=nested_columns_ignore)
-                # create a dictionary, of only the keys/columns requested
-                hash_key = {key: dict_for_hash[key] for key in unique_keys}
-                # hash the data
-                unique_hash = deepdiff.DeepHash(hash_key)[hash_key]
-                # check if the data has already been processed.
-                if unique_hash in return_json:
-                    # raise error if data has already been processed
-                    raise KeyError(f"Unique Key(s) {unique_keys} are not unique, please adjust unique_keys input.")
-                # store the data, using the hash as a key
-                return_json[unique_hash] = dict_for_hash
-        # user passes columns and/or column ignore
-        else:
-            # loop over each response
-            for dict_obj in json_data:
-                dict_for_hash = self._remove_keys_from_dict(dict_object=dict_obj, keys_to_remove=nested_columns_ignore)
-                # hash each object, and store it in a dictionary, with the hash as the key
-                return_json[deepdiff.DeepHash(dict_for_hash)[dict_for_hash]] = dict_for_hash
-        return return_json
-
-    @staticmethod
-    def _make_set(data: Union[list, set, str] = None):
-        if isinstance(data, str):
-            return {data}
-        elif data is None:
-            return set()
-        else:
-            return set(data)
-
-    def compare(
-        self,
-        snapshot_id: str = None,
-        columns: Union[list, set] = None,
-        columns_ignore: Union[list, set, str] = None,
-        unique_keys: Union[list, set, str] = None,
-        nested_columns_ignore: Union[list, set, str] = None,
-        **kwargs,
-    ):
-        """
-        Compares a table from the current snapshot to the snapshot_id passed.
-        Args:
-            snapshot_id: str : The snapshot_id to compare to.
-            columns: list : List of columns to compare. If None, will compare all columns.
-            columns_ignore: list : List of columns to ignore. If None, will always ignore 'id' column.
-            unique_keys: list : List of columns to use as unique keys. If None, will use all columns as primary key.
-            nested_columns_ignore: List of columns that belong to a nested columns
-            **kwargs: dict : Optional Table.all() arguments to apply to the table before comparing.
-
-        Returns:
-            dict : dictionary containing the differences between the two snapshots.
-                   Possible keys are 'added', 'removed' and 'changed'.
-        """
-        return_dict = dict()
-
-        # determine which columns to use in query
-        columns = self._make_set(columns)
-        columns_ignore = self._make_set(columns_ignore)
-        unique_keys = self._make_set(unique_keys)
-        nested_columns_ignore = self._make_set(nested_columns_ignore)
-        cols_for_query, nested_cols = self._compare_determine_columns(
-            columns, columns_ignore, unique_keys, nested_columns_ignore
-        )
-        data = self.all(columns=cols_for_query, **kwargs)
-        data_compare = self.all(snapshot_id=snapshot_id, columns=cols_for_query, **kwargs)
-
-        # since we turned the values into a hash, we can just compare the keys
-        if unique_keys:
-            hashed_data_unique = self._hash_data(data, unique_keys, nested_cols)
-            hashed_data_compare_unique = self._hash_data(data_compare, unique_keys, nested_cols)
-            changed = [
-                hashed_data_unique[hashed_str]
-                for hashed_str in hashed_data_unique.keys()
-                if hashed_str not in hashed_data_compare_unique.keys()
-            ]
-            return_dict["changed"] = changed
-            return return_dict
-        # compare both ways
-        hashed_data = self._hash_data(data, nested_columns_ignore=nested_cols)
-        hashed_data_compare = self._hash_data(data_compare, nested_columns_ignore=nested_cols)
-        added = [
-            hashed_data[hashed_str] for hashed_str in hashed_data.keys() if hashed_str not in hashed_data_compare.keys()
-        ]
-        removed = [
-            hashed_data_compare[hashed_str]
-            for hashed_str in hashed_data_compare.keys()
-            if hashed_str not in hashed_data.keys()
-        ]
-        return_dict["added"] = added
-        return_dict["removed"] = removed
-        return return_dict
-
-    def _is_valid_ipf_table_endpoint(self, endpoint):
-        """
-        Checks if endpoint is a valid table endpoint
-        Args:
-            endpoint: str : URL of table endpoint
-
-        Returns:
-            bool: False if table is not a valid table endpoint
-        """
-
-        attr_ignore = [
-            "__abstractmethods__",
-            "__annotations__",
-            "__class__",
-            "__class_vars__",
-            "__config__",
-            "__custom_root_type__",
-            "__delattr__",
-            "__dict__",
-            "__dir__",
-            "__doc__",
-            "__eq__",
-            "__exclude_fields__",
-            "__fields__",
-            "__fields_set__",
-            "__format__",
-            "__ge__",
-            "__get_validators__",
-            "__getattribute__",
-            "__getstate__",
-            "__gt__",
-            "__hash__",
-            "__include_fields__",
-            "__init__",
-            "__init_subclass__",
-            "__iter__",
-            "__json_encoder__",
-            "__le__",
-            "__lt__",
-            "__module__",
-            "__ne__",
-            "__new__",
-            "__post_root_validators__",
-            "__pre_root_validators__",
-            "__pretty__",
-            "__private_attributes__",
-            "__reduce__",
-            "__reduce_ex__",
-            "__repr__",
-            "__repr_args__",
-            "__repr_name__",
-            "__repr_str__",
-            "__rich_repr__",
-            "__schema_cache__",
-            "__setattr__",
-            "__setstate__",
-            "__signature__",
-            "__sizeof__",
-            "__slots__",
-            "__str__",
-            "__subclasshook__",
-            "__try_update_forward_refs__",
-            "__validators__",
-            "_abc_impl",
-            "_calculate_keys",
-            "_copy_and_set_values",
-            "_decompose_class",
-            "_enforce_dict_if_root",
-            "_get_value",
-            "_init_private_attributes",
-            "_iter",
-            "Config",
-            "client",
-            "construct",
-            "copy",
-            "dict",
-            "from_orm",
-            "json",
-            "oam",
-            "parse_file",
-            "parse_obj",
-            "parse_raw",
-            "schema",
-            "schema_json",
-            "update_forward_refs",
-            "validate",
-        ]
-        dict_of_tech_attrs = dict()
-        tech_attrs = [attr for attr in dir(self.client.technology) if attr not in attr_ignore]
-        for tech_attr in tech_attrs:
-            dict_of_tech_attrs[tech_attr] = list()
-            tech_attr_attrs = [
-                attr for attr in dir(getattr(self.client.technology, tech_attr)) if attr not in attr_ignore
-            ]
-            for tech_attr_attr in tech_attr_attrs:
-                dict_of_tech_attrs[tech_attr].append(tech_attr_attr)
-        inv_attrs = [attr for attr in dir(self.client.inventory) if attr not in attr_ignore]
-        end_of_url = endpoint.split("/")[-1]
-        if end_of_url in inv_attrs:
-            return True
-        for tech_parent_attr, tech_attr in dict_of_tech_attrs.items():
-            if end_of_url in tech_attr:
-                return True
-        return False
-
-    def join_table(self, on_column, join_table_path):
-        """
-        performs a join operation on on_columns, assuming on_columns are columns that
-        exist in both self and join_table_path
-
-        Args:
-            on_column:
-            columns_ignore:
-            join_table_path: URL of table you wish to join to
-
-        Returns:
-        """
-        check_join_table_endpoint = self._is_valid_ipf_table_endpoint(join_table_path)
-        self_cols = set(self.client.get_columns(self.endpoint))
-        if not set(on_column).issubset(self_cols):
-            raise ValueError(f"Column {on_column}, is not subset of {self_cols}.")
-        self_table = self.client.fetch_all(self.endpoint)
-        join_table = self.client.fetch_all(join_table_path)
-
-        joined_data = {
-            self_dict[on_column]: {**self_dict, **join_dict}
-            for self_dict in self_table
-            for join_dict in join_table
-            if self_dict[on_column] == join_dict[on_column]
-        }
-
-        return joined_data
-
-
-class DeviceTable(Table):
-    """model for Device Table data"""
-
-    endpoint = "tables/inventory/devices"
-
-    def _as_model(self, devices, as_model):
-        if not as_model:
-            return devices
-        try:
-            attributes = Attributes(client=self.client, snapshot_id=self.client.snapshot_id).all()
-        except HTTPStatusError:
-            logger.warning(
-                self.client._api_insuf_rights
-                + 'on POST "/tables/snapshot-attributes". Cannot load Attributes in Devices.'
-            )
-            attributes = None
-        try:
-            blob_keys = self.client.fetch_all("/tables/management/configuration/saved", columns=["sn", "blobKey"])
-        except HTTPStatusError:
-            logger.warning(
-                self.client._api_insuf_rights + 'on POST "/tables/management/configuration/saved". '
-                "You will not be able to pull device config from Device model."
-            )
-            blob_keys = None
-        return Devices(snapshot_id=self.client.snapshot_id, devices=devices, attributes=attributes, blob_keys=blob_keys)
-
-    def fetch(
+    @overload
+    def fetch_all(
         self,
-        columns: list = None,
-        filters: Optional[dict] = None,
-        attr_filters: Optional[Dict[str, List[str]]] = None,
+        url: str,
+        export: Literal["df"],
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
-        limit: Optional[int] = 1000,
-        start: Optional[int] = 0,
-        as_model: Optional[bool] = False,
-        csv: bool = False,
-    ) -> Union[List[dict], Devices, bytes]:
-        """Gets all data from corresponding endpoint
-
-        Args:
-            columns: Optional columns to return, default is all
-            filters: Optional filters'
-            attr_filters: dict: Optional dictionary of Attribute filters
-            snapshot_id: Optional snapshot ID to override class
-            reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
-            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
-            limit: Default to 1,000 rows
-            start: Starts at 0
-            as_model: bool: Default False, if True returns Devices model
-            csv: bool: Default False, returns bytes if True. If `as_model` set to True then csv will be set to False.
-        Returns:
-            Union[List[dict], Devices, bytes]: List of Dictionaries, Devices Object if as_model, or bytes if CSV
-        """
-        csv = False if as_model else csv
-        devices = super(DeviceTable, self).fetch(
-            columns=columns,
-            filters=filters,
-            attr_filters=attr_filters,
-            snapshot_id=snapshot_id,
-            reports=reports,
-            sort=sort,
-            limit=limit,
-            start=start,
-            csv=csv,
-        )
-        return self._as_model(devices, as_model)
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot: bool = True,
+    ) -> DataFrame:
+        ...
 
-    def all(
+    def fetch_all(
         self,
-        columns: list = None,
-        filters: Optional[dict] = None,
-        attr_filters: Optional[Dict[str, List[str]]] = None,
+        url: str,
+        export: EXPORT_FORMAT = "json",
+        columns: Optional[List] = None,
+        filters: Optional[Union[dict, str]] = None,
         snapshot_id: Optional[str] = None,
         reports: Optional[Union[bool, list, str]] = False,
         sort: Optional[dict] = None,
-        as_model: Optional[bool] = False,
-        csv: bool = False,
-    ) -> Union[List[dict], Devices, bytes]:
-        """Gets all data from corresponding endpoint
+        attr_filters: Optional[Dict[str, List[str]]] = None,
+        snapshot: bool = True,
+        csv_tz: Optional[str] = None,
+    ):
+        """Gets all data from IP Fabric for specified endpoint
 
         Args:
-            columns: Optional columns to return, default is all
-            filters: Optional filters
-            attr_filters: dict: Optional dictionary of Attribute filters
-            snapshot_id: Optional snapshot ID to override class
-            reports: True to return Intent Rules (also accepts string of frontend URL) or a list of report IDs
-            sort: Dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
-            as_model: bool: Default False, if True returns Devices model
-            csv: bool: Default False, returns bytes if True. If `as_model` set to True then csv will be set to False.
+            url: Example tables/vlan/device-summary
+            export: str: Export format to return [json, csv]; default is json.
+            columns: Optional list of columns to return, None will return all
+            filters: Optional dictionary of filters
+            snapshot_id: Optional snapshot_id to override default
+            reports: String of frontend URL where the reports are displayed or a list of report IDs
+            sort: Optional dictionary to apply sorting: {"order": "desc", "column": "lastChange"}
+            attr_filters: Optional dictionary to apply an Attribute filter
+            snapshot: Set to False for some tables like management endpoints.
+            csv_tz: str: Default None, set a timezone to return human-readable dates when using CSV;
+                         see `ipfabric.tools.shared.TIMEZONES`
         Returns:
-            Union[List[dict], Devices, bytes]: List of Dictionaries, Devices Object if as_model, or bytes if CSV
+            Union[List[dict], bytes, pandas.DataFrame]: List of dict if json, bytes string if CSV, DataFrame is df
         """
-        csv = False if as_model else csv
-        devices = super(DeviceTable, self).all(
-            columns=columns,
-            filters=filters,
-            attr_filters=attr_filters,
-            snapshot_id=snapshot_id,
-            reports=reports,
-            sort=sort,
-            csv=csv,
+        url, payload = self._fetch_setup(
+            url, export, columns, snapshot_id, filters, reports, sort, attr_filters, csv_tz, snapshot
         )
-        return self._as_model(devices, as_model)
+        data = False
+        if export == "csv" or self.streaming:
+            data = self._stream(url, payload, export)
+        if data is False:
+            data = self._ipf_pager(url, payload)
+        if export == "df":
+            data = DataFrame.from_records(data)
+        return data
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/__init__.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 
 from pydantic import BaseModel
 
 from ipfabric import models
-
 from .addressing import Addressing
 from .cloud import Cloud
 from .dhcp import Dhcp
 from .fhrp import Fhrp
 from .interfaces import Interfaces
 from .ip_telephony import IpTelephony
 from .load_balancing import LoadBalancing
@@ -26,15 +25,15 @@
 from .security import Security
 from .stp import Stp
 from .vlans import Vlans
 from .wireless import Wireless
 
 
 class Technology(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def platforms(self):
         return Platforms(client=self.client)
 
     @property
     def interfaces(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/addressing.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/addressing.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Addressing(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def arp_table(self):
         return models.Table(client=self.client, endpoint="tables/addressing/arp")
 
     @property
     def mac_table(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/dhcp.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/dhcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Dhcp(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def relay_interfaces(self):
         return models.Table(client=self.client, endpoint="tables/dhcp/relay/interfaces")
 
     @property
     def relay_interfaces_stats_received(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/fhrp.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/fhrp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Fhrp(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def group_state(self):
         return models.Table(client=self.client, endpoint="tables/fhrp/group-state")
 
     @property
     def group_members(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/interfaces.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Interfaces(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def current_rates_data_inbound(self):
         return models.Table(client=self.client, endpoint="tables/interfaces/load/inbound")
 
     @property
     def current_rates_data_outbound(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/load_balancing.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class LoadBalancing(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def virtual_servers(self):
         return models.Table(client=self.client, endpoint="tables/load-balancing/virtual-servers")
 
     @property
     def virtual_servers_pools(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/management.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/management.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Management(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def aaa_servers(self):
         return models.Table(client=self.client, endpoint="tables/security/aaa/servers")
 
     @property
     def aaa_lines(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/mpls.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/mpls.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Mpls(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def ldp_neighbors(self):
         return models.Table(client=self.client, endpoint="tables/mpls/ldp/neighbors")
 
     @property
     def ldp_interfaces(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/multicast.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/multicast.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Multicast(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def pim_neighbors(self):
         return models.Table(client=self.client, endpoint="tables/multicast/pim/neighbors")
 
     @property
     def pim_interfaces(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/neighbors.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/neighbors.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Neighbors(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def neighbors_all(self):
         return models.Table(client=self.client, endpoint="tables/neighbors/all")
 
     @property
     def neighbors_unmanaged(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/oam.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/oam.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Oam(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def unidirectional_link_detection_neighbors(self):
         return models.Table(
             client=self.client, endpoint="tables/management/oam/unidirectional-link-detection/neighbors"
         )
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/platforms.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/platforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Platforms(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def environment_power_supplies(self):
         return models.Table(client=self.client, endpoint="tables/inventory/power-supplies")
 
     @property
     def environment_power_supplies_fans(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/port_channels.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/port_channels.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class PortChannels(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def inbound_balancing_table(self):
         return models.Table(client=self.client, endpoint="tables/interfaces/port-channel/balance/inbound")
 
     @property
     def outbound_balancing_table(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/qos.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/qos.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Qos(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def policy_maps(self):
         return models.Table(client=self.client, endpoint="tables/qos/policy-maps")
 
     @property
     def shaping(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/routing.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Routing(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def summary_protocols(self):
         return models.Table(client=self.client, endpoint="tables/networks/summary/protocols")
 
     @property
     def summary_protocols_bgp(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/sdn.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/sdn.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Sdn(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def aci_endpoints(self):
         return models.Table(client=self.client, endpoint="tables/aci/endpoints")
 
     @property
     def aci_vlan(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/security.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Security(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def acl(self):
         return models.Table(client=self.client, endpoint="tables/security/acl")
 
     @property
     def acl_interface(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/stp.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/stp.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Stp(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def bridges(self):
         return models.Table(client=self.client, endpoint="tables/spanning-tree/bridges")
 
     @property
     def instances(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/vlans.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/vlans.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Vlans(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def device_summary(self):
         return models.Table(client=self.client, endpoint="tables/vlan/device-summary")
 
     @property
     def device_detail(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/models/technology/wireless.py` & `ipfabric-6.3.1b3/ipfabric/models/technology/wireless.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ipfabric import models
 
 logger = logging.getLogger("ipfabric")
 
 
 class Wireless(BaseModel):
-    client: Any
+    client: Any = None
 
     @property
     def controllers(self):
         return models.Table(client=self.client, endpoint="tables/wireless/controllers")
 
     @property
     def access_points(self):
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/__init__.py` & `ipfabric-6.3.1b3/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/api_tokens.py` & `ipfabric-6.3.1b3/ipfabric/settings/api_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 class Token(BaseModel):
     description: str
     usage: int
     username: str
     expires: Optional[int] = None
     token: Optional[str] = None
     user_id: str = Field(alias="userId")
-    user_role_ids: Optional[List[str]] = Field(alias="userRoleIds", default=None)
+    user_role_ids: Optional[List[str]] = Field(None, alias="userRoleIds")
     token_id: str = Field(alias="id")
     is_expired: bool = Field(alias="isExpired")
-    last_used: Optional[str] = Field(alias="lastUsed")
-    role_ids: List[str] = Field(alias="roleIds")
-    role_names: Optional[List[str]] = Field(alias="roleNames", default=None)
+    last_used: Optional[str] = Field(None, alias="lastUsed")
+    role_ids: List[str] = Field(alias="roleIds", default_factory=list)
+    role_names: Optional[List[str]] = Field(None, alias="roleNames")
 
 
 class APIToken:
     def __init__(self, client):
         self.client: Any = client
         self.tokens = self.get_tokens()
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/attributes.py` & `ipfabric-6.3.1b3/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/authentication.py` & `ipfabric-6.3.1b3/ipfabric/settings/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 from pydantic.dataclasses import dataclass
 
 logger = logging.getLogger("ipfabric")
 
 
 class Expiration(BaseModel):
     enabled: bool
-    value: Optional[datetime]
+    value: Optional[datetime] = None
 
 
 class Credential(BaseModel):
     network: list
-    excluded: list = Field(alias="excludeNetworks")
-    expiration: Expiration = Field(alias="expirationDate")
-    credential_id: str = Field(alias="id")
-    encrypt_password: str = Field(alias="password")
-    priority: Optional[int]
+    excluded: list = Field(None, alias="excludeNetworks")
+    expiration: Expiration = Field(None, alias="expirationDate")
+    credential_id: str = Field(None, alias="id")
+    encrypt_password: str = Field(None, alias="password")
+    priority: Optional[int] = None
     username: str
-    config_mgmt: bool = Field(alias="syslog")
-    notes: Optional[str]
+    config_mgmt: bool = Field(None, alias="syslog")
+    notes: Optional[str] = None
 
 
 class Privilege(BaseModel):
-    network: list = Field(alias="includeNetworks")
-    excluded: list = Field(alias="excludeNetworks")
-    expiration: Expiration = Field(alias="expirationDate")
-    privilege_id: str = Field(alias="id")
-    encrypt_password: str = Field(alias="password")
-    priority: Optional[int]
+    network: list = Field(None, alias="includeNetworks")
+    excluded: list = Field(None, alias="excludeNetworks")
+    expiration: Expiration = Field(None, alias="expirationDate")
+    privilege_id: str = Field(None, alias="id")
+    encrypt_password: str = Field(None, alias="password")
+    priority: Optional[int] = None
     username: str
-    notes: Optional[str]
+    notes: Optional[str] = None
 
 
 @dataclass
 class Authentication:
     client: Any
     credentials: dict = Field(default=dict())
     enables: dict = Field(default=dict())
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/discovery.py` & `ipfabric-6.3.1b3/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/seeds.py` & `ipfabric-6.3.1b3/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/site_separation.py` & `ipfabric-6.3.1b3/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/user_mgmt.py` & `ipfabric-6.3.1b3/ipfabric/settings/user_mgmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 import pytz
 from pydantic import Field, BaseModel
 
 logger = logging.getLogger("ipfabric")
 
 
 class Token(BaseModel):
-    token_id: str = Field(alias="id")
-    description: Optional[str]
-    role_ids: list = Field(alias="roleIds")
+    token_id: str = Field(None, alias="id")
+    description: Optional[str] = None
+    role_ids: list = Field(None, alias="roleIds")
 
 
 class User(BaseModel):
     username: str
-    user_id: str = Field(alias="id")
-    local: Optional[bool] = Field(alias="isLocal")
-    sso_provider: Optional[Any] = Field(alias="ssoProvider")
-    domains: Optional[Any] = Field(alias="domainSuffixes")
+    user_id: str = Field(None, alias="id")
+    local: Optional[bool] = Field(None, alias="isLocal")
+    sso_provider: Optional[Any] = Field(None, alias="ssoProvider")
+    domains: Optional[Any] = Field(None, alias="domainSuffixes")
     role_names: Optional[list] = Field(alias="roleNames", default_factory=list)
-    role_ids: list = Field(alias="roleIds")
-    ldap_id: Optional[Any] = Field(alias="ldapId")
-    timezone: Optional[str]
-    token: Optional[Token]
+    role_ids: list = Field(None, alias="roleIds")
+    ldap_id: Optional[Any] = Field(None, alias="ldapId")
+    timezone: Optional[str] = None
+    token: Optional[Token] = None
     _get_snapshots_settings: Optional[bool] = None
 
-    class Config:
-        underscore_attrs_are_private = True
-
     @property
     def is_admin(self):
         return (
             True
             if (self.token and "admin" in self.token.role_ids) or (not self.token and "admin" in self.role_ids)
             else False
         )
@@ -52,20 +49,20 @@
         msg = f'User "{self.username}" '
         if self.token:
             msg += f'Token "{self.token.description}" '
         return msg
 
 
 class Role(BaseModel):
-    role_id: str = Field(alias="id")
     name: str
-    description: Optional[str]
-    role_type: str = Field(alias="type")
-    admin: bool = Field(alias="isAdmin")
-    system: bool = Field(alias="isSystem")
+    role_id: str = Field(None, alias="id")
+    description: Optional[str] = None
+    role_type: str = Field(None, alias="type")
+    admin: bool = Field(None, alias="isAdmin")
+    system: bool = Field(None, alias="isSystem")
 
 
 class UserMgmt:
     def __init__(self, client):
         self.client: Any = client
         self.roles = self.get_roles()
         self.users = self.get_users()
```

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/vendor_api.py` & `ipfabric-6.3.1b3/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.3.1b3/ipfabric/settings/vendor_api_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Literal
 
-from pydantic import BaseModel, Field, validator, AnyHttpUrl
+from pydantic import field_validator, BaseModel, Field, AnyHttpUrl
 
 AWS_REGIONS = [
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -42,15 +42,16 @@
     base Vendor API config
     """
 
     slug: str
     comment: str = ""
     isEnabled: bool = True
 
-    @validator("slug")
+    @field_validator("slug")
+    @classmethod
     def check_slug(cls, slug):
         if not re.match(SLUG, slug):
             raise ValueError(f"{slug} is not a valid slug and must match regex {SLUG}")
         return slug
 
 
 class SystemProxy(BaseModel):
@@ -87,25 +88,27 @@
     """
     AWS vendor api support
     """
 
     apiKey: str
     apiSecret: str
     regions: list
-    assumeRoles: Optional[List[Union[str, dict, AssumeRole]]] = Field(default=None)
-    type: str = Field(default="aws-ec2", const=True)
+    assumeRoles: Optional[List[Union[str, dict, AssumeRole]]] = None
+    type: Literal["aws-ec2"] = "aws-ec2"
 
-    @validator("regions")
+    @field_validator("regions")
+    @classmethod
     def check_region(cls, regions):
         for r in regions:
             if r.lower() not in AWS_REGIONS:
                 raise ValueError(f"{r} is not a valid AWS Region")
         return [r.lower() for r in regions]
 
-    @validator("assumeRoles")
+    @field_validator("assumeRoles")
+    @classmethod
     def check_roles(cls, roles):
         validated_roles = list()
         for role in roles:
             if isinstance(role, str):
                 validated_roles.append(AssumeRole(role=role))
             elif isinstance(role, dict):
                 if "role" in role:
@@ -122,136 +125,137 @@
     Azure vendor api support
     """
 
     clientId: str
     clientSecret: str
     subscriptionId: str
     tenantId: str
-    type: str = Field(default="azure", const=True)
+    type: Literal["azure"] = "azure"
 
 
 class CheckPointApiKey(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Checkpoint vendor api support
     """
 
     apiKey: str
     baseUrl: AnyHttpUrl
     domains: Optional[List[str]] = Field(default_factory=list)
-    type: str = Field(default="checkpoint-mgmt-api", const=True)
+    type: Literal["checkpoint-mgmt-api"] = "checkpoint-mgmt-api"
 
 
 class CheckPointUserAuth(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     checkpoint authentication vendor api support
     """
 
     domains: Optional[List[str]] = Field(default_factory=list)
-    type: str = Field(default="checkpoint-mgmt-api", const=True)
+    type: Literal["checkpoint-mgmt-api"] = "checkpoint-mgmt-api"
 
 
 class CiscoAPIC(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Cisco APIC vendor api support
     """
 
-    type: str = Field(default="ciscoapic", const=True)
+    type: Literal["ciscoapic"] = "ciscoapic"
 
 
 class CiscoFMC(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Cisco FMC vendor api support
     """
 
-    type: str = Field(default="ciscofmc", const=True)
+    type: Literal["ciscofmc"] = "ciscofmc"
 
 
 class ForcePoint(VendorAPI, RejectUnauthorized, BaseModel):
     """
     ForcePoint vendor api support
     """
 
     authenticationKey: str
     baseUrl: AnyHttpUrl
-    type: str = Field(default="forcepoint", const=True)
+    type: Literal["forcepoint"] = "forcepoint"
 
 
 class JuniperMist(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Juniper Mist vendor api support
     """
 
     apiToken: str
-    apiVer: str = Field(default="v1", const=True)
-    type: str = Field(default="juniper-mist", const=True)
+    apiVer: Literal["v1"] = "v1"
+    type: Literal["juniper-mist"] = "juniper-mist"
     baseUrl: AnyHttpUrl = "https://api.mist.com"
 
 
 class Merakiv1(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Meraki v1 vendor api support
     """
 
     apiKey: str
     baseUrl: AnyHttpUrl
     organizations: Optional[List[str]] = Field(default_factory=list)
-    apiVer: str = Field(default="v1", const=True)
-    type: str = Field(default="meraki-v0", const=True)
+    apiVer: Literal["v1"] = "v1"
+    type: Literal["meraki-v0"] = "meraki-v0"
 
 
 class NSXT(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     NSXT vendor api support
     """
 
-    type: str = Field(default="nsxT", const=True)
+    type: Literal["nsxT"] = "nsxT"
 
 
 class Prisma(VendorAPI, RejectUnauthorized, BaseModel):
     """
     Prisma vendor api support
     """
 
     username: str
     password: str
     tsgid: str
-    type: str = Field(default="prisma", const=True)
+    type: Literal["prisma"] = "prisma"
 
 
 class RuckusVirtualSmartZone(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Ruckus Virtual SmartZone vendor api support
     """
 
-    apiVer: str = Field(default="v9_1", const=True)
-    type: str = Field(default="ruckus-vsz", const=True)
+    apiVer: Literal["v9_1"] = "v9_1"
+    type: Literal["ruckus-vsz"] = "ruckus-vsz"
 
 
 class SilverPeak(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     SilverPeak vendor api support
     """
 
     loginType: str = "Local"
-    type: str = Field(default="nsxT", const=True)
+    type: Literal["nsxT"] = "nsxT"
 
-    @validator("loginType")
+    @field_validator("loginType")
+    @classmethod
     def check_region(cls, login_type):
         if login_type not in ["Local", "RADIUS", "TACACS+"]:
             raise ValueError(f"{login_type} is not a valid login type must be in ['Local', 'RADIUS', 'TACACS+']")
         return login_type
 
 
 class Versa(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Versa vendor api support
     """
 
-    type: str = Field(default="versa", const=True)
+    type: Literal["versa"] = "versa"
 
 
 class Viptela(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     Viptela vendor api support
     """
 
-    type: str = Field(default="viptela", const=True)
+    type: Literal["viptela"] = "viptela"
```

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/configuration.py` & `ipfabric-6.3.1b3/ipfabric/tools/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 from ipfabric.tools.shared import date_parser
 
 logger = logging.getLogger("ipfabric")
 
 
 class Config(BaseModel):
-    config_id: str = Field(alias="id")
+    config_id: str = Field(None, alias="id")
     sn: str
     hostname: str
-    config_hash: str = Field(alias="hash")
+    config_hash: str = Field(None, alias="hash")
     status: str
-    last_change: datetime = Field(alias="lastChangeAt")
-    last_check: datetime = Field(alias="lastCheckAt")
+    last_change: datetime = Field(None, alias="lastChangeAt")
+    last_check: datetime = Field(None, alias="lastCheckAt")
     text: Optional[str] = None
 
     def get_text_config(self, client: Any, sanitized: bool = True) -> str:
         """gets a device config
         Args:
             client: IPF Client
             sanitized: bool to determine to return sensitive data
```

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/discovery_history.py` & `ipfabric-6.3.1b3/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/dashboard.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/groups.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/factory_defaults/v6/3/intents.json` & `ipfabric-6.3.1b3/ipfabric/tools/factory_defaults/v6/3/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/nist.py` & `ipfabric-6.3.1b3/ipfabric/tools/nist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from time import sleep
-from typing import List
+from typing import List, Optional
 
 from httpx import Client, ReadTimeout, HTTPStatusError
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 
 
 class CVE(BaseModel):
     cve_id: str
     description: str
     url: str
 
@@ -16,15 +16,15 @@
     def __hash__(self):
         return hash(self.cve_id)
 
 
 class CVEs(BaseModel):
     total_results: int
     cves: List[CVE]
-    error: str = Field(default=None)
+    error: Optional[str] = None
 
 
 class NIST(Client):
     def __init__(self, nvd_api_key: str, timeout):
         """
         NIST updated to API v2.0.  You must request and pass an API Key which can be obtained at
         https://nvd.nist.gov/developers/request-an-api-key
```

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/restore_intents.py` & `ipfabric-6.3.1b3/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.3.1b3/ipfabric/tools/site_seperation_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 
 @dataclass
 class Matches:
     hostname: str
     sn: str
     old_site_name: str
-    new_site_name: Optional[str]
     rule_type: str
-    rule_number: Optional[int]
-    rule_note: Optional[str]
-    regex: Optional[str]
-    transformation: Optional[str]
+    new_site_name: Optional[str] = None
+    rule_number: Optional[int] = None
+    rule_note: Optional[str] = None
+    regex: Optional[str] = None
+    transformation: Optional[str] = None
 
 
 def check_attributes(ipf, devices):
     matches = list()
     attributes = {a["sn"]: a for a in Attributes(ipf).all(filters={"name": ["eq", "siteName"]})}
     for sn, dev in deepcopy(devices).items():
         if sn in attributes:
```

### Comparing `ipfabric-6.3.1b2/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.3.1b3/ipfabric/tools/vulnerabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from pydantic import BaseModel
 
 from ipfabric.tools.nist import NIST, CVEs
 
 
 class Version(BaseModel):
     vendor: str
-    family: Optional[str]
+    family: Optional[str] = None
     version: str
     cves: CVEs
-    hostname: Optional[str]
-    site: Optional[str]
+    hostname: Optional[str] = None
+    site: Optional[str] = None
 
 
 class Vulnerabilities:
     def __init__(self, ipf, nvd_api_key: str, timeout: int = 30):
         self.ipf = ipf
         self.nist = NIST(nvd_api_key=nvd_api_key, timeout=timeout)
```

### Comparing `ipfabric-6.3.1b2/LICENSE` & `ipfabric-6.3.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.3.1b2/pyproject.toml` & `ipfabric-6.3.1b3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.3.1b2"
+version = "v6.3.1b3"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
-    "Community Fabric <communityfabric@ipfabric.io>"
+    "Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/ip-fabric/integrations/python-ipfabric"
 repository = "https://gitlab.com/ip-fabric/integrations/python-ipfabric"
 keywords = ["ipfabric", "ip-fabric", "community-fabric"]
 
@@ -17,34 +17,38 @@
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/python-ipfabric/-/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.1"
 python-dateutil = "^2.8.2"
-pydantic = "^1.10.4"
+pydantic = "^2.0.3"
 pytz = "^2023.3"
-python-dotenv = "^1.0"
+python-dotenv = "^1.0"  # v1.0.0 requires python3.8
 pandas = {version = "^2.0", optional = true}
 openpyxl = {version = "^3.0.9", optional = true}
 tabulate = {version = ">=0.8.9,<0.10.0",  optional = true}
 python-json-logger = {version = "^2.0.4",  optional = true}
 macaddress = "~2.0.2"
 pyyaml = {version = "^6.0", optional = true}
 deepdiff = "^6.3.1"
 case-insensitive-dictionary = "^0.2.1"
+pydantic-settings = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 flake8 = "^5.0"
 black = "^22.12"
 
 [tool.poetry.extras]
 examples = ["tabulate", "pandas", "openpyxl", "python-json-logger", "pyyaml"]
+pd = ["pandas"]
+all = ["tabulate", "pandas", "openpyxl", "python-json-logger", "pyyaml"]
+
 
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

