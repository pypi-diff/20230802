# Comparing `tmp/zymod-0.0.1.20-py3-none-any.whl.zip` & `tmp/zymod-0.0.1.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,35 @@
-Zip file size: 20813 bytes, number of entries: 26
--rw-r--r--  2.0 unx      271 b- defN 23-Jan-13 09:47 zymod/__init__.py
--rw-r--r--  2.0 unx    21485 b- defN 23-Mar-07 06:08 zymod/zymod.py
--rw-r--r--  2.0 unx     1013 b- defN 23-Feb-28 09:44 zymod/zymod_config.py
--rw-r--r--  2.0 unx      174 b- defN 22-Dec-27 06:15 zymod/event/__init__.py
--rw-r--r--  2.0 unx      117 b- defN 22-Dec-27 06:15 zymod/event/zy_event_level_enum.py
--rw-r--r--  2.0 unx      718 b- defN 23-Feb-28 02:34 zymod/event/zy_internal_event.py
--rw-r--r--  2.0 unx      192 b- defN 22-Dec-27 06:15 zymod/inotify/__init__.py
--rw-r--r--  2.0 unx      611 b- defN 22-Dec-27 06:15 zymod/inotify/zy_file_event_enum.py
--rw-r--r--  2.0 unx     2265 b- defN 23-Mar-07 06:08 zymod/inotify/zy_inotify_file_event.py
--rw-r--r--  2.0 unx      145 b- defN 22-Dec-27 06:15 zymod/ssl/__init__.py
--rw-r--r--  2.0 unx     2243 b- defN 23-Feb-28 09:44 zymod/ssl/zy_cert.py
--rw-r--r--  2.0 unx     8560 b- defN 23-Feb-28 09:44 zymod/ssl/zy_cert_validator.py
--rw-r--r--  2.0 unx      442 b- defN 22-Dec-27 06:15 zymod/systemd/__init__.py
--rw-r--r--  2.0 unx     1943 b- defN 22-Dec-27 06:15 zymod/systemd/zy_systemd_manager.py
--rw-r--r--  2.0 unx     3442 b- defN 22-Dec-27 06:15 zymod/systemd/zy_systemd_timer.py
--rw-r--r--  2.0 unx      560 b- defN 22-Dec-27 06:15 zymod/systemd/zy_systemd_timer_prop.py
--rw-r--r--  2.0 unx      775 b- defN 22-Dec-27 06:15 zymod/systemd/zy_systemd_unit.py
--rw-r--r--  2.0 unx      505 b- defN 22-Dec-27 06:15 zymod/systemd/zy_systemd_unit_prop.py
--rw-r--r--  2.0 unx      197 b- defN 22-Dec-27 06:15 zymod/util/__init__.py
--rw-r--r--  2.0 unx     2087 b- defN 22-Dec-27 06:15 zymod/util/time_duration_calculator.py
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-07 06:08 zymod_help/version.txt
--rw-r--r--  2.0 unx     1072 b- defN 23-Mar-07 06:08 zymod-0.0.1.20.dist-info/LICENSE
--rw-r--r--  2.0 unx     4932 b- defN 23-Mar-07 06:08 zymod-0.0.1.20.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-07 06:08 zymod-0.0.1.20.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-07 06:08 zymod-0.0.1.20.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2166 b- defN 23-Mar-07 06:08 zymod-0.0.1.20.dist-info/RECORD
-26 files, 56032 bytes uncompressed, 17303 bytes compressed:  69.1%
+Zip file size: 25426 bytes, number of entries: 33
+-rw-r--r--  2.0 unx      271 b- defN 23-Mar-13 06:31 zymod/__init__.py
+-rw-r--r--  2.0 unx    22555 b- defN 23-Mar-16 05:55 zymod/zymod.py
+-rw-r--r--  2.0 unx      853 b- defN 23-Mar-16 02:26 zymod/zymod_config.py
+-rw-r--r--  2.0 unx      174 b- defN 23-Mar-13 06:31 zymod/event/__init__.py
+-rw-r--r--  2.0 unx      117 b- defN 23-Mar-13 06:31 zymod/event/zy_event_level_enum.py
+-rw-r--r--  2.0 unx      718 b- defN 23-Mar-13 06:31 zymod/event/zy_internal_event.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Mar-13 06:31 zymod/inotify/__init__.py
+-rw-r--r--  2.0 unx      611 b- defN 23-Mar-13 06:31 zymod/inotify/zy_file_event_enum.py
+-rw-r--r--  2.0 unx     2265 b- defN 23-Mar-13 06:31 zymod/inotify/zy_inotify_file_event.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Mar-13 06:31 zymod/ssl/__init__.py
+-rw-r--r--  2.0 unx     2529 b- defN 23-Mar-22 02:37 zymod/ssl/zy_cert.py
+-rw-r--r--  2.0 unx    10663 b- defN 23-Mar-22 02:37 zymod/ssl/zy_cert_validator.py
+-rw-r--r--  2.0 unx      625 b- defN 23-Jun-29 02:46 zymod/systemd/__init__.py
+-rw-r--r--  2.0 unx     1943 b- defN 23-Mar-13 06:31 zymod/systemd/zy_systemd_manager.py
+-rw-r--r--  2.0 unx     1505 b- defN 23-Jun-29 02:46 zymod/systemd/zy_systemd_service.py
+-rw-r--r--  2.0 unx      441 b- defN 23-Jun-29 02:46 zymod/systemd/zy_systemd_service_prop.py
+-rw-r--r--  2.0 unx     3442 b- defN 23-Mar-13 06:31 zymod/systemd/zy_systemd_timer.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Mar-13 06:31 zymod/systemd/zy_systemd_timer_prop.py
+-rw-r--r--  2.0 unx     1417 b- defN 23-Jun-29 02:46 zymod/systemd/zy_systemd_unit.py
+-rw-r--r--  2.0 unx      505 b- defN 23-Mar-13 06:31 zymod/systemd/zy_systemd_unit_prop.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-29 02:46 zymod/util/__init__.py
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-29 02:46 zymod/util/dbus_utils.py
+-rw-r--r--  2.0 unx     2087 b- defN 23-Mar-13 06:31 zymod/util/time_duration_calculator.py
+-rw-r--r--  2.0 unx      169 b- defN 23-Jun-29 02:46 zymod/zyapp_service/__init__.py
+-rw-r--r--  2.0 unx     7747 b- defN 23-Jun-29 02:46 zymod/zyapp_service/service.py
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-29 02:46 zymod/zyprocfs/__init__.py
+-rw-r--r--  2.0 unx      909 b- defN 23-Jun-29 02:46 zymod/zyprocfs/procfs.py
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 02:46 zymod_help/version.txt
+-rw-r--r--  2.0 unx     1072 b- defN 23-Aug-02 09:36 zymod-0.0.1.26.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2070 b- defN 23-Aug-02 09:36 zymod-0.0.1.26.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 09:36 zymod-0.0.1.26.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 09:36 zymod-0.0.1.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2771 b- defN 23-Aug-02 09:36 zymod-0.0.1.26.dist-info/RECORD
+33 files, 69337 bytes uncompressed, 20964 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -36,14 +36,20 @@
 
 Filename: zymod/systemd/__init__.py
 Comment: 
 
 Filename: zymod/systemd/zy_systemd_manager.py
 Comment: 
 
