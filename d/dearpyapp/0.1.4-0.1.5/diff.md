# Comparing `tmp/dearpyapp-0.1.4-py3-none-win_amd64.whl.zip` & `tmp/dearpyapp-0.1.5-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 20519 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      460 b- defN 23-Aug-01 10:34 dearpyapp/__init__.py
--rw-rw-rw-  2.0 fat    10777 b- defN 23-Aug-01 10:34 dearpyapp/application.py
--rw-rw-rw-  2.0 fat     2622 b- defN 23-Aug-01 10:34 dearpyapp/colors.py
--rw-rw-rw-  2.0 fat     8883 b- defN 23-Aug-01 10:34 dearpyapp/themes.py
--rw-rw-rw-  2.0 fat    10757 b- defN 23-Aug-01 10:34 dearpyapp/utils.py
--rw-rw-rw-  2.0 fat      105 b- defN 23-Aug-01 10:34 dearpyapp/components/__init__.py
--rw-rw-rw-  2.0 fat    13513 b- defN 23-Aug-01 10:34 dearpyapp/components/log.py
--rw-rw-rw-  2.0 fat    12733 b- defN 23-Aug-01 10:34 dearpyapp/components/port_control.py
--rw-rw-rw-  2.0 fat     6455 b- defN 23-Aug-01 10:34 dearpyapp/components/tab.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      900 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1133 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/RECORD
-14 files, 69542 bytes uncompressed, 18649 bytes compressed:  73.2%
+Zip file size: 20895 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      460 b- defN 23-Aug-02 04:16 dearpyapp/__init__.py
+-rw-rw-rw-  2.0 fat    10777 b- defN 23-Aug-02 04:16 dearpyapp/application.py
+-rw-rw-rw-  2.0 fat     2622 b- defN 23-Aug-02 04:16 dearpyapp/colors.py
+-rw-rw-rw-  2.0 fat     8883 b- defN 23-Aug-02 04:16 dearpyapp/themes.py
+-rw-rw-rw-  2.0 fat    11053 b- defN 23-Aug-02 04:16 dearpyapp/utils.py
+-rw-rw-rw-  2.0 fat      105 b- defN 23-Aug-02 04:16 dearpyapp/components/__init__.py
+-rw-rw-rw-  2.0 fat    13599 b- defN 23-Aug-02 04:16 dearpyapp/components/log.py
+-rw-rw-rw-  2.0 fat    12733 b- defN 23-Aug-02 04:16 dearpyapp/components/port_control.py
+-rw-rw-rw-  2.0 fat     7605 b- defN 23-Aug-02 04:16 dearpyapp/components/tab.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 23-Aug-02 04:16 dearpyapp-0.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      900 b- defN 23-Aug-02 04:16 dearpyapp-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Aug-02 04:16 dearpyapp-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-02 04:16 dearpyapp-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1133 b- defN 23-Aug-02 04:16 dearpyapp-0.1.5.dist-info/RECORD
+14 files, 71074 bytes uncompressed, 19025 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: dearpyapp/components/port_control.py
 Comment: 
 
 Filename: dearpyapp/components/tab.py
 Comment: 
 
-Filename: dearpyapp-0.1.4.dist-info/LICENSE
+Filename: dearpyapp-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: dearpyapp-0.1.4.dist-info/METADATA
+Filename: dearpyapp-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: dearpyapp-0.1.4.dist-info/WHEEL
+Filename: dearpyapp-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: dearpyapp-0.1.4.dist-info/top_level.txt
+Filename: dearpyapp-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dearpyapp-0.1.4.dist-info/RECORD
+Filename: dearpyapp-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dearpyapp/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 from . import colors as c
 from .application import DpgApp, get_running_app
 from .themes import (
     dpg_get_color_theme,
     dpg_get_default_theme
 )
