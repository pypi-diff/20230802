# Comparing `tmp/RobertCommonDriver-0.1.46.tar.gz` & `tmp/RobertCommonDriver-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.46.tar", last modified: Mon Jul 24 01:53:55 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.47.tar", last modified: Wed Aug  2 02:33:59 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.46.tar` & `RobertCommonDriver-0.1.47.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:55.014632 RobertCommonDriver-0.1.46/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.46/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.46/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2023-07-24 01:53:55.013347 RobertCommonDriver-0.1.46/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.46/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.907416 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-24 01:53:54.000000 RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      212 2023-06-30 06:01:07.000000 RobertCommonDriver-0.1.46/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.908423 RobertCommonDriver-0.1.46/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.46/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.909425 RobertCommonDriver-0.1.46/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.932626 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.959496 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    69091 2023-07-19 08:00:33.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    95594 2023-07-21 10:00:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    78954 2023-07-14 14:41:30.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32745 2023-07-21 02:43:14.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-07-24 01:53:55.014632 RobertCommonDriver-0.1.46/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-07-24 01:52:25.000000 RobertCommonDriver-0.1.46/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.960493 RobertCommonDriver-0.1.46/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.46/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.961496 RobertCommonDriver-0.1.46/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.46/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:54.980735 RobertCommonDriver-0.1.46/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:53:55.012125 RobertCommonDriver-0.1.46/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     2245 2023-07-20 08:04:16.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9630 2023-07-20 10:41:51.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:59.042779 RobertCommonDriver-0.1.47/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.47/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.47/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-08-02 02:33:59.042779 RobertCommonDriver-0.1.47/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.47/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.936182 RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-08-02 02:33:58.000000 RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-08-02 02:33:58.000000 RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:33:58.000000 RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2023-08-02 02:33:58.000000 RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 02:33:58.000000 RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2023-07-29 08:14:49.000000 RobertCommonDriver-0.1.47/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.937181 RobertCommonDriver-0.1.47/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.47/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.938690 RobertCommonDriver-0.1.47/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.955850 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.983158 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    69640 2023-07-28 15:24:15.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566106 2023-06-15 07:05:44.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0   101229 2023-07-27 06:16:09.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    78958 2023-08-02 02:31:15.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    34947 2023-07-31 04:04:12.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    45078 2023-07-31 03:14:23.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:33:59.043784 RobertCommonDriver-0.1.47/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-07-31 03:26:47.000000 RobertCommonDriver-0.1.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.984159 RobertCommonDriver-0.1.47/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.47/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:58.985169 RobertCommonDriver-0.1.47/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.47/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:59.000187 RobertCommonDriver-0.1.47/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:33:59.040610 RobertCommonDriver-0.1.47/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     4147 2023-07-27 06:18:04.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     5502 2023-07-14 12:58:58.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9674 2023-07-31 03:26:47.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4145 2023-07-27 06:41:53.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.46/LICENSE` & `RobertCommonDriver-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/PKG-INFO` & `RobertCommonDriver-0.1.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.46
+Version: 0.1.47
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.46
+Version: 0.1.47
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.46/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.47/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,26 @@
 disable_warnings(InsecureRequestWarning)
 
 JsonType = TypeVar('JsonType')
 
 
 class IOTBaseCommon:
 
+    class IOTConnectException(Exception):
+        """连接异常"""
+        pass
+
+    class IOTReadException(Exception):
+        """读取异常"""
+        pass
+
+    class IOTWriteException(Exception):
+        """写值异常"""
+        pass
+
     class CloseException(Exception):
         pass
 
     class NormalException(Exception):
         pass
 
     class DataTransform:
@@ -996,19 +1008,20 @@
                 return IOTBaseCommon.IOTNetResult.create_success([IOTBaseCommon.DataTransform.cat_bytes(net_msg.heads, net_msg.contents)])
 
         def get_connected(self):
             return self.iot_socket is not None
 
     class IOTNetworkClient(IOTNetworkBase):
 
-        def __init__(self, host: str, port: int, timeout: Optional[Union[int, float]] = None):
+        def __init__(self, host: str, port: int, timeout: Optional[Union[int, float]] = None, conn_retries: int = 1):
             super().__init__()
             self.host = host
             self.port = port
             self.timeout = timeout
+            self.conn_retries = conn_retries
             self.lock = Lock()
             self.socket_error = False
             self.is_persistent: bool = True     # 是否长连接模式
 
         @abstractmethod
         def get_net_msg(self):
             """获取一个新的消息对象的方法，需要在继承类里面进行重写"""
@@ -1109,19 +1122,23 @@
             return self.unpack_response(send_value, result_receive.contents[0]) if pack_unpack else result_receive
 
         def read_server(self, send: bytearray):
             """使用底层的数据报文来通讯，传入需要发送的消息，返回一条完整的数据指令"""
             result = IOTBaseCommon.IOTNetResult()
             with self.lock:
                 # 获取有用的网络通道，如果没有，就建立新的连接
-                result_socket = self.get_socket()
-                if result_socket.is_success is False:
-                    self.socket_error = True
-                    result.copy(result_socket)
-                    return result
+                for i in range(self.conn_retries):  # S7200需要连接两次
+                    result_socket = self.get_socket()
+                    if result_socket.is_success is True:
+                        break
+                    else:
+                        if i == self.conn_retries - 1:
+                            self.socket_error = True
+                            result.copy(result_socket)
+                            return result
 
                 read = self.read_from_socket(result_socket.contents[0], send)
                 if read.is_success:
                     self.socket_error = False
                     result.is_success = read.is_success
                     result.contents[0] = read.contents[0]
                     result.msg = f"Success"
