# Comparing `tmp/hassmpris_client-0.0.8.tar.gz` & `tmp/hassmpris_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassmpris_client-0.0.8.tar", last modified: Fri Jun 24 15:12:17 2022, max compression
+gzip compressed data, was "hassmpris_client-0.0.9.tar", last modified: Mon Jun 27 22:39:17 2022, max compression
```

## Comparing `hassmpris_client-0.0.8.tar` & `hassmpris_client-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:17.562127 hassmpris_client-0.0.8/
--rw-rw-r--   0 user      (1000) user      (1000)      251 2022-06-23 02:06:01.000000 hassmpris_client-0.0.8/Jenkinsfile
--rw-rw-r--   0 user      (1000) user      (1000)      181 2022-06-23 02:06:01.000000 hassmpris_client-0.0.8/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)      123 2022-06-23 23:27:59.000000 hassmpris_client-0.0.8/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)      923 2022-06-24 15:12:17.562127 hassmpris_client-0.0.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      505 2022-06-23 02:06:01.000000 hassmpris_client-0.0.8/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       21 2022-06-23 02:06:01.000000 hassmpris_client-0.0.8/build.parameters
--rw-rw-r--   0 user      (1000) user      (1000)     1674 2022-06-24 14:48:46.000000 hassmpris_client-0.0.8/hassmpris-client.spec
--rw-rw-r--   0 user      (1000) user      (1000)      656 2022-06-24 04:22:53.000000 hassmpris_client-0.0.8/mypy.ini
--rw-rw-r--   0 user      (1000) user      (1000)       85 2022-06-23 02:06:01.000000 hassmpris_client-0.0.8/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)      793 2022-06-24 15:12:17.563127 hassmpris_client-0.0.8/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:17.559127 hassmpris_client-0.0.8/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:17.561127 hassmpris_client-0.0.8/src/hassmpris_client/
--rw-rw-r--   0 user      (1000) user      (1000)    14626 2022-06-24 14:53:25.000000 hassmpris_client-0.0.8/src/hassmpris_client/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:17.562127 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      923 2022-06-24 15:12:16.000000 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      460 2022-06-24 15:12:17.000000 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-06-24 15:12:16.000000 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       59 2022-06-24 15:12:17.000000 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       84 2022-06-24 15:12:17.000000 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2022-06-24 15:12:17.000000 hassmpris_client-0.0.8/src/hassmpris_client.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:17.562127 hassmpris_client-0.0.8/tests/
--rw-rw-r--   0 user      (1000) user      (1000)      745 2022-06-23 02:06:01.000000 hassmpris_client-0.0.8/tests/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)       35 2022-06-23 02:17:08.000000 hassmpris_client-0.0.8/tests/test_dummy.py
--rw-rw-r--   0 user      (1000) user      (1000)      220 2022-06-24 14:46:30.000000 hassmpris_client-0.0.8/tox.ini
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:39:17.939036 hassmpris_client-0.0.9/
+-rw-rw-r--   0 user      (1000) user      (1000)      251 2022-06-23 02:06:01.000000 hassmpris_client-0.0.9/Jenkinsfile
+-rw-rw-r--   0 user      (1000) user      (1000)      181 2022-06-23 02:06:01.000000 hassmpris_client-0.0.9/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)      123 2022-06-23 23:27:59.000000 hassmpris_client-0.0.9/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      923 2022-06-27 22:39:17.939036 hassmpris_client-0.0.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      505 2022-06-23 02:06:01.000000 hassmpris_client-0.0.9/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       21 2022-06-23 02:06:01.000000 hassmpris_client-0.0.9/build.parameters
+-rw-rw-r--   0 user      (1000) user      (1000)     1674 2022-06-27 22:29:10.000000 hassmpris_client-0.0.9/hassmpris-client.spec
+-rw-rw-r--   0 user      (1000) user      (1000)      656 2022-06-24 04:22:53.000000 hassmpris_client-0.0.9/mypy.ini
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2022-06-23 02:06:01.000000 hassmpris_client-0.0.9/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      794 2022-06-27 22:39:17.939036 hassmpris_client-0.0.9/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:39:17.935037 hassmpris_client-0.0.9/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:39:17.937037 hassmpris_client-0.0.9/src/hassmpris_client/
+-rw-rw-r--   0 user      (1000) user      (1000)    14811 2022-06-27 22:38:50.000000 hassmpris_client-0.0.9/src/hassmpris_client/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:39:17.937037 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      923 2022-06-27 22:39:17.000000 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      460 2022-06-27 22:39:17.000000 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-06-27 22:39:17.000000 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2022-06-27 22:39:17.000000 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2022-06-27 22:39:17.000000 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2022-06-27 22:39:17.000000 hassmpris_client-0.0.9/src/hassmpris_client.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:39:17.938037 hassmpris_client-0.0.9/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)      745 2022-06-23 02:06:01.000000 hassmpris_client-0.0.9/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)       35 2022-06-23 02:17:08.000000 hassmpris_client-0.0.9/tests/test_dummy.py
+-rw-rw-r--   0 user      (1000) user      (1000)      221 2022-06-27 22:29:34.000000 hassmpris_client-0.0.9/tox.ini
```

### Comparing `hassmpris_client-0.0.8/PKG-INFO` & `hassmpris_client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassmpris_client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple command-line client to control the MPRIS multimedia agent
 Home-page: https://github.com/Rudd-O/hassmpris
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Description-Content-Type: text/markdown
```

### Comparing `hassmpris_client-0.0.8/hassmpris-client.spec` & `hassmpris_client-0.0.9/hassmpris-client.spec`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 %define dunder_name hassmpris_client
 %define _name hassmpris-client
 
 %define mybuildnumber %{?build_number}%{?!build_number:1}
 
 Name:           python-%{_name}
-Version:        0.0.8
+Version:        0.0.9
 Release:        %{mybuildnumber}%{?dist}
 Summary:        Simple command-line client to control the MPRIS multimedia agent
 
 License:        LGPLv2.1
 URL:            https://github.com/Rudd-O/%{dunder_name}
 Source:         %{url}/archive/v%{version}/%{dunder_name}-%{version}.tar.gz
```

