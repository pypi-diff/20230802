# Comparing `tmp/pretext-1.7.5.dev20230731.tar.gz` & `tmp/pretext-1.7.5.dev20230802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.7.5.dev20230731.tar", max compression
+gzip compressed data, was "pretext-1.7.5.dev20230802.tar", max compression
```

## Comparing `pretext-1.7.5.dev20230731.tar` & `pretext-1.7.5.dev20230802.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35148 2023-07-31 06:17:17.112354 pretext-1.7.5.dev20230731/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-31 06:17:17.112354 pretext-1.7.5.dev20230731/README.md
--rw-r--r--   0        0        0     1500 2023-07-31 06:17:55.630851 pretext-1.7.5.dev20230731/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/__main__.py
--rw-r--r--   0        0        0    11608 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/build.py
--rw-r--r--   0        0        0    27783 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/cli.py
--rw-r--r--   0        0        0     6149 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      675 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/constants.py
--rw-r--r--   0        0        0      350 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/core/__init__.py
--rw-r--r--   0        0        0   172498 2023-07-31 06:18:00.807160 pretext-1.7.5.dev20230731/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/core/resources.py
--rw-r--r--   0        0        0  1045100 2023-07-31 06:18:00.807160 pretext-1.7.5.dev20230731/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/generate.py
--rw-r--r--   0        0        0    29656 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/project/__init__.py
--rw-r--r--   0        0        0    30392 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/project/refactor.py
--rw-r--r--   0        0        0     2620 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/project/xml.py
--rw-r--r--   0        0        0      739 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/templates/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-31 06:18:00.887165 pretext-1.7.5.dev20230731/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1676 2023-07-31 06:18:00.887165 pretext-1.7.5.dev20230731/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-31 06:18:00.887165 pretext-1.7.5.dev20230731/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   158949 2023-07-31 06:18:00.883165 pretext-1.7.5.dev20230731/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     6455 2023-07-31 06:18:00.871164 pretext-1.7.5.dev20230731/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   172278 2023-07-31 06:18:00.867164 pretext-1.7.5.dev20230731/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     3496 2023-07-31 06:18:00.887165 pretext-1.7.5.dev20230731/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-31 06:18:00.887165 pretext-1.7.5.dev20230731/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-31 06:18:00.887165 pretext-1.7.5.dev20230731/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     7231 2023-07-31 06:18:00.871164 pretext-1.7.5.dev20230731/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      109 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/types.py
--rw-r--r--   0        0        0    25401 2023-07-31 06:17:17.116354 pretext-1.7.5.dev20230731/pretext/utils.py
--rw-r--r--   0        0        0     3353 2023-07-31 06:17:55.630851 pretext-1.7.5.dev20230731/pyproject.toml
--rw-r--r--   0        0        0    10891 1970-01-01 00:00:00.000000 pretext-1.7.5.dev20230731/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/LICENSE
+-rw-r--r--   0        0        0     9757 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/README.md
+-rw-r--r--   0        0        0     1500 2023-08-02 06:15:15.939249 pretext-1.7.5.dev20230802/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/__main__.py
+-rw-r--r--   0        0        0    11608 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/build.py
+-rw-r--r--   0        0        0    27783 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      675 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/constants.py
+-rw-r--r--   0        0        0      350 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172548 2023-08-02 06:15:21.211292 pretext-1.7.5.dev20230802/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/core/resources.py
+-rw-r--r--   0        0        0  1045146 2023-08-02 06:15:21.211292 pretext-1.7.5.dev20230802/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/generate.py
+-rw-r--r--   0        0        0    29656 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/project/__init__.py
+-rw-r--r--   0        0        0    30392 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/project/refactor.py
+-rw-r--r--   0        0        0     2620 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/project/xml.py
+-rw-r--r--   0        0        0      739 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     2480 2023-08-02 06:15:21.291293 pretext-1.7.5.dev20230802/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1676 2023-08-02 06:15:21.291293 pretext-1.7.5.dev20230802/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-08-02 06:15:21.291293 pretext-1.7.5.dev20230802/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   158949 2023-08-02 06:15:21.291293 pretext-1.7.5.dev20230802/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     6455 2023-08-02 06:15:21.259293 pretext-1.7.5.dev20230802/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   172278 2023-08-02 06:15:21.279293 pretext-1.7.5.dev20230802/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     3496 2023-08-02 06:15:21.263293 pretext-1.7.5.dev20230802/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-08-02 06:15:21.291293 pretext-1.7.5.dev20230802/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-08-02 06:15:21.291293 pretext-1.7.5.dev20230802/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     7231 2023-08-02 06:15:21.259293 pretext-1.7.5.dev20230802/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0      109 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/types.py
+-rw-r--r--   0        0        0    25401 2023-08-02 06:14:40.742950 pretext-1.7.5.dev20230802/pretext/utils.py
+-rw-r--r--   0        0        0     3353 2023-08-02 06:15:15.939249 pretext-1.7.5.dev20230802/pyproject.toml
+-rw-r--r--   0        0        0    10891 1970-01-01 00:00:00.000000 pretext-1.7.5.dev20230802/PKG-INFO
```

### Comparing `pretext-1.7.5.dev20230731/LICENSE` & `pretext-1.7.5.dev20230802/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/README.md` & `pretext-1.7.5.dev20230802/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/__init__.py` & `pretext-1.7.5.dev20230802/pretext/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '9bce7e55911fb14e3e6e362bfa78bd6431c38597'
+CORE_COMMIT = '3ee772f9259f9207d4a674f561b802fc8f026876'
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.7.5.dev20230731/pretext/build.py` & `pretext-1.7.5.dev20230802/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/cli.py` & `pretext-1.7.5.dev20230802/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/codechat.py` & `pretext-1.7.5.dev20230802/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/config/xml_overlay.py` & `pretext-1.7.5.dev20230802/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/constants.py` & `pretext-1.7.5.dev20230802/pretext/constants.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/core/pretext.py` & `pretext-1.7.5.dev20230802/pretext/core/pretext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1326,15 +1326,15 @@
 
         no_compile = (
             "ERROR caught by Translator while processing problem file:" in response.text
         )
 
         bad_xml = False
         try:
