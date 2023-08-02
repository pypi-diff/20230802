# Comparing `tmp/genomedata-1.6.0.tar.gz` & `tmp/genomedata-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/genomedata/genomedata/dist/.tmp-7xp49zxi/genomedata-1.6.0.tar", last modified: Mon Dec  5 18:58:22 2022, max compression
+gzip compressed data, was "/home/runner/work/genomedata/genomedata/dist/.tmp-bux8gtgx/genomedata-1.7.0.tar", last modified: Wed Aug  2 18:28:44 2023, max compression
```

## Comparing `genomedata-1.6.0.tar` & `genomedata-1.7.0.tar`

### file list

```diff
@@ -1,229 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2022-12-05 18:58:04.000000 genomedata-1.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2022-12-05 18:58:04.000000 genomedata-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)    18092 2022-12-05 18:58:04.000000 genomedata-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      259 2022-12-05 18:58:04.000000 genomedata-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9215 2022-12-05 18:58:04.000000 genomedata-1.6.0/NEWS
--rw-r--r--   0 runner    (1001) docker     (122)     2215 2022-12-05 18:58:22.000000 genomedata-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1402 2022-12-05 18:58:04.000000 genomedata-1.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      575 2022-12-05 18:58:04.000000 genomedata-1.6.0/TODO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (122)     4598 2022-12-05 18:58:04.000000 genomedata-1.6.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     7198 2022-12-05 18:58:04.000000 genomedata-1.6.0/doc/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    30692 2022-12-05 18:58:04.000000 genomedata-1.6.0/doc/genomedata.rst
--rw-r--r--   0 runner    (1001) docker     (122)      448 2022-12-05 18:58:04.000000 genomedata-1.6.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2022-12-05 18:58:04.000000 genomedata-1.6.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2022-12-05 18:58:04.000000 genomedata-1.6.0/examples/README
--rwxr-xr-x   0 runner    (1001) docker     (122)     1180 2022-12-05 18:58:04.000000 genomedata-1.6.0/examples/genomedata_fill_random.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1957 2022-12-05 18:58:04.000000 genomedata-1.6.0/examples/genomedata_offline_random_access.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      741 2022-12-05 18:58:04.000000 genomedata-1.6.0/examples/genomedata_random_access.pl
--rwxr-xr-x   0 runner    (1001) docker     (122)      956 2022-12-05 18:58:04.000000 genomedata-1.6.0/examples/genomedata_random_access.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3963 2022-12-05 18:58:04.000000 genomedata-1.6.0/examples/random_genomic_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata/
--rw-r--r--   0 runner    (1001) docker     (122)    13392 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23823 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_chromosome.py
--rw-r--r--   0 runner    (1001) docker     (122)    12885 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_close_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_erase_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7993 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_hardmask.py
--rw-r--r--   0 runner    (1001) docker     (122)     8239 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_hardmask_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15670 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_histogram.py
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_load_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    18653 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_load_seq.py
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_open_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)    12878 2022-12-05 18:58:04.000000 genomedata-1.6.0/genomedata/load_genomedata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2215 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      597 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-05 18:58:22.000000 genomedata-1.6.0/genomedata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2184 2022-12-05 18:58:04.000000 genomedata-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       75 2022-12-05 18:58:22.000000 genomedata-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     3235 2022-12-05 18:58:04.000000 genomedata-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)    36482 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/_c_load_data.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/src/build-deps/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (122)    34973 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (122)    32689 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/aclocal.m4
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/src/build-deps/build-aux/
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/arg-nonnull.h
--rw-r--r--   0 runner    (1001) docker     (122)     9980 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/c++defs.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    43420 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/config.guess
--rwxr-xr-x   0 runner    (1001) docker     (122)    31743 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/config.sub
--rwxr-xr-x   0 runner    (1001) docker     (122)    15936 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/depcomp
--rwxr-xr-x   0 runner    (1001) docker     (122)     9233 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/install-sh
--rwxr-xr-x   0 runner    (1001) docker     (122)    11014 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/missing
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/build-aux/warn-on-use.h
--rw-r--r--   0 runner    (1001) docker     (122)    28017 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/config.h.in
--rwxr-xr-x   0 runner    (1001) docker     (122)   573788 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/configure
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/src/build-deps/gllib/
--rw-r--r--   0 runner    (1001) docker     (122)    38449 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (122)    69493 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (122)    14934 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/alloca.c
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/alloca.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-ba.c
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-eexst.c
--rw-r--r--   0 runner    (1001) docker     (122)    13316 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-fmtstream.c
--rw-r--r--   0 runner    (1001) docker     (122)    13986 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-fmtstream.h
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-fs-xinl.c
--rw-r--r--   0 runner    (1001) docker     (122)    63636 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-help.c
--rw-r--r--   0 runner    (1001) docker     (122)     5498 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-namefrob.h
--rw-r--r--   0 runner    (1001) docker     (122)    31712 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-parse.c
--rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-pin.c
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-pv.c
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-pvh.c
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp-xinl.c
--rw-r--r--   0 runner    (1001) docker     (122)    29369 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/argp.h
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/asnprintf.c
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/basename-lgpl.c
--rw-r--r--   0 runner    (1001) docker     (122)     3152 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/dirname-lgpl.c
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/dirname.h
--rw-r--r--   0 runner    (1001) docker     (122)     4622 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/errno.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     9391 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/error.c
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/error.h
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/float+.h
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/float.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/getdelim.c
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/getline.c
--rw-r--r--   0 runner    (1001) docker     (122)    38984 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/getopt.c
--rw-r--r--   0 runner    (1001) docker     (122)     8871 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/getopt.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     4503 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/getopt1.c
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/getopt_int.h
--rw-r--r--   0 runner    (1001) docker     (122)     9805 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/gettext.h
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/intprops.h
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/malloc.c
--rw-r--r--   0 runner    (1001) docker     (122)     5862 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/memchr.c
--rw-r--r--   0 runner    (1001) docker     (122)      426 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/memchr.valgrind
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/mempcpy.c
--rw-r--r--   0 runner    (1001) docker     (122)     6627 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/printf-args.c
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/printf-args.h
--rw-r--r--   0 runner    (1001) docker     (122)    21573 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/printf-parse.c
--rw-r--r--   0 runner    (1001) docker     (122)     4758 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/printf-parse.h
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/progname.c
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/progname.h
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/rawmemchr.c
--rw-r--r--   0 runner    (1001) docker     (122)      259 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/rawmemchr.valgrind
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/realloc.c
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/size_max.h
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/sleep.c
--rw-r--r--   0 runner    (1001) docker     (122)     4906 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stdbool.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stddef.in.h
--rw-r--r--   0 runner    (1001) docker     (122)    16612 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stdint.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     4887 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stdio-write.c
--rw-r--r--   0 runner    (1001) docker     (122)    36538 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stdio.in.h
--rw-r--r--   0 runner    (1001) docker     (122)    24025 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stdlib.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strcasecmp.c
--rw-r--r--   0 runner    (1001) docker     (122)     5658 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strchrnul.c
--rw-r--r--   0 runner    (1001) docker     (122)      259 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strchrnul.valgrind
--rw-r--r--   0 runner    (1001) docker     (122)     8925 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strerror.c
--rw-r--r--   0 runner    (1001) docker     (122)    35064 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/string.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strings.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/stripslash.c
--rw-r--r--   0 runner    (1001) docker     (122)     1976 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strncasecmp.c
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strndup.c
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/strnlen.c
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/sysexits.in.h
--rw-r--r--   0 runner    (1001) docker     (122)    43158 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/unistd.in.h
--rw-r--r--   0 runner    (1001) docker     (122)   221260 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/vasnprintf.c
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/vasnprintf.h
--rw-r--r--   0 runner    (1001) docker     (122)     5614 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/verify.h
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/vsnprintf.c
--rw-r--r--   0 runner    (1001) docker     (122)    13554 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/wchar.in.h
--rw-r--r--   0 runner    (1001) docker     (122)     3533 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/gllib/xsize.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/src/build-deps/glm4/
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/00gnulib.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (122)    25002 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/alloca.m4
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/argp.m4
--rw-r--r--   0 runner    (1001) docker     (122)      712 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/dirname.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/dos.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/double-slash-root.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2917 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/errno_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)      557 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/error.m4
--rw-r--r--   0 runner    (1001) docker     (122)     4439 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/extensions.m4
--rw-r--r--   0 runner    (1001) docker     (122)      525 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/float_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2538 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/getdelim.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/getline.m4
--rw-r--r--   0 runner    (1001) docker     (122)     8323 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/getopt.m4
--rw-r--r--   0 runner    (1001) docker     (122)     7943 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/gnulib-common.m4
--rw-r--r--   0 runner    (1001) docker     (122)     7799 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/include_next.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/intmax_t.m4
--rw-r--r--   0 runner    (1001) docker     (122)      953 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/inttypes_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     4477 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/longlong.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/malloc.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/memchr.m4
--rw-r--r--   0 runner    (1001) docker     (122)      766 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/mempcpy.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/mmap-anon.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/multiarch.m4
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/onceonly.m4
--rw-r--r--   0 runner    (1001) docker     (122)    55812 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/printf.m4
--rw-r--r--   0 runner    (1001) docker     (122)      673 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/rawmemchr.m4
--rw-r--r--   0 runner    (1001) docker     (122)      796 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/realloc.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/size_max.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1769 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/sleep.m4
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/stdbool.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/stddef_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)    15629 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/stdint.m4
--rw-r--r--   0 runner    (1001) docker     (122)      929 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/stdint_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     7501 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/stdio_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     4816 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/stdlib_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/strcase.m4
--rw-r--r--   0 runner    (1001) docker     (122)      667 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/strchrnul.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/strerror.m4
--rw-r--r--   0 runner    (1001) docker     (122)     4872 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/string_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/strings_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/strndup.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/strnlen.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/sysexits.m4
--rw-r--r--   0 runner    (1001) docker     (122)     7190 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/unistd_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)     8091 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/vasnprintf.m4
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/vsnprintf.m4
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/warn-on-use.m4
--rw-r--r--   0 runner    (1001) docker     (122)     5751 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/wchar_h.m4
--rw-r--r--   0 runner    (1001) docker     (122)      747 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/wchar_t.m4
--rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/wint_t.m4
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/build-deps/glm4/xsize.m4
--rwxr-xr-x   0 runner    (1001) docker     (122)      103 2022-12-05 18:58:04.000000 genomedata-1.6.0/src/update_gnulib.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/README
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 18:58:22.000000 genomedata-1.6.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (122)  1411024 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/ENCFF324BPE.bigWig
--rw-r--r--   0 runner    (1001) docker     (122)      270 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/adjacent.agp.gz
--rw-r--r--   0 runner    (1001) docker     (122)    72597 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/assembly_report.txt
--rw-r--r--   0 runner    (1001) docker     (122)      711 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chr1.agp.gz
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chr1.phyloP44way.placental.short.wigFix
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chr1.phyloP44way.primate.short.wigFix
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chr1.phyloP44way.vertebrate.short.wigFix
--rw-r--r--   0 runner    (1001) docker     (122)    25455 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chr1.short.fa
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chr1.wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.wig
--rw-r--r--   0 runner    (1001) docker     (122)      714 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chrY.agp.gz
--rw-r--r--   0 runner    (1001) docker     (122)     6394 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chrY.short.fa.gz
--rw-r--r--   0 runner    (1001) docker     (122)       76 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chunk_test_track1.bed
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/chunk_test_track2.bed
--rw-r--r--   0 runner    (1001) docker     (122)       87 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/filter.bed
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/filter_fixed.wig
--rw-r--r--   0 runner    (1001) docker     (122)      132 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/filter_variable.wig.gz
--rw-r--r--   0 runner    (1001) docker     (122)     9290 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/phyloP44way.placental.short.wigFix
--rw-r--r--   0 runner    (1001) docker     (122)      847 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/test_chunks.agp
--rw-r--r--   0 runner    (1001) docker     (122)      198 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/unfiltered.bed
--rw-r--r--   0 runner    (1001) docker     (122)    42558 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/v0.genomedata
--rw-r--r--   0 runner    (1001) docker     (122)    42558 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/v1.genomedata
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.bed
--rw-r--r--   0 runner    (1001) docker     (122)      112 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.bedGraph
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.dos.bed
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.dos.bedGraph
--rw-r--r--   0 runner    (1001) docker     (122)      214 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.dos.wigVar
--rw-r--r--   0 runner    (1001) docker     (122)      196 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.wigVar
--rwxr-xr-x   0 runner    (1001) docker     (122)     8902 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)    21853 2022-12-05 18:58:04.000000 genomedata-1.6.0/test/test_genomedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:44.000000 genomedata-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-02 18:28:18.000000 genomedata-1.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-02 18:28:18.000000 genomedata-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-08-02 18:28:18.000000 genomedata-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-02 18:28:18.000000 genomedata-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-08-02 18:28:18.000000 genomedata-1.7.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-02 18:28:44.000000 genomedata-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-02 18:28:18.000000 genomedata-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 18:28:18.000000 genomedata-1.7.0/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-08-02 18:28:18.000000 genomedata-1.7.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-02 18:28:18.000000 genomedata-1.7.0/doc/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31312 2023-08-02 18:28:18.000000 genomedata-1.7.0/doc/genomedata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 18:28:18.000000 genomedata-1.7.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 18:28:18.000000 genomedata-1.7.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 18:28:18.000000 genomedata-1.7.0/examples/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-08-02 18:28:18.000000 genomedata-1.7.0/examples/genomedata_fill_random.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-08-02 18:28:18.000000 genomedata-1.7.0/examples/genomedata_offline_random_access.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      741 2023-08-02 18:28:18.000000 genomedata-1.7.0/examples/genomedata_random_access.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 18:28:18.000000 genomedata-1.7.0/examples/genomedata_random_access.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3963 2023-08-02 18:28:18.000000 genomedata-1.7.0/examples/random_genomic_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata/
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_bigwig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_chromosome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_close_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_erase_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_hardmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_hardmask_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_load_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-08-02 18:28:18.000000 genomedata-1.7.0/genomedata/load_genomedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 18:28:43.000000 genomedata-1.7.0/genomedata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-02 18:28:18.000000 genomedata-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 18:28:44.000000 genomedata-1.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3235 2023-08-02 18:28:18.000000 genomedata-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    36482 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/_c_load_data.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/src/build-deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)    34973 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    32689 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/aclocal.m4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:43.000000 genomedata-1.7.0/src/build-deps/build-aux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/arg-nonnull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/c++defs.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43420 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/config.guess
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31743 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/config.sub
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15936 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/depcomp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9233 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/install-sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11014 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/missing
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/build-aux/warn-on-use.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28017 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/config.h.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)   573788 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/configure
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:44.000000 genomedata-1.7.0/src/build-deps/gllib/
+-rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)    69493 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/alloca.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/alloca.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-ba.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-eexst.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-fmtstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-fmtstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-fs-xinl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    63636 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-help.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-namefrob.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31712 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-pin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-pv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-pvh.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp-xinl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    29369 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/argp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/asnprintf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/basename-lgpl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/dirname-lgpl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/dirname.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/errno.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/error.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/float+.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/float.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/getdelim.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/getline.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38984 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/getopt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/getopt.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/getopt1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/getopt_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/gettext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/intprops.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/malloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/memchr.c
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/memchr.valgrind
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/mempcpy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/printf-args.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/printf-args.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21573 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/printf-parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/printf-parse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/progname.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/progname.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/rawmemchr.c
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/rawmemchr.valgrind
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/realloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/size_max.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/sleep.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stdbool.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stddef.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stdint.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stdio-write.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36538 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stdio.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stdlib.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strcasecmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strchrnul.c
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strchrnul.valgrind
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strerror.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35064 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/string.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strings.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/stripslash.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strncasecmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strndup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/strnlen.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/sysexits.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43158 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/unistd.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)   221260 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/vasnprintf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/vasnprintf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/verify.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/vsnprintf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/wchar.in.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/gllib/xsize.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:44.000000 genomedata-1.7.0/src/build-deps/glm4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/00gnulib.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)    25002 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/alloca.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/argp.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/dirname.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/dos.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/double-slash-root.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/errno_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/error.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/extensions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/float_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/getdelim.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/getline.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/getopt.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/gnulib-common.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/include_next.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/intmax_t.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/inttypes_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/longlong.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/malloc.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/memchr.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/mempcpy.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/mmap-anon.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/multiarch.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/onceonly.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    55812 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/printf.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/rawmemchr.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/realloc.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/size_max.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/sleep.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/stdbool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/stddef_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/stdint.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/stdint_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/stdio_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/stdlib_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/strcase.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/strchrnul.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/strerror.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/string_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/strings_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/strndup.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/strnlen.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/sysexits.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/unistd_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/vasnprintf.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/vsnprintf.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/warn-on-use.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/wchar_h.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/wchar_t.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/wint_t.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/build-deps/glm4/xsize.m4
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-08-02 18:28:18.000000 genomedata-1.7.0/src/update_gnulib.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:44.000000 genomedata-1.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:44.000000 genomedata-1.7.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1411024 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/ENCFF324BPE.bigWig
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/adjacent.agp.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    72597 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/assembly_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chr1.agp.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chr1.phyloP44way.placental.short.wigFix
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chr1.phyloP44way.primate.short.wigFix
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chr1.phyloP44way.vertebrate.short.wigFix
+-rw-r--r--   0 runner    (1001) docker     (123)    25455 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chr1.short.fa
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chr1.wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.wig
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chrY.agp.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chrY.short.fa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chunk_test_track1.bed
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/chunk_test_track2.bed
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/filter.bed
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/filter_fixed.wig
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/filter_variable.wig.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/phyloP44way.placental.short.wigFix
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/test_chunks.agp
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/unfiltered.bed
+-rw-r--r--   0 runner    (1001) docker     (123)    42558 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/v0.genomedata
+-rw-r--r--   0 runner    (1001) docker     (123)    42558 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/v1.genomedata
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.bed
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.bedGraph
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.dos.bed
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.dos.bedGraph
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.dos.wigVar
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/data/wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.wigVar
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12322 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21853 2023-08-02 18:28:18.000000 genomedata-1.7.0/test/test_genomedata.py
```

### Comparing `genomedata-1.6.0/CITATION.cff` & `genomedata-1.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/CONTRIBUTING.rst` & `genomedata-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/LICENSE` & `genomedata-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/NEWS` & `genomedata-1.7.0/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+1.7.0:
+* adapted existing python interface to open bigWig files
+
 1.6.0:
 * required Python is now >=3.7
 * genomedata-load-data: changed to a python script with a c-extension
 
 1.5.0:
 * genomedata-load-data: fix bad error message when loading process fails
 * genomedata-load-seq: add chromosome name mapping based on assembly reports
