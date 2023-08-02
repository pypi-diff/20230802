# Comparing `tmp/pih-1.48026.tar.gz` & `tmp/pih-1.48027.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48026.tar", last modified: Tue Aug  1 04:09:28 2023, max compression
+gzip compressed data, was "pih-1.48027.tar", last modified: Wed Aug  2 06:34:26 2023, max compression
```

## Comparing `pih-1.48026.tar` & `pih-1.48027.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 04:09:28.102432 pih-1.48026/
--rw-rw-rw-   0        0        0      261 2023-08-01 04:09:28.102432 pih-1.48026/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 04:09:27.539938 pih-1.48026/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48026/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48026/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48026/pih/console_api.py
--rw-rw-rw-   0        0        0   111144 2023-08-01 00:39:59.000000 pih-1.48026/pih/const.py
--rw-rw-rw-   0        0        0   317307 2023-08-01 04:09:20.000000 pih-1.48026/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48026/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48026/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48026/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48026/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48026/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48026/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48026/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48026/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-01 04:09:28.071182 pih-1.48026/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-01 04:09:25.000000 pih-1.48026/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-01 04:09:26.000000 pih-1.48026/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 04:09:25.000000 pih-1.48026/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 04:09:26.000000 pih-1.48026/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 04:09:26.000000 pih-1.48026/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48026/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-01 04:09:28.118057 pih-1.48026/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 06:34:26.621709 pih-1.48027/
+-rw-rw-rw-   0        0        0      261 2023-08-02 06:34:26.621709 pih-1.48027/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 06:34:26.449792 pih-1.48027/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48027/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48027/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48027/pih/console_api.py
+-rw-rw-rw-   0        0        0   111638 2023-08-02 05:09:57.000000 pih-1.48027/pih/const.py
+-rw-rw-rw-   0        0        0   317651 2023-08-02 06:34:15.000000 pih-1.48027/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48027/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48027/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48027/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48027/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48027/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48027/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48027/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48027/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:34:26.590417 pih-1.48027/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-02 06:34:24.000000 pih-1.48027/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-02 06:34:25.000000 pih-1.48027/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 06:34:24.000000 pih-1.48027/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-02 06:34:25.000000 pih-1.48027/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-02 06:34:25.000000 pih-1.48027/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48027/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 06:34:26.621709 pih-1.48027/setup.cfg
```

### Comparing `pih-1.48026/pih/collection.py` & `pih-1.48027/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/console_api.py` & `pih-1.48027/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/const.py` & `pih-1.48027/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -772,15 +772,15 @@
     PATH: str = os.path.join(AD.PATH_ROOT, NAME)
 
 class PATH_FACADE:
 
     SHARED_POINT_PATH: str = os.path.join("S$", CONST.FACADE.NAME)
     LINUX_MOUNT_POINT_PATH: str = f"/mnt/{CONST.FACADE.NAME}"
 
-    PATH: str = f"\\\\{AD.DOMAIN_ALIAS}\\{CONST.FACADE.NAME}\\"
+    VALUE: str = f"\\\\{AD.DOMAIN_MAIN}\\{CONST.FACADE.NAME}\\"
 
     @staticmethod
     def STORAGE_PATH() -> str:
         return os.path.join(HOSTS.DC1.NAME, PATH_FACADE.SHARED_POINT_PATH)
 
 
 class PATH_SCAN:
@@ -827,20 +827,20 @@
     @staticmethod
     def get_new_employee_path(name: str) -> str:
         return os.path.join(os.path.join(PATH_IT.ROOT, PATH_IT.NEW_EMPLOYEES_NAME), name)
 
 class PATH_APP:
 
     NAME: str = "apps"
-    FOLDER: str = os.path.join(PATH_FACADE.PATH, NAME)
+    FOLDER: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 class PATH_DOCS:
     
     NAME: str = f"Docs{CONST.FACADE.SERVICE_FOLDER_SUFFIX}"
-    FOLDER: str = os.path.join(PATH_FACADE.PATH, NAME)
+    FOLDER: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 class PATH_FONTS:
 
     NAME: str = "fonts"
     FOLDER: str = os.path.join(PATH_DOCS.FOLDER, NAME)
 
     @staticmethod
@@ -903,15 +903,15 @@
 
 class PATH_POLIBASE_APP_DATA:
     
     NAME: str = "polibase"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
     PERSON_CARD_REGISTRY_FOLDER: str = os.path.join(FOLDER, "person card folder")
 
