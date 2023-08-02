# Comparing `tmp/encapsule-0.0.6.tar.gz` & `tmp/encapsule-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.6.tar", last modified: Tue Aug  1 22:20:09 2023, max compression
+gzip compressed data, was "encapsule-0.0.7.tar", last modified: Wed Aug  2 03:37:34 2023, max compression
```

## Comparing `encapsule-0.0.6.tar` & `encapsule-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 22:20:09.182086 encapsule-0.0.6/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 22:20:09.182086 encapsule-0.0.6/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.6/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 22:20:09.166470 encapsule-0.0.6/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.6/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     4665 2023-08-01 21:49:24.000000 encapsule-0.0.6/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     5699 2023-08-01 22:15:41.000000 encapsule-0.0.6/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 22:20:09.182086 encapsule-0.0.6/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 22:20:08.000000 encapsule-0.0.6/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 22:20:09.000000 encapsule-0.0.6/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 22:20:08.000000 encapsule-0.0.6/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 22:20:08.000000 encapsule-0.0.6/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 22:20:09.197715 encapsule-0.0.6/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 22:19:40.000000 encapsule-0.0.6/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 03:37:34.489109 encapsule-0.0.7/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 03:37:34.489109 encapsule-0.0.7/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.7/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 03:37:34.457859 encapsule-0.0.7/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.7/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     4842 2023-08-02 03:25:12.000000 encapsule-0.0.7/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     7100 2023-08-02 03:35:56.000000 encapsule-0.0.7/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 03:37:34.489109 encapsule-0.0.7/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-02 03:37:34.489109 encapsule-0.0.7/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-02 03:37:10.000000 encapsule-0.0.7/setup.py
```

### Comparing `encapsule-0.0.6/PKG-INFO` & `encapsule-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.6
+Version: 0.0.7
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.6/encapsule/isolate_bin.py` & `encapsule-0.0.7/encapsule/isolate_bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 			 content = output))
 
 	sys.stdout.write(output)
 
 
 def buildOptions_parent(options):
 	return namespace \
