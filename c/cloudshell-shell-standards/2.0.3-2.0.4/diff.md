# Comparing `tmp/cloudshell-shell-standards-2.0.3.zip` & `tmp/cloudshell-shell-standards-2.0.4.zip`

## zipinfo {}

```diff
@@ -1,70 +1,70 @@
-Zip file size: 57893 bytes, number of entries: 68
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/
--rw-r--r--  2.0 unx      908 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/README.md
--rw-r--r--  2.0 unx       18 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/test_requirements.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/version.txt
--rw-r--r--  2.0 unx    97622 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/LICENSE.htm
--rw-r--r--  2.0 unx       34 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/MANIFEST.in
--rw-r--r--  2.0 unx       93 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/requirements.txt
--rw-r--r--  2.0 unx      288 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/PKG-INFO
--rw-r--r--  2.0 unx      810 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/setup.py
--rw-r--r--  2.0 unx       71 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/dev_requirements.txt
--rw-r--r--  2.0 unx     1295 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tox.ini
--rw-r--r--  2.0 unx       38 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/setup.cfg
--rw-r--r--  2.0 unx        1 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       93 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/top_level.txt
--rw-r--r--  2.0 unx      288 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     2285 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/
--rw-r--r--  2.0 unx     1803 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/conftest.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/__init__.py
--rw-r--r--  2.0 unx     2248 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/test_autoload_generic_models.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/__init__.py
--rw-r--r--  2.0 unx     8480 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/test_autoload_details_builder.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/
--rw-r--r--  2.0 unx     3160 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/
--rw-r--r--  2.0 unx     1205 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/test_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/__init__.py
--rw-r--r--  2.0 unx     1574 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
--rw-r--r--  2.0 unx     3697 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
--rw-r--r--  2.0 unx      509 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/
--rw-r--r--  2.0 unx       76 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/
--rw-r--r--  2.0 unx       76 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/
--rw-r--r--  2.0 unx     1529 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/attribute_names.py
--rw-r--r--  2.0 unx      178 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/exceptions.py
--rw-r--r--  2.0 unx     4027 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/resource_config_generic_models.py
--rw-r--r--  2.0 unx       76 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/__init__.py
--rw-r--r--  2.0 unx     8113 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/autoload_generic_models.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/
--rw-r--r--  2.0 unx      113 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/namespace_type.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/__init__.py
--rw-r--r--  2.0 unx     1802 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/utils.py
--rw-r--r--  2.0 unx      361 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/enum.py
--rw-r--r--  2.0 unx     3069 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
--rw-r--r--  2.0 unx     1847 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/resource_attr.py
--rw-r--r--  2.0 unx     2092 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/base_conf.py
--rw-r--r--  2.0 unx      316 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/__init__.py
--rw-r--r--  2.0 unx     4551 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
--rw-r--r--  2.0 unx     3712 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_getter.py
--rw-r--r--  2.0 unx     5626 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/resource_model.py
--rw-r--r--  2.0 unx     3641 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/existed_resource_info.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/__init__.py
--rw-r--r--  2.0 unx     4961 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/core_entities.py
--rw-r--r--  2.0 unx     5207 b- defN 23-May-12 13:09 cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/utils.py
-68 files, 177916 bytes uncompressed, 42887 bytes compressed:  75.9%
+Zip file size: 58125 bytes, number of entries: 68
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/
+-rw-r--r--  2.0 unx       93 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/requirements.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/setup.cfg
+-rw-r--r--  2.0 unx       71 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/dev_requirements.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/version.txt
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/PKG-INFO
+-rw-r--r--  2.0 unx       18 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/test_requirements.txt
+-rw-r--r--  2.0 unx       34 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/MANIFEST.in
+-rw-r--r--  2.0 unx      908 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/README.md
+-rw-r--r--  2.0 unx    97622 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/LICENSE.htm
+-rw-r--r--  2.0 unx      810 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/setup.py
+-rw-r--r--  2.0 unx     1295 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tox.ini
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     2285 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       93 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/
+-rw-r--r--  2.0 unx     1803 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/conftest.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/__init__.py
+-rw-r--r--  2.0 unx     2248 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/test_autoload_generic_models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/__init__.py
+-rw-r--r--  2.0 unx     8480 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/test_autoload_details_builder.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/
+-rw-r--r--  2.0 unx     3160 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/
+-rw-r--r--  2.0 unx     1205 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/test_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/__init__.py
+-rw-r--r--  2.0 unx      509 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
+-rw-r--r--  2.0 unx     2236 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
+-rw-r--r--  2.0 unx     3859 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/
+-rw-r--r--  2.0 unx       76 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/
+-rw-r--r--  2.0 unx     1529 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/attribute_names.py
+-rw-r--r--  2.0 unx     8113 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/autoload_generic_models.py
+-rw-r--r--  2.0 unx     4027 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/resource_config_generic_models.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/__init__.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/exceptions.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/
+-rw-r--r--  2.0 unx     1802 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/utils.py
+-rw-r--r--  2.0 unx      113 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/namespace_type.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/__init__.py
+-rw-r--r--  2.0 unx     5626 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/resource_model.py
+-rw-r--r--  2.0 unx     4961 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/core_entities.py
+-rw-r--r--  2.0 unx     3641 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/existed_resource_info.py
+-rw-r--r--  2.0 unx     5207 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/__init__.py
+-rw-r--r--  2.0 unx      361 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/enum.py
+-rw-r--r--  2.0 unx     3069 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
+-rw-r--r--  2.0 unx     2092 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/base_conf.py
+-rw-r--r--  2.0 unx     3737 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_getter.py
+-rw-r--r--  2.0 unx      316 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/__init__.py
+-rw-r--r--  2.0 unx     1847 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/resource_attr.py
+-rw-r--r--  2.0 unx     4551 b- defN 23-Aug-02 14:02 cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
+68 files, 178765 bytes uncompressed, 43119 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,205 +1,205 @@
-Filename: cloudshell-shell-standards-2.0.3/
+Filename: cloudshell-shell-standards-2.0.4/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/
+Filename: cloudshell-shell-standards-2.0.4/tests/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/README.md
+Filename: cloudshell-shell-standards-2.0.4/requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/test_requirements.txt
+Filename: cloudshell-shell-standards-2.0.4/setup.cfg
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/version.txt
+Filename: cloudshell-shell-standards-2.0.4/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/LICENSE.htm
+Filename: cloudshell-shell-standards-2.0.4/version.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/MANIFEST.in
+Filename: cloudshell-shell-standards-2.0.4/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/requirements.txt
+Filename: cloudshell-shell-standards-2.0.4/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/PKG-INFO
+Filename: cloudshell-shell-standards-2.0.4/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/setup.py
+Filename: cloudshell-shell-standards-2.0.4/README.md
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/dev_requirements.txt
+Filename: cloudshell-shell-standards-2.0.4/LICENSE.htm
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tox.ini
+Filename: cloudshell-shell-standards-2.0.4/setup.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/setup.cfg
+Filename: cloudshell-shell-standards-2.0.4/tox.ini
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/dependency_links.txt
+Filename: cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/requires.txt
+Filename: cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/top_level.txt
+Filename: cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/PKG-INFO
+Filename: cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/SOURCES.txt
+Filename: cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/conftest.py
+Filename: cloudshell-shell-standards-2.0.4/tests/conftest.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/test_autoload_generic_models.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/test_autoload_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/test_autoload_details_builder.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/test_autoload_details_builder.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/test_resource_config_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/test_utils.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/test_utils.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_enum.py
+Filename: cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/attribute_names.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/attribute_names.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/exceptions.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/autoload_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/resource_config_generic_models.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/resource_config_generic_models.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/autoload_generic_models.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/exceptions.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/namespace_type.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/utils.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/namespace_type.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/utils.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/enum.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/resource_model.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/core_entities.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/resource_attr.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/existed_resource_info.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/base_conf.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/utils.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/enum.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_getter.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_converters.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/resource_model.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/base_conf.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/existed_resource_info.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_getter.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/__init__.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/core_entities.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/resource_attr.py
 Comment: 
 
-Filename: cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/utils.py
+Filename: cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_converter.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-shell-standards-2.0.3/README.md` & `cloudshell-shell-standards-2.0.4/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/LICENSE.htm` & `cloudshell-shell-standards-2.0.4/LICENSE.htm`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/setup.py` & `cloudshell-shell-standards-2.0.4/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tox.ini` & `cloudshell-shell-standards-2.0.4/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell_shell_standards.egg-info/SOURCES.txt` & `cloudshell-shell-standards-2.0.4/cloudshell_shell_standards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tests/conftest.py` & `cloudshell-shell-standards-2.0.4/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/test_autoload_generic_models.py` & `cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/test_autoload_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tests/cloudshell/shell_standards/test_autoload_details_builder.py` & `cloudshell-shell-standards-2.0.4/tests/cloudshell/shell_standards/test_autoload_details_builder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/test_resource_config_generic_models.py` & `cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/test_resource_config_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/test_utils.py` & `cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/test_utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py` & `cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_simple_conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from enum import Enum
 from ipaddress import IPv4Address
 