```

### Comparing `genomedata-1.6.0/PKG-INFO` & `genomedata-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomedata
-Version: 1.6.0
+Version: 1.7.0
 Summary: tools for accessing large amounts of genomic data
 Author-email: Michael Hoffman <michael.hoffman@utoronto.ca>
 License: GPL-2.0-only
 Project-URL: Bug Tracker, https://github.com/hoffmangroup/genomedata/issues
 Project-URL: Download, https://pypi.python.org/pypi/genomedata
 Project-URL: Homepage, https://hoffmanlab.org/proj/genomedata
 Classifier: Natural Language :: English
@@ -25,24 +25,25 @@
 
 .. image:: https://img.shields.io/pypi/v/genomedata.png
     :target: https://pypi.python.org/pypi/genomedata/
     :alt: Latest Version
 
 Description
 ===========
-Genomedata is a format for efficient storage of multiple tracks of
-numeric data anchored to a genome. The format allows fast random
-access to hundreds of gigabytes of data, while retaining a small disk
-space footprint. We have also developed utilities to load data into
-this format.
+Genomedata is both a format for efficient storage of multiple tracks of
+numeric data anchored to a genome and a python interface to genomic datasets.
+The file format allows fast random access to hundreds of gigabytes of data, 
+while retaining a small disk space footprint. We have also developed utilities
+to load data into this format.
 
