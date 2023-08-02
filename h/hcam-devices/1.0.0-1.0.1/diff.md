# Comparing `tmp/hcam_devices-1.0.0.tar.gz` & `tmp/hcam_devices-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_devices-1.0.0.tar", last modified: Fri Jul 21 10:47:52 2023, max compression
+gzip compressed data, was "hcam_devices-1.0.1.tar", last modified: Wed Aug  2 08:22:37 2023, max compression
```

## Comparing `hcam_devices-1.0.0.tar` & `hcam_devices-1.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.202196 hcam_devices-1.0.0/
--rw-r--r--   0 sl         (501) staff       (20)      166 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3303 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      344 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     5601 2023-07-21 10:47:52.202280 hcam_devices-1.0.0/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     4587 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.192788 hcam_devices-1.0.0/hcam_devices/
--rw-r--r--   0 sl         (501) staff       (20)       96 2023-07-21 10:45:39.000000 hcam_devices-1.0.0/hcam_devices/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.193640 hcam_devices-1.0.0/hcam_devices/components/
--rw-r--r--   0 sl         (501) staff       (20)     5584 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/components/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.195293 hcam_devices-1.0.0/hcam_devices/devices/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     3228 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/devices/honeywell.py
--rw-r--r--   0 sl         (501) staff       (20)     9262 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/devices/meerstetter.py
--rw-r--r--   0 sl         (501) staff       (20)    22137 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/newport.py
--rw-r--r--   0 sl         (501) staff       (20)    11601 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/ngc.py
--rw-r--r--   0 sl         (501) staff       (20)     5308 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/pdr900.py
--rw-r--r--   0 sl         (501) staff       (20)     4293 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/properties.py
--rw-r--r--   0 sl         (501) staff       (20)     4075 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/devices/unichiller.py
--rw-r--r--   0 sl         (501) staff       (20)     9819 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/devices/zaber.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.196100 hcam_devices-1.0.0/hcam_devices/gtc/
--rw-r--r--   0 sl         (501) staff       (20)     5058 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/gtc/corba.py
--rw-r--r--   0 sl         (501) staff       (20)     3063 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/gtc/headers.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.198159 hcam_devices-1.0.0/hcam_devices/machines/
--rw-r--r--   0 sl         (501) staff       (20)      704 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     1366 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/connections.yaml
--rw-r--r--   0 sl         (501) staff       (20)     1736 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/controller.yaml
--rw-r--r--   0 sl         (501) staff       (20)     3982 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/machines/gtc.yaml
--rw-r--r--   0 sl         (501) staff       (20)     4081 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/machines/motors.yaml
--rw-r--r--   0 sl         (501) staff       (20)     1252 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/machines/sensor.yaml
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.199517 hcam_devices-1.0.0/hcam_devices/models/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     5001 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/ccd.py
--rw-r--r--   0 sl         (501) staff       (20)     7703 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/models/compo.py
--rw-r--r--   0 sl         (501) staff       (20)     2979 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/flow_sensor.py
--rw-r--r--   0 sl         (501) staff       (20)     6197 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/meerstetter.py
--rw-r--r--   0 sl         (501) staff       (20)     8967 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/ngc.py
--rw-r--r--   0 sl         (501) staff       (20)     7821 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/models/slide.py
--rw-r--r--   0 sl         (501) staff       (20)     8325 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/hcam_devices/models/telescope.py
--rw-r--r--   0 sl         (501) staff       (20)     1952 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/models/vac_gauge.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200147 hcam_devices-1.0.0/hcam_devices/testing/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     1227 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/axis.py
--rw-r--r--   0 sl         (501) staff       (20)     2989 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/fakeserial.py
--rw-r--r--   0 sl         (501) staff       (20)     2634 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/properties.py
--rw-r--r--   0 sl         (501) staff       (20)     1051 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/testing/sensors.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200493 hcam_devices-1.0.0/hcam_devices/utils/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/utils/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     3334 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/utils/filesystem.py
--rw-r--r--   0 sl         (501) staff       (20)    13201 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/utils/obsmodes.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200631 hcam_devices-1.0.0/hcam_devices/wamp/
--rw-r--r--   0 sl         (501) staff       (20)    10895 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/wamp/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.200771 hcam_devices-1.0.0/hcam_devices/wamp/utils/
--rw-r--r--   0 sl         (501) staff       (20)     2708 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/hcam_devices/wamp/utils/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.193523 hcam_devices-1.0.0/hcam_devices.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     5601 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1711 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)      153 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       13 2023-07-21 10:47:51.000000 hcam_devices-1.0.0/hcam_devices.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:47:52.202059 hcam_devices-1.0.0/scripts/
--rw-r--r--   0 sl         (501) staff       (20)     1784 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/scripts/do_wamp_call
--rw-r--r--   0 sl         (501) staff       (20)      760 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/gtcserver
--rwxr-xr-x   0 sl         (501) staff       (20)      701 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/hserver
--rwxr-xr-x   0 sl         (501) staff       (20)     7021 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/hwlogger
--rwxr-xr-x   0 sl         (501) staff       (20)     6026 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/hwserver
--rw-r--r--   0 sl         (501) staff       (20)      479 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/scripts/make_diagrams.py
--rw-r--r--   0 sl         (501) staff       (20)     1065 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/show_telemetry
--rw-r--r--   0 sl         (501) staff       (20)     7513 2022-10-19 13:15:14.000000 hcam_devices-1.0.0/scripts/tcp_serial_bridge
--rw-r--r--   0 sl         (501) staff       (20)      535 2023-07-21 10:44:48.000000 hcam_devices-1.0.0/scripts/zaber_ascii
--rw-r--r--   0 sl         (501) staff       (20)      313 2023-07-21 10:47:52.202577 hcam_devices-1.0.0/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     2512 2023-07-21 10:45:39.000000 hcam_devices-1.0.0/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.952085 hcam_devices-1.0.1/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3303 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      344 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     5601 2023-08-02 08:22:37.952158 hcam_devices-1.0.1/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     4587 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.944656 hcam_devices-1.0.1/hcam_devices/
+-rw-r--r--   0 sl         (501) staff       (20)       96 2023-08-02 08:22:19.000000 hcam_devices-1.0.1/hcam_devices/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.945438 hcam_devices-1.0.1/hcam_devices/components/
+-rw-r--r--   0 sl         (501) staff       (20)     5584 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/components/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.947329 hcam_devices-1.0.1/hcam_devices/devices/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/devices/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     3228 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/hcam_devices/devices/honeywell.py
+-rw-r--r--   0 sl         (501) staff       (20)     9262 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/hcam_devices/devices/meerstetter.py
+-rw-r--r--   0 sl         (501) staff       (20)    22137 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/devices/newport.py
+-rw-r--r--   0 sl         (501) staff       (20)    11601 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/devices/ngc.py
+-rw-r--r--   0 sl         (501) staff       (20)     5308 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/devices/pdr900.py
+-rw-r--r--   0 sl         (501) staff       (20)     4293 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/devices/properties.py
+-rw-r--r--   0 sl         (501) staff       (20)     4075 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/devices/unichiller.py
+-rw-r--r--   0 sl         (501) staff       (20)     9819 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/hcam_devices/devices/zaber.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.947707 hcam_devices-1.0.1/hcam_devices/gtc/
+-rw-r--r--   0 sl         (501) staff       (20)     5058 2023-08-02 08:20:25.000000 hcam_devices-1.0.1/hcam_devices/gtc/corba.py
+-rw-r--r--   0 sl         (501) staff       (20)     3063 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/gtc/headers.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.948603 hcam_devices-1.0.1/hcam_devices/machines/
+-rw-r--r--   0 sl         (501) staff       (20)      821 2023-07-27 22:31:34.000000 hcam_devices-1.0.1/hcam_devices/machines/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     1366 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/machines/connections.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     1736 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/machines/controller.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     3982 2023-08-02 08:20:25.000000 hcam_devices-1.0.1/hcam_devices/machines/gtc.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     4081 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/hcam_devices/machines/motors.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     1252 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/machines/sensor.yaml
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.949679 hcam_devices-1.0.1/hcam_devices/models/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/models/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     5001 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/models/ccd.py
+-rw-r--r--   0 sl         (501) staff       (20)     7703 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/hcam_devices/models/compo.py
+-rw-r--r--   0 sl         (501) staff       (20)     2979 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/models/flow_sensor.py
+-rw-r--r--   0 sl         (501) staff       (20)     6197 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/models/meerstetter.py
+-rw-r--r--   0 sl         (501) staff       (20)     8967 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/models/ngc.py
+-rw-r--r--   0 sl         (501) staff       (20)     7821 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/hcam_devices/models/slide.py
+-rw-r--r--   0 sl         (501) staff       (20)     8325 2023-08-02 08:20:25.000000 hcam_devices-1.0.1/hcam_devices/models/telescope.py
+-rw-r--r--   0 sl         (501) staff       (20)     1952 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/models/vac_gauge.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.950284 hcam_devices-1.0.1/hcam_devices/testing/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/testing/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     1227 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/testing/axis.py
+-rw-r--r--   0 sl         (501) staff       (20)     2989 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/testing/fakeserial.py
+-rw-r--r--   0 sl         (501) staff       (20)     2634 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/testing/properties.py
+-rw-r--r--   0 sl         (501) staff       (20)     1051 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/testing/sensors.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.950610 hcam_devices-1.0.1/hcam_devices/utils/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/utils/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     3334 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/utils/filesystem.py
+-rw-r--r--   0 sl         (501) staff       (20)    13737 2023-07-27 22:31:34.000000 hcam_devices-1.0.1/hcam_devices/utils/obsmodes.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.950709 hcam_devices-1.0.1/hcam_devices/wamp/
+-rw-r--r--   0 sl         (501) staff       (20)    10895 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/wamp/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.950837 hcam_devices-1.0.1/hcam_devices/wamp/utils/
+-rw-r--r--   0 sl         (501) staff       (20)     2708 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/hcam_devices/wamp/utils/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.945311 hcam_devices-1.0.1/hcam_devices.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     5601 2023-08-02 08:22:37.000000 hcam_devices-1.0.1/hcam_devices.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1711 2023-08-02 08:22:37.000000 hcam_devices-1.0.1/hcam_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-08-02 08:22:37.000000 hcam_devices-1.0.1/hcam_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-08-02 08:22:37.000000 hcam_devices-1.0.1/hcam_devices.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)      153 2023-08-02 08:22:37.000000 hcam_devices-1.0.1/hcam_devices.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       13 2023-08-02 08:22:37.000000 hcam_devices-1.0.1/hcam_devices.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:22:37.951964 hcam_devices-1.0.1/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)     1784 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/scripts/do_wamp_call
+-rw-r--r--   0 sl         (501) staff       (20)      760 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/scripts/gtcserver
+-rwxr-xr-x   0 sl         (501) staff       (20)      701 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/scripts/hserver
+-rwxr-xr-x   0 sl         (501) staff       (20)     7021 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/scripts/hwlogger
+-rwxr-xr-x   0 sl         (501) staff       (20)     6026 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/scripts/hwserver
+-rw-r--r--   0 sl         (501) staff       (20)      479 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/scripts/make_diagrams.py
+-rw-r--r--   0 sl         (501) staff       (20)     1065 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/scripts/show_telemetry
+-rw-r--r--   0 sl         (501) staff       (20)     7513 2022-10-19 13:15:14.000000 hcam_devices-1.0.1/scripts/tcp_serial_bridge
+-rw-r--r--   0 sl         (501) staff       (20)      535 2023-07-21 10:44:48.000000 hcam_devices-1.0.1/scripts/zaber_ascii
+-rw-r--r--   0 sl         (501) staff       (20)      313 2023-08-02 08:22:37.952375 hcam_devices-1.0.1/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     2512 2023-08-02 08:22:19.000000 hcam_devices-1.0.1/setup.py
```

### Comparing `hcam_devices-1.0.0/CONTRIBUTING.rst` & `hcam_devices-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/LICENSE` & `hcam_devices-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/PKG-INFO` & `hcam_devices-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_devices
-Version: 1.0.0
+Version: 1.0.1
 Summary: Device Communication via WAMP for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_devices
-Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.0.0.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.0.1.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_devices
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_devices-1.0.0/README.rst` & `hcam_devices-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/components/__init__.py` & `hcam_devices-1.0.1/hcam_devices/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/honeywell.py` & `hcam_devices-1.0.1/hcam_devices/devices/honeywell.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/meerstetter.py` & `hcam_devices-1.0.1/hcam_devices/devices/meerstetter.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/newport.py` & `hcam_devices-1.0.1/hcam_devices/devices/newport.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/ngc.py` & `hcam_devices-1.0.1/hcam_devices/devices/ngc.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/pdr900.py` & `hcam_devices-1.0.1/hcam_devices/devices/pdr900.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/properties.py` & `hcam_devices-1.0.1/hcam_devices/devices/properties.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/unichiller.py` & `hcam_devices-1.0.1/hcam_devices/devices/unichiller.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/devices/zaber.py` & `hcam_devices-1.0.1/hcam_devices/devices/zaber.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/gtc/corba.py` & `hcam_devices-1.0.1/hcam_devices/gtc/corba.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/gtc/headers.py` & `hcam_devices-1.0.1/hcam_devices/gtc/headers.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/machines/connections.yaml` & `hcam_devices-1.0.1/hcam_devices/machines/connections.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/machines/controller.yaml` & `hcam_devices-1.0.1/hcam_devices/machines/controller.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/machines/gtc.yaml` & `hcam_devices-1.0.1/hcam_devices/machines/gtc.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/machines/motors.yaml` & `hcam_devices-1.0.1/hcam_devices/machines/motors.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/machines/sensor.yaml` & `hcam_devices-1.0.1/hcam_devices/machines/sensor.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/ccd.py` & `hcam_devices-1.0.1/hcam_devices/models/ccd.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/compo.py` & `hcam_devices-1.0.1/hcam_devices/models/compo.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/flow_sensor.py` & `hcam_devices-1.0.1/hcam_devices/models/flow_sensor.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/meerstetter.py` & `hcam_devices-1.0.1/hcam_devices/models/meerstetter.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/ngc.py` & `hcam_devices-1.0.1/hcam_devices/models/ngc.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/slide.py` & `hcam_devices-1.0.1/hcam_devices/models/slide.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/telescope.py` & `hcam_devices-1.0.1/hcam_devices/models/telescope.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/models/vac_gauge.py` & `hcam_devices-1.0.1/hcam_devices/models/vac_gauge.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/testing/axis.py` & `hcam_devices-1.0.1/hcam_devices/testing/axis.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/testing/fakeserial.py` & `hcam_devices-1.0.1/hcam_devices/testing/fakeserial.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/testing/properties.py` & `hcam_devices-1.0.1/hcam_devices/testing/properties.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/testing/sensors.py` & `hcam_devices-1.0.1/hcam_devices/testing/sensors.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/utils/filesystem.py` & `hcam_devices-1.0.1/hcam_devices/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/wamp/__init__.py` & `hcam_devices-1.0.1/hcam_devices/wamp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices/wamp/utils/__init__.py` & `hcam_devices-1.0.1/hcam_devices/wamp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/hcam_devices.egg-info/PKG-INFO` & `hcam_devices-1.0.1/hcam_devices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-devices
-Version: 1.0.0
+Version: 1.0.1
 Summary: Device Communication via WAMP for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_devices
-Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.0.0.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.0.1.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_devices
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_devices-1.0.0/hcam_devices.egg-info/SOURCES.txt` & `hcam_devices-1.0.1/hcam_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/do_wamp_call` & `hcam_devices-1.0.1/scripts/do_wamp_call`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/gtcserver` & `hcam_devices-1.0.1/scripts/gtcserver`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/hserver` & `hcam_devices-1.0.1/scripts/hserver`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/hwlogger` & `hcam_devices-1.0.1/scripts/hwlogger`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/hwserver` & `hcam_devices-1.0.1/scripts/hwserver`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/show_telemetry` & `hcam_devices-1.0.1/scripts/show_telemetry`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/tcp_serial_bridge` & `hcam_devices-1.0.1/scripts/tcp_serial_bridge`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/scripts/zaber_ascii` & `hcam_devices-1.0.1/scripts/zaber_ascii`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.0.0/setup.py` & `hcam_devices-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_devices",
-    version="1.0.0",
+    version="1.0.1",
     description="Device Communication via WAMP for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_devices",
-    download_url="https://github.com/HiPERCAM/hcam_devices/archive/v1.0.0.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_devices/archive/v1.0.1.tar.gz",
     packages=[
         "hcam_devices",
         "hcam_devices.gtc",
         "hcam_devices.devices",
         "hcam_devices.components",
         "hcam_devices.machines",
         "hcam_devices.models",
```

