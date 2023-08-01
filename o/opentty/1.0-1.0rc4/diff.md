# Comparing `tmp/opentty-1.0.tar.gz` & `tmp/opentty-1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentty-1.0.tar", last modified: Tue Aug  1 22:38:14 2023, max compression
+gzip compressed data, was "opentty-1.0rc4.tar", last modified: Mon Jul 31 19:58:48 2023, max compression
```

## Comparing `opentty-1.0.tar` & `opentty-1.0rc4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lubuntu    (999) lubuntu    (999)        0 2023-08-01 22:38:14.592442 opentty-1.0/
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      703 2023-08-01 22:38:14.592442 opentty-1.0/PKG-INFO
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      165 2023-08-01 15:32:24.000000 opentty-1.0/README.md
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)     1163 2023-08-01 15:32:24.000000 opentty-1.0/__init__.py
-drwxrwxr-x   0 lubuntu    (999) lubuntu    (999)        0 2023-08-01 22:38:14.588442 opentty-1.0/opentty.egg-info/
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      703 2023-08-01 22:38:14.000000 opentty-1.0/opentty.egg-info/PKG-INFO
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      165 2023-08-01 22:38:14.000000 opentty-1.0/opentty.egg-info/SOURCES.txt
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)        1 2023-08-01 22:38:14.000000 opentty-1.0/opentty.egg-info/dependency_links.txt
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)        1 2023-08-01 22:38:14.000000 opentty-1.0/opentty.egg-info/top_level.txt
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)    32423 2023-08-01 22:21:42.000000 opentty-1.0/opentty.py
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)       38 2023-08-01 22:38:14.592442 opentty-1.0/setup.cfg
--rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      848 2023-08-01 15:32:24.000000 opentty-1.0/setup.py
+drwxrwxr-x   0 lubuntu    (999) lubuntu    (999)        0 2023-07-31 19:58:48.141596 opentty-1.0rc4/
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      706 2023-07-31 19:58:48.137597 opentty-1.0rc4/PKG-INFO
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      165 2023-07-30 18:33:46.000000 opentty-1.0rc4/README.md
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)     1163 2023-07-31 19:08:20.000000 opentty-1.0rc4/__init__.py
+drwxrwxr-x   0 lubuntu    (999) lubuntu    (999)        0 2023-07-31 19:58:48.137597 opentty-1.0rc4/opentty.egg-info/
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      706 2023-07-31 19:58:47.000000 opentty-1.0rc4/opentty.egg-info/PKG-INFO
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      165 2023-07-31 19:58:47.000000 opentty-1.0rc4/opentty.egg-info/SOURCES.txt
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)        1 2023-07-31 19:58:47.000000 opentty-1.0rc4/opentty.egg-info/dependency_links.txt
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)        1 2023-07-31 19:58:47.000000 opentty-1.0rc4/opentty.egg-info/top_level.txt
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)    33033 2023-07-31 19:50:44.000000 opentty-1.0rc4/opentty.py
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)       38 2023-07-31 19:58:48.141596 opentty-1.0rc4/setup.cfg
+-rw-rw-r--   0 lubuntu    (999) lubuntu    (999)      851 2023-07-31 19:36:57.000000 opentty-1.0rc4/setup.py
```

### Comparing `opentty-1.0/PKG-INFO` & `opentty-1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentty
-Version: 1.0
+Version: 1.0rc4
 Summary: The OpenTTY is a Terminal Emulator created tottaly in python based-on Unix-Like Shells
 Home-page: https://github.com/fetuber4095/OpenTTY
 Author: Mr. Lima
 Author-email: felipebr4095@gmail.com
 License: UNKNOWN
 Description: For more informations see README at Github
 Keywords: python package,emulator,windows,linux,shell,project,posix,unix
```

### Comparing `opentty-1.0/__init__.py` & `opentty-1.0rc4/__init__.py`

 * *Files identical despite different names*

### Comparing `opentty-1.0/opentty.egg-info/PKG-INFO` & `opentty-1.0rc4/opentty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentty
-Version: 1.0
+Version: 1.0rc4
 Summary: The OpenTTY is a Terminal Emulator created tottaly in python based-on Unix-Like Shells
 Home-page: https://github.com/fetuber4095/OpenTTY
 Author: Mr. Lima
 Author-email: felipebr4095@gmail.com
 License: UNKNOWN
 Description: For more informations see README at Github
 Keywords: python package,emulator,windows,linux,shell,project,posix,unix