```

## dearpyapp/utils.py

```diff
@@ -12,14 +12,15 @@
 
 _top_container_name = 'mvWindowAppItem'
 _container_name_lookup = {
     dpg.mvWindowAppItem: _top_container_name,
     dpg.mvChildWindow: 'mvChildWindow',
     dpg.mvGroup: 'mvGroup',
     dpg.mvTab: 'mvTab',
+    dpg.mvTableRow: 'mvTableRow',
 }
 
 _not_container_name_lookup = {
     dpg.mvImage: 'mvImage',
     dpg.mvInputText: 'mvInputText',
     dpg.mvText: 'mvText',
     dpg.mvCombo: 'mvCombo',
@@ -88,26 +89,31 @@
 
 def dpg_get_item_type(item) -> int:
     item_type = _item_type_lookup.get(dpg_get_item_name(item))
     assert item_type is not None
     return item_type
 
 
-def dpg_get_item_by_pos(items: t.Union[list, tuple], mouse_pos, horizontal: bool = False, *,
+def dpg_get_item_by_pos(items: t.Union[int, list[int], tuple[int]], mouse_pos, horizontal: bool = False, *,
                         return_index=False):
+    if type(items) == int:
+        items = dpg.get_item_children(items, 1)
+
+    # TODO разобраться с позицией get_item_pos, get_item_rect_min на различных элементах
+    # TODO если в таблице включен клиппер, то get_item_pos возвращает 0, если элемент вне видимости
+    get_item_pos = dpg.get_item_pos if dpg_get_item_type(items[0]) == dpg.mvText else dpg.get_item_rect_min
+
     index_start = 0
     index_end = len(items)
     while True:
         index = index_start + (index_end - index_start) // 2
         if index == index_start:
             break
         item = items[index]
-        item = item if isinstance(item, (str, int)) else item[0]
-        # TODO если в таблице включен клиппер, то get_item_pos возвращает 0, если элемент вне видимости
-        if mouse_pos[not horizontal] >= dpg.get_item_pos(item)[not horizontal]:
+        if mouse_pos[not horizontal] >= get_item_pos(item)[not horizontal]:
             index_start = index
         else:
             index_end = index
     return (items[index_start], index_start) if return_index else items[index_start]
 
 
 def dpg_set_y_scroll(item, window, offset: float = 0.85):
```

## dearpyapp/components/log.py

```diff
@@ -14,14 +14,15 @@
     # TODO не обновлять лог, если таблица не видна
     # TODO если строк в таблице больше ~900 и ее видно, то ctrl-c на любом input_text приводит к
     #  зависанию(коллбэки не обрабатываются, буфер обмена в других приложениях не работает), если установить в
     #  таблице clipper=True, то все ок, сейчас при больше 900, включается клиппер
     # TODO dpg.clipper для таблиц, так как если таблица видна, то на обновление тратится много ресурсов
     # TODO horizontal scroll + autofit all
     # TODO сделать скрываемые колонки, попробовать использовать нативные хедеры
+    # TODO self.rows to list?
 
     columns = []
     scroll_size = 20
 
     def __init__(self, *, log_size=100):
         self.gui = self._Gui()
         self.log_size = log_size
@@ -161,16 +162,17 @@
             container = dpg_get_item_container(container, dpg.mvChildWindow) or \
                 dpg_get_item_container(container)
 
         mouse_pos = dpg.get_mouse_pos(local=False)
         mouse_pos = (dpg.get_x_scroll(gui.table_window) + mouse_pos[0] - width_offset,
                      dpg.get_y_scroll(gui.table_window) + mouse_pos[1] - height_offset)  # + 15
 
-        row, row_index = dpg_get_item_by_pos(tuple(self.rows.values()), mouse_pos, return_index=True)
-        cell, cell_index = dpg_get_item_by_pos(row, mouse_pos, horizontal=True, return_index=True)
+        rows = tuple(self.rows.values())
+        _, row_index = dpg_get_item_by_pos([cells[0] for cells in rows], mouse_pos, return_index=True)
+        cell, cell_index = dpg_get_item_by_pos(rows[row_index], mouse_pos, horizontal=True, return_index=True)
         text, width, height = dpg_get_text_from_cell(cell, wrap=self.column_widths[cell_index])
         if text is None:
             self._input_text_cleanup()
         else:
             self._input_text_cell and dpg.move_item(self._input_text_cell, before=gui.input_text)
             self._input_text_row = tuple(self.rows)[row_index]
             self._input_text_cell = cell
```

## dearpyapp/components/tab.py

```diff
@@ -21,17 +21,19 @@
     def close(self):
         raise PermissionError
 
     def create_gui(self):
         ...
 
 
+# TODO when tabs not fits to width add combobox with extra tabs
 class TabBar:
     def __init__(self, *, title_height=20, title_width=120, tab_factory=None):
         self.gui = self._Gui()
+        self.drag_tabs = False
         self.title_height = title_height
         self.title_width = title_width
         self.tab_factory = tab_factory
         self.active_tab: t.Optional[Tab, t.Any] = None
         self.tabs: list[t.Union[Tab, t.Any]] = []
 
     def set_tab(self, tab: Tab):
@@ -105,30 +107,50 @@
         with dpg.theme(tag=gui.active_tab_theme):
             with dpg.theme_component(dpg.mvAll):
                 dpg.add_theme_color(dpg.mvThemeCol_Button, c.GRAY_4)
                 dpg.add_theme_color(dpg.mvThemeCol_ButtonHovered, c.GRAY_4)
                 dpg.add_theme_color(dpg.mvThemeCol_ButtonActive, c.GRAY_4)
                 dpg.add_theme_color(dpg.mvThemeCol_Text, c.GRAY_25)
 
+        drag_source_index = 0
+
         def tab_click(s, a, u):
+            nonlocal drag_source_index
             tab: Tab = dpg.get_item_user_data(a[1])
             button = a[0]
             if button == dpg.mvMouseButton_Left:
+                if self.drag_tabs:
+                    drag_source_index = self.tabs.index(tab)
+                    dpg.configure_item(drag_registry, show=True)
                 self.set_tab(tab)
             elif button == dpg.mvMouseButton_Middle:
                 self.close_tab(tab)
 
             if callback := tab.tab_info.click_callback:
                 callback(tab.tab_info.title_id, button)
 
+        def mouse_move(mouse_pos):
+            nonlocal drag_source_index
+            _, target_index = dpg_get_item_by_pos(gui.tab_titles_group, mouse_pos, True, return_index=True)
+            if target_index != drag_source_index:
+                source_tab = self.tabs.pop(drag_source_index)
+                self.tabs.insert(target_index, source_tab)
+                drag_source_index = target_index
+                dpg.reorder_items(gui.tab_titles_group, 1, [tab.tab_info.title_id for tab in self.tabs])
+
         with dpg.item_handler_registry(tag=gui.tab_title_handler):
             dpg.add_item_clicked_handler(dpg.mvMouseButton_Left, callback=tab_click)
             dpg.add_item_clicked_handler(dpg.mvMouseButton_Middle, callback=tab_click)
             dpg.add_item_clicked_handler(dpg.mvMouseButton_Right, callback=tab_click)
 
+        with dpg.handler_registry(show=False) as drag_registry:
+            dpg.add_mouse_release_handler(
+                dpg.mvMouseButton_Left, callback=lambda *_: dpg.configure_item(drag_registry, show=False))
+            dpg.add_mouse_move_handler(callback=lambda s, a, u: mouse_move(a))
+
         with dpg.texture_registry():
             width, height, channels, data = dpg.load_image('icons/add.png')
             add_img = dpg.add_static_texture(width, height, data)
 
         app_ = get_running_app()
         with dpg.group():
             dpg.bind_item_theme(dpg.last_container(), tab_bar_theme)
```

## Comparing `dearpyapp-0.1.4.dist-info/LICENSE` & `dearpyapp-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dearpyapp-0.1.4.dist-info/METADATA` & `dearpyapp-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpyapp
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrapper for DearPyGui
 Home-page: https://github.com/means0nothing/DearPyApp
 Author: Pavel Shevcov
 Author-email: means0nothing@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

