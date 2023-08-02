# Comparing `tmp/gonio-imsoft-0.0.2.tar.gz` & `tmp/gonio-imsoft-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gonio-imsoft-0.0.2.tar", last modified: Sun May  2 20:28:07 2021, max compression
+gzip compressed data, was "gonio-imsoft-0.1.0.tar", last modified: Wed Aug  2 06:42:12 2023, max compression
```

## Comparing `gonio-imsoft-0.0.2.tar` & `gonio-imsoft-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,29 @@
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.426960 gonio-imsoft-0.0.2/
--rw-r--r--   0 joni      (1000) joni      (1000)     1799 2021-04-29 13:37:46.000000 gonio-imsoft-0.0.2/.gitignore
--rw-r--r--   0 joni      (1000) joni      (1000)    35150 2021-05-01 15:44:45.000000 gonio-imsoft-0.0.2/LICENSE
--rw-r--r--   0 joni      (1000) joni      (1000)     3445 2021-05-02 20:28:07.425960 gonio-imsoft-0.0.2/PKG-INFO
--rwxr-xr-x   0 joni      (1000) joni      (1000)     2326 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/README.md
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.419960 gonio-imsoft-0.0.2/gonio_imsoft.egg-info/
--rw-r--r--   0 joni      (1000) joni      (1000)     3445 2021-05-02 20:28:07.000000 gonio-imsoft-0.0.2/gonio_imsoft.egg-info/PKG-INFO
--rw-r--r--   0 joni      (1000) joni      (1000)     1462 2021-05-02 20:28:07.000000 gonio-imsoft-0.0.2/gonio_imsoft.egg-info/SOURCES.txt
--rw-r--r--   0 joni      (1000) joni      (1000)        1 2021-05-02 20:28:07.000000 gonio-imsoft-0.0.2/gonio_imsoft.egg-info/dependency_links.txt
--rw-r--r--   0 joni      (1000) joni      (1000)       63 2021-05-02 20:28:07.000000 gonio-imsoft-0.0.2/gonio_imsoft.egg-info/requires.txt
--rw-r--r--   0 joni      (1000) joni      (1000)       12 2021-05-02 20:28:07.000000 gonio-imsoft-0.0.2/gonio_imsoft.egg-info/top_level.txt
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.422960 gonio-imsoft-0.0.2/gonioimsoft/
--rw-r--r--   0 joni      (1000) joni      (1000)        2 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/__init__.py
--rwxr-xr-x   0 joni      (1000) joni      (1000)      986 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/anglepairs.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.417960 gonio-imsoft-0.0.2/gonioimsoft/arduino/
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.422960 gonio-imsoft-0.0.2/gonioimsoft/arduino/angle_sensors/
--rw-r--r--   0 joni      (1000) joni      (1000)     1126 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/arduino/angle_sensors/angle_sensors.ino
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.422960 gonio-imsoft-0.0.2/gonioimsoft/arduino/combined_sensors_motors/
--rw-r--r--   0 joni      (1000) joni      (1000)     4826 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/arduino/combined_sensors_motors/combined_sensors_motors.ino
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.422960 gonio-imsoft-0.0.2/gonioimsoft/arduino/focus/
--rw-r--r--   0 joni      (1000) joni      (1000)      755 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/arduino/focus/focus.ino
--rwxr-xr-x   0 joni      (1000) joni      (1000)     3526 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/arduino_serial.py
--rwxr-xr-x   0 joni      (1000) joni      (1000)     4634 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/camera_client.py
--rw-r--r--   0 joni      (1000) joni      (1000)      438 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/camera_communication.py
--rwxr-xr-x   0 joni      (1000) joni      (1000)    16694 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/camera_server.py
--rw-r--r--   0 joni      (1000) joni      (1000)    22286 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/core.py
--rw-r--r--   0 joni      (1000) joni      (1000)      338 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/directories.py
--rw-r--r--   0 joni      (1000) joni      (1000)    11006 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/imaging_parameters.py
--rw-r--r--   0 joni      (1000) joni      (1000)       13 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/imsoft.cmd
--rw-r--r--   0 joni      (1000) joni      (1000)    26886 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/logo.ico
--rw-r--r--   0 joni      (1000) joni      (1000)   242832 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/logo.tif
--rw-r--r--   0 joni      (1000) joni      (1000)      897 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/macro.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.422960 gonio-imsoft-0.0.2/gonioimsoft/macros/
--rw-r--r--   0 joni      (1000) joni      (1000)     1593 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/macros/default.txt
--rw-r--r--   0 joni      (1000) joni      (1000)      463 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/make_macro.py
--rw-r--r--   0 joni      (1000) joni      (1000)     4539 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/motors.py
-drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2021-05-02 20:28:07.425960 gonio-imsoft-0.0.2/gonioimsoft/presets/
--rw-r--r--   0 joni      (1000) joni      (1000)      427 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/3step_100ms
--rw-r--r--   0 joni      (1000) joni      (1000)      402 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/default
--rw-r--r--   0 joni      (1000) joni      (1000)      337 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/intensity_series_10p_log
--rw-r--r--   0 joni      (1000) joni      (1000)      763 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/intensser_25p
--rw-r--r--   0 joni      (1000) joni      (1000)      768 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/intensser_25p_isi2s
--rw-r--r--   0 joni      (1000) joni      (1000)      732 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/isisser_25p
--rw-r--r--   0 joni      (1000) joni      (1000)      407 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/manyrepeats
--rw-r--r--   0 joni      (1000) joni      (1000)      412 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/manyrepeats_isi2s
--rw-r--r--   0 joni      (1000) joni      (1000)      306 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/manyrepeats_isi2s_frombg
--rw-r--r--   0 joni      (1000) joni      (1000)      308 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/manyrepeats_isi2s_todark
--rw-r--r--   0 joni      (1000) joni      (1000)      363 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/prettyimages
--rw-r--r--   0 joni      (1000) joni      (1000)      395 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/rotation_trigger
--rw-r--r--   0 joni      (1000) joni      (1000)      399 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/sinelogsweep
--rw-r--r--   0 joni      (1000) joni      (1000)      428 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/sinelogsweep_cam200Hz
--rw-r--r--   0 joni      (1000) joni      (1000)      432 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/squarelogsweep_cam200Hz
--rw-r--r--   0 joni      (1000) joni      (1000)      434 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/presets/squarewave_cam200Hz
--rw-r--r--   0 joni      (1000) joni      (1000)     5223 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/stimulus.py
--rw-r--r--   0 joni      (1000) joni      (1000)    19420 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/tui.py
--rw-r--r--   0 joni      (1000) joni      (1000)       23 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/gonioimsoft/version.py
--rw-r--r--   0 joni      (1000) joni      (1000)       38 2021-05-02 20:28:07.426960 gonio-imsoft-0.0.2/setup.cfg
--rw-r--r--   0 joni      (1000) joni      (1000)     1072 2021-05-02 20:27:16.000000 gonio-imsoft-0.0.2/setup.py
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-02 06:42:12.964060 gonio-imsoft-0.1.0/
+-rw-r--r--   0 joni      (1000) joni      (1000)    35150 2022-02-19 20:03:01.000000 gonio-imsoft-0.1.0/LICENSE
+-rw-r--r--   0 joni      (1000) joni      (1000)     3387 2023-08-02 06:42:12.964060 gonio-imsoft-0.1.0/PKG-INFO
+-rwxr-xr-x   0 joni      (1000) joni      (1000)     2921 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/README.md
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-02 06:42:12.960060 gonio-imsoft-0.1.0/gonio_imsoft.egg-info/
+-rw-r--r--   0 joni      (1000) joni      (1000)     3387 2023-08-02 06:42:12.000000 gonio-imsoft-0.1.0/gonio_imsoft.egg-info/PKG-INFO
+-rw-r--r--   0 joni      (1000) joni      (1000)      617 2023-08-02 06:42:12.000000 gonio-imsoft-0.1.0/gonio_imsoft.egg-info/SOURCES.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)        1 2023-08-02 06:42:12.000000 gonio-imsoft-0.1.0/gonio_imsoft.egg-info/dependency_links.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)       72 2023-08-02 06:42:12.000000 gonio-imsoft-0.1.0/gonio_imsoft.egg-info/requires.txt
+-rw-r--r--   0 joni      (1000) joni      (1000)       12 2023-08-02 06:42:12.000000 gonio-imsoft-0.1.0/gonio_imsoft.egg-info/top_level.txt
+drwxr-xr-x   0 joni      (1000) joni      (1000)        0 2023-08-02 06:42:12.964060 gonio-imsoft-0.1.0/gonioimsoft/
+-rw-r--r--   0 joni      (1000) joni      (1000)        2 2022-02-19 20:03:01.000000 gonio-imsoft-0.1.0/gonioimsoft/__init__.py
+-rwxr-xr-x   0 joni      (1000) joni      (1000)      986 2022-02-19 20:03:01.000000 gonio-imsoft-0.1.0/gonioimsoft/anglepairs.py
+-rwxr-xr-x   0 joni      (1000) joni      (1000)     4327 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/arduino_serial.py
+-rwxr-xr-x   0 joni      (1000) joni      (1000)    10842 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/camera_client.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      202 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/camera_communication.py
+-rwxr-xr-x   0 joni      (1000) joni      (1000)    25064 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/camera_server.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    25196 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/core.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     1105 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/directories.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    11880 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/imaging_parameters.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     5471 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/libtui.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      959 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/macro.py
+-rw-r--r--   0 joni      (1000) joni      (1000)      463 2022-02-19 20:03:01.000000 gonio-imsoft-0.1.0/gonioimsoft/make_macro.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     4539 2022-02-19 20:03:01.000000 gonio-imsoft-0.1.0/gonioimsoft/motors.py
+-rw-r--r--   0 joni      (1000) joni      (1000)     7461 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/stimulus.py
+-rw-r--r--   0 joni      (1000) joni      (1000)    22155 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/tui.py
+-rw-r--r--   0 joni      (1000) joni      (1000)       23 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/gonioimsoft/version.py
+-rw-r--r--   0 joni      (1000) joni      (1000)       38 2023-08-02 06:42:12.964060 gonio-imsoft-0.1.0/setup.cfg
+-rw-r--r--   0 joni      (1000) joni      (1000)     1093 2023-08-02 06:11:02.000000 gonio-imsoft-0.1.0/setup.py
```

### Comparing `gonio-imsoft-0.0.2/LICENSE` & `gonio-imsoft-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gonio-imsoft-0.0.2/PKG-INFO` & `gonio-imsoft-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 Metadata-Version: 2.1
 Name: gonio-imsoft
-Version: 0.0.2
+Version: 0.1.0
 Summary: Goniometric imaging software
 Home-page: https://github.com/jkemppainen/gonio-imsoft
 Author: Joni Kemppainen
