# Comparing `tmp/encapsule-0.0.2.tar.gz` & `tmp/encapsule-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.2.tar", last modified: Tue Aug  1 15:32:32 2023, max compression
+gzip compressed data, was "encapsule-0.0.6.tar", last modified: Tue Aug  1 22:20:09 2023, max compression
```

## Comparing `encapsule-0.0.2.tar` & `encapsule-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.158211 encapsule-0.0.2/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 15:32:32.158211 encapsule-0.0.2/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.2/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.126949 encapsule-0.0.2/encapsule/
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:51:10.000000 encapsule-0.0.2/encapsule/__init__.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)     3237 2023-08-01 14:58:34.000000 encapsule-0.0.2/encapsule/isolate_bin.py
--rwxr-xr-x   0 Owner    (197610) None     (197121)      579 2023-08-01 14:50:28.000000 encapsule-0.0.2/encapsule/isolate_sys.py
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.158211 encapsule-0.0.2/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 15:32:31.000000 encapsule-0.0.2/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 15:32:32.158211 encapsule-0.0.2/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 15:31:12.000000 encapsule-0.0.2/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 22:20:09.182086 encapsule-0.0.6/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 22:20:09.182086 encapsule-0.0.6/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.6/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 22:20:09.166470 encapsule-0.0.6/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2023-08-01 20:07:40.000000 encapsule-0.0.6/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     4665 2023-08-01 21:49:24.000000 encapsule-0.0.6/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     5699 2023-08-01 22:15:41.000000 encapsule-0.0.6/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 22:20:09.182086 encapsule-0.0.6/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 22:20:08.000000 encapsule-0.0.6/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 22:20:09.000000 encapsule-0.0.6/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 22:20:08.000000 encapsule-0.0.6/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 22:20:08.000000 encapsule-0.0.6/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 22:20:09.197715 encapsule-0.0.6/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 22:19:40.000000 encapsule-0.0.6/setup.py
```

### Comparing `encapsule-0.0.2/PKG-INFO` & `encapsule-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.2
+Version: 0.0.6
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.2/encapsule/isolate_bin.py` & `encapsule-0.0.6/encapsule/isolate_bin.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,19 +18,22 @@
 
 '''
 
 import sys
 import op
 
 from json import loads as deserialize, dumps as serialize
+from contextlib import contextmanager
 
 from op.platform.path import CalledProcessError
 
 from . import isolate_sys
 
+__all__ = ['exeCall', 'exeCallObject', 'keyword']
+
 publicName = hash
 
 def invocation(argv = None):
 	try: (options, output) = main(argv)
 	except CalledProcessError as e:
 		sys.stderr.write(e.stderrOutput)
 		sys.exit(e.returncode)
@@ -45,54 +48,95 @@
 				(isolate_sys.effectiveContextId()),
 			 content = output))
 
 	sys.stdout.write(output)
 
 
 def buildOptions_parent(options):
-	pass
+	return namespace \
+		(component_root = isolate_sys.COMPONENTS_PATH,
+		 compartmentalize = options.get('compartmentalize'),
+		 segments = options.get('segments'),
+		 post_context = options.get('post_context'))
 
 def parseCmdln_subjective(argv):
-	pass
+	# Todo: wrong
+	from optparse import OptionParser
+	parser = OptionParser()
+	parser.add_option('--post-context', action = 'store_true')
+
+	(options, args) = parser.parse_args(argv)
+
+	# isolate_bin invocations are always 'compartmentalized',
+	# for now, because it represents an entry point.
+	return ((buildOptions_parent \
+				(namespace(post_context = options.post_context,
+						   compartmentalize = True)),
+			 (args[0],)), args[1:])
 
 
 class Component:
+	# This represents an invocation instance, so, we can
+	# store invocation-specific data.
+
 	@classmethod
 	def Locate(self, options, name):
 		return self(name, options, io.path \
 			(options.component_root) \
 				(*name.split('/')))
 
 	def __init__(self, name, parentOptions, executable):
 		self.name = name
 		self.parentOptions = parentOptions
 		self.executable = executable
 
-	def pipeStringContext(options):
+	def newTaskId_env(self, **kwd):
+		if self.parentOptions.compartmentalize:
+			kwd['env'] = self.env_i = isolate_sys.generateNewTaskId_env()
+
+		return kwd
+
+	@contextmanager
+	def runContext(self, process):
+		# grr
+		with isolate_sys.setTaskFrame_pid \
+			(self.env_i[isolate_sys.TASK_ID_ENV],
+			 process.pid) as x:
+
+			yield x
+
+	def pipeStringContext(self, args):
 		# Subject Main.
 		# Perform access check.
 
 		# setuid pipe invocation
 
-		isolate_sys.checkAccess(self)
+		# XXX DISABLED FOR TESTING XXX
+		# isolate_sys.checkAccessCurrentUser(self.name)
 
-		settings = dict(env = dict(TASK_ID = isolate_sys.generateNewTaskId())) \
-				   if self.parentOptions.compartmentalize \
-				   else dict()
+		settings = self.newTaskId_env(runContext = self.runContext)
 
 		# XXX Todo: inside, set system-level 'current frame process id'
 		# for whatever this task is.  Do this in a python context, when
 		# exiting, reset to 'this frame process id.'
-		return self.executable.pipeStringContext \
-			(isolate_sys.effectiveContextId(), options,
-			 segments = self.parentOptions.segments,
-			 setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
-			 **settings)
+		# return self.executable.pipeStringContext \
+		# 	(isolate_sys.effectiveContextId(), args,
+		# 	 # segments = self.parentOptions.segments,
+		# 	 # setTaskFrame_pid = isolate_sys.setTaskFrame_pid,
+		# 	 **settings)
+
+		# To work:
+		# import pdb; pdb.set_trace()
+		return self.executable.pipe \
+			(*args, **settings) \
+			.decode() # Why subprocess returns bytes stream,
+					  # but sys.stdout is default opened str.
 
 def main(argv):
+	# import pdb; pdb.set_trace()
 	((parentOptions, parentArgs), isoOptions) = \
 		parseCmdln_subjective(argv)
 
 	return (parentOptions, Component.Locate \
 		(parentOptions, *parentArgs)	\
 			.pipeStringContext(isoOptions))
 
@@ -101,17 +145,17 @@
 	def __init__(self, name, value):
 		self.name = name
 		self.value = value
 
 	def __str__(self):
 		return f'--{name}={value}'
 
-def exeCall(name, *args, **kwd)
+def exeCall(name, *args, **kwd):
 	'''