```

### Comparing `opentty-1.0/opentty.py` & `opentty-1.0rc4/opentty.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 from socket import gethostname as hostname
 from random import randint, choice
 from time import sleep as timeout
 from sys import exit as close
 
 import os, sys, json, time, random, platform, subprocess, calendar
 import http, http.server, urllib, socket, socketserver, urllib.request
-import shutil, getpass, zipfile, datetime, shlex, traceback
+import shutil, getpass, zipfile, datetime, shlex
 
 library = {
 	# Informations for current installation
     "appname": "OpenTTY", 
-    "version": "1.0", "build": "06H6",
+    "version": "1.0-preIV", "build": "06H5",
     "subject": "The OpenTTY Upgrade",
 	"patch": [
-		"The first official release",
-		"Better tracebacks messages",
-		"Revised all module OpenTTY code Syntax",
-		"Now psh envirronment name is '__main__'",
+		"Add final touches at code",
+		"Better internal app logic",
+		"Added other builtins functions",
+		"First version uploaded to PyPi"
 	],
     
     "developer": "Mr. Lima",
 
 	# Development Settings
 	"debugmode": False,
 	"profile": "Fabric",
@@ -61,30 +61,27 @@
 	"sh": "psh", "sh-prefix": "\033[32m\033[1m$ ",
 	
 	# Aliases for users [client; root]
 	"aliases": {},
 	"internals": {
 		"cls": "clear", "date": "echo &time", "version": "echo &appname v&version [&subject]", "by": "echo &developer", 
 		"logname": "whoami", "profile": "echo [&profile]", "repo": "github", "globals": ": print(globals())", "logout": "true",
-		"whoami": "echo &self", "hostname": "echo &hostname"
+		"envname": "print(__name__)"
 	},
 	
 	# Firewall and root settings
 	"whitelist": [],
 	"root": f"{hostname()}@root-opentty.py",
 	"passwd": "1234",
 	
 	# Commands settings
 	"head-lines": 10,
 	"max-byte-len": 128, 
 	"ipinfo-token": "",
 
-	"openai-api": "sk-lyUE0nYEgxTbGotkD4IIT3BllbkFJO8YcM8DyzFLvpEsX8bEG",
-	"openai-max-tokens": 150,
-
 	"hidden-files-prefix": ".", # Prefix for hidden files
 	"dircolors": {
 		".py": "\033[32m", ".sh": "\033[32m", ".cmd": "\033[32m", ".bat": "\033[32m", ".json": "\033[36m", ".exe": "\033[31m", 
 		".com": "\033[31m", ".dll": "\033[31m", ".jar": "\033[31m", ".zip": "\033[36m", ".tar": "\033[36m", ".tar.gz": "\033[36m",
 		".tar.xz": "\033[36m", ".7z": "\033[36m", ".rar": "\033[36m", ".bin": "\033[36m", "install": "\033[36m"
 	},
 
@@ -104,16 +101,15 @@
 
 	],
 
 	# Resources Mirrors
 	"resources": {
 		"favicon": {"filename": "favicon.ico", "url": "https://github.com/fetuber4095/OpenTTY/raw/main/assets/favicon.ico"},
 		"ram": {"filename": "ram.py", "url": "https://github.com/fetuber4095/OpenTTY/raw/main/deploy/projects/ram.py"},
-		"forge": {"filename": "forge.py", "url": "https://github.com/fetuber4095/OpenTTY/raw/main/profiles/forge.py"},
-		"nano": {"filename": "nano.exe", "url": "https://github.com/fetuber4095/OpenTTY/raw/main/assets/Win32/nano.exe"}
+		"forge": {"filename": "forge.py", "url": "https://github.com/fetuber4095/OpenTTY/raw/main/profiles/forge.py"}
 	},
 
 	"docs": {
 		"license": "https://github.com/fetuber4095/OpenTTY/raw/main/LICENSE",
 		"inbox": "https://github.com/fetuber4095/OpenTTY/raw/main/server/services/inbox"
 	},
 
@@ -136,45 +132,42 @@
 		self.process = {"python": str(randint(1000, 9999))}
 		
 		self.root, self.puppydir = library['root-dir'], library['root-dir']
 		self.aliases = library['aliases']
 		self.functions = {}
 		
 		self.globals = {
-			"app": self, "library": library, "__name__": "__main__"
+			"app": self, "library": library, "__name__": library['sh']
 		}
 		self.locals = {}
 		
 	# OpenTTY - Client Interface [Module API]
 	def connect(self, host, port=8080):
