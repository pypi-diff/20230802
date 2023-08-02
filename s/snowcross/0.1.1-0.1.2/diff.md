# Comparing `tmp/snowcross-0.1.1.tar.gz` & `tmp/snowcross-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowcross-0.1.1.tar", last modified: Tue Aug  1 05:13:13 2023, max compression
+gzip compressed data, was "snowcross-0.1.2.tar", last modified: Wed Aug  2 03:31:13 2023, max compression
```

## Comparing `snowcross-0.1.1.tar` & `snowcross-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:13:13.479106 snowcross-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 05:12:46.000000 snowcross-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 05:12:46.000000 snowcross-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 05:13:13.479106 snowcross-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 05:12:46.000000 snowcross-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 05:12:46.000000 snowcross-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 05:12:46.000000 snowcross-0.1.1/requirements-locator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 05:12:46.000000 snowcross-0.1.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 05:12:46.000000 snowcross-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:13:13.479106 snowcross-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 05:12:46.000000 snowcross-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:13:13.479106 snowcross-0.1.1/snowcross/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:12:46.000000 snowcross-0.1.1/snowcross/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-08-01 05:12:46.000000 snowcross-0.1.1/snowcross/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 05:12:46.000000 snowcross-0.1.1/snowcross/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-01 05:12:46.000000 snowcross-0.1.1/snowcross/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-08-01 05:12:46.000000 snowcross-0.1.1/snowcross/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:13:13.479106 snowcross-0.1.1/snowcross.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 05:13:13.000000 snowcross-0.1.1/snowcross.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 05:13:13.000000 snowcross-0.1.1/snowcross.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:13:13.000000 snowcross-0.1.1/snowcross.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 05:13:13.000000 snowcross-0.1.1/snowcross.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 05:13:13.000000 snowcross-0.1.1/snowcross.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:13:13.479106 snowcross-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:13:13.479106 snowcross-0.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:12:46.000000 snowcross-0.1.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-01 05:12:46.000000 snowcross-0.1.1/tests/fixtures/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-01 05:12:46.000000 snowcross-0.1.1/tests/fixtures/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:13:13.479106 snowcross-0.1.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:12:46.000000 snowcross-0.1.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-01 05:12:46.000000 snowcross-0.1.1/tests/helpers/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:31:13.004945 snowcross-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 03:30:46.000000 snowcross-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 03:30:46.000000 snowcross-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-02 03:31:13.004945 snowcross-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 03:30:46.000000 snowcross-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-02 03:30:46.000000 snowcross-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 03:30:46.000000 snowcross-0.1.2/requirements-locator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 03:30:46.000000 snowcross-0.1.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 03:30:46.000000 snowcross-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 03:31:13.004945 snowcross-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-02 03:30:46.000000 snowcross-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:31:13.000944 snowcross-0.1.2/snowcross/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 03:30:46.000000 snowcross-0.1.2/snowcross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-08-02 03:30:46.000000 snowcross-0.1.2/snowcross/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 03:30:46.000000 snowcross-0.1.2/snowcross/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-02 03:30:46.000000 snowcross-0.1.2/snowcross/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-08-02 03:30:46.000000 snowcross-0.1.2/snowcross/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:31:13.004945 snowcross-0.1.2/snowcross.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-02 03:31:12.000000 snowcross-0.1.2/snowcross.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-02 03:31:13.000000 snowcross-0.1.2/snowcross.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 03:31:12.000000 snowcross-0.1.2/snowcross.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 03:31:12.000000 snowcross-0.1.2/snowcross.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 03:31:12.000000 snowcross-0.1.2/snowcross.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:31:13.000944 snowcross-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:31:13.004945 snowcross-0.1.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 03:30:46.000000 snowcross-0.1.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-02 03:30:46.000000 snowcross-0.1.2/tests/fixtures/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-02 03:30:46.000000 snowcross-0.1.2/tests/fixtures/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:31:13.004945 snowcross-0.1.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 03:30:46.000000 snowcross-0.1.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 03:30:46.000000 snowcross-0.1.2/tests/helpers/docker.py
```

### Comparing `snowcross-0.1.1/LICENSE` & `snowcross-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/PKG-INFO` & `snowcross-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `snowcross-0.1.1/README.md` & `snowcross-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/setup.py` & `snowcross-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/snowcross/aws.py` & `snowcross-0.1.2/snowcross/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/snowcross/errors.py` & `snowcross-0.1.2/snowcross/errors.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/snowcross/locator.py` & `snowcross-0.1.2/snowcross/locator.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/snowcross/snowflake.py` & `snowcross-0.1.2/snowcross/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,35 +17,40 @@
 
 
 @contextlib.contextmanager
 def connection(
     password: Optional[str] = None,
     private_key_path: Optional[str] = None,
     private_key_passphrase: Optional[str] = None,
+    allow_privatelink: bool = True,
     **kwargs,
 ) -> Iterator[sc.SnowflakeConnection]:
     """Establish connection to Snowflake.
 
     Args:
         password (Optional[str], optional): Password (do not specify with private key). Defaults to None.
         private_key_path (Optional[str], optional): Path to private key file (do not specify with password). Defaults to None.
         private_key_passphrase (Optional[str], optional): Passcode to decrypt private key file, if encrypted (do not specify with password). Defaults to None.
+        allow_privatelink (bool): PrivateLink enabled. Defaults to True.
 
     Yields:
         Iterator[sc.SnowflakeConnection]: Snowflake connection context.
     """
     conn_args = connection_args(
         password=password,
         private_key_path=private_key_path,
         private_key_passphrase=private_key_passphrase,
         **kwargs,
     )
 
     sc.paramstyle = "format"
 
+    if not allow_privatelink:
+        conn_args["account"] = conn_args["account"].replace(".privatelink", "")
+
     try:
         conn = sc.connect(**conn_args)
         yield conn
     finally:
         conn.close()
```

