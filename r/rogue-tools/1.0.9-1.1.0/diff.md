# Comparing `tmp/rogue_tools-1.0.9.tar.gz` & `tmp/rogue_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.0.9.tar", last modified: Wed May 24 09:28:00 2023, max compression
+gzip compressed data, was "rogue_tools-1.1.0.tar", last modified: Wed Aug  2 09:23:24 2023, max compression
```

## Comparing `rogue_tools-1.0.9.tar` & `rogue_tools-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:27:59.999720 rogue_tools-1.0.9/
--rw-rw-rw-   0        0        0      517 2023-05-24 09:27:59.965507 rogue_tools-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 09:27:59.953539 rogue_tools-1.0.9/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6255 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4056 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-04-12 11:49:44.000000 rogue_tools-1.0.9/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0    13260 2023-04-13 10:09:49.000000 rogue_tools-1.0.9/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     3380 2023-05-24 09:26:33.000000 rogue_tools-1.0.9/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      147 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1862 2023-04-20 11:22:01.000000 rogue_tools-1.0.9/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     3817 2023-05-18 09:43:37.000000 rogue_tools-1.0.9/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     2300 2023-04-23 02:16:48.000000 rogue_tools-1.0.9/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3401 2023-05-15 13:12:33.000000 rogue_tools-1.0.9/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-04-12 11:49:45.000000 rogue_tools-1.0.9/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:27:59.964510 rogue_tools-1.0.9/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 09:27:59.000000 rogue_tools-1.0.9/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-24 09:28:00.000331 rogue_tools-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1777 2023-05-24 09:27:03.000000 rogue_tools-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:23:24.861181 rogue_tools-1.1.0/
+-rw-rw-rw-   0        0        0      517 2023-08-02 09:23:24.860204 rogue_tools-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 09:23:24.848493 rogue_tools-1.1.0/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.1.0/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-07-28 08:16:04.000000 rogue_tools-1.1.0/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6558 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4070 2023-07-27 12:24:15.000000 rogue_tools-1.1.0/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0    13293 2023-07-31 06:11:18.000000 rogue_tools-1.1.0/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     3380 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      147 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1287 2023-07-31 09:35:35.000000 rogue_tools-1.1.0/rogue_tools/thread_tool.py
+-rw-rw-rw-   0        0        0     2087 2023-08-01 03:05:11.000000 rogue_tools-1.1.0/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     5052 2023-08-02 08:56:19.000000 rogue_tools-1.1.0/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     2300 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3860 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-07-19 04:12:11.000000 rogue_tools-1.1.0/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:23:24.858253 rogue_tools-1.1.0/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-08-02 09:23:24.000000 rogue_tools-1.1.0/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-08-02 09:23:24.000000 rogue_tools-1.1.0/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:23:24.000000 rogue_tools-1.1.0/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-08-02 09:23:24.000000 rogue_tools-1.1.0/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 09:23:24.000000 rogue_tools-1.1.0/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:23:24.000000 rogue_tools-1.1.0/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:23:24.861181 rogue_tools-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-08-02 09:22:59.000000 rogue_tools-1.1.0/setup.py
```

### Comparing `rogue_tools-1.0.9/PKG-INFO` & `rogue_tools-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.0.9
+Version: 1.1.0
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.9/rogue_tools/excel_tool.py` & `rogue_tools-1.1.0/rogue_tools/excel_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,18 +64,16 @@
         if sheet == None:
             return
         #self.start_line         = 0
         self.error_list         = []
         self.row_list           = [] # 是一个规整的二维矩阵
         self.column_list        = [] # 是一个规整的二维矩阵
         self.key_list           = []
-        self.max_row            = sheet.max_row # 最大行
-        self.max_column         = sheet.max_column # 最大列
         self.name               = sheet.title
-        if self.max_row==0:
+        if sheet.max_row==0 or sheet.max_column==0:
             return
         
         # 加载数据
         for row in sheet.rows:
             row_value = []
             for cell in row:
                 value = cell.value if cell.value or cell.value == 0 else ''
@@ -84,19 +82,26 @@
         
         for column in sheet.columns:
             column_value = []
             for cell in column:
                 value = cell.value if cell.value or cell.value == 0 else ''
                 column_value.append(value)
             self.column_list.append(column_value)
-
         # 标记序列的行
         self.key_list = cut_list_tail(self.row_list[0],'')
-
-
+        self.index_list = cut_list_tail(self.column_list[0],'')
+        # 获得最大行列
+        self.max_row = len(self.index_list)
+        self.max_column= len(self.key_list)
+        # 重新规整数据
+        del self.row_list[self.max_row:]
+        for i in range(0,len(self.row_list)-1):
+            del self.row_list[i][self.max_column:]
+        
+        #print(f'init {self.name}')
 
     def get_value(self,x,y):
         '''
         通过表内坐标获得value,从0,0开始
         '''
         return self.row_list[x][y]
     def get_all_rows(self):