-            response_root = ET.fromstring(response.text)
+            response_root = ET.fromstring(bytes(response.text, encoding='utf-8'))
         except:
             response_root = ET.Element("webwork")
             bad_xml = True
 
         no_statement = False
         if not bad_xml:
             if response_root.find(".//statement") is None:
@@ -1547,15 +1547,15 @@
                             os.path.join(ww_images_dir, ptx_image_name + ".{}".format(ext)),
                         )
                     except:
                         log.warning(msg.format(destination_image_file, ext))
                 os.remove(os.path.join(ww_images_dir, ptx_image_filename))
 
         # Start appending XML children
-        response_root = ET.fromstring(response_text)
+        response_root = ET.fromstring(bytes(response_text, encoding='utf-8'))
         # Use "webwork-reps" as parent tag for the various representations of a problem
         webwork_reps = ET.SubElement(webwork_representations, "webwork-reps")
         webwork_reps.set("version", ww_reps_version)
         webwork_reps.set("ww_major_version", str(ww_major_version))
         webwork_reps.set("ww_minor_version", str(ww_minor_version))
         webwork_reps.set("{%s}id" % (XML), "extracted-" + problem)
         webwork_reps.set("ww-id", problem)
```

### Comparing `pretext-1.7.5.dev20230731/pretext/core/resources.py` & `pretext-1.7.5.dev20230802/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/core/resources.zip` & `pretext-1.7.5.dev20230802/pretext/core/resources.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1045100 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 xsl/
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-31 06:18 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-31 06:18 pretext/module-test.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-31 06:18 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172498 b- defN 23-Jul-31 06:18 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-31 06:18 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 06:18 pretext/__init__.py
--rw-r--r--  2.0 unx    36045 b- defN 23-Jul-31 06:18 pretext/braille_format.py
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-31 06:18 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-31 06:18 schema/xml.xsd
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-31 06:18 schema/pretext.rnc
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-31 06:18 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-31 06:18 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-31 06:18 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-31 06:18 schema/README.md
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-31 06:18 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-31 06:18 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-31 06:18 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-31 06:18 schema/pretext.rng
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-31 06:18 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-31 06:18 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_blue_red.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-31 06:18 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_green_plum.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-31 06:18 css/style_soundwriting.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-31 06:18 css/colors_red_blue.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-31 06:18 css/style_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-31 06:18 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-31 06:18 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-31 06:18 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-31 06:18 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-31 06:18 css/setcolors.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-31 06:18 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-31 06:18 css/README.md
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-31 06:18 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-31 06:18 css/pretext.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-31 06:18 css/mathbook-content.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-31 06:18 css/mathbook-3.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-31 06:18 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-31 06:18 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 06:18 css/colors_green_blue.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-31 06:18 css/pretext_add_on.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-31 06:18 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-31 06:18 css/kindle.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-31 06:18 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-31 06:18 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-31 06:18 xsl/entities.ent
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-31 06:18 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-31 06:18 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-31 06:18 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-31 06:18 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-31 06:18 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-31 06:18 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611284 b- defN 23-Jul-31 06:18 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-31 06:18 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-31 06:18 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-31 06:18 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-31 06:18 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-31 06:18 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Jul-31 06:18 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-31 06:18 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-31 06:18 xsl/README.md
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-31 06:18 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-31 06:18 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-31 06:18 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-31 06:18 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-31 06:18 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-31 06:18 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx   544154 b- defN 23-Jul-31 06:18 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-31 06:18 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Jul-31 06:18 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-31 06:18 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-31 06:18 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   116581 b- defN 23-Jul-31 06:18 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-31 06:18 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-31 06:18 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-31 06:18 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-31 06:18 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-31 06:18 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-31 06:18 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-31 06:18 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   110949 b- defN 23-Jul-31 06:18 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-31 06:18 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-31 06:18 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-31 06:18 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-31 06:18 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-31 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-31 06:18 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-31 06:18 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-31 06:18 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-31 06:18 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-31 06:18 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-31 06:18 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-31 06:18 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 xsl/support/play-button/
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-31 06:18 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-31 06:18 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-31 06:18 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-31 06:18 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-31 06:18 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-31 06:18 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-31 06:18 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-31 06:18 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-31 06:18 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-31 06:18 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-31 06:18 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-31 06:18 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-31 06:18 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-31 06:18 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-31 06:18 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-31 06:18 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-31 06:18 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-31 06:18 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-31 06:18 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-31 06:18 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-31 06:18 xsl/localizations/README.md
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-31 06:18 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-31 06:18 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-31 06:18 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-31 06:18 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-31 06:18 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-31 06:18 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-31 06:18 xsl/localizations/af-ZA.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:18 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-31 06:18 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-31 06:18 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 06:18 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-31 06:18 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-31 06:18 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-31 06:18 script/mjsre/mj-sre-page.js
-142 files, 4848159 bytes uncompressed, 1027526 bytes compressed:  78.8%
+Zip file size: 1045146 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Aug-02 06:15 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Aug-02 06:15 script/mbx
+-rw-r--r--  2.0 unx      116 b- defN 23-Aug-02 06:15 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 06:15 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Aug-02 06:15 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      481 b- defN 23-Aug-02 06:15 script/mjsre/README.md
+-rw-r--r--  2.0 unx   134086 b- defN 23-Aug-02 06:15 schema/pretext.xml
+-rw-r--r--  2.0 unx   125241 b- defN 23-Aug-02 06:15 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Aug-02 06:15 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    25870 b- defN 23-Aug-02 06:15 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    58129 b- defN 23-Aug-02 06:15 schema/pretext.rnc
+-rw-r--r--  2.0 unx      326 b- defN 23-Aug-02 06:15 schema/xml.xsd
+-rw-r--r--  2.0 unx   101895 b- defN 23-Aug-02 06:15 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Aug-02 06:15 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Aug-02 06:15 schema/README.md
+-rw-r--r--  2.0 unx    34210 b- defN 23-Aug-02 06:15 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Aug-02 06:15 schema/build.sh
+-rw-r--r--  2.0 unx     2566 b- defN 23-Aug-02 06:15 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1955 b- defN 23-Aug-02 06:15 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Aug-02 06:15 pretext/pretext
+-rw-r--r--  2.0 unx   172548 b- defN 23-Aug-02 06:15 pretext/pretext.py
+-rw-r--r--  2.0 unx    36045 b- defN 23-Aug-02 06:15 pretext/braille_format.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Aug-02 06:15 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 06:15 pretext/__init__.py
+-rw-r--r--  2.0 unx     2446 b- defN 23-Aug-02 06:15 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Aug-02 06:15 css/update_css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Aug-02 06:15 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Aug-02 06:15 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Aug-02 06:15 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Aug-02 06:15 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Aug-02 06:15 css/kindle.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Aug-02 06:15 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Aug-02 06:15 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Aug-02 06:15 css/epub.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Aug-02 06:15 css/style_soundwriting.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Aug-02 06:15 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Aug-02 06:15 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Aug-02 06:15 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Aug-02 06:15 css/mathbook-3.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Aug-02 06:15 css/style_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Aug-02 06:15 css/colors_red_blue.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Aug-02 06:15 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Aug-02 06:15 css/README.md
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-02 06:15 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Aug-02 06:15 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Aug-02 06:15 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Aug-02 06:15 css/setcolors.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 xsl/utilities/
+-rw-r--r--  2.0 unx     2725 b- defN 23-Aug-02 06:15 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Aug-02 06:15 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Aug-02 06:15 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Aug-02 06:15 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Aug-02 06:15 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Aug-02 06:15 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Aug-02 06:15 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Aug-02 06:15 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Aug-02 06:15 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Aug-02 06:15 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Aug-02 06:15 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Aug-02 06:15 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Aug-02 06:15 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Aug-02 06:15 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Aug-02 06:15 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Aug-02 06:15 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Aug-02 06:15 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   611284 b- defN 23-Aug-02 06:15 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Aug-02 06:15 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Aug-02 06:15 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-Aug-02 06:15 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Aug-02 06:15 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Aug-02 06:15 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Aug-02 06:15 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Aug-02 06:15 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Aug-02 06:15 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Aug-02 06:15 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Aug-02 06:15 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   116581 b- defN 23-Aug-02 06:15 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Aug-02 06:15 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Aug-02 06:15 xsl/README.md
+-rw-r--r--  2.0 unx    13186 b- defN 23-Aug-02 06:15 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Aug-02 06:15 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Aug-02 06:15 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Aug-02 06:15 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Aug-02 06:15 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Aug-02 06:15 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   110953 b- defN 23-Aug-02 06:15 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx   544154 b- defN 23-Aug-02 06:15 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Aug-02 06:15 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx      513 b- defN 23-Aug-02 06:15 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Aug-02 06:15 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Aug-02 06:15 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Aug-02 06:15 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4299 b- defN 23-Aug-02 06:15 xsl/utilities/author-report.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:15 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5879 b- defN 23-Aug-02 06:15 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Aug-02 06:15 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Aug-02 06:15 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx    10306 b- defN 23-Aug-02 06:15 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-Aug-02 06:15 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Aug-02 06:15 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Aug-02 06:15 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Aug-02 06:15 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Aug-02 06:15 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Aug-02 06:15 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    17231 b- defN 23-Aug-02 06:15 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Aug-02 06:15 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Aug-02 06:15 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Aug-02 06:15 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Aug-02 06:15 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16534 b- defN 23-Aug-02 06:15 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Aug-02 06:15 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Aug-02 06:15 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Aug-02 06:15 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Aug-02 06:15 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Aug-02 06:15 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Aug-02 06:15 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Aug-02 06:15 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    19326 b- defN 23-Aug-02 06:15 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Aug-02 06:15 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15866 b- defN 23-Aug-02 06:15 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Aug-02 06:15 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Aug-02 06:15 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx     5135 b- defN 23-Aug-02 06:15 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Aug-02 06:15 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Aug-02 06:15 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Aug-02 06:15 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Aug-02 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
+142 files, 4848471 bytes uncompressed, 1027572 bytes compressed:  78.8%
```

#### zipnote {}

```diff
@@ -9,419 +9,419 @@
 
 Filename: script/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: pretext/pretext