-Specifically, the genomedata package provides access to genome-scale data, using an
-HDF5_ container.
+Specifically, the genomedata package provides access to genome-scale data,
+either using an HDF5_ container or a bigWig_ file.
 
 .. _HDF5: http://www.hdfgroup.org/
+.. _bigWig: http://www.genome.ucsc.edu/goldenPath/help/bigWig.html
 
 Please see the following URL (and linked documentation) for information,
 installation, and support: https://hoffmanlab.org/proj/genomedata/
 
 Documentation
 =============
```

### Comparing `genomedata-1.6.0/README.rst` & `genomedata-1.7.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 .. image:: https://img.shields.io/pypi/v/genomedata.png
     :target: https://pypi.python.org/pypi/genomedata/
     :alt: Latest Version
 
 Description
 ===========
-Genomedata is a format for efficient storage of multiple tracks of
-numeric data anchored to a genome. The format allows fast random
-access to hundreds of gigabytes of data, while retaining a small disk
-space footprint. We have also developed utilities to load data into
-this format.
+Genomedata is both a format for efficient storage of multiple tracks of
+numeric data anchored to a genome and a python interface to genomic datasets.
+The file format allows fast random access to hundreds of gigabytes of data, 
+while retaining a small disk space footprint. We have also developed utilities
+to load data into this format.
 
-Specifically, the genomedata package provides access to genome-scale data, using an
-HDF5_ container.
+Specifically, the genomedata package provides access to genome-scale data,
+either using an HDF5_ container or a bigWig_ file.
 
 .. _HDF5: http://www.hdfgroup.org/
+.. _bigWig: http://www.genome.ucsc.edu/goldenPath/help/bigWig.html
 
 Please see the following URL (and linked documentation) for information,
 installation, and support: https://hoffmanlab.org/proj/genomedata/
 
 Documentation
 =============