-	from encapsulate.isolate_bin import exeCallObject
+	from encapsulate import exeCallObject, keyword
 
 	def run():
 		try: return exeCallObject \
 			('assets/Itham/services/component/query',
 			 keyword('keyword', 'value'),
 			 'arg1', 'arg2', 'arg3',
 			 compartmentalize = True)
@@ -130,8 +174,9 @@
 def exeCallObject(*args, **kwd):
 	return deserialize(exeCall(*args, **kwd))
 
 exeCallObject.error = CalledProcessError
 
 
 if __name__ == '__main__':
-	return main(sys.argv)
+	invocation(sys.argv[1:])
+	# invocation(sys.argv)
```

### Comparing `encapsule-0.0.2/encapsule.egg-info/PKG-INFO` & `encapsule-0.0.6/encapsule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsule
-Version: 0.0.2
+Version: 0.0.6
 Summary: POSIX application security.
 Home-page: 
 Download-URL: 
 Author: 
 Author-email: 
 License: None
 Platform: OS-independent
```

### Comparing `encapsule-0.0.2/setup.py` & `encapsule-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.0.2'
+VERSION = '0.0.6'
 
 try: from setuptools import setup, find_packages
 except ImportError: from distutils.core import setup, find_packages
 
 SETUP_CONF = \
 dict (name = "encapsule",
       description = "POSIX application security.",
```

