# Comparing `tmp/codex-engine-pyqt-0.0.9.tar.gz` & `tmp/codex-engine-pyqt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codex-engine-pyqt-0.0.9.tar", last modified: Mon Apr 26 01:51:55 2021, max compression
+gzip compressed data, was "codex-engine-pyqt-0.1.0.tar", last modified: Wed Aug  2 04:29:07 2023, max compression
```

## Comparing `codex-engine-pyqt-0.0.9.tar` & `codex-engine-pyqt-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-04-26 01:51:55.071673 codex-engine-pyqt-0.0.9/
--rw-rw-rw-   0        0        0     1090 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1331 2021-04-26 01:51:55.071673 codex-engine-pyqt-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      423 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2021-04-26 01:51:54.999718 codex-engine-pyqt-0.0.9/codex/
--rw-rw-rw-   0        0        0      519 2021-04-26 01:46:03.000000 codex-engine-pyqt-0.0.9/codex/__init__.py
--rw-rw-rw-   0        0        0     5156 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/bundles.py
--rw-rw-rw-   0        0        0      340 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/console_device.py
--rw-rw-rw-   0        0        0    10411 2021-04-26 01:46:42.000000 codex-engine-pyqt-0.0.9/codex/device_controls.py
--rw-rw-rw-   0        0        0     5395 2021-04-26 01:47:36.000000 codex-engine-pyqt-0.0.9/codex/device_manager.py
--rw-rw-rw-   0        0        0      797 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/dummy_serial.py
-drwxrwxrwx   0        0        0        0 2021-04-26 01:51:55.008712 codex-engine-pyqt-0.0.9/codex/filters/
--rw-rw-rw-   0        0        0      162 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/filters/__init__.py
--rw-rw-rw-   0        0        0      697 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/filters/delimiter_filter.py
--rw-rw-rw-   0        0        0      811 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/filters/judi_filter.py
--rw-rw-rw-   0        0        0      358 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/filters/newline_filter.py
--rw-rw-rw-   0        0        0      300 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/filters/null_filter.py
--rw-rw-rw-   0        0        0     1105 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/judi_mixin.py
--rw-rw-rw-   0        0        0      627 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/judi_responder.py
--rw-rw-rw-   0        0        0      999 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/remote_serial.py
--rw-rw-rw-   0        0        0     3550 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/serial_device.py
--rw-rw-rw-   0        0        0     5462 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/serial_device_base.py
--rw-rw-rw-   0        0        0     4405 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/subscriptions.py
--rw-rw-rw-   0        0        0     3230 2021-04-26 01:44:11.000000 codex-engine-pyqt-0.0.9/codex/unknown_device.py
-drwxrwxrwx   0        0        0        0 2021-04-26 01:51:55.069674 codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/
--rw-rw-rw-   0        0        0     1331 2021-04-26 01:51:54.000000 codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2021-04-26 01:51:54.000000 codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-26 01:51:54.000000 codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-04-26 01:51:54.000000 codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-04-26 01:51:54.000000 codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2021-04-26 01:51:55.073671 codex-engine-pyqt-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1203 2021-04-26 01:49:45.000000 codex-engine-pyqt-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.302837 codex-engine-pyqt-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1385 2023-08-02 04:29:07.302837 codex-engine-pyqt-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.246340 codex-engine-pyqt-0.1.0/codex/
+-rw-rw-rw-   0        0        0      519 2023-08-02 03:15:29.000000 codex-engine-pyqt-0.1.0/codex/__init__.py
+-rw-rw-rw-   0        0        0     5156 2021-03-25 16:06:34.000000 codex-engine-pyqt-0.1.0/codex/bundles.py
+-rw-rw-rw-   0        0        0      340 2021-03-25 16:06:34.000000 codex-engine-pyqt-0.1.0/codex/console_device.py
+-rw-rw-rw-   0        0        0    10489 2023-03-03 07:13:57.000000 codex-engine-pyqt-0.1.0/codex/device_controls.py
+-rw-rw-rw-   0        0        0     5451 2023-04-20 02:44:02.000000 codex-engine-pyqt-0.1.0/codex/device_manager.py
+-rw-rw-rw-   0        0        0      797 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/codex/dummy_serial.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.255840 codex-engine-pyqt-0.1.0/codex/filters/
+-rw-rw-rw-   0        0        0      162 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/__init__.py
+-rw-rw-rw-   0        0        0      697 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/delimiter_filter.py
+-rw-rw-rw-   0        0        0      811 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/judi_filter.py
+-rw-rw-rw-   0        0        0      358 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/newline_filter.py
+-rw-rw-rw-   0        0        0      300 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/null_filter.py
+-rw-rw-rw-   0        0        0     1105 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/judi_mixin.py
+-rw-rw-rw-   0        0        0      627 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/codex/judi_responder.py
+-rw-rw-rw-   0        0        0      980 2023-08-02 04:22:47.000000 codex-engine-pyqt-0.1.0/codex/local_serial.py
+-rw-rw-rw-   0        0        0     1032 2022-05-01 00:26:31.000000 codex-engine-pyqt-0.1.0/codex/remote_serial.py
+-rw-rw-rw-   0        0        0     3550 2023-08-02 03:15:29.000000 codex-engine-pyqt-0.1.0/codex/serial_device.py
+-rw-rw-rw-   0        0        0     5543 2023-08-02 04:25:14.000000 codex-engine-pyqt-0.1.0/codex/serial_device_base.py
+-rw-rw-rw-   0        0        0     4405 2021-03-25 16:06:34.000000 codex-engine-pyqt-0.1.0/codex/subscriptions.py
+-rw-rw-rw-   0        0        0     3236 2022-12-09 04:35:48.000000 codex-engine-pyqt-0.1.0/codex/unknown_device.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.301338 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/
+-rw-rw-rw-   0        0        0     1385 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-09 04:36:59.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1151 2023-08-02 04:29:07.304840 codex-engine-pyqt-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-12-09 04:23:09.000000 codex-engine-pyqt-0.1.0/setup.py
```

### Comparing `codex-engine-pyqt-0.0.9/LICENSE` & `codex-engine-pyqt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/PKG-INFO` & `codex-engine-pyqt-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: codex-engine-pyqt
-Version: 0.0.9
+Version: 0.1.0
 Summary: A universal translator for serial devices.
 Home-page: https://github.com/Codex-Engine/codex-engine-pyqt
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
-License: UNKNOWN
-Description: # Codex Engine for PyQt
-        
-        A universal translator for serial devices.
-        
-        # Description
-        
-        This is the reference implementation of Codex, a framework for managing serial communication with physical devices. 
-        
-        # Features
-        - serial port detection
-        - automatic handshaking
-        - device profiles as drop-in plugins
-        - supports many styles of serial communication
-        - extensible
-        
-        ## Requirements
-        - pyserial
-        - PyQt5 or PySide2
-        
-Keywords: codex,codex engine,serial
-Platform: any
+License: MIT
+Project-URL: Source, https://github.com/Codex-Engine/codex-engine-pyqt
+Project-URL: Tracker, https://github.com/Codex-Engine/codex-engine-pyqt/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Widget Sets
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+# Codex Engine for PyQt
+
+A universal translator for serial devices.
+
+# Description
+
+This is the reference implementation of Codex, a framework for managing serial communication with physical devices. 
+
+# Features
+- serial port detection
+- automatic handshaking
+- device profiles as drop-in plugins
+- supports many styles of serial communication
+- extensible
+
+## Requirements
+- pyserial
+- PyQt5 or PySide2
```

### Comparing `codex-engine-pyqt-0.0.9/codex/__init__.py` & `codex-engine-pyqt-0.1.0/codex/__init__.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/bundles.py` & `codex-engine-pyqt-0.1.0/codex/bundles.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/device_controls.py` & `codex-engine-pyqt-0.1.0/codex/device_controls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from qtstrap import *
 from codex import DeviceManager
 from serial.tools.list_ports import comports
 
 try:
     from serial_monitor import SerialMonitorWidget