```

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_iec104.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from scapy.fields import ByteEnumField, BitEnumField, BitField, ConditionalField, Field, PacketField, LEShortField, ShortField, XByteField, ByteField, PacketListField
 from scapy.packet import Packet, Padding, NoPayload
 from struct import unpack, pack
 from typing import List, Dict, Any, Optional
+from threading import Event
 
 from .base import IOTBaseCommon, IOTDriver
 
 
 '''
 pip install scapy==2.4.5
 '''
@@ -103,59 +104,83 @@
     主站收到从站发送的结束帧，会回复一个S帧的确认帧；
     进入下一个周期（其中如何数据有变化，从站需要主动上报）
 """
 
 
 class IECDefine:
 
+    # 显示类型
+    ASDU_DISPLAY = 0    # 0 原值 1 英文 2 中文
+
+    @staticmethod
+    def convert_dispay(maps: dict, value: Any, type: int = 1):
+        """转换显示"""
+        if type == 1:
+            if isinstance(maps, dict):
+                values = maps.get(value, ['', ''])
+                if isinstance(values, list):
+                    if len(values) >= 2:
+                        return values[0]
+                else:
+                    return values
+        elif type == 2:
+            if isinstance(maps, dict):
+                values = maps.get(value, ['', ''])
+                if isinstance(values, list):
+                    if len(values) >= 2:
+                        return values[1]
+                else:
+                    return values
+        return value
+
     # 类型标识(1字节)
     ASDU_TYPE = {
-        0x01: 'M_SP_NA_1',  # 单点遥信(带品质描述 不带时标)
-        0x03: 'M_DP_NA_1',  # 双点遥信(带品质描述 不带时标)
-        0x05: 'M_ST_NA_1',  # 步位置信息(带品质描述 不带时标)
-        0x07: 'M_BO_NA_1',  # 32比特串(带品质描述 不带时标)
-        0x09: 'M_ME_NA_1',  # 规一化遥测值(带品质描述 不带时标)
-        0x0B: 'M_ME_NB_1',  # 标度化遥测值(带品质描述 不带时标)
-        0x0D: 'M_ME_NC_1',  # 短浮点遥测值(带品质描述 不带时标)
-        0x0F: 'M_IT_NA_1',  # 累积量(带品质描述 不带时标)
-        0x14: 'M_PS_NA_1',  # 成组单点遥信(只带变量标志)
-        0x15: 'M_ME_ND_1',  # 规一化遥测值(不带品质描述 不带时标)
-        0x1E: 'M_SP_TB_1',  # 单点遥信(带品质描述 带绝对时标)
-        0x1F: 'M_DP_TB_1',  # 双点遥信(带品质描述 带绝对时标)
-        0x20: 'M_ST_TB_1',  # 步位置信息(带品质描述 带绝对时标)
-        0x21: 'M_BO_TB_1',  # 32比特串(带品质描述 带绝对时标)
-        0x22: 'M_ME_TD_1',  # 规一化遥测值(带品质描述 带绝对时标)
-        0x23: 'M_ME_TE_1',  # 标度化遥测值(带品质描述 带绝对时标)
-        0x24: 'M_ME_TF_1',  # 短浮点遥测值(带品质描述 带绝对时标)
-        0x25: 'M_IT_TB_1',  # 累积量(带品质描述 带绝对时标)
-        0x26: 'M_EP_TD_1',  # 继电保护装置事件(带品质描述 带绝对时标)
-        0x27: 'M_EP_TE_1',  # 继电保护装置成组启动事件(带品质描述 带绝对时标)
-        0x28: 'M_EP_TF_1',  # 继电保护装置成组出口信息(带品质描述 带绝对时标)
-        0x2D: 'C_SC_NA_1',  # 单点遥控(一个报文只有一个遥控信息体 不带时标)
-        0x2E: 'C_DC_NA_1',  # 双点遥控(一个报文只有一个遥控信息体 不带时标)
-        0x2F: 'C_RC_NA_1',  # 升降遥控(一个报文只有一个遥控信息体 不带时标)
-        0x30: 'C_SE_NA_1',  # 规一化设定值(一个报文只有一个设定值 不带时标)
-        0x31: 'C_SE_NB_1',  # 标度化设定值(一个报文只有一个设定值 不带时标)
-        0x32: 'C_SE_NC_1',  # 短浮点设定值(一个报文只有一个设定值 不带时标)
-        0x33: 'C_SE_ND_1',  # 32比特串(一个报文只有一个设定值 不带时标)
-        0x3A: 'C_SE_TA_1',  # 单点遥控(一个报文只有一个设定值 带时标)
-        0x3B: 'C_SE_TB_1',  # 双点遥控(一个报文只有一个设定值 带时标)
-        0x3C: 'C_SE_TC_1',  # 升降遥控(一个报文只有一个设定值 带时标)
-        0x3D: 'C_SE_TD_1',  # 规一化设定值(一个报文只有一个设定值 带时标)
-        0x3E: 'C_SE_TE_1',  # 标度化设定值(一个报文只有一个设定值 带时标)
-        0x3F: 'C_SE_TF_1',  # 短浮点设定值(一个报文只有一个设定值 带时标)
-        0x40: 'C_SE_TG_1',  # 32比特串(一个报文只有一个设定值 带时标)
-        0x46: 'M_EI_NA_1',  # 初始化结束(从站发送，主站收到时候会做一次总召)
-        0x64: 'C_IC_NA_1',  # 总召
-        0x65: 'C_CI_NA_1',  # 累积量召唤
-        0x66: 'C_RD_NA_1',  # 读命令
-        0x67: 'C_CS_NA_1',  # 时钟同步命令
-        0x69: 'C_RS_NA_1',  # 复位进程命令
-        0x6B: 'C_TS_NA_1',  # 带时标的测试命令
-        0x88: 'C_SE_NE_1',  # 规一化设定值(一个报文可以包含多个设定值 不带时标)
+        0x01:  'M_SP_NA_1',    #单点遥信(带品质描述 不带时标)
+        0x03:  'M_DP_NA_1',    #双点遥信(带品质描述 不带时标)
+        0x05:  'M_ST_NA_1',    #步位置信息(带品质描述 不带时标)
+        0x07:  'M_BO_NA_1',    #32比特串(带品质描述 不带时标)
+        0x09:  'M_ME_NA_1',    #规一化遥测值(带品质描述 不带时标)
+        0x0B:  'M_ME_NB_1',    #标度化遥测值(带品质描述 不带时标)
+        0x0D:  'M_ME_NC_1',    #短浮点遥测值(带品质描述 不带时标)
+        0x0F:  'M_IT_NA_1',    #累积量(带品质描述 不带时标)
+        0x14:  'M_PS_NA_1',    #成组单点遥信(只带变量标志)
+        0x15:  'M_ME_ND_1',    #规一化遥测值(不带品质描述 不带时标)
+        0x1E:  'M_SP_TB_1',    #单点遥信(带品质描述 带绝对时标)
+        0x1F:  'M_DP_TB_1',    #双点遥信(带品质描述 带绝对时标)
+        0x20:  'M_ST_TB_1',    #步位置信息(带品质描述 带绝对时标)
+        0x21:  'M_BO_TB_1',    #32比特串(带品质描述 带绝对时标)
+        0x22:  'M_ME_TD_1',    #规一化遥测值(带品质描述 带绝对时标)
+        0x23:  'M_ME_TE_1',    #标度化遥测值(带品质描述 带绝对时标)
+        0x24:  'M_ME_TF_1',    #短浮点遥测值(带品质描述 带绝对时标)
+        0x25:  'M_IT_TB_1',    #累积量(带品质描述 带绝对时标)
+        0x26:  'M_EP_TD_1',    #继电保护装置事件(带品质描述 带绝对时标)
+        0x27:  'M_EP_TE_1',    #继电保护装置成组启动事件(带品质描述 带绝对时标)
+        0x28:  'M_EP_TF_1',    #继电保护装置成组出口信息(带品质描述 带绝对时标)
+        0x2D:  'C_SC_NA_1',    #单点遥控(一个报文只有一个遥控信息体 不带时标)
+        0x2E:  'C_DC_NA_1',    #双点遥控(一个报文只有一个遥控信息体 不带时标)
+        0x2F:  'C_RC_NA_1',    #升降遥控(一个报文只有一个遥控信息体 不带时标)
+        0x30:  'C_SE_NA_1',    #规一化设定值(一个报文只有一个设定值 不带时标)
+        0x31:  'C_SE_NB_1',    #标度化设定值(一个报文只有一个设定值 不带时标)
+        0x32:  'C_SE_NC_1',    #短浮点设定值(一个报文只有一个设定值 不带时标)
+        0x33:  'C_SE_ND_1',    #32比特串(一个报文只有一个设定值 不带时标)
+        0x3A:  'C_SE_TA_1',    #单点遥控(一个报文只有一个设定值 带时标)
+        0x3B:  'C_SE_TB_1',    #双点遥控(一个报文只有一个设定值 带时标)
+        0x3C:  'C_SE_TC_1',    #升降遥控(一个报文只有一个设定值 带时标)
+        0x3D:  'C_SE_TD_1',    #规一化设定值(一个报文只有一个设定值 带时标)
+        0x3E:  'C_SE_TE_1',    #标度化设定值(一个报文只有一个设定值 带时标)
+        0x3F:  'C_SE_TF_1',    #短浮点设定值(一个报文只有一个设定值 带时标)
+        0x40:  'C_SE_TG_1',    #32比特串(一个报文只有一个设定值 带时标)
+        0x46:  'M_EI_NA_1',    #初始化结束(从站发送，主站收到时候会做一次总召)
+        0x64:  'C_IC_NA_1',    #总召
+        0x65:  'C_CI_NA_1',    #累积量召唤
+        0x66:  'C_RD_NA_1',    #读命令
+        0x67:  'C_CS_NA_1',    #时钟同步命令
+        0x69:  'C_RS_NA_1',    #复位进程命令
+        0x6B:  'C_TS_NA_1',    #带时标的测试命令
+        0x88:  'C_SE_NE_1',    #规一化设定值(一个报文可以包含多个设定值 不带时标)
     }
 
     # 帧类型
     APCI_TYPE = {
         0x00: 'I',
         0x01: 'S',
         0x03: 'U'
@@ -512,109 +537,109 @@
     ASDU_GS = {
         0x01: 'total startup',
         0x00: 'no total start',
     }
 
     # A相保护
     ASDU_SL_A = {
-        0x01: 'A相保护启动',
-        0x00: 'A相保护未启动',
+        0x01: 'A-phase protection activation',     # A相保护启动
+        0x00: 'A-phase protection not activated',        # A相保护未启动
     }
 
     ASDU_SL_B = {
-        0x01: 'B相保护启动',
-        0x00: 'B相保护未启动',
+        0x01: 'B-phase protection activation',     # B相保护启动
+        0x00: 'B-phase protection not activated',    # B相保护未启动
     }
 
     ASDU_SL_C = {
-        0x01: 'C相保护启动',
-        0x00: 'C相保护未启动',
+        0x01: 'C-phase protection activation',      # C相保护启动
+        0x00: 'C-phase protection not activated',   # C相保护未启动
     }
 
     ASDU_SLE = {
-        0x01: '接地电流保护启动',
-        0x00: '接地电流保护未启动',
+        0x01: 'Ground current protection activation',   # 接地电流保护启动
+        0x00: 'Ground current protection not activated',  # 接地电流保护未启动
     }
 
     ASDU_SRD = {
-        0x01: '反向保护启动',
-        0x00: '反向保护未启动',
+        0x01: 'reverse protection activation',     # 反向保护启动
+        0x00: 'reverse protection not activated',    # 反向保护未启动
     }
 
     ASDU_GC = {
-        0x01: '总命令输出至输出电路',
-        0x00: '无总命令输出至输出电路',
+        0x01: 'general command output to output circuit',     # 总命令输出至输出电路
+        0x00: 'no general command output to output circuit',    # 无总命令输出至输出电路
     }
 
     ASDU_GL_A = {
-        0x01: '命令输出至A相输出电路',
-        0x00: '无命令输出至A相输出电路',
+        0x01: 'command output to A-phase output circuit',    # 命令输出至A相输出电路
+        0x00: 'no command output to A-phase output circuit',   # 无命令输出至A相输出电路
     }
 
     ASDU_GL_B = {
-        0x01: '命令输出至B相输出电路',
-        0x00: '无命令输出至B相输出电路',
+        0x01: 'command output to B-phase output circuit',    # 命令输出至B相输出电路
+        0x00: 'no command output to B-phase output circuit',   # 无命令输出至B相输出电路
     }
 
     ASDU_GL_C = {
-        0x01: '命令输出至C相输出电路',
-        0x00: '无命令输出至C相输出电路',
+        0x01: 'command output to C-phase output circuit',    # 命令输出至C相输出电路
+        0x00: 'no command output to C-phase output circuit',   # 无命令输出至C相输出电路
     }
 
     # 参数种类
     ASDU_KPA = {
-        0x00: '未用',
-        0x01: '门限值',
-        0x02: '平滑系数（滤波时间常数）',
-        0x03: '传送测量值的下限',
-        0x04: '传送测量值的上限',
+        0x00: 'unused',     # 未用
+        0x01: 'threshold',    # 门限值
+        0x02: 'smoothing coefficient (filtering time constant)',   # 平滑系数（滤波时间常数）
+        0x03: 'lower limit for transmitting measurement values',   # 传送测量值的下限
+        0x04: 'upper limit for transmitting measurement values',   # 传送测量值的上限
     }
 
     for i in range(5, 32):
-        ASDU_KPA[i] = f"标准测量值参数限定词{i}"
+        ASDU_KPA[i] = f"standard measured value parameter determiner {i}"  # 标准测量值参数限定词
 
     for i in range(32, 64):
-        ASDU_KPA[i] = f"特定测量值参数限定词{i}"
+        ASDU_KPA[i] = f"specific measured value parameter determiner{i}"  # 特定测量值参数限定词
 
     # 当地参数改变
     ASDU_LPC = {
-        0x01: '改变',
-        0x00: '未改变',
+        0x01: 'change', # 改变
+        0x00: 'unchanged',    # 未改变
     }
 
     # 参数在运行
     ASDU_POP = {
-        0x01: '未运行',
-        0x00: '运行',
+        0x01: 'not running',    # 未运行
+        0x00: 'running',     # 运行
     }
 
     ASDU_QPA = {
-        0x00: '未用',
-        0x01: '激活/停止激活之前装载的参数(信息对象地址=0)',
-        0x02: '激活/停止激活所寻址信息对象的参数',
-        0x03: '激活/停止激活所寻址的持续循环或周期传输的信息对象',
+        0x00: 'unused',     # 未用
+        0x01: 'activate/stop the parameters loaded before activation (information object address=0)',   # 激活/停止激活之前装载的参数(信息对象地址=0)
+        0x02: 'activate/deactivate the parameters of the addressed information object',  # 激活/停止激活所寻址信息对象的参数
+        0x03: 'activating/deactivating the addressed information object for continuous cyclic or periodic transmission',  # 激活/停止激活所寻址的持续循环或周期传输的信息对象
     }
 
     for i in range(4, 128):
-        ASDU_QPA[i] = f"标准参数激活限定词{i}"
+        ASDU_QPA[i] = f"standard parameter activation determiner {i}"   # 标准参数激活限定词
 
     for i in range(128, 256):
-        ASDU_QPA[i] = f"特定参数激活限定词{i}"
+        ASDU_QPA[i] = f"specific parameter activation determiner{i}"   # 特定参数激活限定词
 
     ASDU_QRP = {
-        0x00: '未采用',
-        0x01: '进程的总复位',
-        0x02: '复位事件缓冲区等待处理的带时标的信息',
+        0x00: 'not adopted',    # 未采用
+        0x01: 'total reset of processes',   # 进程的总复位
+        0x02: 'reset the time marked information waiting for processing in the event buffer',     # 复位事件缓冲区等待处理的带时标的信息
     }
 
     for i in range(3, 128):
-        ASDU_QRP[i] = f"标准复位进程命令限定词{i}"
+        ASDU_QRP[i] = f"standard reset process command determiner {i}"     # 标准复位进程命令限定词
 
     for i in range(128, 256):
-        ASDU_QRP[i] = f"特定复位进程命令限定词{i}"
+        ASDU_QRP[i] = f"specific reset process command determiner {i}"     # 特定复位进程命令限定词
 
     # 初始化原因
     ASDU_U17 = {
         0x00: 'Local power switch on',
         0x01: 'Local manual reset',
         0x02: 'Remote reset',
     }
@@ -800,16 +825,16 @@
             ByteField('CY', None),    #
             ByteField('CA', None),
             ByteField('IV', None)
         ]
 
         def do_dissect(self, s):
             cp8 = s[4]
-            self.V = unpack('<i', s[:4])
-            self.SQ = unpack('B', cp8 & 0b11111)
+            self.V = unpack('<i', s[:4])[0]
+            self.SQ = cp8 & 0b11111
             self.CY = IECDefine.ASDU_OV[cp8 & 0b100000]
             self.CA = IECDefine.ASDU_CA[cp8 & 0b1000000]
             self.IV = IECDefine.ASDU_IV[cp8 & 0b10000000]
             return s[5:]
 
         def extract_padding(self, s):
             return None, s
@@ -884,15 +909,14 @@
         def extract_padding(self, s):
             return None, s
 
     class BSI(Packet):
         """7.2.6.13 二进制状态信息"""
         name = 'BSI'
         fields_desc = [
-            ByteField('RAM', None),     # 运行中RAM异常
             ByteField('LSS', None),     # 当地显示子系统
             ByteField('RAM', None),  # 变位遥信使遥控 升降 设定命令取消
             ByteField('UPS', None),  # UPS状态
             ByteField('AGC', None),  # 自动发电控制
             ByteField('TRRL', None),  # 遥控转当地
             ByteField('U', None),  # 无人值班
             ByteField('SR', None),  # 系统重新启动
@@ -2024,22 +2048,24 @@
         1: IOA1,    # 单点遥信(带品质描述 不带时标)
         3: IOA3,    # 双点遥信(带品质描述 不带时标)
         5: IOA5,    # 步位置信息(带品质描述 不带时标)
         7: IOA7,    # 32比特串(带品质描述 不带时标)
         9: IOA9,    # 规一化遥测值(带品质描述 不带时标)
         11: IOA11,  # 短浮点遥测值(带品质描述 不带时标)
         13: IOA13,  # 短浮点遥测值(带品质描述 不带时标)
+        15: IOA15,  # 累积量(带品质描述 不带时标)
         30: IOA30,  # 单点遥信(带品质描述 带绝对时标)
         31: IOA31,  # 双点遥信(带品质描述 带绝对时标)
         36: IOA36,  # 短浮点遥测值(带品质描述 带绝对时标)
         37: IOA37,   # 累积量(带品质描述 带绝对时标)
         45: IOA45,  # 单点遥控(一个报文只有一个遥控信息体 不带时标)
         50: IOA50,   # 短浮点设定值(一个报文只有一个设定值 不带时标)
         70: IOA70,   # 初始化结束(从站发送，主站收到时候会做一次总召)
         100: IOA100,    # 总召
+        101: IOA101,  # 电能脉冲召唤命令
         103: IOA103,     # 时钟同步命令
     }
 
     IOALEN = {
         1: 4,
         2: 7,
         3: 4,
@@ -2297,16 +2323,19 @@
 
         self.reinit()
 
     def reinit(self):
         self.client = None
         self.is_connected = False
         self.ole_zongzhao = IOTBaseCommon.get_datetime()    # 总召时间
-        self.ole_recv = IOTBaseCommon.get_datetime()    # 收到回复数据时间
+        self.ole_dianneng = IOTBaseCommon.get_datetime()    # 电能召唤时间
+        self.ole_recv = IOTBaseCommon.get_datetime()  # 收到回复数据时间
 
+        self.event_zongzhao = None   # 总召事件激活
+        self.event_dianneng = None  # 电能
         self.values = {}
         self.send_count = 0
         self.recv_count = 0
 
     def exit(self):
         self._release_client()
 
@@ -2327,14 +2356,16 @@
         elif type == 'config':
             templates.extend([
                 {'required': True, 'name': '地址' if lan == 'ch' else 'Host', 'code': 'host', 'type': 'string', 'default': '192.168.1.1', 'enum': [], 'tip': ''},
                 {'required': True, 'name': '端口' if lan == 'ch' else 'Port', 'code': 'port', 'type': 'int', 'default': 2404, 'enum': [], 'tip': ''},
                 {'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'float', 'default': 10, 'enum': [], 'tip': ''},
                 {'required': False, 'name': '总召(s)' if lan == 'ch' else 'ZongZhao Interval(s)', 'code': 'zongzhao_interval', 'type': 'int', 'default': 900, 'enum': [], 'tip': ''},
                 {'required': False, 'name': '总召超时(s)' if lan == 'ch' else 'ZongZhao Timeout(s)', 'code': 'zongzhao_timeout', 'type': 'int', 'default': 30, 'enum': [], 'tip': ''},
+                {'required': False, 'name': '电能召唤(s)' if lan == 'ch' else 'DianNeng Interval(s)', 'code': 'dianneng_interval', 'type': 'int', 'default': 60, 'enum': [], 'tip': ''},
+                {'required': False, 'name': '电能召唤超时(s)' if lan == 'ch' else 'DianNeng Timeout(s)', 'code': 'dianneng_timeout', 'type': 'int', 'default': 30, 'enum': [], 'tip': ''},
                 {'required': False, 'name': 'S帧' if lan == 'ch' else 'S Interval', 'code': 's_interval', 'type': 'int', 'default': 0, 'enum': [], 'tip': ''},
                 {'required': False, 'name': '超时U帧测试(s)' if lan == 'ch' else 'U Test Timeout(s)', 'code': 'u_test_timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''},    # 超时发送U帧
             ])
 
         return templates
 
     def read(self, **kwargs):
@@ -2464,15 +2495,16 @@
                         if self.recv_count % (2 * s_interval)  == 0:
                             self._send_s_frame(client)
 
                     if type_id == 100:  # 总召
                         if cause_id == 7:   # 总召确认
                             pass
                         elif cause_id == 10:   # 总召结束
-                            pass
+                            if self.event_zongzhao:
+                                self.event_zongzhao.set()
                     elif type_id in [1, 30]:  # 单点遥信(带品质描述 不带时标) 单点遥信(带品质描述 带绝对时标)
                         for ioa in asdu.get('IOA', []):
                             if 'SIQ' in ioa.keys():
                                 self._update_value(type_id, ioa.get('IOA'), ioa.get('SIQ').get('SPI'))
                     elif type_id in [3, 31]:  # 双点遥信(带品质描述 不带时标) 双点遥信(带品质描述 带绝对时标)
                         for ioa in asdu.get('IOA', []):
                             if 'DIQ' in ioa.keys():
@@ -2491,20 +2523,28 @@
                         for ioa in asdu.get('IOA', []):
                             if 'SVA' in ioa.keys():
                                 self._update_value(type_id, ioa.get('IOA'), ioa.get('SVA'))
                     elif type_id in [13, 36]:     # 短浮点遥测值(带品质描述 不带时标) 短浮点遥测值(带品质描述 带绝对时标)
                         for ioa in asdu.get('IOA', []):
                             if 'Value' in ioa.keys():
                                 self._update_value(type_id, ioa.get('IOA'), ioa.get('Value'))
-                    elif type_id == 37:  # 累积量(带品质描述 带绝对时标)
-                        pass
+                    elif type_id in [15, 37]:  # 累积量(带品质描述 不带时标)
+                        for ioa in asdu.get('IOA', []):
+                            if 'V' in ioa.get('BCR', {}).keys():
+                                self._update_value(type_id, ioa.get('IOA'), ioa.get('BCR', {}).get('V'))
                     elif type_id == 45:     # 单点遥控(一个报文只有一个遥控信息体 不带时标)
                         pass
                     elif type_id == 50:     # 短浮点设定值(一个报文只有一个设定值 不带时标)
                         pass
+                    elif type_id == 101:    # 电能脉冲召唤命令
+                        if cause_id == 7:   # 电能确认
+                            pass
+                        elif cause_id == 10:   # 电能结束
+                            if self.event_dianneng is not None:
+                                self.event_dianneng.set()
                     elif type_id == 103:    # 时钟同步
                         pass
                 elif type == 1:  # S帧
                     self.logging(content=f"iec104({client}) recv S: [{self.format_bytes(datas)}]", pos=self.stack_pos)
                 elif type == 3:
                     self.logging(content=f"iec104({client}) recv U: [{self.format_bytes(datas)}]", pos=self.stack_pos)
                     if info.get('ACPI', {}).get('UType') == 0x02:  # U帧激活确认 发送总召命令
@@ -2551,17 +2591,29 @@
     # 发送总召命令
     def _send_zongzhao(self, client):
         if client is not None:
             pkt = IOTIEC104.APDU()
             pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.send_count, Rx=self.recv_count)
             pkt /= IOTIEC104.ASDU(Type=100, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[100](IOA=0, QOI=0x14)])
 
+            self.event_zongzhao = Event()
             self._send_frame(100, 6, pkt.build())
             self.ole_zongzhao = IOTBaseCommon.get_datetime()
 
+    # 发送电能脉冲召唤命令
+    def _send_dianneng(self, client):
+        if client is not None:
+            pkt = IOTIEC104.APDU()
+            pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=self.send_count, Rx=self.recv_count)
+            pkt /= IOTIEC104.ASDU(Type=101, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[101](IOA=0, QCC=IECPacket.QCC(RQT=0, FRZ=0))])
+
+            self.event_dianneng = Event()
+            self._send_frame(101, 6, pkt.build())
+            self.ole_dianneng = IOTBaseCommon.get_datetime()
+
     def _send_u_test_frame(self, client, utype: int = 0x10):
         """发送U帧测试帧"""
         if client is not None:
             start_frame = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x03, UType=utype)).build()
             self.logging(content=f"iec104({client}) U ({self.format_bytes(start_frame)})", pos=self.stack_pos)
             client.send(start_frame)
             self.ole_recv = IOTBaseCommon.get_datetime()
@@ -2571,24 +2623,45 @@
         if client is not None:
             start_frame = (IOTIEC104.APDU() / IOTIEC104.APCI(ApduLen=4, Type=0x01, Rx=self.recv_count)).build()
             self.logging(content=f"iec104({client}) S ({self.format_bytes(start_frame)})", pos=self.stack_pos)
             client.send(start_frame)
 
     def send_zongzhao_thread(self):
         """总召轮询"""
-        zongzhao_interval = self.configs.get('zongzhao_interval', 0)
-        if zongzhao_interval > 0:
-            while self.is_connected:
-                self.delay(1)
+        while self.is_connected:
+            self.delay(1)
+
+            # 等待电能结束事件
+            dianneng_timeout = self.configs.get('dianneng_timeout', 30)
+            if self.event_dianneng is not None and self.event_dianneng.is_set() is False and (IOTBaseCommon.get_datetime() - self.ole_dianneng).total_seconds() <= dianneng_timeout:  # 尚未收到电能结束命令
+                continue
+
+            # 先发总召
+            zongzhao_interval = self.configs.get('zongzhao_interval', 0)
+            if zongzhao_interval > 0:
                 if (IOTBaseCommon.get_datetime() - self.ole_zongzhao).total_seconds() >= zongzhao_interval:
                     try:
                         self._send_zongzhao(self.client)
                     except:
                         pass
 
+            # 等待总召结束事件
+            zongzhao_timeout = self.configs.get('zongzhao_timeout', 30)
+            if self.event_zongzhao is not None and self.event_zongzhao.is_set() is False and (IOTBaseCommon.get_datetime() - self.ole_zongzhao).total_seconds() <= zongzhao_timeout:    # 尚未收到总召结束命令
+                continue
+
+            # 发送电能脉冲召唤命令
+            dianneng_interval = self.configs.get('dianneng_interval', 0)
+            if dianneng_interval > 0:
+                if (IOTBaseCommon.get_datetime() - self.ole_dianneng).total_seconds() >= dianneng_interval:
+                    try:
+                        self._send_dianneng(self.client)
+                    except:
+                        pass
+
     def send_u_test_thread(self):
         """发送U帧测试帧 超过一定时间没有下发报文或者装置没有上送任何报文"""
         u_test_timeout = self.configs.get('u_test_timeout', 10)
         if u_test_timeout > 0:
             while self.is_connected:
                 self.delay(1)
                 if (IOTBaseCommon.get_datetime() - self.ole_recv).total_seconds() >= u_test_timeout:
```

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import logging
 import time
 import sys
