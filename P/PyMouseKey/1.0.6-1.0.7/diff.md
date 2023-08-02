# Comparing `tmp/PyMouseKey-1.0.6-py3-none-any.whl.zip` & `tmp/PyMouseKey-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6505 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    20833 b- defN 23-Aug-01 08:47 pymousekey/__init__.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 23-Aug-01 08:49 PyMouseKey-1.0.6.dist-info/RECORD
-5 files, 21795 bytes uncompressed, 5779 bytes compressed:  73.5%
+Zip file size: 6506 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    20926 b- defN 23-Aug-02 18:32 pymousekey/__init__.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      389 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/RECORD
+5 files, 21888 bytes uncompressed, 5780 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pymousekey/__init__.py
 Comment: 
 
-Filename: PyMouseKey-1.0.6.dist-info/METADATA
+Filename: PyMouseKey-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: PyMouseKey-1.0.6.dist-info/WHEEL
+Filename: PyMouseKey-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: PyMouseKey-1.0.6.dist-info/top_level.txt
+Filename: PyMouseKey-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMouseKey-1.0.6.dist-info/RECORD
+Filename: PyMouseKey-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymousekey/__init__.py

```diff
@@ -441,28 +441,29 @@
 
     if _pause:
         time.sleep(PAUSE)
 
 
 def autoclick(button=LEFT):
     """
-    Starts a auto clicker at your mouse and clicks the specified button at 200cps\n
+    Starts a auto clicker in a seperate daemon thread at your current mouse location and clicks the specified button at roughly 200cps\n
     USE WITH CAUTION:
     -----
     Make sure you can call this function with a hotkey or another way because it will not automatically toggle off\n
-    If you dont have a way to call it again then you will have to restart your computer
 
     """
     global autoclickState
     autoclickState = not autoclickState
     def autoclick():
         while autoclickState:
             click(None, None, 0.004, 1, button, False)
     if autoclickState:
-        threading.Thread(target=autoclick).start()
+        autoclick_thread = threading.Thread(target=autoclick)
+        autoclick_thread.daemon = True
+        autoclick_thread.start()
 
 
 def doubleClick(x=None, y=None, interval=0.0, button=LEFT, _pause=True):
     click(x, y, interval, 2, button, _pause)
 
 def tripleClick(x=None, y=None, interval=0.0, button=LEFT, _pause=True):
     click(x, y, interval, 3, button, _pause)
@@ -471,15 +472,15 @@
 def scroll(scrollAmount=1):
     """
     Sends a scroll input\n
     scrollAmount(int)\n
     _pause is the sleep after every function call
     Positive numbers scroll upwards, negative numbers scroll downwards\n
 
-    Sometimes games dont take the scroll data thats sent and just takes thes scroll input to scroll at a fixed amount so it may not work for some games
+    Sometimes games dont take the scroll data that gets sent and just takes thes scroll input to scroll at a fixed amount so it may not work for some games
     
     """
     ii_ = Input_I()
     ii_.mi = MouseInput(0,0, scrollAmount*120, MOUSEEVENTF_WHEEL, 0, ctypes.pointer(ctypes.c_ulong(0)))
     xx = Input(ctypes.c_ulong(0), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(xx), ctypes.sizeof(xx))
 
@@ -537,20 +538,20 @@
 
     ii_ = Input_I()
     ii_.ki = KeyBdInput(0, KEYS[key.lower()], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
     x = Input(ctypes.c_ulong(1), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
 
 
-def add_hotkey(key, callback, args=None):
+def add_hotkey(key, callback, args=()):
     """
-    Registers a system wide hotkey with optional args using ctypes and GetMessageW starting it in a seperate thread
+    Registers a system wide hotkey with optional args using ctypes and GetMessageW starting it in a seperate daemon thread
 
     """
-    def add_hotkey_thread(key, callback, args=None):
+    def add_hotkey_thread(key, callback, args=()):
         key_id = len(registered_hotkeys) + 1
         registered_hotkeys[VK_KEYS[key]] = key_id
         hotkey_threads[VK_KEYS[key]] = hotkey_thread.native_id
 
         ctypes.windll.user32.RegisterHotKey(None, key_id , None, VK_KEYS[key])
         
         msg = ctypes.wintypes.MSG()
@@ -566,14 +567,15 @@
         
         try:
             ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
         except(KeyError):
             pass
     if key in VK_KEYS:
         hotkey_thread = threading.Thread(target=add_hotkey_thread, args=[key, callback, args])
+        hotkey_thread.daemon = True
         hotkey_thread.start()
 
 
 def remove_hotkey(key):
     """
     Unregisters and removes the specified hotkey if it was registered previously
```