+Filename: zymod/systemd/zy_systemd_service.py
+Comment: 
+
+Filename: zymod/systemd/zy_systemd_service_prop.py
+Comment: 
+
 Filename: zymod/systemd/zy_systemd_timer.py
 Comment: 
 
 Filename: zymod/systemd/zy_systemd_timer_prop.py
 Comment: 
 
 Filename: zymod/systemd/zy_systemd_unit.py
@@ -51,29 +57,44 @@
 
 Filename: zymod/systemd/zy_systemd_unit_prop.py
 Comment: 
 
 Filename: zymod/util/__init__.py
 Comment: 
 
+Filename: zymod/util/dbus_utils.py
+Comment: 
+
 Filename: zymod/util/time_duration_calculator.py
 Comment: 
 
+Filename: zymod/zyapp_service/__init__.py
+Comment: 
+
+Filename: zymod/zyapp_service/service.py
+Comment: 
+
+Filename: zymod/zyprocfs/__init__.py
+Comment: 
+
+Filename: zymod/zyprocfs/procfs.py
+Comment: 
+
 Filename: zymod_help/version.txt
 Comment: 
 
-Filename: zymod-0.0.1.20.dist-info/LICENSE
+Filename: zymod-0.0.1.26.dist-info/LICENSE
 Comment: 
 
-Filename: zymod-0.0.1.20.dist-info/METADATA
+Filename: zymod-0.0.1.26.dist-info/METADATA
 Comment: 
 
-Filename: zymod-0.0.1.20.dist-info/WHEEL
+Filename: zymod-0.0.1.26.dist-info/WHEEL
 Comment: 
 
-Filename: zymod-0.0.1.20.dist-info/top_level.txt
+Filename: zymod-0.0.1.26.dist-info/top_level.txt
 Comment: 
 
-Filename: zymod-0.0.1.20.dist-info/RECORD
+Filename: zymod-0.0.1.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zymod/zymod.py