+		self.ttyname = host
+		self.process[library['sh']] = str(port)
 
 		for asset in os.listdir(self.root): 
 			if asset.endswith(".sh"): self.build(f"{self.root}/{asset}", root=True)
 		
-		if library['sh'] not in self.process: 
-			self.ttyname = host
-			self.process[library['sh']] = str(port)
-
-			self.clear(), print(f"\n\n{self.appname} v{self.version} ({platform.system()} {platform.release()}) built-in shell ({library['sh']})\nEnter 'help' for more informations.")
-
-
+		self.clear(), print(f"\n\n{self.appname} v{self.version} ({platform.system()} {platform.release()}) built-in shell ({library['sh']})\nEnter 'help' for more informations.")
+		
 		while library['sh'] in self.process:
 			if not "python" in self.process: close()
 
 			try:
-				cmd = input(f"\n\033[31m\033[1m[{library['profile']}] \033[34m\033[1m{os.getcwd()} {library['sh-prefix']}\033[m").strip()
+				cmd = input(f"\n\033[31m\033[1m[{library['profile']}] \033[34m\033[1m{os.getcwd()} {library['sh-prefix']}\033[m")
 				
 				if cmd:
 					if cmd.split()[0] == "logout": break
 					
 					self.shell(cmd, mkprocess=True)
 					
 			except (KeyboardInterrupt, EOFError): self.clear()
 
-		self.__init__(), print("There are stopped jobs.\n")
+		print("There are stopped jobs.\n")
 	def disconnect(self, code=""):
 		if not code: code = 0
 
 		try:
 			print(f"\n------------------")
 			print(f"(program exited with code: {code})")
 			print(f"Press return to continue"), input(), close()
@@ -183,47 +176,48 @@
 	def execfile(self, filename, cmd="", ispkg=False):
 		if self.basename(filename).split()[0] not in library['whitelist'] and not ispkg: raise PermissionError
 
 		if filename.startswith("/"): filename = f"{self.root}{filename}"
 		if os.name == "nt": filename = filename.replace("/", "\\")
 
 		with open(filename, "r") as script:
-			try: exec(self.recognize(script.read()), self.globals, self.locals)
-			except Exception as error: traceback.print_exc()
+			try: exec(self.recognize(script.read()))
+			except Exception as traceback: print(f"{traceback.__class__.__name__}: {traceback}")
 
 	# OpenTTY "Shell"
 	def shell(self, cmd, mkprocess=True):
 		if mkprocess: self.mkprocess(cmd.split()[0])
 		
 		try:
 			cmd = str(self.recognize(cmd)).strip()
 
-			if cmd.split()[0] == ".":
-				if self.replace(cmd): self.execfile(self.replace(cmd), self.replace(self.replace(cmd)))
+			if cmd.split()[0] == ".": 
+				if cmd: self.execfile(self.replace(cmd).split()[0], self.replace(self.replace(cmd)))
 			elif cmd.split()[0] == ":":
 				try: exec(self.replace(cmd), self.globals, self.locals)
-				except Exception as error: traceback.print_exc()
+				except Exception as traceback: print(f"{traceback.__class__.__name__}: {traceback}")
 			
+			elif cmd.split()[0] == "var": self.shell(f": {self.replace(cmd)}", mkprocess=False)
+			elif cmd.split()[0] == "del": self.shell(f": {self.replace(cmd)}", mkprocess=False)
+			elif cmd.startswith("from") or cmd.startswith("import"): self.shell(f": {cmd}", mkprocess=False)
+			elif cmd.startswith("print"): self.shell(f": {cmd}", mkprocess=False)
 			elif cmd.startswith("@"): self.callmethod(cmd.replace("@", ""))
-			elif cmd.split()[0] == "set": self.shell(f": {self.replace(cmd)}", mkprocess=False)
-			elif cmd.startswith("from") or cmd.startswith("import") or cmd.startswith("print") or cmd.startswith("app"): self.shell(f": {cmd}", mkprocess=False)
-			elif cmd.split()[0] == "del": self.shell(f": {cmd}", mkprocess=False)
 			elif cmd.startswith("(") or cmd.startswith('"') or cmd.startswith('f"'):
-				try:
+				try: 
 					run = eval(cmd, self.globals, self.locals)
 
 					if run: print(run)