+
     serial_monitor_available = True
 except:
     serial_monitor_available = False
 
 try:
-    from command_palette import CommandPalette, Command
+    from qtstrap.extras.command_palette import CommandPalette, Command
+
     command_palette_available = True
 except:
     command_palette_available = False
 
 
 class DeviceTreeWidgetItem(QTreeWidgetItem):
     def __init__(self, parent, device):
         super().__init__(parent)
 
         self.device = device
         self.guid = device.guid
-        
+
         self.setText(0, device.profile_name)
 
         parts = device.port.split('link?')
         port = device.port if (len(parts) == 1) else parts[1]
 
         self.setText(1, port)
 
@@ -39,23 +41,23 @@
     def __init__(self, parent=None):
         super().__init__(parent)
         self.setUniformRowHeights(True)
         self.setExpandsOnDoubleClick(False)
         self.setItemsExpandable(False)
         self.setSelectionMode(QAbstractItemView.NoSelection)
         self.setColumnCount(2)
-        self.setColumnWidth(0,150)
+        self.setColumnWidth(0, 150)
         self.setHeaderLabels(['Name', 'Port'])
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
 
         self.nodes = {}
         self.local_device_root = QTreeWidgetItem(self)
-        self.local_device_root.setText(0, "Local Devices")
+        self.local_device_root.setText(0, 'Local Devices')
         self.remote_device_root = QTreeWidgetItem(self)