-import winreg
 import Pyro5.core
 
 from datetime import datetime
 from enum import IntEnum
 from os import getenv as os_getenv, path as os_path, getpid, system as os_system
 from psutil import Process
 from platform import system as platform_system
@@ -19,14 +18,15 @@
 from typing import Optional, Union, List, Dict, Any
 from threading import Event, Thread, Lock
 
 from .base import IOTBaseCommon, IOTDriver
 
 
 if platform_system().lower() == 'windows':
+    import winreg
     import pywintypes
     import win32com.client
 
     from pythoncom import (CoInitialize, CoInitializeEx, CoUninitialize,  COINIT_MULTITHREADED, PumpWaitingMessages, com_error, GetScodeString, Missing)
 
     sys.coinit_flags = 0  # pythoncom.COINIT_MULTITHREADED == 0
     pywintypes.datetime = pywintypes.TimeType
```

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
-from ctypes import create_string_buffer as ctypes_create_string_buffer, c_int32 as ctypes_c_int32, pointer as ctypes_pointer, cast as ctypes_cast, POINTER, c_uint8 as ctypes_c_uint8, string_at as ctypes_string_at
-from snap7.common import error_text, load_library
-from snap7.snap7types import S7DataItem, S7WLByte
-from snap7 import util as snap7_util, client as snap7_client, server as snap7_server, snap7types, types as snap7_types
+from ctypes import create_string_buffer as ctypes_create_string_buffer, c_int32 as ctypes_c_int32, pointer as ctypes_pointer, cast as ctypes_cast, POINTER, c_uint8 as ctypes_c_uint8, c_uint16 as ctypes_c_uint16, string_at as ctypes_string_at
+from enum import Enum
+from snap7.common import error_text, load_library, check_error
+from snap7.types import S7DataItem, S7WLByte, SendTimeout, RecvTimeout, wordlen_to_ctypes
+from snap7 import util as snap7_util, client as snap7_client, server as snap7_server
 
 from typing import List, Dict, Any, Optional
 
 from .base import IOTBaseCommon, IOTDriver, IOTSimulateObject
 
 '''
 pip install python-snap7==0.10
@@ -118,14 +119,23 @@
 '''
     pip install python-snap7==0.10
 '''
 
 
 class IOTPlcS7(IOTDriver):
 
+    # 西门子PLC的类型对象
+    class S7Version(Enum):
+        S7_200 = 1  # 西门子S7-200 需要配置网络模块
+        S7_200Smart = 2
+        S7_300 = 3
+        S7_400 = 4
+        S7_1200 = 5
+        S7_1500 = 6
+
     class S7BlockUnit:
 
         def __init__(self, area, db: int, size: int):
             self.area = area
             self.db = db
             self.size = size
             self.buffers = None
@@ -269,14 +279,15 @@
                 {'required': True, 'name': '倍率' if lan == 'ch' else 'scale'.upper(), 'code': 'point_scale', 'type': 'string', 'default': '1', 'enum': [], 'tip': ''}
             ])
 
         elif type == 'config':
             templates.append({'required': False, 'name': '依赖库路径' if lan == 'ch' else 'Library', 'code': 'library', 'type': 'string', 'default': '', 'enum': [], 'tip': ''})
             if mode == 0:
                 templates.extend([
+                    {'required': False, 'name': '尝试读取次数' if lan == 'ch' else 'Read Retries', 'code': 'read_retries', 'type': 'int', 'default': 2, 'enum': [], 'tip': ''},
                     {'required': True, 'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'code': 'multi_read', 'type': 'int', 'default': 19, 'enum': [], 'tip': ''},
                     {'required': True, 'name': '命令间隔(s)' if lan == 'ch' else 'Cmd Interval(s)', 'code': 'cmd_interval', 'type': 'float', 'default': 0.1, 'enum': [], 'tip': ''},
                     {'required': True, 'name': '发送超时(ms)' if lan == 'ch' else 'Send Timeout(ms)', 'code': 'send_timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''},
                     {'required': True, 'name': '接收超时(ms)' if lan == 'ch' else 'Recv Timeout(ms)', 'code': 'rec_timeout', 'type': 'int', 'default': 3500, 'enum': [], 'tip': ''},
                 ])
         return templates
 
@@ -373,17 +384,17 @@
             area, db, start, length, addr, type = self._get_s7_item(s7_item)
             unit = self.S7ReadUnit(address, area, db, start, length, type)
             if unit.__str__() not in read_units.keys():
                 read_units[unit.__str__()] = unit.get_item()
         return read_units
 
     def _get_address_info(self, device_address: str) -> dict:
-        # ip/port/rack/slot
+        # ip/port/rack/slot/version
         info_list = device_address.split('/')
-        return {'host': info_list[0] if len(info_list) > 0 else '', 'port': int(float(info_list[1])) if len(info_list) > 1 else 102, 'rack': int(float(info_list[2])) if len(info_list) > 2 else 0, 'slot': int(float(info_list[3])) if len(info_list) > 3 else 1, 'type': '' if len(info_list) > 2 else 'plc200'}
+        return {'host': info_list[0] if len(info_list) > 0 else '', 'port': int(float(info_list[1])) if len(info_list) > 1 else 102, 'rack': int(float(info_list[2])) if len(info_list) > 2 else 0, 'slot': int(float(info_list[3])) if len(info_list) > 3 else 1, 'type': IOTPlcS7.S7Version.S7_200Smart if len(info_list) <= 2 else IOTPlcS7.S7Version.S7_1200 if 2 < len(info_list) <= 4 else IOTPlcS7.S7Version(int(info_list[-1]))}
 
     def _release_client(self, address: str):
         client = self.clients.get(address)
         try:
             if client:
                 client.disconnect()
                 client.destroy()
@@ -397,69 +408,86 @@
         if IOTBaseCommon.is_windows():
             library = self.configs.get('library')
             if isinstance(library, str) and len(library) > 0 and IOTBaseCommon.check_file_exist(library):
                 load_library(library)
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
-        if client is not None and (client.get_connected() is False or str(client.get_cpu_state()) == 'S7CpuStatusStop'):
-            self._release_client(address)
-            client = None
+        if client is not None:
+            try:
+                if client.get_connected() is False:  # 连接成功
+                    raise Exception(f"connected is false")
+            except Exception as e:
+                self._release_client(address)
+                client = None
 
         if client is None:
-            info = self._get_address_info(address)
-            if 'type' in info.keys():
-                self._load_library()
-                client = snap7_client.Client()
-                if client:
-                    if self.configs.get('send_timeout', 15) > 0:
-                        client.set_param(snap7types.SendTimeout, self.configs.get('send_timeout'))
-                    if self.configs.get('rec_timeout', 3500) > 0:
-                        client.set_param(snap7types.RecvTimeout, self.configs.get('rec_timeout'))
-
-                if info['type'] == 'plc200':
-                    client.set_connection_type(3)   # 设置连接资源类型，即客户端,连接到PLC
-                client.connect(info['host'], info['rack'], info['slot'], info['port'])
-                if client.get_connected() is True:
-                    self.clients[address] = client
+            try:
+                info = self._get_address_info(address)
+                if 'type' in info.keys():
+                    self._load_library()
+                    client = snap7_client.Client()
+                    if client:
+                        if self.configs.get('send_timeout', 15) > 0:
+                            client.set_param(SendTimeout, self.configs.get('send_timeout'))
+                        if self.configs.get('rec_timeout', 3500) > 0:
+                            client.set_param(RecvTimeout, self.configs.get('rec_timeout'))
+
+                    if info['type'] == IOTPlcS7.S7Version.S7_200:
+                        client._library.Cli_SetConnectionParams(client._pointer, info['host'].encode(), ctypes_c_uint16(info['rack']), ctypes_c_uint16(info['slot']))
+                        result = client._library.Cli_Connect(client._pointer)
+                        check_error(result, context="client")
+                    elif info['type'] == IOTPlcS7.S7Version.S7_200Smart:
+                        client.set_connection_type(3)   # 设置连接资源类型，即客户端,连接到PLC   默认情况下，客户端连接为PG（编程控制台），使用此功能可以将连接资源类型更改为OP（西门子HMI面板）或S7 Basic（通用数据传输连接）
+                        client.connect(info['host'], info['rack'], info['slot'], info['port'])
+                    else:
+                        client.connect(info['host'], info['rack'], info['slot'], info['port'])
+                    if client.get_connected() is True:
+                        self.clients[address] = client
+            except Exception as e:
+                raise IOTBaseCommon.IOTConnectException(e.__str__())
         return self.clients.get(address)
 
     def _parse_result(self, address: str, s7_key: str, s7_item):
         self.update_device(address, s7_key, **self.gen_read_write_result(True, ctypes_string_at(s7_item.pData, s7_item.Amount)))
 
-    def _send_read_cmd(self, address: str, s7_item_list: list, process: Optional[str] = None):
-        try:
-            if self._get_client(address) is not None and len(s7_item_list) > 0:
-                s7_item_byref = (S7DataItem * len(s7_item_list))()
-                for index in range(0, len(s7_item_list)):
-                    s7_item_byref[index] = s7_item_list[index]
-
-                self.logging(content=f"plc({address}) read{'' if process is None else f'({process})'} {len(s7_item_list)}", pos=self.stack_pos)
-                result, s7_data_items = self._get_client(address).read_multi_vars(s7_item_byref)
-                for s7_item in s7_data_items:
-                    s7_key = self._gen_key(s7_item.Area, s7_item.DBNumber, s7_item.Start, s7_item.Amount)
-                    try:
-                        if s7_item.Result:
-                            raise Exception(error_text(s7_item.Result))
-                        else:
-                            self._parse_result(address, s7_key, s7_item)
-                    except Exception as e:
-                        self.update_device(address, s7_key, **self.gen_read_write_result(False, e.__str__()))
-        except Exception as e:
-            for s7_item in s7_item_list:
-                self.update_device(address, self._gen_key(s7_item.Area, s7_item.DBNumber, s7_item.Start, s7_item.Amount), **self.gen_read_write_result(False, e.__str__()))
+    def _send_read_cmd(self, address: str, s7_item_list: list, process: Optional[str] = None, read_retries: int = 2):
+        for i in range(read_retries):
+            try:
+                if self._get_client(address) is not None and len(s7_item_list) > 0:
+                    s7_item_byref = (S7DataItem * len(s7_item_list))()
+                    for index in range(0, len(s7_item_list)):
+                        s7_item_byref[index] = s7_item_list[index]
+
+                    self.logging(content=f"plc({address}) read{'' if process is None else f'({process})'} {len(s7_item_list)} {i + 1}/{read_retries}", pos=self.stack_pos)
+                    result, s7_data_items = self._get_client(address).read_multi_vars(s7_item_byref)
+                    for s7_item in s7_data_items:
+                        s7_key = self._gen_key(s7_item.Area, s7_item.DBNumber, s7_item.Start, s7_item.Amount)
+                        try:
+                            if s7_item.Result:
+                                raise Exception(error_text(s7_item.Result))
+                            else:
+                                self._parse_result(address, s7_key, s7_item)
+                        except Exception as e:
+                            self.update_device(address, s7_key, **self.gen_read_write_result(False, f"read error: {e.__str__()}"))
+                break
+            except (Exception, IOTBaseCommon.IOTConnectException) as e:
+                self._release_client(address)
+                if i == read_retries - 1:
+                    for s7_item in s7_item_list:
+                        self.update_device(address, self._gen_key(s7_item.Area, s7_item.DBNumber, s7_item.Start, s7_item.Amount), **self.gen_read_write_result(False, f"connect error: {e.__str__()}" if isinstance(e, IOTBaseCommon.IOTConnectException) else f"read error: {e.__str__()}"))
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, s7_items) = args
         results = {}
         read_units = self._cread_read_units(address, sorted(s7_items))
 
-        units = list(IOTBaseCommon.chunk_list(list(read_units.values()), self.configs.get('multi_read')))
+        units = list(IOTBaseCommon.chunk_list(list(read_units.values()), self.configs.get('multi_read', 19)))
         for i, unit in enumerate(units):
-            self._send_read_cmd(address, unit, f"{i}/{len(units)}")
+            self._send_read_cmd(address, unit, f"{i}/{len(units)}", self.configs.get('read_retries', 2))
             self.delay(self.configs.get('cmd_interval', 0.3))
         return results
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
             jobs = IOTBaseCommon.SimpleThreadPool(len(read_items), f"{self}")
             for address, s7_items in read_items.items():
@@ -535,19 +563,22 @@
                 length = 1
             elif address[1] == 'W':
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT16
                 length = 2
             elif address[1] == 'D':
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT32
                 length = 4
+            elif address[1] == 'R':     # 额外新增
+                type = IOTBaseCommon.DataTransform.TypeFormat.FLOAT
+                length = 4
             else:
                 type = IOTBaseCommon.DataTransform.TypeFormat.BOOL
                 length = 1
 
-            info = address[2:] if address[1] in ['D', 'B', 'W'] else address[1:]
+            info = address[2:] if address[1] in ['D', 'B', 'W', 'R'] else address[1:]
             pos = info.find('.')
             if pos > 0:
                 start = int(float(info[:pos]))
                 addr = int(float(info[pos+1:]))
             else:
                 start = int(float(info))
 
@@ -657,15 +688,15 @@
                             server.unregister_area(areas.get(block.get('area')), block.get('db'))
                             register = True
                     else:
                         register = True
 
                     if register:
                         self.logging(content=f"register {block.get('area')} {block.get('db')} {block.get('size')}", pos=self.stack_pos)
-                        buffer = (snap7_types.wordlen_to_ctypes[snap7_types.S7WLByte] * block.get('size'))()
+                        buffer = (wordlen_to_ctypes[S7WLByte] * block.get('size'))()
                         server.register_area(areas.get(block.get('area')), block.get('db'), buffer)
                         block['buffer'] = buffer
                         blocks[key] = block
             except Exception as e:
                 self.logging(content=f"create object({port}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _update_value(self, server, block, area, db, start: int, addr: int, type, value):
```

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,16 +301,16 @@
                 command[5 + index: 5 + index + len(data.contents[8])] = data.contents[8]
                 index = index + 4 + len(data.contents[8])
         return IOTBaseCommon.IOTNetResult.create_success([command])
 
 
 class SiemensS7Client(IOTBaseCommon.IOTNetworkDeviceClient):
  