```

### Comparing `genomedata-1.6.0/TODO` & `genomedata-1.7.0/TODO`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/doc/Makefile` & `genomedata-1.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/doc/conf.py` & `genomedata-1.7.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-from pkg_resources import get_distribution
+from importlib.metadata import version
 import sys
 
 sys.path.insert(0, "..")
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
@@ -45,17 +45,16 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 
 # The full version, including alpha/beta/rc tags.
-release = get_distribution('genomedata').version
-# Take major.minor.point
-version = '.'.join(release.split('.')[:3])
+release = version('genomedata')
+version = release.rsplit(".", 1)[0]
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `genomedata-1.6.0/doc/genomedata.rst` & `genomedata-1.7.0/doc/genomedata.rst`

 * *Files 2% similar despite different names*

```diff
@@ -96,24 +96,24 @@
           the support_ section.
 
 .. _genomedata-overview:
 
 Overview
 ========
 
-Genomedata provides a way to store and access large-scale functional
-genomics data in a format which is both space-efficient and allows
-efficient random-access. Genomedata archives are currently write-once,
-although we are working to fix this.
+Genomedata is a file format and Python API for accessing  large-scale functional
+genomics data. The file format is both space-efficient and allows efficient random-access.
+The Python API works with Genomedata archives and bigWig files.
 
-Under the surface, Genomedata is :ref:`implemented <Implementation>`
+Under the surface, the Genomedata file format is :ref:`implemented <Implementation>`
 as one or more HDF5 files, but Genomedata provides a transparent
 interface to interact with your underlying data without having to
 worry about the mess of repeatedly parsing large data files or having
 to keep them in memory for random access.
+The Genomedata archives are currently write-once, although we are working to fix this.
 
 The Genomedata hierarchy:
 
   Each :class:`Genome` contains many :class:`Chromosomes <Chromosome>`
     Each :class:`Chromosome` contains many :class:`Supercontigs <Supercontig>`
       Each :class:`Supercontig` contains one ``continuous`` data set
         Each ``continuous`` data set is a numpy.array of floating
@@ -309,19 +309,19 @@
 .. note::
     The Python API expects that a genomedata archive has already been created.
     This can be done manually via the :ref:`genomedata-load` command.
     Alternatively, this can be done programmatically using
     :_load_seq:`load_seq`.
 
 To appreciate the full benefit of Genomedata,
-it is most easily used as a contextmanager::
+it is most easily used as a context manager::
 
     from genomedata import Genome
     [...]
-    gdfilename = "/path/to/genomedata/archive"
+    gdfilename = "/path/to/genomedata/archive" # or bigWig file
     with Genome(gdfilename) as genome:
         [...]
 
 .. note::
     If Genome is used as a context manager, it will clean up any opened
     Chromosomes automatically.
     If not, the Genome object (and all opened chromosomes) should be
@@ -363,14 +363,27 @@
 array([ 47.], dtype=float32)
 
 .. note:: Specify a slice for the track to keep the data in column form:
 
           >>> col_index = chromosome.index_continuous("sample_track")
           >>> data = chromosome[0:5, col_index:col_index+1]
 
+BigWig differences
+------------------
+There are a number of minor differences between using the genomedata file
+format and the bigWig file format:
+
+- There is only one track per bigWig file and it is implicitly set to the
+  filename of the bigWig.
+- Summary statistics are taken from the bigWig file formation definition
+  which are stored as integers. There may be some differences precision.
+- Each :class:`Chromosome <Chromosome>` is represented with 1 underlying
+  :class:`Supercontig <Supercontig>`.
+
+
 Command-line interface
 ~~~~~~~~~~~~~~~~~~~~~~
 
 Genomedata archives can be created and loaded from the command line
 with the :ref:`genomedata-load` command.
 
 .. _genomedata-load:
```

### Comparing `genomedata-1.6.0/doc/make.bat` & `genomedata-1.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/examples/README` & `genomedata-1.7.0/examples/README`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/examples/genomedata_fill_random.py` & `genomedata-1.7.0/examples/genomedata_fill_random.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/examples/genomedata_offline_random_access.py` & `genomedata-1.7.0/examples/genomedata_offline_random_access.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/examples/genomedata_random_access.pl` & `genomedata-1.7.0/examples/genomedata_random_access.pl`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/examples/genomedata_random_access.py` & `genomedata-1.7.0/examples/genomedata_random_access.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/examples/random_genomic_positions.py` & `genomedata-1.7.0/examples/random_genomic_positions.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/__init__.py` & `genomedata-1.7.0/genomedata/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 large data files or having to keep them in memory for random access.
 
 Copyright 2009-2014 Michael M. Hoffman <michael.hoffman@utoronto.ca>
 
 """
 
 
-from functools import partial
 from pkg_resources import get_distribution
 import sys
 
-from numpy import add, amin, amax, square
+from numpy import square
 from path import Path
 
 from ._hdf5 import _HDF5DirectoryChromosomeList, _HDF5SingleFileChromosomeList
+from ._bigwig import _BigWigChromosomeList, is_big_wig
 
 # Allow raising a DistributionNotFound error if somehow genomedata was not
 # installed
 __version__ = get_distribution(__name__.split('.')[0]).version
 
 FORMAT_VERSION = 1
 
@@ -96,18 +96,24 @@
         filepath = Path(filename).expand()
         while filepath.islink():
             filepath = filepath.readlinkabs()
 
         if not filepath.exists():
             raise IOError("Could not find Genomedata archive: %s" % filepath)
 
+        # If it's a file we are opening
         if filepath.isfile():
-            # Open the Genomedata file
-            self._chromosomes = _HDF5SingleFileChromosomeList(filepath, *args,
-                                                              **kwargs)
+            # Check if the file type is bigWig
+            # NB: Could consider checking by filename extension only
+            if is_big_wig(filepath):
+                self._chromosomes = _BigWigChromosomeList(filepath)
+            # Otherwise assume and attempt to open the Genomedata file
+            else:
+                self._chromosomes = _HDF5SingleFileChromosomeList(
+                    filepath, *args, **kwargs)
         elif filepath.isdir():
             # Genomedata directory
             self._chromosomes = _HDF5DirectoryChromosomeList(filepath, *args,
                                                              **kwargs)
         else:
             raise ValueError("Genomedata archive must be file or directory: %s"
                              % filepath)
@@ -232,20 +238,14 @@
         if self.kwargs:
             items.append("**%r" % self.kwargs)
         return "Genome(%s)" % ", ".join(items)
 
     def __str__(self):
         return repr(self)
 
-    def _accum_extrema(self, name, accumulator):
-        self.tracknames_continuous  # for assertion check
-
-        extrema = [getattr(chromosome, name) for chromosome in self]
-        return accumulator(extrema)
-
     def erase_data(self, trackname):
         """Erase all data for the given track across all chromosomes
 
         The Genome object must have been created with
         :param mode:="r+". Behavior is undefined if this is not the case.
 
         Currently sets the dirty bit, which can only be erased with
@@ -319,87 +319,66 @@
         except AttributeError:
             return 0
 
     @property
     def format_version(self):
         """Genomedata format version
 
-        None means there are no chromosomes in it already.
+        None means there are no chromosomes in it already or there is no
+        information available.
         """
         assert self.isopen
-        # Get the Genomedata format version from the HDF5 file configurations
-        try:
-            return self._chromosomes._file_attrs.genomedata_format_version
-        except AttributeError:
-            pass
-
-        # else: assume self is a genomedata directory
-        chromosomes = iter(self)
-        try:
-            first_chromosome = next(chromosomes)
-        except StopIteration:
-            return None
 
-        # Try to get the format version from a chromsome file
-        try:
-            res = first_chromosome._format_version
-
-            assert all(res == chromosome._format_version
-                       for chromosome in chromosomes)
-        # Otherwise assume we have no format version information
-        except AttributeError:
-            return None
-
-        return res
+        return self._chromosomes._format_version()
 
     # XXX: should memoize these with an off-the-shelf decorator
     @property
     def mins(self):
         """Return the minimum value for each track.
 
         :returns: numpy.array
 
         """
