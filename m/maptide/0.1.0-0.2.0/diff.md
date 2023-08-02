# Comparing `tmp/maptide-0.1.0.tar.gz` & `tmp/maptide-0.2.0.tar.gz`

## Comparing `maptide-0.1.0.tar` & `maptide-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 maptide-0.1.0/Cargo.toml
--rw-rw-r--   0     1000     1000     1553 2023-01-11 11:06:38.000000 maptide-0.1.0/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000     1803 2023-01-13 11:28:42.000000 maptide-0.1.0/README.md
--rw-rw-r--   0     1000     1000       15 2023-01-13 11:28:43.000000 maptide-0.1.0/example.py
--rw-rw-r--   0     1000     1000      403 2023-01-13 11:28:42.000000 maptide-0.1.0/pyproject.toml
--rw-rw-r--   0     1000     1000      165 2023-01-13 11:28:43.000000 maptide-0.1.0/python/maptide/__init__.py
--rw-rw-r--   0     1000     1000     1099 2023-01-13 11:28:43.000000 maptide-0.1.0/python/maptide/api.py
--rw-rw-r--   0     1000     1000     4038 2023-01-12 13:22:16.000000 maptide-0.1.0/python/maptide/cli.py
--rw-rw-r--   0     1000     1000     1950 2023-01-13 11:32:38.000000 maptide-0.1.0/src/error.rs
--rw-rw-r--   0     1000     1000    18096 2023-01-13 11:32:38.000000 maptide-0.1.0/src/lib.rs
--rw-rw-r--   0     1000     1000    14019 2023-01-13 11:28:43.000000 maptide-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 maptide-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 maptide-0.2.0/Cargo.toml
+-rw-r--r--   0      503       20     1553 2023-07-28 11:03:59.000000 maptide-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0      503       20     2200 2023-08-02 12:05:19.000000 maptide-0.2.0/README.md
+-rw-r--r--   0      503       20      403 2023-07-28 11:04:37.000000 maptide-0.2.0/pyproject.toml
+-rw-r--r--   0      503       20      158 2023-07-31 14:28:42.000000 maptide-0.2.0/python/maptide/__init__.py
+-rw-r--r--   0      503       20     1654 2023-08-02 12:20:42.000000 maptide-0.2.0/python/maptide/api.py
+-rw-r--r--   0      503       20     4010 2023-07-31 17:16:04.000000 maptide-0.2.0/python/maptide/cli.py
+-rw-r--r--   0      503       20     1950 2023-07-28 11:03:26.000000 maptide-0.2.0/src/error.rs
+-rw-r--r--   0      503       20    18068 2023-07-31 17:00:23.000000 maptide-0.2.0/src/lib.rs
+-rw-r--r--   0      503       20    14019 2023-07-31 14:50:41.000000 maptide-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 maptide-0.2.0/PKG-INFO
```

### Comparing `maptide-0.1.0/.github/workflows/CI.yml` & `maptide-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `maptide-0.1.0/README.md` & `maptide-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 # `maptide`
 
 ## Setup
-Current setup instructions require Rust to be installed.
+#### Install via pip
+```
+$ pip install maptide
+```
+Depending on your operating system, the Rust compiler may need to be installed.
 
-Installation instructions for Rust can be found here: https://www.rust-lang.org/tools/install
+Installation instructions for the Rust compiler can be found here: https://www.rust-lang.org/tools/install
 
-Once Rust is installed:
+#### Build from source
+Building from source requires the Rust compiler.
+
+Once the Rust compiler is installed:
 ```
 $ git clone https://github.com/CLIMB-COVID/maptide.git
 $ cd maptide/
 $ python -m venv env
 $ source env/bin/activate
 $ pip install --upgrade pip
 $ pip install .
 ```
 
 ## Usage
 ```
 $ maptide -h
-usage: maptide [-h] [--region REGION] [--index INDEX] [--mapq MAPQ] [--baseq BASEQ] [--noindex] [--stats] [--decimals DECIMALS] bam
+usage: maptide [-h] [-v] [-r REGION] [-i INDEX] [-m MAPPING_QUALITY] [-b BASE_QUALITY] [-s] [-d DECIMALS] bam
 
 positional arguments:
-  bam                  Path to BAM file
+  bam                   Path to BAM file
 