```diff
@@ -82,38 +82,44 @@
     describe_format = '%s模块%s' % (module_name, describe_replace)
     summary_format = '%s模块%s' % (module_name, summary_replace)
 
     return {"level": event_level, "summary": summary_format, "description": describe_format,
             "metric": {"name": filed_name, "value": filed_value, "threshold_value": threshold_value}}
 
 
-def upload_zy_exception_event(content: dict, agent_host: str, agent_port: str, mod_name: str, host: str):
+def upload_zy_exception_event(content: dict, info_map):
     fn_name = 'upload_zy_exception_event'
-
     hlog = HappyLog.get_instance()
+
     hlog.enter_func(fn_name)
 
     json_str_content = dict_to_pretty_json(content)
 
     hlog.debug('zymod：正在上传到agent.....')
+
     channel = grpc.insecure_channel(
-        agent_host + ':' + agent_port)
+        info_map["agent_host"] + ':' + info_map["agent_port"])
+
+    if info_map["dry_run"]:
+        hlog.debug('zymod：在不做任何更改的情况下试运行.....')
+    else:
+        try:
+            client = zhiyan_rpc_pb2_grpc.ZhiYanServiceStub(channel)
+
+            response = client.zyevent(zhiyan_rpc_pb2.ZhiYanEventRequest(
+                mod_name=info_map["mod_name"],
+                time=str(utc_time()),
+                host=info_map["host"],
+                event=json_str_content
+            ))
+
+            hlog.info('code:' + response.code + '\tmessage:' + response.message)
 
-    try:
-        client = zhiyan_rpc_pb2_grpc.ZhiYanServiceStub(channel)
-        response = client.zyevent(zhiyan_rpc_pb2.ZhiYanEventRequest(
-            mod_name=mod_name,
-            time=str(utc_time()),
-            host=host,
-            event=json_str_content
-        ))
-
-        hlog.info('code:' + response.code + '\tmessage:' + response.message)
-    except Exception as ex:
-        hlog.error('code:' + "1" + '\tmessage:' + 'Agent连接失败,十秒后进行下一次尝试\tErrorMessage:' + str(ex))
+        except Exception as ex:
+            hlog.error('code:' + "1" + '\tmessage:' + 'Agent连接失败,十秒后进行下一次尝试\tErrorMessage:' + str(ex))
 
     hlog.exit_func(fn_name)
 
 
 def event_level_transformation_en_to_num(event_level):
     event_dict = {
         "notice": 0,
@@ -176,23 +182,31 @@
     hlog = HappyLog.get_instance()
     mod_conf: dict[Any, Any]
     parser: ArgumentParser
 
     def __init__(self, mod_config: Path, is_dry_run_from_cmd_args, is_verbose_from_cmd_args):
         signal.signal(signal.SIGINT, interrupt_from_keyboard_handler)
 
+        if not mod_config.exists():
+            self.hlog.error('智眼模块配置文件（%s）不存在' % mod_config)
+            exit(1)
+
         self.hlog = HappyLog.get_instance(str(mod_config))
 
         self.is_dry_run = True if is_dry_run_from_cmd_args else None
         self.is_verbose = True if is_verbose_from_cmd_args else None
 
         self.public_zymod_config = LoadPublicZymodConfigParser()
         HappyConfigParser.load(str(mod_config), self.public_zymod_config)
         self.mod_config_path = str(mod_config)
 
+        self._dry_run = self.public_zymod_config.dry_run if self.is_dry_run is None else True
+
+        self._dry_run_convert = True if str(self._dry_run).lower() in ['true', '1', 't', 'y', 'yes', 'yeah'] else False
+
     @staticmethod
     def event_level_transformation(event_level: str):
         if event_level == "通知":
             return 0
         elif event_level == "警告":
             return 1
         elif event_level == "警报":
@@ -204,14 +218,21 @@
         if event_type == "log":
             hlog.warning(event)
         elif event_type == "upload":
             self.upload_event(event)
         else:
             hlog.error("事件生成失败，类型识别错误")
 
+    def get_basic_config_info(self):
+        return {'dry_run': self._dry_run_convert,
+                'agent_host': self.public_zymod_config.agent_host,
+                'agent_port': self.public_zymod_config.agent_port,
+                'mod_name': self.public_zymod_config.mod_name,
+                'host': self.public_zymod_config.host}
+
     # def event_status(self):
     #     hlog = HappyLog.get_instance()
     #     hlog.enter_func("event_status")
     #
     #     notice_status = 1 if self.public_zymod_config.notice_report == "true" else 0
     #     event_status = 1 if self.public_zymod_config.event_report == "true" else 0
     #     alert_status = 1 if len(self.public_zymod_config.alert_threshold) != 0 else 0
@@ -341,22 +362,28 @@
         fn_name = 'mod_send_request_grpc'
 
         hlog = HappyLog.get_instance()
         hlog.enter_func(fn_name)
 
         hlog.var('name', self.public_zymod_config.mod_name)
         param_check(self.public_zymod_config.mod_name, 'mod_name')
-        hlog.var('datetime', str(utc_time()),)
+        hlog.var('datetime', str(utc_time()))
 
         json_str_content = dict_to_pretty_json(content)
 
         hlog.debug('content=\n%s' % json_str_content)
 
-        if bool(self.is_dry_run):
-            hlog.debug('zymod：试运行中，不进行注册.....')
+        if self.public_zymod_config.language_file:
+            with open(self.public_zymod_config.language_file, 'r') as language_file:
+                language = str(json.load(language_file))
+        else:
+            language = ''
+
+        if self._dry_run_convert:
+            hlog.info('zymod：试运行中，不进行注册.....')
         else:
             hlog.debug('zymod：正在上传到agent.....')
             channel = grpc.insecure_channel(
                 self.public_zymod_config.agent_host + ':' + str(self.public_zymod_config.agent_port))
 
             param_check(self.public_zymod_config.agent_host, 'agent_host')
             param_check(self.public_zymod_config.agent_port, 'agent_port')
@@ -372,19 +399,18 @@
                     config=str({
                         "host": self.public_zymod_config.host,
                         "active": self.public_zymod_config.active,
                         "debug": self.public_zymod_config.debug,
                         "dry_run": self.public_zymod_config.dry_run,
                         "interval": self.public_zymod_config.interval,
                         "mod_name": self.public_zymod_config.mod_name,
-                        "headers": self.public_zymod_config.headers,
-                        # "unit": self.public_zymod_config.unit,
-                        "chinese_name": self.public_zymod_config.chinese_name,
+                        "language_file": language,
+                        "display_name": self.public_zymod_config.display_name,
                         "mod_type": self.public_zymod_config.mod_type,
-                    }),
+                    })
                 ))
                 hlog.info('code:' + response.code + '\tmessage:' + response.message)
 
                 if response.code != '1':
                     register = True
                 else:
                     register = False
@@ -401,16 +427,16 @@
         fn_name = 'upload_event'
 
         hlog = HappyLog.get_instance()
         hlog.enter_func(fn_name)
 
         json_str_content = dict_to_pretty_json(content)
 
-        if bool(self.is_dry_run):
-            hlog.debug('zymod：在不做任何更改的情况下试运行.....')
+        if self._dry_run_convert:
+            hlog.info('zymod：在不做任何更改的情况下试运行.....')
         else:
             hlog.debug('zymod：正在上传到agent.....')
             channel = grpc.insecure_channel(
                 self.public_zymod_config.agent_host + ':' + str(self.public_zymod_config.agent_port))
 
             try:
                 client = zhiyan_rpc_pb2_grpc.ZhiYanServiceStub(channel)
@@ -434,22 +460,23 @@
         fn_name = 'mod_send_request_grpc'
 
         hlog = HappyLog.get_instance()
         hlog.enter_func(fn_name)
 
         hlog.var('name', self.public_zymod_config.mod_name)
         param_check(self.public_zymod_config.mod_name, 'mod_name')
-        hlog.var('datetime', str(utc_time()),)
+        hlog.var('datetime', str(utc_time()))
 
         json_str_content = dict_to_pretty_json(content)
 
         hlog.debug('content=\n%s' % json_str_content)
 
-        if bool(self.is_dry_run):
-            hlog.debug('zymod：在不做任何更改的情况下试运行.....')
+        if self._dry_run_convert:
+            hlog.info('zymod：在不做任何更改的情况下试运行.....')
+            time.sleep(float(self.public_zymod_config.interval))
         else:
             hlog.debug('zymod：正在上传到agent.....')
             channel = grpc.insecure_channel(
                 self.public_zymod_config.agent_host + ':' + str(self.public_zymod_config.agent_port))
 
             param_check(self.public_zymod_config.agent_host, 'agent_host')
             param_check(self.public_zymod_config.agent_port, 'agent_port')
```