-        return self._accum_extrema("mins", partial(amin, axis=0))
+        return self._chromosomes.mins
 
     @property
     def maxs(self):
         """Return a vector of the maximum value for each track.
 
         :returns: numpy.array
 
         """
-        return self._accum_extrema("maxs", partial(amax, axis=0))
+        return self._chromosomes.maxs
 
     @property
     def sums(self):
         """Return a vector of the sum of the values for each track.
 
         :returns: numpy.array
 
         """
-        return self._accum_extrema("sums", add.reduce)
+        return self._chromosomes.sums
 
     @property
     def sums_squares(self):
         """Return a vector of the sum of squared values for each track's data.
 
         :returns: numpy.array
 
         """
-        return self._accum_extrema("sums_squares", add.reduce)
+        return self._chromosomes.sums_squares
 
     @property
     def num_datapoints(self):
         """Return the number of datapoints in each track.
 
         :returns: a numpy.array vector with an entry for each track.
 
         """
-        return self._accum_extrema("num_datapoints", add.reduce)
+        return self._chromosomes.num_datapoints
 
     @property
     def means(self):
         """Return a vector of the mean value of each track.
 
         :returns: numpy.array
```

### Comparing `genomedata-1.6.0/genomedata/_chromosome.py` & `genomedata-1.7.0/genomedata/_chromosome.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from functools import partial
 from operator import attrgetter
 from warnings import warn
 
-from numpy import (array, empty, float32, nan, ndarray, uint8)
+from numpy import (add, amin, amax, array, empty, float32, nan, ndarray,
+                   uint8)
 from six.moves import range
 
 from ._util import OverlapWarning
 
 CONTINUOUS_DTYPE = float32
 
 SEQ_DTYPE = uint8
@@ -484,14 +486,74 @@
         if (name in self.open_chromosomes and
            self.open_chromosomes[name].isopen):  # NB: manual closure check
             # Return cached object
             return self.open_chromosomes[name]
 
         return None
 
+    def _format_version(self):
+        """Get version information metadata. None by default. Subclasses to
+        implement proper versioning if possible"""
+        return None
+
+    def _accum_extrema(self, name, accumulator):
+        self.tracknames_continuous  # for assertion check
+
+        extrema = [getattr(chromosome, name) for chromosome in self]
+        return accumulator(extrema)
+
+    def tracknames_continuous(self):
+        raise NotImplementedError
+
+    # XXX: should memoize these with an off-the-shelf decorator
+    @property
+    def mins(self):
+        """Return the minimum value for each track.
+
+        :returns: numpy.array
+
+        """
+        return self._accum_extrema("mins", partial(amin, axis=0))
+
+    @property
+    def maxs(self):
+        """Return a vector of the maximum value for each track.
+
+        :returns: numpy.array
+
+        """
+        return self._accum_extrema("maxs", partial(amax, axis=0))
+
+    @property
+    def sums(self):
+        """Return a vector of the sum of the values for each track.
+
+        :returns: numpy.array
+
+        """
+        return self._accum_extrema("sums", add.reduce)
+
+    @property
+    def sums_squares(self):
+        """Return a vector of the sum of squared values for each track's data.
+
+        :returns: numpy.array
+
+        """
+        return self._accum_extrema("sums_squares", add.reduce)
+
+    @property
+    def num_datapoints(self):
+        """Return the number of datapoints in each track.
+
+        :returns: a numpy.array vector with an entry for each track.
+
+        """
+        return self._accum_extrema("num_datapoints", add.reduce)
+
     def close(self):
         self.open_chromosomes = {}
 
 
 class Supercontig(object):
     """A container for a segment of data in one chromosome.
```

### Comparing `genomedata-1.6.0/genomedata/_close_data.py` & `genomedata-1.7.0/genomedata/_close_data.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_erase_data.py` & `genomedata-1.7.0/genomedata/_erase_data.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_hardmask.py` & `genomedata-1.7.0/genomedata/_hardmask.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_hardmask_parsers.py` & `genomedata-1.7.0/genomedata/_hardmask_parsers.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_hdf5.py` & `genomedata-1.7.0/genomedata/_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         assert self.isopen
         supercontigs = []
         for group in self.h5group:
             supercontig = _HDF5Supercontig(group)
             supercontigs.append((supercontig.start, supercontig))
 
         supercontigs.sort()