+Filename: script/mjsre/
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: script/README.md
 Comment: 
 
-Filename: pretext/pretext.cfg
+Filename: script/mbx
 Comment: 
 
-Filename: pretext/pretext.py
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: pretext/README.md
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: pretext/__init__.py
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: script/mjsre/README.md
+Comment: 
+
+Filename: schema/pretext.xml
 Comment: 
 
 Filename: schema/pretext.xsd
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: schema/pretext-schematron.xsl
+Comment: 
+
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
 Filename: schema/pretext.rnc
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: schema/xml.xsd
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: schema/pretext-dev.rnc
 Comment: 
 
 Filename: schema/README.md
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: schema/pretext-dev.rng
 Comment: 
 
 Filename: schema/build.sh
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: pretext/module-test.py
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: pretext/pretext
 Comment: 
 
-Filename: css/colors_default.css
+Filename: pretext/pretext.py
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: pretext/README.md
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: pretext/__init__.py
 Comment: 
 
-Filename: css/style_soundwriting.css
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: css/update_css
 Comment: 
 
-Filename: css/style_default.css
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: css/colors_maroon_grey.css
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: css/mathbook-add-on.css
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: css/kindle.css
 Comment: 
 
-Filename: css/setcolors.css
+Filename: css/pretext.css
 Comment: 
 