-    def __init__(self, version: SiemensS7Version, host: str, port: int, slot: int = 0, rack: int = 0, timeout: int = 10):
-        super().__init__(host, port, timeout)
+    def __init__(self, version: SiemensS7Version, host: str, port: int, slot: int = 0, rack: int = 0, timeout: int = 10, conn_retries: int = 1):
+        super().__init__(host, port, timeout, conn_retries)
         self.version = version
         self.word_length = 2
         self.slot = slot
         self.rack = rack
 
     def get_net_msg(self):
         return SiemensS7Message()
@@ -334,28 +334,28 @@
 
     def extra_on_disconnect(self, socket):
         return IOTBaseCommon.IOTNetResult.create_success()
 
     def init_head(self):
         head1 = SiemensS7Constant.Head1
         head2 = SiemensS7Constant.Head2
-        if self.version == SiemensS7Version.S7_200.value:  # 0, 1
+        if self.version == SiemensS7Version.S7_200:  # 0, 1
             head1 = SiemensS7Constant.Head1_200
             head2 = SiemensS7Constant.Head2_200
-        elif self.version == SiemensS7Version.S7_200Smart.value:  #
+        elif self.version == SiemensS7Version.S7_200Smart:  #
             head1 = SiemensS7Constant.Head1_200Smart
             head2 = SiemensS7Constant.Head2_200Smart