-optional arguments:
-  -h, --help           show this help message and exit
-  --region REGION      Region to view, specified in the form CHROM:START-END (default: everything)
-  --index INDEX        Path to index (BAI) file (default: </path/to/bam>.bai)
-  --mapq MAPQ          Minimum mapping quality (default: 0)
-  --baseq BASEQ        Minimum base quality (default: 0)
-  --noindex            Do not use an index file when querying the BAM file (default: False)
-  --stats              Output additional per-position statistics (default: False)
-  --decimals DECIMALS  Number of decimal places to display (default: 3)
+options:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -r REGION, --region REGION
+                        Region to view, specified in the form CHROM:START-END (default: everything)
+  -i INDEX, --index INDEX
+                        Path to index (BAI) file (default: </path/to/bam>.bai)
+  -m MAPPING_QUALITY, --mapping-quality MAPPING_QUALITY
+                        Minimum mapping quality (default: 0)
+  -b BASE_QUALITY, --base-quality BASE_QUALITY
+                        Minimum base quality (default: 0)
+  -s, --stats           Output additional per-position statistics (default: False)
+  -d DECIMALS, --decimals DECIMALS
+                        Number of decimal places to display (default: 3)
 ```
 
-##### Frequencies over all positions in the reference:
+#### Frequencies over all positions:
 ```
 $ maptide /path/to/file.bam
 ```
 
-##### Frequencies over a specific region (with an index file):
-If the index file has the same path as the BAM file, but with `.bai` appended on the end: 
+#### Frequencies over a region:
 ```
 $ maptide /path/to/file.bam --region chrom:start-end
 ```
+If a region is specified, `maptide` will check for an index file with the same path as the BAM file, but with `.bai` appended on the end (i.e. `/path/to/file.bam.bai`).
 
-Otherwise, the path needs to be specified:
-```
-$ maptide /path/to/file.bam --region chrom:start-end --index /path/to/index.bai
-```
+If an index file does not exist in this location, `maptide` will still run anyway, just without an index file.
 
-##### Frequencies over a specific region (without an index file):
+Index files that do not follow the naming convention `/path/to/file.bam.bai` can still be used, but a path to the file needs to be provided:
 ```
-$ maptide /path/to/file.bam chrom:start-end --region chrom:start-end --noindex
+$ maptide /path/to/file.bam --region chrom:start-end --index /path/to/index.bai
 ```
```

### Comparing `maptide-0.1.0/python/maptide/cli.py` & `maptide-0.2.0/python/maptide/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from .api import query, parse_region
 import argparse
 import math
 import sys
 import csv
+import pkg_resources
+from . import api
 
 
 def entropy(probabilities, normalised=False):
     ent = sum([-(x * math.log2(x)) if x != 0 else 0 for x in probabilities])
 
     if normalised:
         return ent / math.log2(len(probabilities))
@@ -32,15 +33,15 @@
         + counts
         + [round(x, decimals) for x in percentages + [ent, secondary_ent]]
     )
 
 
 def iterate(data, region=None, stats=False, decimals=3):
     if region:
-        chrom, start, end = parse_region(region)
+        chrom, start, end = api.parse_region(region)
         for (pos, ins_pos), row in sorted(data[chrom].items()):
             if (not start or pos >= start) and (not end or pos <= end):
                 if stats:
                     yield [chrom, pos, ins_pos] + get_stats(row, decimals=decimals)
                 else:
                     yield [chrom, pos, ins_pos, sum(row)] + row
     else:
@@ -50,50 +51,54 @@
                     yield [chrom, pos, ins_pos] + get_stats(row, decimals=decimals)
                 else:
                     yield [chrom, pos, ins_pos, sum(row)] + row
 
 
 def run():
     parser = argparse.ArgumentParser()
-    index_group = parser.add_mutually_exclusive_group()
     parser.add_argument("bam", help="Path to BAM file")
     parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version=pkg_resources.get_distribution("maptide").version,
+    )
+    parser.add_argument(
+        "-r",
         "--region",
         help="Region to view, specified in the form CHROM:START-END (default: everything)",
     )
-    index_group.add_argument(
+    parser.add_argument(
+        "-i",
         "--index",
-        default=None,
         help="Path to index (BAI) file (default: </path/to/bam>.bai)",
     )
     parser.add_argument(
-        "--mapq",
+        "-m",
+        "--mapping-quality",
         type=int,
         default=0,
         help="Minimum mapping quality (default: %(default)s)",
     )
     parser.add_argument(
-        "--baseq",
+        "-b",
+        "--base-quality",
         type=int,
         default=0,
         help="Minimum base quality (default: %(default)s)",
     )
-    index_group.add_argument(
-        "--noindex",
-        action="store_true",
-        default=False,
-        help="Do not use an index file when querying the BAM file (default: %(default)s)",
-    )
     parser.add_argument(
+        "-s",
         "--stats",
         action="store_true",
         default=False,
         help="Output additional per-position statistics (default: %(default)s)",
     )
     parser.add_argument(
+        "-d",
         "--decimals",
         type=int,
         default=3,
         help="Number of decimal places to display (default: %(default)s)",
     )
 
     args = parser.parse_args()
@@ -124,20 +129,19 @@
                 "secondary_entropy",
             ]
         )
 
     writer = csv.writer(sys.stdout, delimiter="\t")
     writer.writerow(columns)
 
