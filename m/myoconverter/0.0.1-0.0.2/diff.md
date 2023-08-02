# Comparing `tmp/myoconverter-0.0.1.tar.gz` & `tmp/myoconverter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myoconverter-0.0.1.tar", last modified: Wed Aug  2 12:20:47 2023, max compression
+gzip compressed data, was "myoconverter-0.0.2.tar", last modified: Wed Aug  2 12:36:45 2023, max compression
```

## Comparing `myoconverter-0.0.1.tar` & `myoconverter-0.0.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.169871 myoconverter-0.0.1/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11357 2023-08-02 12:04:59.000000 myoconverter-0.0.1/LICENSE
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    12725 2023-08-02 12:20:47.169871 myoconverter-0.0.1/PKG-INFO
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    12366 2023-08-02 12:04:59.000000 myoconverter-0.0.1/README.md
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.162871 myoconverter-0.0.1/examples/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:00.000000 myoconverter-0.0.1/examples/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3666 2023-08-02 12:05:00.000000 myoconverter-0.0.1/examples/example_models_convert.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.163871 myoconverter-0.0.1/myoconverter/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8561 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/O2MPipeline.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-02 12:05:51.000000 myoconverter-0.0.1/myoconverter/__init__.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.164871 myoconverter-0.0.1/myoconverter/conversion_steps/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11705 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/conversion_steps/O2MStep1.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    30245 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/conversion_steps/O2MStep2.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    23489 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/conversion_steps/O2MStep3.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    13786 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/conversion_steps/O2MSteps.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/conversion_steps/__init__.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.164871 myoconverter-0.0.1/myoconverter/utils/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/utils/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16722 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/utils/generate_pdf.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.164871 myoconverter-0.0.1/myoconverter/xml/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/__init__.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.165871 myoconverter-0.0.1/myoconverter/xml/bodies/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4041 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/bodies/Body.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2912 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/bodies/Ground.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       84 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/bodies/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2963 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/bodies/utils.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5065 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/config.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.165871 myoconverter-0.0.1/myoconverter/xml/constraints/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4646 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/constraints/CoordinateCouplerConstraint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/constraints/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7773 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/converter.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.166871 myoconverter-0.0.1/myoconverter/xml/forces/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      566 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/BushingForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2336 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/CoordinateActuator.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4151 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/CoordinateLimitForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      618 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/FunctionBasedBushingForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1814 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/Ligament.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1129 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5468 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/Muscle.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      556 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/PointActuator.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1534 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      603 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/SpringGeneralizedForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1030 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/Thelen2003Muscle.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      560 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/TorqueActuator.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2770 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/forces/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.167871 myoconverter-0.0.1/myoconverter/xml/joints/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16303 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/CustomJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2118 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/Joint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1983 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/PinJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1944 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/SliderJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2334 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/UniversalJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      652 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/WeldJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3670 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/joints/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.168871 myoconverter-0.0.1/myoconverter/xml/markers/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1070 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/markers/Marker.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       86 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/markers/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6461 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/parsers.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.168871 myoconverter-0.0.1/myoconverter/xml/path_points/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8604 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_points/ConditionalPathPoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6144 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_points/MovingPathPoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1537 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_points/PathPoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       89 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_points/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6796 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_points/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.168871 myoconverter-0.0.1/myoconverter/xml/path_wraps/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3327 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_wraps/PathWrap.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3977 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_wraps/PathWrapSet.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       88 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_wraps/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7758 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/path_wraps/utils.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11328 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.169871 myoconverter-0.0.1/myoconverter/xml/wrap_objects/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1670 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapCylinder.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1729 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapEllipsoid.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3594 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapObject.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1580 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapSphere.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1429 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapTorus.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8219 2023-08-02 12:05:01.000000 myoconverter-0.0.1/myoconverter/xml/wrap_objects/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:20:47.163871 myoconverter-0.0.1/myoconverter.egg-info/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    12725 2023-08-02 12:20:47.000000 myoconverter-0.0.1/myoconverter.egg-info/PKG-INFO
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2650 2023-08-02 12:20:47.000000 myoconverter-0.0.1/myoconverter.egg-info/SOURCES.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        1 2023-08-02 12:20:47.000000 myoconverter-0.0.1/myoconverter.egg-info/dependency_links.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      215 2023-08-02 12:20:47.000000 myoconverter-0.0.1/myoconverter.egg-info/requires.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-02 12:20:47.000000 myoconverter-0.0.1/myoconverter.egg-info/top_level.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      533 2023-08-02 12:05:01.000000 myoconverter-0.0.1/pyproject.toml
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       38 2023-08-02 12:20:47.169871 myoconverter-0.0.1/setup.cfg
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      916 2023-08-02 12:20:38.000000 myoconverter-0.0.1/setup.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.373465 myoconverter-0.0.2/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11357 2023-08-02 12:04:59.000000 myoconverter-0.0.2/LICENSE
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      459 2023-08-02 12:36:45.373465 myoconverter-0.0.2/PKG-INFO
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    12366 2023-08-02 12:04:59.000000 myoconverter-0.0.2/README.md
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.367465 myoconverter-0.0.2/examples/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:00.000000 myoconverter-0.0.2/examples/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3666 2023-08-02 12:05:00.000000 myoconverter-0.0.2/examples/example_models_convert.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.367465 myoconverter-0.0.2/myoconverter/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8561 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/O2MPipeline.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-02 12:05:51.000000 myoconverter-0.0.2/myoconverter/__init__.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.368465 myoconverter-0.0.2/myoconverter/conversion_steps/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11705 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep1.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    30245 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep2.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    23489 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep3.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    13786 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MSteps.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/__init__.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.368465 myoconverter-0.0.2/myoconverter/utils/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/utils/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16722 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/utils/generate_pdf.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.369465 myoconverter-0.0.2/myoconverter/xml/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/__init__.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.369465 myoconverter-0.0.2/myoconverter/xml/bodies/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4041 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/Body.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2912 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/Ground.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       84 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2963 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/utils.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5065 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/config.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.369465 myoconverter-0.0.2/myoconverter/xml/constraints/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4646 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/constraints/CoordinateCouplerConstraint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/constraints/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7773 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/converter.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.370465 myoconverter-0.0.2/myoconverter/xml/forces/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      566 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/BushingForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2336 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/CoordinateActuator.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4151 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/CoordinateLimitForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      618 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/FunctionBasedBushingForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1814 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Ligament.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1129 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5468 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Muscle.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      556 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/PointActuator.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1534 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      603 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/SpringGeneralizedForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1030 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Thelen2003Muscle.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      560 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/TorqueActuator.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2770 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.371465 myoconverter-0.0.2/myoconverter/xml/joints/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16303 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/CustomJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2118 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/Joint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1983 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/PinJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1944 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/SliderJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2334 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/UniversalJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      652 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/WeldJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3670 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.371465 myoconverter-0.0.2/myoconverter/xml/markers/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1070 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/markers/Marker.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       86 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/markers/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6461 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/parsers.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.372465 myoconverter-0.0.2/myoconverter/xml/path_points/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8604 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/ConditionalPathPoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6144 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/MovingPathPoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1537 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/PathPoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       89 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6796 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.372465 myoconverter-0.0.2/myoconverter/xml/path_wraps/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3327 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrap.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3977 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrapSet.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       88 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7758 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/utils.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11328 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.373465 myoconverter-0.0.2/myoconverter/xml/wrap_objects/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1670 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapCylinder.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1729 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapEllipsoid.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3594 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapObject.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1580 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapSphere.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1429 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapTorus.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8219 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.367465 myoconverter-0.0.2/myoconverter.egg-info/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      459 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2650 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        1 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      215 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/requires.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/top_level.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      533 2023-08-02 12:05:01.000000 myoconverter-0.0.2/pyproject.toml
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       38 2023-08-02 12:36:45.373465 myoconverter-0.0.2/setup.cfg
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1001 2023-08-02 12:35:41.000000 myoconverter-0.0.2/setup.py
```

### Comparing `myoconverter-0.0.1/LICENSE` & `myoconverter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/PKG-INFO` & `myoconverter-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: myoconverter
-Version: 0.0.1
-Summary: Tool for converting OpenSim musculoskeletal (MSK) models to the MuJoCo model format with optimized muscle kinematics and kinetics
-Home-page: https://github.com/MyoHub/myo-converter
-Author: Huawei Wang, Aleksi Ikkala
-Author-email: 
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
 <img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/logo-color-fit_horizontal.png?raw=true" width=800>
 </p>
 
 [![Documentation Status](https://readthedocs.org/projects/myoconverter/badge/?version=latest)](https://myoconverter.readthedocs.io/en/latest/)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/MyoHub/myoConverter/blob/main/docs/CONTRIBUTING.md)
 [![License Badge](https://img.shields.io/hexpm/l/apa)](https://github.com/opensim-org/opensim-core/blob/master/LICENSE.txt)
```

### Comparing `myoconverter-0.0.1/examples/example_models_convert.py` & `myoconverter-0.0.2/examples/example_models_convert.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/O2MPipeline.py` & `myoconverter-0.0.2/myoconverter/O2MPipeline.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/conversion_steps/O2MStep1.py` & `myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep1.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/conversion_steps/O2MStep2.py` & `myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep2.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/conversion_steps/O2MStep3.py` & `myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep3.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/conversion_steps/O2MSteps.py` & `myoconverter-0.0.2/myoconverter/conversion_steps/O2MSteps.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/utils/generate_pdf.py` & `myoconverter-0.0.2/myoconverter/utils/generate_pdf.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/bodies/Body.py` & `myoconverter-0.0.2/myoconverter/xml/bodies/Body.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/bodies/Ground.py` & `myoconverter-0.0.2/myoconverter/xml/bodies/Ground.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/bodies/utils.py` & `myoconverter-0.0.2/myoconverter/xml/bodies/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/config.py` & `myoconverter-0.0.2/myoconverter/xml/config.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/constraints/CoordinateCouplerConstraint.py` & `myoconverter-0.0.2/myoconverter/xml/constraints/CoordinateCouplerConstraint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/converter.py` & `myoconverter-0.0.2/myoconverter/xml/converter.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/BushingForce.py` & `myoconverter-0.0.2/myoconverter/xml/forces/BushingForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/CoordinateActuator.py` & `myoconverter-0.0.2/myoconverter/xml/forces/CoordinateActuator.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/CoordinateLimitForce.py` & `myoconverter-0.0.2/myoconverter/xml/forces/CoordinateLimitForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/FunctionBasedBushingForce.py` & `myoconverter-0.0.2/myoconverter/xml/forces/FunctionBasedBushingForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/Ligament.py` & `myoconverter-0.0.2/myoconverter/xml/forces/Ligament.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py` & `myoconverter-0.0.2/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/Muscle.py` & `myoconverter-0.0.2/myoconverter/xml/forces/Muscle.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/PointActuator.py` & `myoconverter-0.0.2/myoconverter/xml/forces/PointActuator.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py` & `myoconverter-0.0.2/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/SpringGeneralizedForce.py` & `myoconverter-0.0.2/myoconverter/xml/forces/SpringGeneralizedForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/Thelen2003Muscle.py` & `myoconverter-0.0.2/myoconverter/xml/forces/Thelen2003Muscle.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/TorqueActuator.py` & `myoconverter-0.0.2/myoconverter/xml/forces/TorqueActuator.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/forces/utils.py` & `myoconverter-0.0.2/myoconverter/xml/forces/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/CustomJoint.py` & `myoconverter-0.0.2/myoconverter/xml/joints/CustomJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/Joint.py` & `myoconverter-0.0.2/myoconverter/xml/joints/Joint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/PinJoint.py` & `myoconverter-0.0.2/myoconverter/xml/joints/PinJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/SliderJoint.py` & `myoconverter-0.0.2/myoconverter/xml/joints/SliderJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/UniversalJoint.py` & `myoconverter-0.0.2/myoconverter/xml/joints/UniversalJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/WeldJoint.py` & `myoconverter-0.0.2/myoconverter/xml/joints/WeldJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/joints/utils.py` & `myoconverter-0.0.2/myoconverter/xml/joints/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/markers/Marker.py` & `myoconverter-0.0.2/myoconverter/xml/markers/Marker.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/parsers.py` & `myoconverter-0.0.2/myoconverter/xml/parsers.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_points/ConditionalPathPoint.py` & `myoconverter-0.0.2/myoconverter/xml/path_points/ConditionalPathPoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_points/MovingPathPoint.py` & `myoconverter-0.0.2/myoconverter/xml/path_points/MovingPathPoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_points/PathPoint.py` & `myoconverter-0.0.2/myoconverter/xml/path_points/PathPoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_points/utils.py` & `myoconverter-0.0.2/myoconverter/xml/path_points/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_wraps/PathWrap.py` & `myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrap.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_wraps/PathWrapSet.py` & `myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrapSet.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/path_wraps/utils.py` & `myoconverter-0.0.2/myoconverter/xml/path_wraps/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/utils.py` & `myoconverter-0.0.2/myoconverter/xml/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapCylinder.py` & `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapCylinder.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapEllipsoid.py` & `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapEllipsoid.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapObject.py` & `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapObject.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapSphere.py` & `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapSphere.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/wrap_objects/WrapTorus.py` & `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapTorus.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter/xml/wrap_objects/utils.py` & `myoconverter-0.0.2/myoconverter/xml/wrap_objects/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/myoconverter.egg-info/SOURCES.txt` & `myoconverter-0.0.2/myoconverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/pyproject.toml` & `myoconverter-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.1/setup.py` & `myoconverter-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="myoconverter",
-    version="0.0.1",
+    version="0.0.2",
     author="Huawei Wang, Aleksi Ikkala",
     author_email="",
     description="Tool for converting OpenSim musculoskeletal (MSK) models to the MuJoCo model format with optimized muscle kinematics and kinetics",
-    long_description=long_description,
+    long_description="Check the [GitHub repository](https://github.com/MyoHub/myo-converter) for up-to-date documentation",
     long_description_content_type="text/markdown",
     url="https://github.com/MyoHub/myo-converter",
     packages=setuptools.find_packages(),
     install_requires=[
-      'python>=3.8',
+      'python>=3.9',
       'mujoco-python==2.3.3',
       'loguru==0.5.3',
       'lxml==4.9.1',
       'numpy==1.21.5',
       'scipy==1.10.0',
       'scikit-learn==1.2.0',
       'opensim==4.4',
```

