# Comparing `tmp/markmini-0.1.0.tar.gz` & `tmp/markmini-0.2.0.tar.gz`

## Comparing `markmini-0.1.0.tar` & `markmini-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 markmini-0.1.0/local_dependencies/markmini/Cargo.toml
--rw-r--r--   0        0        0     4141 2023-07-28 09:07:37.000000 markmini-0.1.0/local_dependencies/markmini/src/lib.rs
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 markmini-0.1.0/Cargo.toml
--rw-r--r--   0        0        0      465 2023-07-28 09:37:39.000000 markmini-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-20 12:23:32.000000 markmini-0.1.0/__init__.py
--rw-r--r--   0        0        0       26 2023-06-20 11:30:09.000000 markmini-0.1.0/devreq.txt
--rw-r--r--   0        0        0        0 2023-06-20 12:46:10.000000 markmini-0.1.0/devserver/__init__.py
--rw-r--r--   0        0        0     1017 2023-07-03 08:18:12.000000 markmini-0.1.0/devserver/main.py
--rw-r--r--   0        0        0    15406 2023-06-20 12:17:13.000000 markmini-0.1.0/devserver/static/favicon.ico
--rw-r--r--   0        0        0      508 2023-06-20 13:07:12.000000 markmini-0.1.0/devserver/static/main.js
--rw-r--r--   0        0        0      320 2023-06-20 13:13:01.000000 markmini-0.1.0/devserver/static/styles.css
--rw-r--r--   0        0        0      543 2023-06-20 13:10:39.000000 markmini-0.1.0/devserver/templates/index.html
--rw-r--r--   0        0        0      275 2023-07-03 08:19:31.000000 markmini-0.1.0/markmini.pyi
--rw-r--r--   0        0        0      328 2023-07-28 09:34:19.000000 markmini-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      164 2023-06-20 12:46:45.000000 markmini-0.1.0/rundev.py
--rw-r--r--   0        0        0     1117 2023-07-03 08:41:44.000000 markmini-0.1.0/src/lib.rs
--rw-r--r--   0        0        0    19952 2023-07-04 07:05:20.000000 markmini-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 markmini-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 markmini-0.2.0/local_dependencies/markmini/Cargo.toml
+-rw-r--r--   0     1001      123     9370 2023-08-02 15:41:18.000000 markmini-0.2.0/local_dependencies/markmini/src/lib.rs
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 markmini-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      434 2023-08-02 15:41:18.000000 markmini-0.2.0/README.md
+-rw-r--r--   0     1001      123        0 2023-08-02 15:41:18.000000 markmini-0.2.0/__init__.py
+-rw-r--r--   0     1001      123       23 2023-08-02 15:41:18.000000 markmini-0.2.0/devreq.txt
+-rw-r--r--   0     1001      123        0 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/__init__.py
+-rw-r--r--   0     1001      123      979 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/main.py
+-rw-r--r--   0     1001      123    15406 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/static/favicon.ico
+-rw-r--r--   0     1001      123      493 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/static/main.js
+-rw-r--r--   0     1001      123      298 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/static/styles.css
+-rw-r--r--   0     1001      123      521 2023-08-02 15:41:18.000000 markmini-0.2.0/devserver/templates/index.html
+-rw-r--r--   0     1001      123      265 2023-08-02 15:41:18.000000 markmini-0.2.0/markmini.pyi
+-rw-r--r--   0     1001      123      316 2023-08-02 15:41:18.000000 markmini-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      159 2023-08-02 15:41:18.000000 markmini-0.2.0/rundev.py
+-rw-r--r--   0     1001      123     1120 2023-08-02 15:41:18.000000 markmini-0.2.0/src/lib.rs
+-rw-r--r--   0        0        0    19244 2023-08-02 15:42:06.000000 markmini-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 markmini-0.2.0/PKG-INFO
```

### Comparing `markmini-0.1.0/devserver/main.py` & `markmini-0.2.0/devserver/main.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from fastapi import FastAPI, Request
-from fastapi.responses import HTMLResponse
-from fastapi.staticfiles import StaticFiles
-from fastapi.templating import Jinja2Templates
-from pydantic import BaseModel
-
-import markmini
-
-app = FastAPI()
-
-app.mount("/static", StaticFiles(directory="devserver/static"), name="static")
-
-templates = Jinja2Templates(directory="devserver/templates")
-
-md = markmini.Markmini()
-
-usernames = ["iverks", "testy"]
-user_ids = ["1", "2"]
-links = [f"/users/{id}" for id in user_ids]
-fullnames = ["Iver Småge", "Testy McTestFace"]
-
-md.add_users(usernames, user_ids, links, fullnames)
-
-
-@app.get("/", response_class=HTMLResponse)
-def rootpage(request: Request):
-    return templates.TemplateResponse("index.html", {"request": request})
-
-
-class Data(BaseModel):
-    input: str
-
-
-# Note: We only expose this function for testing
-# In production we would only do this on submit
-@app.post("/mdcompile")
-def read_item(data: Data):
-    return md.compile(data.input)
+from fastapi import FastAPI, Request
+from fastapi.responses import HTMLResponse
+from fastapi.staticfiles import StaticFiles
+from fastapi.templating import Jinja2Templates
+from pydantic import BaseModel
+
+import markmini
+
+app = FastAPI()
+
+app.mount("/static", StaticFiles(directory="devserver/static"), name="static")
+
+templates = Jinja2Templates(directory="devserver/templates")
+
+md = markmini.Markmini()
+
+usernames = ["iverks", "testy"]
+user_ids = ["1", "2"]
+links = [f"/users/{id}" for id in user_ids]
+fullnames = ["Iver Småge", "Testy McTestFace"]
+
+md.add_users(usernames, user_ids, links, fullnames)
+
+
+@app.get("/", response_class=HTMLResponse)
+def rootpage(request: Request):
+    return templates.TemplateResponse("index.html", {"request": request})
+
+
+class Data(BaseModel):
+    input: str
+
+
+# Note: We only expose this function for testing
+# In production we would only do this on submit
+@app.post("/mdcompile")
+def read_item(data: Data):
+    return md.compile(data.input)
```

### Comparing `markmini-0.1.0/devserver/static/favicon.ico` & `markmini-0.2.0/devserver/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `markmini-0.1.0/src/lib.rs` & `markmini-0.2.0/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -39,11 +39,11 @@
         }
         self.internal.add_users(users);
     }
 }
 
 // This function is the entrypoint to the python module
 #[pymodule]
-fn markmini(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+fn markmini_py(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<Markmini>()?;
     Ok(())
 }
```