### Comparing `snowcross-0.1.1/snowcross.egg-info/PKG-INFO` & `snowcross-0.1.2/snowcross.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `snowcross-0.1.1/tests/fixtures/aws.py` & `snowcross-0.1.2/tests/fixtures/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.1/tests/fixtures/snowflake.py` & `snowcross-0.1.2/tests/fixtures/snowflake.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,22 @@
         os.environ["SNOWFLAKE_ACCOUNT"] = "test_account"
         os.environ["SNOWFLAKE_PASSWORD"] = "test_password"
         os.environ["SNOWFLAKE_USERNAME"] = "test_username"
     yield
 
 
 @pytest.fixture(scope="module")
+def fixture_snowflake_credentials_private_link():
+    """Mocked Snowflake Credentials. Ignored if environment variables have been set."""
+    os.environ["SNOWFLAKE_ACCOUNT"] = "test_account.privatelink"
+    os.environ["SNOWFLAKE_PASSWORD"] = "test_password"
+    os.environ["SNOWFLAKE_USERNAME"] = "test_username"
+
+
+@pytest.fixture(scope="module")
 def fixture_snowflake_credentials_ssm():
     """Mocked Snowflake SSM Credentials. Ignored if environment variables have been set."""
     if not os.environ.get("SNOWFLAKE_ACCOUNT"):
         os.environ["SNOWFLAKE_ACCOUNT"] = "boto+ssm:test/snowflake/account"
         os.environ["SNOWFLAKE_PASSWORD"] = "boto+ssm:test/snowflake/password"
         os.environ["SNOWFLAKE_USERNAME"] = "boto+ssm:test/snowflake/username"
     yield
```

### Comparing `snowcross-0.1.1/tests/helpers/docker.py` & `snowcross-0.1.2/tests/helpers/docker.py`

 * *Files identical despite different names*

