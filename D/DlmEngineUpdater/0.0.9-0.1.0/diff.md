# Comparing `tmp/DlmEngineUpdater-0.0.9.tar.gz` & `tmp/DlmEngineUpdater-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DlmEngineUpdater-0.0.9.tar", last modified: Mon Sep  5 08:05:31 2022, max compression
+gzip compressed data, was "DlmEngineUpdater-0.1.0.tar", last modified: Wed Aug  2 09:04:35 2023, max compression
```

## Comparing `DlmEngineUpdater-0.0.9.tar` & `DlmEngineUpdater-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)        0 2022-09-05 08:05:31.682857 DlmEngineUpdater-0.0.9/
-drwxr-xr-x   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)        0 2022-09-05 08:05:31.677084 DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)      751 2022-09-05 08:05:31.000000 DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/PKG-INFO
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)      309 2022-09-05 08:05:31.000000 DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/SOURCES.txt
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)        1 2022-09-05 08:05:31.000000 DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/dependency_links.txt
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)       23 2022-09-05 08:05:31.000000 DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/requires.txt
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)       19 2022-09-05 08:05:31.000000 DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/top_level.txt
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)     1084 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.0.9/LICENSE.txt
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)       56 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.0.9/MANIFEST.in
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)      751 2022-09-05 08:05:31.683697 DlmEngineUpdater-0.0.9/PKG-INFO
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)     4513 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.0.9/README.md
-drwxr-xr-x   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)        0 2022-09-05 08:05:31.678786 DlmEngineUpdater-0.0.9/contrib/
--rwxr-xr-x   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)       98 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.0.9/contrib/dlm_engine_updater
-drwxr-xr-x   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)        0 2022-09-05 08:05:31.680827 DlmEngineUpdater-0.0.9/dlm_engine_updater/
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)    18942 2022-09-05 08:04:31.000000 DlmEngineUpdater-0.0.9/dlm_engine_updater/__init__.py
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)       67 2022-09-05 08:05:31.687475 DlmEngineUpdater-0.0.9/setup.cfg
--rw-r--r--   0 sschultchen (229327392) GREENWICH\Domain Users (795678076)     1102 2022-09-05 07:57:57.000000 DlmEngineUpdater-0.0.9/setup.py
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      750 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/PKG-INFO
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      309 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/SOURCES.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)        1 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/dependency_links.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       23 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/requires.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       19 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/top_level.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     1084 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/LICENSE.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       56 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/MANIFEST.in
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      750 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/PKG-INFO
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     4513 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/README.md
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/contrib/
+-rwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)       98 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/contrib/dlm_engine_updater
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/dlm_engine_updater/
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)    20373 2023-08-02 09:04:26.000000 DlmEngineUpdater-0.1.0/dlm_engine_updater/__init__.py
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       67 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/setup.cfg
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     1102 2023-08-02 07:17:39.000000 DlmEngineUpdater-0.1.0/setup.py
```

### Comparing `DlmEngineUpdater-0.0.9/DlmEngineUpdater.egg-info/PKG-INFO` & `DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DlmEngineUpdater
-Version: 0.0.9
+Version: 0.1.0
 Summary: DlmEngine, distributed lock implementation on top of MongoDB and Redis
 Home-page: https://github.com/schlitzered/DlmEngineUpdater
 Author: schlitzer
 Author-email: stephan.schultchen@gmail.com
 License: MIT
 Keywords: dlm,distributes lock engine updater
 Platform: posix
@@ -13,12 +13,11 @@
 License-File: LICENSE.txt
 
 
 DLMEngine implements a restful interface that can be used to implement distributed locks.
 
 The main intention was to orchestrate automated system updates, so only one server at a time will do a update.
 
-Copyright (c) 2019, Stephan Schultchen.
+Copyright (c) 2023, Stephan Schultchen.
 
 License: MIT (see LICENSE for details)
     