### Comparing `markmini-0.1.0/Cargo.lock` & `markmini-0.2.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "form_urlencoded"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
@@ -136,17 +136,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -175,17 +175,34 @@
 [[package]]
 name = "markmini"
 version = "0.1.0"
 dependencies = [
  "aho-corasick",
  "ammonia",
  "lazy_static",
- "nom",
  "pulldown-cmark",
- "regex",
+ "regex-lite",
+]
+
+[[package]]
+name = "markmini-py"
+version = "0.2.0"
+dependencies = [
+ "itertools",
+ "markmini",
+ "pyo3",
+]
+
+[[package]]
+name = "markmini-wasm"
+version = "0.2.0"
+dependencies = [
+ "js-sys",
+ "markmini",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "markup5ever"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a2629bb1404f3d34c2e921f21fd34ba00b206124c81f65c50b43b6aaefeb016"
@@ -210,36 +227,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "minimal-lexical"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
-
-[[package]]
 name = "new_debug_unreachable"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
 
 [[package]]
-name = "nom"
-version = "7.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
-dependencies = [
- "memchr",
- "minimal-lexical",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
@@ -318,17 +319,17 @@
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulldown-cmark"
 version = "0.9.3"
@@ -338,86 +339,77 @@
  "bitflags",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
-name = "pyo3-bindings"
-version = "0.1.0"
-dependencies = [
- "itertools",
- "markmini",
- "pyo3",
-]
-
-[[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -454,53 +446,42 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "regex"
-version = "1.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-syntax",
-]
-
-[[package]]
-name = "regex-syntax"
-version = "0.7.2"
+name = "regex-lite"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "f96ede7f386ba6e910092e7ccdc04176cface62abebea07ed6b46d870ed95ca2"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.180"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "0ea67f183f058fe88a4e3ec6e2788e003840893b91bac4559cabedd00863b3ed"
 
 [[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "string_cache"
 version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91138e76242f575eb1d3b38b4f1362f10d3a43f47d182a5b359af488a02293b"
 dependencies = [
@@ -533,28 +514,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "04361975b3f5e348b2189d8dc55bc942f278b2d482a6a0365de5bdd62d351567"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "tendril"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d24a120c5fc464a3458240ee02c299ebcb9d67b5249c8848b09d639dca8d7bb0"
 dependencies = [
@@ -591,17 +572,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -660,15 +641,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.28",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -682,40 +663,30 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.28",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
-name = "wasm-bindings"
-version = "0.1.0"
-dependencies = [
- "itertools",
- "js-sys",
- "markmini",
- "wasm-bindgen",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