-				except Exception as error: traceback.print_exc()
+				except Exception as traceback: print(f"{traceback.__class__.__name__}: {traceback}")
 
 			elif cmd.split()[0] == "exit": self.disconnect(self.replace(cmd))
 			elif cmd.split()[0] == "echo": print(self.replace(cmd))
 			elif cmd.split()[0] == "prompt": input(self.replace(cmd))
 			elif cmd.split()[0] == "basename": print(self.basename(self.replace(cmd)) if self.replace(cmd) else f"basename: missing operand [path]...")
 			elif cmd.split()[0] == "cmatrix": self.ThreadRandom()
-			elif cmd.split()[0] == "ps": self.pslist()
+			elif cmd.split()[0] == "ps": self.pslist() 
 			elif cmd.split()[0] == "kill": self.kill(self.replace(cmd))
 			elif cmd.split()[0] == "mkdir": self.makedir(self.replace(cmd))
 			elif cmd.split()[0] == "rmdir": self.removedir(self.replace(cmd))
 			elif cmd.split()[0] == "rm": self.remove(self.replace(cmd))
 			elif cmd.split()[0] == "ls": self.listdir(self.replace(cmd))
 			elif cmd.split()[0] == "dd": self.txt2bin(self.replace(cmd))
 			elif cmd.split()[0] == "zipinfo": self.zipinfo(self.replace(cmd))
@@ -238,14 +232,15 @@
 			elif cmd.split()[0] == "head": self.headfile(self.replace(cmd))
 			elif cmd.split()[0] == "json": self.json_explorer(self.replace(cmd))
 			elif cmd.split()[0] == "nl": self.nl(self.replace(cmd))
 			elif cmd.split()[0] == "tail": self.tail(self.replace(cmd))
 			elif cmd.split()[0] == "diff": self.diff(self.replace(cmd))
 			elif cmd.split()[0] == "env": self.environ(self.replace(cmd))
 			elif cmd.split()[0] == "export": self.export(self.replace(cmd))
+			elif cmd.split()[0] == "set": self.set(self.replace(cmd))
 			elif cmd.split()[0] == "local": self.ThreadList(self.locals, prefix="local ")
 			elif cmd.split()[0] == "uname": self.uname(self.replace(cmd))
 			elif cmd.split()[0] == "chmod": self.chmod(self.replace(cmd))
 			elif cmd.split()[0] == "clear": self.clear()
 			elif cmd.split()[0] == "stty": self.stty(self.replace(cmd))
 			elif cmd.split()[0] == "tty": print(self.ttyname if self.ttyname else "localhost")
 			elif cmd.split()[0] == "pushd": self.pushdir(self.replace(cmd))
@@ -262,57 +257,55 @@
 			elif cmd.split()[0] == "build": self.build(self.replace(cmd))
 			elif cmd.split()[0] == "function": self.function(self.replace(cmd))
 			elif cmd.split()[0] == "gaddr": self.gaddr(self.replace(cmd))
 			elif cmd.split()[0] == "fw": self.fwadress(self.replace(cmd))
 			elif cmd.split()[0] == "wget": self.wget(self.replace(cmd))
 			elif cmd.split()[0] == "server": self.server(self.replace(cmd))
 			elif cmd.split()[0] == "cal": self.calendar()
+			elif cmd.split()[0] == "sleep": self.sleep(self.replace(cmd))
+			elif cmd.split()[0] == "seq": self.sequence(self.replace(cmd))
 			elif cmd.split()[0] == "github": print(library['github.com'])
 			elif cmd.split()[0] == "passwd": print(f"passwd: your password is {library['passwd']}")
 			elif cmd.split()[0] == "whoami": print(getpass.getuser())
 			elif cmd.split()[0] == "hostname": print(hostname())
 			elif cmd.split()[0] == "pwd": print(os.getcwd())
 			elif cmd.split()[0] == "venv": self.venv(self.replace(cmd))
 			elif cmd.split()[0] == "patch": print('\n'.join(f"- {note}" for note in library['patch']))
 			elif cmd.split()[0] == "rraw": self.rraw(self.replace(cmd), show=True)
 			elif cmd.split()[0] == "exec": local(self.replace(cmd))
-			elif cmd.split()[0] == "insmod": self.build(self.replace(cmd), root=True)
 			elif cmd.split()[0] == "inbox": self.rraw(library['docs']['inbox'], show=True, report="inbox", tbmsg="bad. failed to connect with inbox.")
 			elif cmd.split()[0] == "snapshot": print(library['build'])
