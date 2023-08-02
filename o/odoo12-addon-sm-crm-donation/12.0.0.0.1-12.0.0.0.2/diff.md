# Comparing `tmp/odoo12-addon-sm_crm_donation-12.0.0.0.1.tar.gz` & `tmp/odoo12-addon-sm_crm_donation-12.0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo12-addon-sm_crm_donation-12.0.0.0.1.tar", last modified: Fri Jul 28 10:30:04 2023, max compression
+gzip compressed data, was "dist/odoo12-addon-sm_crm_donation-12.0.0.0.2.tar", last modified: Wed Aug  2 15:34:43 2023, max compression
```

## Comparing `odoo12-addon-sm_crm_donation-12.0.0.0.1.tar` & `odoo12-addon-sm_crm_donation-12.0.0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.398339 odoo12-addon-sm_crm_donation-12.0.0.0.1/
--rw-r--r--   0 daniquilez  (1000) users      (984)      300 2023-07-28 10:30:04.398339 odoo12-addon-sm_crm_donation-12.0.0.0.1/PKG-INFO
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.395006 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.395006 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.395006 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/
--rw-r--r--   0 daniquilez  (1000) users      (984)       21 2023-07-28 10:22:26.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/__init__.py
--rw-r--r--   0 daniquilez  (1000) users      (984)      393 2023-07-28 10:27:34.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/__manifest__.py
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.395006 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/data/
--rw-r--r--   0 daniquilez  (1000) users      (984)      229 2023-07-28 10:22:26.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/data/utm_source_data.xml
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.395006 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/models/
--rw-r--r--   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:22:26.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/models/__init__.py
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.395006 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/views/
--rw-r--r--   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:22:26.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo/addons/sm_crm_donation/views/crm_lead_views.xml
-drwxr-xr-x   0 daniquilez  (1000) users      (984)        0 2023-07-28 10:30:04.398339 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/
--rw-r--r--   0 daniquilez  (1000) users      (984)      300 2023-07-28 10:30:04.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/PKG-INFO
--rw-r--r--   0 daniquilez  (1000) users      (984)      555 2023-07-28 10:30:04.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/SOURCES.txt
--rw-r--r--   0 daniquilez  (1000) users      (984)        1 2023-07-28 10:30:04.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/dependency_links.txt
--rw-r--r--   0 daniquilez  (1000) users      (984)        1 2023-07-28 10:30:04.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/not-zip-safe
--rw-r--r--   0 daniquilez  (1000) users      (984)       47 2023-07-28 10:30:04.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/requires.txt
--rw-r--r--   0 daniquilez  (1000) users      (984)        5 2023-07-28 10:30:04.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/top_level.txt
--rw-r--r--   0 daniquilez  (1000) users      (984)       38 2023-07-28 10:30:04.398339 odoo12-addon-sm_crm_donation-12.0.0.0.1/setup.cfg
--rw-r--r--   0 daniquilez  (1000) users      (984)      100 2023-07-28 10:26:35.000000 odoo12-addon-sm_crm_donation-12.0.0.0.1/setup.py
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      356 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/PKG-INFO
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/
+-rw-rw-r--   0 somit     (1001) somit     (1001)       21 2023-07-31 10:45:53.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/__init__.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)      521 2023-08-02 15:29:44.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/__manifest__.py
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/data/
+-rw-rw-r--   0 somit     (1001) somit     (1001)     1110 2023-08-02 15:18:49.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/data/crm_stage_data.xml
+-rw-rw-r--   0 somit     (1001) somit     (1001)      387 2023-08-02 15:18:49.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/data/crm_team_data.xml
+-rw-rw-r--   0 somit     (1001) somit     (1001)      229 2023-08-01 07:20:29.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/data/utm_source_data.xml
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/models/
+-rw-rw-r--   0 somit     (1001) somit     (1001)        0 2023-08-02 15:13:14.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/models/__init__.py
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/views/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      611 2023-08-02 15:18:49.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo/addons/sm_crm_donation/views/crm_lead_views.xml
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      356 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/PKG-INFO
+-rw-rw-r--   0 somit     (1001) somit     (1001)      658 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/SOURCES.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)        1 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/dependency_links.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)        1 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/not-zip-safe
+-rw-rw-r--   0 somit     (1001) somit     (1001)       80 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/requires.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)        5 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/top_level.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)       38 2023-08-02 15:34:43.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/setup.cfg
+-rw-rw-r--   0 somit     (1001) somit     (1001)      100 2023-07-31 10:45:53.000000 odoo12-addon-sm_crm_donation-12.0.0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `odoo12-addon-sm_crm_donation-12.0.0.0.1/odoo12_addon_sm_crm_donation.egg-info/SOURCES.txt` & `odoo12-addon-sm_crm_donation-12.0.0.0.2/odoo12_addon_sm_crm_donation.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 setup.py
 odoo/addons/sm_crm_donation/__init__.py
 odoo/addons/sm_crm_donation/__manifest__.py
+odoo/addons/sm_crm_donation/data/crm_stage_data.xml
+odoo/addons/sm_crm_donation/data/crm_team_data.xml
 odoo/addons/sm_crm_donation/data/utm_source_data.xml
 odoo/addons/sm_crm_donation/models/__init__.py
 odoo/addons/sm_crm_donation/views/crm_lead_views.xml
 odoo12_addon_sm_crm_donation.egg-info/PKG-INFO
 odoo12_addon_sm_crm_donation.egg-info/SOURCES.txt
 odoo12_addon_sm_crm_donation.egg-info/dependency_links.txt
 odoo12_addon_sm_crm_donation.egg-info/not-zip-safe
```

