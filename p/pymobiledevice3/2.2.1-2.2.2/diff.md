# Comparing `tmp/pymobiledevice3-2.2.1.tar.gz` & `tmp/pymobiledevice3-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymobiledevice3-2.2.1.tar", last modified: Wed Aug  2 05:05:58 2023, max compression
+gzip compressed data, was "pymobiledevice3-2.2.2.tar", last modified: Wed Aug  2 08:20:38 2023, max compression
```

## Comparing `pymobiledevice3-2.2.1.tar` & `pymobiledevice3-2.2.2.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.907809 pymobiledevice3-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    57849 2023-08-02 05:05:58.907809 pymobiledevice3-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.879808 pymobiledevice3-2.2.1/misc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/misc/extract_plist_from_pcaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/misc/remotexpc_sniffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.879808 pymobiledevice3-2.2.1/pymobiledevice3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/bonjour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/ca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.883808 pymobiledevice3-2.2.1/pymobiledevice3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/bonjour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/companion_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    39122 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/developer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/mounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/cli/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/irecv.py
--rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/irecv_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28953 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/lockdown_service_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/pair_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.883808 pymobiledevice3-2.2.1/pymobiledevice3/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/bonjour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.887809 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/core_device_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/diagnostics_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device_tunnel_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/remote_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/remote_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/remotexpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/remote/xpc_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.887809 pymobiledevice3-2.2.1/pymobiledevice3/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/dsc_uuid_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/dsc_uuid_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/firmware_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/notifications.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.887809 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/element_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/element_clear.js
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/enter_fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/find_nodes.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/focus.js
--rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/get_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/is_displayed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/is_editable.js
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/is_enabled.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.895809 pymobiledevice3-2.2.1/pymobiledevice3/restore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/base_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/ftab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    49852 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/restore_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/restored_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/restore/tss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6957 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/service_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.899809 pymobiledevice3-2.2.1/pymobiledevice3/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/accessibilityaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31443 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/crash_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/debugserver_applist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/device_arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/device_link.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6494 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/diagnostics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dtfetchsymbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.899809 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.903809 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/application_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/condition_inducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28098 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/location_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/network_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/process_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/sysmontap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/file_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/heartbeat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/house_arrest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/installation_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/lockdown_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2127 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/misagent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3428 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/mobile_activation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4722 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/mobile_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13817 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/mobile_image_mounter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16764 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/mobilebackup2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2094 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/notification_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/os_trace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9504 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/pcapd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/preboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/restore_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1820 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/simulate_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/syslog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.903809 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/automation_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/cdp_screencast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/cdp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/cdp_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/inspector_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/selenium_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/session_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/switch_to.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/services/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/tcp_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pymobiledevice3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.879808 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57849 2023-08-02 05:05:58.000000 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-08-02 05:05:58.000000 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:05:58.000000 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 05:05:58.000000 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 05:05:58.000000 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:05:58.000000 pymobiledevice3-2.2.1/pymobiledevice3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 05:05:58.907809 pymobiledevice3-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:05:58.907809 pymobiledevice3-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 05:05:37.000000 pymobiledevice3-2.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.885480 pymobiledevice3-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57849 2023-08-02 08:20:38.885480 pymobiledevice3-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.865480 pymobiledevice3-2.2.2/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/misc/extract_plist_from_pcaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/misc/remotexpc_sniffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.865480 pymobiledevice3-2.2.2/pymobiledevice3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/bonjour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/ca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.869480 pymobiledevice3-2.2.2/pymobiledevice3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/bonjour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/companion_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39122 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/mounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/cli/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/irecv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/irecv_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28953 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/lockdown_service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/pair_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.873480 pymobiledevice3-2.2.2/pymobiledevice3/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/bonjour.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.873480 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/core_device_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/diagnostics_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device_tunnel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/remote_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/remote_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/remotexpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/remote/xpc_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.873480 pymobiledevice3-2.2.2/pymobiledevice3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/dsc_uuid_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/dsc_uuid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/firmware_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/notifications.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.877480 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/element_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/element_clear.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/enter_fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/find_nodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/focus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/get_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/is_displayed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/is_editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/is_enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.877480 pymobiledevice3-2.2.2/pymobiledevice3/restore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/base_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/ftab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49852 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/restored_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/restore/tss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6957 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/service_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.881480 pymobiledevice3-2.2.2/pymobiledevice3/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/accessibilityaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31443 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/crash_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/debugserver_applist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/device_arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/device_link.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6494 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/diagnostics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dtfetchsymbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.881480 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.885480 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/application_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/condition_inducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28098 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/location_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/network_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/process_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/sysmontap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/file_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/house_arrest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/installation_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/lockdown_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2127 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/misagent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3428 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/mobile_activation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4722 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/mobile_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13817 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/mobile_image_mounter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16764 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/mobilebackup2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2094 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/notification_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/os_trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9504 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/pcapd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/preboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/restore_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1820 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/simulate_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.885480 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/automation_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/cdp_screencast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/cdp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/cdp_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/inspector_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/selenium_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/session_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/services/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/tcp_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pymobiledevice3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.869480 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57849 2023-08-02 08:20:38.000000 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-08-02 08:20:38.000000 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:20:38.000000 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 08:20:38.000000 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 08:20:38.000000 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 08:20:38.000000 pymobiledevice3-2.2.2/pymobiledevice3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:20:38.885480 pymobiledevice3-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:20:38.885480 pymobiledevice3-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 08:20:23.000000 pymobiledevice3-2.2.2/tests/test_utils.py
```

### Comparing `pymobiledevice3-2.2.1/LICENSE` & `pymobiledevice3-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/PKG-INFO` & `pymobiledevice3-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.2.1
+Version: 2.2.2
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pymobiledevice3-2.2.1/README.md` & `pymobiledevice3-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/misc/extract_plist_from_pcaps.py` & `pymobiledevice3-2.2.2/misc/extract_plist_from_pcaps.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/misc/remotexpc_sniffer.py` & `pymobiledevice3-2.2.2/misc/remotexpc_sniffer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/__main__.py` & `pymobiledevice3-2.2.2/pymobiledevice3/__main__.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/bonjour.py` & `pymobiledevice3-2.2.2/pymobiledevice3/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/ca.py` & `pymobiledevice3-2.2.2/pymobiledevice3/ca.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/activation.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/activation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/afc.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/amfi.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/amfi.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/apps.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/apps.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/backup.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/bonjour.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/cli_common.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/companion_proxy.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/companion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/crash.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/crash.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/developer.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/developer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/diagnostics.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/lockdown.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/lockdown.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/mounter.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/mounter.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/notification.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/notification.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/pcap.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/pcap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/power_assertion.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/processes.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/processes.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/profile.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/provision.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/provision.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/remote.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/remote.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/restore.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/springboard.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/syslog.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/usbmux.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/cli/webinspector.py` & `pymobiledevice3-2.2.2/pymobiledevice3/cli/webinspector.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/exceptions.py` & `pymobiledevice3-2.2.2/pymobiledevice3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/irecv.py` & `pymobiledevice3-2.2.2/pymobiledevice3/irecv.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/irecv_devices.py` & `pymobiledevice3-2.2.2/pymobiledevice3/irecv_devices.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/lockdown.py` & `pymobiledevice3-2.2.2/pymobiledevice3/lockdown.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/lockdown_service_provider.py` & `pymobiledevice3-2.2.2/pymobiledevice3/lockdown_service_provider.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/pair_records.py` & `pymobiledevice3-2.2.2/pymobiledevice3/pair_records.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/bonjour.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/app_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/app_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/core_device_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/core_device_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/device_info.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/device_info.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device/diagnostics_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device/diagnostics_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/core_device_tunnel_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/core_device_tunnel_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/remote_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/remote_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/remote_service_discovery.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/remote_service_discovery.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/remotexpc.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/remotexpc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/remote/xpc_message.py` & `pymobiledevice3-2.2.2/pymobiledevice3/remote/xpc_message.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/dsc_uuid_map.json` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/dsc_uuid_map.json`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/dsc_uuid_map.py` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/dsc_uuid_map.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/firmware_notifications.py` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/firmware_notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/notifications.txt` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/notifications.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/element_clear.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/element_clear.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/enter_fullscreen.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/enter_fullscreen.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/find_nodes.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/find_nodes.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/get_attribute.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/get_attribute.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/is_displayed.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/is_displayed.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/is_editable.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/is_editable.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/resources/webinspector/is_enabled.js` & `pymobiledevice3-2.2.2/pymobiledevice3/resources/webinspector/is_enabled.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/asr.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/asr.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/base_restore.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/base_restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/consts.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/consts.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/device.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/device.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/fdr.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/fdr.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/ftab.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/ftab.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/recovery.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/recovery.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/restore.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/restore_options.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/restore_options.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/restored_client.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/restored_client.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/restore/tss.py` & `pymobiledevice3-2.2.2/pymobiledevice3/restore/tss.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/service_connection.py` & `pymobiledevice3-2.2.2/pymobiledevice3/service_connection.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/accessibilityaudit.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/accessibilityaudit.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/afc.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/amfi.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/amfi.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/companion.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/companion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/crash_reports.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/crash_reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import logging
 import posixpath
+import time
 from typing import Generator, List
 
 from cmd2 import Cmd2ArgumentParser, with_argparser
 from pycrashreport.crash_report import get_crash_report_from_buf
 
 from pymobiledevice3.exceptions import AfcException
 from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
 from pymobiledevice3.services.afc import AfcService, AfcShell
 from pymobiledevice3.services.os_trace import OsTraceService
 
 SYSDIAGNOSE_PROCESS_NAMES = ('sysdiagnose', 'sysdiagnosed')
 
+# on iOS17, we need to wait for a moment before tryint to fetch the sysdiagnose archive
+IOS17_SYSDIAGNOSE_DELAY = 1
+
 
 class CrashReportsManager:
     COPY_MOBILE_NAME = 'com.apple.crashreportcopymobile'
     RSD_COPY_MOBILE_NAME = 'com.apple.crashreportcopymobile.shim.remote'
 
     CRASH_MOVER_NAME = 'com.apple.crashreportmover'
     RSD_CRASH_MOVER_NAME = 'com.apple.crashreportmover.shim.remote'
@@ -148,14 +152,15 @@
                                 sysdiagnose_filename = filename.rsplit(ext)[0]
                                 sysdiagnose_filename = sysdiagnose_filename.replace('IN_PROGRESS_', '')
                                 sysdiagnose_filename = f'{sysdiagnose_filename}.tar.gz'
                                 break
                 break
 
         self.afc.wait_exists(sysdiagnose_filename)
+        time.sleep(IOS17_SYSDIAGNOSE_DELAY)
         self.pull(out, entry=sysdiagnose_filename, erase=erase)
 
 
 parse_parser = Cmd2ArgumentParser(description='parse given crash report file')
 parse_parser.add_argument('filename')
 
 clear_parser = Cmd2ArgumentParser(description='remove all crash reports')
```

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/debugserver_applist.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/debugserver_applist.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/device_arbitration.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/device_arbitration.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/device_link.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/device_link.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import ctypes
 import datetime
 import shutil
 import struct
