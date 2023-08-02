# Comparing `tmp/bbconf-0.3.1.tar.gz` & `tmp/bbconf-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbconf-0.3.1.tar", last modified: Thu Aug 18 22:32:36 2022, max compression
+gzip compressed data, was "bbconf-0.4.0a1.tar", last modified: Wed Aug  2 19:56:28 2023, max compression
```

## Comparing `bbconf-0.3.1.tar` & `bbconf-0.4.0a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 22:32:36.036063 bbconf-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-18 22:32:27.000000 bbconf-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-18 22:32:27.000000 bbconf-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-08-18 22:32:36.036063 bbconf-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-18 22:32:27.000000 bbconf-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 22:32:36.036063 bbconf-0.3.1/bbconf/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    15511 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/bbconf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 22:32:36.036063 bbconf-0.3.1/bbconf/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/schemas/bedfiles_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/schemas/bedsets_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-08-18 22:32:27.000000 bbconf-0.3.1/bbconf/schemas/distance_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 22:32:36.036063 bbconf-0.3.1/bbconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-08-18 22:32:35.000000 bbconf-0.3.1/bbconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-18 22:32:35.000000 bbconf-0.3.1/bbconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 22:32:35.000000 bbconf-0.3.1/bbconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 22:32:35.000000 bbconf-0.3.1/bbconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-18 22:32:35.000000 bbconf-0.3.1/bbconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 22:32:36.036063 bbconf-0.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 22:32:27.000000 bbconf-0.3.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-18 22:32:27.000000 bbconf-0.3.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-18 22:32:27.000000 bbconf-0.3.1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 22:32:36.036063 bbconf-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-08-18 22:32:27.000000 bbconf-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/bbconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/bbconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/bbconf/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/schemas/bedfiles_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/schemas/bedsets_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/bbconf/schemas/distance_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/bbconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-02 19:56:28.000000 bbconf-0.4.0a1/bbconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-02 19:56:28.000000 bbconf-0.4.0a1/bbconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:56:28.000000 bbconf-0.4.0a1/bbconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 19:56:28.000000 bbconf-0.4.0a1/bbconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 19:56:28.000000 bbconf-0.4.0a1/bbconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:56:28.937862 bbconf-0.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-02 19:56:19.000000 bbconf-0.4.0a1/setup.py
```

### Comparing `bbconf-0.3.1/LICENSE.txt` & `bbconf-0.4.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bbconf-0.3.1/PKG-INFO` & `bbconf-0.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbconf
-Version: 0.3.1
+Version: 0.4.0a1
 Summary: Configuration package for bedbase project
 Home-page: https://databio.org
 Author: Michal Stolarczyk
 Author-email: michal@virginia.edu
 License: BSD2
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bbconf-0.3.1/README.md` & `bbconf-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `bbconf-0.3.1/bbconf/const.py` & `bbconf-0.4.0a1/bbconf/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 BED_TABLE = "bedfiles"
 BEDSET_TABLE = "bedsets"
 
 BEDFILES_REL_KEY = "bedfiles"
 BEDSETS_REL_KEY = "bedsets"
 
 
-REL_TABLE = "bedset_bedfiles"
+BEDFILE_BEDSET_ASSOCIATION_TABLE_KEY = "bedset_bedfiles"
 DIST_TABLE = "distances"
 
 CFG_ENV_VARS = ["BEDBASE"]
 
 DB_DEFAULT_HOST = "localhost"
 DB_DEFAULT_USER = "postgres"
 DB_DEFAULT_PASSWORD = "bedbasepassword"
@@ -90,15 +90,15 @@
     "CFG_REMOTE_KEY",
 ]
 
 
 __all__ = [
     "BED_TABLE",
     "BEDSET_TABLE",
-    "REL_TABLE",
+    "BEDFILE_BEDSET_ASSOCIATION_TABLE_KEY",
     "DIST_TABLE",
     "CFG_ENV_VARS",
     "DB_DEFAULT_HOST",
     "SERVER_DEFAULT_PORT",
     "SERVER_DEFAULT_HOST",
     "PKG_NAME",
     "DEFAULT_SECTION_VALUES",
```

### Comparing `bbconf-0.3.1/bbconf/exceptions.py` & `bbconf-0.4.0a1/bbconf/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import abc
-
 from .const import DOC_URL
 
-__all__ = ["BedBaseConfError", "MissingConfigDataError", "BedBaseConnectionError"]
-
 
 class BedBaseConfError(Exception):
     """Base exception type for this package"""
 
     __metaclass__ = abc.ABCMeta
