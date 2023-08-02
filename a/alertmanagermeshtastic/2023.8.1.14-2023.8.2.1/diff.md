# Comparing `tmp/alertmanagermeshtastic-2023.8.1.14.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.1.14.tar", last modified: Tue Aug  1 23:21:09 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.2.1.tar", last modified: Wed Aug  2 19:52:31 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.1.14.tar` & `alertmanagermeshtastic-2023.8.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.993284 alertmanagermeshtastic-2023.8.1.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:52:31.289447 alertmanagermeshtastic-2023.8.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-02 19:52:31.289447 alertmanagermeshtastic-2023.8.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-02 19:52:31.289447 alertmanagermeshtastic-2023.8.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:52:31.281447 alertmanagermeshtastic-2023.8.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:52:31.285447 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:52:31.285447 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 19:52:31.000000 alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:52:31.289447 alertmanagermeshtastic-2023.8.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-02 19:52:21.000000 alertmanagermeshtastic-2023.8.2.1/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.1.14/LICENSE` & `alertmanagermeshtastic-2023.8.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/PKG-INFO` & `alertmanagermeshtastic-2023.8.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.14
+Version: 2023.8.2.1
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
@@ -77,63 +77,67 @@
 timeout = 60
 ```
 
 
 ##  docker compose service example - Hardware Serial (default)
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanagermeshtastic
       ports:
         - 9119:9119
+      devices:
+        -/dev/ttyACM0
       volumes:
-        - /tmp/vcom0:/tmp/vcom0
         - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 ##  docker compose service example - Virtual Serial
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
+If you plan to use a virtual serial port that is provided with socat you have to use the socat connector in this container or run your alertmanagermeshtastic instance on the terminating linux machine, because the reconnecting is not working if you either mount it as volume or as a device.
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanagermeshtastic
       ports:
         - 9119:9119
+      environment:
+        - SOCAT_ENABLE=TRUE
+        - SOCAT_CONNECTION=tcp:192.168.178.46:5000
       volumes:
-        - /tmp/vcom0:/tmp/vcom0
         - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
+Note: If you set SOCAT_ENABLE to TRUE, the tty option from [meshtastic.connection] in config.toml will be overwritten with /tmp/vcom0 as thats the virtual serial port.
 
 ##  Running on docker example - Hardware Serial (default)
 
 ```
     docker run -d --name alertmanagermeshtastic \
 		--device=/dev/ttyACM0 \
 		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
     -p 9119:9119 apfelwurm/alertmanagermeshtastic:latest
 ```
 
 ##  Running on docker example - Virtual Serial
 
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
+If you plan to use a virtual serial port that is provided with socat you have to use the socat connector in this container or run your alertmanagermeshtastic instance on the terminating linux machine, because the reconnecting is not working if you either mount it as volume or as a device.
 
 ```
     docker run -d --name alertmanagermeshtastic \
-		-v /tmp/vcom0:/tmp/vcom0 \
+		--env SOCAT_ENABLE=TRUE --env SOCAT_CONNECTION=tcp:192.168.178.46:5000 \
 		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
     -p 9119:9119 apfelwurm/alertmanagermeshtastic:latest
 ```
+Note: If you set SOCAT_ENABLE to TRUE, the tty option from [meshtastic.connection] in config.toml will be overwritten with /tmp/vcom0 as thats the virtual serial port.
 
 ## Contribution
 
 This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. You can also take a look on the opened Issues, where i have opened some for planned features and work on them if you want. I would appreciate any help.
 
 
 ## Example to test
```

