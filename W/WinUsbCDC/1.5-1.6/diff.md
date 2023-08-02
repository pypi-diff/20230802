# Comparing `tmp/WinUsbCDC-1.5-py3-none-any.whl.zip` & `tmp/WinUsbCDC-1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18930 bytes, number of entries: 14
--rw-r--r--  2.0 unx      176 b- defN 22-Nov-06 06:36 winusbcdc/__init__.py
--rw-r--r--  2.0 unx     2909 b- defN 22-Nov-06 06:36 winusbcdc/__main__.py
--rw-r--r--  2.0 unx      148 b- defN 22-Nov-06 06:36 winusbcdc/__version__.py
--rw-r--r--  2.0 unx    13479 b- defN 22-Nov-06 06:36 winusbcdc/usb_cdc.py
--rw-r--r--  2.0 unx     2007 b- defN 22-Nov-06 06:36 winusbcdc/winusb.py
--rw-r--r--  2.0 unx     3485 b- defN 22-Nov-06 06:36 winusbcdc/winusbclasses.py
--rw-r--r--  2.0 unx      241 b- defN 22-Nov-06 06:36 winusbcdc/winusberror.py
--rw-r--r--  2.0 unx    14734 b- defN 22-Nov-06 06:36 winusbcdc/winusbpy.py
--rw-r--r--  2.0 unx    13569 b- defN 22-Nov-06 06:36 winusbcdc/winusbutils.py
--rw-rw-rw-  2.0 unx     1071 b- defN 22-Nov-06 06:36 WinUsbCDC-1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     6699 b- defN 22-Nov-06 06:36 WinUsbCDC-1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-06 06:36 WinUsbCDC-1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Nov-06 06:36 WinUsbCDC-1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1099 b- defN 22-Nov-06 06:36 WinUsbCDC-1.5.dist-info/RECORD
-14 files, 59719 bytes uncompressed, 17126 bytes compressed:  71.3%
+Zip file size: 18941 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      176 b- defN 23-Aug-02 12:13 winusbcdc/__init__.py
+-rw-r--r--  2.0 unx     2909 b- defN 23-Aug-02 12:13 winusbcdc/__main__.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Aug-02 12:13 winusbcdc/__version__.py
+-rw-r--r--  2.0 unx    13486 b- defN 23-Aug-02 12:13 winusbcdc/usb_cdc.py
+-rw-r--r--  2.0 unx     2007 b- defN 23-Aug-02 12:13 winusbcdc/winusb.py
+-rw-r--r--  2.0 unx     3485 b- defN 23-Aug-02 12:13 winusbcdc/winusbclasses.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Aug-02 12:13 winusbcdc/winusberror.py
+-rw-r--r--  2.0 unx    14744 b- defN 23-Aug-02 12:13 winusbcdc/winusbpy.py
+-rw-r--r--  2.0 unx    13569 b- defN 23-Aug-02 12:13 winusbcdc/winusbutils.py
+-rw-rw-rw-  2.0 unx     1071 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6699 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1099 b- defN 23-Aug-02 12:13 WinUsbCDC-1.6.dist-info/RECORD
+14 files, 59736 bytes uncompressed, 17137 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: winusbcdc/winusbpy.py
 Comment: 
 
 Filename: winusbcdc/winusbutils.py
 Comment: 
 
-Filename: WinUsbCDC-1.5.dist-info/LICENSE
+Filename: WinUsbCDC-1.6.dist-info/LICENSE
 Comment: 
 
-Filename: WinUsbCDC-1.5.dist-info/METADATA
+Filename: WinUsbCDC-1.6.dist-info/METADATA
 Comment: 
 
-Filename: WinUsbCDC-1.5.dist-info/WHEEL
+Filename: WinUsbCDC-1.6.dist-info/WHEEL
 Comment: 
 
-Filename: WinUsbCDC-1.5.dist-info/top_level.txt
+Filename: WinUsbCDC-1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: WinUsbCDC-1.5.dist-info/RECORD
+Filename: WinUsbCDC-1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## winusbcdc/__version__.py

```diff
@@ -1,7 +1,7 @@
 # Version managed by git-versioner
-version = "v1.5"
-version_short = "v1.5"
-git_hash = "5e90344"
-on_tag = "v1.5"
+version = "v1.6"
+version_short = "v1.6"
+git_hash = "74b0dac"
+on_tag = 'v1.6'
 dirty = False
 SUPPORT_PATCH = False
```

## winusbcdc/usb_cdc.py