@@ -186,15 +191,15 @@
     
     def get_sheet_name_list(self):
         return self._sheet_name_list
 
     def get_sheet(self,sheet_name) -> MySheet:
         return self.sheet_dic.get(sheet_name,None)
     
-    def add_sheet(self,sheet_name):
+    def add_sheet(self,sheet_name)-> MySheet:
         self._sheet_name_list.append(sheet_name)
         self.sheet_dic[sheet_name]=MySheet(sheet_name)
         return self.sheet_dic[sheet_name]
 def calc_26_to_10(a_z:str):
     rs=0
     a_z = a_z.lower()
     sq = len(a_z)-1
```

### Comparing `rogue_tools-1.0.9/rogue_tools/file_tool.py` & `rogue_tools-1.1.0/rogue_tools/file_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return rs
 
 def write_str(path,write_string,my_mode="a+",my_encoding='utf8'):
     if not os.path.exists(path):
         base_dir = path_tool.get_file_dirname(path)
         path_tool.make_folder(base_dir)
     with open(path,my_mode,encoding=my_encoding) as f:
-        f.write(write_string)
+        f.write(str(write_string))
 
 def write_lines(path,write_list,mode="a+",encoding='utf8'):
     temp=""
     for line in write_list:
         temp = f'{temp}{line}\n'
         #temp=temp+line+'\n'
     write_str(path,temp,my_mode=mode,my_encoding=encoding)
@@ -37,22 +37,21 @@
         path_tool.make_folder(base_dir)
         write_str(path,'')
 
 def clear_file(path):
     write_str(path,'',my_mode='w+')
 
 def get_file_size(path):
-    fsize = os.path.getsize(path)
-    return fsize
+    return os.path.getsize(path) if os.path.exists(path) else 0
+
 def get_folder_size(path):
     total = 0
     sub_files = path_tool.get_sub_files(path)
     for sub_file in sub_files:
         total = total + get_file_size(sub_file)
-    
     return total
 
 def wait_file(path,time_out=600):
     '''
     等待一个文件可用，并且不再更改。
     适用于目标文件正在创建、下载、复制的情况
     最少需要2秒,默认最大等待600秒
```

### Comparing `rogue_tools-1.0.9/rogue_tools/filter_tool.py` & `rogue_tools-1.1.0/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools/ini_tool.py` & `rogue_tools-1.1.0/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools/path_tool.py` & `rogue_tools-1.1.0/rogue_tools/path_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 import os
 import stat
 import sys
 import re
 import shutil
 import time
-from concurrent.futures import ThreadPoolExecutor
+
 import traceback
-from rogue_tools import path_tool,file_tool,time_tool
+from rogue_tools import path_tool,file_tool,time_tool,thread_tool
 
 pool = None
 def init_pool():
     '''
     用来加快删除文件夹操作的进程
     '''
     global pool
     if pool==None:
-        pool = ThreadPoolExecutor(max_workers=3)
-        print('加载ThreadPoolExecutor')
+        pool = thread_tool.ThreadPool()
+
 
 
 '''        
 #####################################################################
 #                             简易方法                               #    
 #####################################################################   
 '''
@@ -238,24 +238,26 @@
             traceback.print_exc()
 
 def make_folder(folder_path):
     '''
     创建一个文件夹
     '''
     if os.path.exists(folder_path):
-        return
-    if folder_path in ('',None):
-        return
+        return folder_path
+    folder_path = os.path.abspath(folder_path)
+    drive, tail = os.path.splitdrive(folder_path)
+    folder_path = drive+re.sub(r'[/:*?"<>|]', '_', tail)
     try:
-        #print(f'make_folder:{folder_path}')
         os.makedirs(folder_path,mode=0o777)
     except FileExistsError:
-        return
-    except Exception:
+        pass
+    except BaseException:
         traceback.print_exc()
+    finally:
+        return folder_path
 def del_folder(path,is_keep_folder=True):
     '''
     将此目录改名之后,慢慢清理,使用多线程,可以节省很多时间~~~
     '''
     global pool
     init_pool()
     if os.path.exists(path):
@@ -367,15 +369,15 @@
         path2 = (path2)
     for path_add in path2:
         path_add = path_add if isinstance(path_add,str) else str(path_add)
         if path_add.startswith('\\') or path_add.startswith('/'):
             path_add = path_add[1:len(path_add)]
         path1 = os.path.join(path1,path_add)
 
-    return os.path.normpath(path1)
+    return relative_2_absolute(os.path.normpath(path1))
 # 当前这一句，正在执行的py文件的路径
 # os.path.realpath(__file__)
 
 # 当前这一句，正在执行的py文件的目录
 # os.path.split(os.path.realpath(__file__))[0]
 
 # 当前这一句，正在执行的py文件的名字
@@ -405,27 +407,29 @@
     等待一个文件夹完全准备好文件,复制大文件的情况可能不适用(会提前占长度，导致失败)，通常是解压缩文件的时候
     '''
     file_list = get_sub_files(path)
     for file in file_list:
         wait_file_prepare(file)
 
 def wait_file_prepare(path,time_out=600):