-Author-email: jjtkemppainen1@sheffield.ac.uk
-License: UNKNOWN
-Description: # Goniometric imaging software
-        
-        Gonio Imsoft is a command line Python program designed to control the
-        goniometric high-speed imaging experiments where
-        
-        * rotary encoder values are read over serial (pySerial)
-        * NI-DAQmx is used for general input/output (nidaqmx)
-        * the camera is controlled over MicroManager (MMCorePy)
-        
-        It was developed for the need of imaging 200 distinct
-        rotations (eye locations) per specimen fast, requiring
-        only the space bar to be pressed between the rotations.
-        
-        For general imaging, it is more convinient
-        to use MicroManager or similar.
-        
-        
-        ## Required hardware and current limitations
-        
-        * Any MicroManager supported imaging device
-        * Any National Instruments input/output board (NI specificity can be lifted in
-          future by using PyVISA or similar)
-        * Any serial device reporting rotation values in format "pos1,pos2\n"
-        
-        There are currently some limitations however (to be fixed soon)
-        
-        1) Imsoft yet lacks dialogs to select and configure
-          devices in a user-friendly manner.
-          Currently, the same can be achieved by modifications in
-          `camera_server.Camera.__init__`, `core.Dynamic.analog_output`
-          and `arduino_serial.ArduinoReader`.
-        
-        1) At least previously, MicroManager used to ship only Python 2 bindings
-          and because of this, the *camera_server.py*
-          has to be ran with Python 2 and rest of the software with
-          Python 3.
-        
-        1) Some parts only work on Windows (nidaqmx and msvcrt modules)
-        
-        
-        ## How to install
-        
-        ### Rotary encoders
-        
-        We connected two 1024-step rotary encoders to two perpendicular
-        rotation stages (goniometers), and used Arduino for readout.
-        
-        When using similar setup to us, you can modify and flash 
-        `arduino/angle_sensors/angle_sensors.ino`, and use Serial Monitor
-        in the Arduino IDE to confirm that the readout work.
-        
-        Alternatively, any serial device reporting rotations in format "pos1,pos2\n"
-        where pos1 and pos2 are rotation steps of the two encoders will do.
-        
-        
-        ### Main software
-        
-        First please make sure that you have
-        * MicroManager installation with a working camera
-        * National Insturments cards configured with names *Dev1* and *Dev2* for input
-          and output, respectively
-        * Python 3 and Python 2
-        
-        Then, with Python 3's pip
-        
-        ```
-        pip install gonio-imsoft
-        ```
-        
-        ## How to use
-        
-        ```
-        python -m gonioimsoft.tui
-        ```
-        
-        
-Platform: UNKNOWN
+Author-email: joni.kemppainen@windowslive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
-Requires-Python: >=3.0
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Goniometric imaging software
+
+GonioImsoft is a terminal user interface Python program
+designed to control the
+goniometric high-speed imaging experiments where
+
+* rotary encoder values are read over serial (pySerial)
+* NI-DAQmx is used for general input/output (nidaqmx)
+* the camera is controlled over MicroManager (pymmcore)
+
+It was developed for the need of imaging 200 distinct
+rotations (eye locations) per specimen fast, requiring
+only the space bar to be pressed between the rotations.
+
+For general imaging, without these specific needs,
+it is better to use MicroManager or other image
+acquisition software.
+
+Following block diagram illustrates the used software architecture
+
+´´´
+tui.py - GonioImsoft terminal user interface
+  |
+core.py
+  |
+  |__ nidaqmx - Control NI boards (trigger, stimuli)
+  |
+  |__ pyserial - Read Arduino (rotation data)
+  |
+  |__ Camera Client
+        |_Camera Server
+	    |
+	    |__ pymmcore - camera control using MicroManager
+	    |__ tifffile - writes images/stacks
+´´´
+
+Thanks to the camera server/client model,
+the cameras can be ran on separate computers.
+This parallel image acquisition allows using many cameras
+without worrying about memory and bandwidth or processing
+limits.
+
+
+
+## Required hardware and current limitations
+
+Windows (and Linux to some extent) tested.
+
+* A MicroManager-supported camera device
+* National Instruments input/output board (NI specificity can be
+  lifted in future by using PyVISA or similar)
+* Serial device reporting rotation values in format "pos1,pos2\n"
+
+For full description of the used hardware configuration,
+please see
+[the GHS-DPP imaging methods article](https://www.nature.com/articles/s42003-022-03142-0)
+
+
+## How to install
+
+
+### Rotary encoders
+
+Rotary encoders monitor the rotation of the imaged specimen/sample.
+They are
+mechanically attached to their respective rotation stages.
+Their state is digitally read out using an Arduino microcontroller.
+
+In our system, we used two 1024-step rotary encoders attached on
+two perpendicular rotation stages.
+If your system is identical, you can flash 
+`arduino/angle_sensors/angle_sensors.ino` and use the Serial Monitor
+in the Arduino IDE to confirm it works.
+
+If your system differs, you may have to modify the Arduino `ino` file.
+However, any serial device reporting rotations in format "pos1,pos2\n"
+will do. Here, pos1 and pos2 are rotation steps (integers)
+of the two encoders.
+
+
+### Main software (using pip)
+
+First please make sure that you have
+* MicroManager installation with a working camera
+* National Insturments cards configured with
+names *Dev1* and *Dev2* for input and output, respectively
+* Python 3.6 or newer
+
+Then, use pip to install
+
+```
+pip install gonio-imsoft
+```
+
+## How to use
+
+You can launch the main program using
+
+```
+python -m gonioimsoft.tui
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gonio-imsoft-0.0.2/README.md` & `gonio-imsoft-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,103 @@
 # Goniometric imaging software
 
-Gonio Imsoft is a command line Python program designed to control the
+GonioImsoft is a terminal user interface Python program
+designed to control the
 goniometric high-speed imaging experiments where
 
 * rotary encoder values are read over serial (pySerial)
 * NI-DAQmx is used for general input/output (nidaqmx)
-* the camera is controlled over MicroManager (MMCorePy)
+* the camera is controlled over MicroManager (pymmcore)
 
 It was developed for the need of imaging 200 distinct
 rotations (eye locations) per specimen fast, requiring
 only the space bar to be pressed between the rotations.
 
-For general imaging, it is more convinient
-to use MicroManager or similar.
+For general imaging, without these specific needs,
+it is better to use MicroManager or other image
+acquisition software.
+
+Following block diagram illustrates the used software architecture
+
+´´´
+tui.py - GonioImsoft terminal user interface
+  |
+core.py
+  |
+  |__ nidaqmx - Control NI boards (trigger, stimuli)
+  |
+  |__ pyserial - Read Arduino (rotation data)
+  |
+  |__ Camera Client
+        |_Camera Server
+	    |
+	    |__ pymmcore - camera control using MicroManager
+	    |__ tifffile - writes images/stacks
+´´´
+
+Thanks to the camera server/client model,
+the cameras can be ran on separate computers.
+This parallel image acquisition allows using many cameras
+without worrying about memory and bandwidth or processing
+limits.
+
 
 
 ## Required hardware and current limitations
 
-* Any MicroManager supported imaging device
-* Any National Instruments input/output board (NI specificity can be lifted in
-  future by using PyVISA or similar)
-* Any serial device reporting rotation values in format "pos1,pos2\n"
-
-There are currently some limitations however (to be fixed soon)
-
-1) Imsoft yet lacks dialogs to select and configure
-  devices in a user-friendly manner.
-  Currently, the same can be achieved by modifications in
-  `camera_server.Camera.__init__`, `core.Dynamic.analog_output`
-  and `arduino_serial.ArduinoReader`.
-
-1) At least previously, MicroManager used to ship only Python 2 bindings
-  and because of this, the *camera_server.py*
-  has to be ran with Python 2 and rest of the software with
-  Python 3.
+Windows (and Linux to some extent) tested.
 
-1) Some parts only work on Windows (nidaqmx and msvcrt modules)
+* A MicroManager-supported camera device
+* National Instruments input/output board (NI specificity can be
+  lifted in future by using PyVISA or similar)
+* Serial device reporting rotation values in format "pos1,pos2\n"
+
+For full description of the used hardware configuration,
+please see
+[the GHS-DPP imaging methods article](https://www.nature.com/articles/s42003-022-03142-0)
 
 
 ## How to install
 
-### Rotary encoders
-
-We connected two 1024-step rotary encoders to two perpendicular
-rotation stages (goniometers), and used Arduino for readout.
 
-When using similar setup to us, you can modify and flash 
-`arduino/angle_sensors/angle_sensors.ino`, and use Serial Monitor
-in the Arduino IDE to confirm that the readout work.
+### Rotary encoders
 
-Alternatively, any serial device reporting rotations in format "pos1,pos2\n"
-where pos1 and pos2 are rotation steps of the two encoders will do.
+Rotary encoders monitor the rotation of the imaged specimen/sample.
+They are
+mechanically attached to their respective rotation stages.
+Their state is digitally read out using an Arduino microcontroller.
+
+In our system, we used two 1024-step rotary encoders attached on
+two perpendicular rotation stages.
+If your system is identical, you can flash 
+`arduino/angle_sensors/angle_sensors.ino` and use the Serial Monitor
+in the Arduino IDE to confirm it works.
+
+If your system differs, you may have to modify the Arduino `ino` file.
+However, any serial device reporting rotations in format "pos1,pos2\n"
+will do. Here, pos1 and pos2 are rotation steps (integers)
+of the two encoders.
 
 
-### Main software
+### Main software (using pip)
 
 First please make sure that you have
 * MicroManager installation with a working camera
-* National Insturments cards configured with names *Dev1* and *Dev2* for input
-  and output, respectively
-* Python 3 and Python 2
+* National Insturments cards configured with
+names *Dev1* and *Dev2* for input and output, respectively
+* Python 3.6 or newer
 
-Then, with Python 3's pip
+Then, use pip to install
 
 ```
 pip install gonio-imsoft
 ```
 
 ## How to use
 
+You can launch the main program using
+
 ```
 python -m gonioimsoft.tui
 ```
 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gonio-imsoft-0.0.2/gonio_imsoft.egg-info/PKG-INFO` & `gonio-imsoft-0.1.0/gonio_imsoft.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 Metadata-Version: 2.1
 Name: gonio-imsoft
-Version: 0.0.2
+Version: 0.1.0
 Summary: Goniometric imaging software
 Home-page: https://github.com/jkemppainen/gonio-imsoft
 Author: Joni Kemppainen
-Author-email: jjtkemppainen1@sheffield.ac.uk
-License: UNKNOWN
-Description: # Goniometric imaging software
-        
-        Gonio Imsoft is a command line Python program designed to control the
-        goniometric high-speed imaging experiments where
-        
-        * rotary encoder values are read over serial (pySerial)
-        * NI-DAQmx is used for general input/output (nidaqmx)
-        * the camera is controlled over MicroManager (MMCorePy)
-        
-        It was developed for the need of imaging 200 distinct
-        rotations (eye locations) per specimen fast, requiring
-        only the space bar to be pressed between the rotations.
-        
-        For general imaging, it is more convinient
-        to use MicroManager or similar.
-        
-        
-        ## Required hardware and current limitations
-        
-        * Any MicroManager supported imaging device
-        * Any National Instruments input/output board (NI specificity can be lifted in
-          future by using PyVISA or similar)
-        * Any serial device reporting rotation values in format "pos1,pos2\n"
-        
-        There are currently some limitations however (to be fixed soon)
-        
-        1) Imsoft yet lacks dialogs to select and configure
-          devices in a user-friendly manner.
-          Currently, the same can be achieved by modifications in
-          `camera_server.Camera.__init__`, `core.Dynamic.analog_output`
-          and `arduino_serial.ArduinoReader`.
-        
-        1) At least previously, MicroManager used to ship only Python 2 bindings
-          and because of this, the *camera_server.py*
-          has to be ran with Python 2 and rest of the software with
-          Python 3.
-        
-        1) Some parts only work on Windows (nidaqmx and msvcrt modules)
-        
-        
-        ## How to install
-        
-        ### Rotary encoders
-        
-        We connected two 1024-step rotary encoders to two perpendicular
-        rotation stages (goniometers), and used Arduino for readout.
-        
-        When using similar setup to us, you can modify and flash 
-        `arduino/angle_sensors/angle_sensors.ino`, and use Serial Monitor
-        in the Arduino IDE to confirm that the readout work.
-        
-        Alternatively, any serial device reporting rotations in format "pos1,pos2\n"
-        where pos1 and pos2 are rotation steps of the two encoders will do.
-        
-        
-        ### Main software
-        
-        First please make sure that you have
-        * MicroManager installation with a working camera
-        * National Insturments cards configured with names *Dev1* and *Dev2* for input
-          and output, respectively
-        * Python 3 and Python 2
-        
-        Then, with Python 3's pip
-        
-        ```
-        pip install gonio-imsoft
-        ```
-        
-        ## How to use
-        
-        ```
-        python -m gonioimsoft.tui
-        ```
-        
-        
-Platform: UNKNOWN
+Author-email: joni.kemppainen@windowslive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
-Requires-Python: >=3.0
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Goniometric imaging software
+
+GonioImsoft is a terminal user interface Python program
+designed to control the
+goniometric high-speed imaging experiments where
+
+* rotary encoder values are read over serial (pySerial)
+* NI-DAQmx is used for general input/output (nidaqmx)
+* the camera is controlled over MicroManager (pymmcore)
+
+It was developed for the need of imaging 200 distinct
+rotations (eye locations) per specimen fast, requiring
+only the space bar to be pressed between the rotations.
+
+For general imaging, without these specific needs,
+it is better to use MicroManager or other image
+acquisition software.
+
+Following block diagram illustrates the used software architecture
+
+´´´
+tui.py - GonioImsoft terminal user interface
+  |
+core.py
+  |
+  |__ nidaqmx - Control NI boards (trigger, stimuli)
+  |
+  |__ pyserial - Read Arduino (rotation data)
+  |
+  |__ Camera Client
+        |_Camera Server
+	    |
+	    |__ pymmcore - camera control using MicroManager
+	    |__ tifffile - writes images/stacks
+´´´
+
+Thanks to the camera server/client model,
+the cameras can be ran on separate computers.
+This parallel image acquisition allows using many cameras
+without worrying about memory and bandwidth or processing
+limits.
+
+
+
+## Required hardware and current limitations
+
+Windows (and Linux to some extent) tested.
+
+* A MicroManager-supported camera device
+* National Instruments input/output board (NI specificity can be
+  lifted in future by using PyVISA or similar)
+* Serial device reporting rotation values in format "pos1,pos2\n"
+
+For full description of the used hardware configuration,
+please see
+[the GHS-DPP imaging methods article](https://www.nature.com/articles/s42003-022-03142-0)
+
+
+## How to install
+
+
+### Rotary encoders
+
+Rotary encoders monitor the rotation of the imaged specimen/sample.
+They are
+mechanically attached to their respective rotation stages.
+Their state is digitally read out using an Arduino microcontroller.
+
+In our system, we used two 1024-step rotary encoders attached on
+two perpendicular rotation stages.
+If your system is identical, you can flash 
+`arduino/angle_sensors/angle_sensors.ino` and use the Serial Monitor
+in the Arduino IDE to confirm it works.
+
+If your system differs, you may have to modify the Arduino `ino` file.
+However, any serial device reporting rotations in format "pos1,pos2\n"
+will do. Here, pos1 and pos2 are rotation steps (integers)
+of the two encoders.
+
+
+### Main software (using pip)
+
+First please make sure that you have
+* MicroManager installation with a working camera
+* National Insturments cards configured with
+names *Dev1* and *Dev2* for input and output, respectively
+* Python 3.6 or newer
+
+Then, use pip to install
+
+```
+pip install gonio-imsoft
+```
+
+## How to use
+
+You can launch the main program using
+
+```
+python -m gonioimsoft.tui
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/anglepairs.py` & `gonio-imsoft-0.1.0/gonioimsoft/anglepairs.py`

 * *Files identical despite different names*

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/arduino_serial.py` & `gonio-imsoft-0.1.0/gonioimsoft/arduino_serial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 '''
 1) Reading rotation encoder signals from an Arduino Board.
 2) and controlling stepper motors.
 '''
 
 try:
     import serial
+    from serial.tools.list_ports import comports
 except ModuleNotFoundError:
     serial = None
 
-DEFAULT_PORT_NAME = 'COM4'
+
 
 class ArduinoReader:
     '''
     Class for reading  angle pairs (states of the rotation encoders) from Arduino.
     '''
 
-    def __init__(self, port=DEFAULT_PORT_NAME):
+    def __init__(self, port=None):
         '''
         port        On Windows, "COM4" or similar. May change if other serial devices
                     are addded or removed?
         '''
         
         if serial:
-            self.serial = serial.Serial(port=port, baudrate=9600, timeout=0.01)
+            if port is None:
+                # No port provided, use the first one with text "Arduino" in it
+                ports = [str(p) for p in comports()]
+                print(f'Selecting an Arduino from {ports}')
+                for port in ports:
+                    if not 'arduino' in port.lower():
+                        continue
+                    print(f'  Trying {port}')
+                    try:
+                        self.serial = serial.Serial(port=port.split(' ')[0], baudrate=9600, timeout=0.01)
+                        self.serial.readline()
+                        print(f'Accepted port {port}')
+                        break
+                    except Exception as e:
+                        print(e)
+            else:
+                # Use the provided port
+                self.serial = serial.Serial(port=port, baudrate=9600, timeout=0.01)
         else:
             self.serial = None
 
         self.latest_angle = (0,0)
         self.offset = (0,0)
 
     def _offset_correct(self, angles):
```

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/camera_server.py` & `gonio-imsoft-0.1.0/gonioimsoft/camera_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,72 @@
-'''
-Image accusition using Micro-Manager's Python (2) bindings (Camera class)
-and a server program (CameraServer class).
+'''The camera server for using the camera and save images.
 
-On Windows, MM builds come compiled with Python 2 support only, so in this solution
-there is a Python 2 server program that controls the camera and image saving
-and then the client end that can be run with Python 3.
+Functionality
+-------------
+- Image acquisition using Micro-Manager's Python bindings (pymmcore)
+- Live feed using matplotlib
+- File saving using the tifffile module
+
+
+Background
+-----------
+On Windows, MM builds came precompiled with Python 2 support only. The
+camera server/client division here made it possible to run the server
+calling MM using Python 2 (to control the camera and image saving) and
+then the camera client run with Python 3.
+
+It is still usefull; Because it uses (network) sockets, it is trivial
+to use another (or multiple PC) to acqurie images. Or, in future, to
+use another backends than MM.
 '''
 
 import os
+import sys
 import time
 import datetime
 import socket
+import argparse
 import threading
 import multiprocessing
 
-import MMCorePy
+try:
+    import pymmcore
+except ImportError:
+    pymmcore = None
+    print('pymmcore not installed')
 import tifffile
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 from matplotlib.widgets import RectangleSelector
 
-import camera_communication as cac
-from camera_communication import SAVING_DRIVE
-
-DEFAULT_SAVING_DIRECTORY = "D:\imaging_data"
+from .camera_communication import PORT
 
+DEFAULT_SAVING_DIRECTORY = "imaging_data"
+DEFAULT_MICROMANAGER_DIR = 'C:/Program Files/Micro-Manager-2.0'
 
+# Integer between 1-inf (1 = no downsampling), images for imageshower
+LIVE_DOWNSAMPLE = 2
 
 class ImageShower:
-    '''
-    Showing images on the screen on its own window.
+    '''Shows images on the screen in its own window.
 
     In future, may be used to select ROIs as well to allow
     higher frame rate imaging / less data.
     
     ------------------
     Working principle
     ------------------
     Image shower works so that self.loop is started as a separate process
     using multiprocessing library
     
     -------
     Methods
     -------
     self.loop       Set this as multiprocessing target
-
     '''
     def __init__(self):
         self.fig = plt.figure()
         self.ax = self.fig.add_subplot(111)
         self.close = False
 
         #self.cid = self.fig.canvas.mpl_connect('key_press_event', self.callbackButtonPressed)
@@ -91,15 +108,15 @@
         
         data = None
         while not self.queue.empty():
             # Get the latest image in the queue
             data = self.queue.get(True, timeout=0.01)
         if data is None:
             return self.im, ''
-        elif data == 'close':
+        elif isinstance(data, str) and data == 'close':
             self.close = True
             return self.im, ''
 
         if self.selection and data.size != self.image_size:
             self.selection = None
 
         if self.selection:
@@ -111,240 +128,390 @@
             else:
                 inspect_area = data[y:y+h, x:x+w]
         else:
             inspect_area = data
         
         
         per95 = np.percentile(inspect_area, 95)
-        data = np.clip(data, np.percentile(inspect_area, 5), per95)
+        per5 = np.percentile(inspect_area, 5)
+        data = np.clip(data, per5, per95)
         
-        data = data - np.min(data)
-        data_max = np.max(data)
-        data = data.astype(float)/data_max
+        data -= per5
+        data /= (per95-per5)
 
         self.image_size = data.size
-       
         
         self.im.set_array(data)
         self.fig.suptitle('Selection 95th percentile: {}'.format(per95), fontsize=10)
         text = ''
         return self.im, text
            
          
-    def loop(self, queue):
+    def loop(self, queue, title):
         '''
         Runs the ImageShower by reading images from the given queue.
         Set this as a multiprocessing target.
 
         queue           Multiprocessing queue with a get method.
         '''
         self.queue = queue
         self.rectangle = RectangleSelector(self.ax, self.__onSelectRectangle, useblit=True)
         
         image = queue.get()
         self.im = plt.imshow(1000*image/np.max(image), cmap='gray', vmin=0, vmax=1, interpolation='none', aspect='auto')
-        self.ani = FuncAnimation(plt.gcf(), self._updateImage, frames=range(100), interval=5, blit=False)
+        self.ani = FuncAnimation(plt.gcf(), self._updateImage, frames=range(100), interval=50, blit=False)
+
+        self.fig.canvas.toolbar.winfo_toplevel().title(title)
 
-        plt.show(block=False)
+        # Remove the toolbar; Gives more space when having many cameras
+        self.fig.canvas.toolbar.pack_forget()
+        
+        # Take away all white space
+        plt.subplots_adjust(top=1, bottom=0, right=1,left=0,
+                            hspace=0, wspace=0)
         
-        while not self.close:
-            plt.pause(1)
+        plt.show(block=True)
 
 
 class DummyCamera:
+    '''A dummy camera suitable for testing the server/client.
     '''
-    A dummy camera class, used when unable to load the real Camera class
-    due to camera being off or something similar.
-    '''
+    def __init__(self):
+        self.settings = {'setting1' : 'na', 'setting2': 0.0, 'setting3': 1}
+        self.camera = None
+
     def acquire_single(self, save, subdir):
         pass
-    def acquire_series(self, exposure_time, image_interval, N_frames, label, subdir, trigger_direction):
+    def acquire_series(self, exposure_time, image_interval, N_frames, label, subdir):
         pass
     def save_images(images, label, metadata, savedir):
         pass
     def set_saving_directory(self, saving_directory):
         pass
     def set_binning(self, binning):
-        pass
+        self.settings['binning'] = binning
+    def set_roi(self, x,y,w,h):
+        self.settings['roi'] = [x,y,w,h]
+    def set_save_stack(self, boolean):
+        self.settings['save-stack'] = boolean
+
     def save_description(self, filename, string):
         pass
     def close(self):
         pass
+    def get_cameras(self):
+        return ['dummy1', 'dummy2']
+    def get_camera(self):
+        return self.camera
+    def set_camera(self, name):
+        self.camera = name
+    def get_settings(self):
+        return list(self.settings.keys())
+    def get_setting_type(self, setting_name):
+        if setting_name == 'setting1':
+            return 'string'
+        elif setting_name == 'setting2':
+            return 'float'
+        elif setting_name == 'setting3':
+            return 'integer'
+        else:
+            print('Invalid setting')
+            return ''
+    def get_setting(self, setting_name):
+        value = self.settings.get(setting_name, None)
+        if value is None:
+            return ''
+        return value
+    def set_setting(self, setting_name, value):
+        self.settings[setting_name] = value
 
 
-class Camera:
-    '''
-    Controlling ORCA FLASH 4.0 camera using Micro-Manager's
-    Python (2) bindings.
+
+class MMCamera:
+    '''Controls any camera using MicroManager and its pymmcore bindings.
     '''
 
     def __init__(self, saving_directory=DEFAULT_SAVING_DIRECTORY):
 
         self.set_saving_directory(saving_directory)
         
-        self.mmc = MMCorePy.CMMCore() 
-        self.mmc.loadDevice('Camera', 'HamamatsuHam', 'HamamatsuHam_DCAM')
-        self.mmc.initializeAllDevices()
-        self.mmc.setCameraDevice('Camera')
+        self.mmc = pymmcore.CMMCore() 
+        self.mmc.setDeviceAdapterSearchPaths([DEFAULT_MICROMANAGER_DIR])
+
+        self._device_name = None
+        self._configuration_name = ''
+
+        #self.mmc.loadDevice('Camera', 'HamamatsuHam', 'HamamatsuHam_DCAM')
+        #self.mmc.initializeAllDevices()
+        #self.mmc.setCameraDevice('Camera')
             
-        self.settings = {'binning': '1x1'}
+        self.settings = {'exposure_time_scaler': 1}
         
-        self.mmc.prepareSequenceAcquisition('Camera')
         #self.mmc.setCircularBufferMemoryFootprint(4000)
         self.live_queue= False
 
         self.shower = ImageShower()
 
         # Description file string
         self.description_string = ''
 
         self.save_stack = False
 
+        self.title = 'Camera not set'
+        self.servertitle = ''
 
 
-    def acquire_single(self, save, subdir):
+    def get_cameras(self):
+        '''Lists available MicroManager configuration files in .
+        '''
+        return [fn for fn in os.listdir(DEFAULT_MICROMANAGER_DIR) if fn.endswith('.cfg')]
+
+
+    def get_camera(self):
+        '''Returns the label of the current camera.
+        '''
+        return self._configuration_name
+
+    def set_camera(self, name):
+        '''Set the provided configuration file.
+        '''
+        if not os.path.exists(name):
+            path = os.path.join(DEFAULT_MICROMANAGER_DIR, name)
+            
+            if not os.path.exists(path):
+                print(f'Couldnt open configuration file named: {path}')
+                return
+
+        self.mmc.loadSystemConfiguration(path)
+        
+        self._device_name = self.mmc.getCameraDevice()
+        self._configuration_name = name
+        self.mmc.prepareSequenceAcquisition(self._device_name)
+
+        self.title = f'{name} ({self._device_name}) | {self.servertitle}'
+
+    def get_settings(self):
+        '''Returns device property names
+        '''
+        if self._device_name is None:
+            return ''
+        properties = self.mmc.getDevicePropertyNames(self._device_name)
+        
+        return list(properties) + list(self.settings.keys())
+
+
+    def get_setting_type(self, setting_name):
+        '''Returns "string", "integer" or "float".
+
+        Returns an empty string if the setting does not exist.
+        '''
+        if setting_name in self.settings:
+            return 'float'
+
+        try:
+            num = self.mmc.getPropertyType(self._device_name, setting_name)
+        except RuntimeError as e:
+            print(f'Error! No setting named: {setting_name}')
+            return ''
+        
+        if num == 1:
+            return 'string'
+        elif num == 2:
+            return 'float'
+        elif num == 3:
+            return 'integer'
+
+
+    def get_setting(self, setting_name):
+        if setting_name in self.settings:
+            return self.settings[setting_name]
+        return self.mmc.getProperty(self._device_name, setting_name)
+
+    def set_setting(self, setting_name, value):
+        
+        # a) Internal setting
+        if setting_name in self.settings:
+            self.settings[setting_name] = value
+            return
+        
+        # b) Camera device setting
+        type_name = self.get_setting_type(setting_name)
+        if type_name == 'float':
+            value = float(value)
+        elif type_name == 'integer':
+            value = int(value)
+        elif type_name == '':
+            print('Error! No setting named: {setting_name}')
+            return
+
+        print(f'Changing {setting_name} to its new value {value}')
+        try:
+            self.mmc.setProperty(self._device_name, setting_name, value)
+        except RuntimeError as e:
+            print('Error! The set value likely out of range.')
+            print(e)
+
+    def acquire_single(self, exposure_time, save, subdir):
         '''
         Acquire a single image.
 
         save        'True' or 'False'
         subdir      Subdirectory for saving
         '''
         
-        exposure_time = 0.01
-        binning = '2x2'
-
-        self.set_binning(binning)
+        exposure_time = float(exposure_time)
         self.mmc.setExposure(exposure_time*1000)
+        #binning = '2x2'
+
+        #self.set_binning(binning)
 
         start_time = str(datetime.datetime.now())
  
         self.mmc.snapImage()
         image = self.mmc.getImage()
         
         if not self.live_queue:
             self.live_queue = multiprocessing.Queue()
-            self.live_queue.put(image)
+            self.live_queue.put(
+                    image[0::LIVE_DOWNSAMPLE, 0::LIVE_DOWNSAMPLE])
             
-            self.livep = multiprocessing.Process(target=self.shower.loop, args=(self.live_queue,))
+            self.livep = multiprocessing.Process(
+                    target=self.shower.loop,
+                    args=(self.live_queue,self.title))
             self.livep.start()
             
-        self.live_queue.put(image)
+        self.live_queue.put(image[0::LIVE_DOWNSAMPLE, 0::LIVE_DOWNSAMPLE])
 
         if save == 'True':
-            metadata = {'exposure_time_s': exposure_time, 'binning': binning, 'function': 'acquireSingle', 'start_time': start_time}
+            metadata = {'exposure_time_s': exposure_time, 'function': 'acquireSingle', 'start_time': start_time}
 
             save_thread = threading.Thread(target=self.save_images,args=([image],'snap_{}'.format(start_time.replace(':','.').replace(' ','_')), metadata,os.path.join(self.saving_directory, subdir)))
             save_thread.start()
 
 
 
-    def acquire_series(self, exposure_time, image_interval, N_frames, label, subdir, trigger_direction):
+    def acquire_series(self, exposure_time, image_interval, N_frames, label, subdir):
         '''
         Acquire a series of images
 
         exposure_time       How many seconds to expose each image
         image_interval      How many seconds to wait in between the exposures
         N_frames            How many images to take
         label               Label for saving the images (part of the filename later)
         subdir
-        trigger_direction   "send" (camera sends a trigger pulse when it's ready) or "receive" (camera takes an image for every trigger pulse)
         '''
 
         exposure_time = float(exposure_time)
         image_interval = float(image_interval)
         N_frames = int(N_frames)
         label = str(label)
 
-        print "Now aquire_series with label " + label
-        print "- IMAGING PARAMETERS -"
-        print " exposure time " + str(exposure_time) + " seconds"
-        print " image interval " + str(image_interval) + " seconds"
-        print " N_frames " + str(N_frames)
-        print "- CAMERA SETTINGS"
-
-        self.set_binning('2x2')
-        print " Pixel binning 2x2"
-
-        if trigger_direction == 'send':
-            print " Camera sending a trigger pulse"
-            self.mmc.setProperty('Camera', "OUTPUT TRIGGER KIND[0]","EXPOSURE")
-            self.mmc.setProperty('Camera', "OUTPUT TRIGGER POLARITY[0]","NEGATIVE")
-        elif trigger_direction== 'receive':
-            print " Camera recieving / waiting for a trigger pulse"
-            self.mmc.setProperty('Camera', "TRIGGER SOURCE","EXTERNAL")
-            self.mmc.setProperty('Camera', "TriggerPolarity","POSITIVE")
-        else:
-            raise ValueError('trigger_direction has to be {} or {}, not {}'.format('receive', 'send', trigger_direction))
-
-        
-        print "Circular buffer " + str(self.mmc.getCircularBufferMemoryFootprint()) + " MB"
-
-        self.mmc.setExposure(exposure_time*1000)
-
+        print("Now aquire_series with label " + label)
+        print("- IMAGING PARAMETERS -")
+        print(" exposure time " + str(exposure_time) + " seconds")
+        print(" image interval " + str(image_interval) + " seconds")
+        print(" N_frames " + str(N_frames))
+        print("- CAMERA SETTINGS")
+
+        #self.set_binning('2x2')
+        #print(" Pixel binning 2x2")
+        
+        device_name = self.mmc.getDeviceName(self._device_name)
+        print(f'Device name {device_name}')
+
+        #if 'hamamatsu' in device_name.lower():
+        #    if trigger_direction == 'send':
+        #        print(" Camera sending a trigger pulse")
+        #        self.mmc.setProperty(self._device_name, "OUTPUT TRIGGER KIND[0]","EXPOSURE")
+        #        self.mmc.setProperty(self._device_name, "OUTPUT TRIGGER POLARITY[0]","NEGATIVE")
+        #    elif trigger_direction== 'receive':
+        #        print(" Camera recieving / waiting for a trigger pulse")
+        #        self.mmc.setProperty(self._device_name, "TRIGGER SOURCE","EXTERNAL")
+        #        self.mmc.setProperty(self._device_name, "TriggerPolarity","POSITIVE")
+        #    elif trigger_direction == 'none':
+        #        pass
+        #    else:
+        #        raise ValueError('trigger_direction has to be send, receive or none, not {trigger_direction}')
+
+        
+        print("Circular buffer " + str(self.mmc.getCircularBufferMemoryFootprint()) + " MB")
+
+        scaler = float(self.settings['exposure_time_scaler'])
+        exposure = scaler*exposure_time*1000
+        self.mmc.setExposure(exposure)
 
+        self.mmc.clearCircularBuffer()
+        #self.mmc.prepareSequenceAcquisition(self._device_name)
         self.wait_for_client()
         
-
         start_time = str(datetime.datetime.now())
-        self.mmc.startSequenceAcquisition(N_frames, image_interval, False)
-        
+        self.mmc.startSequenceAcquisition(N_frames, image_interval+(1-scaler)*exposure, False)
         
         while self.mmc.isSequenceRunning():
-            time.sleep(exposure_time)
+            self.mmc.sleep(1000*exposure_time)
+
+        self.mmc.sleep(1000)
 
         images = []
 
         for i in range(N_frames):
             while True:
                 try:
                     image = self.mmc.popNextImage()
                     break
-                except MMCorePy.CMMError:
-                    time.sleep(exposure_time)
-                
+                except:
+                    # Index error for example when circular buffer is still empty
+                    self.mmc.sleep(1000*exposure_time)
+            
             images.append(image)
             
             
         metadata = {'exposure_time_s': exposure_time, 'image_interval_s': image_interval,
                     'N_frames': N_frames, 'label': label, 'function': 'acquireSeries', 'start_time': start_time}
         metadata.update(self.settings)
 
         save_thread = threading.Thread(target=self.save_images, args=(images,label,metadata,os.path.join(self.saving_directory, subdir)))
         save_thread.start()
         
-        self.mmc.setProperty('Camera', "TRIGGER SOURCE","INTERNAL")
+        #if 'hamamatsu' in device_name.lower() and trigger_direction == 'receive':
+        #    self.mmc.setProperty(self._device_name, "TRIGGER SOURCE","INTERNAL")
+        
         print('acquired')
 
     
     def save_images(self, images, label, metadata, savedir):
         '''
         Save given images as grayscale tiff images.
         '''
         if not os.path.isdir(savedir):
-            os.makedirs(savedir)
+            try:
+                os.makedirs(savedir)
+            except:
+                # May fail if many local servers creating
+                # the folders simultaneously
+                pass
 
         if self.save_stack == False:
             # Save separate images
             for i, image in enumerate(images):
                 fn = '{}_{}.tiff'.format(label, i)
-                tifffile.imsave(os.path.join(savedir, fn), image, metadata=metadata)
+                tifffile.imwrite(os.path.join(savedir, fn), image, metadata=metadata)
         else:
             # Save a stack
             fn = '{}_stack.tiff'.format(label)
-            tifffile.imsave(os.path.join(savedir, fn), np.asarray(images), metadata=metadata)
+            tifffile.imwrite(os.path.join(savedir, fn), np.asarray(images), metadata=metadata)
         
         self.save_description(os.path.join(savedir, 'description'), self.description_string, internal=True)
 
 
     def set_saving_directory(self, saving_directory):
         '''
         Sets where the specimen folders are saved and if the directory
         does not yet exist, creates it.
         '''
-        saving_directory = os.path.join(SAVING_DRIVE, saving_directory)
         if not os.path.isdir(saving_directory):
             os.makedirs(saving_directory)
             
         self.saving_directory = saving_directory
 
 
     def set_save_stack(self, boolean):
@@ -359,15 +526,15 @@
             print("Did not understand wheter to save stacks. Given {}".format(boolean))
 
     def set_binning(self, binning):
         '''
         Binning '2x2' for example.
         '''
         if not self.settings['binning'] == binning:
-            self.mmc.setProperty('Camera', 'Binning', binning)
+            self.mmc.setProperty(self._device_name, 'Binning', binning)
             self.settings['binning'] =  binning
 
     def set_roi(self, x,y,w,h):
         '''
         In binned pixels
         roi     (x,y,w,h) or None
         '''
@@ -396,130 +563,201 @@
         if internal:
             fn = specimen_name
         else:
             fn = os.path.join(self.saving_directory, specimen_name, specimen_name)
         
         # Check if the folder exists
         if not os.path.exists(os.path.dirname(fn)):
-            #raise OSError('File {} already exsits'.format(fn))
-            os.makedirs(os.path.dirname(fn))
+            try:
+                os.makedirs(os.path.dirname(fn), exist_ok=True)
+            except:
+                # My fail if many local servers. Let's not
+                # care about it, another server has made it
+                pass
         
-        with open(fn+'.txt', 'w') as fp:
-            fp.write(desc_string)
+        try:
+            with open(fn+'.txt', 'w') as fp:
+                fp.write(desc_string)
 
-        print "Wrote file " + fn+'.txt'
-        
+            print("Wrote file " + fn+'.txt') 
+        except:
+            pass
         
         self.description_string = desc_string
 
 
     def close(self):
-        self.live_queue.put('close')
-        self.lifep.join()
+        if self.live_queue:
+            self.live_queue.put('close')
 
     def wait_for_client(self):
         pass
 
 
 class CameraServer:
+    '''Camera server listens incoming connections from the client and
+    controls a camera class.
     '''
-    Camera server listens incoming connections and
-    controls the camera through Camera class
-    '''
-    def __init__(self):
 
-        PORT = cac.PORT
+    def __init__(self, camera, port=None):
+        
+        if port is None:
+            port = PORT
         HOST = ''           # This is not cac.SERVER_HOSTNAME, leave empty
 
         self.running = False
 
+        print(f'Binding a socket (host {HOST}, port {port}))')
+
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket.bind((HOST, PORT))
+        self.socket.bind((HOST, port))
         self.socket.listen(1)
-
-        try:
-            self.cam = Camera()
-            self.cam.wait_for_client = self.wait_for_client
-        except Exception as e:
-            print e
-            print "Using DUMMY camera instead"
-            self.cam = DummyCamera()
+        
+        print(f'Using the camera <{camera.__class__.__name__}>')
+        self.cam = camera
+        self.cam.servertitle = f'Server on port {port}'
+        self.cam.wait_for_client = self.wait_for_client
         
         self.functions = {'acquireSeries': self.cam.acquire_series,
                           'setSavingDirectory': self.cam.set_saving_directory,
                           'acquireSingle': self.cam.acquire_single,
                           'saveDescription': self.cam.save_description,
                           'set_roi': self.cam.set_roi,
                           'set_save_stack': self.cam.set_save_stack,
+                          'get_cameras': self.cam.get_cameras,
+                          'get_camera': self.cam.get_camera,
+                          'set_camera': self.cam.set_camera,
+                          'get_settings': self.cam.get_settings,
+                          'get_setting_type': self.cam.get_setting_type,
+                          'get_setting': self.cam.get_setting,
+                          'set_setting': self.cam.set_setting,
                           'ping': self.ping,
                           'exit': self.stop}
 
-    def ping(self, message):
-        print message
+        self.responding = set([
+            'get_cameras', 'get_camera', 'get_settings', 'get_setting_type', 'get_setting'])
 
 
+    def ping(self, message):
+        print(message)
+
 
     def wait_for_client(self):
-        '''
-        Waits until client confirms that it is ready
+        '''Waits until client confirms that it is ready by sending us
+        anything (usually ping).
         '''
         conn, addr = self.socket.accept()
         string = ''
         while True:
             data = conn.recv(1024)
             if not data: break
-            string += data
+            string += data.decode()
         conn.close()
-        print "Client ready"
+        print("Client ready")
         
 
-
     def run(self):
         '''
         Loop waiting for incoming connections.
         Each established connection can give one command and then the connection
         is closed.
         '''
+        
+        print('Waiting for clients to connect')
+
         self.running = True
         while self.running:
             conn, addr = self.socket.accept()
             string = ''
             while True:
                 data = conn.recv(1024)
-                if not data: break
-                string += data
+                #if not data: break
+                string += data.decode()
+                break
+
+            if not string:
+                conn.close()
+                continue
             
-            conn.close()
             print('Recieved command "'+string+'" at time '+str(time.time()))
-            if string:
+            if ';' in string:
                 func, parameters = string.split(';')
                 parameters = parameters.split(':')
-                target=self.functions[func](*parameters)
+            else:
+                func = string
+                parameters = None
+        
+            # Can close connection early, no response so let's not delay the client
+            if not func in self.responding:
+                conn.close()
             
+            if parameters:
+                response = self.functions[func](*parameters)
+            else:
+                response = self.functions[func]()
+
+            # Say back the response and close because still open
+            if func in self.responding:
+                
+                if isinstance(response, (list, tuple)):
+                    response = ':'.join(response)
+
+                conn.sendall(str(response).encode())
+                conn.close()
+
+
     def stop(self, placeholder):
         '''
         Stop running the camera server.
         '''
-        self.camera.close()
+        self.cam.close()
         self.running = False
 
 
 def test_camera():
     cam = Camera()
     images = cam.acquireSeries(0.01, 1, 5, 'testing')
     
     for image in images:
         plt.imshow(image, cmap='gray')
         plt.show()
 
 
 
-def run_server():
-    '''
-    Running the server.
-    '''
-    cam_server = CameraServer()
+def main():
+    
+    parser = argparse.ArgumentParser(
+            prog='GonioImsoft Camera Server',
+            description='Controls a MicroManager camera')
+
+    parser.add_argument('-p', '--port')
+    parser.add_argument('-c', '--camera')
+    parser.add_argument('-s', '--save-directory')
+
+    args = parser.parse_args()
+
+
+    if args.camera == 'mm':
+        Camera = MMCamera
+    elif args.camera == 'dummy':
+        Camera = DummyCamera
+    else:
+        # Default
+        if pymmcore:
+            Camera = MMCamera
+        else:
+            Camera = DummyCamera
+
+    camera = Camera()
+
+    if args.save_directory:
+        camera.set_saving_directory(args.save_directory)
+
+    if args.port:
+        args.port = int(args.port)
+
+    cam_server = CameraServer(camera, args.port)
     cam_server.run()
             
         
 if __name__ == "__main__":
-    run_server()
+    main()
```

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/core.py` & `gonio-imsoft-0.1.0/gonioimsoft/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-'''
-Pupil Imsoft's core module; Classes for static and dynamic imaging
+'''GonioImsoft main components.
 '''
 
 import os
 import sys
 import time
 import datetime
 import copy
@@ -14,80 +13,117 @@
     import nidaqmx
 except ModuleNotFoundError:
     nidaqmx = None
 
 from gonioimsoft.anglepairs import saveAnglePairs, loadAnglePairs, toDegrees
 from gonioimsoft.arduino_serial import ArduinoReader
 from gonioimsoft.camera_client import CameraClient
-from gonioimsoft.camera_communication import SAVING_DRIVE
 from gonioimsoft.motors import Motor
 from gonioimsoft.imaging_parameters import (
         DEFAULT_DYNAMIC_PARAMETERS,
         load_parameters,
         getModifiedParameters)
 from gonioimsoft.stimulus import StimulusBuilder
 import gonioimsoft.macro as macro
 
+ENABLE_MOTORS = False
 
+class GonioImsoftCore:
+    '''Main interface to control GonioImsoft recordings.
 
-class Dynamic:
-    '''
-    Dynamic imaging procedure.
+    Attributes
+    ----------
+    reader : obj
+        Reading rotary encoder values from the Arduino Board.
+    cameras : list
+        Lis of camera client objects
     '''
 
 
     def __init__(self, dynamic_parameters=DEFAULT_DYNAMIC_PARAMETERS):
         '''
         Sets up ArduinoReader, CameraClient/Server.
         '''
 
         # Angle pairs reader (rotary encoder values)
         self.reader = ArduinoReader()
         
         # Initiate camera client/server
-        self.camera = CameraClient()
-        if not self.camera.isServerRunning():
-            print('Camera server not running')
-        #    self.camera.startServer()
+        self.cameras = []
         
         # Details about preparation (name, sex, age) are saved in this
         self.preparation = {'name': 'test', 'sex': '', 'age': ''}
 
         self.dynamic_parameters = dynamic_parameters
-        self.locked_parameters = {}
 
         self.previous_angle = None
 
         # Suffix to be appended in the subfolders, see set_subfolder_suffix method
         self.suffix = ''
 
         # Set up motors followingly
         # 0)    Horizontal + sensor
         # 1)    Vertical + sensor
         # 2)    Microscope focus (no sensor)
         self.motors = []
-        for i_motor, i_sensor in zip([0,1,2],[0,1,None]):
-            self.motors.append(Motor(self.reader, i_motor, i_sensor))
+        if ENABLE_MOTORS:
+            for i_motor, i_sensor in zip([0,1,2],[0,1,None]):
+                self.motors.append(Motor(self.reader, i_motor, i_sensor))
         
 
         # Macro imaging: Automatically move motors and take images
         # self macro is a list of anglepairs where to move the horizontal/vertical,
         # take image "commands" (string 'image') and other functions.
         # For more details see the tick method of this class.
         self.macro = None
         self.i_macro = 0
         self.waittime = 0
 
         self.trigger_rotation = False
 
-        self.trigger_signal = np.array([5,5,5,0])
+        self.trigger_signal = np.array([3,3,3,0])
         self.triggered_anglepairs = None
 
         self.data_savedir = None
+
+        self.local_servers_running_index = 0
+
+    
+    def add_camera_client(self, host, port):
+        '''Adds a camera client to the given host and port.
+
+        If host is None uses the localhost and starts a local
+        server if no local server running at that port
+        '''
+        client = CameraClient(
+                host, port,
+                running_index=self.local_servers_running_index)
+        self.local_servers_running_index += 1
+
+        if host is None and not client.is_server_running():
+            client.start_server()
+
+        self.cameras.append(client)
+
+        return client
+
+    def remove_camera_client(self, i_client):
+        '''Removes the camera client and closes its server if local server
+        '''
+        # Popping is enough and the client should be garbage collected
+        # by Python (the sockets are not kept alive so nothing is
+        # left open etc. by the client)
+        client = self.cameras.pop(i_client)
         
+        # If the client started a local server, close the server
+        if client.local_server is not None:
+            client.close_server()
+
+        return client
+
 
     def analog_output(self, channels, stimuli, fs, wait_trigger, camera=True):
         '''
 
         channels    List of channel names
         stimuli     List of 1D numpy arrays
         fs          Sampling frequency of the stimuli
@@ -125,24 +161,31 @@
             if wait_trigger:
                 task.triggers.start_trigger.cfg_dig_edge_start_trig("/Dev1/PFI0", trigger_edge=nidaqmx.constants.Edge.RISING)
 
             
             task.start()
 
             if camera:
-                self.camera.sendCommand('ready')
+                for camera in self.cameras:
+                    camera.sendCommand('ready')
                 
             task.wait_until_done(timeout=(len(stimuli[0])/fs)*1.5+20)
 
 
     def send_trigger(self):
         '''
         Sending trigger.
         '''
+
         chan = self.dynamic_parameters.get('trigger_out_channel', None)
+        
+        if nidaqmx is None:
+            print(f'    pretending to send trigger on chan {chan}')
+            return None
+
         if chan:
             with nidaqmx.Task() as task:
                 task.ao_channels.add_ao_voltage_chan(chan)
                 task.timing.cfg_samp_clk_timing(1000., samps_per_chan=4)
                 task.write(self.trigger_signal)
                 task.start()
                 task.wait_until_done(timeout=1.)
@@ -155,14 +198,18 @@
     def set_led(self, device, value, wait_trigger=False):
         '''
         Set an output channel to a specific voltage value.
 
         INPUT ARGUMENTS     DESCRIPTION
         device              A string (single device) or a list of strings (many devices at once)
         '''
+        if nidaqmx is None:
+            print(f'    pretending to set {device} on value {value}')
+            return None
+
         with nidaqmx.Task() as task:
             
             if type(device) == type('string'):
                 # If there's only a single device
                 task.ao_channels.add_ao_voltage_chan(device)
             else:
                 # If device is actually a list of devices
@@ -177,14 +224,18 @@
             
 
 
     def wait_for_trigger(self):
         '''
         Doesn't return until trigger signal is received.
         '''
+        if nidaqmx is None:
+            print(f'    waiting for trigger')
+            return None
+
         with nidaqmx.Task() as task:
             device = nidaqmx.system.device.Device('Dev1')
             
             task.ai_channels.add_ai_voltage_chan('Dev1/ai0' )
             
             task.timing.cfg_samp_clk_timing(10000)
             
@@ -202,29 +253,30 @@
         Takes a snap image.
         
         save        Whether to save the image directly or not.
         '''
         if save:
             self.set_led(self.dynamic_parameters['ir_channel'], self.dynamic_parameters['ir_imaging'])
             time.sleep(0.3)
-            self.camera.acquireSingle(True, os.path.join(self.preparation['name'], 'snaps'))
+            for camera in self.cameras:
+                camera.acquireSingle(True, os.path.join(self.preparation['name'], 'snaps'))
             self.set_led(self.dynamic_parameters['ir_channel'], self.dynamic_parameters['ir_livefeed'])
             time.sleep(0.2)
 
             print('A snap image taken')
         else:
-            self.camera.acquireSingle(False, '')
+            for camera in self.cameras:
+                camera.acquireSingle(False, '')
             time.sleep(0.1)
 
 
 
     
     def image_trigger_softhard(self):
-        '''
-        For dynamic imaging of pseudopupil movements.
+        '''Software triggering of the cameras.
 
         How this works?
         CameraClient (self.camera) send message to CameraServer to start image acquisition. Starting
         image acquistion takes some time, so to synchronize, we wait a trigger signal from the camera
         before turning the LED on. What is done is essentially half software half hardware triggering.
         Not ideal but seems to work.
         '''
@@ -320,15 +372,16 @@
             
             elif len(dynamic_parameters[param]) != int(dynamic_parameters['repeats']):
                 print('Warning! Dynamic parameter {} length is {} but repeats is set to {}'.format(param,
                     len(dynamic_parameters[param]), dynamic_parameters['repeats'] ))
                 dynamic_parameters[param] = [dynamic_parameters[param][0]] * dynamic_parameters['repeats'] 
 
         # Set stack save option
-        self.camera.set_save_stack(dynamic_parameters.get('save_stack', False))
+        for camera in self.cameras:
+            camera.set_save_stack(dynamic_parameters.get('save_stack', False))
         
 
         # Get the current rotation stage angles and use this through the repeating
         # (even if it would change during imaging)
         imaging_angle = self.reader.get_latest()
         
         # Prepare some variables that stay constant over imaging
@@ -361,14 +414,21 @@
 
             if i==0 and dynamic_parameters['avgint_adaptation']:
                 self.set_led(dynamic_parameters['flash_channel'], np.mean(builder.get_stimulus_pulse()))
                 time.sleep(dynamic_parameters['avgint_adaptation'])
             
             imaging_function(dynamic_parameters, builder, label, N_frames, image_directory, set_led=bool(dynamic_parameters['isi'][i]))
 
+            # Dirtyfix
+            if dynamic_parameters['reboot_cameras']:
+                print("Rebooting cameras")
+                for i_camera, camera in enumerate(self.cameras):
+                    print(f'  cam_{i_camera}...')
+                    camera.reboot()
+
             # Wait the total imaging period; If ISI is short and imaging period is long, we would
             # start the second imaging even before the camera is ready
             # Better would be wait everything clear signal from the camera.
             #total_imaging_time = dynamic_parameters['pre_stim'] + dynamic_parameters['stim'] + dynamic_parameters['post_stim']
             #print("Total imaging time " + str(total_imaging_time))
             # Do the actual waiting together with ISI, see just below
             
@@ -406,36 +466,60 @@
         if set_led:
             self.set_led(dynamic_parameters['ir_channel'], dynamic_parameters['ir_imaging'])
             time.sleep(0.5)
         
         fs = builder.fs
           
         stimulus = builder.get_stimulus_pulse()
+        if isinstance(stimulus, list):
+            NN = len(stimulus[0])
+        else:
+            NN = stimulus.shape
+        irwave = dynamic_parameters['ir_imaging'] * np.ones(NN)
 
-        irwave = dynamic_parameters['ir_imaging'] * np.ones(stimulus.shape)
+        #irwave = dynamic_parameters['ir_imaging'] * np.ones(stimulus.shape)
         if set_led:
             irwave[-1] = dynamic_parameters['ir_waiting']
 
+        stimuli = []
+        channels = []
+
+        if isinstance(stimulus, list):
+            # Many stimulus channels
+            print('Many stimulus channels')
+            stimuli = [*stimulus, irwave]
+            channels = [*dynamic_parameters['flash_channel'], dynamic_parameters['ir_channel']]
+        else:
+            # One stimulus channel
+            stimuli = [stimulus, irwave]
+            channels = [dynamic_parameters['flash_channel'], dynamic_parameters['ir_channel']]
 
-        self.camera.acquireSeries(dynamic_parameters['frame_length'], 0, N_frames, label, image_directory, 'send')
 
-        self.analog_output([dynamic_parameters['flash_channel'], dynamic_parameters['ir_channel']], [stimulus,irwave], fs, wait_trigger=True)
+        if len(self.cameras) == 1:
+            self.cameras[0].acquireSeries(dynamic_parameters['frame_length'], 0, N_frames, label, image_directory)
+        elif len(self.cameras) > 1:
+            # With many cameras, add camN suffix to the label
+            for i_camera, camera in enumerate(self.cameras):
+                camera.acquireSeries(dynamic_parameters['frame_length'], 0, N_frames, f'{label}_cam{i_camera}', image_directory)
+
+        self.analog_output(channels, stimuli, fs, wait_trigger=True)
 
         
 
 
     def set_savedir(self, savedir, camera=True):
         '''
         Set the directory where the taken images are saved.
 
         camera : bool
             If False, do not attempt to update save folder to the camera server
         '''
         if camera:
-            self.camera.setSavingDirectory(savedir)
+            for camera in self.cameras:
+                camera.setSavingDirectory(savedir)
         self.data_savedir = savedir
 
 
     def set_subfolder_suffix(self, suffix):
         '''
         Set any suffix to a data folder containing the images.
         For example
@@ -448,57 +532,66 @@
 
     def _update_descriptions_file(self):
         # Saving description file
         desc_string = "name {}\nsex {}\nage {}".format(self.preparation['name'], self.preparation['sex'], self.preparation['age'])
         desc_string += "\n\n#DYNAMIC PROTOCOL PARAMETERS\n"
         for name, value in self.dynamic_parameters.items():
             desc_string += '{} {}\n'.format(name, value)
-        print(desc_string)
-        self.camera.saveDescription(self.preparation['name'], desc_string)
+        for camera in self.cameras:
+            camera.saveDescription(self.preparation['name'], desc_string)
         
 
     def initialize(self, name, sex, age, camera=False):
-        '''
-        Call this to initialize the experiments.
+        '''Call this to initialize the experiments.
+
+        Returns True if worked or None if user cancelled.
+
 
         name, sex age       Can be '' (empty string)
         '''
         # Preparations, ask droso name
         if name != '':
             self.preparation['name'] = name
         if sex != '':
             self.preparation['sex'] = sex
         if age != '':
             self.preparation['age'] = age
 
-        self.dynamic_parameters = getModifiedParameters(
-                locked_parameters=self.locked_parameters)
-        print('Preparation name set as {}, sex {}, age {} days.'.format(self.preparation['name'], self.preparation['sex'], self.preparation['age']))
+        params = getModifiedParameters()
+        if params is None:
+            return None 
+
+        self.dynamic_parameters = params
 
         if camera:
             self._update_descriptions_file()
         else:
             self.triggered_anglepairs = []
         
         self.set_led(self.dynamic_parameters['ir_channel'], self.dynamic_parameters['ir_livefeed'])
         self.set_led(self.dynamic_parameters['flash_channel'], self.dynamic_parameters['flash_off'])
+       
+        roi = self.dynamic_parameters['ROI']
+        if roi is not None:
+            for camera in self.cameras:
+                camera.set_roi(roi)
 
+        return True
 
     def load_preset(self, preset_name):
         fn = os.path.join('presets', preset_name)
-        self.dynamic_parameters = {**load_parameters(fn), **self.locked_parameters}
+        self.dynamic_parameters = load_parameters(fn)
         self._update_descriptions_file()
 
 
 
     def tick(self, horizontal_trigger=True, vertical_trigger=False):
-        '''
-        Updates the current angle. In the future may do other houskeeping functions also.
+        '''Updates the current angle and performs all "houskeeping" duties also.
         
-        Call this once while in a loop that the angles have to be updated.
+        Meant to be called repeatedly inside the UI loop.
         '''
 
         change = False
         
         while True:
             
             # Update current angle and echo it to the console
@@ -527,15 +620,15 @@
 
             action = self.macro[self.i_macro]
             print(action)
 
             
             if type(action) == type((0,0)):
                 # Move motors only if they have reached their positions
-                if all([self.motors[i].reached_target() for i in [0,1]]):
+                if self.motors and all([self.motors[i].reached_target() for i in [0,1]]):
                     self.motors[0].move_to(action[0])
                     self.motors[1].move_to(action[1])
                     next_macro_step = True
             if 'wait' in action:
                 self.waittime = time.time() + float(action.split(' ')[-1])
                 next_macro_step = True
             
@@ -556,33 +649,34 @@
 
     def finalize(self):
         '''
         Finalising the experiments, houskeeping stuff.
         '''
         self.set_led(self.dynamic_parameters['ir_channel'], 0)
         self.set_led(self.dynamic_parameters['flash_channel'], 0)
-
+        
         for motor in self.motors:
             motor.move_to(0)
 
         if self.triggered_anglepairs:
-            fn = os.path.join(SAVING_DRIVE, self.data_savedir, self.preparation['name'], 'anglepairs.txt')
+            fn = os.path.join(self.data_savedir, self.preparation['name'], 'anglepairs.txt')
             os.makedirs(os.path.dirname(fn), exist_ok=True)
 
             print(fn)
             
             with open(fn, 'w') as fp:
                 for line in self.triggered_anglepairs:
                     fp.write(str(line).strip('()').replace(' ', '')+'\n')
 
             self.triggered_anglepairs = None
 
 
     def exit(self):
-        self.camera.close_server()
+        for camera in self.cameras:
+            camera.close_server()
 
     #
     # CONTROLLING LEDS, MOTORS ETC
     #
     
     def move_motor(*args, **kwargs):
         self.reader.move_motor(*args, **kwargs)
```

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/imaging_parameters.py` & `gonio-imsoft-0.1.0/gonioimsoft/imaging_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,73 @@
-'''
-Default dynamic parameters and ParameterEditor for letting the user
+'''Settting and getting imaging parameters.
+
+Default imaging parameters, and ParameterEditor for letting the user
 modify them in the program.
 '''
+
 import os
 import time
 import ast
 import json
 
-from gonioimsoft.directories import PUPILDIR
+from gonioimsoft.directories import USERDATA_DIR
 
 
-DEFAULT_DYNAMIC_PARAMETERS = {'isi': 10.0, 'repeats': 1, 'pre_stim': 0.000,
+DEFAULT_DYNAMIC_PARAMETERS = {
+        'isi': 10.0, 'repeats': 1, 'pre_stim': 0.000,
         'stim': 0.200, 'post_stim': 0.00, 'frame_length' : 0.010,
         'ir_imaging': 5, 'ir_waiting': 0, 'ir_livefeed': 1,
-        'flash_on': 8, 'flash_off': 0,
+        'flash_on': 5, 'flash_off': 0,
         'ir_channel': "Dev1/ao1", 'flash_channel': "Dev1/ao0",
         'suffix': '', 'trigger_channel': "/Dev1/PFI0",
         'trigger_out_channel': "Dev2/ao0",
         'biosyst_stimulus': '',
         'biosyst_channel': 2,
         'avgint_adaptation': 0,
         'flash_type': 'square',
-        'save_stack': False}
+        'save_stack': True,
+        'reboot_cameras': False,
+        'ROI': None,
+        }
 
-DYNAMIC_PARAMETERS_TYPES = {'seconds': ['isi', 'pre_stim', 'stim', 'post_stim', 'frame_length', 'avgint_adaptation'],
+DYNAMIC_PARAMETERS_TYPES = {
+        'seconds': ['isi', 'pre_stim', 'stim', 'post_stim', 'frame_length', 'avgint_adaptation'],
         'voltage': ['ir_imaging', 'ir_waiting', 'ir_livefeed', 'flash_on', 'flash_off'],
         'channel': ['ir_channel', 'flash_channel', 'trigger_channel', 'trigger_out_channel'],
         'integer': ['repeats', 'biosyst_channel'],
         'string': ['suffix', 'biosyst_stimulus', 'flash_type'],
-        'boolean': ['save_stack']}
+        'boolean': ['save_stack', 'reboot_cameras'],
+        'roibox': ['ROI']}
 
 
-DYNAMIC_PARAMETERS_HELP = {'isi': 'Inter stimulus intervali[s]',
-        'repeats': 'How many times the protocol is repeated',
+DYNAMIC_PARAMETERS_HELP = {
+        'isi': 'Inter stimulus interval [s]',
+        'repeats': 'How many times the protocol is repeated [1-inf]',
         'pre_stim': 'How long to image before the pulse [s]',
         'stim': 'Stimulus (step pulse) length [s]',
         'post_stim': 'How long to image after the pulse [s]',
-        'frame_length': 'Exposure time / inter-frame interval',
-        'ir_imaging': 'IR brightness during image acqusition',
-        'ir_waiting': 'IR brightness when waiting ISI',
-        'ir_livefeed': 'IR brightness while updating the live image',
-        'flash_on': 'Flash brightness during stim',
-        'flash_off':' Flash brightness during image acqustition',
-        'ir_channel': 'NI channel for IR',
+        'frame_length': 'Exposure time / inter-frame interval [s]',
+        'ir_imaging': 'IR brightness during image acqusition [0-10]',
+        'ir_waiting': 'IR brightness when waiting ISI [0-10]',
+        'ir_livefeed': 'IR brightness while updating the live image[0-10]',
+        'flash_on': 'Flash brightness during stim [0-10]',
+        'flash_off': 'Flash brightness during pre- and post-stim [0-10]',
+        'ir_channel': 'NI channel for IR [0-10]',
         'flash_channel': 'NI channel for Flash',
-        'trigger_channel': 'Trigger recieve/in channel',
-        'trigger_out_channel': 'Trigger send/out channel',
+        'trigger_channel': 'Trigger recieve/in channel for NI',
+        'trigger_out_channel': 'Trigger send/out channel from NI',
         'suffix': 'Tag added to the saved folders',
-        'biosyst_stimulus': 'Override the square pulse by a biosyst stimulus',
-        'biosyst_channel': 'Channel of the biosyst simulus',
+        'biosyst_stimulus': 'Override the square pulse by a biosyst stimulus [filename]',
+        'biosyst_channel': 'The channel read from the biosyst simulus file if set',
         'avgint_adaptation': 'Time to show stimulus mean value before imaging [s]',
-        'flash_type': '"square" or sinelogsweep',
-        'save_stack': 'If true, save stack instead separate images'}
+        'flash_type': 'square, sinelogsweep, squarelogsweep or 3steplogsweep. "{sweep},f0,f1" for Hz',
+        'save_stack': 'If true, save a stack instead separate images',
+        'reboot_cameras': 'If true, reboots cameras after each run (dirtyfix)',
+        'ROI': 'If set, crops the sensor area (allows higher fps). x,y,w,h',
+        }
 
 
 def getRightType(parameter_name, string_value):
     '''
     Convert user inputted string to correct parameter value based on
     DYNAMIC_PARAMETER_TYPES
 
@@ -89,15 +101,15 @@
             voltage = float(string_value)
             if not -10<=voltage<=10:
                 raise ValueError('Voltage value range -10 to 10 V exceeded.')
             return voltage
 
     if parameter_name in  DYNAMIC_PARAMETERS_TYPES['channel']:
         if type(string_value) == type(''):
-            if string_value.startswith('[') and string_value.endswith([']']):
+            if string_value.startswith('[') and string_value.endswith(']'):
                 return ast.literal_eval(string_value)
             else:
                 return string_value
     
     if parameter_name in DYNAMIC_PARAMETERS_TYPES['string']:
         return str(string_value)
 
@@ -105,14 +117,22 @@
         if string_value.lower() == 'true':
             return True
         elif string_value.lower() == 'false':
             return False
         else:
             raise ValueError('Boolean falue has to be either "True" or "False"')
 
+
+    if parameter_name in DYNAMIC_PARAMETERS_TYPES['roibox']:
+        try:
+            x,y,w,h = [int(num) for num in string_value.split(',')]
+            return (x,y,w,h)
+        except:
+            return None
+
     raise NotImplementedError('Add {} correctly to DYNAMIC_PARAMETER_TYPES in dynamic_parameters.py')
 
 
 
 def load_parameters(fn):
     '''
     Loading imaging parameters, saved as a json file.
@@ -131,26 +151,24 @@
 
 
 
 class ParameterEditor:
     '''
     Dictionary editor on command line with ability to load and save presets.
     '''
-    def __init__(self, dynamic_parameters, locked_parameters={}):
+    def __init__(self, dynamic_parameters):
         '''
         dynamic_parameters      Dictionary of the dynamic imaging parameters.
         '''
         self.dynamic_parameters = dynamic_parameters
         self.parameter_names = sorted(self.dynamic_parameters.keys())
 
-        self.presets_savedir = os.path.join(PUPILDIR, 'presets')
+        self.presets_savedir = os.path.join(USERDATA_DIR, 'presets')
         self.presets = self.load_presets(self.presets_savedir)
 
-        self.locked_parameters = locked_parameters
-
     
     def load_presets(self, directory):
         
         presets = {}
         
         if os.path.isdir(directory):
             files = [os.path.join(directory, fn) for fn in os.listdir(directory)]
@@ -181,33 +199,40 @@
                  
         parameter_names = sorted(self.dynamic_parameters.keys())
 
         print()
         
         print('{:<20} {:<40} {}'.format('PARAMETER NAME', 'VALUE', 'DESCRIPTION'))
         for parameter in parameter_names:
-            if parameter in self.locked_parameters:
-                lck = ' (LOCKED to {})'.format(self.locked_parameters[parameter])
-            else:
-                lck = ''
-            print('{:<20} {:<40} {}'.format(parameter, str(preset[parameter])+lck,
-                DYNAMIC_PARAMETERS_HELP[parameter]))
+
+            value = str(preset[parameter])
+
+            # Special addition for frame_length parameter; Show Hz so that
+            # it is harder to do mistakes
+            if parameter == 'frame_length':
+                hz = str(round(1/float(value)))
+                if hz == 1:
+                    hz = str(1/float(value))
+                value += ' ({} Hz)'.format(hz)
+
+            print('{:<20} {:<40} {}'.format(
+                parameter, value, DYNAMIC_PARAMETERS_HELP[parameter]))
         print()
 
 
     def getModified(self):
         '''
         Ask user to edit the parameters until happy and then return
         the parameters.
         '''
         
         while True:
             print('MODIFYING IMAGING PARAMETERS')
             self.print_preset(self.dynamic_parameters)
-            parameter = input('Parameter name or (list/save/load) (Enter to continue) >> ')
+            parameter = input('Parameter name or (list/save/load/back) (Enter to continue) >> ')
             
             # If breaking free
             if parameter == '':
                 break
             
 
             self.presets = self.load_presets(self.presets_savedir)
@@ -215,19 +240,19 @@
             
             # If saving preset
             if parameter.lower() == 'save':
                 name = input('Save current parameters under preset name (if empty == suffix) >> ')
                 if name == '' and self.dynamic_parameters['suffix'] != '':
                     name = self.dynamic_parameters['suffix']
                 
-                if os.path.isdir(PUPILDIR):
+                if os.path.isdir(USERDATA_DIR):
                     os.makedirs(self.presets_savedir, exist_ok=True)
                     save_parameters(os.path.join(self.presets_savedir, name), self.dynamic_parameters)
                 else:
-                    print('Saving the preset failed, {} does not exist'.format(PUPILDIR))
+                    print('Saving the preset failed, {} does not exist'.format(USERDATA_DIR))
 
                 continue        
 
             if parameter.lower() == 'list':
                 if self.presets is {}:
                     print('There are no existing presets!')
                 else:
@@ -253,14 +278,17 @@
                         to_load = preset_names[int(sel)-1]
                         break
                     except:
                         print('Invalid preset.')
 
                 parameter = to_load
 
+            if parameter == 'back':
+                return None
+
             if parameter in self.presets.keys():
                 self.print_preset(self.presets[parameter])
                 
                 confirm = input('Load this (y/n)>> ').lower()
                 if confirm and confirm[0] == 'y':
                     self.dynamic_parameters = self.presets[parameter]
                 else:
@@ -289,15 +317,15 @@
                     print(str(e))
                     print('Could not convert the value to right type. Try againg or Enter to skip.')
                     continue
 
                 self.dynamic_parameters[parameter] = value
                 break
 
-        return {**self.dynamic_parameters, **self.locked_parameters}
+        return self.dynamic_parameters
 
 
 def getModifiedParameters(**kwargs):
     '''
     Take in the DEFAULT parameters in the beginning of this code file
     and let the user modify them using text based ParameterEditor
     '''
```

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/macro.py` & `gonio-imsoft-0.1.0/gonioimsoft/macro.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 import os
 import ast
 
+from .directories import USERDATA_DIR
+
 def list_macros():
     '''
     Lists all available macros by names that can be
     directly passed to load function in this module.
     '''
 
     return [fn[:-4] for fn in os.listdir('macros') if fn.endswith('.txt')]
@@ -19,15 +21,16 @@
 
     Loaded macro that is returned is a list whose items
     are macro commands understood by DynamicImaging in core.py
     '''
 
     macro = []
 
-    with open(os.path.join('macros', macro_name+'.txt'), 'r') as fp:
+    with open(os.path.join(
+        USERDATA_DIR, 'macros', macro_name+'.txt'), 'r') as fp:
         for line in fp:
             if line:
                 macro.append(ast.literal_eval(line))
     
     return macro
 
 def save(macro_name, macro):
```

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/motors.py` & `gonio-imsoft-0.1.0/gonioimsoft/motors.py`

 * *Files identical despite different names*

### Comparing `gonio-imsoft-0.0.2/gonioimsoft/stimulus.py` & `gonio-imsoft-0.1.0/gonioimsoft/stimulus.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 
 import os
 
 import numpy as np
-import scipy.signal
+import json
 
-from biosystfiles import extract as bsextract
+try:
+    import scipy.signal
+except ModuleNotFoundError:
+    scipy = None
+
+try:
+    from biosystfiles import extract as bsextract
+except ModuleNotFoundError:
+    bsextract = None
+
+from .directories import USERDATA_DIR
 
 class StimulusBuilder:
     '''
     Get various stimulus waveforms
     - to the stimulus LED
     - and on pulse for illumination LED
     - and square wave for triggering the camera.
@@ -43,23 +53,42 @@
             self.wtype = wtype
 
             self.N_frames = int(round((stim_time+prestim_time+poststim_time)/frame_length))
 
             self.overload_stimulus = None
             
 
-
     def overload_biosyst_stimulus(self, fn, channel=0):
         '''
         Loads a Biosyst stimulus that gets returned then at
         get_stimulus_pulse instead.
 
         Returns the overload stimulus and new fs
         '''
-        ffn = os.path.join('biosyst_stimuli', fn)
+        
+        if fn.endswith('.json'):
+            ffn = os.path.join(USERDATA_DIR, 'biosyst_stimuli', fn)
+            with open(fnn, 'r') as fp:
+                data = json.load(fp)
+
+            self.fs = data['fs']
+            self.overload_stimulus = []
+
+            for i_stim in range(10):
+                key = f'stim_{i_stim}'
+                if key not in data:
+                    continue
+                self.overload_stimulus.append(np.array(data[key]))
+
+            return self.overload_stimulus[0], self.fs
+
+        if bsextract is None:
+            raise ModuleNotFoundError('Module required\npip install python-biosystfiles')
+
+        ffn = os.path.join(USERDATA_DIR, 'biosyst_stimuli', fn)
         self.overload_stimulus, self.fs = bsextract(ffn, channel)
         self.overload_stimulus = self.overload_stimulus.flatten()
         print(self.overload_stimulus.shape)
         print(np.max(self.overload_stimulus))
 
         return self.overload_stimulus, self.fs
     
@@ -150,7 +179,54 @@
         
         camera = np.concatenate( ( np.ones((samples_per_frame, self.N_frames)), np.zeros((samples_per_frame, self.N_frames)) ) ).T.flatten()
         camera = 5*camera
     
         camera[-1] = 0
 
         return camera
+
+
+
+def main():
+    '''Saves stimulus as a json.
+    '''
+    from .imaging_parameters import getModifiedParameters
+
+    data = {}
+    for i_stim in range(10):
+
+        dynamic_parameters = getModifiedParameters()
+
+        fs = 10000
+        builder = StimulusBuilder(
+                dynamic_parameters['stim'],
+                dynamic_parameters['pre_stim'],
+                dynamic_parameters['post_stim'],
+                dynamic_parameters['frame_length'],
+                dynamic_parameters['flash_on'],
+                dynamic_parameters['ir_imaging'],
+                fs,
+                stimulus_finalval=dynamic_parameters['flash_off'],
+                illumination_finalval=dynamic_parameters['ir_waiting'],
+                wtype=dynamic_parameters['flash_type'])
+
+        if dynamic_parameters.get('biosyst_stimulus', ''):
+            bsstim, fs = builder.overload_biosyst_stimulus(
+                    dynamic_parameters['biosyst_stimulus'], dynamic_parameters['biosyst_channel'])
+            #N_frames = int(round((len(bsstim)/fs) / dynamic_parameters['frame_length']))
+
+        stimulus = builder.get_stimulus_pulse().tolist()
+
+        data['fs'] = fs
+        data[f'stim_{i_stim}'] = stimulus
+
+        cont = input('Add more (y/n)')
+
+        if cont.lower().startswith('n'):
+            break
+
+    with open('test.json', 'w') as fp:
+        json.dump(data, fp)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `gonio-imsoft-0.0.2/setup.py` & `gonio-imsoft-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 # Version number to __version__ variable
 exec(open("gonioimsoft/version.py").read())
 
 install_requires = [
         'numpy',
         'matplotlib',
         'tifffile',
+        'pymmcore',
         'nidaqmx',
         'pyserial',
         'python-biosystfiles',
         ]
 
 setuptools.setup(
     name="gonio-imsoft",
     version=__version__,
     author="Joni Kemppainen",
-    author_email="jjtkemppainen1@sheffield.ac.uk",
+    author_email="joni.kemppainen@windowslive.com",
     description="Goniometric imaging software",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jkemppainen/gonio-imsoft",
     packages=setuptools.find_packages(),
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3) ",
         "Operating System :: Microsoft :: Windows",
         'Intended Audience :: Science/Research',
         "Environment :: Console",
     ],
-    python_requires='>=3.0',
+    python_requires='>=3.6',
 )
```