-    data = query(
+    data = api.query(
         bam=args.bam,
         region=args.region,
         bai=args.index,
-        mapping_quality=args.mapq,
-        base_quality=args.baseq,
-        indexed=not args.noindex,
+        mapping_quality=args.mapping_quality,
+        base_quality=args.base_quality,
     )
 
     for row in iterate(
         data, region=args.region, stats=args.stats, decimals=args.decimals
     ):
         writer.writerow(row)
```

### Comparing `maptide-0.1.0/src/error.rs` & `maptide-0.2.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `maptide-0.1.0/src/lib.rs` & `maptide-0.2.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -283,34 +283,34 @@
     } else {
         Ok(false)
     }
 }
 
 fn init_maps() -> (RefMap, MapTide, RefLengths) {
     // Map of reference names to vector for storing base counts
-    let ref_arrs: RefMap = HashMap::new();
+    let ref_arrs: RefMap = RefMap::new();
 
     // Map of reference names to CoordinateMap, for storing insertion data
     let ins_maps: MapTide = MapTide::new();
 
     // Map of reference names to reference lengths
-    let ref_lengths: RefLengths = HashMap::new();
+    let ref_lengths: RefLengths = RefLengths::new();
 
     (ref_arrs, ins_maps, ref_lengths)
 }
 
 /// Initialise arrays in `ref_arrs`, and CoordinateMaps in `ins_maps`.
 ///
 /// If `region` is `None`, initialises arrays for all positions across all references.
 ///
 /// If `region` is `Some`, initialises array over the region specified.
 fn init_coordinates(
     ref_arrs: &mut RefMap,
     ins_maps: &mut MapTide,
-    ref_lengths: &HashMap<String, usize>,
+    ref_lengths: &RefLengths,
     region: Option<&Region>,
 ) -> Result<(), MapTideError> {
     if let Some(reg) = region {
         let region_name = reg.name();
         let interval = reg.interval();
 
         // Get length of the region name's sequence
@@ -357,15 +357,15 @@
     Ok(())
 }
 
 /// Merge `ref_arrs` into `ins_maps` to have a single `MapTide` containing all coordinates and counts.
 fn merge_into_base_map(
     ref_arrs: &RefMap,
     mut ins_maps: MapTide,
-    ref_lengths: &HashMap<String, usize>,
+    ref_lengths: &RefLengths,
 ) -> Result<MapTide, MapTideError> {
     for (ref_name, _) in ref_lengths.iter() {
         let (ref_arr, offset) = ref_arrs
             .get(ref_name)
             .ok_or_else(|| MapTideError::KeyNotFound)?;
 
         let ins_map = ins_maps
@@ -376,15 +376,15 @@
             ins_map.entry(Coordinate(i + offset + 1, 0)).or_insert(*row);
         }
     }
     Ok(ins_maps)
 }
 
 #[pyfunction]
-fn all_(bam_path: String, mapping_quality: usize, base_quality: usize) -> PyResult<MapTide> {
+fn all(bam_path: String, mapping_quality: usize, base_quality: usize) -> PyResult<MapTide> {
     // Create initial maps
     let (mut ref_arrs, mut ins_maps, mut ref_lengths) = init_maps();
 
     // Reader for iterating through records
     let mut reader = get_reader(bam_path)?;
 
     // Reference sequence information
@@ -447,15 +447,15 @@
     }
 
     let base_map = merge_into_base_map(&ref_arrs, ins_maps, &ref_lengths)?;
     Ok(base_map)
 }
 
 #[pyfunction]
-fn query_(
+fn query(
     bam_path: String,
     bai_path: Option<String>,
     region: String,
     mapping_quality: usize,
     base_quality: usize,
 ) -> PyResult<MapTide> {
     // Create initial maps
@@ -568,15 +568,15 @@
     }
 
     let base_map = merge_into_base_map(&ref_arrs, ins_maps, &ref_lengths)?;
     Ok(base_map)
 }
 
 #[pyfunction]
-fn parse_region_(region: String) -> PyResult<(String, Option<usize>, Option<usize>)> {
+fn parse_region(region: String) -> PyResult<(String, Option<usize>, Option<usize>)> {
     let region: Region = region
         .parse()
         .map_err(|x: ParseError| PyException::new_err(x.to_string()))?;
     let interval = region.interval();
     let start = match interval.start() {
         Some(x) => Some(x.get()),
         None => None,
@@ -588,13 +588,13 @@
 
     Ok((region.name().to_string(), start, end))
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn maptide(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(all_, m)?)?;
-    m.add_function(wrap_pyfunction!(query_, m)?)?;
-    m.add_function(wrap_pyfunction!(parse_region_, m)?)?;
+    m.add_function(wrap_pyfunction!(all, m)?)?;
+    m.add_function(wrap_pyfunction!(query, m)?)?;
+    m.add_function(wrap_pyfunction!(parse_region, m)?)?;
 
     Ok(())
 }
```

### Comparing `maptide-0.1.0/Cargo.lock` & `maptide-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "maptide"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "noodles",
  "pyo3",
 ]
 
 [[package]]
 name = "memchr"