-    total = 0
-    start_time = time_tool.time_stamp_s()
-    while True and time_tool.time_stamp_s() - start_time < time_out:
+    start_time = time.time()
+    total = file_tool.get_file_size(path)
+    while time.time() - start_time < time_out:
         time.sleep(2)
         temp = file_tool.get_file_size(path)
-        #print(f'waiting file:{time_tool.time_stamp_s() - start_time}s , {int(temp/1024)}kb')
         if temp == total and temp > 0:
             return True
-        else:
-            total = temp
+        total = temp
     return False
 
 def is_exists(path):
     return os.path.exists(path)
 
 def is_dir(path):
     return os.path.isdir(path)
 
 def is_file(path):
-    return os.path.isfile(path)
+    return os.path.isfile(path)
+
+def relative_2_absolute(path):
+    '''可以直接调用join_path'''
+    return os.path.abspath(path)
```

### Comparing `rogue_tools-1.0.9/rogue_tools/robot_tool.py` & `rogue_tools-1.1.0/rogue_tools/robot_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools/show_tool.py` & `rogue_tools-1.1.0/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools/time_tool.py` & `rogue_tools-1.1.0/rogue_tools/time_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import time
 def time_stamp():
 	'''
 	超精准时间戳
 	'''
 	return int(round(time.time() * 1000000))
 
+def check_time_stamp(ts=0,print_func=None):
+	'''
+	配合time_stamp使用,debug时候用的时间戳
+	'''
+	now = time_stamp()
+	if ts>0:
+		if print_func:
+			print_func(f'{now - ts}')
+		else:
+			print(f'{now - ts}')
+	return now
 
 def time_stamp_s():
 	'''
 	秒级时间戳
 	'''
 	return int(round(time.time()))
```

### Comparing `rogue_tools-1.0.9/rogue_tools/ui_tool.py` & `rogue_tools-1.1.0/rogue_tools/ui_tool.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,110 @@
 import os
 import sys
 import time
 import traceback
 
 from PyQt5 import QtCore
+from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import *
 from concurrent.futures import ThreadPoolExecutor
-from rogue_tools import file_tool,path_tool
+from rogue_tools import file_tool,path_tool,thread_tool
 
 
 
 class mainUI():
     def __init__(self,w,h,title='PyQt5 - UI by [rogue_tools]',is_center=True):
-        self.config_path        = 'save_params.text'
+        self.config_path        = 'save_params.txt'
         self.save_dic           = self.load_input()
+        self.editor_dic         = {}
         self.ui_width           = w
         self.ui_height          = h
-        self.pool               = ThreadPoolExecutor(max_workers=3)
+        self.pool               = thread_tool.ThreadPool()
         self.app                = QApplication(sys.argv)
         self.windows            = QWidget()
         self.windows.resize(self.ui_width,self.ui_height)
         self.windows.setWindowTitle(title)
         # 居中
         if is_center:
             qr = self.windows.frameGeometry()
             cp = QDesktopWidget().availableGeometry().center()
             qr.moveCenter(cp)
             self.windows.move(qr.topLeft())
 
+
     def show(self):
         #show()方法在屏幕上显示出widget组件
         self.windows.show()
         #循环执行窗口触发事件，结束后不留垃圾的退出，不添加的话新建的widget组件就会一闪而过
         sys.exit(self.app.exec_())
     
     def add_label(self,line_index,title, start_pos = (0,0),obj_w=200,obj_h=20):
         label = QLabel(self.windows)
+        label.setAlignment(QtCore.Qt.AlignTop | QtCore.Qt.AlignLeft)
         label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w , obj_h))
         label.setText(title)
 
     def add_btn(self,line_index,title, start_pos = (0,0),call_func=None,obj_w=100,obj_h=20):
         #设置按钮并给按钮命名
         btn = QPushButton(title,self.windows)
         btn.setGeometry(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w , obj_h)
         if call_func:
             btn.clicked.connect(call_func)
         return btn
-        
+
+    def add_btn_horizontal(self,line_index,title, start_pos = (0,0),call_func=None,obj_w=100,obj_h=20):
+        #设置按钮并给按钮命名
+        btn = QPushButton(title,self.windows)
+        btn.setGeometry(obj_w * line_index+start_pos[0],start_pos[1] , obj_w , obj_h)
+        if call_func:
+            btn.clicked.connect(call_func)
+        return btn
+
     def add_input_editor(self,line_index,title, start_pos = (0,0) ,edit_text='',edit_tips='',obj_w_1=70,obj_w_2=200,obj_h = 20):
