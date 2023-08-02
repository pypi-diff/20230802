# Comparing `tmp/mkdocs-autorefs-0.4.1.tar.gz` & `tmp/mkdocs_autorefs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-autorefs-0.4.1.tar", last modified: Mon Mar  7 16:43:45 2022, max compression
+gzip compressed data, was "mkdocs_autorefs-0.5.0.tar", last modified: Wed Aug  2 19:40:45 2023, max compression
```

## Comparing `mkdocs-autorefs-0.4.1.tar` & `mkdocs_autorefs-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0 pawamoy   (1000) users      (985)      786 2022-02-05 13:58:12.404956 mkdocs-autorefs-0.4.1/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (985)     2970 2022-03-07 16:36:29.939083 mkdocs-autorefs-0.4.1/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)     3176 2022-03-07 16:36:29.939083 mkdocs-autorefs-0.4.1/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)       76 2022-03-07 16:36:29.939083 mkdocs-autorefs-0.4.1/src/mkdocs_autorefs/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     8784 2022-03-07 12:30:49.043671 mkdocs-autorefs-0.4.1/src/mkdocs_autorefs/plugin.py
--rw-r--r--   0 pawamoy   (1000) users      (985)        0 2022-02-05 17:57:23.686678 mkdocs-autorefs-0.4.1/src/mkdocs_autorefs/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (985)     7802 2022-03-07 12:30:49.060337 mkdocs-autorefs-0.4.1/src/mkdocs_autorefs/references.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       37 2021-02-17 19:48:51.503463 mkdocs-autorefs-0.4.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0 pawamoy   (1000) users      (985)      194 2021-02-17 19:48:51.503463 mkdocs-autorefs-0.4.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 pawamoy   (1000) users      (985)      295 2021-02-17 19:48:51.503463 mkdocs-autorefs-0.4.1/tests/.pytest_cache/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2021-11-29 23:24:54.080180 mkdocs-autorefs-0.4.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2021-12-27 22:14:23.988055 mkdocs-autorefs-0.4.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2021-12-27 22:14:23.988055 mkdocs-autorefs-0.4.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 pawamoy   (1000) users      (985)       10 2021-12-27 22:14:23.601393 mkdocs-autorefs-0.4.1/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0 pawamoy   (1000) users      (985)       47 2022-02-05 13:58:12.218294 mkdocs-autorefs-0.4.1/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2516 2022-03-07 12:30:49.070337 mkdocs-autorefs-0.4.1/tests/test_plugin.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     7584 2022-03-07 12:30:49.083671 mkdocs-autorefs-0.4.1/tests/test_references.py
--rw-------   0 pawamoy   (1000) users      (985)     5117 2022-03-07 16:43:45.679244 mkdocs-autorefs-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-08-02 18:24:39.295849 mkdocs_autorefs-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2407 2023-08-02 19:37:00.424420 mkdocs_autorefs-0.5.0/README.md
+-rw-r--r--   0        0        0     2810 2023-08-02 19:40:45.807001 mkdocs_autorefs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-08-02 18:24:36.755869 mkdocs_autorefs-0.5.0/src/mkdocs_autorefs/__init__.py
+-rw-r--r--   0        0        0     8703 2023-08-02 19:33:32.435113 mkdocs_autorefs-0.5.0/src/mkdocs_autorefs/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:24:36.752536 mkdocs_autorefs-0.5.0/src/mkdocs_autorefs/py.typed
+-rw-r--r--   0        0        0     7786 2023-08-02 18:23:04.336603 mkdocs_autorefs-0.5.0/src/mkdocs_autorefs/references.py
+-rw-r--r--   0        0        0       37 2021-02-17 19:48:51.503463 mkdocs_autorefs-0.5.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2021-02-17 19:48:51.503463 mkdocs_autorefs-0.5.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2021-02-17 19:48:51.503463 mkdocs_autorefs-0.5.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2021-11-29 23:24:54.080180 mkdocs_autorefs-0.5.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2021-12-27 22:14:23.988055 mkdocs_autorefs-0.5.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2021-12-27 22:14:23.988055 mkdocs_autorefs-0.5.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       10 2021-12-27 22:14:23.601393 mkdocs_autorefs-0.5.0/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0        0        0       45 2023-08-02 18:24:39.295849 mkdocs_autorefs-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-02 18:24:36.732536 mkdocs_autorefs-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     2585 2023-08-02 18:23:04.336603 mkdocs_autorefs-0.5.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     7740 2023-08-02 18:23:04.336603 mkdocs_autorefs-0.5.0/tests/test_references.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 mkdocs_autorefs-0.5.0/PKG-INFO
```

### Comparing `mkdocs-autorefs-0.4.1/LICENSE` & `mkdocs_autorefs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-autorefs-0.4.1/README.md` & `mkdocs_autorefs-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -41,146 +41,111 @@
 00000280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000290: 6f6d 2f6d 6b64 6f63 7374 7269 6e67 732f  om/mkdocstrings/
 000002a0: 6175 746f 7265 6673 290a 5b21 5b67 6974  autorefs).[![git
 000002b0: 7465 725d 2868 7474 7073 3a2f 2f62 6164  ter](https://bad
 000002c0: 6765 732e 6769 7474 6572 2e69 6d2f 6a6f  ges.gitter.im/jo
 000002d0: 696e 2532 3063 6861 742e 7376 6729 5d28  in%20chat.svg)](
 000002e0: 6874 7470 733a 2f2f 6769 7474 6572 2e69  https://gitter.i
-000002f0: 6d2f 6175 746f 7265 6673 2f63 6f6d 6d75  m/autorefs/commu
-00000300: 6e69 7479 290a 0a41 7574 6f6d 6174 6963  nity)..Automatic
-00000310: 616c 6c79 206c 696e 6b20 6163 726f 7373  ally link across
-00000320: 2070 6167 6573 2069 6e20 4d6b 446f 6373   pages in MkDocs
-00000330: 2e0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
-00000340: 6f6e 0a0a 5769 7468 2060 7069 7060 3a0a  on..With `pip`:.
-00000350: 6060 6062 6173 680a 7079 7468 6f6e 3320  ```bash.python3 
-00000360: 2d6d 2070 6970 2069 6e73 7461 6c6c 206d  -m pip install m
-00000370: 6b64 6f63 732d 6175 746f 7265 6673 0a60  kdocs-autorefs.`
-00000380: 6060 0a0a 2323 2055 7361 6765 0a0a 6060  ``..## Usage..``
-00000390: 6079 616d 6c0a 2320 6d6b 646f 6373 2e79  `yaml.# mkdocs.y
-000003a0: 6d6c 0a70 6c75 6769 6e73 3a0a 2020 2d20  ml.plugins:.  - 
-000003b0: 7365 6172 6368 0a20 202d 2061 7574 6f72  search.  - autor
-000003c0: 6566 730a 6060 600a 0a49 6e20 6f6e 6520  efs.```..In one 
-000003d0: 6f66 2079 6f75 7220 4d61 726b 646f 776e  of your Markdown
-000003e0: 2066 696c 6573 2028 652e 672e 2060 646f   files (e.g. `do
-000003f0: 6331 2e6d 6460 2920 6372 6561 7465 2073  c1.md`) create s
-00000400: 6f6d 6520 6865 6164 696e 6773 3a0a 0a60  ome headings:..`
-00000410: 6060 6d61 726b 646f 776e 0a23 2320 4865  ``markdown.## He
-00000420: 6c6c 6f2c 2077 6f72 6c64 210a 0a23 2320  llo, world!..## 
-00000430: 416e 6f74 6865 7220 6865 6164 696e 670a  Another heading.
-00000440: 0a4c 696e 6b20 746f 205b 4865 6c6c 6f2c  .Link to [Hello,
-00000450: 2057 6f72 6c64 215d 2823 6865 6c6c 6f2d   World!](#hello-
-00000460: 776f 726c 6429 206f 6e20 7468 6520 7361  world) on the sa
-00000470: 6d65 2070 6167 652e 0a60 6060 0a0a 5468  me page..```..Th
-00000480: 6973 2069 7320 6120 5b2a 6e6f 726d 616c  is is a [*normal
-00000490: 2a20 6c69 6e6b 2074 6f20 616e 2061 6e63  * link to an anc
-000004a0: 686f 725d 2868 7474 7073 3a2f 2f77 7777  hor](https://www
-000004b0: 2e6d 6b64 6f63 732e 6f72 672f 7573 6572  .mkdocs.org/user
-000004c0: 2d67 7569 6465 2f77 7269 7469 6e67 2d79  -guide/writing-y
-000004d0: 6f75 722d 646f 6373 2f23 6c69 6e6b 696e  our-docs/#linkin
-000004e0: 672d 746f 2d70 6167 6573 292e 204d 6b44  g-to-pages). MkD
-000004f0: 6f63 7320 6765 6e65 7261 7465 7320 616e  ocs generates an
-00000500: 6368 6f72 7320 666f 7220 6561 6368 2068  chors for each h
-00000510: 6561 6469 6e67 2c20 616e 6420 7468 6579  eading, and they
-00000520: 2063 616e 2061 6c77 6179 7320 6265 2075   can always be u
-00000530: 7365 6420 746f 206c 696e 6b20 746f 2073  sed to link to s
-00000540: 6f6d 6574 6869 6e67 2c20 6569 7468 6572  omething, either
-00000550: 2077 6974 6869 6e20 7468 6520 7361 6d65   within the same
-00000560: 2070 6167 6520 2861 7320 7368 6f77 6e20   page (as shown 
-00000570: 6865 7265 2920 6f72 2062 7920 7370 6563  here) or by spec
-00000580: 6966 7969 6e67 2074 6865 2070 6174 6820  ifying the path 
-00000590: 6f66 2074 6865 206f 7468 6572 2070 6167  of the other pag
-000005a0: 652e 0a0a 4275 7420 7769 7468 2074 6869  e...But with thi
-000005b0: 7320 706c 7567 696e 2c20 796f 7520 6361  s plugin, you ca
-000005c0: 6e20 2a2a 6c69 6e6b 2074 6f20 6120 6865  n **link to a he
-000005d0: 6164 696e 6720 6672 6f6d 2061 6e79 206f  ading from any o
-000005e0: 7468 6572 2070 6167 652a 2a20 6f6e 2074  ther page** on t
-000005f0: 6865 2073 6974 6520 2a77 6974 686f 7574  he site *without
-00000600: 2a20 6e65 6564 696e 6720 746f 206b 6e6f  * needing to kno
-00000610: 7720 7468 6520 7061 7468 206f 6620 6569  w the path of ei
-00000620: 7468 6572 206f 6620 7468 6520 7061 6765  ther of the page
-00000630: 732c 206a 7573 7420 7468 6520 6865 6164  s, just the head
-00000640: 696e 6720 7469 746c 6520 6974 7365 6c66  ing title itself
-00000650: 2e20 200a 4c65 7427 7320 6372 6561 7465  .  .Let's create
-00000660: 2061 6e6f 7468 6572 204d 6172 6b64 6f77   another Markdow
-00000670: 6e20 7061 6765 2074 6f20 7472 7920 7468  n page to try th
-00000680: 6973 2c20 6073 7562 6469 722f 646f 6332  is, `subdir/doc2
-00000690: 2e6d 6460 3a0a 0a60 6060 6d61 726b 646f  .md`:..```markdo
-000006a0: 776e 0a57 6520 6361 6e20 5b6c 696e 6b20  wn.We can [link 
-000006b0: 746f 2074 6861 7420 6865 6164 696e 675d  to that heading]
-000006c0: 5b68 656c 6c6f 2d77 6f72 6c64 5d20 6672  [hello-world] fr
-000006d0: 6f6d 2061 6e6f 7468 6572 2070 6167 6520  om another page 
-000006e0: 746f 6f2e 0a0a 5468 6973 2077 6f72 6b73  too...This works
-000006f0: 2074 6865 2073 616d 6520 6173 205b 6120   the same as [a 
-00000700: 6e6f 726d 616c 206c 696e 6b20 746f 2074  normal link to t
-00000710: 6861 7420 6865 6164 696e 675d 282e 2e2f  hat heading](../
-00000720: 646f 6331 2e6d 6423 6865 6c6c 6f2d 776f  doc1.md#hello-wo
-00000730: 726c 6429 2e0a 6060 600a 0a4c 696e 6b69  rld)..```..Linki
-00000740: 6e67 2074 6f20 6120 6865 6164 696e 6720  ng to a heading 
-00000750: 7769 7468 6f75 7420 6e65 6564 696e 6720  without needing 
-00000760: 746f 206b 6e6f 7720 7468 6520 6465 7374  to know the dest
-00000770: 696e 6174 696f 6e20 7061 6765 2063 616e  ination page can
-00000780: 2062 6520 7573 6566 756c 2069 6620 7370   be useful if sp
-00000790: 6563 6966 7969 6e67 2074 6861 7420 7061  ecifying that pa
-000007a0: 7468 2069 7320 6375 6d62 6572 736f 6d65  th is cumbersome
-000007b0: 2c20 652e 672e 2077 6865 6e20 7468 6520  , e.g. when the 
-000007c0: 7061 6765 7320 6861 7665 2064 6565 706c  pages have deepl
-000007d0: 7920 6e65 7374 6564 2070 6174 6873 2c20  y nested paths, 
-000007e0: 6172 6520 6661 7220 6170 6172 742c 206f  are far apart, o
-000007f0: 7220 6172 6520 6d6f 7665 6420 6172 6f75  r are moved arou
-00000800: 6e64 2066 7265 7175 656e 746c 792e 2041  nd frequently. A
-00000810: 6e64 2074 6865 2069 7373 7565 2069 7320  nd the issue is 
-00000820: 736f 6d65 7768 6174 2065 7861 6365 7262  somewhat exacerb
-00000830: 6174 6564 2062 7920 7468 6520 6661 6374  ated by the fact
-00000840: 2074 6861 7420 5b4d 6b44 6f63 7320 7375   that [MkDocs su
-00000850: 7070 6f72 7473 206f 6e6c 7920 2a72 656c  pports only *rel
-00000860: 6174 6976 652a 206c 696e 6b73 2062 6574  ative* links bet
-00000870: 7765 656e 2070 6167 6573 5d28 6874 7470  ween pages](http
-00000880: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000890: 6b64 6f63 732f 6d6b 646f 6373 2f69 7373  kdocs/mkdocs/iss
-000008a0: 7565 732f 3135 3932 292e 0a0a 4e6f 7465  ues/1592)...Note
-000008b0: 2074 6861 7420 7468 6973 2070 6c75 6769   that this plugi
-000008c0: 6e27 7320 6265 6861 7669 6f72 2069 7320  n's behavior is 
-000008d0: 756e 6465 6669 6e65 6420 7768 656e 2074  undefined when t
-000008e0: 7279 696e 6720 746f 206c 696e 6b20 746f  rying to link to
-000008f0: 2061 2068 6561 6469 6e67 2074 6974 6c65   a heading title
-00000900: 2074 6861 7420 6170 7065 6172 7320 7365   that appears se
-00000910: 7665 7261 6c20 7469 6d65 7320 7468 726f  veral times thro
-00000920: 7567 686f 7574 2074 6865 2073 6974 652e  ughout the site.
-00000930: 2043 7572 7265 6e74 6c79 2069 7420 6172   Currently it ar
-00000940: 6269 7472 6172 696c 7920 6368 6f6f 7365  bitrarily choose
-00000950: 7320 6f6e 6520 6f66 2074 6865 2070 6167  s one of the pag
-00000960: 6573 2e0a 0a23 2320 5265 7175 6972 656d  es...## Requirem
-00000970: 656e 7473 0a0a 6d6b 646f 6373 2d61 7574  ents..mkdocs-aut
-00000980: 6f72 6566 7320 7265 7175 6972 6573 2050  orefs requires P
-00000990: 7974 686f 6e20 332e 3720 6f72 2061 626f  ython 3.7 or abo
-000009a0: 7665 2e0a 0a3c 6465 7461 696c 733e 0a3c  ve...<details>.<
-000009b0: 7375 6d6d 6172 793e 546f 2069 6e73 7461  summary>To insta
-000009c0: 6c6c 2050 7974 686f 6e20 332e 372c 2049  ll Python 3.7, I
-000009d0: 2072 6563 6f6d 6d65 6e64 2075 7369 6e67   recommend using
-000009e0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000009f0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7965  //github.com/pye
-00000a00: 6e76 2f70 7965 6e76 223e 3c63 6f64 653e  nv/pyenv"><code>
-00000a10: 7079 656e 763c 2f63 6f64 653e 3c2f 613e  pyenv</code></a>
-00000a20: 2e3c 2f73 756d 6d61 7279 3e0a 0a60 6060  .</summary>..```
-00000a30: 6261 7368 0a23 2069 6e73 7461 6c6c 2070  bash.# install p
-00000a40: 7965 6e76 0a67 6974 2063 6c6f 6e65 2068  yenv.git clone h
-00000a50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000a60: 6d2f 7079 656e 762f 7079 656e 7620 7e2f  m/pyenv/pyenv ~/
-00000a70: 2e70 7965 6e76 0a0a 2320 7365 7475 7020  .pyenv..# setup 
-00000a80: 7079 656e 7620 2879 6f75 2073 686f 756c  pyenv (you shoul
-00000a90: 6420 616c 736f 2070 7574 2074 6865 7365  d also put these
-00000aa0: 2074 6872 6565 206c 696e 6573 2069 6e20   three lines in 
-00000ab0: 2e62 6173 6872 6320 6f72 2073 696d 696c  .bashrc or simil
-00000ac0: 6172 290a 6578 706f 7274 2050 4154 483d  ar).export PATH=
-00000ad0: 2224 7b48 4f4d 457d 2f2e 7079 656e 762f  "${HOME}/.pyenv/
-00000ae0: 6269 6e3a 247b 5041 5448 7d22 0a65 7870  bin:${PATH}".exp
-00000af0: 6f72 7420 5059 454e 565f 524f 4f54 3d22  ort PYENV_ROOT="
-00000b00: 247b 484f 4d45 7d2f 2e70 7965 6e76 220a  ${HOME}/.pyenv".
-00000b10: 6576 616c 2022 2428 7079 656e 7620 696e  eval "$(pyenv in
-00000b20: 6974 202d 2922 0a0a 2320 696e 7374 616c  it -)"..# instal
-00000b30: 6c20 5079 7468 6f6e 2033 2e37 0a70 7965  l Python 3.7.pye
-00000b40: 6e76 2069 6e73 7461 6c6c 2033 2e37 2e31  nv install 3.7.1
-00000b50: 320a 0a23 206d 616b 6520 6974 2061 7661  2..# make it ava
-00000b60: 696c 6162 6c65 2067 6c6f 6261 6c6c 790a  ilable globally.
-00000b70: 7079 656e 7620 676c 6f62 616c 2073 7973  pyenv global sys
-00000b80: 7465 6d20 332e 372e 3132 0a60 6060 0a3c  tem 3.7.12.```.<
-00000b90: 2f64 6574 6169 6c73 3e0a                 /details>.
+000002f0: 6d2f 6d6b 646f 6373 7472 696e 6773 2f61  m/mkdocstrings/a
+00000300: 7574 6f72 6566 7329 0a0a 4175 746f 6d61  utorefs)..Automa
+00000310: 7469 6361 6c6c 7920 6c69 6e6b 2061 6372  tically link acr
+00000320: 6f73 7320 7061 6765 7320 696e 204d 6b44  oss pages in MkD
+00000330: 6f63 732e 0a0a 2323 2049 6e73 7461 6c6c  ocs...## Install
+00000340: 6174 696f 6e0a 0a57 6974 6820 6070 6970  ation..With `pip
+00000350: 603a 0a60 6060 6261 7368 0a70 7974 686f  `:.```bash.pytho
+00000360: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
+00000370: 6c20 6d6b 646f 6373 2d61 7574 6f72 6566  l mkdocs-autoref
+00000380: 730a 6060 600a 0a23 2320 5573 6167 650a  s.```..## Usage.
+00000390: 0a60 6060 7961 6d6c 0a23 206d 6b64 6f63  .```yaml.# mkdoc
+000003a0: 732e 796d 6c0a 706c 7567 696e 733a 0a20  s.yml.plugins:. 
+000003b0: 202d 2073 6561 7263 680a 2020 2d20 6175   - search.  - au
+000003c0: 746f 7265 6673 0a60 6060 0a0a 496e 206f  torefs.```..In o
+000003d0: 6e65 206f 6620 796f 7572 204d 6172 6b64  ne of your Markd
+000003e0: 6f77 6e20 6669 6c65 7320 2865 2e67 2e20  own files (e.g. 
+000003f0: 6064 6f63 312e 6d64 6029 2063 7265 6174  `doc1.md`) creat
+00000400: 6520 736f 6d65 2068 6561 6469 6e67 733a  e some headings:
+00000410: 0a0a 6060 606d 6172 6b64 6f77 6e0a 2323  ..```markdown.##
+00000420: 2048 656c 6c6f 2c20 776f 726c 6421 0a0a   Hello, world!..
+00000430: 2323 2041 6e6f 7468 6572 2068 6561 6469  ## Another headi
+00000440: 6e67 0a0a 4c69 6e6b 2074 6f20 5b48 656c  ng..Link to [Hel
+00000450: 6c6f 2c20 576f 726c 6421 5d28 2368 656c  lo, World!](#hel
+00000460: 6c6f 2d77 6f72 6c64 2920 6f6e 2074 6865  lo-world) on the
+00000470: 2073 616d 6520 7061 6765 2e0a 6060 600a   same page..```.
+00000480: 0a54 6869 7320 6973 2061 205b 2a6e 6f72  .This is a [*nor
+00000490: 6d61 6c2a 206c 696e 6b20 746f 2061 6e20  mal* link to an 
+000004a0: 616e 6368 6f72 5d28 6874 7470 733a 2f2f  anchor](https://
+000004b0: 7777 772e 6d6b 646f 6373 2e6f 7267 2f75  www.mkdocs.org/u
+000004c0: 7365 722d 6775 6964 652f 7772 6974 696e  ser-guide/writin
+000004d0: 672d 796f 7572 2d64 6f63 732f 236c 696e  g-your-docs/#lin
+000004e0: 6b69 6e67 2d74 6f2d 7061 6765 7329 2e20  king-to-pages). 
+000004f0: 4d6b 446f 6373 2067 656e 6572 6174 6573  MkDocs generates
+00000500: 2061 6e63 686f 7273 2066 6f72 2065 6163   anchors for eac
+00000510: 6820 6865 6164 696e 672c 2061 6e64 2074  h heading, and t
+00000520: 6865 7920 6361 6e20 616c 7761 7973 2062  hey can always b
+00000530: 6520 7573 6564 2074 6f20 6c69 6e6b 2074  e used to link t
+00000540: 6f20 736f 6d65 7468 696e 672c 2065 6974  o something, eit
+00000550: 6865 7220 7769 7468 696e 2074 6865 2073  her within the s
+00000560: 616d 6520 7061 6765 2028 6173 2073 686f  ame page (as sho
+00000570: 776e 2068 6572 6529 206f 7220 6279 2073  wn here) or by s
+00000580: 7065 6369 6679 696e 6720 7468 6520 7061  pecifying the pa
+00000590: 7468 206f 6620 7468 6520 6f74 6865 7220  th of the other 
+000005a0: 7061 6765 2e0a 0a42 7574 2077 6974 6820  page...But with 
+000005b0: 7468 6973 2070 6c75 6769 6e2c 2079 6f75  this plugin, you
+000005c0: 2063 616e 202a 2a6c 696e 6b20 746f 2061   can **link to a
+000005d0: 2068 6561 6469 6e67 2066 726f 6d20 616e   heading from an
+000005e0: 7920 6f74 6865 7220 7061 6765 2a2a 206f  y other page** o
+000005f0: 6e20 7468 6520 7369 7465 202a 7769 7468  n the site *with
+00000600: 6f75 742a 206e 6565 6469 6e67 2074 6f20  out* needing to 
+00000610: 6b6e 6f77 2074 6865 2070 6174 6820 6f66  know the path of
+00000620: 2065 6974 6865 7220 6f66 2074 6865 2070   either of the p
+00000630: 6167 6573 2c20 6a75 7374 2074 6865 2068  ages, just the h
+00000640: 6561 6469 6e67 2074 6974 6c65 2069 7473  eading title its
+00000650: 656c 662e 2020 0a4c 6574 2773 2063 7265  elf.  .Let's cre
+00000660: 6174 6520 616e 6f74 6865 7220 4d61 726b  ate another Mark
+00000670: 646f 776e 2070 6167 6520 746f 2074 7279  down page to try
+00000680: 2074 6869 732c 2060 7375 6264 6972 2f64   this, `subdir/d
+00000690: 6f63 322e 6d64 603a 0a0a 6060 606d 6172  oc2.md`:..```mar
+000006a0: 6b64 6f77 6e0a 5765 2063 616e 205b 6c69  kdown.We can [li
+000006b0: 6e6b 2074 6f20 7468 6174 2068 6561 6469  nk to that headi
+000006c0: 6e67 5d5b 6865 6c6c 6f2d 776f 726c 645d  ng][hello-world]
+000006d0: 2066 726f 6d20 616e 6f74 6865 7220 7061   from another pa
+000006e0: 6765 2074 6f6f 2e0a 0a54 6869 7320 776f  ge too...This wo
+000006f0: 726b 7320 7468 6520 7361 6d65 2061 7320  rks the same as 
+00000700: 5b61 206e 6f72 6d61 6c20 6c69 6e6b 2074  [a normal link t
+00000710: 6f20 7468 6174 2068 6561 6469 6e67 5d28  o that heading](
+00000720: 2e2e 2f64 6f63 312e 6d64 2368 656c 6c6f  ../doc1.md#hello
+00000730: 2d77 6f72 6c64 292e 0a60 6060 0a0a 4c69  -world)..```..Li
+00000740: 6e6b 696e 6720 746f 2061 2068 6561 6469  nking to a headi
+00000750: 6e67 2077 6974 686f 7574 206e 6565 6469  ng without needi
+00000760: 6e67 2074 6f20 6b6e 6f77 2074 6865 2064  ng to know the d
+00000770: 6573 7469 6e61 7469 6f6e 2070 6167 6520  estination page 
+00000780: 6361 6e20 6265 2075 7365 6675 6c20 6966  can be useful if
+00000790: 2073 7065 6369 6679 696e 6720 7468 6174   specifying that
+000007a0: 2070 6174 6820 6973 2063 756d 6265 7273   path is cumbers
+000007b0: 6f6d 652c 2065 2e67 2e20 7768 656e 2074  ome, e.g. when t
+000007c0: 6865 2070 6167 6573 2068 6176 6520 6465  he pages have de
+000007d0: 6570 6c79 206e 6573 7465 6420 7061 7468  eply nested path
+000007e0: 732c 2061 7265 2066 6172 2061 7061 7274  s, are far apart
+000007f0: 2c20 6f72 2061 7265 206d 6f76 6564 2061  , or are moved a
+00000800: 726f 756e 6420 6672 6571 7565 6e74 6c79  round frequently
+00000810: 2e20 416e 6420 7468 6520 6973 7375 6520  . And the issue 
+00000820: 6973 2073 6f6d 6577 6861 7420 6578 6163  is somewhat exac
+00000830: 6572 6261 7465 6420 6279 2074 6865 2066  erbated by the f
+00000840: 6163 7420 7468 6174 205b 4d6b 446f 6373  act that [MkDocs
+00000850: 2073 7570 706f 7274 7320 6f6e 6c79 202a   supports only *
+00000860: 7265 6c61 7469 7665 2a20 6c69 6e6b 7320  relative* links 
+00000870: 6265 7477 6565 6e20 7061 6765 735d 2868  between pages](h
+00000880: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000890: 6d2f 6d6b 646f 6373 2f6d 6b64 6f63 732f  m/mkdocs/mkdocs/
+000008a0: 6973 7375 6573 2f31 3539 3229 2e0a 0a4e  issues/1592)...N
+000008b0: 6f74 6520 7468 6174 2074 6869 7320 706c  ote that this pl
+000008c0: 7567 696e 2773 2062 6568 6176 696f 7220  ugin's behavior 
+000008d0: 6973 2075 6e64 6566 696e 6564 2077 6865  is undefined whe
+000008e0: 6e20 7472 7969 6e67 2074 6f20 6c69 6e6b  n trying to link
+000008f0: 2074 6f20 6120 6865 6164 696e 6720 7469   to a heading ti
+00000900: 746c 6520 7468 6174 2061 7070 6561 7273  tle that appears
+00000910: 2073 6576 6572 616c 2074 696d 6573 2074   several times t
+00000920: 6872 6f75 6768 6f75 7420 7468 6520 7369  hroughout the si
+00000930: 7465 2e20 4375 7272 656e 746c 7920 6974  te. Currently it
+00000940: 2061 7262 6974 7261 7269 6c79 2063 686f   arbitrarily cho
+00000950: 6f73 6573 206f 6e65 206f 6620 7468 6520  oses one of the 
+00000960: 7061 6765 732e 0a                        pages..
```

### Comparing `mkdocs-autorefs-0.4.1/src/mkdocs_autorefs/plugin.py` & `mkdocs_autorefs-0.5.0/src/mkdocs_autorefs/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,30 +6,38 @@
 
 Just before writing the final HTML to the disc, during the
 [`on_post_page` event hook](https://www.mkdocs.org/user-guide/plugins/#on_post_page),
 this plugin searches for references of the form `[identifier][]` or `[title][identifier]` that were not resolved,
 and fixes them using the previously stored identifier-URL mapping.
 """
 
+from __future__ import annotations
+
 import contextlib
 import functools
 import logging
-from typing import Callable, Dict, Optional, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Sequence
 from urllib.parse import urlsplit
 
-from mkdocs.config import Config
 from mkdocs.plugins import BasePlugin
-from mkdocs.structure.pages import Page
-from mkdocs.structure.toc import AnchorLink
-from mkdocs.utils import warning_filter
 
 from mkdocs_autorefs.references import AutorefsExtension, fix_refs, relative_url
 
-log = logging.getLogger(f"mkdocs.plugins.{__name__}")
-log.addFilter(warning_filter)
+if TYPE_CHECKING:
+    from mkdocs.config.defaults import MkDocsConfig
+    from mkdocs.structure.pages import Page
+    from mkdocs.structure.toc import AnchorLink
+
+try:
+    from mkdocs.plugins import get_plugin_logger
+
+    log = get_plugin_logger(__name__)
+except ImportError:
+    # TODO: remove once support for MkDocs <1.5 is dropped
+    log = logging.getLogger(f"mkdocs.plugins.{__name__}")  # type: ignore[assignment]
 
 
 class AutorefsPlugin(BasePlugin):
     """An `mkdocs` plugin.
 
     This plugin defines the following event hooks:
 
@@ -38,45 +46,45 @@
     - `on_post_page`
 
     Check the [Developing Plugins](https://www.mkdocs.org/user-guide/plugins/#developing-plugins) page of `mkdocs`
     for more information about its plugin system.
     """
 
     scan_toc: bool = True
-    current_page: Optional[str] = None
+    current_page: str | None = None
 
     def __init__(self) -> None:
         """Initialize the object."""
         super().__init__()
-        self._url_map: Dict[str, str] = {}
-        self._abs_url_map: Dict[str, str] = {}
-        self.get_fallback_anchor: Optional[Callable[[str], Optional[str]]] = None  # noqa: WPS234
+        self._url_map: dict[str, str] = {}
+        self._abs_url_map: dict[str, str] = {}
+        self.get_fallback_anchor: Callable[[str], str | None] | None = None
 
-    def register_anchor(self, page: str, identifier: str):
+    def register_anchor(self, page: str, identifier: str) -> None:
         """Register that an anchor corresponding to an identifier was encountered when rendering the page.
 
         Arguments:
             page: The relative URL of the current page. Examples: `'foo/bar/'`, `'foo/index.html'`
             identifier: The HTML anchor (without '#') as a string.
         """
         self._url_map[identifier] = f"{page}#{identifier}"
 
-    def register_url(self, identifier: str, url: str):
+    def register_url(self, identifier: str, url: str) -> None:
         """Register that the identifier should be turned into a link to this URL.
 
         Arguments:
             identifier: The new identifier.
             url: The absolute URL (including anchor, if needed) where this item can be found.
         """
         self._abs_url_map[identifier] = url
 
-    def _get_item_url(  # noqa: WPS234
+    def _get_item_url(
         self,
         identifier: str,
-        fallback: Optional[Callable[[str], Sequence[str]]] = None,
+        fallback: Callable[[str], Sequence[str]] | None = None,
     ) -> str:
         try:
             return self._url_map[identifier]
         except KeyError:
             if identifier in self._abs_url_map:
                 return self._abs_url_map[identifier]
             if fallback:
@@ -84,19 +92,19 @@
                 for new_identifier in new_identifiers:
                     with contextlib.suppress(KeyError):
                         url = self._get_item_url(new_identifier)
                         self._url_map[identifier] = url
                         return url
             raise
 
-    def get_item_url(  # noqa: WPS234
+    def get_item_url(
         self,
         identifier: str,
-        from_url: Optional[str] = None,
-        fallback: Optional[Callable[[str], Sequence[str]]] = None,
+        from_url: str | None = None,
+        fallback: Callable[[str], Sequence[str]] | None = None,
     ) -> str:
         """Return a site-relative URL with anchor to the identifier, if it's present anywhere.
 
         Arguments:
             identifier: The anchor (without '#').
             from_url: The URL of the base page, from which we link towards the targeted pages.
             fallback: An optional function to suggest alternative anchors to try on failure.
@@ -107,47 +115,46 @@
         url = self._get_item_url(identifier, fallback)
         if from_url is not None:
             parsed = urlsplit(url)
             if not parsed.scheme and not parsed.netloc:
                 return relative_url(from_url, url)
         return url
 
-    def on_config(self, config: Config, **kwargs) -> Config:  # noqa: W0613,R0201 (unused arguments, cannot be static)
+    def on_config(self, config: MkDocsConfig) -> MkDocsConfig | None:
         """Instantiate our Markdown extension.
 
         Hook for the [`on_config` event](https://www.mkdocs.org/user-guide/plugins/#on_config).
         In this hook, we instantiate our [`AutorefsExtension`][mkdocs_autorefs.references.AutorefsExtension]
         and add it to the list of Markdown extensions used by `mkdocs`.
 
         Arguments:
             config: The MkDocs config object.
-            kwargs: Additional arguments passed by MkDocs.
 
         Returns:
             The modified config.
         """
-        log.debug(f"{__name__}: Adding AutorefsExtension to the list")
+        log.debug("Adding AutorefsExtension to the list")
         config["markdown_extensions"].append(AutorefsExtension())
         return config
 
-    def on_page_markdown(self, markdown: str, page: Page, **kwargs) -> str:  # noqa: W0613 (unused arguments)
+    def on_page_markdown(self, markdown: str, page: Page, **kwargs: Any) -> str:  # noqa: ARG002
         """Remember which page is the current one.
 
         Arguments:
             markdown: Input Markdown.
             page: The related MkDocs page instance.
             kwargs: Additional arguments passed by MkDocs.
 
         Returns:
             The same Markdown. We only use this hook to map anchors to URLs.
         """
-        self.current_page = page.url  # noqa: WPS601
+        self.current_page = page.url
         return markdown
 
-    def on_page_content(self, html: str, page: Page, **kwargs) -> str:  # noqa: W0613 (unused arguments)
+    def on_page_content(self, html: str, page: Page, **kwargs: Any) -> str:  # noqa: ARG002
         """Map anchors to URLs.
 
         Hook for the [`on_page_content` event](https://www.mkdocs.org/user-guide/plugins/#on_page_content).
         In this hook, we map the IDs of every anchor found in the table of contents to the anchors absolute URLs.
         This mapping will be used later to fix unresolved reference of the form `[title][identifier]` or
         `[identifier][]`.
 
@@ -156,15 +163,15 @@
             page: The related MkDocs page instance.
             kwargs: Additional arguments passed by MkDocs.
 
         Returns:
             The same HTML. We only use this hook to map anchors to URLs.
         """
         if self.scan_toc:
-            log.debug(f"{__name__}: Mapping identifiers to URLs for page {page.file.src_path}")
+            log.debug(f"Mapping identifiers to URLs for page {page.file.src_path}")
             for item in page.toc.items:
                 self.map_urls(page.url, item)
         return html
 
     def map_urls(self, base_url: str, anchor: AnchorLink) -> None:
         """Recurse on every anchor to map its ID to its absolute URL.
 
@@ -174,15 +181,15 @@
             base_url: The base URL to use as a prefix for each anchor's relative URL.
             anchor: The anchor to process and to recurse on.
         """
         self.register_anchor(base_url, anchor.id)
         for child in anchor.children:
             self.map_urls(base_url, child)
 
-    def on_post_page(self, output: str, page: Page, **kwargs) -> str:  # noqa: W0613 (unused arguments)
+    def on_post_page(self, output: str, page: Page, **kwargs: Any) -> str:  # noqa: ARG002
         """Fix cross-references.
 
         Hook for the [`on_post_page` event](https://www.mkdocs.org/user-guide/plugins/#on_post_page).
         In this hook, we try to fix unresolved references of the form `[title][identifier]` or `[identifier][]`.
         Doing that allows the user of `autorefs` to cross-reference objects in their documentation strings.
         It uses the native Markdown syntax so it's easy to remember and use.
 
@@ -195,19 +202,17 @@
             output: HTML converted from Markdown.
             page: The related MkDocs page instance.
             kwargs: Additional arguments passed by MkDocs.
 
         Returns:
             Modified HTML.
         """
-        log.debug(f"{__name__}: Fixing references in page {page.file.src_path}")
+        log.debug(f"Fixing references in page {page.file.src_path}")
 
         url_mapper = functools.partial(self.get_item_url, from_url=page.url, fallback=self.get_fallback_anchor)
         fixed_output, unmapped = fix_refs(output, url_mapper)
 
         if unmapped and log.isEnabledFor(logging.WARNING):
             for ref in unmapped:
-                log.warning(
-                    f"{__name__}: {page.file.src_path}: Could not find cross-reference target '[{ref}]'",
-                )
+                log.warning(f"{page.file.src_path}: Could not find cross-reference target '[{ref}]'")
 
         return fixed_output
```

### Comparing `mkdocs-autorefs-0.4.1/src/mkdocs_autorefs/references.py` & `mkdocs_autorefs-0.5.0/src/mkdocs_autorefs/references.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """Cross-references module."""
 
+from __future__ import annotations
+
 import re
 from html import escape, unescape
-from typing import Any, Callable, List, Match, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Match, Tuple
 from urllib.parse import urlsplit
 from xml.etree.ElementTree import Element
 
-from markdown import Markdown
 from markdown.extensions import Extension
 from markdown.inlinepatterns import REFERENCE_RE, ReferenceInlineProcessor
 from markdown.util import INLINE_PLACEHOLDER_RE
 
+if TYPE_CHECKING:
+    from markdown import Markdown
+
 AUTO_REF_RE = re.compile(
     r"<span data-(?P<kind>autorefs-identifier|autorefs-optional|autorefs-optional-hover)="
-    r'("?)(?P<identifier>[^"<>]*)\2>(?P<title>.*?)</span>'
+    r'("?)(?P<identifier>[^"<>]*)\2>(?P<title>.*?)</span>',
 )
 """A regular expression to match mkdocs-autorefs' special reference markers
 in the [`on_post_page` hook][mkdocs_autorefs.plugin.AutorefsPlugin.on_post_page].
 """
 
 EvalIDType = Tuple[Any, Any, Any]
 
 
 class AutoRefInlineProcessor(ReferenceInlineProcessor):
     """A Markdown extension."""
 
-    def __init__(self, *args, **kwargs):  # noqa: D107
+    def __init__(self, *args: Any, **kwargs: Any) -> None:  # noqa: D107
         super().__init__(REFERENCE_RE, *args, **kwargs)
 
     # Code based on
     # https://github.com/Python-Markdown/markdown/blob/8e7528fa5c98bf4652deb13206d6e6241d61630b/markdown/inlinepatterns.py#L780
 
-    def handleMatch(self, m, data) -> Union[Element, EvalIDType]:  # type: ignore[override]  # noqa: N802,WPS111
+    def handleMatch(self, m: Match[str], data: Any) -> Element | EvalIDType:  # type: ignore[override]  # noqa: N802
         """Handle an element that matched.
 
         Arguments:
             m: The match object.
             data: The matched data.
 
         Returns:
@@ -67,15 +71,15 @@
             data: The data to evaluate.
             index: The starting position.
             text: The text to use when no identifier.
 
         Returns:
             A tuple containing the identifier, its end position, and whether it matched.
         """
-        m = self.RE_LINK.match(data, pos=index)  # noqa: WPS111
+        m = self.RE_LINK.match(data, pos=index)
         if not m:
             return None, index, False
 
         identifier = m.group(1)
         if not identifier:
             identifier = text
             # Allow the entire content to be one placeholder, with the intent of catching things like [`Foo`][].
@@ -83,15 +87,15 @@
             # https://github.com/Python-Markdown/markdown/blob/1858c1b601ead62ed49646ae0d99298f41b1a271/markdown/inlinepatterns.py#L78
             if INLINE_PLACEHOLDER_RE.fullmatch(identifier):
                 identifier = self.unescape(identifier)
 
         end = m.end(0)
         return identifier, end, True
 
-    def makeTag(self, identifier: str, text: str) -> Element:  # type: ignore[override]  # noqa: N802,W0221
+    def makeTag(self, identifier: str, text: str) -> Element:  # type: ignore[override]  # noqa: N802
         """Create a tag that can be matched by `AUTO_REF_RE`.
 
         Arguments:
             identifier: The identifier to use in the HTML property.
             text: The text to use in the HTML tag.
 
         Returns:
@@ -120,20 +124,20 @@
     # remove common left parts
     while parts_a and parts_b and parts_a[0] == parts_b[0]:
         parts_a.pop(0)
         parts_b.pop(0)
 
     # go up as many times as remaining a parts' depth
     levels = len(parts_a) - 1
-    parts_relative = [".."] * levels + parts_b  # noqa: WPS435
+    parts_relative = [".."] * levels + parts_b
     relative = "/".join(parts_relative)
     return f"{relative}#{anchor}"
 
 
-def fix_ref(url_mapper: Callable[[str], str], unmapped: List[str]) -> Callable:  # noqa: WPS212,WPS231
+def fix_ref(url_mapper: Callable[[str], str], unmapped: list[str]) -> Callable:
     """Return a `repl` function for [`re.sub`](https://docs.python.org/3/library/re.html#re.sub).
 
     In our context, we match Markdown references and replace them with HTML links.
 
     When the matched reference's identifier was not mapped to an URL, we append the identifier to the outer
     `unmapped` list. It generally means the user is trying to cross-reference an object that was not collected
     and rendered, making it impossible to link to it. We catch this exception in the caller to issue a warning.
@@ -144,25 +148,25 @@
         unmapped: A list to store unmapped identifiers.
 
     Returns:
         The actual function accepting a [`Match` object](https://docs.python.org/3/library/re.html#match-objects)
         and returning the replacement strings.
     """
 
-    def inner(match: Match):  # noqa: WPS212,WPS430
+    def inner(match: Match) -> str:
         identifier = match["identifier"]
         title = match["title"]
         kind = match["kind"]
 
         try:
             url = url_mapper(unescape(identifier))
         except KeyError:
             if kind == "autorefs-optional":
                 return title
-            elif kind == "autorefs-optional-hover":
+            if kind == "autorefs-optional-hover":
                 return f'<span title="{identifier}">{title}</span>'
             unmapped.append(identifier)
             if title == identifier:
                 return f"[{identifier}][]"
             return f"[{title}][{identifier}]"
 
         parsed = urlsplit(url)
@@ -172,26 +176,26 @@
         if kind == "autorefs-optional-hover":
             return f'<a class="{class_attr}" title="{identifier}" href="{escape(url)}">{title}</a>'
         return f'<a class="{class_attr}" href="{escape(url)}">{title}</a>'
 
     return inner
 
 
-def fix_refs(html: str, url_mapper: Callable[[str], str]) -> Tuple[str, List[str]]:
+def fix_refs(html: str, url_mapper: Callable[[str], str]) -> tuple[str, list[str]]:
     """Fix all references in the given HTML text.
 
     Arguments:
         html: The text to fix.
         url_mapper: A callable that gets an object's site URL by its identifier,
             such as [mkdocs_autorefs.plugin.AutorefsPlugin.get_item_url][].
 
     Returns:
         The fixed HTML.
     """
-    unmapped = []  # type: ignore
+    unmapped: list[str] = []
     html = AUTO_REF_RE.sub(fix_ref(url_mapper, unmapped), html)
     return html, unmapped
 
 
 class AutorefsExtension(Extension):
     """Extension that inserts auto-references in Markdown."""
 
@@ -202,9 +206,9 @@
 
         Arguments:
             md: A `markdown.Markdown` instance.
         """
         md.inlinePatterns.register(
             AutoRefInlineProcessor(md),
             "mkdocs-autorefs",
-            priority=168,  # noqa: WPS432  # Right after markdown.inlinepatterns.ReferenceInlineProcessor
+            priority=168,  # Right after markdown.inlinepatterns.ReferenceInlineProcessor
         )
```

### Comparing `mkdocs-autorefs-0.4.1/tests/test_plugin.py` & `mkdocs_autorefs-0.5.0/tests/test_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """Tests for the plugin module."""
+
+from __future__ import annotations
+
 import pytest
 
 from mkdocs_autorefs.plugin import AutorefsPlugin
 
 
-def test_url_registration():
+def test_url_registration() -> None:
     """Check that URLs can be registered, then obtained."""
     plugin = AutorefsPlugin()
     plugin.register_anchor(identifier="foo", page="foo1.html")
     plugin.register_url(identifier="bar", url="https://example.org/bar.html")
 
     assert plugin.get_item_url("foo") == "foo1.html#foo"
     assert plugin.get_item_url("bar") == "https://example.org/bar.html"
     with pytest.raises(KeyError):
         plugin.get_item_url("baz")
 
 
-def test_url_registration_with_from_url():
+def test_url_registration_with_from_url() -> None:
     """Check that URLs can be registered, then obtained, relative to a page."""
     plugin = AutorefsPlugin()
     plugin.register_anchor(identifier="foo", page="foo1.html")
     plugin.register_url(identifier="bar", url="https://example.org/bar.html")
 
     assert plugin.get_item_url("foo", from_url="a/b.html") == "../foo1.html#foo"
     assert plugin.get_item_url("bar", from_url="a/b.html") == "https://example.org/bar.html"
     with pytest.raises(KeyError):
         plugin.get_item_url("baz", from_url="a/b.html")
 
 
-def test_url_registration_with_fallback():
+def test_url_registration_with_fallback() -> None:
     """Check that URLs can be registered, then obtained through a fallback."""
     plugin = AutorefsPlugin()
     plugin.register_anchor(identifier="foo", page="foo1.html")
     plugin.register_url(identifier="bar", url="https://example.org/bar.html")
 
     # URL map will be updated with baz -> foo1.html#foo
     assert plugin.get_item_url("baz", fallback=lambda _: ("foo",)) == "foo1.html#foo"
@@ -43,15 +46,15 @@
 
     with pytest.raises(KeyError):
         plugin.get_item_url("foobar", fallback=lambda _: ("baaaa",))
     with pytest.raises(KeyError):
         plugin.get_item_url("foobar", fallback=lambda _: ())
 
 
-def test_dont_make_relative_urls_relative_again():
+def test_dont_make_relative_urls_relative_again() -> None:
     """Check that URLs are not made relative more than once."""
     plugin = AutorefsPlugin()
     plugin.register_anchor(identifier="foo.bar.baz", page="foo/bar/baz.html")
 
     for _ in range(2):
         assert (
             plugin.get_item_url("hello", from_url="baz/bar/foo.html", fallback=lambda _: ("foo.bar.baz",))
```

### Comparing `mkdocs-autorefs-0.4.1/tests/test_references.py` & `mkdocs_autorefs-0.5.0/tests/test_references.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Tests for the references module."""
+
+from __future__ import annotations
+
 import markdown
 import pytest
 
 from mkdocs_autorefs.references import AutorefsExtension, fix_refs, relative_url
 
 
 @pytest.mark.parametrize(
@@ -26,183 +29,189 @@
         ("", "#x", "#x"),
         ("a/", "#x", "../#x"),
         ("a/b.html", "#x", "../#x"),
         ("", "a/#x", "a/#x"),
         ("", "a/b.html#x", "a/b.html#x"),
     ],
 )
-def test_relative_url(current_url, to_url, href_url):
+def test_relative_url(current_url: str, to_url: str, href_url: str) -> None:
     """Compute relative URLs correctly."""
     assert relative_url(current_url, to_url) == href_url
 
 
-def run_references_test(url_map, source, output, unmapped=None, from_url="page.html"):
+def run_references_test(
+    url_map: dict[str, str],
+    source: str,
+    output: str,
+    unmapped: list[str] | None = None,
+    from_url: str = "page.html",
+) -> None:
     """Help running tests about references.
 
     Arguments:
         url_map: The URL mapping.
         source: The source text.
         output: The expected output.
         unmapped: The expected unmapped list.
         from_url: The source page URL.
     """
     md = markdown.Markdown(extensions=[AutorefsExtension()])
     content = md.convert(source)
 
-    def url_mapper(identifier):  # noqa: WPS430
+    def url_mapper(identifier: str) -> str:
         return relative_url(from_url, url_map[identifier])
 
     actual_output, actual_unmapped = fix_refs(content, url_mapper)
     assert actual_output == output
     assert actual_unmapped == (unmapped or [])
 
 
-def test_reference_implicit():
+def test_reference_implicit() -> None:
     """Check implicit references (identifier only)."""
     run_references_test(
         url_map={"Foo": "foo.html#Foo"},
         source="This [Foo][].",
         output='<p>This <a class="autorefs autorefs-internal" href="foo.html#Foo">Foo</a>.</p>',
     )
 
 
-def test_reference_explicit_with_markdown_text():
+def test_reference_explicit_with_markdown_text() -> None:
     """Check explicit references with Markdown formatting."""
     run_references_test(
         url_map={"Foo": "foo.html#Foo"},
         source="This [**Foo**][Foo].",
         output='<p>This <a class="autorefs autorefs-internal" href="foo.html#Foo"><strong>Foo</strong></a>.</p>',
     )
 
 
-def test_reference_implicit_with_code():
+def test_reference_implicit_with_code() -> None:
     """Check implicit references (identifier only, wrapped in backticks)."""
     run_references_test(
         url_map={"Foo": "foo.html#Foo"},
         source="This [`Foo`][].",
         output='<p>This <a class="autorefs autorefs-internal" href="foo.html#Foo"><code>Foo</code></a>.</p>',
     )
 
 
-def test_reference_with_punctuation():
+def test_reference_with_punctuation() -> None:
     """Check references with punctuation."""
     run_references_test(
         url_map={'Foo&"bar': 'foo.html#Foo&"bar'},
         source='This [Foo&"bar][].',
         output='<p>This <a class="autorefs autorefs-internal" href="foo.html#Foo&amp;&quot;bar">Foo&amp;"bar</a>.</p>',
     )
 
 
-def test_reference_to_relative_path():
+def test_reference_to_relative_path() -> None:
     """Check references from a page at a nested path."""
     run_references_test(
         from_url="sub/sub/page.html",
         url_map={"zz": "foo.html#zz"},
         source="This [zz][].",
         output='<p>This <a class="autorefs autorefs-internal" href="../../foo.html#zz">zz</a>.</p>',
     )
 
 
-def test_no_reference_with_space():
+def test_no_reference_with_space() -> None:
     """Check that references with spaces are not fixed."""
     run_references_test(
         url_map={"Foo bar": "foo.html#Foo bar"},
         source="This [Foo bar][].",
         output="<p>This [Foo bar][].</p>",
     )
 
 
-def test_no_reference_inside_markdown():
+def test_no_reference_inside_markdown() -> None:
     """Check that references inside code are not fixed."""
     run_references_test(
         url_map={"Foo": "foo.html#Foo"},
         source="This `[Foo][]`.",
         output="<p>This <code>[Foo][]</code>.</p>",
     )
 
 
-def test_missing_reference():
+def test_missing_reference() -> None:
     """Check that implicit references are correctly seen as unmapped."""
     run_references_test(
         url_map={"NotFoo": "foo.html#NotFoo"},
         source="[Foo][]",
         output="<p>[Foo][]</p>",
         unmapped=["Foo"],
     )
 
 
-def test_missing_reference_with_markdown_text():
+def test_missing_reference_with_markdown_text() -> None:
     """Check unmapped explicit references."""
     run_references_test(
         url_map={"NotFoo": "foo.html#NotFoo"},
         source="[`Foo`][Foo]",
         output="<p>[<code>Foo</code>][Foo]</p>",
         unmapped=["Foo"],
     )
 
 
-def test_missing_reference_with_markdown_id():
+def test_missing_reference_with_markdown_id() -> None:
     """Check unmapped explicit references with Markdown in the identifier."""
     run_references_test(
         url_map={"Foo": "foo.html#Foo", "NotFoo": "foo.html#NotFoo"},
         source="[Foo][*NotFoo*]",
         output="<p>[Foo][*NotFoo*]</p>",
         unmapped=["*NotFoo*"],
     )
 
 
-def test_missing_reference_with_markdown_implicit():
+def test_missing_reference_with_markdown_implicit() -> None:
     """Check that implicit references are not fixed when the identifier is not the exact one."""
     run_references_test(
         url_map={"Foo-bar": "foo.html#Foo-bar"},
         source="[*Foo-bar*][] and [`Foo`-bar][]",
         output="<p>[<em>Foo-bar</em>][*Foo-bar*] and [<code>Foo</code>-bar][]</p>",
         unmapped=["*Foo-bar*"],
     )
 
 
-def test_ignore_reference_with_special_char():
+def test_ignore_reference_with_special_char() -> None:
     """Check that references are not considered if there is a space character inside."""
     run_references_test(
         url_map={"a b": "foo.html#Foo"},
         source="This [*a b*][].",
         output="<p>This [<em>a b</em>][].</p>",
     )
 
 
-def test_custom_required_reference():
+def test_custom_required_reference() -> None:
     """Check that external HTML-based references are expanded or reported missing."""
     url_map = {"ok": "ok.html#ok"}
     source = "<span data-autorefs-identifier=bar>foo</span> <span data-autorefs-identifier=ok>ok</span>"
-    output, unmapped = fix_refs(source, url_map.__getitem__)  # noqa: WPS609
+    output, unmapped = fix_refs(source, url_map.__getitem__)
     assert output == '[foo][bar] <a class="autorefs autorefs-internal" href="ok.html#ok">ok</a>'
     assert unmapped == ["bar"]
 
 
-def test_custom_optional_reference():
+def test_custom_optional_reference() -> None:
     """Check that optional HTML-based references are expanded and never reported missing."""
     url_map = {"ok": "ok.html#ok"}
     source = '<span data-autorefs-optional="bar">foo</span> <span data-autorefs-optional=ok>ok</span>'
-    output, unmapped = fix_refs(source, url_map.__getitem__)  # noqa: WPS609
+    output, unmapped = fix_refs(source, url_map.__getitem__)
     assert output == 'foo <a class="autorefs autorefs-internal" href="ok.html#ok">ok</a>'
-    assert unmapped == []  # noqa: WPS520
+    assert unmapped == []
 
 
-def test_custom_optional_hover_reference():
+def test_custom_optional_hover_reference() -> None:
     """Check that optional-hover HTML-based references are expanded and never reported missing."""
     url_map = {"ok": "ok.html#ok"}
     source = '<span data-autorefs-optional-hover="bar">foo</span> <span data-autorefs-optional-hover=ok>ok</span>'
-    output, unmapped = fix_refs(source, url_map.__getitem__)  # noqa: WPS609
+    output, unmapped = fix_refs(source, url_map.__getitem__)
     assert (
         output
         == '<span title="bar">foo</span> <a class="autorefs autorefs-internal" title="ok" href="ok.html#ok">ok</a>'
     )
-    assert unmapped == []  # noqa: WPS520
+    assert unmapped == []
 
 
-def test_external_references():
+def test_external_references() -> None:
     """Check that external references are marked as such."""
     url_map = {"example": "https://example.com"}
     source = '<span data-autorefs-optional="example">example</span>'
-    output, unmapped = fix_refs(source, url_map.__getitem__)  # noqa: WPS609
+    output, unmapped = fix_refs(source, url_map.__getitem__)
     assert output == '<a class="autorefs autorefs-external" href="https://example.com">example</a>'
-    assert unmapped == []  # noqa: WPS520
+    assert unmapped == []
```

### Comparing `mkdocs-autorefs-0.4.1/PKG-INFO` & `mkdocs_autorefs-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,86 @@
 Metadata-Version: 2.1
 Name: mkdocs-autorefs
-Version: 0.4.1
+Version: 0.5.0
 Summary: Automatically link across pages in MkDocs.
-License: UNKNOWN
-Keywords: mkdocs,mkdocs-plugin,docstrings,autodoc
-Author-email: Oleh Prypin <oleh@pryp.in>,Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
+Keywords: mkdocs mkdocs-plugin docstrings autodoc
+Author-Email: Oleh Prypin <oleh@pryp.in>, Timothée Mazzucotelli <pawamoy@pm.me>
+License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Project-URL: Changelog, https://mkdocstrings.github.io/autorefs/changelog
-Project-URL: Discussions, https://github.com/mkdocstrings/autorefs/discussions
-Project-URL: Documentation, https://mkdocstrings.github.io/autorefs
-Project-URL: Gitter, https://gitter.im/mkdocstrings/community
 Project-URL: Homepage, https://mkdocstrings.github.io/autorefs
-Project-URL: Issues, https://github.com/mkdocstrings/autorefs/issues
+Project-URL: Documentation, https://mkdocstrings.github.io/autorefs
+Project-URL: Changelog, https://mkdocstrings.github.io/autorefs/changelog
 Project-URL: Repository, https://github.com/mkdocstrings/autorefs
+Project-URL: Issues, https://github.com/mkdocstrings/autorefs/issues
+Project-URL: Discussions, https://github.com/mkdocstrings/autorefs/discussions
+Project-URL: Gitter, https://gitter.im/mkdocstrings/autorefs
+Requires-Python: >=3.8
+Requires-Dist: Markdown>=3.3
+Requires-Dist: mkdocs>=1.1
 Description-Content-Type: text/markdown
-Description: # mkdocs-autorefs
-        
-        [![ci](https://github.com/mkdocstrings/autorefs/workflows/ci/badge.svg)](https://github.com/mkdocstrings/autorefs/actions?query=workflow%3Aci)
-        [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://mkdocstrings.github.io/autorefs/)
-        [![pypi version](https://img.shields.io/pypi/v/mkdocs-autorefs.svg)](https://pypi.org/project/mkdocs-autorefs/)
-        [![conda version](https://img.shields.io/conda/vn/conda-forge/mkdocs-autorefs.svg)](https://anaconda.org/conda-forge/mkdocs-autorefs)
-        [![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/mkdocstrings/autorefs)
-        [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/autorefs/community)
-        
-        Automatically link across pages in MkDocs.
-        
-        ## Installation
-        
-        With `pip`:
-        ```bash
-        python3 -m pip install mkdocs-autorefs
-        ```
-        
-        ## Usage
-        
-        ```yaml
-        # mkdocs.yml
-        plugins:
-          - search
-          - autorefs
-        ```
-        
-        In one of your Markdown files (e.g. `doc1.md`) create some headings:
-        
-        ```markdown
-        ## Hello, world!
-        
-        ## Another heading
-        
-        Link to [Hello, World!](#hello-world) on the same page.
-        ```
-        
-        This is a [*normal* link to an anchor](https://www.mkdocs.org/user-guide/writing-your-docs/#linking-to-pages). MkDocs generates anchors for each heading, and they can always be used to link to something, either within the same page (as shown here) or by specifying the path of the other page.
-        
-        But with this plugin, you can **link to a heading from any other page** on the site *without* needing to know the path of either of the pages, just the heading title itself.  
-        Let's create another Markdown page to try this, `subdir/doc2.md`:
-        
-        ```markdown
-        We can [link to that heading][hello-world] from another page too.
-        
-        This works the same as [a normal link to that heading](../doc1.md#hello-world).
-        ```
-        
-        Linking to a heading without needing to know the destination page can be useful if specifying that path is cumbersome, e.g. when the pages have deeply nested paths, are far apart, or are moved around frequently. And the issue is somewhat exacerbated by the fact that [MkDocs supports only *relative* links between pages](https://github.com/mkdocs/mkdocs/issues/1592).
-        
-        Note that this plugin's behavior is undefined when trying to link to a heading title that appears several times throughout the site. Currently it arbitrarily chooses one of the pages.
-        
-        ## Requirements
-        
-        mkdocs-autorefs requires Python 3.7 or above.
-        
-        <details>
-        <summary>To install Python 3.7, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
-        
-        ```bash
-        # install pyenv
-        git clone https://github.com/pyenv/pyenv ~/.pyenv
-        
-        # setup pyenv (you should also put these three lines in .bashrc or similar)
-        export PATH="${HOME}/.pyenv/bin:${PATH}"
-        export PYENV_ROOT="${HOME}/.pyenv"
-        eval "$(pyenv init -)"
-        
-        # install Python 3.7
-        pyenv install 3.7.12
-        
-        # make it available globally
-        pyenv global system 3.7.12
-        ```
-        </details>
 
+# mkdocs-autorefs
+
+[![ci](https://github.com/mkdocstrings/autorefs/workflows/ci/badge.svg)](https://github.com/mkdocstrings/autorefs/actions?query=workflow%3Aci)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://mkdocstrings.github.io/autorefs/)
+[![pypi version](https://img.shields.io/pypi/v/mkdocs-autorefs.svg)](https://pypi.org/project/mkdocs-autorefs/)
+[![conda version](https://img.shields.io/conda/vn/conda-forge/mkdocs-autorefs.svg)](https://anaconda.org/conda-forge/mkdocs-autorefs)
+[![gitpod](https://img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/#https://github.com/mkdocstrings/autorefs)
+[![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/mkdocstrings/autorefs)
+
+Automatically link across pages in MkDocs.
+
+## Installation
+
+With `pip`:
+```bash
+python3 -m pip install mkdocs-autorefs
+```
+
+## Usage
+
+```yaml
+# mkdocs.yml
+plugins:
+  - search
+  - autorefs
+```
+
+In one of your Markdown files (e.g. `doc1.md`) create some headings:
+
+```markdown
+## Hello, world!
+
+## Another heading
+
+Link to [Hello, World!](#hello-world) on the same page.
+```
+
+This is a [*normal* link to an anchor](https://www.mkdocs.org/user-guide/writing-your-docs/#linking-to-pages). MkDocs generates anchors for each heading, and they can always be used to link to something, either within the same page (as shown here) or by specifying the path of the other page.
+
+But with this plugin, you can **link to a heading from any other page** on the site *without* needing to know the path of either of the pages, just the heading title itself.  
+Let's create another Markdown page to try this, `subdir/doc2.md`:
+
+```markdown
+We can [link to that heading][hello-world] from another page too.
+
+This works the same as [a normal link to that heading](../doc1.md#hello-world).
+```
+
+Linking to a heading without needing to know the destination page can be useful if specifying that path is cumbersome, e.g. when the pages have deeply nested paths, are far apart, or are moved around frequently. And the issue is somewhat exacerbated by the fact that [MkDocs supports only *relative* links between pages](https://github.com/mkdocs/mkdocs/issues/1592).
+
+Note that this plugin's behavior is undefined when trying to link to a heading title that appears several times throughout the site. Currently it arbitrarily chooses one of the pages.
```