-        elif self.version == SiemensS7Version.S7_300.value:   # 0, 2
+        elif self.version == SiemensS7Version.S7_300:   # 0, 2
             head1[21] = self.rack * 0x20 + self.slot
-        elif self.version == SiemensS7Version.S7_400.value:  # 具体看硬件组态
+        elif self.version == SiemensS7Version.S7_400:  # 具体看硬件组态
             head1[21] = self.rack * 0x20 + self.slot
             head1[17] = 0
-        elif self.version == SiemensS7Version.S7_1200.value:   # 0, 0/1
+        elif self.version == SiemensS7Version.S7_1200:   # 0, 0/1
             head1[21] = self.rack * 0x20 + self.slot
-        elif self.version == SiemensS7Version.S7_1500.value:   # 0, 0/1
+        elif self.version == SiemensS7Version.S7_1500:   # 0, 0/1
             head1[21] = self.rack * 0x20 + self.slot
         else:
             head1[18] = 0
 
         return head1, head2
 
     def read(self, address: Union[tuple, list]):
@@ -637,14 +637,15 @@
                 {'required': True, 'name': '是否启用' if lan == 'ch' else 'enable'.upper(), 'code': 'point_enabled', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''},
                 {'required': True, 'name': '倍率' if lan == 'ch' else 'scale'.upper(), 'code': 'point_scale', 'type': 'string', 'default': '1', 'enum': [], 'tip': ''}
             ])
 
         elif type == 'config':
             if mode == 0:
                 templates.extend([
+                    {'required': False, 'name': '连接重试' if lan == 'ch' else 'Conn Retries', 'code': 'conn_retries', 'type': 'int', 'default': 1, 'enum': [], 'tip': ''},
                     {'required': True, 'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'code': 'multi_read', 'type': 'int', 'default': 19, 'enum': [], 'tip': ''},
                     {'required': True, 'name': '命令间隔(s)' if lan == 'ch' else 'Cmd Interval(s)', 'code': 'cmd_interval', 'type': 'float', 'default': 0.1, 'enum': [], 'tip': ''},
                 ])
             templates.append({'required': True, 'name': '超时(s)' if lan == 'ch' else 'Timeout(s)', 'code': 'timeout', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
         return templates
 
     def read(self, **kwargs):
@@ -776,15 +777,15 @@
         if client is not None and client.get_connected() is False:
             self._release_client(address)
             client = None
 
         if client is None:
             info = self._get_address_info(address)
             if 'type' in info.keys():
-                client = SiemensS7Client(SiemensS7Version(info['type']), info['host'], info['port'], info['rack'], info['slot'], self.configs.get('timeout'))
+                client = SiemensS7Client(SiemensS7Version(info['type']), info['host'], info['port'], info['rack'], info['slot'], self.configs.get('timeout'), self.configs.get('conn_retries', 1))
                 client.logging(call_logging=self.logging)
                 result = client.connect()
                 if result.is_success is True and client.get_connected() is True:
                     self.clients[address] = client
                 else:
                     raise Exception(f"{result.msg}")
         return self.clients.get(address)
```

### Comparing `RobertCommonDriver-0.1.46/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.47/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/setup.py` & `RobertCommonDriver-0.1.47/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.46'
-DATE = '2023-07-24'
+VERSION = '0.1.47'
+DATE = '2023-07-31'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,61 @@
+import random
 import time
-from robertcommondriver.system.iot.iot_iec104 import IOTIEC104, unpack
+from robertcommondriver.system.iot.iot_plc_omron import OmronFinsClient, IOTPlcOmronFins
 
 
 def logging_print(**kwargs):
     print(kwargs)
 
 
-def test_read():
-    dict_config = {'host': '192.168.1.184', 'port': 2404, 'timeout': 4}
-    dict_point = {}
-    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 1, 'point_scale': '1'}
-    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 16386, 'point_scale': '1'}
+def test_read_write():
+    omron = OmronFinsClient('192.168.1.12', 9600, 0x0B)
+    omron.logging(call_logging=logging_print)
+    while True:
+        aa = omron.write(('D263', 18, 2.234))
+        print(aa.contents[0].contents[8])
+        time.sleep(4)
+
 
-    client = IOTIEC104(configs = dict_config, points= dict_point)
+def test_iot_omron_read():
+    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
+    dict_point = {}
+    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '192.168.1.12/9600/11', 'point_address': 'D263', 'point_type': 18, 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '192.168.1.12/9600/11', 'point_address': 'W320', 'point_type': 6, 'point_scale': '1'}
+    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '192.168.1.12/9600/11', 'point_address': 'W330.2', 'point_type': 0, 'point_scale': '1'}
+    client = IOTPlcOmronFins(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
-            result = client.read(names=list(dict_point.keys()))
-            print(result)
+            aa = client.write(values={'plc10': random.randint(1, 100)})
+            print(aa)
+
+            re = client.read()
+            print(re)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(1)
+        time.sleep(4)
 
 
-def test_parse():
-    #r = IOTIEC104.APDU(bytes.fromhex('68 0E 06 00 08 00 64 01 06 00 01 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00'))
-    r = IOTIEC104.APDU(bytes.fromhex('68 0E 02 00 02 00 01 82 14 00 01 00 01 00 00 01 68 0E 04 00 02 00 64 01 0A 00 01 00 00 00 00 14'))
-    #r = IOTIEC104.APDU(bytes.fromhex('68 0E 02 00 02 00 01 82 14 00 01 00 01 00 00 01'))
-    print(r.info())
-
-
-def test_read1():
-    dict_config = {'host': '192.168.1.184', 'port': 2404, 'timeout': 5, 'zongzhao_interval': 0, 'zongzhao_timeout': 30, 'u_test_timeout': 10,  's_interval': 1}
+def test_iot_omron_simulate():
+    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
     dict_point = {}
-    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 100, 'point_scale': '1'}
-    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 600, 'point_scale': '1'}
-
-    client = IOTIEC104(configs = dict_config, points= dict_point)
+    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '0.0.0.0/9600/11', 'point_address': 'D263', 'point_type': 18, 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '0.0.0.0/9600/11', 'point_address': 'W320', 'point_type': 6, 'point_scale': '1'}
+    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '0.0.0.0/9600/11', 'point_address': 'W330.2', 'point_type': 0, 'point_scale': '1'}
+    client = IOTPlcOmronFins(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
-            result = client.read(names=list(dict_point.keys()))
-            print(result)
+            for name, point in dict_point.items():
+                if name in ['plc12']:
+                    point['point_value'] = random.randint(0, 1)
+                else:
+                    point['point_value'] = random.randint(0, 100)
+                print(f"{point['point_address']}: {point['point_value']}")
+            client.simulate(points=dict_point)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(5)
-
-
-def test_frame():
-    info = IOTIEC104.APDU(bytes.fromhex('68 0f 08 00 02 00 05 01 14 00 01 00 2c 01 00 00 00 ')).info()
-    print(info)
+        time.sleep(400)
 
 
-test_frame()
+test_iot_omron_read()
```

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,83 @@
 import random
 import time
-from robertcommondriver.system.iot.iot_plc_omron import OmronFinsClient, IOTPlcOmronFins
+from robertcommondriver.system.iot.iot_plc_siemens import SiemensS7Client, SiemensS7Version, SiemensS7Server, IOTPlcSiemensS7
 
 
 def logging_print(**kwargs):
     print(kwargs)
 
 
-def test_read_write():
-    omron = OmronFinsClient('192.168.1.12', 9600, 0x0B)
-    omron.logging(call_logging=logging_print)
+def test_siemens():
+    s7 = SiemensS7Client(SiemensS7Version.S7_200, '192.168.1.184', 102, 0, 1)
+    aa = s7.read(('V2634', 8))
+    print(aa)
+
+
+def test_siemens_server():
+    s7 = SiemensS7Server(SiemensS7Version.S7_1500, '0.0.0.0', 102, 0, 1)
+    s7.start_server()
     while True:
-        aa = omron.write(('D263', 18, 2.234))
-        print(aa.contents[0].contents[8])
-        time.sleep(4)
+        time.sleep(1)
 
 
-def test_iot_omron_read():
+def test_iot_siemens_read():
     dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
     dict_point = {}
-    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '192.168.1.12/9600/11', 'point_address': 'D263', 'point_type': 18, 'point_scale': '1'}
-    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '192.168.1.12/9600/11', 'point_address': 'W320', 'point_type': 6, 'point_scale': '1'}
-    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '192.168.1.12/9600/11', 'point_address': 'W330.2', 'point_type': 0, 'point_scale': '1'}
-    client = IOTPlcOmronFins(configs=dict_config, points=dict_point)
+    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'I0.0', 'point_type': 0, 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '6/192.168.1.11/102/0/1', 'point_address': 'DB1,0.3', 'point_type': 0, 'point_scale': '1'}
+    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'MW300', 'point_type': 10, 'point_scale': '1'}
+    client = IOTPlcSiemensS7(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
-            aa = client.write(values={'plc10': random.randint(1, 100)})
-            print(aa)
+            re = client.read()
+            print(re)
+        except Exception as e:
+            print(f"error: {e.__str__()}")
+        time.sleep(4)
 
+
+def test_iot_siemens_write():
+    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
+    dict_point = {}
+    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'I0.0', 'point_type': 0, 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'DB1,0.3', 'point_type': 0, 'point_scale': '1'}
+    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'MW300', 'point_type': 10, 'point_scale': '1'}
+    client = IOTPlcSiemensS7(configs=dict_config, points=dict_point)
+    client.logging(call_logging=logging_print)
+    while True:
+        try:
+            #print(client.write(values={'plc10': 1, 'plc11': 0, 'plc12': 22}))
+            print(client.write(values={'plc10': random.randint(0,1), 'plc11': random.randint(0,1), 'plc12': random.randint(0,100)}))
             re = client.read()
             print(re)
         except Exception as e:
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
-def test_iot_omron_simulate():
+def test_iot_siemens_server():
+
     dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
     dict_point = {}
-    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '0.0.0.0/9600/11', 'point_address': 'D263', 'point_type': 18, 'point_scale': '1'}
-    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '0.0.0.0/9600/11', 'point_address': 'W320', 'point_type': 6, 'point_scale': '1'}
-    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '0.0.0.0/9600/11', 'point_address': 'W330.2', 'point_type': 0, 'point_scale': '1'}
-    client = IOTPlcOmronFins(configs=dict_config, points=dict_point)
+    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '6/0.0.0.0/102/0/1', 'point_address': 'I0.3', 'point_type': 0, 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '6/0.0.0.0/102/0/1', 'point_address': 'DB1,0.3', 'point_type': 0, 'point_scale': '1'}
+    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '6/0.0.0.0/102/0/1', 'point_address': 'MW300', 'point_type': 10, 'point_scale': '1'}
+    client = IOTPlcSiemensS7(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
+            #print(client.write(values={'plc10': 1, 'plc11': 0, 'plc12': 22}))
             for name, point in dict_point.items():
-                if name in ['plc12']:
+                if name in ['plc10', 'plc11']:
                     point['point_value'] = random.randint(0, 1)
                 else:
                     point['point_value'] = random.randint(0, 100)
                 print(f"{point['point_address']}: {point['point_value']}")
             client.simulate(points=dict_point)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(400)
+        time.sleep(4)
 
 
-test_iot_omron_read()
+test_siemens()
```

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
 def test_read_200():
     dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'send_timeout': 15, 'rec_timeout': 3500}
     dict_point = {}