-        key = f'{line_index}_{title}'
-        input_str = self.save_dic.get(key,'') if edit_text=='' else edit_text
+        input_str = self.save_dic.get(title,'') if edit_text=='' else edit_text
         # 显示标签
         label = QLabel(self.windows)
         label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_1 , obj_h))
         label.setText(title)
         # 输入框
         edit = QLineEdit(self.windows)
         edit.setPlaceholderText(str(edit_tips))
         edit.setText(str(input_str))
         edit.setGeometry(QtCore.QRect(obj_w_1+start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_2 , obj_h))
         # 管理内容
-        self.save_dic[key] = edit
+        self.editor_dic[title] = edit.text
         return edit
+    
+    def add_combo_box(self,line_index,title, start_pos = (0,0),item_list=[],obj_w_1=70,obj_w_2=200,obj_h = 20):
+        currentText = self.save_dic.get(title,1)
+        # 显示标签
+        label = QLabel(self.windows)
+        label.setGeometry(QtCore.QRect(start_pos[0] , obj_h * line_index+start_pos[1] , obj_w_1 , obj_h))
+        label.setText(title)
+        # 下拉框
+        comb_box = QComboBox(self.windows)
+        comb_box.addItems(item_list)
+        comb_box.setGeometry(QtCore.QRect(start_pos[0]+obj_w_1 , obj_h * line_index+start_pos[1] , obj_w_2 , obj_h))
+        comb_box.setCurrentText(currentText)
+        self.editor_dic[title]=comb_box.currentText
+        return comb_box
+
     def exit_exe(self):
         QtCore.QCoreApplication.instance().quit()
 
     def msgbox(self,msg_str,title=''):
         QMessageBox.about(self.windows, title,msg_str)
+
     def save_input(self):
         write_lines=[]
-        for key in self.save_dic:
-            write_lines.append(f'{key}={self.save_dic[key].text()}')
-        file_tool.write_lines(self.config_path,write_lines)
+        for key in self.editor_dic:
+            write_lines.append(f'{key}={self.editor_dic[key]()}')
+        print(f'save:{write_lines}')
+        file_tool.write_lines(self.config_path,write_lines,'w+')
+
     def load_input(self):
         rs_dic = {}
         if not path_tool.is_exists(self.config_path):
             return rs_dic
         lines = file_tool.read_simple_text(self.config_path)
         
         for line in lines:
```

### Comparing `rogue_tools-1.0.9/rogue_tools/web_tool.py` & `rogue_tools-1.1.0/rogue_tools/web_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools/win_tool.py` & `rogue_tools-1.1.0/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools/zip_tool.py` & `rogue_tools-1.1.0/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.0.9/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.1.0/rogue_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.0.9
+Version: 1.1.0
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.0.9/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.1.0/rogue_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 rogue_tools/file_tool.py
 rogue_tools/filter_tool.py
 rogue_tools/ini_tool.py
 rogue_tools/path_tool.py
 rogue_tools/robot_tool.py
 rogue_tools/show_tool.py
 rogue_tools/string_tool.py
+rogue_tools/thread_tool.py
 rogue_tools/time_tool.py
 rogue_tools/ui_tool.py
 rogue_tools/web_tool.py
 rogue_tools/win_tool.py
 rogue_tools/yaml_tool.py
 rogue_tools/zip_tool.py
 rogue_tools.egg-info/PKG-INFO
```

### Comparing `rogue_tools-1.0.9/setup.py` & `rogue_tools-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 path_tool.del_('rogue_tools.egg-info')
 time.sleep(3)
 
 
 setup(
     name='rogue_tools',  # 包的名字
     author='luohao',  # 作者
-    version='1.0.9',  # 版本号
+    version='1.1.0',  # 版本号
     license='MIT',
 
     description='private tools',  # 描述
     long_description='''long description''',
     author_email='luohao@aobi.com',  # 你的邮箱**
     url='',  # 可以写github上的地址，或者其他地址
     # 包内需要引用的文件夹
@@ -31,15 +31,14 @@
     # package_data={'jieba':['*.*','finalseg/*','analyse/*','posseg/*']},
 
     # 依赖包
     install_requires=[
         'openpyxl >= 3.0.10',
         "requests >= 2.28.1",
         "matplotlib >= 3.7.0",
-        "PyQt5 >= 5.15.7",
         "tqdm >= 4.64.1",
         
     ],
     classifiers=[
         # 'Development Status :: 4 - Beta',
         'Operating System :: Microsoft',  # 你的操作系统  OS Independent      Microsoft
         'Intended Audience :: Developers',
```