-        self.remote_device_root.setText(0, "Remote Devices")
+        self.remote_device_root.setText(0, 'Remote Devices')
 
         self.open_monitors = {}
 
     def device_added(self, device):
         if device.port[:5] == 'ws://':
             parent = self.remote_device_root
         else:
@@ -86,28 +88,28 @@
             menu = QMenu()
             menu.addAction(QAction('Add device', self))
             menu.addAction(QAction('Configure', self))
             menu.exec_(pos)
 
         if hasattr(item, 'device'):
             menu = QMenu()
-            
+
             if hasattr(item.device, 'settings'):
-                menu.addAction(QAction("Settings", self, triggered=lambda: self.open_settings(item)))
+                menu.addAction(QAction('Settings', self, triggered=lambda: self.open_settings(item)))
 
             if hasattr(item.device, 'widget'):
-                menu.addAction(QAction("Open Device Controls", self, triggered=lambda: self.open_widget(item)))
+                menu.addAction(QAction('Open Device Controls', self, triggered=lambda: self.open_widget(item)))
 
             if hasattr(item.device, 'locate'):
-                menu.addAction(QAction("Locate Device", self, triggered=item.device.locate))
+                menu.addAction(QAction('Locate Device', self, triggered=item.device.locate))
 
             if serial_monitor_available:
-                menu.addAction(QAction("Open Serial Monitor", self, triggered=lambda: self.open_monitor(item)))
-                menu.addAction(QAction("Open Serial Port", self, triggered=lambda: self.open_serial_port(item)))
-            menu.addAction(QAction("Remove", self, triggered=lambda: self.remove_clicked(item)))
+                menu.addAction(QAction('Open Serial Monitor', self, triggered=lambda: self.open_monitor(item)))
+                menu.addAction(QAction('Open Serial Port', self, triggered=lambda: self.open_serial_port(item)))
+            menu.addAction(QAction('Remove', self, triggered=lambda: self.remove_clicked(item)))
             menu.exec_(pos)
 
     def open_settings(self, item):
         if hasattr(item, 'device'):
             if hasattr(item.device, 'widget'):
                 print('settings:', item.device.profile_name)
 
@@ -144,23 +146,23 @@
         super().__init__(parent)
         self.title = QLabel(title)
         self.list = QListWidget()
         self.line = QLineEdit(self)
         self.line.returnPressed.connect(self.on_add)
         self.add = QPushButton('Add', clicked=self.on_add)
 
-        with CVBoxLayout(self, margins=(0,0,0,0)) as layout:
-            with layout.hbox(margins=(0,0,0,0)) as layout:
+        with CVBoxLayout(self, margins=(0, 0, 0, 0)) as layout:
+            with layout.hbox(margins=(0, 0, 0, 0)) as layout:
                 layout.add(self.title)