```

### Comparing `bbconf-0.3.1/bbconf/schemas/bedfiles_schema.yaml` & `bbconf-0.4.0a1/bbconf/schemas/bedfiles_schema.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-name:
-  type: string
-  description: BED file name
-md5sum:
-  type: string
-  description: BED file checksum
-genome:
-  type: object
-  description: genome assembly of the BED files
-bedfile:
-  type: file
-  label: bed
-  description: BED file
-bigbedfile:
-  type: file
-  label: bigBed
-  description: bigBed file
-regions_no:
-  type: integer
-  description: Number of regions
-gc_content:
-  type: number
-  description: GC content
-median_tss_dist:
-  type: number
-  description: Median TSS distance
-mean_region_width:
-  type: number
-  description: Mean region width
-exon_frequency:
-  type: number
-  description: Exon frequency
-intron_frequency:
-  type: number
-  description: Intron frequency
-promoterprox_frequency:
-  type: number
-  description: Promoter frequency
-intergenic_frequency:
-  type: number
-  description: Intergenic frequency
-promotercore_frequency:
-  type: number
-  description: Promoter core frequency
-fiveutr_frequency:
-  type: number
-  description: 5' UTR frequency
-threeutr_frequency:
-  type: number
-  description: 3' UTR frequency
-fiveutr_percentage:
-  type: number
-  description: 5' UTR percentage
-threeutr_percentage:
-  type: number
-  description: 3' UTR percentage
-promoterprox_percentage:
-  type: number
-  description: Promoter proc percentage
-exon_percentage:
-  type: number
-  description: Exon percentage
-intron_percentage:
-  type: number
-  description: Intron percentage
-intergenic_percentage:
-  type: number
-  description: Intergenic percentage
-promotercore_percentage:
-  type: number
-  description: Promoter core percentage
-tssdist:
-  type: image
-  label: TSS_distance
-  description: Region-TSS distance plot
-chrombins:
-  type: image
-  label: Chromosome_bins
-  description: Regions distribution over chromosomes plot
-gccontent:
-  type: image
-  label: GC_content
-  description: GC content plot
-paritions:
-  type: image
-  label: Regions_dist_partitions
-  description: Regions distribution over genomic partitions plot
-expected_partitions:
-  type: image
-  label: Expected_partitions
-  description: Expected distribution over genomic partitions plot
-cumulative_partitions:
-  type: image
-  label: Cumulative_partitions
-  description: Cumulative distribution over genomic partitions plot
-widths_histogram:
-  type: image
-  label: Widths_histogram 
-  description: Quantile-trimmed histogram of widths
-neighbor_distances:
-  type: image
-  label: Neighbor_distance
-  description: Distance between neighbor regions
-open_chromatin:
-  type: image
-  label: Open_chromatin
-  description: Cell specific enrichment for open chromatin plot
-other:
-  type: object
-  description: Other, not categorized BED file metadata
+pipeline_name: bedfile
+samples:
+  name:
+    type: string
+    description: BED file name
+  md5sum:
+    type: string
+    description: BED file checksum
+  genome:
+    type: object
+    description: genome assembly of the BED files
+  bedfile:
+    type: file
+    label: bed
+    description: BED file
+  bigbedfile:
+    type: file
+    label: bigBed
+    description: bigBed file
+  regions_no:
+    type: integer
+    description: Number of regions
+  gc_content:
+    type: number
+    description: GC content
+  median_tss_dist:
+    type: number
+    description: Median TSS distance
+  mean_region_width:
+    type: number
+    description: Mean region width
+  exon_frequency:
+    type: number
+    description: Exon frequency
+  intron_frequency:
+    type: number
+    description: Intron frequency
+  promoterprox_frequency:
+    type: number
+    description: Promoter frequency
+  intergenic_frequency:
+    type: number
+    description: Intergenic frequency
+  promotercore_frequency:
+    type: number
+    description: Promoter core frequency
+  fiveutr_frequency:
+    type: number
+    description: 5' UTR frequency
+  threeutr_frequency:
+    type: number
+    description: 3' UTR frequency
+  fiveutr_percentage:
+    type: number
+    description: 5' UTR percentage
+  threeutr_percentage:
+    type: number
+    description: 3' UTR percentage
+  promoterprox_percentage:
+    type: number
+    description: Promoter proc percentage
+  exon_percentage:
+    type: number
+    description: Exon percentage
+  intron_percentage:
+    type: number
+    description: Intron percentage
+  intergenic_percentage:
+    type: number
+    description: Intergenic percentage
+  promotercore_percentage:
+    type: number
+    description: Promoter core percentage
+  tssdist:
+    type: image
+    label: TSS_distance
+    description: Region-TSS distance plot
+  chrombins:
+    type: image
+    label: Chromosome_bins
+    description: Regions distribution over chromosomes plot
+  gccontent:
+    type: image
+    label: GC_content
+    description: GC content plot
+  paritions:
+    type: image
+    label: Regions_dist_partitions
+    description: Regions distribution over genomic partitions plot
+  expected_partitions:
+    type: image
+    label: Expected_partitions
+    description: Expected distribution over genomic partitions plot
+  cumulative_partitions:
+    type: image
+    label: Cumulative_partitions
+    description: Cumulative distribution over genomic partitions plot
+  widths_histogram:
+    type: image
+    label: Widths_histogram
+    description: Quantile-trimmed histogram of widths
+  neighbor_distances:
+    type: image
+    label: Neighbor_distance
+    description: Distance between neighbor regions
+  open_chromatin:
+    type: image
+    label: Open_chromatin
+    description: Cell specific enrichment for open chromatin plot
+  other:
+    type: object
+    description: Other, not categorized BED file metadata
```

### Comparing `bbconf-0.3.1/bbconf.egg-info/PKG-INFO` & `bbconf-0.4.0a1/bbconf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbconf
-Version: 0.3.1
+Version: 0.4.0a1
 Summary: Configuration package for bedbase project
 Home-page: https://databio.org
 Author: Michal Stolarczyk
 Author-email: michal@virginia.edu
 License: BSD2
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bbconf-0.3.1/setup.py` & `bbconf-0.4.0a1/setup.py`

 * *Files identical despite different names*