## zymod/zymod_config.py

```diff
@@ -23,15 +23,10 @@
         self.agent_host = ''
         self.agent_port = ''
         self.debug = ''
         self.dry_run = ''
         self.interval = ''
         self.token = ''
         self.host = ''
-        self.headers = ''
-        # self.unit = ''
-        self.chinese_name = ''
+        self.language_file = ''
+        self.display_name = ''
         self.mod_type = ''
-        # self.event_report = ''
-        # self.notice_report = ''
-        # self.alert_threshold = ''
-        # self.warning_threshold = ''
```

## zymod/ssl/zy_cert.py

```diff
@@ -34,25 +34,28 @@
     """
     不要在此设置字段默认值，限制用户必须使用__init__初始化ZyCert。
     否则，会出现类成员变量数据累加问题。而不是作为类实例成员变量，每次都将被初始化。
     """
     cert_path: str
     root_cert_path: str
     private_key_path: str
+    # RSA or ECDSA
+    private_key_type: str
     issued_to: IssuedTo
     issued_by: IssuedBy
     validity_period: ValidityPeriod
     subject_alt_name: SubjectAltName
     domain: str
 
     def asdict(self) -> dict:
         return {
             'Domain': self.domain,
             'Certificate Path': self.cert_path,
             'Private Key Path': self.private_key_path,
+            'Private Key Type': self.private_key_type,
             'Root Certificate Path': self.root_cert_path,
             'Certificate': {
                 'Issued To': {
                     'Common Name': self.issued_to.common_name,
                     'Organization': self.issued_to.organization,
                     'Organization Unit': self.issued_to.organization_unit,
                 },
@@ -63,11 +66,13 @@
                 },
                 'Subject Alternative Name': {
                     'DNS Names': self.subject_alt_name.dns_names
                 },
                 'Validity Period': {
                     'Issued On': self.validity_period.issued_on,
                     'Expires On': self.validity_period.expires_on,
-                    'Time Left': self.validity_period.time_left.asdict(),
+                    'Time Left': "%s天%s时%s分%s秒" % (
+                        self.validity_period.time_left.day, self.validity_period.time_left.hour,
+                        self.validity_period.time_left.minute, self.validity_period.time_left.second),
                 }
             }
         }
```