```diff
@@ -91,40 +91,39 @@
         self.stopbits = 1
         self.databits = 8
         self.maximum_packet_size = 0
 
         self._timeout = 0
 
         self.is_open = False
+        self.device = self._select_device(self.name, self.vid, self.pid)
         if start:
             self.open()
 
     def open(self):
         # Control interface
-        api = self._select_device(self.name, self.vid, self.pid)
-        if not api:
+        if not self.device:
             return False
 
         # interface_descriptor = api.query_interface_settings(0)
         # pipe_info_list = map(api.query_pipe, range(interface_descriptor.b_num_endpoints))
 
         # Data Interface
-        api.change_interface(0)
-        interface2_descriptor = api.query_interface_settings(0)
+        self.device.change_interface(0)
+        interface2_descriptor = self.device.query_interface_settings(0)
 
-        pipe_info_list = map(api.query_pipe, range(interface2_descriptor.b_num_endpoints))
+        pipe_info_list = map(self.device.query_pipe, range(interface2_descriptor.b_num_endpoints))
         for item in pipe_info_list:
             if item.pipe_id & 0x80:
                 self._ep_in = item.pipe_id
             else:
                 self._ep_out = item.pipe_id
             self.maximum_packet_size = min(item.maximum_packet_size, self.maximum_packet_size) or item.maximum_packet_size
 
-        self.device = api  # type: WinUsbPy
-
+        self.name = self.device.name
         self.is_open = True
 
         self.setControlLineState(True, True)
         self.setLineCoding()
         self.device.set_timeout(self._ep_in, 2)
         self.reset_input_buffer()
 
@@ -360,17 +359,16 @@
     #     print("  {0} baud, parity mode {1}".format(self.baudrate, self.parity))
     #     print(
     #         "  {0} data bits, {1} stop bits".format(
     #             self.databits,
     #             self.stopbits))
 
     def disconnect(self):
-        if not self.is_open:
-            return None
-        self.device.close_winusb_device()
+        if self.device:
+            self.device.close_winusb_device()
         self.is_open = False
 
     def __del__(self):
         self.disconnect()
 
     def reset_input_buffer(self):
         if self.is_open:
```

## winusbcdc/winusbpy.py

```diff
@@ -107,37 +107,38 @@
                         ctypes.byref(buff_parent_path),
                         ctypes.sizeof(buff_parent_path) - 1,
                         0,
                     )
                     if not ret:
                         parent = buff_parent_path.value
 
+            # friendly name
+            uname = path
+            buff_friendly_name = ctypes.create_unicode_buffer(250)
+            if self.api.exec_function_setupapi(SetupDiGetDeviceRegistryProperty, self.handle,
+                                                byref(sp_device_info_data),
+                                                SPDRP_FRIENDLYNAME,
+                                                None,
+                                                ctypes.byref(buff_friendly_name),
+                                                ctypes.sizeof(buff_friendly_name) - 1,
+                                                None):
+
+                uname = buff_friendly_name.value
+            else:
+                err = self.get_last_error_code()
+                # print(ctypes.WinError())
+
+
             if vid is not None and pid is not None:
                 if is_device(name, vid, pid, path):
-                    self.device_paths.append(WinUsbPyDevice(path, path, parent))
+                    self.device_paths.append(WinUsbPyDevice(path, uname, parent))
                     return self.device_paths
             else:
-
-                # friendly name
-                uname = path
-                buff_friendly_name = ctypes.create_unicode_buffer(250)
-                if self.api.exec_function_setupapi(SetupDiGetDeviceRegistryProperty, self.handle,
-                                                   byref(sp_device_info_data),
-                                                   SPDRP_FRIENDLYNAME,
-                                                   None,
-                                                   ctypes.byref(buff_friendly_name),
-                                                   ctypes.sizeof(buff_friendly_name) - 1,
-                                                   None):
-
-                    uname = buff_friendly_name.value
-                else:
-                    err = self.get_last_error_code()
-                    # print(ctypes.WinError())
-                self.device_paths.append(WinUsbPyDevice(path, uname, parent))
                 if name is not None and uname == name:
+                    self.device_paths.append(WinUsbPyDevice(path, uname, parent))
                     return self.device_paths
             i += 1
             member_index = DWORD(i)
             required_size = c_ulong(0)
             resize(sp_device_interface_detail_data, sizeof(SpDeviceInterfaceDetailData))
         return self.device_paths
 
@@ -168,14 +169,15 @@
         self._pid = pid
         self._name = name
         path = None
         try:
             for d in self.device_paths:
                 if self.find_device(d.name) or self.find_device(d.path):
                     path = d.path
+                    self._name = self._name or d.name
                     break
 
         except IndexError:
             return False
 
         return self.init_winusb_device_with_path(path)
```

## Comparing `WinUsbCDC-1.5.dist-info/LICENSE` & `WinUsbCDC-1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `WinUsbCDC-1.5.dist-info/METADATA` & `WinUsbCDC-1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinUsbCDC
-Version: 1.5
+Version: 1.6
 Summary: Python package for communicating with USB / CDC devices on windows via the WinUsb driver
 Home-page: https://gitlab.com/alelec/winusbcdc
 Author: Andrew Leech
 Author-email: andrew@alelec.net
 License: MIT
 License-File: LICENSE
 
@@ -181,8 +181,8 @@
 Api <https://github.com/felHR85/WinUsbPy/blob/master/winusbpy/examples/winusbtest.py>`__
 
 `Using WinUsbPy High Level
 Api <https://github.com/felHR85/WinUsbPy/blob/master/winusbpy/examples/winusbtest2.py>`__
 
 
 
-version: 1.5
+version: 1.6
```