-    dict_point['plc1'] = {'point_writable': True, 'point_name': 'plc1', 'point_device_address': '192.168.100.107/102', 'point_address': 'I1.1', 'point_scale': '1'}
+    dict_point['PMPower_DHU_B1_4F_13'] = {'point_writable': True, 'point_name': 'PMPower_DHU_B1_4F_13', 'point_device_address': '192.168.1.184/102/0/1/2', 'point_address': 'DB1,REAL3000', 'point_scale': '1'}
     client = IOTPlcS7(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
             re = client.read()
             print(re)
         except Exception as e:
```

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,79 @@
-import random
 import time
-from robertcommondriver.system.iot.iot_plc_siemens import SiemensS7Client, SiemensS7Version, SiemensS7Server, IOTPlcSiemensS7
+from robertcommondriver.system.iot.iot_iec104 import IOTIEC104, unpack, IECData, IECPacket
 
 
 def logging_print(**kwargs):
     print(kwargs)
 
 
-def test_siemens():
-    s7 = SiemensS7Client(SiemensS7Version.S7_1500, '192.168.1.12', 102, 0, 1)
-    aa = s7.read(('V2634', 8))
-    print(aa)
-
-
-def test_siemens_server():
-    s7 = SiemensS7Server(SiemensS7Version.S7_1500, '0.0.0.0', 102, 0, 1)
-    s7.start_server()
-    while True:
-        time.sleep(1)
-
-
-def test_iot_siemens_read():
-    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
+def test_read():
+    dict_config = {'host': '192.168.1.184', 'port': 2404, 'timeout': 4}
     dict_point = {}
-    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'I0.0', 'point_type': 0, 'point_scale': '1'}
-    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '6/192.168.1.11/102/0/1', 'point_address': 'DB1,0.3', 'point_type': 0, 'point_scale': '1'}
-    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'MW300', 'point_type': 10, 'point_scale': '1'}
-    client = IOTPlcSiemensS7(configs=dict_config, points=dict_point)
+    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 1, 'point_scale': '1'}
+    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 16386, 'point_scale': '1'}
+
+    client = IOTIEC104(configs = dict_config, points= dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
-            re = client.read()
-            print(re)
+            result = client.read(names=list(dict_point.keys()))
+            print(result)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(4)
+        time.sleep(1)
+
 
+def test_parse():
+    #r = IOTIEC104.APDU(bytes.fromhex('68 0E 06 00 08 00 64 01 06 00 01 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00'))
+    r = IOTIEC104.APDU(bytes.fromhex('68 0E 02 00 02 00 01 82 14 00 01 00 01 00 00 01 68 0E 04 00 02 00 64 01 0A 00 01 00 00 00 00 14'))
+    #r = IOTIEC104.APDU(bytes.fromhex('68 0E 02 00 02 00 01 82 14 00 01 00 01 00 00 01'))
+    print(r.info())
 
-def test_iot_siemens_write():
-    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
+
+def test_read1():
+    dict_config = {'host': '192.168.1.184', 'port': 2404, 'timeout': 5, 'zongzhao_interval': 0, 'zongzhao_timeout': 30, 'u_test_timeout': 10,  's_interval': 1}
     dict_point = {}
-    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'I0.0', 'point_type': 0, 'point_scale': '1'}
-    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'DB1,0.3', 'point_type': 0, 'point_scale': '1'}
-    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '6/192.168.1.12/102/0/1', 'point_address': 'MW300', 'point_type': 10, 'point_scale': '1'}
-    client = IOTPlcSiemensS7(configs=dict_config, points=dict_point)
+    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 100, 'point_scale': '1'}
+    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 600, 'point_scale': '1'}
+
+    client = IOTIEC104(configs = dict_config, points= dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
-            #print(client.write(values={'plc10': 1, 'plc11': 0, 'plc12': 22}))
-            print(client.write(values={'plc10': random.randint(0,1), 'plc11': random.randint(0,1), 'plc12': random.randint(0,100)}))
-            re = client.read()
-            print(re)
+            result = client.read(names=list(dict_point.keys()))
+            print(result)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(4)
+        time.sleep(5)
 
 
-def test_iot_siemens_server():
+def test_frame():
+    pkt = IOTIEC104.APDU()
+    pkt /= IOTIEC104.APCI(ApduLen=14, Type=0x00, Tx=1, Rx=4)
+    pkt /= IOTIEC104.ASDU(Type=101, SQ=0, Cause=6, Num=1, Test=0, OA=0, Addr=1, IOA=[IECData.IOAS[101](IOA=0, QCC=IECPacket.QCC(RQT=0, FRZ=0))])
+    print(IOTIEC104().format_bytes(pkt.build()))
 
-    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'timeout': 5}
+    info = IOTIEC104.APDU(bytes.fromhex('68 a3 26 00 04 00 0f 9e 14 00 01 00 a5 65 00 02 00 00 00 00 00 00 00 00 00 13 51 00 00 00 f5 18 00 00 00 00 27 00 00 00 7a 3f 00 00 00 ed 73 00 00 00 9d 27 c7 00 00 00 00 00 00 00 65 12 00 00 00 b3 5d 01 00 00 08 40 f4 01 00 26 41 0b 00 00 5c 00 00 00 00 00 00 00 00 00 18 0a 00 00 00 5f 00 00 00 00 7a b9 7f 00 00 02 db 00 00 00 00 00 00 00 00 4a 9c 9d 00 00 36 01 00 00 00 32 40 89 00 00 01 00 00 00 00 05 00 00 00 00 1d 00 00 00 00 cf 1c 00 00 00 13 29 15 00 00 00 00 00 00 00 8e 00 00 00 00')).info()
+    print(info)
+
+
+def test_dianneng():
+    dict_config = {'host': '127.0.0.1', 'port': 2404, 'timeout': 5, 'zongzhao_interval': 0, 'zongzhao_timeout': 30, 'dianneng_interval': 20, 'dianneng_timeout': 10, 'u_test_timeout': 10,  's_interval': 1}
     dict_point = {}
-    dict_point['plc10'] = {'point_writable': True, 'point_name': 'plc10', 'point_device_address': '6/0.0.0.0/102/0/1', 'point_address': 'I0.3', 'point_type': 0, 'point_scale': '1'}
-    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '6/0.0.0.0/102/0/1', 'point_address': 'DB1,0.3', 'point_type': 0, 'point_scale': '1'}
-    dict_point['plc12'] = {'point_writable': True, 'point_name': 'plc12', 'point_device_address': '6/0.0.0.0/102/0/1', 'point_address': 'MW300', 'point_type': 10, 'point_scale': '1'}
-    client = IOTPlcSiemensS7(configs=dict_config, points=dict_point)
+    dict_point['iec1'] = {'point_writable': True, 'point_name': 'iec1', 'point_type': 1, 'point_address': 100, 'point_scale': '1'}
+    dict_point['iec2'] = {'point_writable': True, 'point_name': 'iec2', 'point_type': 13, 'point_address': 600, 'point_scale': '1'}
+    dict_point['iec3'] = {'point_writable': True, 'point_name': 'iec3', 'point_type': 15, 'point_address': 25633, 'point_scale': '1'}   # 37515
+    dict_point['iec4'] = {'point_writable': True, 'point_name': 'iec4', 'point_type': 15, 'point_address': 25697, 'point_scale': '1'}   # 500315
+
+    client = IOTIEC104(configs = dict_config, points= dict_point)
     client.logging(call_logging=logging_print)
     while True:
         try:
-            #print(client.write(values={'plc10': 1, 'plc11': 0, 'plc12': 22}))
-            for name, point in dict_point.items():
-                if name in ['plc10', 'plc11']:
-                    point['point_value'] = random.randint(0, 1)
-                else:
-                    point['point_value'] = random.randint(0, 100)
-                print(f"{point['point_address']}: {point['point_value']}")
-            client.simulate(points=dict_point)
+            result = client.read(names=list(dict_point.keys()))
+            print(result)
         except Exception as e:
             print(f"error: {e.__str__()}")
-        time.sleep(4)
+        time.sleep(5)
 
 
-test_iot_siemens_read()
+test_dianneng()
```

### Comparing `RobertCommonDriver-0.1.46/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.47/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