-            with layout.hbox(margins=(0,0,0,0)) as layout:
+            with layout.hbox(margins=(0, 0, 0, 0)) as layout:
                 layout.add(self.line, 1)
                 layout.add(self.add)
             layout.add(self.list)
 
-    def contextMenuEvent(self, event: PySide2.QtGui.QContextMenuEvent) -> None:
+    def contextMenuEvent(self, event: QtGui.QContextMenuEvent) -> None:
         pos = event.globalPos()
         item = self.list.itemAt(self.list.viewport().mapFromGlobal(pos))
         index = self.list.indexFromItem(item).row()
 
         menu = QMenu()
         menu.addAction(QAction('Remove', self, triggered=lambda: self.on_remove(index)))
         menu.exec_(pos)
@@ -197,15 +199,15 @@
         self.starting_devices.addItems(self.dm.starting_devices)
         self.starting_devices.list_changed.connect(self.dm.set_starting_devices)
 
         self.ignored_ports = CustomListWidget('Ignored Ports:')
         self.ignored_ports.addItems(self.dm.ignored_ports)
         self.ignored_ports.list_changed.connect(self.dm.set_ignored_ports)
 
-        with CVBoxLayout(self, margins=(0,0,0,0)) as layout:
+        with CVBoxLayout(self, margins=(0, 0, 0, 0)) as layout:
             layout.add(self.ignored_ports)
             layout.add(self.starting_devices)
 
 
 @DeviceManager.subscribe
 class NewDeviceWidget(QWidget):
     def __init__(self, parent=None):
@@ -213,35 +215,35 @@
 
         self.profile = QComboBox()
         self.port = QComboBox()
         self.add = QPushButton('Add Device', clicked=self.add_pressed)
 
         names = [p for p in DeviceManager.profile_names() if p != 'no profile']
         self.profile.addItems(names)
-        ports = ["DummyPort", *[port.device for port in sorted(comports())]]
+        ports = ['DummyPort', *[port.device for port in sorted(comports())]]
         self.port.addItems(ports)
 
-        with CVBoxLayout(self, margins=(0,0,0,0)) as layout:
+        with CVBoxLayout(self, margins=(0, 0, 0, 0)) as layout:
             # layout.add(QLabel('Add a device:'))
-            with layout.hbox(margins=(0,0,0,0)) as layout:
-                with layout.vbox(margins=(0,0,0,0)) as layout:
+            with layout.hbox(margins=(0, 0, 0, 0)) as layout:
+                with layout.vbox(margins=(0, 0, 0, 0)) as layout:
                     layout.add(QLabel('Profiles:'))
                     layout.add(QLabel('Ports:'))
-                with layout.vbox(margins=(0,0,0,0)) as layout:
-                    with layout.hbox(margins=(0,0,0,0)) as layout:
+                with layout.vbox(margins=(0, 0, 0, 0)) as layout:
+                    with layout.hbox(margins=(0, 0, 0, 0)) as layout:
                         layout.add(self.profile, 1)
-                    with layout.hbox(margins=(0,0,0,0)) as layout:
+                    with layout.hbox(margins=(0, 0, 0, 0)) as layout:
                         layout.add(self.port, 1)
                         layout.add(self.add)
 
     def add_pressed(self):
         profile = self.profile.currentText()
         port = self.port.currentText()
 
-        device = profiles[profile](port)
+        device = DeviceManager.profiles()[profile](port)
         self.signals.add_device.emit(device)
 
 
 class DeviceControlsWidget(QWidget):
     def __init__(self, parent=None):
         super().__init__(parent=parent)
 
@@ -250,30 +252,33 @@
             layout.add(NewDeviceWidget(self))
             layout.add(DeviceTree(self))
 
         settings = QWidget()
         with CVBoxLayout(settings) as layout:
             layout.add(DeviceManagerSettings(self))
 