-		(component_root = isolate_sys.COMPONENTS_PATH,
+		(component_root = isolate_sys.ENCAPSULE_COMPONENTS_PATH,
 		 compartmentalize = options.get('compartmentalize'),
 		 segments = options.get('segments'),
 		 post_context = options.get('post_context'))
 
 def parseCmdln_subjective(argv):
 	# Todo: wrong
 	from optparse import OptionParser
@@ -89,22 +89,25 @@
 		self.parentOptions = parentOptions
 		self.executable = executable
 
 	def newTaskId_env(self, **kwd):
 		if self.parentOptions.compartmentalize:
 			kwd['env'] = self.env_i = isolate_sys.generateNewTaskId_env()
 
+		# _posixsubprocess-setuid: is this available on cygwin?
+		kwd['user'] = isolate_sys.componentOwnerUser(self.name)
+
 		return kwd
 
 	@contextmanager
 	def runContext(self, process):
 		# grr
 		with isolate_sys.setTaskFrame_pid \
-			(self.env_i[isolate_sys.TASK_ID_ENV],
-			 process.pid) as x:
+			(self.env_i[isolate_sys.ENCAPSULE_TASK_ID_ENV],
+			 process.pid, self.parentOptions.compartmentalize) as x:
 
 			yield x
 
 	def pipeStringContext(self, args):
 		# Subject Main.
 		# Perform access check.
```

### Comparing `encapsule-0.0.6/encapsule/isolate_sys.py` & `encapsule-0.0.7/encapsule/isolate_sys.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 from posix import geteuid as effectiveContextId
 
-from os import kill as processKill, environ as osEnviron
+from os import kill as processKill, environ as os_environ
 from signal import SIGSTOP, SIGCONT, SIGTERM # , SIGKILL
 from contextlib import contextmanager
 from string import ascii_letters as _taskId_alphabet
 from base64 import b32encode
 
 from random import choice # XXX entropy
 
 
+# Environment.
+ENCAPSULE_TASK_ID_ENV = 'ENCAPSULE_TASK_ID'
+ENCAPSULE_STORE_ENV = 'ENCAPSULE_KERNEL'
+ENCAPSULE_COMPONENTS_PATH_ENV = 'ENCAPSULE_COMPONENTS'
+ENCAPSULE_OWNERSHIP_ENV = 'ENCAPSULE_OWNERSHIP'
+
+
 class NoFramesError(RuntimeError):
 	pass
 class NoAccessException(Exception):
 	pass
 
 
 # Storage.
-TASK_ID_ENV = 'TASK_ID'
-
 class storageClass:
 	TASKS = 'tasks'
 	ACCESS = 'access'
+	EXE_OWNER = 'ownership'
 
 class localFS(storageClass):
 	SEP = ':'
 
-	def __init__(self, path):
+	def __init__(self, path, exe_owner_path = None):
+		# !!! These paths should be ROOT-ONLY !!!
 		self.path = io.path(path)
 
+		if exe_owner_path is None:
+			exe_owner_path = self.path(self.EXE_OWNER)
+
+		self.exe_owner_path = exe_owner_path
+
 	def pathOf(self, i, name = ''):
-		return self.path(i, *name.split(self.SEP))
+		return i(name) if callable(i) else \
+				self.path(i, *name.split(self.SEP))
 
 	@contextmanager
 	def pathOf_c(self, *args, **kwd):
 		yield self.pathOf(*args, **kwd)
 
 	def __iter__(self):
 		yield self.store
@@ -59,20 +72,20 @@
 
 	def touch(self, i, name):
 		return self.store(i, name, '')
 
 
 # Task:Identifiable
 def taskId():
-	return osEnviron[TASK_ID_ENV]
+	return os_environ[ENCAPSULE_TASK_ID_ENV]
 
 
 # Todo: move into orchObject
 @contextmanager
-def setTaskFrame_pid(i, pid):
+def setTaskFrame_pid(i, pid, compartment):
 	# "addTaskFrame"
 
 	# i = taskId()
 
 	# import pdb; pdb.set_trace()
 
 	u = int(retrieve(storageClass.TASKS, f'{i}:frameCurrent', default = -1))
@@ -84,20 +97,45 @@
 	fu = f'{i}:frameCurrent'
 	store(storageClass.TASKS, fu, ui)
 
 	try: yield
 	finally:
 		erase(storageClass.TASKS, newU)
 
-		if u < 0:
+		if compartment:
+			completeTask(i)
+		elif u < 0:
 			erase(storageClass.TASKS, fu)
 		else:
 			store(storageClass.TASKS, fu, u)
 
 
+def completeTask(i):
+	try: taskCompletion = orchObject_i.storage.pathOf \
+		(storageClass.TASKS, f'{i}:completions').listing
+
+	except FileNotFoundError:
+		taskCompletion = []
+
+	for complete in taskCompletion:
+		try: r = task_initiateCompletionScript(complete, i)
+		except: pass
+		else:
+			if r:
+				break
+
+	try: erase(storageClass.TASKS, i)
+	except IsADirectoryError:
+		pass # not yet implemented
+
+def task_initiateCompletionScript(pathScript, taskId):
+	# todo: pathScript could be a folder containing identity info
+	pass
+
+
 INVALID_PID = -1
 
 def pidOf_taskFrame(taskId, invalid_onerror = False):
 	u = retrieve(storageClass.TASKS, f'{taskId}:frameCurrent', default = -1)
 	if u < 0:
 		raise NoFramesError()
 
@@ -118,27 +156,37 @@
 
 		if not orchObject_i.taskOf(i).exists:
 			return i
 
 	raise ValueError(tries)
 
 def generateNewTaskId_env():
-	return {TASK_ID_ENV: generateNewTaskId()}
+	return {ENCAPSULE_TASK_ID_ENV: generateNewTaskId()}
 
 
 # Permissions.
 def encodeComponent(name):
 	return b32encode(name.encode())
 
 
+def exe_perm_owner(name):
+	return localFS_i.exe_owner_path \
+		(encodeComponent(name))
+
+def componentOwnerUser(name):
+	return retrieve(exe_perm_owner, name, default = None)
+def setComponentOwner(name, userId):
+	return store(exe_perm_owner, name, userId)
+
+
 def permOf(userId, name, access = 'read'):
-	return f'{storageClass.ACCESS}:{userId}:{encodeComponent(name)}:{access}'
+	return f'{userId}:{encodeComponent(name)}:{access}'
 
 def checkAccess(userId, name, access = 'read', fail_onerror = False):
-	if retrieve(storageClass.TASKS, permOf(userId, name, access),
+	if retrieve(storageClass.ACCESS, permOf(userId, name, access),
 				default = False) is not False:
 
 		return True
 
 	if fail_onerror:
 		return False
 
@@ -177,15 +225,15 @@
 	def environ(self):
 		return dict(x.split('=', 1) for x in
 					self.path.environ.read() \
 						.split('\x00'))
 
 	@property
 	def taskId(self):
-		return self.environ.get(TASK_ID_ENV)
+		return self.environ.get(ENCAPSULE_TASK_ID_ENV)
 
 
 	def suspend(self):
 		return suspend_process(self.pid)
 	def resume(self):
 		return resume_process(self.pid)
 
@@ -244,21 +292,22 @@
 
 	def __init__(self, storage):
 		self.storage = storage
 
 	def __iter__(self):
 		return (self.taskObject(path, orch = self)
 				for path in self.storage.pathOf \
-				(storageClass.TASKS).listing)
+					(storageClass.TASKS).listing)
 
 	def taskOf(self, taskId):
 		return self.taskObject(self.storage.pathOf \
 			(storageClass.TASKS, taskId))
 
 
 # Install.
 (store, retrieve, erase, touch) = localFS_i = localFS \
-	(osEnviron['ENCAPSULE_STORE'])
+	(os_environ[ENCAPSULE_STORE_ENV],
+	 exe_owner_path = os_environ.get(ENCAPSULE_OWNERSHIP_ENV))
 
-COMPONENTS_PATH = osEnviron['COMPONENTS_PATH']
+ENCAPSULE_COMPONENTS_PATH = os_environ[ENCAPSULE_COMPONENTS_PATH_ENV]
 
 orchObject_i = orchObject(localFS_i)
```

### Comparing `encapsule-0.0.6/encapsule.egg-info/PKG-INFO` & `encapsule-0.0.7/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.6
+Version: 0.0.7
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.6/setup.py` & `encapsule-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

