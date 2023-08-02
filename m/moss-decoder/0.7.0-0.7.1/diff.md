# Comparing `tmp/moss_decoder-0.7.0.tar.gz` & `tmp/moss_decoder-0.7.1.tar.gz`

## Comparing `moss_decoder-0.7.0.tar` & `moss_decoder-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.7.0/Cargo.toml
--rw-r--r--   0     1001      123      633 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      373 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.github/workflows/bench-py.yml
--rw-r--r--   0     1001      123      404 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      715 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.gitignore
--rw-r--r--   0     1001      123      757 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     8953 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/README.md
--rw-r--r--   0     1001      123      360 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/benchmark.rs
--rw-r--r--   0     1001      123      406 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/decode_from_file_bench.rs
--rw-r--r--   0     1001      123      450 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/decode_multiple_events_bench.rs
--rw-r--r--   0     1001      123      446 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/decode_single_event_bench.rs
--rw-r--r--   0     1001      123     1090 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/python310.dll
--rw-r--r--   0     1001      123    15038 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/decode_hits_fsm.rs
--rw-r--r--   0     1001      123    13880 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1854 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     2847 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol/test_util.rs
--rw-r--r--   0     1001      123     2263 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol.rs
--rw-r--r--   0     1001      123     1321 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/parse_error.rs
--rw-r--r--   0     1001      123     3992 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/parse_util.rs
--rwxr-xr-x   0     1001      123      435 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123    10901 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/integration.py
--rw-r--r--   0     1001      123    14398 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/integration_test.rs
--rwxr-xr-x   0     1001      123     1190 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      840 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123  9582576 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/moss_noise.raw
--rw-r--r--   0     1001      123      500 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/moss_noise_0-499b.raw
--rw-r--r--   0     1001      123      500 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/moss_noise_500-999b.raw
--rw-r--r--   0     1001      123    26544 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/noise_all_regions.raw
--rw-r--r--   0     1001      123    22700 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/noise_random_region.raw
--rw-r--r--   0     1001      123    20000 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/pattern_all_regions.raw
--rw-r--r--   0     1001      123      954 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/utils.sh
--rw-r--r--   0     1001      123    24141 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/Cargo.lock
--rw-r--r--   0        0        0     9507 1970-01-01 00:00:00.000000 moss_decoder-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.7.1/Cargo.toml
+-rw-r--r--   0     1001      123      633 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      373 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/.github/workflows/bench-py.yml
+-rw-r--r--   0     1001      123      404 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123      715 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/.gitignore
+-rw-r--r--   0     1001      123      757 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     8953 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/README.md
+-rw-r--r--   0     1001      123      360 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/benches/benchmark.rs
+-rw-r--r--   0     1001      123      406 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/benches/decode_from_file_bench.rs
+-rw-r--r--   0     1001      123      450 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/benches/decode_multiple_events_bench.rs
+-rw-r--r--   0     1001      123      446 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/benches/decode_single_event_bench.rs
+-rw-r--r--   0     1001      123     1090 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/python310.dll
+-rw-r--r--   0     1001      123    15038 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/decode_hits_fsm.rs
+-rw-r--r--   0     1001      123    13689 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1854 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     2847 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/moss_protocol/test_util.rs
+-rw-r--r--   0     1001      123     2263 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/moss_protocol.rs
+-rw-r--r--   0     1001      123     1321 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/parse_error.rs
+-rw-r--r--   0     1001      123     3992 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/src/parse_util.rs
+-rwxr-xr-x   0     1001      123      435 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123    13191 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/integration.py
+-rw-r--r--   0     1001      123    14398 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/integration_test.rs
+-rwxr-xr-x   0     1001      123     1190 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      840 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123  9582576 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/test-data/moss_noise.raw
+-rw-r--r--   0     1001      123      500 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/test-data/moss_noise_0-499b.raw
+-rw-r--r--   0     1001      123      500 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/test-data/moss_noise_500-999b.raw
+-rw-r--r--   0     1001      123    26544 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/test-data/noise_all_regions.raw
+-rw-r--r--   0     1001      123    22700 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/test-data/noise_random_region.raw
+-rw-r--r--   0     1001      123    20000 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/test-data/pattern_all_regions.raw
+-rw-r--r--   0     1001      123      954 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/tests/utils.sh
+-rw-r--r--   0     1001      123    24141 2023-08-02 10:18:11.000000 moss_decoder-0.7.1/Cargo.lock
+-rw-r--r--   0        0        0     9507 1970-01-01 00:00:00.000000 moss_decoder-0.7.1/PKG-INFO
```

### Comparing `moss_decoder-0.7.0/Cargo.toml` & `moss_decoder-0.7.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.7.0"
+version = "0.7.1"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.7.0/.CERN-gitlab-ci.yml` & `moss_decoder-0.7.1/.CERN-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/.github/workflows/CI.yml` & `moss_decoder-0.7.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/.gitignore` & `moss_decoder-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/.pre-commit-config.yaml` & `moss_decoder-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/README.md` & `moss_decoder-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/moss_decoder.pyi` & `moss_decoder-0.7.1/moss_decoder.pyi`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/pyproject.toml` & `moss_decoder-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/python310.dll` & `moss_decoder-0.7.1/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/decode_hits_fsm.rs` & `moss_decoder-0.7.1/src/decode_hits_fsm.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/lib.rs` & `moss_decoder-0.7.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -148,18 +148,15 @@
         while last_trailer_idx < bytes_read - MINIMUM_EVENT_SIZE - 1 {
             match rust_only::extract_packet_from_buf(&bytes_to_decode[last_trailer_idx..], None) {
                 Ok((moss_packet, trailer_idx)) => {
                     moss_packets.push(moss_packet);
                     last_trailer_idx += trailer_idx + 1;
                 }
                 Err(e) if e.kind() == ParseErrorKind::EndOfBufferNoTrailer => {
-                    return Err(PyBytesWarning::new_err(format!(
-                        "Failed decoding packet #{packet_cnt}: {e}",
-                        packet_cnt = moss_packets.len() + 1
-                    )));
+                    break;
                 }
                 Err(e) => return Err(PyAssertionError::new_err(format!("Decoding failed: {e}",))),
             }
         }
 
         // Remove the processed bytes from bytes_to_decode (it now contains the remaining bytes that could did not form a complete event)
         bytes_to_decode = bytes_to_decode[last_trailer_idx..].to_vec();
```