-        tabs = {'Devices':tree, 'Settings':settings, }
+        tabs = {
+            'Devices': tree,
+            'Settings': settings,
+        }
         with CVBoxLayout(self) as layout:
             self.tabs = layout.add(PersistentTabWidget('device_control_tabs', tabs=tabs))
 
 
 class DeviceControlsDockWidget(QDockWidget):
     def __init__(self, parent=None):
         super().__init__('Device Controls', parent=parent)
         self.setObjectName('DeviceControls')
 
         self.setWidget(DeviceControlsWidget(self))
 
         if command_palette_available:
             self.commands = [
-                Command("Device List: Show device list", triggered=self.show, shortcut='Ctrl+D'),
-                Command("Device List: Hide device list", triggered=self.hide),
+                Command('Device List: Show device list', triggered=self.show, shortcut='Ctrl+D'),
+                Command('Device List: Hide device list', triggered=self.hide),
             ]
 
         self.setAllowedAreas(Qt.LeftDockWidgetArea | Qt.RightDockWidgetArea)
         self.setFeatures(QDockWidget.DockWidgetClosable | QDockWidget.DockWidgetMovable)
 
         self.starting_area = Qt.RightDockWidgetArea
 
@@ -281,8 +286,8 @@
             self.parent().addDockWidget(self.starting_area, self)
 
         self.closeEvent = lambda x: self.hide()
 
     def toggleViewAction(self):
         action = super().toggleViewAction()
         action.setShortcut('Ctrl+D')
-        return action
+        return action
```

### Comparing `codex-engine-pyqt-0.0.9/codex/device_manager.py` & `codex-engine-pyqt-0.1.0/codex/device_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
         self.devices = {}
         self.new_devices = []
         self.first_scan = True
         self.ports = []
 
         self.sub_manager = SubscriptionManager(self)
         
-        prev = QSettings().value('starting_devices', [])
+        prev = QSettings().value('codex/starting_devices', [])
         if isinstance(prev, str):
             prev = [prev]
         self.starting_devices = prev
 
-        prev = QSettings().value('ignored_ports', [])
+        prev = QSettings().value('codex/ignored_ports', [])
         if isinstance(prev, str):
             prev = [prev]
         self.ignored_ports = prev
 
         self.scan_timer = QTimer()
         self.scan_timer.timeout.connect(lambda: self.scan())
         self.scan_timer.start(250)
@@ -56,19 +56,19 @@
         
         self.sub_manager.check_for_new_subscribers()
 
         UnknownDevice.register_autodetect_info(self.profiles())
         
     def set_starting_devices(self, devices):
         self.starting_devices = devices
-        QSettings().setValue('starting_devices', devices)
+        QSettings().setValue('codex/starting_devices', devices)
 
     def set_ignored_ports(self, ports):
         self.ignored_ports = ports
-        QSettings().setValue('ignored_ports', ports)
+        QSettings().setValue('codex/ignored_ports', ports)
 
     def close(self):
         self.scan_timer.stop()
         self.update_timer.stop()
         for _, device in self.devices.items():
             device.close()
 
@@ -84,15 +84,15 @@
     def do_first_scan(self, new_ports):
         if self.starting_devices:
             for string in self.starting_devices:
                 parts = string.split(':')
                 profile = parts[0]
                 port = parts[1]
                 baud = parts[2] if len(parts) == 3 else None
-                if profile in profile_names:
+                if profile in DeviceManager.profile_names():
                     if port in new_ports or port == 'DummyPort':
                         if baud:
                             self.on_add_device(self.profiles()[profile](port=port, baud=baud))
                         else:
                             self.on_add_device(self.profiles()[profile](port=port))
                         if port != 'DummyPort':
                             self.ports.append(port)
@@ -128,15 +128,15 @@
 
             if device.state == DeviceStates.enumeration_failed:
                 self.log.debug(f"Enumeration failed on ({device.port})")
                 device.close()
                 self.new_devices.remove(device)
         
             elif device.state == DeviceStates.enumeration_succeeded:
-                if device.name in profile_names:
+                if device.name in DeviceManager.profile_names():
                     device.close()
                     new_device = self.profiles()[device.name](device=device)
 
                     self.log.debug(f"Enumeration succeeded on ({new_device.port})")
 
                     self.devices[new_device.guid] = new_device
                     self.new_devices.remove(device)
