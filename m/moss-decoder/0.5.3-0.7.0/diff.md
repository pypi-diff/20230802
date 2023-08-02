# Comparing `tmp/moss_decoder-0.5.3.tar.gz` & `tmp/moss_decoder-0.7.0.tar.gz`

## Comparing `moss_decoder-0.5.3.tar` & `moss_decoder-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.5.3/Cargo.toml
--rw-r--r--   0     1001      123      633 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      373 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/.github/workflows/bench-py.yml
--rw-r--r--   0     1001      123      404 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      715 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/.gitignore
--rw-r--r--   0     1001      123      757 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7662 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/README.md
--rw-r--r--   0     1001      123      360 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/benches/benchmark.rs
--rw-r--r--   0     1001      123      396 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/benches/decode_from_file_bench.rs
--rw-r--r--   0     1001      123      445 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/benches/decode_multiple_events_bench.rs
--rw-r--r--   0     1001      123      436 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/benches/decode_single_event_bench.rs
--rw-r--r--   0     1001      123      799 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/python310.dll
--rw-r--r--   0     1001      123    14999 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/decode_hits_fsm.rs
--rw-r--r--   0     1001      123    11918 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1854 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     2847 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/moss_protocol/test_util.rs
--rw-r--r--   0     1001      123     2263 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/moss_protocol.rs
--rw-r--r--   0     1001      123     1321 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/parse_error.rs
--rw-r--r--   0     1001      123     3992 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/src/parse_util.rs
--rwxr-xr-x   0     1001      123      435 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     6433 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/integration.py
--rw-r--r--   0     1001      123    11186 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/moss_noise.raw
--rw-r--r--   0     1001      123      500 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/moss_noise_0-499b.raw
--rw-r--r--   0     1001      123      500 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/moss_noise_500-999b.raw
--rwxr-xr-x   0     1001      123     1190 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      840 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      954 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/tests/utils.sh
--rw-r--r--   0     1001      123    24141 2023-08-01 14:06:42.000000 moss_decoder-0.5.3/Cargo.lock
--rw-r--r--   0        0        0     8216 1970-01-01 00:00:00.000000 moss_decoder-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 moss_decoder-0.7.0/Cargo.toml
+-rw-r--r--   0     1001      123      633 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      373 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.github/workflows/bench-py.yml
+-rw-r--r--   0     1001      123      404 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123      715 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.gitignore
+-rw-r--r--   0     1001      123      757 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     8953 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/README.md
+-rw-r--r--   0     1001      123      360 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/benchmark.rs
+-rw-r--r--   0     1001      123      406 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/decode_from_file_bench.rs
+-rw-r--r--   0     1001      123      450 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/decode_multiple_events_bench.rs
+-rw-r--r--   0     1001      123      446 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/benches/decode_single_event_bench.rs
+-rw-r--r--   0     1001      123     1090 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/python310.dll
+-rw-r--r--   0     1001      123    15038 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/decode_hits_fsm.rs
+-rw-r--r--   0     1001      123    13880 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1854 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     2847 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol/test_util.rs
+-rw-r--r--   0     1001      123     2263 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/moss_protocol.rs
+-rw-r--r--   0     1001      123     1321 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/parse_error.rs
+-rw-r--r--   0     1001      123     3992 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/src/parse_util.rs
+-rwxr-xr-x   0     1001      123      435 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123    10901 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/integration.py
+-rw-r--r--   0     1001      123    14398 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/integration_test.rs
+-rwxr-xr-x   0     1001      123     1190 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      840 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123  9582576 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/moss_noise.raw
+-rw-r--r--   0     1001      123      500 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/moss_noise_0-499b.raw
+-rw-r--r--   0     1001      123      500 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/moss_noise_500-999b.raw
+-rw-r--r--   0     1001      123    26544 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/noise_all_regions.raw
+-rw-r--r--   0     1001      123    22700 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/noise_random_region.raw
+-rw-r--r--   0     1001      123    20000 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/test-data/pattern_all_regions.raw
+-rw-r--r--   0     1001      123      954 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/tests/utils.sh
+-rw-r--r--   0     1001      123    24141 2023-08-02 09:00:41.000000 moss_decoder-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     9507 1970-01-01 00:00:00.000000 moss_decoder-0.7.0/PKG-INFO
```

### Comparing `moss_decoder-0.5.3/Cargo.toml` & `moss_decoder-0.7.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.5.3"
+version = "0.7.0"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.5.3/.CERN-gitlab-ci.yml` & `moss_decoder-0.7.0/.CERN-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/.github/workflows/CI.yml` & `moss_decoder-0.7.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/.gitignore` & `moss_decoder-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/.pre-commit-config.yaml` & `moss_decoder-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/README.md` & `moss_decoder-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Python package implemented in Rust for high-performance decoding of readout data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
 
 - [MOSS Decoder](#moss-decoder)
   - [Installation](#installation)
     - [Example](#example)
   - [Features](#features)
-    - [3 types of functions are provided](#3-types-of-functions-are-provided)
+    - [5 types of idempotent functions are provided](#5-types-of-idempotent-functions-are-provided)
   - [MOSS event data packet protocol FSM](#moss-event-data-packet-protocol-fsm)
   - [MOSS event data packet decoder FSM](#moss-event-data-packet-decoder-fsm)
   - [Event packet hit decoder FSM](#event-packet-hit-decoder-fsm)
   - [Motivation \& Purpose](#motivation--purpose)
   - [@CERN Gitlab installation for CentOS and similar distributions from local build](#cern-gitlab-installation-for-centos-and-similar-distributions-from-local-build)
     - [Troubleshooting](#troubleshooting)
 
@@ -41,35 +41,61 @@
 ```
 
 ## Features
 See [python types](moss_decoder.pyi) for the type information the package exposes to Python.
 
 Two classes are provided: `MossPacket` & `MossHit`.
 
-### 3 types of functions are provided
+### 5 types of idempotent functions are provided
 ```python
 decode_event(arg: bytes)  -> tuple[MossPacket, int]: ...
 # allows decoding a single event from an iterable of bytes
 ```
 
 **Returns**: the decoded `MossPacket` and the index the *unit frame trailer* was found. Throws if no valid `MossPacket` is found.
 ```python
-decode_multiple_events(arg: bytes) -> tuple[list[MossPacket], int]: ...
+decode_all_events(arg: bytes) -> tuple[list[MossPacket], int]: ...
 # returns as many `MossPacket`s as can be decoded from the bytes iterable.
 # This is much more effecient than calling `decode_event` multiple times.
 ```
-**Returns**: A list of `MossPacket`s and the index of the last observed *unit frame trailer*. Throws if no valid `MossPacket`s are found.
+**Returns**: A list of `MossPacket`s and the index of the last observed *unit frame trailer*. Throws if no valid `MossPacket`s are found or a protocol error is encountered.
 
 ```python
 decode_from_file(arg: str | Path) -> list[MossPacket]: ...
 # takes a `Path` and returns as many `MossPacket` as can be decoded from file.
 # This is the most effecient way of decoding data from a file.
 ```
-**Returns**: A list of `MossPacket`s. Throws if the file is not found or no valid `MossPacket`s are found.
+**Returns**: A list of `MossPacket`s. Throws if the file is not found, no valid `MossPacket`s are found, or a protocol error is encountered.
 
+```python
+decode_n_events(
+    bytes: bytes,
+    take: int,
+    skip: Optional[int] = None,
+    prepend_buffer: Optional[bytes] = None,
+) -> tuple[list[MossPacket], int]: ...
+# Decode N events from bytes
+# Optionally provide either (not both):
+#    - Skip M events before decoding N events
+#    - Prepend a buffer before decoding N events.
+```
+**Returns**: A list of `MossPacket`s. Throws if the file is not found, no valid `MossPacket`s are found, or a protocol error is encountered.
+
+A `BytesWarning` exception is thrown if the end of the `bytes` is reached while decoding a packet (no trailer is found)
+
+```python
+def skip_n_take_all(
+    bytes: bytes, skip: int = None
+) -> tuple[list[MossPacket], Optional[bytes]]: ...
+# Decode all events, optionally skip N events first.
+# return all decoded events and the remaining bytes after decoding the last MossPacket
+```
+**Returns**: All decoded events and any remaining bytes after the last trailer seen.
+
+Using `decode_n_events` and `skip_n_take_all` it is possible to continuously decode multiple files that potentially ends or starts with partial events.
 
 ## MOSS event data packet protocol FSM
 The a MOSS half-unit event data packet follows the states seen in the FSM below. The region header state is simplified here.
 ```mermaid
 stateDiagram-v2
   frame_header : Unit Frame Header
   frame_trailer : Unit Frame Trailer
@@ -78,14 +104,15 @@
   data_1 : Data 1
   data_2 : Data 2
   idle : Idle
 
     [*] --> frame_header
 
     frame_header --> region_header
+    frame_header --> frame_trailer
 
     region_header --> region_header
     region_header --> frame_trailer
     region_header --> DATA
 
     state DATA {
       direction LR
@@ -98,14 +125,15 @@
 
     DATA --> idle
     DATA --> region_header
     DATA --> frame_trailer
 
 
     idle --> DATA
+    idle --> idle
     idle --> frame_trailer
 
     frame_trailer --> [*]
 
 ```
 
 ## MOSS event data packet decoder FSM
@@ -125,14 +153,15 @@
   delimiter --> delimiter
 
   state EVENT {
 
     [*] --> frame_header
 
     frame_header --> HITS
+    frame_header --> frame_trailer
 
     state HITS {
       [*] --> [*] : decode hits
     }
 
     HITS --> frame_trailer
```

### Comparing `moss_decoder-0.5.3/moss_decoder.pyi` & `moss_decoder-0.7.0/moss_decoder.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Performant decoding of MOSS readout data implemented in Rust"""
 
 from pathlib import Path
+from typing import Optional
 
 class MossHit:
     """A MOSS hit instance"""
 
     region: int
     column: int
     row: int
@@ -20,10 +21,19 @@
     unit_id: int
     hits: list[MossHit]
 
     def __init__(self, unit_id: int) -> MossPacket:
         self.unit_id = unit_id
         self.hits = []
 
-def decode_event(raw_bytes: bytes) -> tuple[MossPacket, int]: ...
-def decode_multiple_events(raw_bytes: bytes) -> tuple[list[MossPacket], int]: ...
+def decode_event(bytes: bytes) -> tuple[MossPacket, int]: ...
+def decode_all_events(bytes: bytes) -> tuple[list[MossPacket], int]: ...
 def decode_from_file(path: str | Path) -> list[MossPacket]: ...
+def decode_n_events(
+    bytes: bytes,
+    take: int,
+    skip: Optional[int] = None,
+    prepend_buffer: Optional[bytes] = None,
+) -> tuple[list[MossPacket], int]: ...
+def skip_n_take_all(
+    bytes: bytes, skip: int = None
+) -> tuple[list[MossPacket], Optional[bytes]]: ...
```

### Comparing `moss_decoder-0.5.3/pyproject.toml` & `moss_decoder-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/python310.dll` & `moss_decoder-0.7.0/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/src/decode_hits_fsm.rs` & `moss_decoder-0.7.0/src/decode_hits_fsm.rs`

 * *Files 2% similar despite different names*

```diff
@@ -350,15 +350,15 @@
     moss_hits.last_mut().unwrap().column |= (data2 & 0x3F) as u16;
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::moss_protocol::test_util::*;
-    use crate::rust_only::extract_packet;
+    use crate::rust_only::extract_packet_from_buf;
     use pretty_assertions::assert_eq;
 
     #[test]
     fn test_fsm() {
         //
         let event_data_packet = fake_event_simple();
         let slice = &event_data_packet;
@@ -425,26 +425,26 @@
             panic!("Decoding failed")
         }
     }
 
     #[test]
     fn test_extract_packet() {
         let packet = fake_event_simple();
-        let p = extract_packet(&packet);
+        let p = extract_packet_from_buf(&packet, None);
         println!("{p:?}");
         assert!(p.is_ok());
         let (p, trailer_idx) = p.unwrap();
         assert_eq!(p.hits.len(), 4);
         assert_eq!(trailer_idx, 18);
     }
 
     #[test]
     fn test_protocol_error() {
         let packet = fake_event_protocol_error();
 
-        if let Err(e) = extract_packet(&packet) {
+        if let Err(e) = extract_packet_from_buf(&packet, None) {
             println!("{e:?}");
         } else {
             panic!("Expected error, got OK")
         }
     }
 }
```

### Comparing `moss_decoder-0.5.3/src/lib.rs` & `moss_decoder-0.7.0/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -17,75 +17,85 @@
     clippy::needless_pass_by_value,
     clippy::unnecessary_wraps,
     clippy::mutex_integer,
     clippy::mem_forget,
     clippy::maybe_infinite_iter
 )]
 
-use std::io::Read;
-
 pub use moss_protocol::MossPacket;
 use parse_error::ParseErrorKind;
 use parse_util::find_trailer_n_idx;
 use pyo3::exceptions::{PyAssertionError, PyBytesWarning, PyFileNotFoundError, PyValueError};
 use pyo3::prelude::*;
+use std::io::Read;
 
 pub mod moss_protocol;
 pub use moss_protocol::MossHit;
 pub mod decode_hits_fsm;
 pub(crate) mod parse_error;
 pub(crate) mod parse_util;
 
 /// A Python module for decoding raw MOSS data effeciently in Rust.
 #[pymodule]
 fn moss_decoder(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(decode_event, m)?)?;
-    m.add_function(wrap_pyfunction!(decode_multiple_events, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_all_events, m)?)?;
     m.add_function(wrap_pyfunction!(decode_from_file, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_n_events, m)?)?;
+    m.add_function(wrap_pyfunction!(skip_n_take_all, m)?)?;
 
     m.add_class::<MossHit>()?;
     m.add_class::<MossPacket>()?;
 
     Ok(())
 }
 
+#[allow(non_camel_case_types)]
+type List_MossPackets = Vec<MossPacket>;
+
+#[allow(non_camel_case_types)]
+type Tuple_MossPacket_LastTrailerIdx = (MossPacket, usize);
+
+#[allow(non_camel_case_types)]
+type Tuple_List_MossPackets_LastTrailerIdx = (List_MossPackets, usize);
+
 const READER_BUFFER_CAPACITY: usize = 10 * 1024 * 1024; // 10 MiB
 const MINIMUM_EVENT_SIZE: usize = 2;
 
 /// Decodes a single MOSS event into a [MossPacket] and the index of the trailer byte.
 /// This function returns an error if no MOSS packet is found, therefor if there's any chance the argument does not contain a valid `MossPacket`
-/// the call should be enclosed in a try/catch.
+/// the call should be enclosed in a try/except.
 #[pyfunction]
-pub fn decode_event(bytes: &[u8]) -> PyResult<(MossPacket, usize)> {
+pub fn decode_event(bytes: &[u8]) -> PyResult<Tuple_MossPacket_LastTrailerIdx> {
     let byte_cnt = bytes.len();
 
     if byte_cnt < MINIMUM_EVENT_SIZE {
         return Err(PyValueError::new_err(
             "Received less than the minimum event size",
         ));
     }
 
-    match rust_only::extract_packet(bytes) {
+    match rust_only::extract_packet_from_buf(bytes, None) {
         Ok((moss_packet, trailer_idx)) => Ok((moss_packet, trailer_idx)),
         Err(e) => Err(PyAssertionError::new_err(format!("Decoding failed: {e}",))),
     }
 }
 
 #[pyfunction]
-/// Decodes multiple MOSS events into a list of [MossPacket]s.
-/// This function is optimized for speed and memory usage.
-pub fn decode_multiple_events(bytes: &[u8]) -> PyResult<(Vec<MossPacket>, usize)> {
+/// Decodes as many MOSS events as possible into a list of [MossPacket]s.
+/// Optimized for speed and memory usage.
+pub fn decode_all_events(bytes: &[u8]) -> PyResult<Tuple_List_MossPackets_LastTrailerIdx> {
     let approx_moss_packets = rust_only::calc_prealloc_val(bytes)?;
 
     let mut moss_packets: Vec<MossPacket> = Vec::with_capacity(approx_moss_packets);
 
     let mut last_trailer_idx = 0;
 
     while last_trailer_idx < bytes.len() - MINIMUM_EVENT_SIZE - 1 {
-        match rust_only::extract_packet(&bytes[last_trailer_idx..]) {
+        match rust_only::extract_packet_from_buf(&bytes[last_trailer_idx..], None) {
             Ok((moss_packet, trailer_idx)) => {
                 moss_packets.push(moss_packet);
                 last_trailer_idx += trailer_idx + 1;
             }
             Err(e) if e.kind() == ParseErrorKind::EndOfBufferNoTrailer => {
                 return Err(PyBytesWarning::new_err(format!(
                     "Failed decoding packet #{packet_cnt}: {e}",
@@ -99,21 +109,21 @@
     if moss_packets.is_empty() {
         Err(PyAssertionError::new_err("No MOSS Packets in events"))
     } else {
         Ok((moss_packets, last_trailer_idx - 1))
     }
 }
 
-#[pyfunction]
 /// Decodes a file containing raw MOSS data into a list of [MossPacket]s.
 ///
 /// The file is read in chunks of 10 MiB until the end of the file is reached.
-/// If any errors are encountered while reading the file, any successfully decoded events are returned.
+/// If any errors are encountered while reading the file, an exception is thrown.
 /// There's no attempt to run over errors.
-pub fn decode_from_file(path: std::path::PathBuf) -> PyResult<Vec<MossPacket>> {
+#[pyfunction]
+pub fn decode_from_file(path: std::path::PathBuf) -> PyResult<List_MossPackets> {
     // Open file (get file descriptor)
     let file = match std::fs::File::open(path) {
         Ok(file) => file,
         Err(e) => return Err(PyFileNotFoundError::new_err(e.to_string())),
     };
 
     // Create buffered reader with 1MB capacity to minimize syscalls to read
@@ -132,15 +142,15 @@
         let mut last_trailer_idx = 0;
 
         // Extend bytes_to_decode with the new data
         bytes_to_decode.extend_from_slice(&buf[..bytes_read]);
 
         // Decode the bytes one event at a time until there's no more events to decode
         while last_trailer_idx < bytes_read - MINIMUM_EVENT_SIZE - 1 {
-            match rust_only::extract_packet(&bytes_to_decode[last_trailer_idx..]) {
+            match rust_only::extract_packet_from_buf(&bytes_to_decode[last_trailer_idx..], None) {
                 Ok((moss_packet, trailer_idx)) => {
                     moss_packets.push(moss_packet);
                     last_trailer_idx += trailer_idx + 1;
                 }
                 Err(e) if e.kind() == ParseErrorKind::EndOfBufferNoTrailer => {
                     return Err(PyBytesWarning::new_err(format!(
                         "Failed decoding packet #{packet_cnt}: {e}",
@@ -158,36 +168,45 @@
     if moss_packets.is_empty() {
         Err(PyAssertionError::new_err("No MOSS Packets in events"))
     } else {
         Ok(moss_packets)
     }
 }
 
+/// Decodes N events from the given bytes.
+/// Optionally allows for either (not both):
+/// - skipping `skip` events before decoding.
+/// - prepending `prepend_buffer` to the bytes before decoding.
 #[pyfunction]
-/// Decodes N events from the given bytes. Optionally skips `skip` events before decoding.
-pub fn decode_events_take_n(
+pub fn decode_n_events(
     bytes: &[u8],
     take: usize,
     skip: Option<usize>,
-) -> PyResult<(Vec<MossPacket>, usize)> {
+    mut prepend_buffer: Option<Vec<u8>>,
+) -> PyResult<Tuple_List_MossPackets_LastTrailerIdx> {
     let mut moss_packets: Vec<MossPacket> = Vec::with_capacity(take);
 
     // Skip N events
     if skip.is_some_and(|s| s == 0) {
         return Err(PyValueError::new_err("skip value must be greater than 0"));
+    } else if skip.is_some() && prepend_buffer.is_some() {
+        return Err(PyValueError::new_err(
+            "skip and prepend_buffer cannot be used together",
+        ));
     }
 
     let mut last_trailer_idx = if let Some(skip) = skip {
         find_trailer_n_idx(bytes, skip)?
     } else {
         0
     };
 
     for i in 0..take {
-        match rust_only::extract_packet(&bytes[last_trailer_idx..]) {
+        match rust_only::extract_packet_from_buf(&bytes[last_trailer_idx..], prepend_buffer.take())
+        {
             Ok((moss_packet, trailer_idx)) => {
                 moss_packets.push(moss_packet);
                 last_trailer_idx += trailer_idx + 1;
             }
             Err(e) if e.kind() == ParseErrorKind::EndOfBufferNoTrailer => {
                 return Err(PyBytesWarning::new_err(format!(
                     "Failed decoding packet #{packet_cnt}: {e}",
@@ -206,32 +225,41 @@
     if moss_packets.is_empty() {
         Err(PyAssertionError::new_err("No MOSS Packets in events"))
     } else {
         Ok((moss_packets, last_trailer_idx - 1))
     }
 }
 
+#[allow(non_camel_case_types)]
+type Remainder_Bytes = Vec<u8>;
+
+/// Skips N events in the given bytes and decode as many packets as possible until end of buffer,
+/// If any packets are decoded, they are returned as a list of MOSS Packets.
+/// if the end of the buffer contains a partial event, those bytes are returned as a remainder.
+///
+/// Arguments: bytes: `bytes`, skip: `int`
+///
+/// Returns: `Tuple[Optional[List[MossPacket]], Optional[bytes]]`
 #[pyfunction]
-/// Skips N events in the given bytes and decode as many packets as possible until end of buffer, if the end of the buffer contains a partial event, those bytes are returned as a remainder.
-pub fn decode_events_skip_n_take_all_with_remainder(
+pub fn skip_n_take_all(
     bytes: &[u8],
     skip: usize,
-) -> PyResult<(Vec<MossPacket>, Option<Vec<u8>>)> {
+) -> PyResult<(Option<List_MossPackets>, Option<Remainder_Bytes>)> {
     let mut moss_packets: Vec<MossPacket> = Vec::new();
     let mut remainder: Option<Vec<u8>> = None;
 
     // Skip N events
     let mut last_trailer_idx = if skip > 0 {
         find_trailer_n_idx(bytes, skip)?
     } else {
         0
     };
 
     while last_trailer_idx < bytes.len() - MINIMUM_EVENT_SIZE - 1 {
-        match rust_only::extract_packet(&bytes[last_trailer_idx..]) {
+        match rust_only::extract_packet_from_buf(&bytes[last_trailer_idx..], None) {
             Ok((moss_packet, trailer_idx)) => {
                 moss_packets.push(moss_packet);
                 last_trailer_idx += trailer_idx + 1;
             }
             Err(e) if e.kind() == ParseErrorKind::EndOfBufferNoTrailer => {
                 remainder = Some(bytes[last_trailer_idx..].to_vec());
                 break;
@@ -242,37 +270,37 @@
                     packet_cnt = moss_packets.len() + 1
                 )))
             }
         }
     }
 
     if moss_packets.is_empty() {
-        Err(PyAssertionError::new_err("No MOSS Packets in events"))
+        Ok((None, remainder))
     } else {
-        Ok((moss_packets, remainder))
+        Ok((Some(moss_packets), remainder))
     }
 }
 
 mod rust_only {
     use pyo3::exceptions::PyValueError;
     use pyo3::PyResult;
 
     use crate::decode_hits_fsm::extract_hits;
     use crate::moss_protocol::MossWord;
     use crate::parse_error::{ParseError, ParseErrorKind};
-    use crate::MossPacket;
+    use crate::{MossPacket, Tuple_MossPacket_LastTrailerIdx};
 
     /// Functions that are only used in Rust and not exposed to Python.
 
     const MIN_PREALLOC: usize = 10;
     #[inline]
     pub(super) fn calc_prealloc_val(bytes: &[u8]) -> PyResult<usize> {
         let byte_cnt = bytes.len();
 
-        if byte_cnt < 6 {
+        if byte_cnt < crate::MINIMUM_EVENT_SIZE {
             return Err(PyValueError::new_err(
                 "Received less than the minimum event size",
             ));
         }
 
         let prealloc = if byte_cnt / 1024 > MIN_PREALLOC {
             byte_cnt / 1024
@@ -281,15 +309,15 @@
         };
         Ok(prealloc)
     }
 
     /// Advances the iterator until a Unit Frame Header is encountered, saves the unit ID,
     /// and extracts the hits with the [extract_hits] function, before returning a MossPacket if one is found.
     #[inline]
-    pub(crate) fn extract_packet(bytes: &[u8]) -> Result<(MossPacket, usize), ParseError> {
+    fn extract_packet(bytes: &[u8]) -> Result<Tuple_MossPacket_LastTrailerIdx, ParseError> {
         if let Some(header_idx) = bytes
             .iter()
             .position(|b| MossWord::UNIT_FRAME_HEADER_RANGE.contains(b))
         {
             let mut bytes_iter = bytes.iter().skip(header_idx + 1);
             match extract_hits(&mut bytes_iter) {
                 Ok(hits) => Ok((
@@ -310,14 +338,36 @@
                 ParseErrorKind::NoHeaderFound,
                 "No Unit Frame Header found",
                 0,
             ))
         }
     }
 
+    #[inline]
+    /// If a prepend buffer is given, it is prepended to `bytes` and the packet is extracted from the combined buffer.
+    /// If no prepend buffer is given, the packet is extracted from `bytes`.
+    pub(crate) fn extract_packet_from_buf(
+        bytes: &[u8],
+        prepend_bytes: Option<Vec<u8>>,
+    ) -> Result<Tuple_MossPacket_LastTrailerIdx, ParseError> {
+        // Collect bytes from `bytes` until a header is seen
+
+        if let Some(mut prepend) = prepend_bytes {
+            prepend.extend(
+                bytes
+                    .iter()
+                    .take_while(|b| **b != MossWord::UNIT_FRAME_TRAILER),
+            );
+            prepend.push(MossWord::UNIT_FRAME_TRAILER); // Add the trailer back since `take_while` is EXCLUSIVE
+            extract_packet(&prepend)
+        } else {
+            extract_packet(bytes)
+        }
+    }
+
     /// Formats an error message with an error description and the byte that triggered the error.
     ///
     /// Also includes a dump of the bytes from the header and 10 bytes past the error.
     fn format_error_msg(err_str: &str, err_idx: usize, bytes: &[u8]) -> String {
         format!(
         "{err_str}, got: 0x{error_byte:02X}. Dump from header and 10 bytes past error: {prev} [ERROR = {error_byte:02X}] {next}",
         prev = bytes
```

### Comparing `moss_decoder-0.5.3/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.7.0/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.7.0/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/src/moss_protocol/test_util.rs` & `moss_decoder-0.7.0/src/moss_protocol/test_util.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/src/moss_protocol.rs` & `moss_decoder-0.7.0/src/moss_protocol.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/src/parse_error.rs` & `moss_decoder-0.7.0/src/parse_error.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/src/parse_util.rs` & `moss_decoder-0.7.0/src/parse_util.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/tests/integration_test.rs` & `moss_decoder-0.7.0/tests/integration_test.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 use crate::moss_protocol::test_util::*;
 use moss_decoder::*;
 
 use pretty_assertions::assert_eq;
 
+const FILE_MOSS_NOISE: &str = "tests/test-data/moss_noise.raw";
+const FILE_4_EVENTS_PARTIAL_END: &str = "tests/test-data/moss_noise_0-499b.raw"; // 4 events, last event is partial ~4.5 events
+const FILE_3_EVENTS_PARTIAL_START: &str = "tests/test-data/moss_noise_500-999b.raw"; // 3 events, first event is partial ~3.5 events
+const FILE_MOSS_NOISE_ALL_REGION: &str = "tests/test-data/noise_all_regions.raw";
+const FILE_NOISE_RANDOM_REGION: &str = "tests/test-data/noise_random_region.raw";
+const FILE_PATTERN_ALL_REGIONS: &str = "tests/test-data/pattern_all_regions.raw";
+
 #[test]
 fn test_decoding_single_event() {
     //
     let event = fake_event_simple();
 
     let (packet, last_trailer_idx) = decode_event(&event).unwrap();
 
@@ -110,23 +117,23 @@
 }
 
 #[test]
 fn test_read_file_decode() {
     let time = std::time::Instant::now();
 
     println!("Reading file...");
-    let f = std::fs::read(std::path::PathBuf::from("tests/moss_noise.raw")).unwrap();
+    let f = std::fs::read(std::path::PathBuf::from(FILE_MOSS_NOISE)).unwrap();
     println!(
         "Read file in: {t:?}. Bytes: {cnt}",
         t = time.elapsed(),
         cnt = f.len()
     );
 
     println!("Decoding content...");
-    let (p, last_trailer_idx) = decode_multiple_events(&f).unwrap();
+    let (p, last_trailer_idx) = decode_all_events(&f).unwrap();
     println!("Decoded in: {t:?}\n", t = time.elapsed());
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
 
     assert_eq!(
         last_trailer_idx,
@@ -140,16 +147,15 @@
 
 #[test]
 fn test_decode_from_file() {
     let time = std::time::Instant::now();
     let expect_packets = 100000;
     let expect_hits = 2716940;
 
-    let packets =
-        moss_decoder::decode_from_file("tests/moss_noise.raw".to_string().into()).unwrap();
+    let packets = moss_decoder::decode_from_file(FILE_MOSS_NOISE.to_string().into()).unwrap();
     println!("Decoded in: {t:?}\n", t = time.elapsed());
 
     println!("Got: {packets}", packets = packets.len());
 
     assert_eq!(
         packets.len(),
         expect_packets,
@@ -162,14 +168,77 @@
     assert_eq!(
         total_hits, expect_hits,
         "Expected {expect_hits} hits, got {total_hits}",
     );
 }
 
 #[test]
+fn test_decode_from_file_noise_all_region() {
+    let expect_packets = 1000;
+    let expect_hits = 6085;
+
+    let packets =
+        moss_decoder::decode_from_file(FILE_MOSS_NOISE_ALL_REGION.to_string().into()).unwrap();
+    assert_eq!(
+        packets.len(),
+        expect_packets,
+        "Expected {expect_packets} packets, got {}",
+        packets.len()
+    );
+    // Count total hits
+    let total_hits = packets.iter().fold(0, |acc, p| acc + p.hits.len());
+    assert_eq!(
+        total_hits, expect_hits,
+        "Expected {expect_hits} hits, got {total_hits}",
+    );
+}
+
+#[test]
+fn test_decode_from_file_noise_random_region() {
+    let expect_packets = 1044;
+    let expect_hits = 5380;
+
+    let packets =
+        moss_decoder::decode_from_file(FILE_NOISE_RANDOM_REGION.to_string().into()).unwrap();
+    assert_eq!(
+        packets.len(),
+        expect_packets,
+        "Expected {expect_packets} packets, got {}",
+        packets.len()
+    );
+    // Count total hits
+    let total_hits = packets.iter().fold(0, |acc, p| acc + p.hits.len());
+    assert_eq!(
+        total_hits, expect_hits,
+        "Expected {expect_hits} hits, got {total_hits}",
+    );
+}
+
+#[test]
+fn test_decode_from_file_pattern_all_region() {
+    let expect_packets = 1000;
+    let expect_hits = 4000;
+
+    let packets =
+        moss_decoder::decode_from_file(FILE_PATTERN_ALL_REGIONS.to_string().into()).unwrap();
+    assert_eq!(
+        packets.len(),
+        expect_packets,
+        "Expected {expect_packets} packets, got {}",
+        packets.len()
+    );
+    // Count total hits
+    let total_hits = packets.iter().fold(0, |acc, p| acc + p.hits.len());
+    assert_eq!(
+        total_hits, expect_hits,
+        "Expected {expect_hits} hits, got {total_hits}",
+    );
+}
+
+#[test]
 fn test_decode_protocol_error() {
     pyo3::prepare_freethreaded_python();
 
     let event = fake_event_protocol_error();
 
     match decode_event(&event) {
         Ok(_) => {
@@ -188,23 +257,23 @@
 fn test_decode_multiple_events_fsm() {
     let expect_packets = 100000;
     let expect_hits = 2716940;
 
     println!("Reading file...");
     let time = std::time::Instant::now();
 
-    let f = std::fs::read(std::path::PathBuf::from("tests/moss_noise.raw")).unwrap();
+    let f = std::fs::read(std::path::PathBuf::from(FILE_MOSS_NOISE)).unwrap();
     println!(
         "Read file in: {t:?}. Bytes: {cnt}",
         t = time.elapsed(),
         cnt = f.len()
     );
 
     println!("Decoding content...");
-    let (p, last_trailer_idx) = decode_multiple_events(&f).unwrap();
+    let (p, last_trailer_idx) = decode_all_events(&f).unwrap();
     println!("Decoded in: {t:?}\n", t = time.elapsed());
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     println!("Last 10 bytes of file: {:X?}", f.get(f.len() - 10..));
 
     assert_eq!(
@@ -229,16 +298,15 @@
 
 #[test]
 fn test_decode_from_file_fsm() {
     let time = std::time::Instant::now();
     let expect_packets = 100000;
     let expect_hits = 2716940;
 
-    let packets =
-        moss_decoder::decode_from_file("tests/moss_noise.raw".to_string().into()).unwrap();
+    let packets = moss_decoder::decode_from_file(FILE_MOSS_NOISE.to_string().into()).unwrap();
     println!("Decoded in: {t:?}\n", t = time.elapsed());
 
     println!("Got: {packets}", packets = packets.len());
 
     assert_eq!(
         packets.len(),
         expect_packets,
@@ -272,115 +340,138 @@
         }
     }
 }
 
 #[test]
 fn test_decode_events_skip_0_take_10() {
     let take = 10;
-    let f = std::fs::read(std::path::PathBuf::from("tests/moss_noise.raw")).unwrap();
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, None).unwrap();
+    let f = std::fs::read(std::path::PathBuf::from(FILE_MOSS_NOISE)).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, None, None).unwrap();
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_events_skip_10_take_1() {
     let skip = 10;
     let take = 1;
-    let f = std::fs::read(std::path::PathBuf::from("tests/moss_noise.raw")).unwrap();
+    let f = std::fs::read(std::path::PathBuf::from(FILE_MOSS_NOISE)).unwrap();
 
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, Some(skip)).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, Some(skip), None).unwrap();
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_events_skip_500_take_100() {
     let skip = 500;
     let take = 100;
-    let f = std::fs::read(std::path::PathBuf::from("tests/moss_noise.raw")).unwrap();
+    let f = std::fs::read(std::path::PathBuf::from(FILE_MOSS_NOISE)).unwrap();
 
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, Some(skip)).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, Some(skip), None).unwrap();
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_events_skip_99000_take_1000() {
     let skip = 99000;
     let take = 1000;
-    let f = std::fs::read(std::path::PathBuf::from("tests/moss_noise.raw")).unwrap();
+    let f = std::fs::read(std::path::PathBuf::from(FILE_MOSS_NOISE)).unwrap();
 
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, Some(skip)).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, Some(skip), None).unwrap();
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
-const FILE_4_EVENTS_PARTIAL_END: &str = "tests/moss_noise_0-499b.raw";
-const FILE_3_EVENTS_PARTIAL_START: &str = "tests/moss_noise_500-999b.raw";
-
 #[test]
 #[should_panic = "Failed decoding packet #5"]
 fn test_decode_split_events_skip_0_take_5() {
     pyo3::prepare_freethreaded_python();
     let take = 5;
     let f = std::fs::read(std::path::PathBuf::from(FILE_4_EVENTS_PARTIAL_END)).unwrap();
 
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, None).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, None, None).unwrap();
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_split_events_skip_1_take_2() {
     pyo3::prepare_freethreaded_python();
     let skip = 1;
     let take = 2;
     let f = std::fs::read(std::path::PathBuf::from(FILE_4_EVENTS_PARTIAL_END)).unwrap();
 
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, Some(skip)).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, Some(skip), None).unwrap();
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_split_events_from_partial_event_skip_1_take_2() {
     pyo3::prepare_freethreaded_python();
     let skip = 1;
     let take = 2;
     let f = std::fs::read(std::path::PathBuf::from(FILE_3_EVENTS_PARTIAL_START)).unwrap();
 
-    let (p, last_trailer_idx) = decode_events_take_n(&f, take, Some(skip)).unwrap();
+    let (p, last_trailer_idx) = decode_n_events(&f, take, Some(skip), None).unwrap();
 
     println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
     assert_eq!(p.len(), take, "Expected {take} packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_split_events_with_remainder() {
     pyo3::prepare_freethreaded_python();
     let take = 100;
     let f = std::fs::read(std::path::PathBuf::from(FILE_4_EVENTS_PARTIAL_END)).unwrap();
 
-    assert!(decode_events_take_n(&f, take, None).is_err());
+    assert!(decode_n_events(&f, take, None, None).is_err());
 
-    let (packets, remainder) = decode_events_skip_n_take_all_with_remainder(&f, 0).unwrap();
+    let (packets, remainder) = skip_n_take_all(&f, 0).unwrap();
 
     let remainder = remainder.unwrap();
+    let packets = packets.unwrap();
 
     println!("Got: {packets} packets", packets = packets.len());
     println!("Remainder: {remainder} bytes", remainder = remainder.len());
     assert_eq!(packets.len(), 4);
     assert_eq!(remainder.len(), 43);
 }
+
+#[test]
+fn test_decode_split_events_from_both_files() {
+    pyo3::prepare_freethreaded_python();
+    let take = 6;
+    let f = std::fs::read(std::path::PathBuf::from(FILE_4_EVENTS_PARTIAL_END)).unwrap();
+    let f2 = std::fs::read(std::path::PathBuf::from(FILE_3_EVENTS_PARTIAL_START)).unwrap();
+
+    // First attempt to decode 6 events from the first file, that should fail
+    assert!(decode_n_events(&f, take, None, None).is_err());
+
+    // Then fall back to decoding as many as possible and returning the remainder
+    let (packets, remainder) = skip_n_take_all(&f, 0).unwrap();
+    let packets = packets.unwrap();
+    let decoded_packets = packets.len();
+
+    // Now take the rest from the remainder and the next file
+    let (packets2, last_trailer_idx) =
+        decode_n_events(&f2, take - decoded_packets, None, remainder).unwrap();
+
+    println!("Got: {packets} packets", packets = packets.len());
+    println!("Got: {packets2} packets", packets2 = packets2.len());
+    println!("Last trailer at index: {last_trailer_idx}");
+    assert_eq!(packets.len() + packets2.len(), take);
+}
```

### Comparing `moss_decoder-0.5.3/tests/moss_noise.raw` & `moss_decoder-0.7.0/tests/test-data/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/tests/performance_dev_py.sh` & `moss_decoder-0.7.0/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/tests/performance_prod_py.sh` & `moss_decoder-0.7.0/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/tests/utils.sh` & `moss_decoder-0.7.0/tests/utils.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.5.3/Cargo.lock` & `moss_decoder-0.7.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.5.3"
+version = "0.7.0"
 dependencies = [
  "criterion",
  "pretty_assertions",
  "pyo3",
  "sm",
 ]
```

### Comparing `moss_decoder-0.5.3/PKG-INFO` & `moss_decoder-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.5.3
+Version: 0.7.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
@@ -25,15 +25,15 @@
 
 Python package implemented in Rust for high-performance decoding of readout data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
 
 - [MOSS Decoder](#moss-decoder)
   - [Installation](#installation)
     - [Example](#example)
   - [Features](#features)
-    - [3 types of functions are provided](#3-types-of-functions-are-provided)
+    - [5 types of idempotent functions are provided](#5-types-of-idempotent-functions-are-provided)
   - [MOSS event data packet protocol FSM](#moss-event-data-packet-protocol-fsm)
   - [MOSS event data packet decoder FSM](#moss-event-data-packet-decoder-fsm)
   - [Event packet hit decoder FSM](#event-packet-hit-decoder-fsm)
   - [Motivation \& Purpose](#motivation--purpose)
   - [@CERN Gitlab installation for CentOS and similar distributions from local build](#cern-gitlab-installation-for-centos-and-similar-distributions-from-local-build)
     - [Troubleshooting](#troubleshooting)
 
@@ -55,35 +55,61 @@
 ```
 
 ## Features
 See [python types](moss_decoder.pyi) for the type information the package exposes to Python.
 
 Two classes are provided: `MossPacket` & `MossHit`.
 
-### 3 types of functions are provided
+### 5 types of idempotent functions are provided
 ```python
 decode_event(arg: bytes)  -> tuple[MossPacket, int]: ...
 # allows decoding a single event from an iterable of bytes
 ```
 
 **Returns**: the decoded `MossPacket` and the index the *unit frame trailer* was found. Throws if no valid `MossPacket` is found.
 ```python
-decode_multiple_events(arg: bytes) -> tuple[list[MossPacket], int]: ...
+decode_all_events(arg: bytes) -> tuple[list[MossPacket], int]: ...
 # returns as many `MossPacket`s as can be decoded from the bytes iterable.
 # This is much more effecient than calling `decode_event` multiple times.
 ```
-**Returns**: A list of `MossPacket`s and the index of the last observed *unit frame trailer*. Throws if no valid `MossPacket`s are found.
+**Returns**: A list of `MossPacket`s and the index of the last observed *unit frame trailer*. Throws if no valid `MossPacket`s are found or a protocol error is encountered.
 
 ```python
 decode_from_file(arg: str | Path) -> list[MossPacket]: ...
 # takes a `Path` and returns as many `MossPacket` as can be decoded from file.
 # This is the most effecient way of decoding data from a file.
 ```
-**Returns**: A list of `MossPacket`s. Throws if the file is not found or no valid `MossPacket`s are found.
+**Returns**: A list of `MossPacket`s. Throws if the file is not found, no valid `MossPacket`s are found, or a protocol error is encountered.
 
+```python
+decode_n_events(
+    bytes: bytes,
+    take: int,
+    skip: Optional[int] = None,
+    prepend_buffer: Optional[bytes] = None,
+) -> tuple[list[MossPacket], int]: ...
+# Decode N events from bytes
+# Optionally provide either (not both):
+#    - Skip M events before decoding N events
+#    - Prepend a buffer before decoding N events.
+```
+**Returns**: A list of `MossPacket`s. Throws if the file is not found, no valid `MossPacket`s are found, or a protocol error is encountered.
+
+A `BytesWarning` exception is thrown if the end of the `bytes` is reached while decoding a packet (no trailer is found)
+
+```python
+def skip_n_take_all(
+    bytes: bytes, skip: int = None
+) -> tuple[list[MossPacket], Optional[bytes]]: ...
+# Decode all events, optionally skip N events first.
+# return all decoded events and the remaining bytes after decoding the last MossPacket
+```
+**Returns**: All decoded events and any remaining bytes after the last trailer seen.
+
+Using `decode_n_events` and `skip_n_take_all` it is possible to continuously decode multiple files that potentially ends or starts with partial events.
 
 ## MOSS event data packet protocol FSM
 The a MOSS half-unit event data packet follows the states seen in the FSM below. The region header state is simplified here.
 ```mermaid
 stateDiagram-v2
   frame_header : Unit Frame Header
   frame_trailer : Unit Frame Trailer
@@ -92,14 +118,15 @@
   data_1 : Data 1
   data_2 : Data 2
   idle : Idle
 
     [*] --> frame_header
 
     frame_header --> region_header
+    frame_header --> frame_trailer
 
     region_header --> region_header
     region_header --> frame_trailer
     region_header --> DATA
 
     state DATA {
       direction LR
@@ -112,14 +139,15 @@
 
     DATA --> idle
     DATA --> region_header
     DATA --> frame_trailer
 
 
     idle --> DATA
+    idle --> idle
     idle --> frame_trailer
 
     frame_trailer --> [*]
 
 ```
 
 ## MOSS event data packet decoder FSM
@@ -139,14 +167,15 @@
   delimiter --> delimiter
 
   state EVENT {
 
     [*] --> frame_header
 
     frame_header --> HITS
+    frame_header --> frame_trailer
 
     state HITS {
       [*] --> [*] : decode hits
     }
 
     HITS --> frame_trailer
```