## zymod/ssl/zy_cert_validator.py

```diff
@@ -1,16 +1,18 @@
+import datetime
 from typing import Any
 
 from cryptography import x509
 from cryptography.exceptions import InvalidSignature
 from cryptography.x509 import Name, ObjectIdentifier, Certificate
+from cryptography.x509.extensions import ExtensionNotFound
 from cryptography.x509.oid import NameOID, ExtensionOID
 from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.asymmetric import padding
-from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric import padding, ec, utils
+from cryptography.hazmat.primitives import serialization, hashes
 from happy_python import HappyLog
 
 from zymod.event import ZyInternalEvent, ZyEventLevel
 from zymod.ssl import ZyCert
 from zymod.util import TimeDurationCalculator
 
 
@@ -26,46 +28,49 @@
     __cert_chain: Certificate = None
     __hlog = HappyLog.get_instance()
     __private_key: Any = None
 
     __cert_path: str = ''
     __root_cert_path: str = ''
     __private_key_path: str = ''
+    __private_key_type: str = ''
 
     def __init__(self, cert_path: str, root_cert_path: str, private_key_path: str):
         self.__cert_path = cert_path
         self.__root_cert_path = root_cert_path
         self.__private_key_path = private_key_path
 
     @staticmethod
     def __get_nameoid_value(name: Name, oid: ObjectIdentifier) -> str:
         r = name.get_attributes_for_oid(oid)
 
         # <未包含在证书中>
-        return r[0].value if r else "<Not Part of Certificate>"
+        return r[0].value if r else "<未包含在证书中>"
 
     @staticmethod
     def __load_cert_path(file: str, desc: str) -> Certificate:
         try:
             with open(file, 'rb') as f_handler:
                 return x509.load_pem_x509_certificate(data=f_handler.read(), backend=default_backend())
         except ValueError:
             raise ZyInternalEvent(level=ZyEventLevel.Alert,
                                   summary='SSL证书验证失败',
-                                  description='无效的%s文件：%s' % (desc, file))
+                                  description='无效的%s文件：%s' % (desc, file),
+                                  trigger="无效的SSL证书文件")
         except OSError as e:  # IsADirectoryError | FileNotFoundError | ...
             raise ZyInternalEvent(level=ZyEventLevel.Alert,
                                   summary='SSL证书验证失败',
-                                  description='载入%s文件时，出现系统错误：%s' % (desc, e))
+                                  description='载入%s文件时，出现系统错误：%s' % (desc, e),
+                                  trigger="无效的SSL证书文件")
 
     def __load_cert(self, file: str) -> None:
         self.__cert = self.__load_cert_path(file, 'SSL证书')
 
     def __load_root_cert(self, file: str) -> None:
-        self.__cert_chain = self.__load_cert_path(file, 'SSL证书密钥')
+        self.__cert_chain = self.__load_cert_path(file, 'SSL根证书')
 
     def __load_private_key(self) -> None:
         try:
             with open(self.__private_key_path, 'rb') as f_handler:
                 self.__private_key = serialization.load_pem_private_key(data=f_handler.read(),
                                                                         password=None,
                                                                         backend=default_backend())
@@ -76,14 +81,39 @@
                                   trigger='无效的SSL密钥文件')
         except OSError as e:  # IsADirectoryError | FileNotFoundError | ...
             raise ZyInternalEvent(level=ZyEventLevel.Alert,
                                   summary='SSL证书验证失败',
                                   description='载入SSL密钥文件时，出现系统错误：%s' % e,
                                   trigger='载入SSL密钥文件时，出现系统错误')
 
+    def __verify_rsa_signature(self, digest, cert_sign_hash_algo) -> None:
+        signature_algorithm = utils.Prehashed(cert_sign_hash_algo)
+
+        signature = self.__private_key.sign(data=digest,
+                                            padding=padding.PSS(
+                                                mgf=padding.MGF1(cert_sign_hash_algo),
+                                                salt_length=padding.PSS.MAX_LENGTH),
+                                            algorithm=signature_algorithm)
+
+        self.__cert.public_key().verify(signature=signature,
+                                        data=digest,
+                                        padding=padding.PSS(
+                                            mgf=padding.MGF1(cert_sign_hash_algo),
+                                            salt_length=padding.PSS.MAX_LENGTH),
+                                        algorithm=signature_algorithm)
+
+    def __verify_ecdsa_signature(self, digest, cert_sign_hash_algo) -> None:
+        signature_algorithm = ec.ECDSA(utils.Prehashed(cert_sign_hash_algo))
+
+        signature = self.__private_key.sign(data=digest,
+                                            signature_algorithm=signature_algorithm)
+        self.__cert.public_key().verify(signature=signature,
+                                        data=digest,
+                                        signature_algorithm=signature_algorithm)
+
     def __step1_verify_cert_files(self) -> None:
         """
         验证证书（公钥）文件和根证书文件（如fullchain.pem, chain.pem）
         :return:
         """
         self.__load_cert(self.__cert_path)
         self.__load_root_cert(self.__root_cert_path)
@@ -115,26 +145,30 @@
     def __step4_verify_signature(self) -> None:
         """
         验证签名
 
         完整执行一次明文->密文（签名字符串）->明文的加解密流程，验证证书和密钥是否匹配（如fullchain.pem+privkey.pem）
         :return:
         """
-        plain_text = b'Hello world!'
-
-        cipher_text = self.__private_key.sign(data=plain_text,
-                                              padding=padding.PKCS1v15(),
-                                              algorithm=self.__cert.signature_hash_algorithm)
+        chosen_hash = self.__cert.signature_hash_algorithm
+        hasher = hashes.Hash(chosen_hash)
+        hasher.update(b'Hello world!')
+        digest = hasher.finalize()
 
         try:
-            self.__cert.public_key().verify(
-                signature=cipher_text,
-                data=plain_text,
-                padding=padding.PKCS1v15(),
-                algorithm=self.__cert.signature_hash_algorithm)
+            # _EllipticCurvePrivateKey->ECDSA
+            # _RSAPrivateKey->RSA
+            private_key_type = type(self.__private_key).__name__
+
+            if private_key_type == '_EllipticCurvePrivateKey':
+                self.__private_key_type = 'ECDSA'
+                self.__verify_ecdsa_signature(digest, chosen_hash)
+            else:
+                self.__private_key_type = 'RSA'
+                self.__verify_rsa_signature(digest, chosen_hash)
         except InvalidSignature:
             raise ZyInternalEvent(level=ZyEventLevel.Alert,
                                   summary='SSL证书验证失败',
                                   description='签名验证失败，证书文件：%s，密钥文件：%s' % (self.__cert_path, self.__private_key_path),
                                   trigger='签名验证失败')
 
     def verify(self):
@@ -146,34 +180,41 @@
     def dump_formatted_data(self) -> ZyCert:
         """
         导出格式化后的证书数据
         :return:
         """
         assert self.__cert
 
-        subject_alt_name_oid_value = \
-            self.__cert.extensions.get_extension_for_oid(ExtensionOID.SUBJECT_ALTERNATIVE_NAME).value
+        dns_names: list[str] = list()
+        common_name = self.__get_nameoid_value(self.__cert.subject, NameOID.COMMON_NAME)
 
         try:
-            dns_names: list[str] = list()
+            subject_alt_name_oid_value = \
+                self.__cert.extensions.get_extension_for_oid(ExtensionOID.SUBJECT_ALTERNATIVE_NAME).value
+
             get_values_for_type_func = getattr(subject_alt_name_oid_value, 'get_values_for_type')
 
             for dns in get_values_for_type_func(x509.DNSName):
                 dns_names.append(dns)
         except AttributeError:
             assert False
+        except ExtensionNotFound:
+            # ExtensionOID.SUBJECT_ALTERNATIVE_NAME属性不存在
+            if len(dns_names) == 0:
+                dns_names.append(common_name)
 
-        time_duration = TimeDurationCalculator.calculate(self.__cert.not_valid_after, self.__cert.not_valid_before)
+        time_duration = TimeDurationCalculator.calculate(self.__cert.not_valid_after, datetime.datetime.utcnow())
 
         output = ZyCert(domain=dns_names[0],
                         cert_path=self.__cert_path,
                         root_cert_path=self.__root_cert_path,
                         private_key_path=self.__private_key_path,
+                        private_key_type=self.__private_key_type,
                         issued_to=ZyCert.IssuedTo(
-                            common_name=self.__get_nameoid_value(self.__cert.subject, NameOID.COMMON_NAME),
+                            common_name=common_name,
                             organization=self.__get_nameoid_value(self.__cert.subject, NameOID.ORGANIZATION_NAME),
                             organization_unit=self.__get_nameoid_value(self.__cert.subject,
                                                                        NameOID.ORGANIZATIONAL_UNIT_NAME)),
                         issued_by=ZyCert.IssuedBy(
                             common_name=self.__get_nameoid_value(self.__cert.issuer, NameOID.COMMON_NAME),
                             organization=self.__get_nameoid_value(self.__cert.issuer, NameOID.ORGANIZATION_NAME),
                             organization_unit=self.__get_nameoid_value(self.__cert.issuer,
```