### Comparing `hassmpris_client-0.0.8/mypy.ini` & `hassmpris_client-0.0.9/mypy.ini`

 * *Files identical despite different names*

### Comparing `hassmpris_client-0.0.8/setup.cfg` & `hassmpris_client-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [options]
 install_requires = 
 	cryptography
 	blindecdh>=0.1.8
 	shortauthstrings>=0.1.8
 	cakes>=0.1.6
-	hassmpris>=0.1.8
+	hassmpris>=0.1.10
 package_dir = 
 	= src
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	hassmpris-client = hassmpris_client:main
```

### Comparing `hassmpris_client-0.0.8/src/hassmpris_client/__init__.py` & `hassmpris_client-0.0.9/src/hassmpris_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 from hassmpris.proto import mpris_pb2  # noqa: E402
 import hassmpris.certs as certs  # noqa: E402
 
 from hassmpris import config  # noqa: E402
 
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_TIMEOUT = 15.0
 
 
 Ignored = cakes.Ignored
@@ -129,14 +129,16 @@
             return await f(*args)
         except ssl.SSLCertVerificationError as e:
             raise Unauthenticated(e)
         except ConnectionRefusedError as e:
             raise CannotConnect(e)
         except OSError as e:
             raise CannotConnect(e)
+        except grpclib.exceptions.StreamTerminatedError as e:
+            raise Disconnected(e)
         except asyncio.exceptions.TimeoutError as e:
             raise Timeout(e)
 
     return cast(StubFunc, inner)
 
 
 def normalize_connection_errors_iterable(f: StubFunc) -> StubFunc:
@@ -147,14 +149,16 @@
                 yield x
         except ssl.SSLCertVerificationError as e:
             raise Unauthenticated(e)
         except ConnectionRefusedError as e:
             raise CannotConnect(e)
         except OSError as e:
             raise CannotConnect(e)
+        except asyncio.exceptions.CancelledError as e:
+            raise Disconnected(e)
         except grpclib.exceptions.StreamTerminatedError as e:
             raise Disconnected(e)
         except asyncio.exceptions.TimeoutError as e:
             raise Timeout(e)
 
     return cast(StubFunc, inner)
```

### Comparing `hassmpris_client-0.0.8/src/hassmpris_client.egg-info/PKG-INFO` & `hassmpris_client-0.0.9/src/hassmpris_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassmpris-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple command-line client to control the MPRIS multimedia agent
 Home-page: https://github.com/Rudd-O/hassmpris
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Description-Content-Type: text/markdown
```

### Comparing `hassmpris_client-0.0.8/tests/conftest.py` & `hassmpris_client-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