-			#elif cmd.split()[0] == "":
+			elif cmd.split()[0] == "name": print(__name__)
 			#elif cmd.split()[0] == "":
 
 			elif cmd.split()[0] == "true": pass
 			elif cmd.split()[0] == "false": return self.rmprocess(cmd.split()[0])
 
 			else:
 				if cmd.split()[0] in self.aliases: self.shell(f"{self.aliases[cmd.split()[0]]} {self.replace(cmd)}", mkprocess=False)
 				elif cmd.split()[0] in library['internals']: self.shell(f"{library['internals'][cmd.split()[0]]} {self.replace(cmd)}", mkprocess=False)
 				elif f"{cmd.split()[0]}.py" in os.listdir(self.root): self.execfile(f"/{cmd.split()[0]}.py", self.replace(cmd), ispkg=True)
 				elif cmd.split()[0] in library[f'{os.name}-commands']: local(cmd)
 
 				elif cmd.split()[0] in library['resources']:
 					if library['resources'][cmd.split()[0]]['filename'] in os.listdir(self.root): print(f"{cmd.split()[0]}: asset is actived.")
-					elif library['resources'][cmd.split()[0]]['filename'] in os.listdir(self.root): print(f"{cmd.split()[0]}: asset is actived.")
 					else: print(f"{cmd.split()[0]}: asset not installed.")
 
 				else: return print(f"{cmd.split()[0]}: command not found"), self.rmprocess(cmd.split()[0])	
 				
 		except (KeyboardInterrupt, EOFError): return self.rmprocess(cmd.split()[0])	
 
 		except FileNotFoundError: return print(f"{cmd.split()[0]}: {self.basename(self.replace(cmd)).split()[0]}: file not found")
 		except FileExistsError: return print(f"{cmd.split()[0]}: {self.basename(self.replace(cmd)).split()[0]}: file with this name already exists")
 		except IsADirectoryError: return print(f"{cmd.split()[0]}: {self.basename(self.replace(cmd)).split()[0]}: is a directory")
 		except NotADirectoryError: return print(f"{cmd.split()[0]}: {self.basename(self.replace(cmd).split()[0])}: not a directory")
 		except UnicodeDecodeError: return print(f"{cmd.split()[0]}: {self.basename(self.replace(cmd).split()[0])}: is a binary-like file.")
-		except IndexError as missing: print(f"{cmd.split()[0]}: missing operand [{missing}]...")
 		except PermissionError: return print(f"{cmd.split()[0]}: permission denied")
-
 		