## zymod/systemd/__init__.py

```diff
@@ -1,14 +1,17 @@
 from zymod.systemd.zy_systemd_unit_prop import ZySystemdUnitProp
 from zymod.systemd.zy_systemd_timer_prop import ZySystemdTimerProp
 from zymod.systemd.zy_systemd_manager import ZySystemdManager
 from zymod.systemd.zy_systemd_unit import ZySystemdUnit
 from zymod.systemd.zy_systemd_timer import ZySystemdTimer
-
+from zymod.systemd.zy_systemd_service import ZySystemdService
+from zymod.systemd.zy_systemd_service_prop import ZySystemdServiceProp
 
 __all__ = [
     'ZySystemdManager',
     'ZySystemdUnit',
     'ZySystemdUnitProp',
     'ZySystemdTimer',
     'ZySystemdTimerProp',
+    'ZySystemdService',
+    'ZySystemdServiceProp'
 ]
```

## zymod/systemd/zy_systemd_unit.py

```diff
@@ -1,11 +1,11 @@
 import dbus
 from happy_python import HappyLog
 
-from zymod.systemd import ZySystemdManager
+from zymod.systemd import ZySystemdManager, ZySystemdUnitProp
 
 
 class ZySystemdUnit:
     def __init__(self, name: str):
         self.hlog = HappyLog.get_instance()
         self.name = name
         self.manager = ZySystemdManager()
@@ -14,9 +14,19 @@
                                              object_path=self.manager.get_unit(self.name))
 
         self.interface_props = dbus.Interface(object=self.obj_timer,
                                               dbus_interface='org.freedesktop.DBus.Properties')
 
     def get_prop(self, name: str):
         props = self.interface_props.GetAll('org.freedesktop.systemd1.Unit')
-
         return props[name]
+
+    def get_props(self) -> ZySystemdUnitProp:
+        prop_list = self.manager.list_units()
+
+        for i in prop_list:
+            if i.primary_unit_name == self.name:
+                return ZySystemdUnitProp(active_state=i.active_state, desc=i.desc,
+                                         load_state=i.load_state, object_path=i.object_path,
+                                         primary_unit_name=i.primary_unit_name, sub_state=i.sub_state,
+                                         followed=i.followed,job_object_path=i.job_object_path,job_id=i.job_id,
+                                         job_type=i.job_type)
```

