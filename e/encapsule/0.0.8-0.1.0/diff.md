# Comparing `tmp/encapsule-0.0.8.tar.gz` & `tmp/encapsule-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.8.tar", last modified: Wed Aug  2 13:27:54 2023, max compression
+gzip compressed data, was "encapsule-0.1.0.tar", last modified: Wed Aug  2 13:51:55 2023, max compression
```

## Comparing `encapsule-0.0.8.tar` & `encapsule-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:27:54.743031 encapsule-0.0.8/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:27:54.743031 encapsule-0.0.8/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.8/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:27:54.711771 encapsule-0.0.8/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.8/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     5895 2023-08-02 13:08:09.000000 encapsule-0.0.8/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     1386 2023-08-02 13:26:50.000000 encapsule-0.0.8/encapsule/isolate_mgr.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     7603 2023-08-02 13:13:45.000000 encapsule-0.0.8/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:27:54.727395 encapsule-0.0.8/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      254 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-02 13:27:54.000000 encapsule-0.0.8/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-02 13:27:54.743031 encapsule-0.0.8/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-02 13:27:28.000000 encapsule-0.0.8/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:51:55.630334 encapsule-0.1.0/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:51:55.630334 encapsule-0.1.0/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.1.0/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:51:55.599224 encapsule-0.1.0/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.1.0/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     6232 2023-08-02 13:50:54.000000 encapsule-0.1.0/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     1386 2023-08-02 13:26:50.000000 encapsule-0.1.0/encapsule/isolate_mgr.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     7603 2023-08-02 13:13:45.000000 encapsule-0.1.0/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-02 13:51:55.630334 encapsule-0.1.0/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      254 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-02 13:51:54.000000 encapsule-0.1.0/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-02 13:51:55.630334 encapsule-0.1.0/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-02 13:51:12.000000 encapsule-0.1.0/setup.py
```

### Comparing `encapsule-0.0.8/PKG-INFO` & `encapsule-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.8
+Version: 0.1.0
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.8/encapsule/isolate_bin.py` & `encapsule-0.1.0/encapsule/isolate_bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,37 +15,43 @@
 	component::
 		def query():
 			return 'text/json/dumps' \
 				(mapping(arguments = args$(), \
 					     keywords = keywords$()))
 
 	encapsule::
+		XXX:
+			This needs 
+
 		def argsOf(kwdClass, args, kwd):
 			for pair in keywords$().items():
 				args.append(act(kwdClass, pair))
 
 			return args
 
-		def compartmentalize(name):
+		def compartmentalize(context, name):
 			exe = 'kernel/lookup$'('encapsule.exeCallObject')
 			exe$error = exe.error
 
 			try: return act(exe, argsOf \
 					(exe.keyword, args$(), keywords$()), \
-						mapping(compartmentalize = true))
+						mapping(compartmentalize = true, \
+							    impersonateAs = context(programmer))
 
 			except exe$error e:
 				return namespace \
 					(code = e.returncode, \
 					 error = e.stderrOutput, \
 					 output = e.stdOutput)
 
 			usage:
 				'services/encapsule/compartmentalize'.action \
-					('assets/Itham/services/component/query', \
+					(security$context$new(), \
+					 'assets/Itham/services/component/query', \
+
 					 keyword = 'value') \
 					 	('arg1', 'arg2', 'arg3')
 
 '''
 
 import sys
 import op
@@ -68,14 +74,15 @@
 		sys.exit(e.returncode)
 
 		raise SystemError(f'Could not exit (returncode: {e.returncode})')
 
 
 	if options.post_context:
 		# XXX Shouldn't be json
+		# XXX limited UID specification here
 		output = serialize(dict \
 			(context = publicName \
 				(isolate_sys.effectiveContextId()),
 			 content = output))
 
 	sys.stdout.write(output)
 
@@ -125,38 +132,42 @@
 			(kwd['env'], self.taskId_new) = isolate_sys.generateNewTaskId_env()
 		else:
 			# todo: Is this always true?
 			self.taskId_new	= isolate_sys.taskId()
 
 		# _posixsubprocess-setuid: is this available on cygwin?
 		# Todo: cygwin multi-user testing setup.
+		# Todo: specification of UID?
 		kwd['user'] = isolate_sys.componentOwnerUser \
-			(self.name, enforce = isolate_sys.effectiveContextId())
+			(self.name, enforce = kwd.get('userId') \
+				or isolate_sys.effectiveContextId())
 
 		return kwd
 
 	@contextmanager
 	def runContext(self, process):
 		# grr
 		with isolate_sys.setTaskFrame_pid \
 			(self.taskId_new, process.pid,
 			 self.parentOptions.compartmentalize) as x:
 
 			yield x
 
-	def pipeStringContext(self, args):
+	def pipeStringContext(self, args, **kwd):
 		# Subject Main.
 		# Perform access check.
 
 		# setuid pipe invocation
 
 		# XXX DISABLED FOR TESTING XXX
 		# isolate_sys.checkAccessCurrentUser(self.name)
 
-		settings = self.newTaskId_env(runContext = self.runContext)
+		settings = self.newTaskId_env \
+			(runContext = self.runContext,
+			 userId = kwd.get('userId'))
 
 		# XXX Todo: inside, set system-level 'current frame process id'
 		# for whatever this task is.  Do this in a python context, when
 		# exiting, reset to 'this frame process id.'
 		# return self.executable.pipeStringContext \
 		# 	(isolate_sys.effectiveContextId(), args,
 		# 	 # segments = self.parentOptions.segments,
@@ -202,17 +213,21 @@
 		except exeCallObject.error as e:
 			return namespace(code = e.returncode,
 							 error = e.stderrOutput,
 							 output = e.stdOutput)
 
 	'''
 
+	userId = kwd.pop('impersonateAs')
+
 	return Component.Locate \
 		(buildOptions_parent(kwd), name) \
-			.pipeStringContext(' '.join(map(str, args)))
+			.pipeStringContext \
+				(' '.join(map(str, args)),
+				 userId = userId)
 
 def exeCallObject(*args, **kwd):
 	return deserialize(exeCall(*args, **kwd))
 
 exeCallObject.error = CalledProcessError
 exeCallObject.keyword = keyword
```

### Comparing `encapsule-0.0.8/encapsule/isolate_mgr.py` & `encapsule-0.1.0/encapsule/isolate_mgr.py`

 * *Files identical despite different names*

### Comparing `encapsule-0.0.8/encapsule/isolate_sys.py` & `encapsule-0.1.0/encapsule/isolate_sys.py`

 * *Files identical despite different names*

### Comparing `encapsule-0.0.8/encapsule.egg-info/PKG-INFO` & `encapsule-0.1.0/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.8
+Version: 0.1.0
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.8/setup.py` & `encapsule-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.8'
+VERSION = '0.1.0'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