+import pytest
 from attrs import define
 
 from cloudshell.shell.standards.core.resource_conf import BaseConfig, attr
 
 
 class EnumSubClass(Enum):
     VALUE_1 = "Value 1"
@@ -15,36 +16,60 @@
 
 @define(slots=False, str=False)
 class SimpleConf(BaseConfig):
     str_res_attr: str = attr("Str Attribute")
     int_res_attr: int = attr("Int Attribute")
     enum_res_attr: EnumSubClass = attr("Enum Attribute")
     ip: IPv4Address = attr("IP Address")
+    list_attr: list[str] = attr("List Attribute")
 
 
-def test_from_context(api, context_creator):
+@pytest.mark.parametrize(
+    ("attr_values", "expected_values"),
+    (
+        (
+            ("str_attr", "12", "Value 2", "192.168.12.13", "a;b,c"),
+            (
+                "str_attr",
+                12,
+                EnumSubClass.VALUE_2,
+                IPv4Address("192.168.12.13"),
+                ["a", "b", "c"],
+            ),
+        ),
+        (
+            ("str_attr", "10", "Value 1", "127.0.0.1", ""),
+            ("str_attr", 10, EnumSubClass.VALUE_1, IPv4Address("127.0.0.1"), []),
+        ),
+    ),
+)
+def test_from_context(api, context_creator, attr_values, expected_values):
     r_name = "resource name"
     r_model = "resource model"
     r_family = "resource family"
     r_address = "resource address"