## zymod/util/__init__.py

```diff
@@ -1,7 +1,9 @@
 from zymod.util.time_duration_calculator import TimeDuration
 from zymod.util.time_duration_calculator import TimeDurationCalculator
+from zymod.util.dbus_utils import cmd_array_to_str
 
 __all__ = [
     'TimeDuration',
     'TimeDurationCalculator',
+    'cmd_array_to_str'
 ]
```

## zymod_help/version.txt

```diff
@@ -1 +1 @@
-0.0.1.20
+0.0.1.26
```

## Comparing `zymod-0.0.1.20.dist-info/LICENSE` & `zymod-0.0.1.26.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zymod-0.0.1.20.dist-info/RECORD` & `zymod-0.0.1.26.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 zymod/__init__.py,sha256=ik-iCc45prp7G7pfjYHaLQoWwXJoKCBerHUhm6DRFYE,271
-zymod/zymod.py,sha256=RnHdq9aOMUZQM55tQ-ZBLPKAsQ4o0vJlCHcHQk7jW-o,21485
-zymod/zymod_config.py,sha256=j8KnJVcxVbgKXAhPux5K7FEhKoyW8V8kM-FTWM4QKEk,1013
+zymod/zymod.py,sha256=Vebo8D-OVKRoG5-S2gd6nIws35yX7qNqTi5672p8EEs,22555
+zymod/zymod_config.py,sha256=ACLz7pXxE5I7a7X-113Yi91MVo3_UlaaMP65g5IIFFM,853
 zymod/event/__init__.py,sha256=_jHTCIRENwxwn-hVoWGopkVuzOXEBaR1TYc2OFYNX0M,174
 zymod/event/zy_event_level_enum.py,sha256=HIDEIYR2UdC1X-7HO7nFxGJ77dz0qbRtisT5RIsaoRQ,117
 zymod/event/zy_internal_event.py,sha256=Efm3NHfPwFMDNsoVdaxW27FIcNcfNxfpM8kJe61crY0,718
 zymod/inotify/__init__.py,sha256=iCyvryAHBBxMeNq2hOIos5Ac_yoEUK4TVoFKMOo7yjU,192
 zymod/inotify/zy_file_event_enum.py,sha256=dGteZep_BI08VptspOcmBmGUYDW3v4jMxmHmYB4xDQs,611
 zymod/inotify/zy_inotify_file_event.py,sha256=_S5R9VCTZlqy6Vct8jJDJflPjMBtvTd5jsbitJz0Lbo,2265
 zymod/ssl/__init__.py,sha256=2iP1syFGXUfy0PNXGN3zOMPOR6NyIhN6SiLHJ4Gxn0A,145