### Comparing `moss_decoder-0.7.0/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.7.1/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.7.1/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/moss_protocol/test_util.rs` & `moss_decoder-0.7.1/src/moss_protocol/test_util.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/moss_protocol.rs` & `moss_decoder-0.7.1/src/moss_protocol.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/parse_error.rs` & `moss_decoder-0.7.1/src/parse_error.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/src/parse_util.rs` & `moss_decoder-0.7.1/src/parse_util.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/integration.py` & `moss_decoder-0.7.1/tests/integration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Integration tests. Uses the `moss_decoder` package
 from python and allows benchmarks."""
 import sys  # Don't want to depend on `argparse`
 import time
 from pathlib import Path
+from typing import Optional
 import moss_decoder
 from moss_decoder import MossPacket, MossHit
 from moss_decoder import decode_event
 
 FILE_MOSS_NOISE = Path("tests/test-data/moss_noise.raw")
 FILE_MOSS_NOISE_ALL_REGION = Path("tests/test-data/noise_all_regions.raw")
 FILE_NOISE_RANDOM_REGION = Path("tests/test-data/noise_random_region.raw")
 FILE_PATTERN_ALL_REGIONS = Path("tests/test-data/pattern_all_regions.raw")
 FILE_4_EVENTS_PARTIAL_END = Path("tests/test-data/moss_noise_0-499b.raw")
 FILE_3_EVENTS_PARTIAL_START = Path("tests/test-data/moss_noise_500-999b.raw")
 
 
 class MockMossDecoder:
-    _data_files: list[Path] = None
+    _data_files: Optional[list[Path]] = None
     _current_file_idx = 0
     _current_file_events_decoded = 0
 
-    def __init__(self, data_files: list[Path]) -> "MockMossDecoder":
+    def __init__(self, data_files: Optional[list[Path]] = None) -> "MockMossDecoder":
         self._data_files = data_files
 
     def get_next_n_events(self, events: int) -> list[MossPacket]:
         """Read N events from the current file, if it has less than N events,
         try to get the rest in the next file"""
         buf = read_bytes_from_file(self._data_files[self._current_file_idx])
         try:
@@ -75,14 +76,27 @@
             )
             if len(rest_of_packets) != 0:
                 self._current_file_events_decoded += len(rest_of_packets) - 1
             print(f"Second file read, got: {len(rest_of_packets)}")
             packets.extend(rest_of_packets)
             return packets
 
+    def decode_from_file(self, file_path: Path) -> list[MossPacket]:
+        """Decode raw MOSS readout data `MossPacket` objects from a file
+        and return list of `MossPacket` objects"""
+        assert isinstance(
+            file_path, Path
+        ), f'Argument must be type Path, got {type(file_path)}. \
+    Supply the file path with: Path("path/to/file")'
+        assert file_path.is_file(), f"File does not exist: {file_path}"
+
+        packets = moss_decoder.decode_from_file(file_path)
+
+        return packets
+
 
 def read_bytes_from_file(file_path: Path) -> bytes:
     """Open file at `file_path` and read as binary, return `bytes`"""
     print(f"Reading from file {file_path}")
     with open(file_path, "rb") as readout_file:
         raw_bytes = readout_file.read()
 
@@ -114,14 +128,42 @@
         + region_header_3
         + unit_frame_trailer
         + padding
     )
     return simple_packet
 
 
+def test_decode_100mb_file(file_path: Path, expect_packets: int):
+    big_file = Path("100mb-data.raw")
+    if big_file.exists():
+        big_file.unlink()
+    # Read the content of the input binary file
+    with open(file_path, "rb") as input_file:
+        content = input_file.read()
+
+    # Append the content multiple times to the output binary file
+    with open(big_file, "ab") as output_file:
+        for _ in range(10):
+            output_file.write(content)
+    start = time.time()
+    test_decode_all_from_file(file_path=big_file, expect_packets=expect_packets * 10)
+    print(f"Done in: {time.time()-start:.3f} s\n")
+    big_file.unlink()
+
+
+def test_decode_all_from_file(file_path: Path, expect_packets: int):
+    decoder = MockMossDecoder()
+    print(f"Decoding all from file {file_path}")
+    packets = decoder.decode_from_file(file_path)
+    assert (
+        len(packets) == expect_packets
+    ), f"Expected {expect_packets}, got {len(packets)}"
+    print("==> Test OK")
+
+
 def test_decode_partial_events_from_two_files():
     decoder = MockMossDecoder([FILE_4_EVENTS_PARTIAL_END, FILE_3_EVENTS_PARTIAL_START])
 
     packets = decoder.get_next_n_events(2)
     assert len(packets) == 2, f"Expected 2 packets, got {len(packets)}: {packets}"
     packets = decoder.get_next_n_events(2)
     assert len(packets) == 2, f"Expected 2 packets, got {len(packets)}: {packets}"
@@ -280,14 +322,30 @@
             test_decode_multi_event(path=FILE_MOSS_NOISE, expect_remainder_bytes=1)
             sys.exit(0)
 
     test_fundamental_class_comparisons()
     test_decode_partial_events_from_two_files()
 
     start = time.time()
+    test_decode_all_from_file(file_path=FILE_MOSS_NOISE, expect_packets=100000)
+    print(f"Done in: {time.time()-start:.3f} s\n")
+
+    start = time.time()
+    test_decode_all_from_file(file_path=FILE_NOISE_RANDOM_REGION, expect_packets=1044)
+    print(f"Done in: {time.time()-start:.3f} s\n")
+
+    start = time.time()
+    test_decode_all_from_file(file_path=FILE_PATTERN_ALL_REGIONS, expect_packets=1000)
+    print(f"Done in: {time.time()-start:.3f} s\n")
+
+    start = time.time()
+    test_decode_all_from_file(file_path=FILE_MOSS_NOISE_ALL_REGION, expect_packets=1000)
+    print(f"Done in: {time.time()-start:.3f} s\n")
+
+    start = time.time()
     test_decode_multi_event(path=FILE_MOSS_NOISE, expect_remainder_bytes=1)
     print(f"Done in: {time.time()-start:.3f} s\n")
 
     start = time.time()
     test_decode_multi_event(path=FILE_MOSS_NOISE_ALL_REGION, expect_remainder_bytes=1)
     print(f"Done in: {time.time()-start:.3f} s\n")
 
@@ -299,10 +357,12 @@
     test_decode_multi_event(path=FILE_PATTERN_ALL_REGIONS, expect_remainder_bytes=2)
     print(f"Done in: {time.time()-start:.3f} s\n")
 
     start = time.time()
     test_moss_packet_print()
     print(f"Done in: {time.time()-start:.3f} s\n")
 
+    test_decode_100mb_file(file_path=FILE_MOSS_NOISE, expect_packets=100000)
+
     start = time.time()
     test_100k_single_decodes()
     print(f"Done in: {time.time()-start:.3f} s\n")
```

### Comparing `moss_decoder-0.7.0/tests/integration_test.rs` & `moss_decoder-0.7.1/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/performance_dev_py.sh` & `moss_decoder-0.7.1/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/performance_prod_py.sh` & `moss_decoder-0.7.1/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/test-data/moss_noise.raw` & `moss_decoder-0.7.1/tests/test-data/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/test-data/noise_all_regions.raw` & `moss_decoder-0.7.1/tests/test-data/noise_all_regions.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/test-data/noise_random_region.raw` & `moss_decoder-0.7.1/tests/test-data/noise_random_region.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/test-data/pattern_all_regions.raw` & `moss_decoder-0.7.1/tests/test-data/pattern_all_regions.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/tests/utils.sh` & `moss_decoder-0.7.1/tests/utils.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.7.0/Cargo.lock` & `moss_decoder-0.7.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "criterion",
  "pretty_assertions",
  "pyo3",
  "sm",
 ]
```

### Comparing `moss_decoder-0.7.0/PKG-INFO` & `moss_decoder-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.7.0
+Version: 0.7.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
```