-    SERVICE_FOLDER_PATH: str = os.path.join(PATH_FACADE.PATH, f"{NAME}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}")
+    SERVICE_FOLDER_PATH: str = os.path.join(PATH_FACADE.VALUE, f"{NAME}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}")
     
     class SETTINGS:
         MAIN: str = "polibase_main_settings.vbs"
         TEST: str = "polibase_test_settings.vbs"
 
 class PATH_USER:
 
@@ -944,29 +944,29 @@
             else:
                 root += PATH_POLIBASE.TEST_SUFFIX
         return os.path.join(os.path.join(f"//{root}", "polibaseData", "PERSONS"), str(pin))
 
 class PATH_WS:
 
     NAME: str = f"WS{CONST.FACADE.SERVICE_FOLDER_SUFFIX}"
-    PATH: str = os.path.join(PATH_FACADE.PATH, NAME)
+    PATH: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 
 class PATH_BACKUP:
 
     class ROBOCOPY_CONFIG:
 
         NAME: str = "robocopy_config"
-        ROOT: str = os.path.join(PATH_FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
+        ROOT: str = os.path.join(PATH_FACADE.VALUE, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
 
     class COMMAND:
 
         NAME: str = "command"
         ROOT: str = os.path.join(
-            PATH_FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
+            PATH_FACADE.VALUE, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
         
         ATTACH_SHARED_DISKS: str = os.path.join(ROOT, "attach_shared_disks.ps1")
 
     
 
 class PATHS:
 
@@ -1449,26 +1449,40 @@
         if isinstance(value, ServiceInformationBase):
             return isolated_name(ServiceRoles.description(value.name) if get_source_description else value)
         return isolated_name(value.value)
     
     SERVICE_ADMIN: ServiceDescription = ServiceDescription(
         name="ServiceAdmin",
         description="Service admin",
-        host=CONST.HOST.WS735.NAME,
+        host=CONST.HOST.DC1.NAME,
         port=CONST.RPC.PORT(20),
         host_changeable=False,
         commands=[
             ServiceCommands.on_service_starts,
             ServiceCommands.on_service_stops,
             ServiceCommands.get_service_information_table,
             ServiceCommands.heart_beat
         ],
-        modules=["schedule"]
+        modules=["schedule", "lmdbm"]
     )
 
+    '''SERVICE_ADMIN: ServiceDescription = ServiceDescription(
+        name="ServiceAdmin",
+        description="Service admin",
+        host=CONST.HOST.DC1.NAME,
+        port=CONST.RPC.PORT(20),
+        host_changeable=False,
+        commands=[
+            ServiceCommands.on_service_starts,
+            ServiceCommands.on_service_stops,
+            ServiceCommands.get_service_information_table,
+            ServiceCommands.heart_beat
+        ]
+    )'''
+
     EVENT_AND_LOG: ServiceDescription = ServiceDescription(
                                             name="EventAndLog",
                                             description="Log and Event service",
                                             host=CONST.HOST.BACKUP_WORKER.NAME, 
                                             commands=[
                                                         ServiceCommands.send_log_message,
                                                         ServiceCommands.send_event
@@ -1629,15 +1643,15 @@
                                                                      "kaleido", "plotly"
                                                                      ]
                                                         )
 
     MARK: ServiceDescription = ServiceDescription(
                                                 name="Orion",
                                                 description="Orion service",
-                                                host=CONST.HOST.DC2.NAME,
+                                                host=CONST.HOST.BACKUP_WORKER.NAME,
                                                 commands=
                                                         [
                                                             ServiceCommands.get_free_mark_list,
                                                             ServiceCommands.get_temporary_mark_list,
                                                             ServiceCommands.get_mark_person_division_list,
                                                             ServiceCommands.get_time_tracking,
                                                             ServiceCommands.get_mark_list,
```

### Comparing `pih-1.48026/pih/pih.py` & `pih-1.48027/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,15 +530,16 @@
     @property
     def argv(self) -> list[str]:
         raise NotImplemented()
 
     def arg(self, index: int = None, default_value: str | None = None) -> str:
         raise NotImplemented()
 
-    def get_file_path(self) -> str:
+    @property
+    def file_path(self) -> str:
         raise NotImplemented()
 
     @property
     def file_name(self) -> str:
         raise NotImplemented()
 
     def authenticate(self, exit_on_fail: bool = True) -> bool:
@@ -610,25 +611,30 @@
             self.output.new_line()
             return
         self.output.error(f"Ты кто такой? Давай, до свидания...")
         self.exit()
 
     @property
     def argv(self) -> list[str]:
-        return sys.argv[1:] if len(sys.argv) > 1 else None
+        return sys.argv[1:] if len(sys.argv) > 1 else []
     
     def arg(self, index: int = 0, default_value: Any | None = None) -> str:
         return DataTool.by_index(self.argv, index, default_value)
 
-    def get_file_path(self) -> str:
+    @property
+    def file_path(self) -> str:
         return sys.argv[0]
 
     @property
+    def is_standalone(self) -> bool:
+        return self.file_path.endswith(FILE.EXTENSION.EXE)
+
+    @property
     def file_name(self) -> str:
-        return PathTool.get_file_name(self.get_file_path())
+        return PathTool.get_file_name(self.file_path)
 
     def authenticate(self, exit_on_fail: bool = True, once: bool = True) -> bool:
         try:
             if once and self.authenticated:
                 return True
             self.output.green("Инициализация...")
             self.output.clear_screen()
@@ -1637,15 +1643,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48020"  
 
         @staticmethod
         def local() -> str:
-            return "1.48026"
+            return "1.48027"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1746,14 +1752,16 @@
                     start = "Неактивный пользователь"
                 return NotFound(f"{start} с {title} '{value}' не найден", value)
 
     class UPDATER:
 
         @staticmethod
         def update_for_service(role_or_information: ServiceRoles | ServiceDescription, pih_update: bool = False, modules_update: bool = True, show_output: bool = True) -> bool:
+            if PIH.session.is_standalone:
+                return True
             description: ServiceDescription = ServiceRoles.description(role_or_information)
             returncode: int = 0
             if pih_update:
                 remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(description, True)
                 command_list: list[str] = remote_executor_command_list + \
                     PIH.UPDATER.get_module_updater_command_list(PIH.NAME, None)
                 process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(
@@ -1992,16 +2000,16 @@
         @staticmethod
         def get_executor_path(executor_name: str) -> str:
             return os.path.join(
                 PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
 
         @staticmethod
         def create_command_list_for_command(executor_name: str, command_list: list[str], login: str | None = None, password: str | None = None) -> list[str]:
-            login = "\\".join([AD.DOMAIN_NAME, login or PIH.OS.get_variable(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
-            password = password or PIH.OS.get_variable(CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
+            login = "\\".join([AD.DOMAIN_NAME, login or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
+            password = password or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
             return [PIH.PSTOOLS.get_executor_path(executor_name), CONST.PSTOOLS.NO_BANNER, CONST.PSTOOLS.ACCEPTEULA, "-u", login, "-p", password]  + command_list
         
         @staticmethod
         def create_command_list_for_psexec_command(command_list: list[str], host: str | None = None, login: str | None = None, password: str | None = None, interactive: bool | None = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> list[str]:
             result_command_list: list[str] = DataTool.check_not_none(interactive, lambda: [["-d", "-i"][interactive]], [])
             host_start: str = r"\\"
             if not DataTool.is_empty(host):
@@ -2022,14 +2030,15 @@
             login: str | None = DataTool.check_not_none(description.login, lambda: PIH.DATA.FORMAT.variable(description.login))
             password: str | None = DataTool.check_not_none(description.password, lambda: PIH.DATA.FORMAT.variable(description.password))
             return PIH.PSTOOLS.create_command_list_for_psexec_command([role_or_information.pyton_executor_path or CONST.PYTHON.EXECUTOR_ALIAS], PIH.SERVICE.get_host(description), login, password, interactive, description.run_from_system_account)
 
         @staticmethod
         def execute_command_list(command: list[str] | str, show_output: bool, capture_output: bool = False, as_text: bool = True, as_shell: bool = False) -> CompletedProcess:
             if show_output:
+                print(" ".join(command))
                 if capture_output:
                     process_result = subprocess.run(
                         command, capture_output=True, text=as_text, shell=as_shell)
                 else:
                     process_result = subprocess.run(
                         command, text=as_text)
             else:
@@ -2044,17 +2053,16 @@
                 return PIH.PSTOOLS.execute_command_list(["taskkill", "/s", host, "/t", "/f", "/im" if is_string else "/pid", PIH.PATH.add_extension(name_or_pid, FILE.EXTENSION.EXE) if is_string else str(name_or_pid)], show_output).returncode < 2
            return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, [PIH.DATA.FORMAT.host(host), "-t", str(name_or_pid)]), show_output).returncode == 0
 
         @staticmethod
         def process_is_exists(pid: int, host: str | None = None, login: str | None = None, password: str | None = None) -> str:
             command_list: list[str] = ["tasklist", "/fi", f"pid eq {pid}", "/fo", "list"]
             login = "\\".join(
-                [AD.DOMAIN_NAME, login or PIH.OS.get_variable(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
-            password = password or PIH.OS.get_variable(
-                CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
+                [AD.DOMAIN_NAME, login or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
+            password = password or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
             if not DataTool.is_empty(host):
                 command_list += ["/s", host]
                 command_list += ["/u", login]
                 command_list += ["/p", password]
             output: str = PIH.PSTOOLS.execute_command_list(
                 command_list, True, True, as_text=False).stdout.decode(WINDOWS.CHARSETS.ALTERNATIVE).lower()
             return output.find("pid") != -1
@@ -2538,31 +2546,32 @@
                 ServiceRoles.description(role_or_information).host = PIH.OS.host()
 
             @staticmethod
             def service_information_list() -> list[ServiceInformation]:
                 return DataTool.to_list(PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP)
 
             @staticmethod
-            def kill_all(via_pskill: bool = False, local: bool = False) -> bool:
+            def kill_all(local: bool = True, via_taskkill: bool = True, exclude_me: bool = False) -> bool:
                 hosts: set[str] = set()
                 for server_role in ServiceRoles:
                     host: str | None = ServiceRoles.description(server_role).host
                     if not DataTool.is_empty(host):
                         hosts.add(host)
-                def kill(host: str, local: bool, via_pskill: bool) -> None:
+                def kill(host: str, local: bool, via_taskkill: bool) -> None:
                     if local:
-                        PIH.PSTOOLS.kill_python_process(host, via_pskill)
+                        PIH.PSTOOLS.kill_python_process(host, via_taskkill)
                     else:
-                        PIH.ACTION.WORKSTATION.kill_python_process(host, via_pskill)
+                        PIH.ACTION.WORKSTATION.kill_python_process(host, via_taskkill)
                 for host in hosts:
                     if host != PIH.OS.host():
-                        kill(host, local, via_pskill)
-                for host in hosts:
-                    if host == PIH.OS.host():
-                        kill(host, local, via_pskill)
+                        kill(host, local, via_taskkill)
+                if not exclude_me:
+                    for host in hosts:
+                        if host == PIH.OS.host():
+                            kill(host, local, via_taskkill)
 
             @staticmethod
             def subscribe_on(service_command: ServiceCommands, type: int = SubscribtionTypes.ON_RESULT, name: str | None = None) -> bool:
                 return RPC.service.subscribe_on(service_command, type, name)
 
             @staticmethod
             def unsubscribe(service_command: ServiceCommands, type: int) -> bool:
@@ -2620,15 +2629,15 @@
                 if check_if_started:
                     if PIH.SERVICE.check_accessibility(description):
                         return None
                 remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(description, False)
                 service_file_path: str | None = None
                 if DataTool.is_empty(description.service_path):
                     service_file_path = os.path.join(
-                        PATH_FACADE.PATH, f"{description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
+                        PATH_FACADE.VALUE, f"{description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 else:
                     service_file_path = os.path.join(
                         description.service_path, PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 remote_executor_command_list.append(service_file_path)
                 remote_executor_command_list.append("false")
                 process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(remote_executor_command_list, show_output)
                 returncode = process_result.returncode
@@ -2661,15 +2670,15 @@
                 if isolate:
                      PIH.SERVICE.ADMIN.isolate(service_description)
                 else:
                     if not PIH.DATA.contains(host, service_description.host):
                         if service_description.host_changeable:
                             PIH.SERVICE.ADMIN.change_host_on_local(service_description)
                         else:
-                            pass
+                            raise Exception("")
                     if stop_before:
                         if PIH.SERVICE.check_accessibility(service_description):
                             PIH.SERVICE.ADMIN.stop(service_description)
                 def internal_start_handler(service: IService) -> None:
                     if PIH.OS.is_linux():
                         PIH.PATH.make_directory_if_not_exists(PATHS.FACADE.LINUX_MOUNT_POINT_PATH, host)
                         PIH.PATH.mount_facade_storage_on_linux_host(host)
@@ -2832,15 +2841,15 @@
         def get_creation_time(path: str) -> str:
             return os.path.getctime(PIH.PATH.adapt_if_linux(path))
 
         @staticmethod
         def adapt_if_linux(path: str) -> str:
             if PIH.OS.is_linux():
                 path = PIH.PATH.convert_for_unix(path)
-                alias: str = PIH.PATH.convert_for_unix(PATH_FACADE.PATH)
+                alias: str = PIH.PATH.convert_for_unix(PATH_FACADE.VALUE)
                 if path.find(alias) == 0:
                     path = path[len(alias):]
                     path = PATHS.FACADE.LINUX_MOUNT_POINT_PATH + path
             return path
 
         @staticmethod
         def get_command_for_mount_storage_on_linux_host(storage_path: str, linux_mount_point: str, linux_host_user_password: str, storage_host_user_login: str, storage_host_user_password: str) -> str:
@@ -2921,18 +2930,14 @@
             def mobile_helper_command(name: str) -> str:
                 name = PIH.DATA.FORMAT.mobile_helper_command(name)
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
 
     class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
 
         @staticmethod
-        def make_sudo(command: str, password: str) -> str:
-            return f"echo -e '{password}\n' | sudo -S " + command
-
-        @staticmethod
         def translit(value, language_code=None, reversed=False, strict=False):
             return translit(value, language_code, reversed, strict)
 
         @staticmethod
         def find_variables(name: str | None) -> list[StorageValue]:
             return PIH.DATA.MATERIALIZED_RESOURCES.find(name) + PIH.SETTINGS.find(name)
         
@@ -3057,15 +3062,15 @@
                 return DataTool.fill_data_from_source(NewMailMessage(), value)
 
             @staticmethod
             def mailbox_info(value: dict | None) -> MailboxInfo | None:
                 if DataTool.is_none(value):
                     return None
                 result: MailboxInfo = DataTool.fill_data_from_source(MailboxInfo(), value)
-                result.timestamp = DataTool.datetime_from_string(result.timestamp)
+                result.timestamp = DateTimeTool.datetime_from_string(result.timestamp)
                 return result
 
             @staticmethod
             def polibase_person(value: dict) -> PolibasePerson:
                 polibase_person: PolibasePerson = DataTool.fill_data_from_source(PolibasePerson(), value)
                 polibase_person.Birth = DateTimeTool.datetime_from_string(polibase_person.Birth)
                 polibase_person.registrationDate = DateTimeTool.datetime_from_string(polibase_person.registrationDate )
@@ -3382,17 +3387,17 @@
 
         class FORMAT:
 
             @staticmethod
             def variable(value: str, parse: bool = True) -> str:
                 fields: list[str] | None = if_else(parse, [name for _, name, _, _ in Formatter().parse(value) if name], [value])
                 if DataTool.is_empty(fields):
-                    return None
+                    return value
                 variable_name: str = fields[0]
-                return PIH.OS.get_variable(variable_name) or PIH.SETTINGS.get(variable_name)
+                return PIH.DATA.get_variable_value(variable_name)
 
             @staticmethod
             def statistics(type: MATERIALIZED_RESOURCES.TYPES) -> str | None:
                 statistics: TimeSeriesStatistics | None = PIH.DATA.STATISTICS.by_name(type.name)
                 if DataTool.is_none(statistics):
                     return None
                 count: int = PIH.DATA.MATERIALIZED_RESOURCES.get_count(type)
@@ -3619,15 +3624,15 @@
                     return user.telephoneNumber is not None
                 def map_function(user: User) -> str:
                     return PIH.DATA.FORMAT.telephone_number(user.telephoneNumber)
                 return ResultTool.map(ResultTool.filter(PIH.RESULT.USER.by_name(AD.SEARCH_ALL_PATTERN, active=active), filter_function), map_function).data
 
             @staticmethod
             def it_administrator() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(PIH.OS.get_variable(CONST.ADMINISTRATOR_LOGIN_ALIAS))
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_LOGIN_ALIAS))
 
             @staticmethod
             def call_centre_administrator() -> str:
                 return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.USER.CALL_CENTRE_ADMINISTRATOR)
 
             @staticmethod
             def marketer() -> str:
@@ -3724,14 +3729,18 @@
                     return sort_function
                 value.sort(key=sort_function)
                 return value
 
     class OS:
 
         @staticmethod
+        def make_sudo(command: str, password: str) -> str:
+            return f"echo -e '{password}\n' | sudo -S " + command
+
+        @staticmethod
         def python_path() -> str | None:
             name: str = "\\Python\\Python"
             for item in PIH.OS.get_variable("PATH").split(";"):
                 index: int = item.find(name)
                 if index != -1 and len(item) - (index + len(name)) <= 4:
                     return os.path.join(item, j((CONST.PYTHON.EXECUTOR, FILE.EXTENSION.EXE), "."))
             return None
```

### Comparing `pih-1.48026/pih/rpc.py` & `pih-1.48027/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/rpcCommandCall_pb2.py` & `pih-1.48027/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48027/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/rpc_collection.py` & `pih-1.48027/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/rpc_const.py` & `pih-1.48027/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/service_example.py` & `pih-1.48027/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/tools.py` & `pih-1.48027/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih/widgets.py` & `pih-1.48027/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48026/pih_setup.py` & `pih-1.48027/pih_setup.py`

 * *Files identical despite different names*