-		return True, self.rmprocess(cmd)
+		return True, self.rmprocess(cmd.split()[0])
 			
 	# OpenTTY "Text API"
 	def basename(self, path): return os.path.basename(path)
 	def replace(self, text): return ' '.join(text.split()[1:])
 	
 	def recognize(self, text):
 		self.values = {
@@ -346,42 +339,44 @@
 	
 	# OpenTTY "Process Methods"
 	def mkprocess(self, pname): self.process[pname] = str(randint(1000, 9999))
 	def rmprocess(self, pname): 
 		try: 
 			if pname in ['sh', 'python']: return 
 
-			del self.process[pname.split()[0]]
-		except Exception as error: return
+			del self.process[pname]
+		except KeyError: return
 	
 	def pslist(self):
 		print(f"     PID  CMD")
 		for process in self.process:
 			print(f"    {self.process[process]}  {process}")
+
+		return self.process
 	def kill(self, pid):
 		for process in self.process:
 			if self.process[process] == str(pid): 
 				del self.process[process]
 
 				return True
 		
 		print(f"kill: ({pid}) - No such process" if pid else f"kill: missing operand [PID]...")
 
 	# OpenTTY "Applications"
 	#
 	# [File Utilities]
 	def makedir(self, dirname):
 		if dirname: os.makedirs(dirname)
-		else: raise IndexError("dirname")
+		else: print(f"mkdir: missing operand [dirname]...")
 	def removedir(self, dirname):
 		if dirname: shutil.rmtree(dirname)
-		else: raise IndexError("dirname")
+		else: print(f"rmdir: missing operand [dirname]...")
 	def remove(self, filename):
 		if filename != "": os.remove(filename)
-		else: raise IndexError("filename")
+		else: print(f"rm: missing operand [filename]...")
 	def listdir(self, path=""):
 		if path:
 			files = os.listdir(path)
 
 			for file in files:
 				if file.startswith(library['hidden-files-prefix']): continue
 				elif os.path.isfile(f"{path}/{file}"):
@@ -399,15 +394,15 @@
 		def writeBytes(source, output): 
 			with open(source, "r") as source: text = source.read()
 			with open(output, "wb") as output: output.write(hashbytes(text))
 
 			return len(hashbytes(text)), len(text.splitlines())
 
 		if len(shlex.split(filenames)) < 2:
-			if filenames: raise IndexError("output")
+			if filenames: return print("dd: missing operand [output]...")
 
 			text = []
 
 			for _ in range(library['max-byte-len']):
 				try: text.append(input())
 				except (KeyboardInterrupt, EOFError): return print(f"\n0+{len(hashbytes(text))} record in\n0+{randint(0, 1)} record out")
 				
@@ -423,74 +418,74 @@
 					print("File List:")
 					print("--------------------------------------------\n")
 					for file in zip_file.filelist:
 						print(f"- {file.filename}")
 
 			except zipfile.BadZipFile: print(f"zipinfo: {zip_path}: zip file is invalid or corromped")
 			except zipfile.LargeZipFile: print(f"zipinfo: {zip_path}: zip file is too Large")
-		else: raise IndexError("filename")
+		else: print("zipinfo: missing operand [filename]...")
 	def unzip(self, cmdline):
-		if len(shlex.split(cmdline)) < 2: raise IndexError("extract path" if cmdline != "" else "archive >> path")
+		if len(shlex.split(cmdline)) < 2: return print("unzip: missing operand [extract path]..." if cmdline != "" else "unzip: missing operand [archive >> path]...")
 		
 		with zipfile.ZipFile(shlex.split(cmdline)[0], 'r') as zf:
 			try: zf.extractall(shlex.split(cmdline)[1])
 			except Exception as traceback: print(traceback)
 	def touch(self, filename): 
 		if filename: open(filename, "wt+").close()
-		else: raise IndexError("filename")
+		else: print("touch: missing operand [filename]... ")
 	def tree(self, directory, indent=""):
 		if directory:
 			print(indent + os.path.basename(directory))
 			if os.path.isdir(directory):
 				indent += "│   "
 				files = os.listdir(directory)
 				for file in sorted(files):
 					path = os.path.join(directory, file)
 
 					self.tree(path, indent)
 
 		else: self.tree(".")
 	def move(self, cmdline=""): 
 		if cmdline:
-			if len(shlex.split(cmdline)) < 2: raise IndexError("new.path")
+			if len(shlex.split(cmdline)) < 2: return print(f"mv: {cmdline}: missing operand [new path]...")
 
 			shutil.move(shlex.split(cmdline)[0], shlex.split(cmdline)[1])
 
-		else: raise IndexError("sorce >> path")
+		else: print(f"mv: missing operand [source >> path]...")
 	def copy(self, cmdline=""): 
 		if cmdline:
-			if len(shlex.split(cmdline)) < 2: raise IndexError("copy.path")
+			if len(shlex.split(cmdline)) < 2: return print(f"cp: {cmdline}: missing operand [copy.path]...")
 
 			shutil.copy(shlex.split(cmdline)[0], shlex.split(cmdline)[1])
 
-		else: raise IndexError("source >> copy")
+		else: print(f"cp: missing operand [source >> copy]...")
 	def gunzip(self, cmdline):
 		if cmdline:
-			if len(shlex.split(cmdline)) < 2: raise IndexError("source: folder | file")
+			if len(shlex.split(cmdline)) < 2: return print(f"gzip: missing operand [source: folder | file]...")
 				
 			zip_filename = shlex.split(cmdline)[0]
 			source_path = shlex.split(cmdline)[1]
 			
 			if os.path.isfile(source_path):
 				with zipfile.ZipFile(zip_filename, 'w') as zipf:
 					zipf.write(source_path, os.path.basename(source_path))
 			elif os.path.isdir(source_path):
 				with zipfile.ZipFile(zip_filename, 'w') as zipf:
 					for foldername, subfolders, filenames in os.walk(source_path):
 						for filename in filenames:
 							file_path = os.path.join(foldername, filename)
 							zipf.write(file_path, os.path.relpath(file_path, source_path))
 
-		else: raise IndexError("filename << source")
+		else: print(f"gzip: missing operand [filename << source]...")
 	def install(self, filename):
 		if filename: 
 			if self.basename(filename) in library['whitelist']: return shutil.copy(filename, f"{self.root}/{self.basename(filename)}")
 			else: raise PermissionError
 		
-		raise IndexError("filename")
+		print("install: missing operand [filename]...")
 	#
 	# [Text Utilities]
 	def catfile(self, filename): 
 		if filename: print(self.recognize(open(filename, "r").read()))
 		else: self.ThreadIn()
 	def headfile(self, filename): 
 		if filename != "":
@@ -531,15 +526,15 @@
 					if jsondata:
 						print(f"Key mapper for JSON File: \033[1m[{filename}]\033[m\n")
 						explore_json(jsondata, indent)
 
 			except json.decoder.JSONDecodeError as traceback: print(f"json: file is malformed [{traceback}]")
 		
 		elif jsoniten: explore_json(jsoniten, indent)
-		else: raise IndexError("filename")
+		else: print(f"json: missing operand [filename]...")
 	def nl(self, filename):
 		if filename:
 			with open(filename, "r") as file:
 				line_number = 1
 				for line in file:
 					print(f"   {line_number}\t{line}", end="")
 					line_number += 1
@@ -556,15 +551,15 @@
 					else:
 						return ''.join(lines[-library['head-lines']:])
 
 			print(tailrepliant(filename))
 
 		else: self.ThreadIn()
 	def diff(self, filenames):
-		if len(shlex.split(filenames)) < 2: raise IndexError("2filename" if filenames else "filename <> filename")
+		if len(shlex.split(filenames)) < 2: return print("diff: missing operand [2filename]..." if filenames else "diff: missing operand [filename <> filename]...")
 			
 		print(shlex.split(filenames)[0])
 		print(shlex.split(filenames)[1])
 
 		lines1 = open(shlex.split(filenames)[0], "r").readlines()
 		lines2 = open(shlex.split(filenames)[1], "r").readlines()
 
@@ -577,14 +572,24 @@
 	# [Envirronment Utilities]
 	def environ(self, key=""):
 		if key: print(os.environ[key] if key in os.environ else f"env: {key}: register not found")
 		else: self.ThreadList(os.environ)
 	def export(self, cmdline=""):
 		if cmdline: os.environ[cmdline.split()[0]] = self.replace(cmdline)
 		else: print('from opentty import *\n\n\nif __name__ == "__main__":\n\tapp = OpenTTY()\n\n\tapp.connect("localhost")\n\tapp.disconnect(0)')
+	def set(self, cmdline):
+		if cmdline:
+			if len(cmdline.split()) < 2:
+				print(f"local {cmdline}='{self.locals[cmdline]}'" if cmdline in self.locals else f"set: {cmdline}: value not found")
+
+				return False
+
+			self.locals[cmdline.split()[0]] = self.replace(cmdline)
+		
+		else: self.ThreadList(self.locals)
 	def uname(self, argv=""):
 		if argv:
 			if "-a" in argv: print(f"{platform.system()} {platform.node()} {platform.release()} {platform.version()} {platform.machine()}")
 
 			elif "-s" in argv: print(platform.system()) 
 			elif "-n" in argv: print(platform.node()) 
 			elif "-r" in argv: print(platform.release()) 
@@ -621,14 +626,15 @@
 		if alias:
 			try: del self.aliases[alias]
 			except KeyError: print(f"unalias: {alias}: alias not found")
 		else: print("unalias: usage: unalias [-a] name [name ...]")	
 	def diskfree(self, cmdline=""):
 		if os.name == "posix": os.system(f"df {cmdline}")
 		elif os.name == "nt": os.system("wmic logicaldisk get deviceid,size,freespace")
+		else: print(f"df: this tool doesnt support {platform.system()} systems")
 	def status(self):
 		try: package = json.load(urllib.request.urlopen(library['sync']))
 		except Exception as traceback: return print("status: failed to connect with github.")
 
 		if package['version'] != library['version']: return print(f"status: a new version of {self.appname} was released.")
 		elif package['build'] != library['build']: return print(f"status: a new snapshot of {self.appname} was released.")
 		else: print(f"status: {self.appname} is up-to-date.")
@@ -660,15 +666,16 @@
 
 		else: print(f"sync: {self.appname} is up-to-date.")	
 	def venv(self, venvname):
 		if venvname:
 			try: urllib.request.urlretrieve(library['venv'], f"{self.root}/{venvname}.py")
 			except Exception as traceback: print("venv: bad. download of template failed.")
 		
-		else: raise IndexError("profile.name")
+		else: print("venv: missing operand [profile.name]...")
+	#
 	# [Asset Manager]
 	def asset(self):
 		root_files = os.listdir(self.root)
 		assets = []
 
 		for file in root_files:
 			if file.startswith(library['hidden-files-prefix']): continue
@@ -678,38 +685,37 @@
 
 		for asset in assets: print(f"    {asset}")
 	def get_asset(self, asset):
 		if asset:
 			for resource in asset.split():
 				try: urllib.request.urlretrieve(library['resources'][resource]['url'], f"{self.root}/{library['resources'][resource]['filename']}"), print(f"get: asset '{resource}' installed.")
 				except Exception as traceback: print(f"get: bad. asset installation failed.")
-				
-		else: raise IndexError("asset")
+		else: print("get: missing operand [asset]...")
 	def build(self, filename, root=False):
 		if filename: 
 			if self.basename(filename) not in library['whitelist'] and not root: raise PermissionError
 
 			with open(filename, "r") as script:
 				script = script.read().splitlines()
 
 				self.functions[self.basename(filename).split(".")[0].replace(" ", ".")] = script
 
-		else: raise IndexError("script")
+		else: print("build: missing operand [script]...")
 	def function(self, function):
 		if function:
 			commands = []
 
 			while True:
 				try: commands.append(input(f"\033[1m\033[31m[{library['profile']}]\033[m >>> ").strip())
 				except (KeyboardInterrupt, EOFError): break
 
 			self.functions[function.replace(" ", ".")] = commands
 			print()
 		
-		else: raise IndexError("method.name")
+		else: print("function: missing operand [method.name]...")
 	
 	def callmethod(self, function):
 		if function in self.functions:
 
 			for cmd in self.functions[function]:
 				if cmd:
 					if cmd.startswith("#"): run = True
@@ -742,19 +748,19 @@
 				socket.inet_aton(ipadress)
 				ip_info = get_ip_info(ipadress)
 
 				if ip_info:
 					for key, value in ip_info.items(): print(f"{key}: {value}")
 			except socket.error: print(f"fw: {ipadress}: ip adress is invalid.")
 
-		else: raise IndexError("ip.adress")
+		else: print("fw: missing operand [ip adress]...")
 	def wget(self, cmdline):
 		if len(cmdline.split()) < 2:
 			if cmdline: return self.wget(f"{cmdline} {self.basename(cmdline)}")
-			else: raise IndexError("url")
+			else: return print("wget: missing operand [url]...")
 
 		try: urllib.request.urlretrieve(cmdline.split()[0], self.replace(cmdline)), print(f"wget: {self.replace(cmdline)}: download complete.")
 		except urllib.error.URLError: return print("wget: the url is inacessible or invalid")
 		except urllib.error.HTTPError: return print("wget: page not found or url is inacessible")
 		except socket.timeout: return print("wget: timeout: server dont answer your request")
 		except FileNotFoundError: return print("wget: path for save file was not found")
 	def server(self, port):
@@ -773,29 +779,30 @@
 			try: html = urllib.request.urlopen(url).read().decode()
 			except Exception as traceback: return print(f"{report}: {tbmsg}")
 
 			if show: print(self.recognize(html))
 			
 			return html
 		
-		else: raise IndexError("url")
+		else: print(f"{report}: missing operand [url]...")
 	#
 	# [Other Utilities]
 	def calendar(self): 
 		now = datetime.datetime.now()
 
 		calendar.setfirstweekday(calendar.SUNDAY), print(calendar.month(now.year, now.month), end="")
 	def sleep(self, time):
 		try: timeout(int(time))
-		except ValueError: print(f"sleep: invalid time interval '{time}'" if time else f"sleep: missing operand [delay]...")
+		except ValueError: print(f"sleep: invalid time interval '{time}'" if time else f"sleep: missing operand [delay: sec]...")
 	def sequence(self, limit): 
 		if limit:
 			try: cache = int(limit) + 1
 			except: print(f"seq: range need be a int number")
 			else:
 				for i in range(cache):
 					if i != 0: print(i)
 
+
 if __name__ == "__main__":
 	app = OpenTTY()
 	
 	app.connect("localhost")
```

### Comparing `opentty-1.0/setup.py` & `opentty-1.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='opentty',
-    version='1.0',
+    version='1.0rc4',
     author='Mr. Lima',
     author_email='felipebr4095@gmail.com',
     description='The OpenTTY is a Terminal Emulator created tottaly in python based-on Unix-Like Shells',
     long_description='For more informations see README at Github',
     long_description_content_type='text/markdown',
     url='https://github.com/fetuber4095/OpenTTY',
     packages=['.'],
```