-zymod/ssl/zy_cert.py,sha256=6IjM_vVyLNVlXFwiYX-Hfy30cAnPv68wzZ4CscLEqWw,2243
-zymod/ssl/zy_cert_validator.py,sha256=XCORKtmKq12aNN_zO8I1qIy-uKmZcHNcobkkC5cvTrM,8560
-zymod/systemd/__init__.py,sha256=3UW4foCTl2WKVpdruPAgA-uJ_Lj0b8ppbE8lr1i3NEk,442
+zymod/ssl/zy_cert.py,sha256=YxmUB1J2z22WDKE3AkYr7ahRbQ3AdjbLEubNJeevvdk,2529
+zymod/ssl/zy_cert_validator.py,sha256=XrRYksyql2j_B9ahKAqbqrpMSM7wR6iClBd9-3Tfgvc,10663
+zymod/systemd/__init__.py,sha256=ZaajYNhdQ8JxHEhzOJUCgOAfP8jui-c9Elwv7_udlTQ,625
 zymod/systemd/zy_systemd_manager.py,sha256=NvO9BjMJDvFfd_tB-Bxr1MDACSzsSGPMKNCJTT-DKgQ,1943
+zymod/systemd/zy_systemd_service.py,sha256=jg7vMNSCWbPdsNxrfvxG6KuX_2utcQrdNwPgOPwppwM,1505
+zymod/systemd/zy_systemd_service_prop.py,sha256=A1dLGzT9oFMpFPZTFTVMF5A7KUbNVwMoBbEgB8UmuYw,441
 zymod/systemd/zy_systemd_timer.py,sha256=FsGIg_JwyytdkCtIKxMCbRZNwhx8njg179R7yCETC14,3442
 zymod/systemd/zy_systemd_timer_prop.py,sha256=Qa6y42GsXGX4caoDcrTHXLOc0hAxyTNUNf6fQMsc5Ec,560
-zymod/systemd/zy_systemd_unit.py,sha256=UQfdJ6YihfwFlnSihWyYW7lX0BYCF2x7gNHeB9-bDm0,775
+zymod/systemd/zy_systemd_unit.py,sha256=qFwTLn8ajFT3MTK3wuYG2GfsjsGntpbXbTughvQY-0o,1417
 zymod/systemd/zy_systemd_unit_prop.py,sha256=ir6YE1qVGhtOcsGrxeOionhZSwod6vMO0xWjEkwF5Zc,505
-zymod/util/__init__.py,sha256=iMEh7D6vLSOYf3L6PMlm6iMrOJubOATsdZMl-afzNUs,197
+zymod/util/__init__.py,sha256=XG-oPm6WT185qkR1blxnZE8864DtVLEtphnmhFgKB2U,271
+zymod/util/dbus_utils.py,sha256=IQ2wEIY2j0K5jHpBSxHkdbbG31N3xqp5a6FmUWjVmYU,449
 zymod/util/time_duration_calculator.py,sha256=AA-FV5wJbQB22CGubkqVfDEgHnBaoZiLQBzeUZPQsJY,2087
-zymod_help/version.txt,sha256=omm2F-cFZnBLkfndCVZN9cOjbN4Ut7wOv9m0IWh1698,8
-zymod-0.0.1.20.dist-info/LICENSE,sha256=NrK0nvgt_x7V38ZcVzPA06RWRUyUMGdWba9i1-svAO0,1072
-zymod-0.0.1.20.dist-info/METADATA,sha256=WraxR8EWJhuZgdzxoV_p84jGqIuLduLmBfFW8kJlQfg,4932
-zymod-0.0.1.20.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-zymod-0.0.1.20.dist-info/top_level.txt,sha256=988RU54rZF6ShPstgA4AvJekX8bc4mw_smYNge0m_-k,17
-zymod-0.0.1.20.dist-info/RECORD,,
+zymod/zyapp_service/__init__.py,sha256=FO0CKNs7-KyaODN8XLGtFicLQZ_Wl5WgBAkkF-ngzxI,169
+zymod/zyapp_service/service.py,sha256=2m13Vvwh8DD1h3ktTid_lNUdxUwZamg9L8brF8zRHQU,7747
+zymod/zyprocfs/__init__.py,sha256=usq8EHhHuPoZFb7-CK4gIlaenSjUQnLuBgOJADK38oA,144
+zymod/zyprocfs/procfs.py,sha256=4Zkqo0lTNTlZDM0bENuHP0NRSSw_9-9rpfRaBdD7CJw,909
+zymod_help/version.txt,sha256=r1B0fQJ0yZqPgl_qMF2W-ajP0ZQA7wtNNQD5W8eY8XE,8
+zymod-0.0.1.26.dist-info/LICENSE,sha256=NrK0nvgt_x7V38ZcVzPA06RWRUyUMGdWba9i1-svAO0,1072
+zymod-0.0.1.26.dist-info/METADATA,sha256=VvWF0mze-G5GHjGdJX6XLzm9U93CNSx8rBHllqODg9A,2070
+zymod-0.0.1.26.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+zymod-0.0.1.26.dist-info/top_level.txt,sha256=988RU54rZF6ShPstgA4AvJekX8bc4mw_smYNge0m_-k,17
+zymod-0.0.1.26.dist-info/RECORD,,
```