-Filename: css/update_css
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: css/README.md
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: css/epub.css
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: css/pretext.css
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: css/mathbook-content.css
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: css/mathbook-3.css
+Filename: css/colors_default.css
 Comment: 
 
-Filename: css/epub.css
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: css/mathbook-3.css
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: css/style_default.css
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: css/mathbook-add-on.css
+Filename: css/mathbook-content.css
 Comment: 
 
-Filename: css/kindle.css
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: xsl/latex/
+Filename: css/README.md
 Comment: 
 
-Filename: xsl/localizations/
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: xsl/support/
+Filename: css/colors_blue_green.css
 Comment: 
 
-Filename: xsl/utilities/
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: xsl/extract-mom.xsl
+Filename: css/setcolors.css
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: xsl/latex/
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: xsl/localizations/
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: xsl/support/
 Comment: 
 
-Filename: xsl/extract-datafile.xsl
+Filename: xsl/utilities/
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone-static.xsl
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/publisher-variables.xsl
+Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: xsl/pretext-common.xsl
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: xsl/pretext-litprog.xsl
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
-Filename: xsl/README.md
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/pretext-numbers.xsl
+Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: xsl/pretext-jupyter.xsl
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: xsl/README.md
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: xsl/xml-to-json.xsl
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-chaos.xsl
+Filename: xsl/xml-to-json.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/extract-identity.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-CLP.xsl
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
 Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
 Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