### Comparing `alertmanagermeshtastic-2023.8.1.14/README.md` & `alertmanagermeshtastic-2023.8.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -43,63 +43,67 @@
 timeout = 60
 ```
 
 
 ##  docker compose service example - Hardware Serial (default)
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanagermeshtastic
       ports:
         - 9119:9119
+      devices:
+        -/dev/ttyACM0
       volumes:
-        - /tmp/vcom0:/tmp/vcom0
         - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 ##  docker compose service example - Virtual Serial
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
+If you plan to use a virtual serial port that is provided with socat you have to use the socat connector in this container or run your alertmanagermeshtastic instance on the terminating linux machine, because the reconnecting is not working if you either mount it as volume or as a device.
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanagermeshtastic
       ports:
         - 9119:9119
+      environment:
+        - SOCAT_ENABLE=TRUE
+        - SOCAT_CONNECTION=tcp:192.168.178.46:5000
       volumes:
-        - /tmp/vcom0:/tmp/vcom0
         - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
+Note: If you set SOCAT_ENABLE to TRUE, the tty option from [meshtastic.connection] in config.toml will be overwritten with /tmp/vcom0 as thats the virtual serial port.
 
 ##  Running on docker example - Hardware Serial (default)
 
 ```
     docker run -d --name alertmanagermeshtastic \
 		--device=/dev/ttyACM0 \
 		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
     -p 9119:9119 apfelwurm/alertmanagermeshtastic:latest
 ```
 
 ##  Running on docker example - Virtual Serial
 
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
+If you plan to use a virtual serial port that is provided with socat you have to use the socat connector in this container or run your alertmanagermeshtastic instance on the terminating linux machine, because the reconnecting is not working if you either mount it as volume or as a device.
 
 ```
     docker run -d --name alertmanagermeshtastic \
-		-v /tmp/vcom0:/tmp/vcom0 \
+		--env SOCAT_ENABLE=TRUE --env SOCAT_CONNECTION=tcp:192.168.178.46:5000 \
 		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
     -p 9119:9119 apfelwurm/alertmanagermeshtastic:latest
 ```
+Note: If you set SOCAT_ENABLE to TRUE, the tty option from [meshtastic.connection] in config.toml will be overwritten with /tmp/vcom0 as thats the virtual serial port.
 
 ## Contribution
 
 This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. You can also take a look on the opened Issues, where i have opened some for planned features and work on them if you want. I would appreciate any help.
 
 
 ## Example to test
```

### Comparing `alertmanagermeshtastic-2023.8.1.14/setup.cfg` & `alertmanagermeshtastic-2023.8.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/meshtastic.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.14
+Version: 2023.8.2.1
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
@@ -77,63 +77,67 @@
 timeout = 60
 ```
 
 
 ##  docker compose service example - Hardware Serial (default)
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanagermeshtastic
       ports:
         - 9119:9119
+      devices:
+        -/dev/ttyACM0
       volumes:
-        - /tmp/vcom0:/tmp/vcom0
         - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 ##  docker compose service example - Virtual Serial
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
+If you plan to use a virtual serial port that is provided with socat you have to use the socat connector in this container or run your alertmanagermeshtastic instance on the terminating linux machine, because the reconnecting is not working if you either mount it as volume or as a device.
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanagermeshtastic
       ports:
         - 9119:9119
+      environment:
+        - SOCAT_ENABLE=TRUE
+        - SOCAT_CONNECTION=tcp:192.168.178.46:5000
       volumes:
-        - /tmp/vcom0:/tmp/vcom0
         - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
+Note: If you set SOCAT_ENABLE to TRUE, the tty option from [meshtastic.connection] in config.toml will be overwritten with /tmp/vcom0 as thats the virtual serial port.
 
 ##  Running on docker example - Hardware Serial (default)
 
 ```
     docker run -d --name alertmanagermeshtastic \
 		--device=/dev/ttyACM0 \
 		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
     -p 9119:9119 apfelwurm/alertmanagermeshtastic:latest
 ```
 
 ##  Running on docker example - Virtual Serial
 
-If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
+If you plan to use a virtual serial port that is provided with socat you have to use the socat connector in this container or run your alertmanagermeshtastic instance on the terminating linux machine, because the reconnecting is not working if you either mount it as volume or as a device.
 
 ```
     docker run -d --name alertmanagermeshtastic \
-		-v /tmp/vcom0:/tmp/vcom0 \
+		--env SOCAT_ENABLE=TRUE --env SOCAT_CONNECTION=tcp:192.168.178.46:5000 \
 		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
     -p 9119:9119 apfelwurm/alertmanagermeshtastic:latest
 ```
+Note: If you set SOCAT_ENABLE to TRUE, the tty option from [meshtastic.connection] in config.toml will be overwritten with /tmp/vcom0 as thats the virtual serial port.
 
 ## Contribution
 
 This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. You can also take a look on the opened Issues, where i have opened some for planned features and work on them if you want. I would appreciate any help.
 
 
 ## Example to test
```

### Comparing `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.2.1/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.2.1/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.2.1/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.2.1/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.2.1/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.2.1/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.14/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.2.1/tests/test_token_cli.py`

 * *Files identical despite different names*

