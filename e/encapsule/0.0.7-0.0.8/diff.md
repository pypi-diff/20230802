# Comparing `tmp/encapsule-0.0.7.tar.gz` & `tmp/encapsule-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.7.tar", last modified: Wed Aug  2 03:37:34 2023, max compression
+gzip compressed data, was "encapsule-0.0.8.tar", last modified: Wed Aug  2 13:27:54 2023, max compression
```

## Comparing `encapsule-0.0.7.tar` & `encapsule-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 03:37:34.489109 encapsule-0.0.7/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 03:37:34.489109 encapsule-0.0.7/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.7/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 03:37:34.457859 encapsule-0.0.7/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.7/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     4842 2023-08-02 03:25:12.000000 encapsule-0.0.7/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     7100 2023-08-02 03:35:56.000000 encapsule-0.0.7/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 03:37:34.489109 encapsule-0.0.7/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-02 03:37:34.000000 encapsule-0.0.7/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-02 03:37:34.489109 encapsule-0.0.7/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-02 03:37:10.000000 encapsule-0.0.7/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:27:54.743031 encapsule-0.0.8/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:27:54.743031 encapsule-0.0.8/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.8/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:27:54.711771 encapsule-0.0.8/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.8/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     5895 2023-08-02 13:08:09.000000 encapsule-0.0.8/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     1386 2023-08-02 13:26:50.000000 encapsule-0.0.8/encapsule/isolate_mgr.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     7603 2023-08-02 13:13:45.000000 encapsule-0.0.8/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:27:54.727395 encapsule-0.0.8/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      254 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-02 13:27:54.743031 encapsule-0.0.8/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-02 13:27:28.000000 encapsule-0.0.8/setup.py
```

### Comparing `encapsule-0.0.7/PKG-INFO` & `encapsule-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.7
+Version: 0.0.8
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.7/encapsule/isolate_bin.py` & `encapsule-0.0.8/encapsule/isolate_bin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,53 @@
-# !!! This runs as SETUID=0 !!!
+# XXX Todo: use a setuid-0 installation of python exe
+
 '''
 SYSBIN=/system/bin
 
 setuid -u 0 "$SYSBIN/.isolate"
 PATH=$SYSBIN:$PATH
 
 .isolate --post-context assets/Itham/services/component/query \
 	--keyword=value arg1 arg2 arg3 \
 	| wget 'https://network/channel/x' -x post
 
 
-assets/Itham/services/component::
-	def query():
-		return 'text/json/dumps' \
-			(mapping(arguments = args$(), \
-				     keywords = keywords$()))
+assets/Itham/services:
+	component::
+		def query():
+			return 'text/json/dumps' \
+				(mapping(arguments = args$(), \
+					     keywords = keywords$()))
+
+	encapsule::
+		def argsOf(kwdClass, args, kwd):
+			for pair in keywords$().items():
+				args.append(act(kwdClass, pair))
+
+			return args
+
+		def compartmentalize(name):
+			exe = 'kernel/lookup$'('encapsule.exeCallObject')
+			exe$error = exe.error
+
+			try: return act(exe, argsOf \
+					(exe.keyword, args$(), keywords$()), \
+						mapping(compartmentalize = true))
+
+			except exe$error e:
+				return namespace \
+					(code = e.returncode, \
+					 error = e.stderrOutput, \
+					 output = e.stdOutput)
+
+			usage:
+				'services/encapsule/compartmentalize'.action \
+					('assets/Itham/services/component/query', \
+					 keyword = 'value') \
+					 	('arg1', 'arg2', 'arg3')
 
 '''
 
 import sys
 import op
 
 from json import loads as deserialize, dumps as serialize
@@ -31,15 +60,15 @@
 __all__ = ['exeCall', 'exeCallObject', 'keyword']
 
 publicName = hash
 
 def invocation(argv = None):
 	try: (options, output) = main(argv)
 	except CalledProcessError as e:
-		sys.stderr.write(e.stderrOutput)
+		sys.stderr.write(e.stderrOutput.decode())
 		sys.exit(e.returncode)
 
 		raise SystemError(f'Could not exit (returncode: {e.returncode})')
 
 
 	if options.post_context:
 		# XXX Shouldn't be json
@@ -49,15 +78,17 @@
 			 content = output))
 
 	sys.stdout.write(output)
 
 
 def buildOptions_parent(options):
 	return namespace \
-		(component_root = isolate_sys.ENCAPSULE_COMPONENTS_PATH,
+		(# "chroot" mount point:
+		 component_root = isolate_sys.ENCAPSULE_COMPONENTS_PATH,
+
 		 compartmentalize = options.get('compartmentalize'),
 		 segments = options.get('segments'),
 		 post_context = options.get('post_context'))
 
 def parseCmdln_subjective(argv):
 	# Todo: wrong
 	from optparse import OptionParser
@@ -72,42 +103,47 @@
 				(namespace(post_context = options.post_context,
 						   compartmentalize = True)),
 			 (args[0],)), args[1:])
 
 
 class Component:
 	# This represents an invocation instance, so, we can
-	# store invocation-specific data.
+	# store invocation-specific data (taskId_new).
 
 	@classmethod
 	def Locate(self, options, name):
-		return self(name, options, io.path \
-			(options.component_root) \
-				(*name.split('/')))
+		return self(name, options, isolate_sys.restrict_path \
+					# Note: splitting on '/' means empty components are ignored.
+					(options.component_root, name.split('/')))
 
 	def __init__(self, name, parentOptions, executable):
 		self.name = name
 		self.parentOptions = parentOptions
 		self.executable = executable
 
 	def newTaskId_env(self, **kwd):
 		if self.parentOptions.compartmentalize:
-			kwd['env'] = self.env_i = isolate_sys.generateNewTaskId_env()
+			(kwd['env'], self.taskId_new) = isolate_sys.generateNewTaskId_env()
+		else:
+			# todo: Is this always true?
+			self.taskId_new	= isolate_sys.taskId()
 
 		# _posixsubprocess-setuid: is this available on cygwin?
-		kwd['user'] = isolate_sys.componentOwnerUser(self.name)
+		# Todo: cygwin multi-user testing setup.
+		kwd['user'] = isolate_sys.componentOwnerUser \
+			(self.name, enforce = isolate_sys.effectiveContextId())
 
 		return kwd
 
 	@contextmanager
 	def runContext(self, process):
 		# grr
 		with isolate_sys.setTaskFrame_pid \
-			(self.env_i[isolate_sys.ENCAPSULE_TASK_ID_ENV],
-			 process.pid, self.parentOptions.compartmentalize) as x:
+			(self.taskId_new, process.pid,
+			 self.parentOptions.compartmentalize) as x:
 
 			yield x
 
 	def pipeStringContext(self, args):
 		# Subject Main.
 		# Perform access check.
 
@@ -150,20 +186,20 @@
 		self.value = value
 
 	def __str__(self):
 		return f'--{name}={value}'
 
 def exeCall(name, *args, **kwd):
 	'''
-	from encapsulate import exeCallObject, keyword
+	from encapsulate import exeCallObject
 
 	def run():
 		try: return exeCallObject \
 			('assets/Itham/services/component/query',
-			 keyword('keyword', 'value'),
+			 exeCallObject.keyword('keyword', 'value'),
 			 'arg1', 'arg2', 'arg3',
 			 compartmentalize = True)
 
 		except exeCallObject.error as e:
 			return namespace(code = e.returncode,
 							 error = e.stderrOutput,
 							 output = e.stdOutput)
@@ -174,12 +210,13 @@
 		(buildOptions_parent(kwd), name) \
 			.pipeStringContext(' '.join(map(str, args)))
 
 def exeCallObject(*args, **kwd):
 	return deserialize(exeCall(*args, **kwd))
 
 exeCallObject.error = CalledProcessError
+exeCallObject.keyword = keyword
 
 
 if __name__ == '__main__':
 	invocation(sys.argv[1:])
 	# invocation(sys.argv)
```

### Comparing `encapsule-0.0.7/encapsule/isolate_sys.py` & `encapsule-0.0.8/encapsule/isolate_sys.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,39 @@
 			try: return kwd['default']
 			except:
 				raise e
 
 	def erase(self, i, name):
 		return self.pathOf(i, name).delete()
 
+		# path = self.pathOf(i, name)
+
+		# if path.isdir:
+		#   # XXX removedirs doesn't remove non-empty dirs
+		#	from os import removedirs
+		# 	return removedirs(path)
+
+		# return path.delete()
+
 	def touch(self, i, name):
 		return self.store(i, name, '')
 
 
+# Filesystem
+def restrict_path(root, path):
+	r = root = io.path(root)
+
+	for p in path:
+		if p != '..' or r != root:
+			# Note: empty components are ignored.
+			r = r(p)
+
+	return r
+
+
 # Task:Identifiable
 def taskId():
 	return os_environ[ENCAPSULE_TASK_ID_ENV]
 
 
 # Todo: move into orchObject
 @contextmanager
@@ -121,15 +142,15 @@
 		except: pass
 		else:
 			if r:
 				break
 
 	try: erase(storageClass.TASKS, i)
 	except IsADirectoryError:
-		pass # not yet implemented
+		pass # not yet implemented: need a rigorously-safe impl
 
 def task_initiateCompletionScript(pathScript, taskId):
 	# todo: pathScript could be a folder containing identity info
 	pass
 
 
 INVALID_PID = -1
@@ -156,28 +177,29 @@
 
 		if not orchObject_i.taskOf(i).exists:
 			return i
 
 	raise ValueError(tries)
 
 def generateNewTaskId_env():
-	return {ENCAPSULE_TASK_ID_ENV: generateNewTaskId()}
+	i = generateNewTaskId()
+	return ({ENCAPSULE_TASK_ID_ENV: i}, i)
 
 
 # Permissions.
 def encodeComponent(name):
 	return b32encode(name.encode())
 
 
 def exe_perm_owner(name):
 	return localFS_i.exe_owner_path \
 		(encodeComponent(name))
 
-def componentOwnerUser(name):
-	return retrieve(exe_perm_owner, name, default = None)
+def componentOwnerUser(name, enforce = None):
+	return retrieve(exe_perm_owner, name, default = enforce)
 def setComponentOwner(name, userId):
 	return store(exe_perm_owner, name, userId)
 
 
 def permOf(userId, name, access = 'read'):
 	return f'{userId}:{encodeComponent(name)}:{access}'
 
@@ -299,15 +321,15 @@
 					(storageClass.TASKS).listing)
 
 	def taskOf(self, taskId):
 		return self.taskObject(self.storage.pathOf \
 			(storageClass.TASKS, taskId))
 
 
-# Install.
+# Install - XXX These shouldn't be set by the environment.
 (store, retrieve, erase, touch) = localFS_i = localFS \
 	(os_environ[ENCAPSULE_STORE_ENV],
 	 exe_owner_path = os_environ.get(ENCAPSULE_OWNERSHIP_ENV))
 
 ENCAPSULE_COMPONENTS_PATH = os_environ[ENCAPSULE_COMPONENTS_PATH_ENV]
 
 orchObject_i = orchObject(localFS_i)
```

### Comparing `encapsule-0.0.7/encapsule.egg-info/PKG-INFO` & `encapsule-0.0.8/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.7
+Version: 0.0.8
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.7/setup.py` & `encapsule-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