-Comment: 
-
-Filename: xsl/utilities/author-report.xsl
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
 Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: xsl/support/play-button/
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: xsl/support/play-button/
 Comment: 
 
 Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: xsl/support/README.md
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
 Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: xsl/support/README.md
 Comment: 
 
-Filename: xsl/support/play-button/play-button.png
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
 Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
 Filename: xsl/support/play-button/README.md
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
-Comment: 
-
-Filename: xsl/localizations/fr-FR.xml
+Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
 Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
-Filename: xsl/localizations/cs-CZ.xml
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
-Filename: xsl/localizations/bg-BG.xml
+Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: xsl/localizations/hu-HU.xml
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: xsl/localizations/ca-ES.xml
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: xsl/localizations/fi-FI.xml
+Filename: xsl/localizations/ku-CKB.xml
 Comment: 
 
-Filename: xsl/localizations/ku-CKB.xml
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
-Filename: script/mjsre/
+Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: script/README.md
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: script/mbx
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
 Zip file comment:
```

#### pretext/pretext.py

```diff
@@ -1326,15 +1326,15 @@
 
         no_compile = (
             "ERROR caught by Translator while processing problem file:" in response.text
         )
 
         bad_xml = False
         try:
-            response_root = ET.fromstring(response.text)
+            response_root = ET.fromstring(bytes(response.text, encoding='utf-8'))
         except:
             response_root = ET.Element("webwork")
             bad_xml = True
 
         no_statement = False
         if not bad_xml:
             if response_root.find(".//statement") is None:
@@ -1547,15 +1547,15 @@
                             os.path.join(ww_images_dir, ptx_image_name + ".{}".format(ext)),
                         )
                     except:
                         log.warning(msg.format(destination_image_file, ext))
                 os.remove(os.path.join(ww_images_dir, ptx_image_filename))
 
         # Start appending XML children
-        response_root = ET.fromstring(response_text)
+        response_root = ET.fromstring(bytes(response_text, encoding='utf-8'))
         # Use "webwork-reps" as parent tag for the various representations of a problem
         webwork_reps = ET.SubElement(webwork_representations, "webwork-reps")
         webwork_reps.set("version", ww_reps_version)
         webwork_reps.set("ww_major_version", str(ww_major_version))
         webwork_reps.set("ww_minor_version", str(ww_minor_version))
         webwork_reps.set("{%s}id" % (XML), "extracted-" + problem)
         webwork_reps.set("ww-id", problem)
```

#### schema/pretext.xsd

##### schema/pretext.xsd

```diff
@@ -3361,14 +3361,15 @@
       <xs:choice>
         <xs:element ref="ellipsis"/>
         <xs:element ref="midpoint"/>
         <xs:element ref="swungdash"/>
         <xs:element ref="permille"/>
         <xs:element ref="pilcrow"/>
         <xs:element ref="section-mark"/>
+        <xs:element ref="copyleft"/>
         <xs:element ref="copyright"/>
         <xs:element ref="registered"/>
         <xs:element ref="trademark"/>
         <xs:element ref="phonomark"/>
         <xs:element ref="servicemark"/>
       </xs:choice>
       <xs:element ref="icon"/>
@@ -3440,14 +3441,17 @@
   </xs:element>
   <xs:element name="pilcrow">
     <xs:complexType/>
   </xs:element>
   <xs:element name="section-mark">
     <xs:complexType/>
   </xs:element>
+  <xs:element name="copyleft">
+    <xs:complexType/>
+  </xs:element>
   <xs:element name="copyright">
     <xs:complexType/>
   </xs:element>
   <xs:element name="registered">
     <xs:complexType/>
   </xs:element>
   <xs:element name="trademark">
```

#### schema/pretext.rnc

```diff
@@ -1493,14 +1493,15 @@
             Character |=
                 element ellipsis {empty} |
                 element midpoint {empty} |
                 element swungdash {empty} |
                 element permille {empty} |
                 element pilcrow {empty} |
                 element section-mark {empty} |
+                element copyleft {empty} |
                 element copyright {empty} |
                 element registered {empty} |
                 element trademark {empty} |
                 element phonomark {empty} |
                 element servicemark {empty}
             
             Character |=
```

#### schema/pretext.xml

##### schema/pretext.xml

```diff
@@ -916,14 +916,15 @@
         <code>Character |=
                 element ellipsis {empty} |
                 element midpoint {empty} |
                 element swungdash {empty} |
                 element permille {empty} |
                 element pilcrow {empty} |
                 element section-mark {empty} |
+                element copyleft {empty} |
                 element copyright {empty} |
                 element registered {empty} |
                 element trademark {empty} |
                 element phonomark {empty} |
                 element servicemark {empty}</code>
       </fragment>
       <p>
```

#### schema/pretext.rng

##### schema/pretext.rng

```diff
@@ -3805,14 +3805,17 @@
       </element>
       <element name="pilcrow">
         <empty/>
       </element>
       <element name="section-mark">
         <empty/>
       </element>
+      <element name="copyleft">
+        <empty/>
+      </element>
       <element name="copyright">
         <empty/>
       </element>
       <element name="registered">
         <empty/>
       </element>
       <element name="trademark">
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -355,16 +355,16 @@
         <div class="dropdown-content">
           <xsl:text/>
           <xsl:text>{% if settings.academy_mode: %}</xsl:text>
           <a href="/runestone/assignments/chooseAssignment">Assignments</a>
           <a href="/runestone/assignments/practice">Practice</a>
           <hr/>
           <!-- if reader is not an instructor the next link will be removed by javascript -->