+import warnings
 from pathlib import Path
 
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 
 SIZE_FORMAT = '>I'
 CODE_FORMAT = '>B'
 CODE_FILE_DATA = 0xc
+CODE_ERROR_REMOTE = 0xb
 CODE_ERROR_LOCAL = 0x6
 CODE_SUCCESS = 0
 FILE_TRANSFER_TERMINATOR = b'\x00\x00\x00\x00'
 BULK_OPERATION_ERROR = -13
 APPLE_EPOCH = 978307200
 ERRNO_TO_DEVICE_ERROR = {
     2: -6,
@@ -121,14 +123,20 @@
             size -= struct.calcsize(CODE_FORMAT)
             with open(self.root_path / file_name, 'wb') as fd:
                 while size and code == CODE_FILE_DATA:
                     fd.write(self.service.recvall(size))
                     size, = struct.unpack(SIZE_FORMAT, self.service.recvall(struct.calcsize(SIZE_FORMAT)))
                     code, = struct.unpack(CODE_FORMAT, self.service.recvall(struct.calcsize(CODE_FORMAT)))
                     size -= struct.calcsize(CODE_FORMAT)
+            if code == CODE_ERROR_REMOTE:
+                # iOS 17 beta devices give this error for: backup_manifest.db
+                error_message = self.service.recvall(size).decode()
+                warnings.warn(f'Failed to fully upload: {file_name}. Device file name: {device_name}. Reason: '
+                              f'{error_message}')
+                continue
             assert code == CODE_SUCCESS
         self.status_response(0)
 
     def get_free_disk_space(self, message):
         freespace = shutil.disk_usage(self.root_path).free
         self.status_response(0, status_dict=freespace)
```

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/diagnostics.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dtfetchsymbols.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dtfetchsymbols.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/application_listing.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/application_listing.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/condition_inducer.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/condition_inducer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/device_info.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/device_info.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/energy_monitor.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/graphics.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/graphics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/location_simulation.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/location_simulation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/network_monitor.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/network_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/notifications.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/process_control.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/process_control.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/dvt/instruments/sysmontap.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/dvt/instruments/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/file_relay.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/file_relay.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/heartbeat.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/house_arrest.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/house_arrest.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/installation_proxy.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/lockdown_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/lockdown_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/misagent.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/misagent.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/mobile_activation.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/mobile_activation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/mobile_config.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/mobile_config.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/mobile_image_mounter.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/mobile_image_mounter.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/mobilebackup2.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/mobilebackup2.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/notification_proxy.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/os_trace.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/os_trace.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/pcapd.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/pcapd.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/power_assertion.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/preboard.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/preboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/remote_server.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/remote_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/restore_service.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/restore_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/screenshot.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/screenshot.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/simulate_location.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/simulate_location.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/springboard.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/syslog.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/alert.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/alert.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/automation_session.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/automation_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/cdp_screencast.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/cdp_screencast.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/cdp_server.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/cdp_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/cdp_target.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/cdp_target.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/driver.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/driver.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/element.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/element.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/inspector_session.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/inspector_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/selenium_api.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/selenium_api.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/session_protocol.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/session_protocol.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/web_protocol/switch_to.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/web_protocol/switch_to.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/services/webinspector.py` & `pymobiledevice3-2.2.2/pymobiledevice3/services/webinspector.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/tcp_forwarder.py` & `pymobiledevice3-2.2.2/pymobiledevice3/tcp_forwarder.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/usbmux.py` & `pymobiledevice3-2.2.2/pymobiledevice3/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3/utils.py` & `pymobiledevice3-2.2.2/pymobiledevice3/utils.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3.egg-info/PKG-INFO` & `pymobiledevice3-2.2.2/pymobiledevice3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.2.1
+Version: 2.2.2
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pymobiledevice3-2.2.1/pymobiledevice3.egg-info/SOURCES.txt` & `pymobiledevice3-2.2.2/pymobiledevice3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.2.1/pyproject.toml` & `pymobiledevice3-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymobiledevice3"
-version = "2.2.1"
+version = "2.2.2"
 description = "Pure python3 implementation for working with iDevices (iPhone, etc...)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "protocol", "lockdownd", "instruments", "automation", "cli", "afc"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```