```

### Comparing `maptide-0.1.0/PKG-INFO` & `maptide-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 Metadata-Version: 2.1
 Name: maptide
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # `maptide`
 
 ## Setup
-Current setup instructions require Rust to be installed.
+#### Install via pip
+```
+$ pip install maptide
+```
+Depending on your operating system, the Rust compiler may need to be installed.
 
-Installation instructions for Rust can be found here: https://www.rust-lang.org/tools/install
+Installation instructions for the Rust compiler can be found here: https://www.rust-lang.org/tools/install
 
-Once Rust is installed:
+#### Build from source
+Building from source requires the Rust compiler.
+
+Once the Rust compiler is installed:
 ```
 $ git clone https://github.com/CLIMB-COVID/maptide.git
 $ cd maptide/
 $ python -m venv env
 $ source env/bin/activate
 $ pip install --upgrade pip
 $ pip install .
 ```
 
 ## Usage
 ```
 $ maptide -h
-usage: maptide [-h] [--region REGION] [--index INDEX] [--mapq MAPQ] [--baseq BASEQ] [--noindex] [--stats] [--decimals DECIMALS] bam
+usage: maptide [-h] [-v] [-r REGION] [-i INDEX] [-m MAPPING_QUALITY] [-b BASE_QUALITY] [-s] [-d DECIMALS] bam
 
 positional arguments:
-  bam                  Path to BAM file
+  bam                   Path to BAM file
 
-optional arguments:
-  -h, --help           show this help message and exit
-  --region REGION      Region to view, specified in the form CHROM:START-END (default: everything)
-  --index INDEX        Path to index (BAI) file (default: </path/to/bam>.bai)
-  --mapq MAPQ          Minimum mapping quality (default: 0)
-  --baseq BASEQ        Minimum base quality (default: 0)
-  --noindex            Do not use an index file when querying the BAM file (default: False)
-  --stats              Output additional per-position statistics (default: False)
-  --decimals DECIMALS  Number of decimal places to display (default: 3)
+options:
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
+  -r REGION, --region REGION
+                        Region to view, specified in the form CHROM:START-END (default: everything)
+  -i INDEX, --index INDEX
+                        Path to index (BAI) file (default: </path/to/bam>.bai)
+  -m MAPPING_QUALITY, --mapping-quality MAPPING_QUALITY
+                        Minimum mapping quality (default: 0)
+  -b BASE_QUALITY, --base-quality BASE_QUALITY
+                        Minimum base quality (default: 0)
+  -s, --stats           Output additional per-position statistics (default: False)
+  -d DECIMALS, --decimals DECIMALS
+                        Number of decimal places to display (default: 3)
 ```
 
-##### Frequencies over all positions in the reference:
+#### Frequencies over all positions:
 ```
 $ maptide /path/to/file.bam
 ```
 
-##### Frequencies over a specific region (with an index file):
-If the index file has the same path as the BAM file, but with `.bai` appended on the end: 
+#### Frequencies over a region:
 ```
 $ maptide /path/to/file.bam --region chrom:start-end
 ```
+If a region is specified, `maptide` will check for an index file with the same path as the BAM file, but with `.bai` appended on the end (i.e. `/path/to/file.bam.bai`).
 
-Otherwise, the path needs to be specified:
-```
-$ maptide /path/to/file.bam --region chrom:start-end --index /path/to/index.bai
-```
+If an index file does not exist in this location, `maptide` will still run anyway, just without an index file.
 
-##### Frequencies over a specific region (without an index file):
+Index files that do not follow the naming convention `/path/to/file.bam.bai` can still be used, but a path to the file needs to be provided:
 ```
-$ maptide /path/to/file.bam chrom:start-end --region chrom:start-end --noindex
+$ maptide /path/to/file.bam --region chrom:start-end --index /path/to/index.bai
 ```
```