-          <a id="inst_peer_link" href="/{{appname}}/peer/instructor.html">Peer Instruction (Instructor)</a>
-          <a href="/{{appname}}/peer/student.html">Peer Instruction (Student)</a>
+          <a id="inst_peer_link" href="/~._appname_.~/peer/instructor.html">Peer Instruction (Instructor)</a>
+          <a href="/~._appname_.~/peer/student.html">Peer Instruction (Student)</a>
           <hr/>
           <a href="/runestone/default/courses">Change Course</a>
           <hr/>
           <a id="ip_dropdown_link" href="/runestone/admin/index">Instructor's Page</a>
           <hr/>
           <xsl:text/>
           <xsl:text>{% endif %}</xsl:text>
```

### Comparing `pretext-1.7.5.dev20230731/pretext/generate.py` & `pretext-1.7.5.dev20230802/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/project/__init__.py` & `pretext-1.7.5.dev20230802/pretext/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/project/refactor.py` & `pretext-1.7.5.dev20230802/pretext/project/refactor.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/project/xml.py` & `pretext-1.7.5.dev20230802/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/__init__.py` & `pretext-1.7.5.dev20230802/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/.devcontainer.json` & `pretext-1.7.5.dev20230802/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/.gitignore` & `pretext-1.7.5.dev20230802/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/article.zip` & `pretext-1.7.5.dev20230802/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 158949 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 06:18 .gitignore
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-31 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-31 06:18 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-31 06:17 source/section-2.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-31 06:17 source/section-1.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-31 06:17 source/main.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-31 06:17 assets/frog.jpg
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-02 06:15 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-02 06:15 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-02 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-Aug-02 06:14 README.md
+-rw-r--r--  2.0 unx      449 b- defN 23-Aug-02 06:14 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Aug-02 06:14 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Aug-02 06:14 source/main.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Aug-02 06:14 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-02 06:14 publication/publication.ptx
 12 files, 162919 bytes uncompressed, 157669 bytes compressed:  3.2%
```

#### zipnote {}

```diff
@@ -6,32 +6,32 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: README.md
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: README.md
 Comment: 
 
-Filename: source/section-2.ptx
+Filename: source/section-1.ptx
 Comment: 
 
-Filename: source/section-1.ptx
+Filename: source/section-2.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/book.zip` & `pretext-1.7.5.dev20230802/pretext/templates/resources/book.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6455 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 06:18 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-31 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-31 06:18 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-31 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-31 06:17 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-02 06:15 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-02 06:15 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-02 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-02 06:14 README.md
+-rw-r--r--  2.0 unx     1767 b- defN 23-Aug-02 06:14 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Aug-02 06:14 publication/publication.ptx
 8 files, 13887 bytes uncompressed, 5603 bytes compressed:  59.7%
```

#### zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: README.md
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: README.md
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/demo.zip` & `pretext-1.7.5.dev20230802/pretext/templates/resources/demo.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,35 +1,35 @@
 Zip file size: 172278 bytes, number of entries: 33
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 06:18 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-31 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-31 06:18 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-31 06:17 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-31 06:17 source/ex-first.ptx
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-31 06:17 source/ch-generate.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-31 06:17 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-31 06:17 source/sec-features.ptx
--rw-r--r--  2.0 unx      777 b- defN 23-Jul-31 06:17 source/ww.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-31 06:17 source/ch-empty.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-31 06:17 source/frontmatter.ptx
--rw-r--r--  2.0 unx     2428 b- defN 23-Jul-31 06:17 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-31 06:17 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-31 06:17 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-31 06:17 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-31 06:17 source/ch-features.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-31 06:17 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-31 06:17 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-31 06:17 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-31 06:17 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-31 06:17 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-31 06:17 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-31 06:17 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-31 06:17 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-31 06:17 source/images/tikz.tex
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-31 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-31 06:17 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-02 06:15 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-02 06:15 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-02 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-02 06:14 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-Aug-02 06:14 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Aug-02 06:14 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Aug-02 06:14 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Aug-02 06:14 source/backmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Aug-02 06:14 source/sec-features.ptx
+-rw-r--r--  2.0 unx     2295 b- defN 23-Aug-02 06:14 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Aug-02 06:14 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Aug-02 06:14 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Aug-02 06:14 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Aug-02 06:14 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Aug-02 06:14 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Aug-02 06:14 source/ex-first.ptx
+-rw-r--r--  2.0 unx      777 b- defN 23-Aug-02 06:14 source/ww.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Aug-02 06:14 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Aug-02 06:14 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Aug-02 06:14 source/docinfo.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 23-Aug-02 06:14 source/main.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Aug-02 06:14 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Aug-02 06:14 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Aug-02 06:14 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-02 06:14 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Aug-02 06:14 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Aug-02 06:14 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Aug-02 06:14 publication/publication.ptx
 33 files, 188129 bytes uncompressed, 168462 bytes compressed:  10.5%
```