-    str_attr = "str attr"
-    int_attr = 12
-    enum_attr = EnumSubClass.VALUE_2
-    ip_attr = IPv4Address("192.168.12.13")
-    r_attributes = {
-        "Str Attribute": str_attr,
-        "Int Attribute": str(int_attr),
-        "Enum Attribute": enum_attr.value,
-        "IP Address": str(ip_attr),
-    }
+
+    r_attributes = dict(
+        zip(
+            [
+                "Str Attribute",
+                "Int Attribute",
+                "Enum Attribute",
+                "IP Address",
+                "List Attribute",
+            ],
+            attr_values,
+        )
+    )
     r_attributes = {f"{r_model}.{k}": v for k, v in r_attributes.items()}
     context = context_creator(r_name, r_model, r_family, r_address, r_attributes)
 
     conf = SimpleConf.from_context(context, api)
 
+    str_attr, int_attr, enum_attr, ip_attr, list_attr = expected_values
     assert conf.name == r_name
     assert conf.shell_name == r_model
     assert conf.family_name == r_family
     assert conf.address == r_address
     assert conf.str_res_attr == str_attr
     assert conf.int_res_attr == int_attr
     assert conf.enum_res_attr is enum_attr
```

## Comparing `cloudshell-shell-standards-2.0.3/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py` & `cloudshell-shell-standards-2.0.4/tests/cloudshell/shell/standards/core/resource_conf/test_attrs_converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,23 @@
 def test_invalid_bool(meta):
     conv = BoolConverter("abc", meta)
 
     with pytest.raises(AttributeConvertError):
         conv.convert()
 
 
-def test_collection_converter(meta):
+@pytest.mark.parametrize(
+    ("str_val", "expected"),
+    (
+        ("str", ["str"]),
+        ("a,b;c", ["a", "b", "c"]),
+        ("", []),
+    ),
+)
+def test_collection_converter(str_val, expected, meta):
     class TestCollectionConverter(CollectionConverter):
         type_ = list
 
-    conv = TestCollectionConverter("a,b;c", meta)
+    conv = TestCollectionConverter(str_val, meta)
 
-    assert conv.convert() == ["a", "b", "c"]
+    assert conv.convert() == expected
     assert conv.get_str_child_type("list[str]") == "str"
```

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/attribute_names.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/attribute_names.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/resource_config_generic_models.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/resource_config_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/autoload_generic_models.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/autoload_generic_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/utils.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_converters.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_converters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/resource_attr.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/resource_attr.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/base_conf.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/base_conf.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_converter.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_converter.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/resource_conf/attrs_getter.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/resource_conf/attrs_getter.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,19 +74,20 @@
         str_type = get_str_type(f)
         error = ValueError(f"Resource attribute {meta.name} is missing")
         default = f.default
 
         if default is RAISE:
             if not attr_present:
                 raise error
-            elif str_type != "str":
-                # empty string is not valid value for non-str types
+            elif (
+                str_type != "str"  # empty string valid for str type
+                and "[str]" not in str_type  # empty string valid for sequence of str
+            ):
                 raise error
             else:
-                # empty string is valid value for str types
                 default = ""
 
         return default
 
 
 class ResourceContextAttrsGetter(AbsAttrsGetter):
     def __init__(
```

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/resource_model.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/resource_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/existed_resource_info.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/existed_resource_info.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/core_entities.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/core_entities.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-standards-2.0.3/cloudshell/shell/standards/core/autoload/utils.py` & `cloudshell-shell-standards-2.0.4/cloudshell/shell/standards/core/autoload/utils.py`

 * *Files identical despite different names*