-        for start, supercontig in supercontigs:
+        for _start, supercontig in supercontigs:
             yield supercontig
 
     def close(self):
         if self.attrs.dirty:
             warn("Closing Chromosome with modified data. Metadata needs to"
                  " be recalculated by calling genomedata-close-data on the"
                  " Genomedata archive before re-accessing it",
@@ -302,14 +302,35 @@
             except IOError:
                 raise KeyError("Could not find chromosome: %s" % name)
 
             self.open_chromosomes[name] = res
 
         return res
 
+    def _format_version(self):
+        res = None
+        chromosomes = iter(self)
+
+        try:
+            first_chromosome = next(chromosomes)
+        except StopIteration:
+            return res
+
+        # Try to get the format version from a chromsome file
+        try:
+            res = first_chromosome._format_version
+
+            assert all(res == chromosome._format_version
+                       for chromosome in chromosomes)
+        # Otherwise assume we have no format version information
+        except AttributeError:
+            return res
+
+        return res
+
     def tracknames_continuous(self):
         # check that all chromosomes have the same tracknames_continuous
         res = None
         for chromosome in self:
             if res is None:
                 res = chromosome.tracknames_continuous
             else:
@@ -359,14 +380,21 @@
                 res = _HDF5FileChromosome(self.h5file, where="/" + name)
             except tables.NoSuchNodeError:
                 raise KeyError("Could not find chromosome: %s" % name)
             self.open_chromosomes[name] = res
 
         return res
 
+    def _format_version(self):
+        # Get the Genomedata format version from the HDF5 file configurations
+        try:
+            return self._file_attrs.genomedata_format_version
+        except AttributeError:
+            return None
+
     def add_trackname(self, trackname):
         _hdf5_add_trackname(self.h5file, trackname)
 
     def tracknames_continuous(self):
         # Tracknames are stored at the root of each file, so we can
         # access them directly in this case
         return [decode_trackname(trackname)
```

### Comparing `genomedata-1.6.0/genomedata/_histogram.py` & `genomedata-1.7.0/genomedata/_histogram.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_info.py` & `genomedata-1.7.0/genomedata/_info.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_load_data.py` & `genomedata-1.7.0/genomedata/_load_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 from __future__ import absolute_import, division, print_function
 
 """
 _load_data.py: A python interface for both genomedata_load_data.c and
 load_genomedata.py
 """
 
-import struct
 import sys
 
 from argparse import ArgumentParser
 from subprocess import PIPE, Popen
 
 from . import __version__
+from ._bigwig import is_big_wig
 from ._c_load_data import load_data_from_stdin
 from ._util import SUFFIX_GZ, die
 
-BIG_WIG_SIGNATURE = 0x888FFC26
-BIG_WIG_SIGNATURE_BYTE_SIZE = 4
 BIG_WIG_READ_CMD = "bigWigToBedGraph"
 BEDTOOLS_CMD = "bedtools"
 BEDTOOLS_INTERSECT_CMD = "intersect"
 BEDTOOLS_STDIN = "stdin"
 DEFAULT_CHUNK_SIZE = 10000
 LOAD_DATA_CMD = "genomedata-load-data"
 MSG_LOAD_ERROR = ("Error loading data from track file %%s. " +
@@ -120,32 +118,14 @@
     loader_input_process.communicate()
     retcodes = [loader_input_process.poll()]
     retcodes.append(loader.poll())
     if any(retcodes):
         die(MSG_LOAD_ERROR % (datafile, retcodes))
 
 
-def is_big_wig(filename):
-    """ Checks that the given filename refers to a valid bigWig file """
-    with open(filename, "rb") as big_wig_file:
-        signature_string = big_wig_file.read(BIG_WIG_SIGNATURE_BYTE_SIZE)
-
-    # unpack returns a tuple regardless of length
-    # the kent reference checks both little endian and big endian packing
-    # of the 4 byte signature
-    little_endian_signature = struct.unpack("<L", signature_string)[0]
-    big_endian_signature = struct.unpack(">L", signature_string)[0]
-
-    if (little_endian_signature == BIG_WIG_SIGNATURE or
-       big_endian_signature == BIG_WIG_SIGNATURE):
-        return True
-
-    return False
-
-
 def parse_args(args):
 
     description = ("Load data into genomedata format. "
                    "Takes track data in on stdin")
 
     parser = ArgumentParser(description=description,
                             prog='genomedata-load-data')
```

### Comparing `genomedata-1.6.0/genomedata/_load_seq.py` & `genomedata-1.7.0/genomedata/_load_seq.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_open_data.py` & `genomedata-1.7.0/genomedata/_open_data.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_query.py` & `genomedata-1.7.0/genomedata/_query.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_report.py` & `genomedata-1.7.0/genomedata/_report.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/_util.py` & `genomedata-1.7.0/genomedata/_util.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata/load_genomedata.py` & `genomedata-1.7.0/genomedata/load_genomedata.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/genomedata.egg-info/PKG-INFO` & `genomedata-1.7.0/genomedata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomedata
-Version: 1.6.0
+Version: 1.7.0
 Summary: tools for accessing large amounts of genomic data
 Author-email: Michael Hoffman <michael.hoffman@utoronto.ca>
 License: GPL-2.0-only
 Project-URL: Bug Tracker, https://github.com/hoffmangroup/genomedata/issues
 Project-URL: Download, https://pypi.python.org/pypi/genomedata
 Project-URL: Homepage, https://hoffmanlab.org/proj/genomedata
 Classifier: Natural Language :: English
@@ -25,24 +25,25 @@
 
 .. image:: https://img.shields.io/pypi/v/genomedata.png
     :target: https://pypi.python.org/pypi/genomedata/
     :alt: Latest Version
 
 Description
 ===========
-Genomedata is a format for efficient storage of multiple tracks of
-numeric data anchored to a genome. The format allows fast random
-access to hundreds of gigabytes of data, while retaining a small disk
-space footprint. We have also developed utilities to load data into
-this format.
+Genomedata is both a format for efficient storage of multiple tracks of
+numeric data anchored to a genome and a python interface to genomic datasets.
+The file format allows fast random access to hundreds of gigabytes of data, 
+while retaining a small disk space footprint. We have also developed utilities
+to load data into this format.
 
-Specifically, the genomedata package provides access to genome-scale data, using an
-HDF5_ container.
+Specifically, the genomedata package provides access to genome-scale data,
+either using an HDF5_ container or a bigWig_ file.
 
 .. _HDF5: http://www.hdfgroup.org/
+.. _bigWig: http://www.genome.ucsc.edu/goldenPath/help/bigWig.html
 
 Please see the following URL (and linked documentation) for information,
 installation, and support: https://hoffmanlab.org/proj/genomedata/
 
 Documentation
 =============
```

### Comparing `genomedata-1.6.0/genomedata.egg-info/SOURCES.txt` & `genomedata-1.7.0/genomedata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 examples/README
 examples/genomedata_fill_random.py
 examples/genomedata_offline_random_access.py
 examples/genomedata_random_access.pl
 examples/genomedata_random_access.py
 examples/random_genomic_positions.py
 genomedata/__init__.py
+genomedata/_bigwig.py
 genomedata/_chromosome.py
 genomedata/_close_data.py
 genomedata/_erase_data.py
 genomedata/_hardmask.py
 genomedata/_hardmask_parsers.py
 genomedata/_hdf5.py
 genomedata/_histogram.py
```

### Comparing `genomedata-1.6.0/genomedata.egg-info/entry_points.txt` & `genomedata-1.7.0/genomedata.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/pyproject.toml` & `genomedata-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # https://bitbucket.org/hoffmanlab/genomedata/issues/38/pytables-341-causes-a-core-dump-when
 dependencies = [
   "numpy",
   "tables>=3.0,!=3.4.1",
   "six",
   "textinput>=0.2.0",
   "path.py>=11",
+  "pybigwig",
 ]
 description = "tools for accessing large amounts of genomic data"
 dynamic = ["version"]
 name = "genomedata"
 readme = "README.rst"
 requires-python = ">=3.7"
```

### Comparing `genomedata-1.6.0/setup.py` & `genomedata-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/_c_load_data.c` & `genomedata-1.7.0/src/_c_load_data.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/Makefile.in` & `genomedata-1.7.0/src/build-deps/Makefile.in`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/aclocal.m4` & `genomedata-1.7.0/src/build-deps/aclocal.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/arg-nonnull.h` & `genomedata-1.7.0/src/build-deps/build-aux/arg-nonnull.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/c++defs.h` & `genomedata-1.7.0/src/build-deps/build-aux/c++defs.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/config.guess` & `genomedata-1.7.0/src/build-deps/build-aux/config.guess`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/config.sub` & `genomedata-1.7.0/src/build-deps/build-aux/config.sub`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/depcomp` & `genomedata-1.7.0/src/build-deps/build-aux/depcomp`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/install-sh` & `genomedata-1.7.0/src/build-deps/build-aux/install-sh`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/missing` & `genomedata-1.7.0/src/build-deps/build-aux/missing`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/build-aux/warn-on-use.h` & `genomedata-1.7.0/src/build-deps/build-aux/warn-on-use.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/config.h.in` & `genomedata-1.7.0/src/build-deps/config.h.in`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/configure` & `genomedata-1.7.0/src/build-deps/configure`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/configure.ac` & `genomedata-1.7.0/src/build-deps/configure.ac`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/Makefile.am` & `genomedata-1.7.0/src/build-deps/gllib/Makefile.am`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/Makefile.in` & `genomedata-1.7.0/src/build-deps/gllib/Makefile.in`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/alloca.c` & `genomedata-1.7.0/src/build-deps/gllib/alloca.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/alloca.in.h` & `genomedata-1.7.0/src/build-deps/gllib/alloca.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-ba.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-ba.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-eexst.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-eexst.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-fmtstream.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-fmtstream.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-fmtstream.h` & `genomedata-1.7.0/src/build-deps/gllib/argp-fmtstream.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-fs-xinl.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-fs-xinl.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-help.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-help.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-namefrob.h` & `genomedata-1.7.0/src/build-deps/gllib/argp-namefrob.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-parse.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-parse.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-pin.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-pin.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-pv.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-pv.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-pvh.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-pvh.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp-xinl.c` & `genomedata-1.7.0/src/build-deps/gllib/argp-xinl.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/argp.h` & `genomedata-1.7.0/src/build-deps/gllib/argp.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/asnprintf.c` & `genomedata-1.7.0/src/build-deps/gllib/asnprintf.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/basename-lgpl.c` & `genomedata-1.7.0/src/build-deps/gllib/basename-lgpl.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/dirname-lgpl.c` & `genomedata-1.7.0/src/build-deps/gllib/dirname-lgpl.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/dirname.h` & `genomedata-1.7.0/src/build-deps/gllib/dirname.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/errno.in.h` & `genomedata-1.7.0/src/build-deps/gllib/errno.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/error.c` & `genomedata-1.7.0/src/build-deps/gllib/error.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/error.h` & `genomedata-1.7.0/src/build-deps/gllib/error.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/float+.h` & `genomedata-1.7.0/src/build-deps/gllib/float+.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/float.in.h` & `genomedata-1.7.0/src/build-deps/gllib/float.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/getdelim.c` & `genomedata-1.7.0/src/build-deps/gllib/getdelim.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/getline.c` & `genomedata-1.7.0/src/build-deps/gllib/getline.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/getopt.c` & `genomedata-1.7.0/src/build-deps/gllib/getopt.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/getopt.in.h` & `genomedata-1.7.0/src/build-deps/gllib/getopt.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/getopt1.c` & `genomedata-1.7.0/src/build-deps/gllib/getopt1.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/getopt_int.h` & `genomedata-1.7.0/src/build-deps/gllib/getopt_int.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/gettext.h` & `genomedata-1.7.0/src/build-deps/gllib/gettext.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/intprops.h` & `genomedata-1.7.0/src/build-deps/gllib/intprops.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/malloc.c` & `genomedata-1.7.0/src/build-deps/gllib/malloc.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/memchr.c` & `genomedata-1.7.0/src/build-deps/gllib/memchr.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/mempcpy.c` & `genomedata-1.7.0/src/build-deps/gllib/mempcpy.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/printf-args.c` & `genomedata-1.7.0/src/build-deps/gllib/printf-args.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/printf-args.h` & `genomedata-1.7.0/src/build-deps/gllib/printf-args.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/printf-parse.c` & `genomedata-1.7.0/src/build-deps/gllib/printf-parse.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/printf-parse.h` & `genomedata-1.7.0/src/build-deps/gllib/printf-parse.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/progname.c` & `genomedata-1.7.0/src/build-deps/gllib/progname.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/progname.h` & `genomedata-1.7.0/src/build-deps/gllib/progname.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/rawmemchr.c` & `genomedata-1.7.0/src/build-deps/gllib/rawmemchr.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/realloc.c` & `genomedata-1.7.0/src/build-deps/gllib/realloc.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/size_max.h` & `genomedata-1.7.0/src/build-deps/gllib/size_max.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/sleep.c` & `genomedata-1.7.0/src/build-deps/gllib/sleep.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stdbool.in.h` & `genomedata-1.7.0/src/build-deps/gllib/stdbool.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stddef.in.h` & `genomedata-1.7.0/src/build-deps/gllib/stddef.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stdint.in.h` & `genomedata-1.7.0/src/build-deps/gllib/stdint.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stdio-write.c` & `genomedata-1.7.0/src/build-deps/gllib/stdio-write.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stdio.in.h` & `genomedata-1.7.0/src/build-deps/gllib/stdio.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stdlib.in.h` & `genomedata-1.7.0/src/build-deps/gllib/stdlib.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strcasecmp.c` & `genomedata-1.7.0/src/build-deps/gllib/strcasecmp.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strchrnul.c` & `genomedata-1.7.0/src/build-deps/gllib/strchrnul.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strerror.c` & `genomedata-1.7.0/src/build-deps/gllib/strerror.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/string.in.h` & `genomedata-1.7.0/src/build-deps/gllib/string.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strings.in.h` & `genomedata-1.7.0/src/build-deps/gllib/strings.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/stripslash.c` & `genomedata-1.7.0/src/build-deps/gllib/stripslash.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strncasecmp.c` & `genomedata-1.7.0/src/build-deps/gllib/strncasecmp.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strndup.c` & `genomedata-1.7.0/src/build-deps/gllib/strndup.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/strnlen.c` & `genomedata-1.7.0/src/build-deps/gllib/strnlen.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/sysexits.in.h` & `genomedata-1.7.0/src/build-deps/gllib/sysexits.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/unistd.in.h` & `genomedata-1.7.0/src/build-deps/gllib/unistd.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/vasnprintf.c` & `genomedata-1.7.0/src/build-deps/gllib/vasnprintf.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/vasnprintf.h` & `genomedata-1.7.0/src/build-deps/gllib/vasnprintf.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/verify.h` & `genomedata-1.7.0/src/build-deps/gllib/verify.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/vsnprintf.c` & `genomedata-1.7.0/src/build-deps/gllib/vsnprintf.c`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/wchar.in.h` & `genomedata-1.7.0/src/build-deps/gllib/wchar.in.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/gllib/xsize.h` & `genomedata-1.7.0/src/build-deps/gllib/xsize.h`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/00gnulib.m4` & `genomedata-1.7.0/src/build-deps/glm4/00gnulib.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/Makefile.am` & `genomedata-1.7.0/src/build-deps/glm4/Makefile.am`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/Makefile.in` & `genomedata-1.7.0/src/build-deps/glm4/Makefile.in`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/alloca.m4` & `genomedata-1.7.0/src/build-deps/glm4/alloca.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/argp.m4` & `genomedata-1.7.0/src/build-deps/glm4/argp.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/dirname.m4` & `genomedata-1.7.0/src/build-deps/glm4/dirname.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/dos.m4` & `genomedata-1.7.0/src/build-deps/glm4/dos.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/double-slash-root.m4` & `genomedata-1.7.0/src/build-deps/glm4/double-slash-root.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/errno_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/errno_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/error.m4` & `genomedata-1.7.0/src/build-deps/glm4/error.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/extensions.m4` & `genomedata-1.7.0/src/build-deps/glm4/extensions.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/float_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/float_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/getdelim.m4` & `genomedata-1.7.0/src/build-deps/glm4/getdelim.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/getline.m4` & `genomedata-1.7.0/src/build-deps/glm4/getline.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/getopt.m4` & `genomedata-1.7.0/src/build-deps/glm4/getopt.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/gnulib-common.m4` & `genomedata-1.7.0/src/build-deps/glm4/gnulib-common.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/include_next.m4` & `genomedata-1.7.0/src/build-deps/glm4/include_next.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/intmax_t.m4` & `genomedata-1.7.0/src/build-deps/glm4/intmax_t.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/inttypes_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/inttypes_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/longlong.m4` & `genomedata-1.7.0/src/build-deps/glm4/longlong.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/malloc.m4` & `genomedata-1.7.0/src/build-deps/glm4/malloc.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/memchr.m4` & `genomedata-1.7.0/src/build-deps/glm4/memchr.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/mempcpy.m4` & `genomedata-1.7.0/src/build-deps/glm4/mempcpy.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/mmap-anon.m4` & `genomedata-1.7.0/src/build-deps/glm4/mmap-anon.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/multiarch.m4` & `genomedata-1.7.0/src/build-deps/glm4/multiarch.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/onceonly.m4` & `genomedata-1.7.0/src/build-deps/glm4/onceonly.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/printf.m4` & `genomedata-1.7.0/src/build-deps/glm4/printf.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/rawmemchr.m4` & `genomedata-1.7.0/src/build-deps/glm4/rawmemchr.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/realloc.m4` & `genomedata-1.7.0/src/build-deps/glm4/realloc.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/size_max.m4` & `genomedata-1.7.0/src/build-deps/glm4/size_max.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/sleep.m4` & `genomedata-1.7.0/src/build-deps/glm4/sleep.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/stdbool.m4` & `genomedata-1.7.0/src/build-deps/glm4/stdbool.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/stddef_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/stddef_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/stdint.m4` & `genomedata-1.7.0/src/build-deps/glm4/stdint.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/stdint_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/stdint_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/stdio_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/stdio_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/stdlib_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/stdlib_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/strcase.m4` & `genomedata-1.7.0/src/build-deps/glm4/strcase.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/strchrnul.m4` & `genomedata-1.7.0/src/build-deps/glm4/strchrnul.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/strerror.m4` & `genomedata-1.7.0/src/build-deps/glm4/strerror.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/string_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/string_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/strings_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/strings_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/strndup.m4` & `genomedata-1.7.0/src/build-deps/glm4/strndup.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/strnlen.m4` & `genomedata-1.7.0/src/build-deps/glm4/strnlen.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/sysexits.m4` & `genomedata-1.7.0/src/build-deps/glm4/sysexits.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/unistd_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/unistd_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/vasnprintf.m4` & `genomedata-1.7.0/src/build-deps/glm4/vasnprintf.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/vsnprintf.m4` & `genomedata-1.7.0/src/build-deps/glm4/vsnprintf.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/warn-on-use.m4` & `genomedata-1.7.0/src/build-deps/glm4/warn-on-use.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/wchar_h.m4` & `genomedata-1.7.0/src/build-deps/glm4/wchar_h.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/wchar_t.m4` & `genomedata-1.7.0/src/build-deps/glm4/wchar_t.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/src/build-deps/glm4/wint_t.m4` & `genomedata-1.7.0/src/build-deps/glm4/wint_t.m4`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/ENCFF324BPE.bigWig` & `genomedata-1.7.0/test/data/ENCFF324BPE.bigWig`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/assembly_report.txt` & `genomedata-1.7.0/test/data/assembly_report.txt`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chr1.agp.gz` & `genomedata-1.7.0/test/data/chr1.agp.gz`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chr1.phyloP44way.placental.short.wigFix` & `genomedata-1.7.0/test/data/chr1.phyloP44way.placental.short.wigFix`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chr1.phyloP44way.primate.short.wigFix` & `genomedata-1.7.0/test/data/chr1.phyloP44way.primate.short.wigFix`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chr1.phyloP44way.vertebrate.short.wigFix` & `genomedata-1.7.0/test/data/chr1.phyloP44way.vertebrate.short.wigFix`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chr1.short.fa` & `genomedata-1.7.0/test/data/chr1.short.fa`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chr1.wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.wig` & `genomedata-1.7.0/test/data/chr1.wgEncodeDukeDNaseSeqBaseOverlapSignalK562V2.wig`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chrY.agp.gz` & `genomedata-1.7.0/test/data/chrY.agp.gz`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/chrY.short.fa.gz` & `genomedata-1.7.0/test/data/chrY.short.fa.gz`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/phyloP44way.placental.short.wigFix` & `genomedata-1.7.0/test/data/phyloP44way.placental.short.wigFix`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/test_chunks.agp` & `genomedata-1.7.0/test/data/test_chunks.agp`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/v0.genomedata` & `genomedata-1.7.0/test/data/v0.genomedata`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/data/v1.genomedata` & `genomedata-1.7.0/test/data/v1.genomedata`

 * *Files identical despite different names*

### Comparing `genomedata-1.6.0/test/run_tests.py` & `genomedata-1.7.0/test/run_tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 
 from __future__ import absolute_import, division, print_function
 
+from math import isnan
 import os
 from os import chdir, remove
 import subprocess
 import unittest
 
+from numpy import nan
 from path import Path
 
 from genomedata._load_seq import load_seq
 from genomedata._close_data import close_data
 from genomedata.load_genomedata import load_genomedata
 from genomedata import Genome
 
@@ -263,14 +265,102 @@
         self.assertIn("chr1", chromosome_names)
         self.assertIn("chrY", chromosome_names)
 
     def tearDown(self):
         remove(self.genomedata_name)
 
 
+class GenomedataBigWigTester(unittest.TestCase):
+    def setUp(self):
+        self.bigwig_name = test_data_path("ENCFF324BPE.bigWig")
+
+    def test_interface(self):
+        with Genome(self.bigwig_name) as genome:
+            # TODO: Genome interface testing
+
+            # Test sorted order of chromosomes
+            chr_names = [chromosome.name for chromosome in genome]
+            self.assertListEqual(chr_names, sorted(chr_names))
+
+            # Test chromosome attrbutes
+            self.assertTrue("chr1" in genome)
+            self.assertFalse("chrY" in genome)
+
+            # Test for no format version
+            self.assertTrue(genome.format_version is None)
+
+            # Test genome is open
+            self.assertTrue(genome.isopen)
+
+            # Test failure for attempting to erase data
+            with self.assertRaises(NotImplementedError):
+                genome.erase_data(self.bigwig_name)
+
+            # Test for trackname "list"
+            self.assertListEqual(genome.tracknames_continuous,
+                                 [self.bigwig_name])
+
+            self.assertEqual(genome.num_datapoints, [3088137])
+            self.assertEqual(genome.mins, [0])
+            self.assertEqual(genome.maxs, [93473])
+            self.assertEqual(genome.sums, [32720078])
+            self.assertEqual(genome.sums_squares, [1280737190372])
+            self.assertAlmostEqual(genome.vars, 414615.8372, places=4)
+
+            # Test chromosome retrieval
+            chr1 = genome["chr1"]  # memoization
+
+            # Chromosome interface testing
+            # chr1	569800	569801	0.01108
+            # chr1	569801	569829	0.02215
+
+            self.assertAlmostEqualList(
+                chr1[569798:569802],
+                [nan, nan, 0.01108, 0.02215],
+                places=5  # NB: Number of original input decimal places
+            )
+
+            # Test the trackname is implictly the filename
+            self.assertEqual(self.bigwig_name, chr1.tracknames_continuous[0])
+
+            # Test chromosome attributes
+            self.assertEqual(chr1.start, 569800)
+            self.assertEqual(chr1.end, 249200695)
+
+            # Test sequence data should error
+            with self.assertRaises(NotImplementedError):
+                _ = chr1.seq[0:20]
+
+            # Test entire Supercontig interface
+            # Get first (and only) supercontig
+            for supercontig in chr1:
+                break
+
+            # Slice indexing
+            self.assertAlmostEqualList(supercontig.continuous[1:2],
+                                       [0.02215, 0.02215],
+                                       places=5)
+            # Single indexing
+            self.assertAlmostEqualList(supercontig.continuous[0], [0.01108],
+                                       places=5)
+
+    def assertAlmostEqualList(self, first, second, places=1):
+        """ Compares floating point numbers in a list based on decimal places.
+        Does not apply to nans """
+
+        for first_elem, second_elem in zip(first, second):
+            # NB: NaN values are never considered equal
+            is_first_nan = isnan(first_elem)
+            is_second_nan = isnan(second_elem)
+            if is_first_nan or is_second_nan:
+                self.assertTrue(is_first_nan and is_second_nan)
+            else:
+                self.assertAlmostEqual(first_elem, second_elem, places)
+
+
 def main():
     dirpath = Path(__file__).dirname()
     if dirpath:
         chdir(dirpath)
 
     unittest.main()
```

### Comparing `genomedata-1.6.0/test/test_genomedata.py` & `genomedata-1.7.0/test/test_genomedata.py`

 * *Files identical despite different names*