#### zipnote {}

```diff
@@ -6,95 +6,95 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: README.md
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: README.md
 Comment: 
 
 Filename: source/images/
 Comment: 
 
-Filename: source/ex-first.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/ch-generate.ptx
+Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/backmatter.ptx
 Comment: 
 
-Filename: source/ww.ptx
+Filename: source/sec-features.ptx
 Comment: 
 
-Filename: source/ch-empty.ptx
+Filename: source/ch-generate.ptx
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/sec-first-examples.ptx
+Filename: source/fig-tikz.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/ch-empty.ptx
 Comment: 
 
 Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/ch-features.ptx
-Comment: 
-
-Filename: source/fig-sage2d.ptx
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: source/fig-tikz.ptx
+Filename: source/ww.ptx
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/fig-sage3d.ptx
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
 Filename: source/docinfo.ptx
 Comment: 
 
-Filename: source/images/sageplot2d.sage
+Filename: source/main.ptx
 Comment: 
 
 Filename: source/images/cflag.asy
 Comment: 
 
 Filename: source/images/sageplot3d.sage
 Comment: 
 
 Filename: source/images/tikz.tex
 Comment: 
 
+Filename: source/images/sageplot2d.sage
+Comment: 
+
 Filename: assets/jsxgraph/
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/hello.zip` & `pretext-1.7.5.dev20230802/pretext/templates/resources/hello.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 3496 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 06:18 .gitignore
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-31 06:17 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-31 06:17 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-31 06:17 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-02 06:15 .gitignore
+-rw-r--r--  2.0 unx     1217 b- defN 23-Aug-02 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-02 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-Aug-02 06:14 README.md
+-rw-r--r--  2.0 unx      156 b- defN 23-Aug-02 06:14 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-02 06:14 publication/publication.ptx
 8 files, 5898 bytes uncompressed, 2644 bytes compressed:  55.2%
```

#### zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: README.md
-Comment: 
-
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: README.md
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/project.ptx` & `pretext-1.7.5.dev20230802/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pretext/templates/resources/slideshow.zip` & `pretext-1.7.5.dev20230802/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7231 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 06:17 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 06:18 .gitignore
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-31 06:17 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-31 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-31 06:17 source/main.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-31 06:17 xsl/slides.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-02 06:14 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-02 06:15 .gitignore
+-rw-r--r--  2.0 unx      784 b- defN 23-Aug-02 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-02 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx    11200 b- defN 23-Aug-02 06:14 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Aug-02 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Aug-02 06:14 xsl/slides.xsl
 9 files, 18485 bytes uncompressed, 6285 bytes compressed:  66.0%
```

#### zipnote {}

```diff
@@ -12,17 +12,17 @@
 
 Filename: project.ptx
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: publication/publication.ptx
 Comment: 
 
 Filename: xsl/slides.xsl
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.7.5.dev20230731/pretext/utils.py` & `pretext-1.7.5.dev20230802/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.5.dev20230731/pyproject.toml` & `pretext-1.7.5.dev20230802/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.7.5.dev20230731"
+version = "1.7.5.dev20230802"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.7.5.dev20230731/PKG-INFO` & `pretext-1.7.5.dev20230802/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.7.5.dev20230731
+Version: 1.7.5.dev20230802
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