```

### Comparing `codex-engine-pyqt-0.0.9/codex/dummy_serial.py` & `codex-engine-pyqt-0.1.0/codex/dummy_serial.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/filters/delimiter_filter.py` & `codex-engine-pyqt-0.1.0/codex/filters/delimiter_filter.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/filters/judi_filter.py` & `codex-engine-pyqt-0.1.0/codex/filters/judi_filter.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/judi_mixin.py` & `codex-engine-pyqt-0.1.0/codex/judi_mixin.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/judi_responder.py` & `codex-engine-pyqt-0.1.0/codex/judi_responder.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/remote_serial.py` & `codex-engine-pyqt-0.1.0/codex/remote_serial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from qtstrap import *
+from qtpy.QtWebSockets import *
 
 
 class RemoteSerial:
     def __init__(self, port=None, timeout=0):
         self.port = port
         self.read_buffer = ""
```

### Comparing `codex-engine-pyqt-0.0.9/codex/serial_device.py` & `codex-engine-pyqt-0.1.0/codex/serial_device.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/serial_device_base.py` & `codex-engine-pyqt-0.1.0/codex/serial_device_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from queue import Queue
 from .filters import JudiFilter
-from serial import Serial, SerialException
+from serial import SerialException
 from serial.tools.list_ports_common import ListPortInfo
 from .dummy_serial import DummySerial
 from .remote_serial import RemoteSerial
+from .local_serial import LocalSerial
 import logging
 from qtstrap import *
 import time
 
 
 class Signals(QObject):
     data_received = Signal(str) # pre filter
     char_accepted = Signal(str) # passes filter
     char_rejected = Signal(str) # fails filter
     msg_completed = Signal(str) # complete message
 
 
 class SerialDeviceBase:
-    log = None
+    log: logging.Logger | None = None
 
     def __init__(self, port=None, baud=9600):
-        if self.log == None:
+        if self.log is None:
             self.log = logging.getLogger(__name__)
             
         self.base_signals = Signals()
 
         self.queue = Queue()
         self.filter = JudiFilter(self.base_signals.char_accepted.emit, self.base_signals.char_rejected.emit)
         self.active = False
@@ -53,33 +54,33 @@
 
     def connect_socket(self, socket):
         socket.textMessageReceived.connect(self.send)
 
         def send_text_message(s):
             try:
                 socket.sendTextMessage(s)
-            except ValueError as e:
+            except ValueError:
                 self.log.exception(f'{self.port}')
             
         self.base_signals.data_received.connect(lambda s: send_text_message(s))
 
-    def connect_stream(self, stream, type='completed'):
+    def connect_stream(self, stream, stream_type='completed'):
         """
         connect a stream monitor to this SerialDevice
         types: raw, accepted, rejected, completed
         """
         stream.tx.connect(self.send)
         types = {
             'raw': self.base_signals.data_received,
             'accepted': self.base_signals.char_accepted,
             'rejected': self.base_signals.char_rejected,
             'completed': self.base_signals.msg_completed,
         }
-        if type in types:
-            types[type].connect(stream.rx)
+        if stream_type in types:
+            types[stream_type].connect(stream.rx)
 
     def open(self):
         """
         Open the serial port and set the device to active.
 
         Some port names trigger special behavior.
         """
@@ -91,19 +92,19 @@
         if self.port.startswith("RemoteSerial"):
             self.port = 'ws://' + self.port[len("RemoteSerial:"):]
             self.ser = RemoteSerial(port=self.port)
             self.active = True
             return
 
         try:
-            self.ser = Serial(port=self.port, baudrate=self.baud, timeout=0, write_timeout=0)
+            self.ser = LocalSerial(port=self.port, baudrate=self.baud)
             self.active = True
-        except Exception as e:
+        except PermissionError:
             # TODO: bad exception handling, it's not always a permission error
-            self.log.exception("PermissionError" + str(e))
+            self.log.exception(f"failed to open serial port on {self.port}")
 
     def close(self):
         """ close the serial port and set the device to inactive """
         if not self.active:
             return
 
         self.filter.reset()