-
```

### Comparing `DlmEngineUpdater-0.0.9/LICENSE.txt` & `DlmEngineUpdater-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DlmEngineUpdater-0.0.9/PKG-INFO` & `DlmEngineUpdater-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DlmEngineUpdater
-Version: 0.0.9
+Version: 0.1.0
 Summary: DlmEngine, distributed lock implementation on top of MongoDB and Redis
 Home-page: https://github.com/schlitzered/DlmEngineUpdater
 Author: schlitzer
 Author-email: stephan.schultchen@gmail.com
 License: MIT
 Keywords: dlm,distributes lock engine updater
 Platform: posix
@@ -13,12 +13,11 @@
 License-File: LICENSE.txt
 
 
 DLMEngine implements a restful interface that can be used to implement distributed locks.
 
 The main intention was to orchestrate automated system updates, so only one server at a time will do a update.
 
-Copyright (c) 2019, Stephan Schultchen.
+Copyright (c) 2023, Stephan Schultchen.
 
 License: MIT (see LICENSE for details)
     
-
```

### Comparing `DlmEngineUpdater-0.0.9/README.md` & `DlmEngineUpdater-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `DlmEngineUpdater-0.0.9/dlm_engine_updater/__init__.py` & `DlmEngineUpdater-0.1.0/dlm_engine_updater/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,389 +13,464 @@
 from logging.handlers import TimedRotatingFileHandler
 
 from pep3143daemon import PidFile
 import requests
 
 
 def main():
-    parser = argparse.ArgumentParser(description="DLM Updater Updater")
+    parser = argparse.ArgumentParser(description="DLM Updater")
 
-    parser.add_argument("--cfg", dest="cfg", action="store",
-                        default="/etc/dlm_engine_updater/config.ini",
-                        help="Full path to configuration")
-
-    parser.add_argument("--after_reboot", dest="rbt", action="store_true",
-                        default=False,
-                        help="has to be used from init systems, to indicated that the script was called while booting.")
-
-    parser.add_argument("--date_constraint", dest="date_constraint", action="store",
-                        default=None,
-                        help="exit if date constraint is not fulfilled."
-                             "example value: 3:Friday"
-                             "would only run if this is the 3rd Friday of a month."
-                        )
-
-    parser.add_argument("--random_sleep", dest="random_sleep", action="store", required=False,
-                        default=0, type=int,
-                        help="add random sleep before acutally doing something"
-                        )
+    parser.add_argument(
+        "--cfg",
+        dest="cfg",
+        action="store",
+        default="/etc/dlm_engine_updater/config.ini",
+        help="Full path to configuration",
+    )
+
+    parser.add_argument(
+        "--after_reboot",
+        dest="rbt",
+        action="store_true",
+        default=False,
+        help="has to be used from init systems, to indicate that the script was called while booting.",
+    )
+
+    parser.add_argument(
+        "--date_constraint",
+        dest="date_constraint",
+        action="store",
+        default=None,
+        help="exit if date constraint is not fulfilled."
+        "example value: 3:Friday"
+        "would only run if this is the 3rd Friday of a month.",
+    )
+
+    parser.add_argument(
+        "--random_sleep",
+        dest="random_sleep",
+        action="store",
+        required=False,
+        default=0,
+        type=int,
+        help="add random sleep before acutally doing something",
+    )
 
     parsed_args = parser.parse_args()
 
     instance = DlmEngineUpdater(
         cfg=parsed_args.cfg,
         after_reboot=parsed_args.rbt,
         date_constraint=parsed_args.date_constraint,
-        random_sleep=parsed_args.random_sleep
+        random_sleep=parsed_args.random_sleep,
     )
     instance.work()
 
 
 class DlmEngineLock(object):
-    def __init__(self, log, lock_name, ca, secret, secret_id, endpoint, wait, wait_max):
+    def __init__(self, log, lock_name, ca, secret, secret_id, endpoint, wait, wait_max, org_id):
+        self._api_version = None
         self._ca = ca
-        self._secret = secret
-        self._secret_id = secret_id
         self._endpoint = endpoint
         self._lock_name = lock_name
+        self._org_id = org_id
+        self._secret = secret
+        self._secret_id = secret_id
+        self._session = None
         self._wait = wait
         self._wait_max = wait_max
         self.log = log
 
     @property
+    def api_version(self):
+        if not self._api_version:
+            url = f"{self.endpoint}/versions"
+            resp = self.session.get(
+                url=url,
+            )
+            if resp.status_code == 404:
+                self._api_version = "1"
+            else:
+                for version in resp.json()['versions']:
+                    if not self._api_version:
+                        self._api_version = version['version']
+                    elif version['version'] > self._api_version:
+                        self._api_version = version['version']
+        return self._api_version
+
+    @property
     def ca(self):
         return self._ca
 
     @property
+    def endpoint(self):
+        if self._endpoint.endswith('/api/v1/'):
+            return self._endpoint[:-8]
+        return self._endpoint
+
+    @property
+    def org_id(self):
+        return self._org_id
+
+    @property
     def secret(self):
         return self._secret
 
     @property
     def secret_id(self):
         return self._secret_id
 
     @property
-    def endpoint(self):
-        return self._endpoint
+    def session(self):
+        if not self._session:
+            self._session = requests.Session()
+            self._session.headers = {
+                "x-id": self.secret_id,
+                "x-secret-id": self.secret_id,
+                "x-secret": self.secret
+            }
+            self._session.verify = self.ca
+        return self._session
 
     @property
     def lock_name(self):
         return self._lock_name
 
     @property
+    def payload_acquire(self):
+        if self.api_version == "1":
+            return {"data": {"acquired_by": socket.getfqdn()}}
+        elif self.api_version == "2":
+            return {"acquired_by": socket.getfqdn()}
+
+    def payload_release(self):
+        if self.api_version == "1":
+            return {"data": {"acquired_by": socket.getfqdn()}}
+
+    @property
     def wait(self):
         return self._wait
 
     @property
     def wait_max(self):
         return self._wait_max
 
     @property
     def lock_url(self):
-        return "{0}locks/{1}".format(self._endpoint, self.lock_name)
+        if self.api_version == "1":
+            return f"{self.endpoint}/api/v1/locks/{self.lock_name}"
+        elif self.api_version == "2":
+            return f"{self.endpoint}/api/v2/orgs/{self.org_id}/locks/{self.lock_name}"
+        else:
+            self.log.fatal(f"unsupported api version: {self.api_version}")
+            sys.exit(1)
 
     def acquire(self):
         # todo check if lock is already acquired
-        self.log.debug("waiting is set to {0}".format(self.wait))
-        self.log.debug("max wait time is set to {0}".format(self.wait_max))
+        self.log.debug(f"waiting is set to {self.wait}")
+        self.log.debug(f"max wait time is set to {self.wait_max}")
         if self.wait:
             _waited = 0
             while True:
                 if self._acquire():
-                    self.log.error("blarg")
                     return
                 else:
                     if _waited > self.wait_max:
                         self.log.error("exceeded max wait time, quiting")
                         sys.exit(1)
                     _sleep = random.randint(10, 60)
                     _waited += _sleep + 2
-                    self.log.error("sleeping {0} seconds".format(_sleep))
+                    self.log.error(f"sleeping {_sleep} seconds")
                     time.sleep(_sleep)
         else:
             if not self._acquire():
                 self.log.error("quiting")
                 sys.exit(1)
 
     def _acquire(self):
-        self.log.info("trying to acquire: {0}".format(self.lock_url))
+        self.log.info(f"trying to acquire: {self.lock_url}")
+        if self._acquire_check():
+            return True
         try:
-            resp = requests.post(
-                json={
-                    "data": {
-                        "acquired_by": socket.getfqdn()
-                    }
-                },
-                headers={
-                    'x-id': self.secret_id,
-                    'x-secret': self.secret
-                },
+            resp = self.session.post(
+                json=self.payload_acquire,
                 timeout=10.0,
                 url=self.lock_url,
-                verify=self.ca
             )
-            self.log.debug("http status_code is: {0}".format(resp.status_code))
-            self.log.debug("http_response is {0}".format(resp.json()))
+            self.log.debug(f"http status_code is: {resp.status_code}")
+            self.log.debug(f"http_response is {resp.json()}")
             if resp.status_code == 201:
                 self.log.info("success acquiring lock")
                 return True
             else:
-                self.log.error("could not acquire lock: {0}".format(resp.json()))
+                self.log.error(f"could not acquire lock: {resp.json()}")
                 return False
         except requests.RequestException as err:
-            self.log.error("request error: {0}".format(err))
+            self.log.error(f"request error: {err}")
+
+    def _acquire_check(self):
+        self.log.info("checking if lock has been acquired")
+        resp = self.session.get(
+            json=self.payload_acquire,
+            timeout=10.0,
+            url=self.lock_url,
+        )
+        if not resp.status_code == 200:
+            self.log.info("lock currently not present in the system")
+            return
+
+        if not resp.json()['acquired_by'] == socket.getfqdn():
+            self.log.info(f"lock is currently acquired by {resp.json()['acquired_by']}")
+            return
+
+        self.log.info("lock has been already acquired by this instance")
+        return True
 
     def release(self):
-        self.log.info("trying to release: {0}".format(self.lock_url))
+        self.log.info(f"trying to release: {self.lock_url}")
         retries = 10
         while retries > 0:
             try:
-                resp = requests.delete(
-                    json={
-                        "data": {
-                            "acquired_by": socket.getfqdn()
-                        }
-                    },
-                    headers={
-                        'x-id': self.secret_id,
-                        'x-secret': self.secret
-                    },
-                    timeout=2.0,
+                resp = self.session.delete(
+                    json=self.payload_release(),
+                    timeout=10.0,
                     url=self.lock_url,
-                    verify=self.ca
                 )
-                self.log.debug("http status_code is: {0}".format(resp.status_code))
-                self.log.debug("http_response is {0}".format(resp.json()))
+                self.log.debug(f"http status_code is: {resp.status_code}")
+                self.log.debug(f"http_response is {resp.json()}")
                 if resp.status_code == 200:
                     self.log.info("success releasing lock")
                     return
                 else:
-                    self.log.error("could not release lock: {0}".format(resp.json()))
+                    self.log.error(f"could not release lock: {resp.json()}")
                     sys.exit(1)
             except requests.RequestException as err:
-                self.log.error("connection error, retrying: {0}".format(err))
+                self.log.error(f"connection error, retrying: {err}")
                 retries -= 1
                 time.sleep(5)
         self.log.fatal("could not release lock")
         sys.exit(1)
 
 
 class DlmEngineUpdater(object):
     def __init__(self, cfg, after_reboot, date_constraint, random_sleep):
         self._config_file = cfg
         self._config = configparser.ConfigParser()
         self._config_dict = None
         self._after_reboot = after_reboot
         self._date_constraint = None
         self._random_sleep = random_sleep
-        self.log = logging.getLogger('application')
+        self.log = logging.getLogger("application")
         self.config.read_file(open(self._config_file))
         self._logging()
-        self._lock = PidFile(self.config.get('main', 'lock'))
+        self._lock = PidFile(self.config.get("main", "lock"))
         self.date_constraint = date_constraint
         self._dlm_lock = DlmEngineLock(
             log=self.log,
-            ca=self.config.get('main', 'ca', fallback=None),
-            endpoint=self.config.get('main', 'endpoint'),
-            secret=self.config.get('main', 'secret'),
-            secret_id=self.config.get('main', 'secret_id'),
-            lock_name=self.config.get('main', 'lock_name'),
-            wait=self.config.getboolean('main', 'wait', fallback=False),
-            wait_max=self.config.getint('main', 'wait_max', fallback=3600),
+            ca=self.config.get("main", "ca", fallback=None),
+            endpoint=self.config.get("main", "endpoint"),
+            org_id=self.config.get("main", "org_id", fallback='DLMUpdater'),
+            secret=self.config.get("main", "secret"),
+            secret_id=self.config.get("main", "secret_id"),
+            lock_name=self.config.get("main", "lock_name"),
+            wait=self.config.getboolean("main", "wait", fallback=False),
+            wait_max=self.config.getint("main", "wait_max", fallback=3600),
         )
-        self._dlm_lock_aquired = False
+        self._dlm_lock_acquired = False
 
     @property
     def config(self):
         return self._config
 
     @property
     def date_constraint(self):
         return self._date_constraint
 
     @date_constraint.setter
     def date_constraint(self, value):
         if not value:
             return
         try:
-            nth, day = value.split(':', maxsplit=1)
+            nth, day = value.split(":", maxsplit=1)
         except ValueError:
             self.log.fatal("Invalid date constraint, must match NUM:DAY_ABBR")
             sys.exit(1)
         try:
             nth = int(nth)
         except ValueError:
             self.log.fatal("Invalid date constraint, number must be between 1 and 4")
             sys.exit(1)
         if nth not in range(1, 5):
             self.log.fatal("Invalid date constraint, number must be between 1 and 4")
             sys.exit(1)
         if day not in calendar.day_abbr:
-            self.log.fatal("Invalid date constraint, day must be one of {0}".format(list(calendar.day_abbr)))
+            self.log.fatal(
+                f"Invalid date constraint, day must be one of {list(calendar.day_abbr)}"
+            )
             sys.exit(1)
-        self._date_constraint = {'nth': nth, 'day': day}
+        self._date_constraint = {"nth": nth, "day": day}
 
     @property
     def dlm_lock(self):
         return self._dlm_lock
 
     @property
     def dlm_lock_acquired(self):
-        return self._dlm_lock_aquired
+        return self._dlm_lock_acquired
 
     @dlm_lock_acquired.setter
     def dlm_lock_acquired(self, value):
-        self._dlm_lock_aquired = value
+        self._dlm_lock_acquired = value
 
     @property
     def lock(self):
         return self._lock
 
     @property
     def after_reboot(self):
         return self._after_reboot
 
     def _logging(self):
-        logfmt = logging.Formatter('%(asctime)sUTC - %(levelname)s - %(threadName)s - %(message)s')
+        logfmt = logging.Formatter(
+            "%(asctime)sUTC - %(levelname)s - %(threadName)s - %(message)s"
+        )
         logfmt.converter = time.gmtime
         handlers = []
-        aap_level = self.config.get('main', 'log_level')
-        log = self.config.get('main', 'log')
-        retention = self.config.getint('main', 'log_retention')
-        handlers.append(TimedRotatingFileHandler(log, 'd', 1, retention))
+        aap_level = self.config.get("main", "log_level")
+        log = self.config.get("main", "log")
+        retention = self.config.getint("main", "log_retention")
+        handlers.append(TimedRotatingFileHandler(log, "d", 1, retention))
 
         for handler in handlers:
             handler.setFormatter(logfmt)
             self.log.addHandler(handler)
         self.log.setLevel(aap_level)
         self.log.debug("logger is up")
 
     def random_sleep(self):
         sleep = random.randint(0, self._random_sleep)
-        self.log.info("sleeping {0} seconds".format(sleep))
+        self.log.info(f"sleeping {sleep} seconds")
         time.sleep(sleep)
-        self.log.info("sleeping {0} seconds,done ".format(sleep))
+        self.log.info(f"sleeping {sleep} seconds,done ")
 
     def execute_shell(self, args):
-        p = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+        p = subprocess.Popen(
+            args,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            universal_newlines=True,
+        )
         for line in p.stdout:
             self.log.info(line.rstrip())
         p.stdout.close()
         return p.wait()
 
     @property
     def task(self):
         try:
-            with open(self.config.get('main', 'state'), 'r') as state:
+            with open(self.config.get("main", "state"), "r") as state:
                 return state.readline().rstrip("\n")
         except FileNotFoundError:
-            return 'needs_update'
+            return "needs_update"
 
     @task.deleter
     def task(self):
         try:
-            os.remove(self.config.get('main', 'state'))
+            os.remove(self.config.get("main", "state"))
         except OSError as err:
-            self.log.error("could not remove state file: {0}".format(err))
+            self.log.error(f"could not remove state file: {err}")
 
     @task.setter
     def task(self, task):
-        self.log.info("setting task to {0}".format(task))
+        self.log.info(f"setting task to {task}")
         try:
-            with open(self.config.get('main', 'state'), 'w') as state:
-                state.write("{0}\n".format(task))
+            with open(self.config.get("main", "state"), "w") as state:
+                state.write(f"{task}\n")
         except OSError as err:
-            self.log.fatal("could not set state: {0}".format(err))
+            self.log.fatal(f"could not set state: {err}")
             sys.exit(1)
 
     def check_date_constraint(self):
         if not self.date_constraint:
             self.log.info("no date constraint set")
             return
-        self.log.info("date constraint set to {0}. {1}".format(
-            self.date_constraint['nth'],
-            self.date_constraint['day']
-        ))
+        self.log.info(
+            f"date constraint set to {self.date_constraint['nth']}. {self.date_constraint['day']}"
+        )
         now = datetime.datetime.now()
         month_start = datetime.datetime(year=now.year, month=now.month, day=1)
         delta = now - month_start
-        if now.strftime("%a") != self.date_constraint['day']:
-            self.log.fatal("today is not {0}".format(
-                self.date_constraint['day']
-            ))
+        if now.strftime("%a") != self.date_constraint["day"]:
+            self.log.fatal(f"today is not {self.date_constraint['day']}")
+            sys.exit(1)
         nth_count = 0
         for i in range(1, delta.days + 2):
             _day = datetime.datetime(year=now.year, month=now.month, day=i)
-            if _day.strftime("%a") == self.date_constraint['day']:
+            if _day.strftime("%a") == self.date_constraint["day"]:
                 nth_count += 1
-        if nth_count != self.date_constraint['nth']:
-            self.log.fatal("today is not the {0}. {1}".format(
-                self.date_constraint['nth'],
-                self.date_constraint['day']
-            ))
+        if nth_count != self.date_constraint["nth"]:
+            self.log.fatal(
+                f"today is not the {self.date_constraint['nth']}. {self.date_constraint['day']}"
+            )
             sys.exit(1)
-        self.log.fatal("today is the {0}. {1}, running dlm_engine_updater".format(
-            self.date_constraint['nth'],
-            self.date_constraint['day']
-        ))
+        self.log.fatal(
+            f"today is the {self.date_constraint['nth']}. {self.date_constraint['day']}, running dlm_engine_updater"
+        )
         return True
 
     def check_reboot(self):
         if self.after_reboot:
-            if self.task != 'post_update':
+            if self.task != "post_update":
                 self.log.info("reboot was not triggered by dlm_engine_updater, exiting")
                 sys.exit(0)
             else:
-                self.log.info("reboot was triggered by dlm_engine_updater, picking up remaining tasks")
+                self.log.info(
+                    "reboot was triggered by dlm_engine_updater, picking up remaining tasks"
+                )
 
     def dlm_lock_get(self):
         self.dlm_lock.acquire()
         self.dlm_lock_acquired = True
-        self.do_ext_notify(
-            phase='main',
-            script='none',
-            return_code=0
-        )
+        self.do_ext_notify(phase="main", script="none", return_code=0)
         self.task = "pre_update"
 
     def dlm_lock_release(self):
         self.log.info("releasing lock")
         self.dlm_lock.release()
         self.dlm_lock_acquired = False
         self.do_ext_notify(
-            phase='main',
-            script='none',
-            return_code=0,
-            updater_running=False
+            phase="main", script="none", return_code=0, updater_running=False
         )
         del self.task
         sys.exit(0)
 
     def do_ext_notify(self, phase, script, return_code, updater_running=True):
-        files = self.get_scripts('ext_notify.d')
+        files = self.get_scripts("ext_notify.d")
         for _file in files:
-            self.log.info("running ext notify script: {0}".format(_file))
-            self.execute_shell([
-                _file,
-                self.dlm_lock.lock_name,
-                str(self._dlm_lock_aquired),
-                str(updater_running),
-                phase,
-                script,
-                str(return_code)
-            ])
+            self.log.info(f"running ext notify script: {_file}")
+            self.execute_shell(
+                [
+                    _file,
+                    self.dlm_lock.lock_name,
+                    str(self.dlm_lock_acquired),
+                    str(updater_running),
+                    phase,
+                    script,
+                    str(return_code),
+                ]
+            )
 
     def get_scripts(self, path):
-        _path = self.config.get('main', path)
+        _path = self.config.get("main", path)
         files = list()
         candidates = os.listdir(_path)
         candidates.sort()
         for _file in candidates:
             _file = os.path.join(_path, _file)
-            self.log.debug("found the file: {0}".format(_file))
+            self.log.debug(f"found the file: {_file}")
             if not os.path.isfile(_file):
                 continue
             if not os.stat(_file).st_uid == 0:
                 self.log.warning("file not owned by root")
                 continue
             if os.stat(_file).st_mode & stat.S_IXUSR != 64:
                 self.log.warning("file not executable by root")
@@ -408,115 +483,100 @@
                 continue
             files.append(_file)
         return files
 
     def needs_update(self):
         update = False
         self.log.info("checking if updates are available")
-        files = self.get_scripts('needs_update.d')
+        files = self.get_scripts("needs_update.d")
         for _file in files:
-            self.log.info("running: {0}".format(_file))
+            self.log.info(f"running: {_file}")
             return_code = self.execute_shell([_file])
             if return_code != 0:
                 self.log.info("updates are available")
                 update = True
             self.do_ext_notify(
-                phase='needs_update',
-                script=_file,
-                return_code=return_code
+                phase="needs_update", script=_file, return_code=return_code
             )
-            self.log.info("running: {0} done".format(_file))
+            self.log.info(f"running: {_file} done")
         if update:
             self.task = "lock_get"
         else:
             self.log.info("no updates available")
             self.do_ext_notify(
-                phase='main',
-                script='none',
-                return_code=0,
-                updater_running=False
+                phase="main", script="none", return_code=0, updater_running=False
             )
             sys.exit(0)
 
     def update(self):
         self.log.info("running_update scripts")
-        files = self.get_scripts('update.d')
+        files = self.get_scripts("update.d")
         for _file in files:
-            self.log.info("running: {0}".format(_file))
+            self.log.info(f"running: {_file}")
             return_code = self.execute_shell([_file])
             if return_code != 0:
                 self.log.info("script failed, stopping, keeping lock")
                 sys.exit(1)
-            self.do_ext_notify(
-                phase='update',
-                script=_file,
-                return_code=return_code
-            )
-            self.log.info("running: {0} done".format(_file))
+            self.do_ext_notify(phase="update", script=_file, return_code=return_code)
+            self.log.info(f"running: {_file} done")
         self.task = "needs_reboot"
 
     def post_update(self):
         self.log.info("running post_update scripts")
         self.dlm_lock_acquired = True
-        files = self.get_scripts('post_update.d')
+        files = self.get_scripts("post_update.d")
         for _file in files:
-            self.log.info("running: {0}".format(_file))
+            self.log.info(f"running: {_file}")
             return_code = self.execute_shell([_file])
             if return_code != 0:
                 self.log.info("script failed, stopping, keeping lock")
                 sys.exit(1)
             self.do_ext_notify(
-                phase='post_update',
-                script=_file,
-                return_code=return_code
+                phase="post_update", script=_file, return_code=return_code
             )
-            self.log.info("running: {0} done".format(_file))
+            self.log.info(f"running: {_file} done")
         self.task = "lock_release"
 
     def pre_update(self):
         self.log.info("running pre_update scripts")
-        files = self.get_scripts('pre_update.d')
+        files = self.get_scripts("pre_update.d")
         for _file in files:
-            self.log.info("running: {0}".format(_file))
+            self.log.info(f"running: {_file}")
             return_code = self.execute_shell([_file])
             if return_code != 0:
                 self.log.info("script failed, stopping, keeping lock")
                 sys.exit(1)
             self.do_ext_notify(
-                phase='pre_update',
-                script=_file,
-                return_code=return_code
+                phase="pre_update", script=_file, return_code=return_code
             )
-            self.log.info("running: {0} done".format(_file))
+            self.log.info(f"running: {_file} done")
         self.task = "update"
 
     def reboot(self):
         self.log.info("rebooting")
         self.task = "post_update"
-        sys.exit(self.execute_shell([self.config.get('main', 'reboot_cmd')]))
+        sys.exit(self.execute_shell([self.config.get("main", "reboot_cmd")]))
 
     def needs_reboot(self):
         self.log.info("running needs reboot scripts")
         reboot = True
-        files = self.get_scripts('needs_reboot.d')
+        files = self.get_scripts("needs_reboot.d")
         for _file in files:
-            self.log.info("running: {0}".format(_file))
+            self.log.info(f"running: {_file}")
             return_code = self.execute_shell([_file])
             if return_code != 0:
-                self.log.info("running: {0} done".format(_file))
+                self.log.info(f"running: {_file} done")
                 self.do_ext_notify(
-                    phase='needs_reboot',
-                    script=_file,
-                    return_code=return_code
+                    phase="needs_reboot", script=_file, return_code=return_code
                 )
                 reboot = True
                 break
             else:
                 reboot = False
-            self.log.info("running: {0} done".format(_file))
+            self.log.info(f"running: {_file} done")
         if reboot:
             self.task = "reboot"
         else:
             self.task = "post_update"
 
     def work(self):
         self.check_date_constraint()
@@ -538,10 +598,10 @@
             elif task == "needs_reboot":
                 self.needs_reboot()
             elif task == "reboot":
                 self.reboot()
             elif task == "post_update":
                 self.post_update()
             else:
-                self.log.fatal("found garbage in status file: {0}".format(self.task))
+                self.log.fatal(f"found garbage in status file: {self.task}")
                 del self.task
                 sys.exit(1)
```

### Comparing `DlmEngineUpdater-0.0.9/setup.py` & `DlmEngineUpdater-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DlmEngineUpdater',
-    version='0.0.9',
+    version='0.1.0',
     description='DlmEngine, distributed lock implementation on top of MongoDB and Redis',
     long_description="""
 DLMEngine implements a restful interface that can be used to implement distributed locks.
 
 The main intention was to orchestrate automated system updates, so only one server at a time will do a update.
 
-Copyright (c) 2019, Stephan Schultchen.
+Copyright (c) 2023, Stephan Schultchen.
 
 License: MIT (see LICENSE for details)
     """,
     packages=find_packages(),
     scripts=[
         'contrib/dlm_engine_updater',
     ],
```

