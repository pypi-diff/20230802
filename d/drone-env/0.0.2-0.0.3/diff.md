# Comparing `tmp/drone_env-0.0.2.tar.gz` & `tmp/drone_env-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drone_env-0.0.2.tar", last modified: Tue Aug  1 16:35:22 2023, max compression
+gzip compressed data, was "drone_env-0.0.3.tar", last modified: Wed Aug  2 01:48:24 2023, max compression
```

## Comparing `drone_env-0.0.2.tar` & `drone_env-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.054769 drone_env-0.0.2/
--rw-rw-rw-   0        0        0      105 2023-08-01 16:35:22.054769 drone_env-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.028976 drone_env-0.0.2/drone_env/
--rw-rw-rw-   0        0        0      134 2023-08-01 16:30:50.000000 drone_env-0.0.2/drone_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.052769 drone_env-0.0.2/drone_env/envs/
--rw-rw-rw-   0        0        0      171 2023-07-17 06:28:27.000000 drone_env-0.0.2/drone_env/envs/__init__.py
--rw-rw-rw-   0        0        0     8394 2023-08-01 14:47:42.000000 drone_env-0.0.2/drone_env/envs/drone_env.py
--rw-rw-rw-   0        0        0     3167 2023-07-17 06:58:43.000000 drone_env-0.0.2/drone_env/envs/simulink_connect.py
--rw-rw-rw-   0        0        0     4349 2023-08-01 14:25:09.000000 drone_env-0.0.2/drone_env/envs/track_generation.py
--rw-rw-rw-   0        0        0     2155 2023-08-01 07:44:59.000000 drone_env-0.0.2/drone_env/envs/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.053769 drone_env-0.0.2/drone_env/wrappers/
--rw-rw-rw-   0        0        0        0 2023-07-10 04:08:02.000000 drone_env-0.0.2/drone_env/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.048777 drone_env-0.0.2/drone_env.egg-info/
--rw-rw-rw-   0        0        0      105 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-08-01 16:35:22.000000 drone_env-0.0.2/drone_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 16:35:22.054769 drone_env-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-08-01 16:35:14.000000 drone_env-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:48:24.558594 drone_env-0.0.3/
+-rw-rw-rw-   0        0        0      105 2023-08-02 01:48:24.557595 drone_env-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 01:48:24.538594 drone_env-0.0.3/drone_env/
+-rw-rw-rw-   0        0        0      174 2023-08-02 01:45:33.000000 drone_env-0.0.3/drone_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:48:24.556594 drone_env-0.0.3/drone_env/envs/
+-rw-rw-rw-   0        0        0      206 2023-08-02 01:45:33.000000 drone_env-0.0.3/drone_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     8397 2023-08-02 01:45:33.000000 drone_env-0.0.3/drone_env/envs/drone_env.py
+-rw-rw-rw-   0        0        0     3167 2023-07-17 06:58:43.000000 drone_env-0.0.3/drone_env/envs/simulink_connect.py
+-rw-rw-rw-   0        0        0     4350 2023-08-02 01:45:33.000000 drone_env-0.0.3/drone_env/envs/track_generation.py
+-rw-rw-rw-   0        0        0     2155 2023-08-01 07:44:59.000000 drone_env-0.0.3/drone_env/envs/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:48:24.557595 drone_env-0.0.3/drone_env/wrappers/
+-rw-rw-rw-   0        0        0        0 2023-07-10 04:08:02.000000 drone_env-0.0.3/drone_env/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:48:24.552594 drone_env-0.0.3/drone_env.egg-info/
+-rw-rw-rw-   0        0        0      105 2023-08-02 01:48:24.000000 drone_env-0.0.3/drone_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-08-02 01:48:24.000000 drone_env-0.0.3/drone_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 01:48:24.000000 drone_env-0.0.3/drone_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-02 01:48:24.000000 drone_env-0.0.3/drone_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 01:48:24.000000 drone_env-0.0.3/drone_env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 01:48:24.558594 drone_env-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-08-02 01:45:33.000000 drone_env-0.0.3/setup.py
```

### Comparing `drone_env-0.0.2/drone_env/envs/drone_env.py` & `drone_env-0.0.3/drone_env/envs/drone_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gymnasium as gym
 import numpy as np
 from gymnasium import spaces
-from simulink_connect import MatlabProjectPlant
-from track_generation import TrackGenerator
-from utils import separation, projection, offtrack
+from .simulink_connect import MatlabProjectPlant
+from .track_generation import TrackGenerator
+from .utils import separation, projection, offtrack
 
 
 class DroneEnv(gym.Env):
     metadata = {"render.modes": ["human"]}
 
     def __init__(self):
         super().__init__()
```

### Comparing `drone_env-0.0.2/drone_env/envs/simulink_connect.py` & `drone_env-0.0.3/drone_env/envs/simulink_connect.py`

 * *Files identical despite different names*

### Comparing `drone_env-0.0.2/drone_env/envs/track_generation.py` & `drone_env-0.0.3/drone_env/envs/track_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from itertools import combinations
-from utils import separation, intersect
+from .utils import separation, intersect
 
 
 class TrackGenerator:
     def __init__(self, size, border, collinear_threshold, separation_threshold, segment_count=0):
         self.offset = None
         self.scale = None
         if segment_count == 0:
```

### Comparing `drone_env-0.0.2/drone_env/envs/utils.py` & `drone_env-0.0.3/drone_env/envs/utils.py`

 * *Files identical despite different names*