@@ -127,16 +128,16 @@
         if self.queue.empty():
             return
 
         if time_since(self.last_transmit_time) > self.transmit_rate_limit:
             try:
                 self.ser.write(self.queue.get().encode())
                 self.last_transmit_time = time.time()
-            except SerialException as e:
-                self.log.exception(e)
+            except SerialException:
+                self.log.exception('serial write failed')
 
     def receive(self, string):
         """ do something when a complete string is captured in self.communicate() """
         self.log.debug(f"RX: {string}")
         self.base_signals.msg_completed.emit(string)
 
     def check_incoming_data(self):
```

### Comparing `codex-engine-pyqt-0.0.9/codex/subscriptions.py` & `codex-engine-pyqt-0.1.0/codex/subscriptions.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.0.9/codex/unknown_device.py` & `codex-engine-pyqt-0.1.0/codex/unknown_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         super().__init__(*args, **kwargs)
         self.message_tree.merge(self.common_message_tree)
         self.filter = NullFilter()
 
         self.state = DeviceStates.enumeration_pending
         self.bauds = iter(self._bauds)
 
-        self.cache_name = f'autodetect_cache:{self.port}'
+        self.cache_name = f'codex/autodetect_cache:{self.port}'
         baud, name = QSettings().value(self.cache_name, (9600, ''))
 
         self.set_baud_rate(int(baud))
         
         if name in self.handshake_table[baud]:
             self.handshake_table[baud][name](self.send)
```

### Comparing `codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/PKG-INFO` & `codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: codex-engine-pyqt
-Version: 0.0.9
+Version: 0.1.0
 Summary: A universal translator for serial devices.
 Home-page: https://github.com/Codex-Engine/codex-engine-pyqt
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
-License: UNKNOWN
-Description: # Codex Engine for PyQt
-        
-        A universal translator for serial devices.
-        
-        # Description
-        
-        This is the reference implementation of Codex, a framework for managing serial communication with physical devices. 
-        
-        # Features
-        - serial port detection
-        - automatic handshaking
-        - device profiles as drop-in plugins
-        - supports many styles of serial communication
-        - extensible
-        
-        ## Requirements
-        - pyserial
-        - PyQt5 or PySide2
-        
-Keywords: codex,codex engine,serial
-Platform: any
+License: MIT
+Project-URL: Source, https://github.com/Codex-Engine/codex-engine-pyqt
+Project-URL: Tracker, https://github.com/Codex-Engine/codex-engine-pyqt/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Widget Sets
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+# Codex Engine for PyQt
+
+A universal translator for serial devices.
+
+# Description
+
+This is the reference implementation of Codex, a framework for managing serial communication with physical devices. 
+
+# Features
+- serial port detection
+- automatic handshaking
+- device profiles as drop-in plugins
+- supports many styles of serial communication
+- extensible
+
+## Requirements
+- pyserial
+- PyQt5 or PySide2
```

### Comparing `codex-engine-pyqt-0.0.9/codex_engine_pyqt.egg-info/SOURCES.txt` & `codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 codex/bundles.py
 codex/console_device.py
 codex/device_controls.py
 codex/device_manager.py
 codex/dummy_serial.py
 codex/judi_mixin.py
 codex/judi_responder.py
+codex/local_serial.py
 codex/remote_serial.py
 codex/serial_device.py
 codex/serial_device_base.py
 codex/subscriptions.py
 codex/unknown_device.py
 codex/filters/__init__.py
 codex/filters/delimiter_filter.py
 codex/filters/judi_filter.py
 codex/filters/newline_filter.py
 codex/filters/null_filter.py
 codex_engine_pyqt.egg-info/PKG-INFO
 codex_engine_pyqt.egg-info/SOURCES.txt
 codex_engine_pyqt.egg-info/dependency_links.txt
+codex_engine_pyqt.egg-info/not-zip-safe
 codex_engine_pyqt.egg-info/requires.txt
 codex_engine_pyqt.egg-info/top_level.txt
```

