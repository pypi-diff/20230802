# Comparing `tmp/openlane-2.0.0a9.tar.gz` & `tmp/openlane-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.0a9.tar", last modified: Tue Mar 28 20:05:45 2023, max compression
+gzip compressed data, was "openlane-2.0.0b1.tar", last modified: Wed Aug  2 04:24:58 2023, max compression
```

## Comparing `openlane-2.0.0a9.tar` & `openlane-2.0.0b1.tar`

### file list

```diff
@@ -1,146 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.087321 openlane-2.0.0a9/
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-28 20:05:45.087321 openlane-2.0.0a9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.075321 openlane-2.0.0a9/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/tcleval.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/env_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/optimizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/open_pdks_rev
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/base.sdc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/klayout/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/Readme.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2681 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/open_design.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4581 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/render.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6482 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/stream_out.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/xor.drc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/def/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2699 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/mag_gds.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/read.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/drc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/extract_spice.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/gds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/drc_batch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/erase_box.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/extras_mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/mag_with_pointers.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/read.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/lef/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/lef/extras_maglef.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/lef/maglef.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/mag/
--rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/mag/lef.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/odbpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/apply_def_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/defutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/diodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/io_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/label_macro_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/lefutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/manual_macro_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/padringer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39971 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/power_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/random_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/remove_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/snap_to_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/wire_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/openroad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      741 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/basic_mp.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/check_antennae.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/openroad/common/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/dpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/dpl_cell_pad.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/io.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/pdn_cfg.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/resizer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_global_connections.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_layer_adjustments.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_power_nets.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_rc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_routing_layers.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/cts.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/dpl.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/drt.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/fill.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/floorplan.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/gpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/insert_buffer.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1635 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/ioplacer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/irdrop.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/pdn.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/rcx.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/repair_design.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postcts.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postgrt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/sta.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     8648 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/sta_multi_corner.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/tapcell.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/write_views.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/tclsh/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/tclsh/hello.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/yosys/
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/yosys/synthesize.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/smoke_test_design/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/smoke_test_design/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/smoke_test_design/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/smoke_test_design/src/spm.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/state/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/state/design_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.087321 openlane-2.0.0a9/openlane/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/common_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/klayout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/netgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/odb.py
--rw-r--r--   0 runner    (1001) docker     (123)    35320 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/openroad.py
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/tclstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/yosys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.087321 openlane-2.0.0a9/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/drc.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 20:05:45.087321 openlane-2.0.0a9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-03-28 19:59:10.000000 openlane-2.0.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.732571 openlane-2.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-08-02 04:24:58.732571 openlane-2.0.0b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.708571 openlane-2.0.0b1/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.712571 openlane-2.0.0b1/openlane/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/generic_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/common/test_tcl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.712571 openlane-2.0.0b1/openlane/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27479 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/test_pdk_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/test_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20441 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/config/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/env_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/optimizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/flows/test_sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/open_pdks_rev
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/base.sdc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/scripts/klayout/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/klayout/Readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/klayout/open_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4670 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/klayout/render.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6512 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/klayout/stream_out.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/klayout/xor.drc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/scripts/magic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/scripts/magic/def/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/def/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/def/mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2740 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/def/mag_gds.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/def/read.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/drc.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/extract_spice.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.716570 openlane-2.0.0b1/openlane/scripts/magic/gds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/gds/drc_batch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/gds/erase_box.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/gds/extras_mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/gds/mag_with_pointers.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/gds/read.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.720571 openlane-2.0.0b1/openlane/scripts/magic/lef/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/lef/extras_maglef.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/lef/maglef.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/lef.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/magic/wrapper.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.720571 openlane-2.0.0b1/openlane/scripts/odbpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/apply_def_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/defutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/diodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/disconnected_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/io_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/label_macro_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/lefutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/manual_macro_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/padringer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/power_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/random_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/remove_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/set_power_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/snap_to_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/odbpy/wire_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.724571 openlane-2.0.0b1/openlane/scripts/openroad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/basic_mp.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/check_antennas.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/scripts/openroad/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/dpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/dpl_cell_pad.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/io.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/pdn_cfg.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/resizer.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/set_global_connections.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/set_layer_adjustments.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/set_power_nets.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/set_rc.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/common/set_routing_layers.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/cts.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/dpl.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/drt.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/fill.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3636 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/floorplan.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/gpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/insert_buffer.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/ioplacer.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/irdrop.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/pdn.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/rcx.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/repair_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/rsz_timing_postcts.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/rsz_timing_postgrt.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/scripts/openroad/sta/
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/sta/corner.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/sta/multi_corner.tcl.bk
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/tapcell.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/openroad/write_views.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/scripts/tclsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/tclsh/hello.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/scripts/yosys/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/yosys/common.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/yosys/json_header.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/scripts/yosys/synthesize.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/smoke_test_design/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/smoke_test_design/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/smoke_test_design/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/smoke_test_design/src/spm.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.728571 openlane-2.0.0b1/openlane/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/state/design_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/state/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/state/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.732571 openlane-2.0.0b1/openlane/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/common_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/netgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54794 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/openroad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/test_tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/steps/yosys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.732571 openlane-2.0.0b1/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/utils/drc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/utils/test_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-08-02 04:21:58.000000 openlane-2.0.0b1/openlane/utils/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:24:58.712571 openlane-2.0.0b1/openlane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-08-02 04:24:58.000000 openlane-2.0.0b1/openlane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-08-02 04:24:58.000000 openlane-2.0.0b1/openlane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:24:58.000000 openlane-2.0.0b1/openlane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 04:24:58.000000 openlane-2.0.0b1/openlane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 04:24:58.000000 openlane-2.0.0b1/openlane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 04:24:58.000000 openlane-2.0.0b1/openlane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:24:58.732571 openlane-2.0.0b1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1482 2023-08-02 04:21:58.000000 openlane-2.0.0b1/setup.py
```

### Comparing `openlane-2.0.0a9/PKG-INFO` & `openlane-2.0.0b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0a9
+Version: 2.0.0b1
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > Efabless OpenLane 2 is in early access and all APIs are, presently, highly unstable and subject to change without notice.
         >
-        > If you don't know why you're here, you're probably looking for the stable version of OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
+        > If you *don't* know why you're here, you're probably looking for the stable version of OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
         
         <h1 align="center">OpenLane</h1>
         <p align="center">
             <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0"/></a>
             <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 or higher" /></a>
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style: black"/></a>
             <a href="https://mypy-lang.org/"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" alt="Checked with mypy"/></a>
@@ -21,20 +21,22 @@
         <p align="center">
             <a href="https://openlane2.readthedocs.io/"><img src="https://readthedocs.org/projects/openlane2/badge/?version=latest" alt="Documentation Build Status Badge"/></a>
             <a href="https://invite.skywater.tools"><img src="https://img.shields.io/badge/Community-Open%20Source%20Silicon%20Slack-ff69b4?logo=slack" alt="Invite to the Open Source Silicon Slack"/></a>
         </p>
         
         OpenLane is a RTL to GDSII infrastructure library based on several components including OpenROAD, Yosys, Magic, Netgen, CVC, KLayout and a number of custom scripts for design exploration and optimization. A reference flow performs all ASIC implementation steps from RTL all the way down to GDSII.
         
+        You can find the documentation [here](https://openlane2.readthedocs.io/en/latest/getting_started/) to get started.
+        
         ```python
-        from openlane import Flow
+        from openlane.flows import Flow
         
-        Classic = Flow.get("Classic")
+        Classic = Flow.factory.get("Classic")
         
-        flow = Classic.init_with_config(
+        flow = Classic(
             {
                 "PDK": "sky130A",
                 "DESIGN_NAME": "spm",
                 "VERILOG_FILES": ["./src/spm.v"],
                 "CLOCK_PORT": "clk",
                 "CLOCK_PERIOD": 10,
             },
@@ -42,75 +44,73 @@
         )
         
         flow.start()
         ```
         
         
         ## Installation
-        ### Binary Dependencies
         You'll need the following:
         * Python **3.8** or higher with PIP, Venv and Tkinter
-        * Yosys 0.23+ (preferably 0.26+) from https://github.com/YosysHQ/Yosys
-        * A reasonably modern version of OpenROAD from https://github.com/The-OpenROAD-Project/OpenROAD
-        * A reasonably modern version of Magic from https://github.com/RTimothyEdwards/Magic
-        * A reasonably modern version of Netgen from https://github.com/RTimothyEdwards/netgen
-        * KLayout 0.28.5+ from https://github.com/KLayout/klayout
         
-        ### Docker
-        Works for Windows, macOS and Linux. Easier to set up, but less integrated with your filesystem. Recommended for general users.
+        ### Nix (Recommended)
+        Works for macOS and Linux (x86-64). Recommended, as it is more integrated with your filesystem and overall has less upload and download deltas.
         
-        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/docker_installation/index.html) in the docs.
+        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html) in the docs.
         
-        ### Nix
-        Works for macOS and Linux. A bit more complex to set up, but more integrated with your filesystem and overall less upload and download deltas.
+        ### Docker
+        Works for Windows, macOS and Linux (x86-64, aarch64 with emulation).
         
-        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html) in the docs.
+        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/docker_installation/index.html) in the docs.
         
-        ### Conda
-        TBA
+        Do note you'll need to add `--dockerized` right after `openlane` in most CLI invocations.
         
-        ### Python-only Installation
-        You'll need to bring your own compiled tools, but otherwise, simply install OpenLane as follows:
+        ### Python-only Installation (Advanced)
+        You'll need to bring your own compiled utilities, but otherwise, simply install OpenLane as follows:
         
         ```sh
         python3 -m pip install --upgrade openlane
         ```
         
-        To quickly test your installation, run `openlane --smoke-test`. This may take up to 10 minutes depending on your computer's speed and internet connection.
-        
-        #### Troubleshooting
-        With a typical Python 3.8 or higher installation with PIP, installing OpenLane is usually as simple as a `pip install`.
-        
-        ***Despite that***, there are some peculiarities with PIP itself: For example, you may see a warning among these lines:
+        ## Usage
+        In the root folder of the repository, you may invoke:
         
         ```sh
-          WARNING: The script openlane is installed in '/home/test/.local/bin' which is not on PATH.
-          Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+        python3 -m openlane --pdk-root <path/to/pdk> </path/to/config.json>
         ```
         
-        The solution is as simple as adding something like this to your shell's profile:
+        To start with, you can try:
         
         ```sh
-        export PATH="/home/test/.local/bin:$PATH"
+        python3 -m openlane --pdk-root $HOME/.volare ./designs/spm/config.json
         ```
         
-        Do note that the path (`/home/test/.local/bin` in this example) varies depending on your operating system and version of Python you install, and whether you use `sudo` (absolutely not recommended) or not, so ensure that you actually read the warning and add the correct path.
+        ## Publication
+        If you use OpenLane in your research, please cite the following paper.
         
-        ## Usage
-        In the root folder of the repository with the `venv` activated, you may invoke:
+        * M. Shalan and T. Edwards, “Building OpenLANE: A 130nm OpenROAD-based Tapeout-Proven Flow: Invited Paper,” *2020 IEEE/ACM International Conference On Computer Aided Design (ICCAD)*, San Diego, CA, USA, 2020, pp. 1-6. [Paper](https://ieeexplore.ieee.org/document/9256623)
         
-        ```sh
-        openlane --pdk-root <path/to/pdk> </path/to/config.json>
+        ```bibtex
+        @INPROCEEDINGS{9256623,
+          author={Shalan, Mohamed and Edwards, Tim},
+          booktitle={2020 IEEE/ACM International Conference On Computer Aided Design (ICCAD)}, 
+          title={Building OpenLANE: A 130nm OpenROAD-based Tapeout- Proven Flow : Invited Paper}, 
+          year={2020},
+          volume={},
+          number={},
+          pages={1-6},
+          doi={}}
         ```
         
-        To start with, you can try:
+        ## License
+        [The Apache License, version 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt).
         
-        ```sh
-        openlane --pdk-root $HOME/.volare ./designs/spm/config.json
-        ```
+        Docker images distributed by Efabless Corporation under the same license.
+        
+        Binaries bundled with OpenLane either via Cachix or Docker are distributed by
+        Efabless Corporation and may fall under stricter open source licenses.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,58 +1,53 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0a9 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0b1 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > Efabless OpenLane 2 is in early access and all APIs are,
 presently, highly unstable and subject to change without notice. > > If you
-don't know why you're here, you're probably looking for the stable version of
+*don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ****** OpenLane ******
 [License:_Apache_2.0] [Python_3.8_or_higher] [Code_Style:_black] [Checked_with
                             mypy] [Built_with_Nix]
  [Documentation_Build_Status_Badge] [Invite_to_the_Open_Source_Silicon_Slack]
 OpenLane is a RTL to GDSII infrastructure library based on several components
 including OpenROAD, Yosys, Magic, Netgen, CVC, KLayout and a number of custom
 scripts for design exploration and optimization. A reference flow performs all
-ASIC implementation steps from RTL all the way down to GDSII. ```python from
-openlane import Flow Classic = Flow.get("Classic") flow =
-Classic.init_with_config( { "PDK": "sky130A", "DESIGN_NAME": "spm",
-"VERILOG_FILES": ["./src/spm.v"], "CLOCK_PORT": "clk", "CLOCK_PERIOD": 10, },
-design_dir=".", ) flow.start() ``` ## Installation ### Binary Dependencies
+ASIC implementation steps from RTL all the way down to GDSII. You can find the
+documentation [here](https://openlane2.readthedocs.io/en/latest/
+getting_started/) to get started. ```python from openlane.flows import Flow
+Classic = Flow.factory.get("Classic") flow = Classic( { "PDK": "sky130A",
+"DESIGN_NAME": "spm", "VERILOG_FILES": ["./src/spm.v"], "CLOCK_PORT": "clk",
+"CLOCK_PERIOD": 10, }, design_dir=".", ) flow.start() ``` ## Installation
 You'll need the following: * Python **3.8** or higher with PIP, Venv and
-Tkinter * Yosys 0.23+ (preferably 0.26+) from https://github.com/YosysHQ/Yosys
-* A reasonably modern version of OpenROAD from https://github.com/The-OpenROAD-
-Project/OpenROAD * A reasonably modern version of Magic from https://
-github.com/RTimothyEdwards/Magic * A reasonably modern version of Netgen from
-https://github.com/RTimothyEdwards/netgen * KLayout 0.28.5+ from https://
-github.com/KLayout/klayout ### Docker Works for Windows, macOS and Linux.
-Easier to set up, but less integrated with your filesystem. Recommended for
-general users. See [Docker-based installation](https://
-openlane2.readthedocs.io/en/latest/getting_started/docker_installation/
-index.html) in the docs. ### Nix Works for macOS and Linux. A bit more complex
-to set up, but more integrated with your filesystem and overall less upload and
+Tkinter ### Nix (Recommended) Works for macOS and Linux (x86-64). Recommended,
+as it is more integrated with your filesystem and overall has less upload and
 download deltas. See [Nix-based installation](https://openlane2.readthedocs.io/
-en/latest/getting_started/nix_installation/index.html) in the docs. ### Conda
-TBA ### Python-only Installation You'll need to bring your own compiled tools,
-but otherwise, simply install OpenLane as follows: ```sh python3 -m pip install
---upgrade openlane ``` To quickly test your installation, run `openlane --
-smoke-test`. This may take up to 10 minutes depending on your computer's speed
-and internet connection. #### Troubleshooting With a typical Python 3.8 or
-higher installation with PIP, installing OpenLane is usually as simple as a
-`pip install`. ***Despite that***, there are some peculiarities with PIP
-itself: For example, you may see a warning among these lines: ```sh WARNING:
-The script openlane is installed in '/home/test/.local/bin' which is not on
-PATH. Consider adding this directory to PATH or, if you prefer to suppress this
-warning, use --no-warn-script-location. ``` The solution is as simple as adding
-something like this to your shell's profile: ```sh export PATH="/home/
-test/.local/bin:$PATH" ``` Do note that the path (`/home/test/.local/bin` in
-this example) varies depending on your operating system and version of Python
-you install, and whether you use `sudo` (absolutely not recommended) or not, so
-ensure that you actually read the warning and add the correct path. ## Usage In
-the root folder of the repository with the `venv` activated, you may invoke:
-```sh openlane --pdk-root
+en/latest/getting_started/nix_installation/index.html) in the docs. ### Docker
+Works for Windows, macOS and Linux (x86-64, aarch64 with emulation). See
+[Docker-based installation](https://openlane2.readthedocs.io/en/latest/
+getting_started/docker_installation/index.html) in the docs. Do note you'll
+need to add `--dockerized` right after `openlane` in most CLI invocations. ###
+Python-only Installation (Advanced) You'll need to bring your own compiled
+utilities, but otherwise, simply install OpenLane as follows: ```sh python3 -
+m pip install --upgrade openlane ``` ## Usage In the root folder of the
+repository, you may invoke: ```sh python3 -m openlane --pdk-root
 o/pdk>
-o/config.json> ``` To start with, you can try: ```sh openlane --pdk-root
-$HOME/.volare ./designs/spm/config.json ``` Platform: UNKNOWN Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python :: 3 Classifier: Intended Audience :: Developers Classifier:
-Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
-MacOS X Requires-Python: >3.8 Description-Content-Type: text/markdown
+o/config.json> ``` To start with, you can try: ```sh python3 -m openlane --pdk-
+root $HOME/.volare ./designs/spm/config.json ``` ## Publication If you use
+OpenLane in your research, please cite the following paper. * M. Shalan and T.
+Edwards, âBuilding OpenLANE: A 130nm OpenROAD-based Tapeout-Proven Flow:
+Invited Paper,â *2020 IEEE/ACM International Conference On Computer Aided
+Design (ICCAD)*, San Diego, CA, USA, 2020, pp. 1-6. [Paper](https://
+ieeexplore.ieee.org/document/9256623) ```bibtex @INPROCEEDINGS{9256623, author=
+{Shalan, Mohamed and Edwards, Tim}, booktitle={2020 IEEE/ACM International
+Conference On Computer Aided Design (ICCAD)}, title={Building OpenLANE: A 130nm
+OpenROAD-based Tapeout- Proven Flow : Invited Paper}, year={2020}, volume={},
+number={}, pages={1-6}, doi={}} ``` ## License [The Apache License, version
+2.0](https://www.apache.org/licenses/LICENSE-2.0.txt). Docker images
+distributed by Efabless Corporation under the same license. Binaries bundled
+with OpenLane either via Cachix or Docker are distributed by Efabless
+Corporation and may fall under stricter open source licenses. Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Intended Audience :: Developers
+Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
+MacOS :: MacOS X Requires-Python: >3.8 Description-Content-Type: text/markdown
```

### Comparing `openlane-2.0.0a9/openlane/__init__.py` & `openlane-2.0.0b1/openlane/flows/builtins.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,25 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 # flake8: noqa
-"""
-The OpenLane API
-
-These modules serve as the infrastructure for OpenLane-based flows.
-Using these functions, users may either utilize built-in flows, or build custom
-Flows and/or custom Steps for the design of more sophisticated chips.
-
-..
-    no-imported-members
-"""
-
-from .flows import Flow
-from .steps import Step
-from .config import Variable, Config, ConfigBuilder, InvalidConfig
-from .common import *
-from .__version__ import __version__
+from .optimizing import Optimizing
+from .classic import Classic
+from .misc import OpenInKLayout, OpenInOpenROAD
```

### Comparing `openlane-2.0.0a9/openlane/__main__.py` & `openlane-2.0.0b1/openlane/flows/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,417 +8,358 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import sys
-import glob
-import shutil
-import marshal
-import tempfile
-import subprocess
 from textwrap import dedent
 from functools import partial
-import traceback
-from typing import Tuple, Type, Optional, List, Union
+from concurrent.futures import ThreadPoolExecutor
+from typing import Optional, Union
 
-import click
 
-from .state import State
-from .__version__ import __version__
-from .logging import (
-    LogLevelsDict,
-    set_log_level,
-    err,
-    warn,
-    info,
+from click import Parameter, echo
+from cloup import (
+    option,
+    argument,
+    option_group,
+    Context,
+    Choice,
+    Path,
 )
-from .common import (
-    get_opdks_rev,
-    get_openlane_root,
+from cloup.constraints import (
+    mutually_exclusive,
 )
-from .container import run_in_container, sanitize_path
-from .flows import Flow, SequentialFlow, FlowException, FlowError
-from .config import Config, InvalidConfig
-
-
-def run(
-    ctx: click.Context,
-    flow_name: Optional[str],
-    use_volare: bool,
-    pdk_root: Optional[str],
-    pdk: str,
-    scl: Optional[str],
-    config_files: str,
-    run_tag: Optional[str],
-    last_run: bool,
-    frm: Optional[str],
-    to: Optional[str],
-    initial_state_json: Optional[str],
-    config_override_strings: List[str],
-    log_level: str,
-):
-    try:
-        set_log_level(log_level)
-    except ValueError:
-        err(f"Invalid logging level: {log_level}.")
-        click.echo(ctx.get_help())
-        exit(-1)
-
-    if use_volare:
-        import volare
-
-        pdk_root = volare.get_volare_home(pdk_root)
-
-        volare.enable(pdk_root, pdk[:-1], get_opdks_rev())
-
-    config_file = config_files[0]
-
-    # Enforce Mutual Exclusion
-    if run_tag is not None and last_run:
-        err("--run-tag and --last-run are mutually exclusive.")
-        exit(-1)
-
-    flow_description: Union[str, List[str]] = flow_name or "Classic"
-
-    if meta := Config.get_meta(config_file, flow_override=flow_name):
-        if flow_ids := meta.flow:
-            flow_description = flow_ids
-
-    TargetFlow: Type[Flow]
-
-    if not isinstance(flow_description, str):
-        TargetFlow = SequentialFlow.make(flow_description)
-    else:
-        if FlowClass := Flow.get(flow_description):
-            TargetFlow = FlowClass
-        else:
-            err(
-                f"Unknown flow '{flow_description}' specified in configuration file's 'meta' object."
-            )
-            exit(-1)
+from cloup.typing import Decorator
 
-    try:
-        flow = TargetFlow.init_with_config(
-            config_in=config_file,
-            pdk_root=pdk_root,
-            pdk=pdk,
-            scl=scl,
-            config_override_strings=config_override_strings,
-        )
-    except InvalidConfig as e:
-        info(f"[green]Errors have occurred while loading the {e.config}.")
-        for error in e.errors:
-            err(error)
-
-        if len(e.warnings) > 0:
-            info("The following warnings have also been generated:")
-            for warning in e.warnings:
-                warn(warning)
-        info("OpenLane will now quit. Please check your configuration.")
-        exit(1)
-    except ValueError as e:
-        err(e)
-        info("OpenLane will now quit.")
-        exit(1)
+from openlane.state.state import InvalidState
 
-    initial_state: Optional[State] = None
-    if initial_state_json is not None:
-        initial_state = State.loads(open(initial_state_json).read())
-
-    if last_run:
-        runs = glob.glob(os.path.join(flow.design_dir, "runs", "*"))
-
-        latest_time: float = 0
-        latest_run: Optional[str] = None
-        for run in runs:
-            time = os.path.getmtime(run)
-            if time > latest_time:
-                latest_time = time
-                latest_run = run
-
-        if latest_run is None:
-            err("--last-run specified, but no runs found.")
-            exit(1)
 
-        run_tag = os.path.basename(latest_run)
+from .flow import Flow
+from ..common import set_tpe, get_opdks_rev
+from ..logging import set_log_level, err, LogLevelsDict
+from ..state import State
 
-    try:
-        flow.start(
-            tag=run_tag,
-            frm=frm,
-            to=to,
-            with_initial_state=initial_state,
-        )
-    except FlowException as e:
-        err(f"The flow has encountered an unexpected error: {e}")
-        err("OpenLane will now quit.")
-        exit(1)
-    except FlowError as e:
-        err(f"The following error was encountered while running the flow: {e}")
-        err("OpenLane will now quit.")
-        exit(2)
-
-
-def print_bare_version(
-    ctx: click.Context,
-    param: click.Parameter,
-    value: bool,
+
+def set_log_level_cb(
+    ctx: Context,
+    param: Parameter,
+    value: str,
 ):
-    if not value:
-        return
-    print(__version__, end="")
-    ctx.exit(0)
+    level: Union[str, int] = value
+    try:
+        try:
+            level = int(value)
+        except ValueError:
+            pass
+        set_log_level(level)
+    except ValueError as e:
+        err(f"Invalid logging level {value}: {e}.")
+        echo(ctx.get_help())
+        ctx.exit(-1)
 
 
-def run_smoke_test(
-    ctx: click.Context,
-    param: click.Parameter,
-    value: bool,
+def set_worker_count_cb(
+    ctx: Context,
+    param: Parameter,
+    value: Optional[int],
 ):
-    if not value:
-        return
-    dockerized = ctx.params["dockerized"]
+    if value is None:
+        return None
 
-    with tempfile.TemporaryDirectory("_ol2design") as d:
-        final_path = os.path.join(d, "spm")
-        shutil.copytree(
-            os.path.join(get_openlane_root(), "smoke_test_design"),
-            final_path,
-        )
-
-        cmd = (
-            [
-                (sys.executable if not dockerized else "python3"),
-                "-m",
-                "openlane",
-            ]
-            + (["--dockerized", "--docker-mount", d] if dockerized else [])
-            + [os.path.join(final_path, "config.json")]
-        )
+    set_tpe(ThreadPoolExecutor(max_workers=value))
 
-        try:
-            subprocess.check_call(cmd)
-        except subprocess.CalledProcessError:
-            print("")
-            err("Smoke test failed.")
-            ctx.exit(-1)
-
-    ctx.exit(0)
 
+def initial_state_cb(
+    ctx: Context,
+    param: Parameter,
+    value: Optional[str],
+):
+    if value is None:
+        return None
 
-def cli_in_container(ctx: click.Context, docker_mounts: Tuple[str], kwargs: dict):
-    f = None
-    status = 0
     try:
-        if isj := kwargs.get("initial_state_json"):
-            _, kwargs["initial_state_json"] = sanitize_path(isj)
+        initial_state_str = open(value, encoding="utf8").read()
+    except Exception as e:
+        err(f"Failed to read initial state: {e}")
+        ctx.exit(-1)
+    try:
+        initial_state = State.loads(initial_state_str, validate_path=True)
+    except InvalidState as e:
+        err(e)
+        ctx.exit(-1)
 
-        config_files: List[str] = []
-        for file in kwargs["config_files"]:
-            _, target = sanitize_path(file)
-            config_files.append(target)
-        kwargs["config_files"] = config_files
-
-        pdk_root = kwargs.pop("pdk_root")
-        pdk = kwargs.pop("pdk")
-        scl = kwargs.pop("scl")
-
-        f = tempfile.NamedTemporaryFile("wb", suffix=".marshalled", delete=False)
-        marshal.dump(kwargs, f, 4)
-        f.close()
-        _, binary = sanitize_path(f.name)
-
-        run_in_container(
-            f"ghcr.io/efabless/openlane2:{__version__}",
-            ["python3", "-m", "openlane", binary],
-            pdk_root=pdk_root,
-            pdk=pdk,
-            scl=scl,
-            other_mounts=docker_mounts + (os.path.dirname(f.name),),
-        )
-    except ValueError as e:
-        print(e)
-        status = -1
-    except subprocess.CalledProcessError as e:
-        status = e.returncode
-    except Exception:
-        traceback.print_exc()
-        status = -1
-    finally:
-        if f is not None:
-            try:
-                os.unlink(f.name)
-            except FileNotFoundError:
-                pass
-        ctx.exit(status)
+    return initial_state
 
 
-o = partial(click.option, show_default=True)
+def only_cb(
+    ctx: Context,
+    param: Parameter,
+    value: Optional[str],
+):
+    if value is not None:
+        ctx.obj = ctx.obj or {}
+        ctx.obj["only"] = value
+    return value
 
 
-@click.command(
-    no_args_is_help=True,
-)
-@click.version_option(
-    __version__,
-    prog_name="OpenLane",
-    message=dedent(
-        """
-        %(prog)s v%(version)s
-
-        Copyright ©2020-2023 Efabless Corporation and other contributors.
-
-        Available under the Apache License, version 2. Included with the source code,
-        but you can also get a copy at https://www.apache.org/licenses/LICENSE-2.0
-
-        Included tools and utilities may be distributed under stricter licenses.
-        """
-    ).strip(),
-)
-@o(
-    "--bare-version",
-    is_flag=True,
-    is_eager=True,
-    expose_value=False,
-    callback=print_bare_version,
-    hidden=True,
-)
-@o(
-    "--dockerized/--native",
-    is_eager=True,
-    default=False,
-    help="Run OpenLane primarily using a Docker container. Some caveats apply.",
-)
-@o(
-    "--docker-mount",
-    "docker_mounts",
-    multiple=True,
-    default=[],
-    help="Mount this directory in dockerized mode. Can be supplied multiple times to mount multiple directories.",
-)
-@o(
-    "-f",
-    "--flow",
-    "flow_name",
-    type=click.Choice(Flow.factory.list(), case_sensitive=False),
-    default=None,
-    help="The built-in OpenLane flow to use",
-)
-@o(
-    "--volare-pdk/--manual-pdk",
-    "use_volare",
-    default=True,
-    help="Automatically use Volare for PDK version installation and enablement. Set --manual if you want to use a custom PDK version.",
-)
-@o(
-    "--pdk-root",
-    default=os.environ.pop("PDK_ROOT", None),
-    help="Override volare PDK root folder. Required if Volare is not installed.",
-)
-@o(
-    "-p",
-    "--pdk",
-    type=str,
-    default=os.environ.pop("PDK", "sky130A"),
-    help="The process design kit to use.",
-)
-@o(
-    "-s",
-    "--scl",
-    type=str,
-    default=os.environ.pop("STD_CELL_LIBRARY", None),
-    help="The standard cell library to use. If None, the PDK's default standard cell library is used.",
-)
-@o(
-    "--run-tag",
-    default=None,
-    type=str,
-    help="An optional name to use for this particular run of an OpenLane-based flow. Mutually exclusive with --last-run.",
-)
-@o(
-    "-I",
-    "--with-initial-state",
-    "initial_state_json",
-    type=click.Path(
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-    ),
-    default=None,
-    help="Use this JSON file as an initial state. If this is not specified, the latest `state_out.json` of the run directory will be used if available.",
-)
-@o(
-    "-c",
-    "--override-config",
-    "config_override_strings",
-    type=str,
-    multiple=True,
-    help="For this run only- override a configuration variable with a certain value. In the format KEY=VALUE. Can be specified multiple times. Values must be valid JSON values.",
-)
-@o(
-    "--smoke-test",
-    is_flag=True,
-    help="Runs a basic OpenLane smoke test.",
-    expose_value=False,
-    callback=run_smoke_test,
-)
-@o(
-    "--last-run",
-    is_flag=True,
-    default=False,
-    help="Attempt to resume the last run. Supported by sequential flows. Mutually exclusive with --run-tag.",
-)
-@o(
-    "-F",
-    "--from",
-    "frm",
-    type=str,
-    default=None,
-    help="Start from a step with this id. Supported by sequential flows.",
-)
-@o(
-    "-T",
-    "--to",
-    type=str,
-    default=None,
-    help="Stop at a step with this id. Supported by sequential flows.",
-)
-@o(
-    "--log-level",
-    type=str,
-    default="VERBOSE",
-    help=dedent(
-        """
-        A logging level. Set to INFO or higher to silence subprocess logs.
-
-        You can provide either a number or a string out of the following (higher is more silent):
-        """
-    )
-    + ",".join([f"{name}={value}" for name, value in LogLevelsDict.items()]),
-)
-@click.argument(
-    "config_files",
-    required=True,
-    nargs=-1,
-    type=click.Path(
-        exists=True,
-        file_okay=True,
-        dir_okay=True,
-    ),
-)
-@click.pass_context
-def cli(ctx: click.Context, dockerized: bool, docker_mounts: Tuple[str], **kwargs):
-    if dockerized:
-        cli_in_container(ctx, docker_mounts, kwargs)
-    run_kwargs = kwargs
-    args = kwargs["config_files"]
-    if len(args) == 1 and args[0].endswith(".marshalled"):
-        run_kwargs = marshal.load(open(args[0], "rb"))
-        run_kwargs.update(**{k: kwargs[k] for k in ["pdk_root", "pdk", "scl"]})
-    run(ctx, **run_kwargs)
+def from_to_cb(
+    ctx: Context,
+    param: Parameter,
+    value: Optional[str],
+):
+    if isinstance(ctx.obj, dict) and ctx.obj.get("only"):
+        return ctx.obj.get("only")
+    return value
+
+
+def use_volare_cb(
+    ctx: Context,
+    param: Parameter,
+    value: bool,
+):
+    ctx.obj = ctx.obj or {}
+    ctx.obj["use_volare"] = value
+
+
+def pdk_scl_cb(
+    ctx: Context,
+    param: Parameter,
+    value: Optional[str],
+):
+    if param.name is None:
+        return
 
+    values = ctx.params.copy()
+    values[param.name] = value
+    if "pdk" in values and "scl" in values:
+        pdk = values["pdk"]
+        pdk_family = pdk[:-1]
+        if ctx.obj and ctx.obj.get("use_volare"):
+            import volare
+
+            pdk_root = volare.get_volare_home(values["pdk_root"])
+
+            volare.enable(pdk_root, pdk_family, get_opdks_rev())
+    return value
+
+
+def cloup_flow_opts(
+    config_options: bool = True,
+    run_options: bool = True,
+    sequential_flow_controls: bool = True,
+    pdk_options: bool = True,
+    log_level: bool = True,
+    jobs: bool = True,
+    accept_config_files: bool = True,
+    volare_by_default: bool = True,
+) -> Decorator:
+    """
+    Creates a wrapper that appends a number of OpenLane flow-related flags to a
+    function decorated with `@cloup.command https://cloup.readthedocs.io/en/stable/autoapi/cloup/index.html#cloup.command`_.
+
+    The following keyword arguments will be passed to the decorated function.
+    * Those postfixed ‡ are compatible with the constructor for :class:`Flow`.
+    * Those postfixed § are compatible with the :meth:`Flow.start`.
+
+    * Flow configuration options (if parameter ``config_options`` is ``True``):
+        * ``flow_name``: ``Optional[str]``: A valid flow ID to be used with :meth:`Flow.factory.get`
+        * ``config_override_strings``‡: ``Optional[Iterable[str]]``
+    * Sequential flow controls (if parameter ``sequential_flow_controls`` is ``True``)
+        * ``frm``§: ``str``: Start from a step with this ID. Supported by sequential flows.
+        * ``to``§: ``str``: Stop at a step with this id. Supported by sequential flows.
+        * ``skip``§: ``Iterable[str]``: Skip these steps. Supported by sequential flows.
+    * Flow run options (if parameter ``run_options`` is ``True``):
+        * ``tag``§: ``Optional[str]``
+        * ``last_run``§: ``bool``: If ``True``, ``tag`` is guaranteed to be None.
+        * ``with_initial_state``§: ``Optional[State]``
+    * PDK options
+        * ``use_volare``: ``bool``
+        * ``pdk_root``‡: ``Optional[str]``
+        * ``pdk``‡: ``str``
+        * ``scl``‡: ``Optional[str]``
+    * ``config_files``: ``Iterable[str]``: Paths to configuration files (if
+      parameter  ``accept_config_files`` is ``True``)
+
+    :param config_options: Enables flow configuration and starting CLI flags
+    :param sequential_flow_controls: Enables flow control CLI flags
+    :param flow_run_options: Enables tag CLI flags
+    :param pdk_options: Enables PDK CLI flags
+    :param log_level: Enables ``--log-level`` CLI flag
+    :param jobs: Enables ``-j/--jobs`` CLI flag
+    :param accept_config_files: Accepts configuration file paths as CLI arguments
+    :param volare_by_default: If ``pdk_options`` is ``True``, this changes whether
+        Volare is used by default for this CLI or not.
+    :returns: The wrapper
+    """
+    o = partial(option, show_default=True)
+
+    def decorator(f):
+        if config_options:
+            f = option_group(
+                "Flow configuration options",
+                o(
+                    "-f",
+                    "--flow",
+                    "flow_name",
+                    type=Choice(Flow.factory.list(), case_sensitive=False),
+                    default=None,
+                    help="The built-in OpenLane flow to use for this run",
+                ),
+                o(
+                    "-c",
+                    "--override-config",
+                    "config_override_strings",
+                    type=str,
+                    multiple=True,
+                    help="For this run only- override a configuration variable with a certain value. In the format KEY=VALUE. Can be specified multiple times. Values must be valid JSON values.",
+                ),
+            )(f)
+        if run_options:
+            f = option_group(
+                "Run options",
+                o(
+                    "--run-tag",
+                    "tag",
+                    default=None,
+                    type=str,
+                    help="An optional name to use for this particular run of an OpenLane-based flow. Used to create the run directory.",
+                ),
+                o(
+                    "-i",
+                    "--with-initial-state",
+                    type=Path(
+                        exists=True,
+                        file_okay=True,
+                        dir_okay=False,
+                    ),
+                    default=None,
+                    callback=initial_state_cb,
+                    help="Use this JSON file as an initial state. If this is not specified, the latest `state_out.json` of the run directory will be used if available.",
+                ),
+                o(
+                    "--last-run",
+                    is_flag=True,
+                    default=False,
+                    help="Use the last run as the run tag.",
+                ),
+                constraint=mutually_exclusive,
+            )(f)
+        if sequential_flow_controls:
+            f = option_group(
+                "Sequential flow controls",
+                o(
+                    "-F",
+                    "--from",
+                    "frm",
+                    type=str,
+                    default=None,
+                    callback=from_to_cb,
+                    help="Start from a step with this id. Supported by sequential flows.",
+                ),
+                o(
+                    "-T",
+                    "--to",
+                    type=str,
+                    default=None,
+                    callback=from_to_cb,
+                    help="Stop at a step with this id. Supported by sequential flows.",
+                ),
+                o(
+                    "--only",
+                    type=str,
+                    default=None,
+                    expose_value=False,
+                    is_eager=True,
+                    callback=only_cb,
+                    help="Shorthand to set both --from and --to to the same value. Overrides the values from both.",
+                ),
+                o(
+                    "-S",
+                    "--skip",
+                    type=str,
+                    multiple=True,
+                    help="Skip these steps. Supported by sequential flows.",
+                ),
+            )(f)
+        if log_level:
+            f = o(
+                "--log-level",
+                type=str,
+                default="VERBOSE",
+                help=dedent(
+                    """
+                    A logging level. Set to INFO or higher to silence subprocess logs.
+
+                    You can provide either a number or a string out of the following (higher is more silent):
+                    """
+                )
+                + ",".join(
+                    [f"{name}={value}" for name, value in LogLevelsDict.items()]
+                ),
+                callback=set_log_level_cb,
+                expose_value=False,
+            )(f)
+        if pdk_options:
+            f = option_group(
+                "PDK options",
+                o(
+                    "--volare-pdk/--manual-pdk",
+                    "use_volare",
+                    is_eager=True,
+                    default=volare_by_default,
+                    help="Automatically use Volare for PDK version installation and enablement. Set --manual if you want to use a custom PDK version.",
+                    expose_value=False,
+                    callback=use_volare_cb,
+                ),
+                o(
+                    "--pdk-root",
+                    type=Path(
+                        exists=True,
+                        file_okay=False,
+                        dir_okay=True,
+                    ),
+                    is_eager=True,
+                    default=os.environ.pop("PDK_ROOT", None),
+                    help="Override volare PDK root folder. Required if Volare is not installed.",
+                ),
+                o(
+                    "-p",
+                    "--pdk",
+                    type=str,
+                    default=os.environ.pop("PDK", "sky130A"),
+                    help="The process design kit to use.",
+                    callback=pdk_scl_cb,
+                ),
+                o(
+                    "-s",
+                    "--scl",
+                    type=str,
+                    default=os.environ.pop("STD_CELL_LIBRARY", None),
+                    help="The standard cell library to use. If None, the PDK's default standard cell library is used.",
+                    callback=pdk_scl_cb,
+                ),
+            )(f)
+        if jobs:
+            f = o(
+                "-j",
+                "--jobs",
+                type=int,
+                default=os.cpu_count(),
+                help="The maximum number of threads or processes that can be used by OpenLane.",
+                callback=set_worker_count_cb,
+                expose_value=False,
+            )(f)
+        if accept_config_files:
+            f = argument(
+                "config_files",
+                nargs=-1,
+                type=Path(
+                    exists=True,
+                    file_okay=True,
+                    dir_okay=True,
+                ),
+            )(f)
+        return f
 
-if __name__ == "__main__":
-    cli()
+    return decorator
```

### Comparing `openlane-2.0.0a9/openlane/__version__.py` & `openlane-2.0.0b1/openlane/scripts/magic/wrapper.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright 2023 Efabless Corporation
+# Copyright 2020-2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "2.0.0a9"
 
-if __name__ == "__main__":
-    print(__version__, end="")
+if {[catch {source $::env(MAGIC_SCRIPT)} err]} {
+    puts "Error: $err"
+    exit 1
+}
```

### Comparing `openlane-2.0.0a9/openlane/common.py` & `openlane-2.0.0b1/openlane/common/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,64 +7,67 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-Common Utilities
-
-A number of common utility functions used throughout the codebase.
-"""
 import os
 import re
 import typing
 import pathlib
 import unicodedata
+from enum import Enum
+from collections import UserString
 
+from typing import (
+    Any,
+    Iterable,
+    Sequence,
+    TypeVar,
+)
 
-def mkdirp(path: typing.Union[str, os.PathLike]):
-    """
-    Attempts to create a directory and all of its parents.
 
-    Does not fail if the directory already exists, however, it does fail
-    if it is unable to create any of the components and/or if
-
-    :param path: A filesystem path for the directory
-    """
-    return pathlib.Path(path).mkdir(parents=True, exist_ok=True)
+T = TypeVar("T")
 
 
-openlane_root = os.path.dirname(os.path.abspath(__file__))
+def idem(obj: T, *args, **kwargs) -> T:
+    """
+    :returns: the parameter ``obj`` unchanged. Useful for some lambdas.
+    """
+    return obj
 
 
 def get_openlane_root() -> str:
     """
     Returns the root OpenLane folder, i.e., the folder containing the
     ``__init__.py``.
     """
-    return openlane_root
+    return os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 
 def get_script_dir() -> str:
     """
     Gets the OpenLane tool `scripts` directory.
+
+    :meta private:
     """
     return os.path.join(
-        openlane_root,
+        get_openlane_root(),
         "scripts",
     )
 
 
 def get_opdks_rev() -> str:
     """
-    Gets the Open_PDKs revision.
+    Gets the Open_PDKs revision confirmed compatible with this version of OpenLane.
     """
-    return open(os.path.join(openlane_root, "open_pdks_rev"), encoding="utf8").read()
+    return open(
+        os.path.join(get_openlane_root(), "open_pdks_rev"), encoding="utf8"
+    ).read()
 
 
 # The following code snippet has been adapted under the following license:
 #
 # Copyright (c) Django Software Foundation and individual contributors.
 # All rights reserved.
 
@@ -92,38 +95,99 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 def slugify(value: str) -> str:
     """
     :param value: Input string
-    :returns: The input string converted to lower case, with non-word
-        (alphanumeric/underscore) characters removed, and spaces converted
-        into hyphens.
+    :returns: The input string converted to lower case, with all characters
+        except alphanumerics, underscores and hyphens removed, and spaces and\
+        dots converted into hyphens.
 
         Leading and trailing whitespace is stripped.
     """
     value = (
         unicodedata.normalize("NFKD", value).encode("ascii", "ignore").decode("ascii")
     )
     value = re.sub(r"[^\w\s\-\.]", "", value).strip().lower()
-    return re.sub(r"[-\s\.]+", "-", value)
+    return re.sub(r"[\s\.]+", "-", value)
 
 
-final = typing.final
+def protected(method):
+    """A decorator to indicate protected methods.
 
+    It dynamically adds a statement to the effect in the docstring as well
+    as setting an attribute, ``protected``, to ``True``, but has no other effects.
 
-def internal(method):
-    """A decorator to indicate internal methods.
-
-    It dynamically adds a statement to the effect in the docstring, but has no
-    other runtime effects.
-
-    :param f: Method to mark as internal
+    :param f: Method to mark as protected
     """
     if method.__doc__ is None:
         method.__doc__ = ""
-    method.__doc__ = (
-        "**This method is considered internal and should only be called by this class or its subclass hierarchy.**\n"
-        + method.__doc__
-    )
+    method.__doc__ = "**protected**\n" + method.__doc__
+
+    setattr(method, "protected", True)
     return method
+
+
+final = typing.final
+
+
+def mkdirp(path: typing.Union[str, os.PathLike]):
+    """
+    Attempts to create a directory and all of its parents.
+
+    Does not fail if the directory already exists, however, it does fail
+    if it is unable to create any of the components and/or if the path
+    already exists as a file.
+
+    :param path: A filesystem path for the directory
+    """
+    return pathlib.Path(path).mkdir(parents=True, exist_ok=True)
+
+
+def StringEnum(name: str, values: Sequence[str]):
+    """
+    Creates a string enumeration class where the keys and values are the same.
+    """
+    return Enum(name, [(value, value) for value in values])
+
+
+class Path(UserString, os.PathLike):
+    """
+    A Path type for OpenLane configuration variables.
+
+    Basically just a string.
+    """
+
+    def __fspath__(self) -> str:
+        return str(self)
+
+    def exists(self) -> bool:
+        """
+        A convenience method calling :meth:`os.path.exists`
+        """
+        return os.path.exists(self)
+
+
+class zip_first(object):
+    """
+    Works like ``zip_longest`` if |a| > |b| and ``zip`` if |a| <= |b|.
+    """
+
+    def __init__(self, a: Iterable, b: Iterable, fillvalue: Any) -> None:
+        self.a = a
+        self.b = b
+        self.fillvalue = fillvalue
+
+    def __iter__(self):
+        self.iter_a = iter(self.a)
+        self.iter_b = iter(self.b)
+        return self
+
+    def __next__(self):
+        a = next(self.iter_a)
+        b = self.fillvalue
+        try:
+            b = next(self.iter_b)
+        except StopIteration:
+            pass
+        return (a, b)
```

### Comparing `openlane-2.0.0a9/openlane/config/__init__.py` & `openlane-2.0.0b1/openlane/scripts/magic/def/mag.tcl`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# Copyright 2023 Efabless Corporation
+# Copyright 2020-2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-The Configuration Module
 
-This modules includes various functions for importing and/or generating OpenLane
-configuration objects. Configuration objects are the primary input to a flow.
-"""
-from .builder import ConfigBuilder, InvalidConfig
-from .config import Config
-from .variable import Variable, StringEnum, Path
-from .resolve import Keys
+source $::env(SCRIPTS_DIR)/magic/def/read.tcl
 
-from .tcleval import env_from_tcl
-from .flow import all_variables as universal_flow_config_variables
+save $::env(SAVE_MAG)
+
+puts "[INFO] Done exporting $::env(SAVE_MAG)."
```

### Comparing `openlane-2.0.0a9/openlane/config/builder.py` & `openlane-2.0.0b1/openlane/config/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,29 +9,49 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import json
+import yaml
+import dataclasses
 from glob import glob
 from decimal import Decimal
-from typing import List, Sequence, Tuple, Optional, Callable, Union, Dict
+from textwrap import dedent
+from dataclasses import dataclass
+from typing import (
+    Any,
+    ClassVar,
+    Tuple,
+    Union,
+    List,
+    Optional,
+    Sequence,
+    Callable,
+    Dict,
+    Set,
+)
 
-from .resolve import resolve, Keys
+from .variable import Macro, Variable
+from .preprocessor import preprocess_dict, Keys as SpecialKeys
+from .flow import removed_variables, all_variables as flow_common_variables
 from .pdk import (
     all_variables as pdk_variables,
     removed_variables as pdk_removed_variables,
     migrate_old_config,
 )
-from .flow import removed_variables, all_variables as flow_common_variables
-from .tcleval import env_from_tcl
-from .config import Config, Meta
-from .variable import Variable
 from ..logging import info, warn
+from ..common import GenericDict, GenericImmutableDict, TclUtils, Path
+
+
+@dataclass
+class Meta:
+    version: int = 1
+    flow: Union[None, str, List[str]] = "Classic"
 
 
 class InvalidConfig(ValueError):
     """
     An error raised when a configuration under resolution is invalid.
 
     :param config: A human-readable name for the particular configuration file
@@ -39,53 +59,151 @@
         user configuration file.
     :param warnings: A list of warnings generated during the loading of this
         configuration file.
     :param errors: A list of errors generated during the loading of this
         configuration file.
     :param args: Further arguments to be passed onto the constructor of
         :class:`ValueError`.
+    :param message: An optional override for the Exception message.
     :param kwargs: Further keyword arguments to be passed onto the constructor of
         :class:`ValueError`.
     """
 
     def __init__(
         self,
         config: str,
         warnings: List[str],
         errors: List[str],
+        message: Optional[str] = None,
         *args,
         **kwargs,
     ) -> None:
         self.config = config
         self.warnings = warnings
         self.errors = errors
+        if message is None:
+            message = "The following errors were encountered: \n"
+            for error in self.errors:
+                message += f"\t* {error}"
+        super().__init__(message, *args, **kwargs)
+
+
+class Config(GenericImmutableDict[str, Any]):
+    """
+    A map from OpenLane configuration variable keys to their values.
+
+    It is recommended that you use :meth:`load` to create new, validated
+    configurations from dictionaries or files.
+    """
+
+    current_interactive: ClassVar[Optional["Config"]] = None
+    meta: Meta
+    __interactive: bool = False
+
+    def __init__(self, *args, meta: Optional[Meta] = None, **kwargs):
+        if meta is None:
+            meta = Meta(version=1)
+
+        self.meta = meta
+
         super().__init__(*args, **kwargs)
 
+    def copy(self, **overrides) -> "Config":
+        """
+        Produces a *shallow* copy of the configuration object.
 
-class DecimalDecoder(json.JSONDecoder):
-    def default(self, o):
-        if isinstance(o, float) or isinstance(o, int):
-            return Decimal(o)
-        return super(DecimalDecoder, self).default(o)
+        :param overrides: A series of configuration overrides as key-value pairs.
+            These values are NOT validated and you should not be overriding these
+            haphazardly.
+        """
+        return Config(self, meta=self.meta, overrides=overrides)
 
+    def to_raw_dict(self) -> Dict[str, Any]:
+        """
+        :returns: A raw dictionary representation including the ``meta`` object.
+        """
+        final = super().to_raw_dict()
+        final["meta"] = self.meta
+        return final
 
-class ConfigBuilder(object):
-    """
-    Various constructors for OpenLane configuration objects.
-    """
+    def copy_filtered(
+        self,
+        config_vars: List[Variable],
+        include_pdk_variables: bool = True,
+        include_common_variables: bool = True,
+    ) -> "Config":
+        variables: Set[str] = set([variable.name for variable in config_vars])
+        if include_pdk_variables:
+            variables = variables.union(
+                set([variable.name for variable in pdk_variables])
+            )
+        if include_common_variables:
+            variables = variables.union(
+                set([variable.name for variable in flow_common_variables])
+            )
+
+        return Config(
+            {variable: self[variable] for variable in variables},
+            meta=dataclasses.replace(self.meta),
+        )
+
+    def _repr_markdown_(self) -> str:  # pragma: no cover
+        title = "Interactive Configuration" if self.__interactive else "Configuration"
+        values_title = "Initial Values" if self.__interactive else "Values"
+        return (
+            dedent(
+                f"""
+                ### {title}
+                #### {values_title}
+
+                <br />
+
+                ```yml
+                %s
+                ```
+                """
+            )
+            % yaml.safe_dump(json.loads(self.dumps()))
+        )
+
+    @classmethod
+    def get_meta(
+        Self,
+        json_config_in: Union[str, os.PathLike],
+        flow_override: Optional[str] = None,
+    ) -> Optional[Meta]:
+        """
+        Returns the Meta object of a JSON configuration file
+
+        :param config_in: A configuration file.
+        :returns: Either a Meta object, or if the file is not a JSON file, None.
+        """
+        try:
+            obj = json.load(open(json_config_in, encoding="utf8"))
+        except (json.JSONDecodeError, IsADirectoryError):
+            return None
+
+        meta = Meta()
+        if meta_raw := obj.get("meta"):
+            meta = Meta(**meta_raw)
+
+        if flow_override is not None:
+            meta.flow = flow_override
+
+        return meta
 
     @classmethod
     def interactive(
         Self,
         DESIGN_NAME: str,
         PDK: str,
         STD_CELL_LIBRARY: Optional[str] = None,
         PDK_ROOT: Optional[str] = None,
         **kwargs,
-    ) -> Config:
+    ) -> "Config":
         """
         This constructs a partial configuration object that may be incrementally
         adjusted per-step, and activates OpenLane's **interactive mode**.
 
         The interactive mode is overall less rigid than the pure mode, adding various
         references to global objects to make the REPL or Notebook experience more
         pleasant, however, it is not as resilient as the pure mode and should not
@@ -103,69 +221,75 @@
 
         :param kwargs: Any overrides to PDK values and/or common flow default variables
             can be passed as keyword arguments to this function.
 
             Useful examples are CLOCK_PORT, CLOCK_PERIOD, et cetera, which while
             not bound to a specific :class:`Step`, affects most Steps' behavior.
         """
-        config_in, _, _ = Self._get_pdk_config(
+        PDK_ROOT = Self.__resolve_pdk_root(PDK_ROOT)
+
+        config_in, _, _ = Self.__get_pdk_config(
             PDK,
             STD_CELL_LIBRARY,
             PDK_ROOT,
         )
 
-        config_in["PDK_ROOT"] = PDK_ROOT
-        config_in["DESIGN_NAME"] = DESIGN_NAME
+        kwargs["DESIGN_NAME"] = DESIGN_NAME
 
-        config_in.update(kwargs)
+        config_in = Config(config_in, overrides=kwargs)
 
-        config_in, design_warnings, design_errors = Variable.process_config(
-            config_in,
-            pdk_variables + list(flow_common_variables),
+        config_in, design_warnings, design_errors = config_in.__process_variable_list(
+            pdk_variables,
+            list(flow_common_variables),
             removed_variables,
+            unknown_key_warn=False,
         )
 
         if len(design_errors) != 0:
             raise InvalidConfig("default configuration", design_warnings, design_errors)
 
         if len(design_warnings) > 0:
             info(
                 "Loading the default configuration has generated the following warnings:"
             )
         for warning in design_warnings:
             warn(warning)
 
-        config_in.interactive = True
-
+        config_in.__interactive = True
         Config.current_interactive = config_in
 
         return config_in
 
     @classmethod
     def load(
         Self,
-        config_in: Union[str, os.PathLike, Dict],
+        config_in: Union[str, os.PathLike, Dict[str, Any]],
         flow_config_vars: Sequence[Variable],
         config_override_strings: Optional[Sequence[str]] = None,
         pdk: Optional[str] = None,
         pdk_root: Optional[str] = None,
         scl: Optional[str] = None,
         design_dir: Optional[str] = None,
     ) -> Tuple["Config", str]:
         """
+        Creates a new Config object based on a Tcl file, a JSON file, or a
+        dictionary.
+
+        The returned config object is locked and cannot be modified.
+
         :param config_in: Either a file path to a JSON file or a Python
             dictionary representing an unprocessed OpenLane configuration
             object.
 
             Tcl files are also supported, but are deprecated and will be removed
             in the future.
 
         :param config_override_strings: A list of "overrides" in the form of
             NAME=VALUE strings. These are primarily for running OpenLane from
-            the commandline and strictly speaking should not be used in the API.
+            the command-line and strictly speaking should not be used in the API.
 
         :param design_dir: The design directory for said configuration.
             Supported and required *if and only if* config_in is a dictionary.
 
         :param pdk: A process design kit to use. Required unless specified via the
             "PDK" key in a configuration object.
 
@@ -173,222 +297,240 @@
 
             If Volare is installed, this value can be used to optionally override
             Volare's default.
 
         :param scl: A standard cell library to use. If not specified, the PDK's
             default standard cell library will be used instead.
 
-        :returns: A tuple containing a ConfigBuilder and the design directory.
+        :returns: A tuple containing a Config object and the design directory.
         """
-
-        loader: Callable = Self._loads
+        loader: Callable = Self.__loads
         raw: Union[str, dict] = ""
+        default_meta_version = 1
         if not isinstance(config_in, dict):
             if design_dir is not None:
                 raise TypeError(
                     "The argument design_dir is not supported when config_in is not a dictionary."
                 )
             config_in = os.path.abspath(config_in)
 
             design_dir = str(os.path.dirname(config_in))
             config_in = str(config_in)
             if config_in.endswith(".json"):
                 raw = open(config_in, encoding="utf8").read()
             elif config_in.endswith(".tcl"):
                 raw = open(config_in, encoding="utf8").read()
-                loader = Self._loads_tcl
-                if config_override_strings is None:
-                    raise ValueError(
-                        "CLI override strings are not supported with .Tcl configuration files."
-                    )
+                loader = Self.__loads_tcl
             else:
                 if os.path.isdir(config_in):
                     raise ValueError(
-                        "Passing design folders as arguments is unsupported in OpenLane 2.0+: please pass the JSON configuration file directly."
+                        "Passing design folders as arguments is unsupported in OpenLane 2 or higher: please pass the JSON configuration file directly."
                     )
                 _, ext = os.path.splitext(config_in)
                 raise ValueError(
                     f"Unsupported configuration file extension '{ext}' for '{config_in}'."
                 )
         else:
+            default_meta_version = 2
             if design_dir is None:
                 raise TypeError(
-                    "The argument design_dir is required when using ConfigBuilder with a dictionary."
+                    "The argument design_dir is required when using attempting to load a Config with a dictionary."
                 )
             raw = config_in
-            loader = Self._load_dict
+            loader = Self.__load_dict
+
+        pdk_root = Self.__resolve_pdk_root(pdk_root)
 
         loaded = loader(
             raw,
             design_dir,
             flow_config_vars=flow_config_vars,
-            pdk=pdk,
             pdk_root=pdk_root,
+            pdk=pdk,
             scl=scl,
             config_override_strings=(config_override_strings or []),
+            default_meta_version=default_meta_version,
         )
 
         return (loaded, design_dir)
 
     @classmethod
-    def _loads(
+    def __loads(
         Self,
         json_str: str,
         *args,
         **kwargs,
     ):
-        raw = json.loads(json_str, cls=DecimalDecoder)
-        kwargs["resolve_json"] = True
-        return Self._load_dict(
+        raw = json.loads(json_str, parse_float=Decimal)
+        return Self.__load_dict(
             raw,
             *args,
             **kwargs,
         )
 
     @classmethod
-    def _load_dict(
+    def __load_dict(
         Self,
-        raw: dict,
+        raw: Dict[str, Any],
         design_dir: str,
         flow_config_vars: Sequence[Variable],
         config_override_strings: Sequence[str],
+        pdk_root: str,
         pdk: Optional[str] = None,
-        pdk_root: Optional[str] = None,
         scl: Optional[str] = None,
         full_pdk_warnings: bool = False,
-        resolve_json: bool = False,
+        default_meta_version: int = 1,
     ) -> "Config":
-        meta_raw: Optional[dict] = None
+        meta: Optional[Meta] = None
         if raw.get("meta") is not None:
             meta_raw = raw["meta"]
             del raw["meta"]
+            try:
+                meta = Meta(**meta_raw)
+            except TypeError as e:
+                raise InvalidConfig(
+                    "design configuration file", [], [f"'meta' object is invalid: {e}"]
+                )
+
+        if meta is None:
+            meta = Meta(version=default_meta_version)
 
         for string in config_override_strings:
             key, value = string.split("=", 1)
             raw[key] = value
 
-        process_info = resolve(
+        process_info = preprocess_dict(
             raw,
             only_extract_process_info=True,
             design_dir=design_dir,
         )
 
-        pdk = process_info.get(Keys.pdk) or pdk
+        pdk = process_info.get(SpecialKeys.pdk) or pdk
         if pdk is None:
             raise ValueError(
                 "The pdk argument is required as the configuration object lacks a 'PDK' key."
             )
 
-        config_in, pdkpath, scl = Self._get_pdk_config(
+        config_in, pdkpath, scl = Self.__get_pdk_config(
             pdk=pdk,
             scl=scl,
             pdk_root=pdk_root,
             full_pdk_warnings=full_pdk_warnings,
         )
 
-        resolve_maybe = resolve if resolve_json else lambda x, *args, **kwargs: x
-
-        resolved = resolve_maybe(
-            raw,
-            pdk=pdk,
-            pdkpath=pdkpath,
-            scl=config_in["STD_CELL_LIBRARY"],
-            design_dir=design_dir,
-        )
-
-        config_in.update(**resolved)
-
-        config_in, design_warnings, design_errors = Variable.process_config(
+        config_in = Config(
             config_in,
-            pdk_variables + list(flow_config_vars),
+            overrides=preprocess_dict(
+                raw,
+                pdk=pdk,
+                pdkpath=pdkpath,
+                scl=config_in[SpecialKeys.scl],
+                design_dir=design_dir,
+                readable_paths=[
+                    os.path.abspath(pdkpath),
+                    os.path.abspath(design_dir),
+                ],
+            ),
+            meta=meta,
+        )
+
+        permissive_variables = pdk_variables
+        strict_variables = list(flow_config_vars)
+        unknown_key_warn = False
+        if meta.version < 2:
+            permissive_variables = permissive_variables + strict_variables
+            strict_variables = []
+            unknown_key_warn = True
+
+        config_in, design_warnings, design_errors = config_in.__process_variable_list(
+            permissive_variables,
+            strict_variables,
             removed_variables,
+            unknown_key_warn,
         )
 
-        if meta_raw is not None:
-            try:
-                config_in.meta = Meta(**meta_raw)
-            except TypeError as e:
-                design_errors.append(f"'meta' object is invalid: {e}")
-
         if len(design_errors) != 0:
             raise InvalidConfig(
                 "design configuration file", design_warnings, design_errors
             )
 
         if len(design_warnings) > 0:
             info(
                 "Loading the design configuration file has generated the following warnings:"
             )
         for warning in design_warnings:
             warn(warning)
 
-        config_in["PDK_ROOT"] = pdk_root
         return config_in
 
     @classmethod
-    def _loads_tcl(
+    def __loads_tcl(
         Self,
         config: str,
         design_dir: str,
         flow_config_vars: Sequence[Variable],
         config_override_strings: Sequence[str],  # Unused, kept for API consistency
+        pdk_root: str,
         pdk: Optional[str] = None,
-        pdk_root: Optional[str] = None,
         scl: Optional[str] = None,
         full_pdk_warnings: bool = False,
+        default_meta_version: int = 1,  # Unused, kept for API consistency
     ) -> "Config":
         warn(
             "Support for .tcl configuration files is deprecated. Please migrate to a .json file at your earliest convenience."
         )
 
-        pdk_root = Self._resolve_pdk_root(pdk_root)
+        pdk_root = Self.__resolve_pdk_root(pdk_root)
 
         config_in = Config(
             {
-                "PDK_ROOT": pdk_root,
-                Keys.pdk: pdk,
+                SpecialKeys.pdk_root: pdk_root,
+                SpecialKeys.pdk: pdk,
             }
         )
 
-        tcl_vars_in = config_in.copy()
-        tcl_vars_in[Keys.scl] = ""
-        tcl_vars_in[Keys.design_dir] = design_dir
-        tcl_config = env_from_tcl(tcl_vars_in, config)
+        tcl_vars_in = dict(config_in)
+        tcl_vars_in[SpecialKeys.scl] = ""
+        tcl_vars_in[SpecialKeys.design_dir] = design_dir
+        tcl_config = dict(TclUtils._eval_env(tcl_vars_in, config))
 
-        process_info = resolve(
-            tcl_config.data,
+        process_info = preprocess_dict(
+            tcl_config,
             only_extract_process_info=True,
             design_dir=design_dir,
         )
 
-        pdk = process_info.get(Keys.pdk) or pdk
+        pdk = process_info.get(SpecialKeys.pdk) or pdk
 
         if pdk is None:
             raise ValueError(
                 "The pdk argument is required as the configuration object lacks a 'PDK' key."
             )
 
-        config_in, _, scl = Self._get_pdk_config(
+        config_in, _, scl = Self.__get_pdk_config(
             pdk=pdk,
             scl=scl,
             pdk_root=pdk_root,
             full_pdk_warnings=full_pdk_warnings,
         )
 
-        tcl_vars_in[Keys.pdk] = pdk
-        tcl_vars_in[Keys.scl] = scl
-        tcl_vars_in[Keys.design_dir] = design_dir
+        tcl_vars_in[SpecialKeys.pdk] = pdk
+        tcl_vars_in[SpecialKeys.scl] = scl
+        tcl_vars_in[SpecialKeys.design_dir] = design_dir
 
-        design_config = env_from_tcl(tcl_vars_in, config)
+        design_config = TclUtils._eval_env(tcl_vars_in, config)
 
-        config_in.update(**design_config)
+        config_in = Config(config_in, overrides=design_config)
+        for string in config_override_strings:
+            key, value = string.split("=", 1)
+            config_in[key] = value
 
-        config_in, design_warnings, design_errors = Variable.process_config(
-            config_in,
+        config_in, design_warnings, design_errors = config_in.__process_variable_list(
             pdk_variables + list(flow_config_vars),
+            [],
             removed_variables,
         )
 
         if len(design_errors) != 0:
             raise InvalidConfig(
                 "design configuration file", design_warnings, design_errors
             )
@@ -396,88 +538,87 @@
         if len(design_warnings) > 0:
             info(
                 "Loading the design configuration file has generated the following warnings:"
             )
         for warning in design_warnings:
             warn(warning)
 
-        config_in["PDK_ROOT"] = pdk_root
-
         return config_in
 
     @classmethod
-    def _resolve_pdk_root(Self, pdk_root: Optional[str]) -> str:
+    def __resolve_pdk_root(Self, pdk_root: Optional[str]) -> str:
         try:
             import volare
 
             pdk_root = volare.get_volare_home(pdk_root)
         except ImportError:
             if pdk_root is None:
                 raise ValueError(
                     "The pdk_root argument is required as Volare is not installed."
                 )
         return os.path.abspath(pdk_root)
 
     @classmethod
-    def _get_pdk_config(
+    def __get_pdk_config(
         Self,
         pdk: str,
-        scl: Optional[str] = None,
-        pdk_root: Optional[str] = None,
+        scl: Optional[str],
+        pdk_root: str,
         full_pdk_warnings: Optional[bool] = False,
-    ) -> Tuple[Config, str, str]:
+    ) -> Tuple["Config", str, str]:
         """
         :returns: A tuple of the PDK configuration, the PDK path and the SCL.
         """
-        pdk_root = Self._resolve_pdk_root(pdk_root)
 
-        config_in = Config(
+        pdk_config: GenericDict[str, Any] = GenericDict(
             {
-                "PDK_ROOT": pdk_root,
-                Keys.pdk: pdk,
+                SpecialKeys.pdk_root: pdk_root,
+                SpecialKeys.pdk: pdk,
             }
         )
         if scl is not None:
-            config_in[Keys.scl] = scl
+            pdk_config[SpecialKeys.scl] = scl
 
         pdkpath = os.path.join(pdk_root, pdk)
         if not os.path.exists(pdkpath):
             matches = glob(f"{pdkpath}*")
             errors = [f"The PDK {pdk} was not found."]
             warnings = []
             for match in matches:
                 basename = os.path.basename(match)
                 warnings.append(f"A similarly-named PDK was found: {basename}")
             raise InvalidConfig("PDK configuration", warnings, errors)
 
         pdk_config_path = os.path.join(pdkpath, "libs.tech", "openlane", "config.tcl")
 
-        config_in = env_from_tcl(
-            config_in,
+        pdk_env = TclUtils._eval_env(
+            pdk_config,
             open(pdk_config_path, encoding="utf8").read(),
         )
 
-        scl = config_in["STD_CELL_LIBRARY"]
+        scl = pdk_env["STD_CELL_LIBRARY"]
         assert (
             scl is not None
         ), "Fatal error: STD_CELL_LIBRARY default value not set by PDK."
 
         scl_config_path = os.path.join(
             pdkpath, "libs.tech", "openlane", scl, "config.tcl"
         )
-        config_in = migrate_old_config(
-            env_from_tcl(
-                config_in,
+
+        scl_env = migrate_old_config(
+            TclUtils._eval_env(
+                pdk_env,
                 open(scl_config_path, encoding="utf8").read(),
             )
         )
 
-        config_in, pdk_warnings, pdk_errors = Variable.process_config(
-            config_in,
+        config_in = Config(scl_env)
+        config_in, pdk_warnings, pdk_errors = config_in.__process_variable_list(
             pdk_variables,
+            [],
             pdk_removed_variables,
         )
 
         if len(pdk_errors) != 0:
             raise InvalidConfig("PDK configuration files", pdk_warnings, pdk_errors)
 
         if len(pdk_warnings) > 0:
@@ -485,7 +626,170 @@
                 info(
                     "Loading the PDK configuration files has generated the following warnings:"
                 )
                 for warning in pdk_warnings:
                     warn(warning)
 
         return (config_in, pdkpath, scl)
+
+    def __process_variable_list(
+        self,
+        variables: Sequence["Variable"],
+        strict_variables: Sequence["Variable"],
+        removed: Optional[Dict[str, str]] = None,
+        unknown_key_warn: bool = True,
+    ) -> Tuple["Config", List[str], List[str]]:
+        """
+        Verifies a configuration object against a list of variables, returning
+        an object with the variables normalized according to their types.
+
+        :param config: The input, raw configuration object.
+        :param variables: A sequence or some other iterable of variables.
+        :param removed: A dictionary of variables that may have existed at a point in
+            time, but then have gotten removed. Useful to give feedback to the user.
+        :returns: A tuple of:
+            [0] A final, processed configuration.
+            [1] A list of warnings.
+            [2] A list of errors.
+
+            If the third element is non-empty, the first object is invalid.
+        """
+        if removed is None:
+            removed = {}
+        warnings: List[str] = []
+        errors = []
+        final: GenericDict[str, Any] = GenericDict()
+        mutable = self.copy_mut()
+
+        # Special Deprecation Behaviors
+        if (
+            mutable.get("DIODE_INSERTION_STRATEGY") is not None
+        ):  # Can't use := because 0 is a valid value
+            dis = mutable["DIODE_INSERTION_STRATEGY"]
+            del mutable["DIODE_INSERTION_STRATEGY"]
+            try:
+                dis = int(dis)
+            except ValueError:
+                pass
+            if not isinstance(dis, int) or dis in [1, 2, 5] or dis > 6:
+                errors.append(
+                    f"DIODE_INSERTION_STRATEGY '{dis}' is not available in OpenLane 2 or higher. See 'Migrating DIODE_INSERTION_STRATEGY' in the docs for more info."
+                )
+            else:
+                warnings.append(
+                    "The DIODE_INSERTION_STRATEGY variable has been deprecated. See 'Migrating DIODE_INSERTION_STRATEGY' in the docs for more info."
+                )
+
+                mutable["GRT_REPAIR_ANTENNAS"] = False
+                mutable["RUN_HEURISTIC_DIODE_INSERTION"] = False
+                mutable["DIODE_ON_PORTS"] = "none"
+                if dis in [3, 6]:
+                    mutable["GRT_REPAIR_ANTENNAS"] = True
+                if dis in [4, 6]:
+                    mutable["RUN_HEURISTIC_DIODE_INSERTION"] = True
+                    mutable["DIODE_ON_PORTS"] = "in"
+
+        # Macros
+        translated_macros = False
+        if mutable.get("EXTRA_SPEFS") is not None and mutable.get("MACROS") is None:
+            mutable["MACROS"] = {}
+
+            extra_spef_list = mutable["EXTRA_SPEFS"]
+            del mutable["EXTRA_SPEFS"]
+            if isinstance(extra_spef_list, str):
+                extra_spef_list = extra_spef_list.split(" ")
+
+            if not isinstance(extra_spef_list, list):
+                errors.append(
+                    f"Invalid type for 'EXTRA_SPEFS': {type(extra_spef_list)}. It is recommended that you update your configuration to use the Macro object."
+                )
+            elif len(extra_spef_list) % 4 != 0:
+                errors.append(
+                    "Invalid value for 'EXTRA_SPEFS': Element count not divisible by four. It is recommended that you update your configuration to use the Macro object."
+                )
+            else:
+                translated_macros = True
+                warnings.append(
+                    "The configuration variable 'EXTRA_SPEFS' is deprecated. Check the docs on how to use the new 'MACROS' configuration variable."
+                )
+                for i in range(len(extra_spef_list) // 4):
+                    start = i * 4
+                    module, min, nom, max = (
+                        extra_spef_list[start],
+                        extra_spef_list[start + 1],
+                        extra_spef_list[start + 2],
+                        extra_spef_list[start + 3],
+                    )
+                    macro_dict = {
+                        "module": module,
+                        "gds": ["/dev/null"],
+                        "lef": ["/dev/null"],
+                    }
+                    macro_dict["spef"] = {
+                        "min_*": [min],
+                        "nom_*": [nom],
+                        "max_*": [max],
+                    }
+                    mutable["MACROS"][module] = macro_dict
+        elif (
+            mutable.get("EXTRA_SPEFS") is not None and mutable.get("MACROS") is not None
+        ):
+            errors.append(
+                "EXTRA_SPEFS cannot be defined simultaneously with its successor variable, MACROS"
+            )
+
+        for variable in variables:
+            try:
+                key, value_processed = variable.compile(
+                    mutable_config=mutable,
+                    warning_list_ref=warnings,
+                    values_so_far=final,
+                    permissive_typing=True,
+                )
+                if key is not None:
+                    del mutable[key]
+                final[variable.name] = value_processed
+            except ValueError as e:
+                errors.append(str(e))
+            if variable.name in mutable:
+                del mutable[variable.name]
+
+        for variable in strict_variables:
+            try:
+                key, value_processed = variable.compile(
+                    mutable_config=mutable,
+                    warning_list_ref=warnings,
+                    values_so_far=final,
+                    permissive_typing=False,
+                )
+                if key is not None:
+                    del mutable[key]
+                final[variable.name] = value_processed
+            except ValueError as e:
+                errors.append(str(e))
+            if variable.name in mutable:
+                del mutable[variable.name]
+
+        for key in sorted(mutable.keys()):
+            assert isinstance(key, str)
+
+            if key in vars(SpecialKeys).values():
+                continue
+            if key in removed:
+                warnings.append(f"'{key}' has been removed: {removed[key]}")
+            elif "_OPT" not in key and key != "//":
+                if unknown_key_warn:
+                    warnings.append(f"Unknown key '{key}' provided.")
+                else:
+                    errors.append(f"Unknown key '{key}' provided.")
+
+        if (
+            translated_macros and final.get("MACROS") is not None
+        ):  # Second check in case an error was generated
+            for macro in final["MACROS"].values():
+                assert isinstance(macro, Macro)
+                if "/dev/null" in macro.gds:
+                    macro.gds = [Path("")]
+                if "/dev/null" in macro.lef:
+                    macro.lef = [Path("")]
+
+        return (Config(final, meta=self.meta), warnings, errors)
```

### Comparing `openlane-2.0.0a9/openlane/config/flow.py` & `openlane-2.0.0b1/openlane/config/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from decimal import Decimal
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Union
 
-from .variable import Path, Variable, StringEnum
+from .variable import Variable, Macro
+from ..common import StringEnum, Path
 
 all_variables = [
     # Common
     Variable(
+        "DESIGN_DIR",
+        Path,
+        "The directory of the design. Does not need to be provided explicitly.",
+    ),
+    Variable(
         "DESIGN_NAME",
         str,
         "The name of the top level module of the design. This is the only required variable for all steps and all flows.",
     ),
     Variable(
         "PDK",
         str,
@@ -40,22 +46,21 @@
         Decimal,
         "The clock period for the design.",
         units="ns",
         default=10.0,
     ),
     Variable(
         "CLOCK_PORT",
-        Optional[str],
-        "The name of the design's clock port.",
+        Union[None, str, List[str]],
+        "The name(s) of the design's clock port(s).",
     ),
     Variable(
         "CLOCK_NET",
-        Optional[str],
-        "The name of the net input to root clock buffer.",
-        default="ref::$CLOCK_PORT",
+        Union[None, str, List[str]],
+        "The name of the net input to root clock buffer. If unset, it is presumed to be equal to CLOCK_PORT.",
     ),
     Variable(
         "VDD_NETS",
         Optional[List[str]],
         "Specifies the power nets/pins to be used when creating the power grid for the design.",
     ),
     Variable(
@@ -63,37 +68,42 @@
         Optional[List[str]],
         "Specifies the ground nets/pins to be used when creating the power grid for the design.",
     ),
     Variable(
         "DIE_AREA",
         Optional[str],
         'Specific die area to be used in floorplanning when `FP_SIZING` is set to `absolute`. Specified as a 4-corner rectangle "x0 y0 x1 y1".',
-        units="μm",
+        units="µm",
     ),
     # Macros
     Variable(
-        "EXTRA_VERILOG_MODELS",
+        "MACROS",
+        Optional[Dict[str, Macro]],
+        "A dictionary of Macro definition objects. See {py:class}`openlane.config.Macro` for more info.",
+    ),
+    Variable(
+        "EXTRA_LEFS",
         Optional[List[Path]],
-        "Black-boxed Verilog models of pre-hardened macros used in the current design, used in synthesis.",
-        deprecated_names=["VERILOG_FILES_BLACKBOX"],
+        "Specifies miscellaneous LEF files to be loaded indiscriminately whenever LEFs are loaded.",
     ),
     Variable(
-        "EXTRA_SPICE_MODELS",
+        "EXTRA_VERILOG_MODELS",
         Optional[List[Path]],
-        "Black-boxed SPICE models of pre-hardened macros used in the current design, used in LVS.",
+        "Specifies miscellaneous Verilog models to be loaded indiscriminately during synthesis.",
+        deprecated_names=["VERILOG_FILES_BLACKBOX"],
     ),
     Variable(
-        "EXTRA_LEFS",
+        "EXTRA_SPICE_MODELS",
         Optional[List[Path]],
-        "Specifies LEF files of pre-hardened macros used in the current design, used in placement and routing.",
+        "Miscellaneous SPICE files .",
     ),
     Variable(
         "EXTRA_LIBS",
         Optional[List[Path]],
-        "Specifies LIB files of pre-hardened macros used in the current design, used during timing analysis. (Optional).",
+        "Specifies LIB files of pre-hardened macros used in the current design, used during timing analyses (and during parasitics-based STA as a fallback). These are loaded indiscriminately for all timing corners.",
     ),
     Variable(
         "EXTRA_GDS_FILES",
         Optional[List[Path]],
         "Specifies GDS files of pre-hardened macros used in the current design, used during tape-out.",
     ),
     # Unimplemented - To be moved to steps
@@ -104,19 +114,14 @@
     ),
     Variable(
         "FP_CONTEXT_LEF",
         Optional[Path],
         "Points to the parent LEF file that includes this macro/design and uses this LEF file to determine the best locations for the pins. It must be used with `FP_CONTEXT_DEF`, otherwise it's considered non-existing. If not set, then the IO pins will be placed based on one of the other methods depending on the rest of the configurations.",
     ),
     Variable(
-        "SYNTH_USE_PG_PINS_DEFINES",
-        Optional[List[str]],
-        "Specifies the power guard used in the verilog source code to specify the power and ground pins. This is used to automatically extract `VDD_NETS` and `GND_NET` variables from the verilog, with the assumption that they will be order `inout vdd1, inout gnd1, inout vdd2, inout gnd2, ...`.",
-    ),
-    Variable(
         "FP_PADFRAME_CFG",
         Optional[str],
         "A configuration file passed to `padringer`, a padframe generator.",
     ),
     Variable(
         "GRT_OBS",
         Optional[List[str]],
@@ -149,20 +154,14 @@
     Variable(
         "LEC_ENABLE",
         bool,
         "Enables logic verification using yosys, for comparing each netlist at each stage of the flow with the previous netlist and verifying that they are logically equivalent. Warning: this will increase the runtime significantly.",
         default=False,
     ),
     Variable(
-        "CHECK_UNMAPPED_CELLS",
-        bool,
-        "Checks if there are unmapped cells after synthesis and aborts if any was found.",
-        default=True,
-    ),
-    Variable(
         "CHECK_ASSIGN_STATEMENTS",
         bool,
         "Checks for assign statement in the generated gate level netlist and aborts if any were found.",
         default=False,
     ),
 ]
 removed_variables: Dict[str, str] = {
@@ -173,10 +172,13 @@
     "MAGIC_GENERATE_GDS": "The GDS view is always generated when MAGIC_RUN_STREAMOUT is set.",
     "CLOCK_BUFFER_FANOUT": "The simple CTS script that used this variable no longer exists.",
     "FP_IO_HMETAL": "Replaced by FP_IO_HLAYER in the PDK configuration variables, which uses a more specific layer name.",
     "FP_IO_VMETAL": "Replaced by FP_IO_VLAYER in the PDK  configuration variables, which uses a more specific layer name.",
     "GLB_OPTIMIZE_MIRRORING": "Shares DPL_OPTIMIZE_MIRRORING.",
     "GRT_MAX_DIODE_INS_ITERS": "Relevant diode insertion strategies removed.",
     "TAKE_LAYOUT_SCROT": "Buggy/dubious utility.",
+    "MAGIC_PAD": "Hacky/dubious utility.",
     "GENERATE_FINAL_SUMMARY_REPORT": "To be specified via API/CLI- not much of a configuration variable.",
     "USE_GPIO_PADS": "Add the pad's files to EXTRA_LEFS and EXTRA_VERILOG_MODELS as apprioriate.",
+    "PL_ESTIMATE_PARASITICS": "Parasitics are always estimated whenever possible.",
+    "GRT_ESTIMATE_PARASITICS": "Parasitics are always estimated whenever possible.",
 }
```

### Comparing `openlane-2.0.0a9/openlane/config/resolve.py` & `openlane-2.0.0b1/openlane/config/preprocessor.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 import re
 import os
 import glob
 import fnmatch
 from enum import Enum
 from decimal import Decimal
 from types import SimpleNamespace
-from typing import Any, Dict, List, Tuple, Union, Optional
+from typing import Any, Dict, List, Mapping, Sequence, Tuple, Union, Optional
+
+from ..common import is_string
 
 Keys = SimpleNamespace(
     pdk_root="PDK_ROOT",
     pdk="PDK",
     pdkpath="PDKPATH",
     scl="STD_CELL_LIBRARY",
     design_dir="DESIGN_DIR",
@@ -31,28 +33,19 @@
 PROCESS_INFO_ALLOWLIST = [
     Keys.pdk,
     Keys.scl,
     f"{Keys.scl}_OPT",
 ]
 
 
-Scalar = Union[str, int, float, bool, None]
-
-
-class InvalidConfig(Exception):
-    pass
-
-
-State = dict
+Scalar = Union[str, int, Decimal, float, bool, None]
+Valid = Union[Scalar, dict, list]
 
 
 class Expr(object):
-    class SyntaxError(Exception):
-        pass
-
     class Token(object):
         class Type(Enum):
             VAR = 0
             NUMBER = 1
             OP = 2
             LPAREN = 3
             RPAREN = 4
@@ -79,15 +72,15 @@
                 raise TypeError(
                     f"pre-assoc not supported for non-token operators: '{self.value}'"
                 )
 
     @staticmethod
     def tokenize(expr: str) -> List["Expr.Token"]:
         rx_list = [
-            (re.compile(r"^\$(\w+)"), Expr.Token.Type.VAR),
+            (re.compile(r"^\$([A-Za-z_][A-Za-z0-9_\.\[\]]*)"), Expr.Token.Type.VAR),
             (re.compile(r"^(-?\d+\.?\d*)"), Expr.Token.Type.NUMBER),
             (re.compile(r"^(\*\*)"), Expr.Token.Type.OP),
             (re.compile(r"^(\+|\-|\*|\/)"), Expr.Token.Type.OP),
             (re.compile(r"^(\()"), Expr.Token.Type.LPAREN),
             (re.compile(r"^(\))"), Expr.Token.Type.RPAREN),
             (re.compile(r"^\s+"), None),
         ]
@@ -110,15 +103,15 @@
             if not found:
                 raise SyntaxError(
                     f"Unexpected token at the start of the following string '{str_so_far}'."
                 )
         return tokens
 
     @staticmethod
-    def evaluate(expression: str, vars: Dict[str, str]) -> float:
+    def evaluate(expression: str, symbols: Mapping[str, Any]) -> Decimal:
         tokens: List["Expr.Token"] = Expr.tokenize(expression)
         ETT = Expr.Token.Type
 
         # Infix to Postfix
         postfix: List["Expr.Token"] = []
         opstack: List["Expr.Token"] = []
         for token in tokens:
@@ -159,252 +152,301 @@
             postfix.append(opstack[-1])
             opstack.pop()
 
         # Evaluate
         eval_stack = []
         for token in postfix:
             if token.type == ETT.NUMBER:
-                eval_stack.append(float(token.value))
+                eval_stack.append(Decimal(token.value))
             elif token.type == ETT.VAR:
                 try:
-                    value = vars[token.value]
-                    eval_stack.append(float(value))
+                    value = symbols[token.value]
+                    if not (
+                        isinstance(value, int)
+                        or isinstance(value, float)
+                        or isinstance(value, Decimal)
+                    ):
+                        raise TypeError(
+                            f"Referenced variable {token.value} is not of a valid numeric type: f{type(value)}"
+                        )
+                    eval_stack.append(Decimal(value))
                 except KeyError:
-                    raise SyntaxError(
+                    raise TypeError(
                         f"Configuration variable '{token.value}' not found."
                     )
-                except Exception:
-                    raise SyntaxError(
-                        f"Invalid non-numeric value '{value}' for variable ${token.value}."
-                    )
             elif token.type == ETT.OP:
                 try:
                     number1 = eval_stack[-2]
                     number2 = eval_stack[-1]
                     eval_stack.pop()
                     eval_stack.pop()
 
-                    result = 0.0
+                    result = Decimal(0.0)
                     if token.value == "**":
                         result = number1**number2
                     elif token.value == "*":
                         result = number1 * number2
                     elif token.value == "/":
                         result = number1 / number2
                     elif token.value == "+":
                         result = number1 + number2
                     elif token.value == "-":
                         result = number1 + number2
 
                     eval_stack.append(result)
                 except IndexError:
                     raise SyntaxError(
-                        f"Not enough operands for operator '{token.value}'."
+                        f"not enough operands for operator '{token.value}'"
                     )
 
         if len(eval_stack) > 1:
-            raise SyntaxError("Expression does not reduce to one value.")
+            raise ValueError("expression reduces to multiple values")
         elif len(eval_stack) == 0:
-            raise SyntaxError("Expression is empty.")
+            raise ValueError("expression is empty")
 
         return eval_stack[0]
 
 
-ref_rx = re.compile(r"^\$([A-Za-z_][A-Za-z0-9_]*)")
+ref_rx = re.compile(r"^\$([A-Za-z_][A-Za-z0-9_\.\[\]]*)")
 
 
-def process_string(value: str, state: State) -> Optional[str]:
+def process_string(
+    value: str,
+    symbols: Mapping[str, Any],
+    readable_paths: Optional[List[str]] = None,
+) -> Valid:
     global ref_rx
     EXPR_PREFIX = "expr::"
     REF_PREFIX = "ref::"
+    REFG_PREFIX = "refg::"
 
     DIR_PREFIX = "dir::"
     PDK_DIR_PREFIX = "pdk_dir::"
 
+    mutable: str = value
+
     if value.startswith(DIR_PREFIX):
-        value = value.replace(DIR_PREFIX, f"ref::${Keys.design_dir}/")
+        mutable = value.replace(DIR_PREFIX, f"refg::${Keys.design_dir}/")
     elif value.startswith(PDK_DIR_PREFIX):
-        value = value.replace(PDK_DIR_PREFIX, f"ref::${Keys.pdkpath}/")
+        mutable = value.replace(PDK_DIR_PREFIX, f"refg::${Keys.pdkpath}/")
 
-    if value.startswith(EXPR_PREFIX):
+    if mutable.startswith(EXPR_PREFIX):
         try:
-            value = f"{Expr.evaluate(value[len(EXPR_PREFIX):], state)}"
+            return Expr.evaluate(value[len(EXPR_PREFIX) :], symbols)
         except SyntaxError as e:
-            raise InvalidConfig(f"Invalid expression '{value}': {e}")
-    elif value.startswith(REF_PREFIX):
-        reference = value[len(REF_PREFIX) :]
+            raise SyntaxError(f"Invalid expression '{value}': {e}") from None
+    elif mutable.startswith(REF_PREFIX) or mutable.startswith(REFG_PREFIX):
+        reference = mutable[mutable.index("::") + 2 :]
         match = ref_rx.match(reference)
         if match is None:
-            raise InvalidConfig(f"Invalid reference string '{reference}'")
+            raise SyntaxError(f"Invalid reference string '{reference}'") from None
+
         reference_variable = match[1]
-        try:
-            found = state[reference_variable]
-            if found is None:
-                return None
-
-            if type(found) != str:
-                if type(found) in [int, float]:
-                    raise InvalidConfig(
-                        f"Referenced variable {reference_variable} is a number and not a string: use expr::{match[0]} if you want to reference this number."
-                    )
-                else:
-                    raise InvalidConfig(
-                        f"Referenced variable {reference_variable} is not a string: {type(found)}."
-                    )
+        if reference_variable not in symbols:
+            raise KeyError(
+                f"Referenced variable '{reference_variable}' not found"
+            ) from None
+
+        target = symbols[reference_variable]
+        if target is None:
+            return None
 
-            value = reference.replace(match[0], found)
+        if not is_string(target):
+            if type(target) in [int, float, Decimal]:
+                raise TypeError(
+                    f"Referenced variable {reference_variable} is a number and not a string: use expr::{match[0]} if you want to reference this number."
+                ) from None
+            else:
+                raise TypeError(
+                    f"Referenced variable {reference_variable} is not a valid string: {type(target)}."
+                ) from None
 
-            found_abs = os.path.abspath(found)
-            full_abspath = os.path.abspath(value)
+        target = str(target)
+        concatenated = reference.replace(match[0], target)
 
-            # Resolve globs for paths that are inside the exposed directory
-            if full_abspath.startswith(found_abs):
-                files = glob.glob(full_abspath)
-                files_escaped = [file.replace("$", r"\$") for file in files]
-                if len(files_escaped) != 0:
-                    value = " ".join(files_escaped)
-        except KeyError:
-            raise InvalidConfig(
-                f"Referenced variable '{reference_variable}' not found."
+        # Glob only if Refg
+        if not mutable.startswith(REFG_PREFIX):
+            return concatenated
+
+        # Glob only if readable_paths isn't null
+        if readable_paths is None:
+            return target
+
+        final_abspath = os.path.abspath(concatenated)
+        in_exposed = [final_abspath.startswith(p) for p in readable_paths]
+        if True not in in_exposed:
+            raise PermissionError(
+                f"'{concatenated}' is not located any path readable to OpenLane"
+            )
+        files = glob.glob(final_abspath)
+        files_escaped = [file.replace("$", r"\$") for file in files]
+        files_escaped.sort()
+        return files_escaped
+    else:
+        return mutable
+
+
+PDK_PREFIX = "pdk::"
+SCL_PREFIX = "scl::"
+
+
+def process_list_recursive(
+    input: Sequence[Any],
+    ref: List[Any],
+    symbols: Dict[str, Any],
+    readable_paths: Optional[List[str]],
+    /,
+    key_path: str = "",
+):
+    for i, value in enumerate(input):
+        current_key_path = f"{key_path}[{i}]"
+        processed: Any = None
+        if isinstance(value, Mapping):
+            processed = {}
+            process_dict_recursive(
+                value,
+                processed,
+                symbols,
+                readable_paths,
+                key_path=current_key_path,
+            )
+        elif isinstance(value, Sequence) and not is_string(value):
+            processed = []
+            process_list_recursive(
+                value,
+                processed,
+                symbols,
+                readable_paths,
+                key_path=current_key_path,
             )
-    return value
+        elif is_string(value):
+            processed = process_string(value, symbols, readable_paths)
+        else:
+            processed = value
+
+        if processed is not None:
+            ref.append(processed)
+            symbols[current_key_path] = processed
 
 
-def process_scalar(key: str, value: Scalar, state: State) -> Scalar:
-    if isinstance(value, str):
-        value = process_string(value, state)
-    elif value is None:
-        value = ""
-    elif not (
-        isinstance(value, bool)
-        or isinstance(value, int)
-        or isinstance(value, float)
-        or isinstance(value, Decimal)
-    ):
-        raise InvalidConfig(f"Invalid value type {type(value)} for key '{key}'.")
-
-    return value
-
-
-def process_config_dict_recursive(config_in: Dict[str, Any], state: State):
-    PDK_PREFIX = "pdk::"
-    SCL_PREFIX = "scl::"
-
-    for key, value in config_in.items():
-        withhold = False
-        if not isinstance(key, str):
-            raise InvalidConfig(f"Invalid key {key}: must be a string.")
-        if isinstance(value, dict):
-            withhold = True
+def process_dict_recursive(
+    input: Mapping[str, Any],
+    ref: Dict[str, Any],
+    symbols: Dict[str, Any],
+    readable_paths: Optional[List[str]],
+    /,
+    key_path: str = "",
+):
+    for key, value in input.items():
+        current_key_path = key
+        if key_path != "":
+            current_key_path = f"{key_path}.{key}"
+        processed: Any = None
+        if isinstance(value, Mapping):
             if key.startswith(PDK_PREFIX):
                 pdk_match = key[len(PDK_PREFIX) :]
-                if fnmatch.fnmatch(state[Keys.pdk], pdk_match):
-                    process_config_dict_recursive(value, state)
+                if fnmatch.fnmatch(ref[Keys.pdk], pdk_match):
+                    process_dict_recursive(
+                        value,
+                        ref,
+                        symbols,
+                        readable_paths,
+                        key_path=key_path,
+                    )
             elif key.startswith(SCL_PREFIX):
                 scl_match = key[len(SCL_PREFIX) :]
-                if state[Keys.scl] is not None and fnmatch.fnmatch(
-                    state[Keys.scl], scl_match
+                if ref[Keys.scl] is not None and fnmatch.fnmatch(
+                    ref[Keys.scl], scl_match
                 ):
-                    process_config_dict_recursive(value, state)
+                    process_dict_recursive(
+                        value,
+                        ref,
+                        symbols,
+                        readable_paths,
+                        key_path=key_path,
+                    )
             else:
-                raise InvalidConfig(
-                    f"Invalid value type {type(value)} for key '{key}'."
+                processed = {}
+                process_dict_recursive(
+                    value,
+                    processed,
+                    symbols,
+                    readable_paths,
+                    key_path=current_key_path,
                 )
-        elif isinstance(value, list):
-            valid = True
+
+        elif isinstance(value, Sequence) and not is_string(value):
             processed = []
-            for i, item in enumerate(value):
-                current_key = f"{key}[{i}]"
-                processed.append(f"{process_scalar(current_key, item, state)}")
-
-            if not valid:
-                raise InvalidConfig(
-                    f"Invalid value for key '{key}': Arrays must consist only of strings."
-                )
-            value = " ".join(processed)
+            process_list_recursive(
+                value,
+                processed,
+                symbols,
+                readable_paths,
+                key_path=current_key_path,
+            )
+        elif is_string(value):
+            processed = process_string(value, symbols, readable_paths)
         else:
-            value = process_scalar(key, value, state)
+            processed = value
 
-        if not withhold:
-            state[key] = value
+        if processed is not None:
+            ref[key] = processed
+            symbols[current_key_path] = processed
 
 
-def process_config_dict(config_in: dict, exposed_variables: Dict[str, str]):
-    state = State(exposed_variables)
-    process_config_dict_recursive(config_in, state)
+def process_config_dict(
+    config_in: Mapping[str, Any],
+    exposed_variables: Dict[str, Any],
+    readable_paths: Optional[List[str]],
+) -> Dict[str, Any]:
+    state = dict(exposed_variables)
+    symbols = dict(exposed_variables)
+    process_dict_recursive(config_in, state, symbols, readable_paths)
     return state
 
 
 def extract_process_vars(config_in: Dict[str, str]) -> Dict[str, str]:
     return {
         key: config_in[key]
         for key in PROCESS_INFO_ALLOWLIST
         if config_in.get(key) is not None and config_in.get(key) != ""
     }
 
 
-def resolve(
-    config_dict: Dict[str, Any],
+def preprocess_dict(
+    config_dict: Mapping[str, Any],
     design_dir: str,
     only_extract_process_info: bool = False,
-    exposing: Optional[List[str]] = None,
     pdk: Optional[str] = None,
     pdkpath: Optional[str] = None,
     scl: Optional[str] = None,
-):
-    if exposing is None:
-        exposing = []
-
-    exposed_dict = {}
-
-    implicitly_exposed = [
-        Keys.pdk,
-        Keys.pdkpath,
-        Keys.scl,
-        Keys.design_dir,
-    ]
-    if only_extract_process_info:
-        implicitly_exposed = [Keys.design_dir]
-
-        # So we don't crash on conditional processing:
-        def coalesce(variable_name: str):
-            nonlocal implicitly_exposed, exposed_dict
-            if os.environ.get(variable_name) is not None:
-                implicitly_exposed += [variable_name]
-            else:
-                exposed_dict[variable_name] = ""
-
-        for variable in [
-            Keys.pdk,
-            Keys.pdkpath,
-            Keys.scl,
-        ]:
-            coalesce(variable)
+    readable_paths: Optional[List[str]] = None,
+) -> Dict[str, Any]:
+    """
+    If readable_paths are set to None, refg:: will not work
+    """
+    if None in (pdk, pdkpath, scl):
+        if only_extract_process_info:
+            pdkpath = ""
+            scl = ""
+            pdk = ""
+        else:
+            raise TypeError(
+                "pdk, pdkpath and scl all need to be non-None unless only_extract_process_info is passed"
+            )
 
     base_vars = {
         Keys.pdk: pdk,
         Keys.pdkpath: pdkpath,
         Keys.scl: scl,
         Keys.design_dir: design_dir,
     }
-    base_vars_clean = {k: v for k, v in base_vars.items() if v is not None}
-
-    env_copy = os.environ.copy()
-    env_copy.update(base_vars_clean)
-
-    exposed = list(exposing) + implicitly_exposed
-    for key in exposed:
-        if value := env_copy.get(key):
-            exposed_dict[key] = value
-
-    for key in implicitly_exposed:
-        if exposed_dict.get(key) is None:
-            raise ValueError(
-                f"{key} environment variable must be set.",
-            )
 
-    resolved = process_config_dict(config_dict, exposed_dict)
+    preprocessed = process_config_dict(
+        config_dict,
+        base_vars,
+        readable_paths,
+    )
     if only_extract_process_info:
-        resolved = extract_process_vars(resolved)
+        preprocessed = extract_process_vars(preprocessed)
 
-    resolved.update(base_vars_clean)
-    return resolved
+    return preprocessed
```

### Comparing `openlane-2.0.0a9/openlane/config/tcleval.py` & `openlane-2.0.0b1/openlane/common/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,55 +7,62 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+Common Utilities Module
+-----------------------
+
+A number of common utility functions and classes used throughout the codebase.
+"""
 import os
-import tkinter
-import tempfile
-from decimal import Decimal, InvalidOperation
-
-from .config import Config
-
-
-def env_from_tcl(env_in: Config, tcl_in: str) -> Config:
-    interpreter = tkinter.Tcl()
-
-    initial_env = os.environ.copy()
-    env_out = env_in.copy()
-
-    with tempfile.NamedTemporaryFile("r+") as f:
-        env_str = ""
-        unset_env_str = ""
-        for key, value in env_in.items():
-            env_str += f"set ::env({key}) {{{value}}}\n"
-            unset_env_str += f"unset ::env({key})\n"
-
-        tcl_script = f"""
-        {env_str}
-        {tcl_in}
-        set f [open {f.name} WRONLY]
-        foreach key [array names ::env] {{
-            puts $f "$key $::env($key)\\0"
-        }}
-        close $f
-        {unset_env_str}
-        """
-        interpreter.eval(tcl_script)
-
-        f.seek(0)
-        env_strings = f.read()
-
-        for line in env_strings.split("\0\n"):
-            if line.strip() == "":
-                continue
-            key, value = line.split(" ", 1)
-            try:
-                value = Decimal(value)
-            except InvalidOperation:
-                pass
-            if initial_env.get(key) is None and env_in.get(key) != value:
-                env_out[key] = value
+from concurrent.futures import ThreadPoolExecutor
 
-    return env_out
+from .tcl import TclUtils
+from .metrics import parse_metric_modifiers, aggregate_metrics
+from .generic_dict import (
+    GenericDictEncoder,
+    GenericDict,
+    GenericImmutableDict,
+    copy_recursive,
+    is_string,
+)
+from .misc import (
+    idem,
+    get_openlane_root,
+    get_script_dir,
+    get_opdks_rev,
+    slugify,
+    protected,
+    final,
+    mkdirp,
+    StringEnum,
+    Path,
+    zip_first,
+)
+
+
+## TPE
+
+TPE = ThreadPoolExecutor(max_workers=os.cpu_count())
+
+
+def set_tpe(tpe: ThreadPoolExecutor):
+    """
+    Allows replacing OpenLane's global ``ThreadPoolExecutor`` with a customized
+    one.
+
+    :param tpe: The replacemend ThreadPoolExecutor
+    """
+    global TPE
+    TPE = tpe
+
+
+def get_tpe() -> ThreadPoolExecutor:
+    """
+    :returns: OpenLane's global ``ThreadPoolExecutor``
+    """
+    global TPE
+    return TPE
```

### Comparing `openlane-2.0.0a9/openlane/container.py` & `openlane-2.0.0b1/openlane/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+## This file is internal to OpenLane 2 and is not part of the API.
+
 import os
 import re
+import shlex
 import pathlib
 import getpass
 import tempfile
 import requests
 import subprocess
-from typing import List, Sequence, Set, Optional, Union, Tuple
+from typing import List, Sequence, Optional, Union, Tuple
 
-from .logging import err, info, print, warn
+from .logging import err, info, warn
 from .env_info import OSInfo
 
 CONTAINER_ENGINE = os.getenv("OPENLANE_CONTAINER_ENGINE", "docker")
 
 
 def permission_args(osinfo: OSInfo) -> List[str]:
     if (
@@ -95,15 +99,14 @@
         tag = elements[1]
 
     url = None
     if registry == "docker.io":
         url = f"https://registry.hub.docker.com/v2/repositories/{repo}/tags/{tag}"
     elif registry == "ghcr.io":
         url = f"https://ghcr.io/v2/{repo}/manifests/{tag}"
-        print(url)
     else:
         err(f"Unknown registry '{registry}'.")
         return False
 
     try:
         request = requests.get(url, headers={"Accept": "application/json"})
         request.raise_for_status()
@@ -127,43 +130,39 @@
     except subprocess.CalledProcessError:
         err(f"Failed to pull image {image} from the container registries.")
         return False
 
     return True
 
 
-docker_ids: Set[str] = set()
-
 win_path_sep = re.compile(r"\\")
 
 
 def sanitize_path(path: Union[str, os.PathLike]) -> Tuple[str, str]:
     path_str = str(path)
     abspath = os.path.abspath(path_str)
     mountable_path = abspath
-    print()
     if os.path.sep == "\\":
         mountable_path = win_path_sep.sub("/", abspath)[2:]
     return (abspath, mountable_path)
 
 
 def run_in_container(
     image: str,
     args: Sequence[str],
-    pdk_root: Optional[str],
-    pdk: Optional[str],
-    scl: Optional[str],
-    other_mounts: Optional[Sequence[str]],
-):
+    pdk_root: Optional[str] = None,
+    pdk: Optional[str] = None,
+    scl: Optional[str] = None,
+    other_mounts: Optional[Sequence[str]] = None,
+    interactive: bool = False,
+) -> int:
     # If imported at the top level, would interfere with Conda where Volare
     # would not be installed.
     import volare
 
-    global docker_ids
-
     osinfo = OSInfo.get()
     if not osinfo.supported:
         warn(
             f"Unsupported host operating system '{osinfo.kernel}'. You may encounter unexpected issues."
         )
 
     if osinfo.container_info is None:
@@ -195,46 +194,44 @@
         ]
 
     from_cwd, to_cwd = sanitize_path(os.getcwd())
     if not from_cwd.startswith(from_home):
         mount_args += ["-v", f"{from_cwd}:{to_cwd}"]
     mount_args += ["-w", to_cwd]
 
+    tempdir = tempfile.mkdtemp("openlane_docker")
+
     mount_args += [
         "-v",
-        f"{tempfile.gettempdir()}:/tmp",
+        f"{tempdir}:/tmp",
         "-e",
         "TMPDIR=/tmp",
     ]
 
     if other_mounts is not None:
         for mount in other_mounts:
             mount_from, mount_to = sanitize_path(mount)
             mount_args += ["-v", f"{mount_from}:{mount_to}"]
 
     cmd = (
         [
             CONTAINER_ENGINE,
             "run",
             "--rm",
-            "-t",
+            "-ti" if interactive else "-t",
         ]
         + permission_args(osinfo)
         + mount_args
         + gui_args(osinfo)
         + [image]
         + list(args)
     )
 
-    cmd_escaped = []
-    for el in cmd:
-        if " " in cmd:
-            cmd_escaped.append(f"'{cmd}'")
-        else:
-            cmd_escaped.append(el)
-
     info("Running containerized command:")
-    print(" ".join(cmd_escaped))
-    subprocess.check_call(
+    print(shlex.join(cmd))
+
+    result = subprocess.call(
         cmd,
         stderr=subprocess.STDOUT,
     )
+
+    return result
```

### Comparing `openlane-2.0.0a9/openlane/env_info.py` & `openlane-2.0.0b1/openlane/env_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Note: This file may be run with no dependencies installed as part of
 # environment surveys. Please ensure all code as compatible as possible
 # with ancient versions of Python.
 
+## This file is internal to OpenLane 2 and is not part of the API.
+import os
 import re
 import sys
 import json
 import platform
 import subprocess
 
 try:
     from typing import Optional  # noqa: F401
 except ImportError:
     pass
 
+CONTAINER_ENGINE = os.getenv("OPENLANE_CONTAINER_ENGINE", "docker")
+
 
 class StringRepresentable(object):
     def __str__(self):
         return str(self.__dict__)
 
     def __repr__(self):
         return str(self.__dict__)
@@ -54,15 +58,15 @@
     def get():
         # type: () -> Optional['ContainerInfo']
         try:
             cinfo = ContainerInfo()
 
             try:
                 info_str = subprocess.check_output(
-                    ["docker", "info", "--format", "{{json .}}"]
+                    [CONTAINER_ENGINE, "info", "--format", "{{json .}}"]
                 ).decode("utf8")
             except Exception:
                 return None
 
             try:
                 info = json.loads(info_str)
             except Exception:
@@ -83,15 +87,15 @@
                 or info.get("DockerRootDir") is not None
             ):
                 cinfo.engine = "docker"
 
                 # Get Version
                 try:
                     version_output = (
-                        subprocess.check_output(["docker", "--version"])
+                        subprocess.check_output([CONTAINER_ENGINE, "--version"])
                         .decode("utf8")
                         .strip()
                     )
                     cinfo.version = re.split(r"\s", version_output)[2].strip(",")
                 except Exception:
                     print("Could not extract Docker version.", file=sys.stderr)
```

### Comparing `openlane-2.0.0a9/openlane/flows/__init__.py` & `openlane-2.0.0b1/openlane/scripts/openroad/basic_mp.tcl`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Copyright 2023 Efabless Corporation
+# Copyright 2020-2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-The Flow Module
+source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+read_current_odb
 
-An API for implementing new flows using the OpenLane infrastructure, as well
-as a number of built-in flows.
-"""
-from . import builtins
-from .flow import Flow, FlowException, FlowError
-from .sequential import SequentialFlow
+macro_placement\
+    -channel $::env(PL_MACRO_CHANNEL)\
+    -halo $::env(PL_MACRO_HALO)
+
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/flows/builtins.py` & `openlane-2.0.0b1/openlane/flows/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Built-in Flows
+The Flow Module
+---------------
 
-A list of flows that are included with the OpenLane infrastructure, serving as
-defaults and examples.
+An API for implementing new flows using the OpenLane infrastructure, as well
+as a number of built-in flows.
 """
-
-# flake8: noqa
-from .optimizing import Optimizing
-from .classic import Classic
-from .misc import OpenInKLayout, OpenInOpenROAD
+from .flow import FlowError, FlowException, FlowProgressBar, Flow
+from .sequential import SequentialFlow
+from . import builtins
+from .cli import cloup_flow_opts
```

### Comparing `openlane-2.0.0a9/openlane/flows/classic.py` & `openlane-2.0.0b1/openlane/flows/classic.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,49 +28,63 @@
 from .flow import Flow
 from .sequential import SequentialFlow
 
 
 @Flow.factory.register()
 class Classic(SequentialFlow):
     """
-    The flow most similar to the original Tcl-based OpenLane.
+    A flow of type :class:`openlane.flows.SequentialFlow` that is the most
+    similar to the original OpenLane 1.0 flow, running the Verilog RTL through
+    Yosys, OpenROAD, KLayout and Magic to produce a valid GDSII for simpler designs.
+
+    This is the default when using OpenLane via the command-line.
     """
 
     Steps: List[Type[Step]] = [
+        Yosys.JsonHeader,
         Yosys.Synthesis,
         Checker.YosysUnmappedCells,
+        Checker.YosysSynthChecks,
         Misc.LoadBaseSDC,
-        OpenROAD.NetlistSTA,
+        OpenROAD.STAPrePNR,
         OpenROAD.Floorplan,
+        Odb.SetPowerConnections,
         Odb.ManualMacroPlacement,
-        Odb.ApplyDEFTemplate,
-        OpenROAD.TapDecapInsertion,
+        OpenROAD.TapEndcapInsertion,
         OpenROAD.IOPlacement,
         Odb.CustomIOPlacement,
         OpenROAD.GeneratePDN,
         OpenROAD.GlobalPlacement,
+        OpenROAD.STAMidPNR,
         Odb.DiodesOnPorts,
         Odb.HeuristicDiodeInsertion,
         OpenROAD.RepairDesign,
         OpenROAD.DetailedPlacement,
         OpenROAD.CTS,
+        OpenROAD.STAMidPNR,
         OpenROAD.ResizerTimingPostCTS,
+        OpenROAD.STAMidPNR,
         OpenROAD.GlobalRouting,
         OpenROAD.ResizerTimingPostGRT,
+        OpenROAD.STAMidPNR,
         OpenROAD.DetailedRouting,
         Checker.TrDRC,
+        Odb.ReportDisconnectedPins,
+        Checker.DisconnectedPins,
         Odb.ReportWireLength,
         Checker.WireLength,
         OpenROAD.FillInsertion,
-        OpenROAD.ParasiticsExtraction,
-        OpenROAD.ParasiticsSTA,
+        OpenROAD.RCX,
+        OpenROAD.STAPostPNR,
         OpenROAD.IRDropReport,
         Magic.StreamOut,
         KLayout.StreamOut,
+        Magic.WriteLEF,
         KLayout.XOR,
+        Checker.XOR,
         Magic.DRC,
         Checker.MagicDRC,
         Magic.SpiceExtraction,
         Checker.IllegalOverlap,
         Netgen.LVS,
         Checker.LVS,
     ]
```

### Comparing `openlane-2.0.0a9/openlane/flows/misc.py` & `openlane-2.0.0b1/openlane/steps/misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,111 +7,54 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from __future__ import annotations
-
 import os
-import sys
-import tempfile
-import subprocess
-from typing import List, Tuple
-
-from .flow import Flow
-from ..common import get_script_dir
-from ..state import State
-from ..steps import Step, KLayout
-
-
-@Flow.factory.register()
-class OpenInKLayout(Flow):
-    """
-    This 'flow' actually just opens the LEF/DEF from the initial state object
-    in KLayout. Fancy that.
-
-    Intended for use with run tags that have already been run with
-    another flow.
-    """
-
-    Steps = [KLayout.StreamOut]
+from typing import Optional, Tuple
 
-    name = "Opening in KLayout"
+from ..logging import info
+from ..config import Variable
+from ..state import State, DesignFormat
+from ..common import Path, get_script_dir
+from .step import ViewsUpdate, MetricsUpdate, Step
 
-    def run(
-        self,
-        initial_state: State,
-        **kwargs,
-    ) -> Tuple[State, List[Step]]:
-        self.set_max_stage_count(1)
-        self.start_stage("Opening in KLayout")
-
-        lefs = ["--input-lef", self.config["TECH_LEF"]]
-        for lef in self.config["CELL_LEFS"]:
-            lefs.append("--input-lef")
-            lefs.append(lef)
-        if extra_lefs := self.config["EXTRA_LEFS"]:
-            for lef in extra_lefs:
-                lefs.append("--input-lef")
-                lefs.append(lef)
-
-        subprocess.check_call(
-            [
-                sys.executable,
-                os.path.join(
-                    get_script_dir(),
-                    "klayout",
-                    "open_design.py",
-                ),
-                "--lyt",
-                self.config["KLAYOUT_TECH"],
-                "--lyp",
-                self.config["KLAYOUT_PROPERTIES"],
-                "--lym",
-                self.config["KLAYOUT_DEF_LAYER_MAP"],
-                initial_state["def"],
-            ]
-            + lefs
-        )
-        self.end_stage()
-
-        return (initial_state, [])
 
-
-@Flow.factory.register()
-class OpenInOpenROAD(Flow):
+@Step.factory.register()
+class LoadBaseSDC(Step):
     """
-    This 'flow' actually just opens the ODB from the initial state object
-    in the OpenROAD GUI.
-
-    Intended for use with run tags that have already been run with
-    another flow.
+    Loads an SDC file specified as a configuration variable into the state
+    object unaltered.
     """
 
-    name = "Opening in OpenROAD"
-
-    Steps = []
-
-    def run(
-        self,
-        initial_state: State,
-        **kwargs,
-    ) -> Tuple[State, List[Step]]:
-        self.set_max_stage_count(1)
-
-        with tempfile.NamedTemporaryFile("a+", suffix=".tcl") as f:
-            f.write(f"read_db \"{initial_state['odb']}\"")
-            f.flush()
-
-            subprocess.check_call(
-                [
-                    "openroad",
-                    "-no_splash",
-                    "-gui",
-                    f.name,
-                ]
+    id = "Misc.LoadBaseSDC"
+    name = "Load Base SDC"
+    long_name = "Load Base Design Constraints File"
+
+    inputs = []
+    outputs = [DesignFormat.SDC]
+
+    config_vars = [
+        Variable(
+            "BASE_SDC_FILE",
+            Optional[Path],
+            "Specifies the base SDC file to source before running Static Timing Analysis.",
+            deprecated_names=["SDC_FILE"],
+        ),
+    ]
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        path = Path(
+            os.path.join(
+                get_script_dir(),
+                "base.sdc",
             )
-        self.end_stage()
+        )
+        if self.config.get("BASE_SDC_FILE") is not None:
+            info(f"Loading SDC file at '{self.config['BASE_SDC_FILE']}'.")
+            path = self.config["BASE_SDC_FILE"]
+        else:
+            info("Loading default SDC file.")
 
-        return (initial_state, [])
+        return {DesignFormat.SDC: path}, {}
```

### Comparing `openlane-2.0.0a9/openlane/flows/optimizing.py` & `openlane-2.0.0b1/openlane/flows/optimizing.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
-import subprocess
 from typing import List, Tuple
 from concurrent.futures import Future
 
 from .flow import Flow
-from ..logging import get_log_level, set_log_level, LogLevels, success, info
 from ..state import State
-from ..steps import Step, Yosys, OpenROAD
 from ..config import Config
+from ..steps import Step, Yosys, OpenROAD, Misc, StepError
+from ..logging import get_log_level, set_log_level, LogLevels, success, info
 
 
+#   "Optimizing" is a custom demo flow to show what's possible with non-sequential Flows in OpenLane 2+.
+#   It works across two steps:
+#   * The Synthesis Exploration - tries multiple synthesis strategies in *parallel*.
+#       The best-performing strategy in terms of minimizing the area makes it to the next stage.
+#   * Floorplanning and Placement - tries FP and placement with a high utilization.
+#       If the high utilization fails, a lower is fallen back to as a suggestion.
 @Flow.factory.register()
 class Optimizing(Flow):
-    """
-    A customized flow composed of two stages:
-
-    * The Synthesis Exploration - tries multiple synthesis strategies in *parallel*.
-
-    The best-performing strategy in terms of minimizing the area makes it to the next stage.
-
-    * Floorplanning and Placement - tries FP and placement with a high utilization.
-
-    If the high utilization fails, a lower is fallen back to as a suggestion.
-    """
-
     Steps = [
         Yosys.Synthesis,
-        OpenROAD.NetlistSTA,
+        Misc.LoadBaseSDC,
+        OpenROAD.STAPrePNR,
         OpenROAD.Floorplan,
         OpenROAD.IOPlacement,
         OpenROAD.GlobalPlacement,
     ]
 
     def run(
         self,
@@ -58,29 +52,37 @@
         synthesis_futures: List[Tuple[Config, Future[State]]] = []
         self.start_stage("Synthesis Exploration")
 
         log_level_bk = get_log_level()
         set_log_level(LogLevels.ERROR)
 
         for strategy in ["AREA 0", "AREA 2", "DELAY 1"]:
-            config = self.config.copy()
-            config["SYNTH_STRATEGY"] = strategy
+            config = self.config.copy(SYNTH_STRATEGY=strategy)
 
             synth_step = Yosys.Synthesis(
                 config,
                 id=f"synthesis-{strategy}",
                 state_in=initial_state,
                 flow=self,
             )
             synth_future = self.start_step_async(synth_step)
             step_list.append(synth_step)
 
-            sta_step = OpenROAD.NetlistSTA(
+            sdc_step = Misc.LoadBaseSDC(
                 config,
+                id=f"sdc-{strategy}",
                 state_in=synth_future,
+                flow=self,
+            )
+            sdc_future = self.start_step_async(sdc_step)
+            step_list.append(sdc_step)
+
+            sta_step = OpenROAD.STAPrePNR(
+                config,
+                state_in=sdc_future,
                 id=f"sta-{strategy}",
                 flow=self,
             )
 
             step_list.append(sta_step)
             sta_future = self.start_step_async(sta_step)
 
@@ -106,73 +108,72 @@
                 min_strat = strategy
                 min_config = config
 
         info(f"Using result from '{min_strat}…")
 
         self.start_stage("Floorplanning and Placement")
 
-        fp_config = min_config.copy()
-        fp_config["FP_CORE_UTIL"] = 99
+        fp_config = min_config.copy(FP_CORE_UTIL=99)
         fp = OpenROAD.Floorplan(
             fp_config,
             state_in=min_area_state,
             id="fp_highutl",
             long_name="Floorplanning (High Util)",
             flow=self,
         )
-        fp.start()
+        self.start_step(fp)
         step_list.append(fp)
         try:
             io = OpenROAD.IOPlacement(
                 fp_config,
                 state_in=fp.state_out,
                 id="io-highutl",
                 long_name="I/O Placement (High Util)",
                 flow=self,
             )
-            io.start()
+            self.start_step(io)
             step_list.append(io)
             gpl = OpenROAD.GlobalPlacement(
                 fp_config,
                 state_in=io.state_out,
                 id="gpl-highutil",
                 long_name="Global Placement (High Util)",
                 flow=self,
             )
-            gpl.start()
+            self.start_step(gpl)
             step_list.append(gpl)
-        except subprocess.CalledProcessError:
+        except StepError:
             info("High utilization failed- attempting low utilization…")
-            fp_config = min_config.copy()
-            fp_config["FP_CORE_UTIL"] = 40
+            fp_config = min_config.copy(FP_CORE_UTIL=40)
             fp = OpenROAD.Floorplan(
                 fp_config,
                 state_in=min_area_state,
                 id="fp-lowutl",
                 long_name="Floorplanning (Low Util)",
                 flow=self,
             )
-            fp.start()
+            self.start_step(fp)
             step_list.append(fp)
             io = OpenROAD.IOPlacement(
                 fp_config,
                 state_in=fp.state_out,
                 id="io-lowutl",
                 long_name="I/O Placement (Low Util)",
                 flow=self,
             )
-            io.start()
+            self.start_step(io)
             step_list.append(io)
             gpl = OpenROAD.GlobalPlacement(
                 fp_config,
                 state_in=io.state_out,
                 id="gpl-lowutl",
                 long_name="Global Placement (Low Util)",
                 flow=self,
             )
-            gpl.start()
+            self.start_step(gpl)
             step_list.append(gpl)
 
         self.end_stage()
 
         success("Flow complete.")
+        assert gpl.state_out is not None  # We should be done with the execution by now
         return (gpl.state_out, step_list)
```

### Comparing `openlane-2.0.0a9/openlane/scripts/base.sdc` & `openlane-2.0.0b1/openlane/scripts/base.sdc`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,70 @@
-if {[info exists ::env(CLOCK_PORT)] && $::env(CLOCK_PORT) != ""} {
-    create_clock [get_ports $::env(CLOCK_PORT)]  -name $::env(CLOCK_PORT)  -period $::env(CLOCK_PERIOD)
-} else {
-    create_clock -name __VIRTUAL_CLK__ -period $::env(CLOCK_PERIOD)
-    set ::env(CLOCK_PORT) __VIRTUAL_CLK__
+set clock_port __VIRTUAL_CLK__
+if { [info exists ::env(CLOCK_PORT)] } {
+    set port_count [llength $::env(CLOCK_PORT)]
+
+    if { $port_count == "0" } {
+        puts "\[WARN] No CLOCK_PORT found. A dummy clock will be used."
+    } elseif { $port_count != "1" } {
+        puts "\[WARN] Multi-clock files are not currently supported by the base SDC file. Only the first clock will be constrained."
+    }
+
+    if { $port_count > "0" } {
+        set ::clock_port [lindex $::env(CLOCK_PORT) 0]
+    }
 }
-set input_delay_value [expr $::env(CLOCK_PERIOD) * $::env(IO_PCT)]
-set output_delay_value [expr $::env(CLOCK_PERIOD) * $::env(IO_PCT)]
-puts "\[INFO\] Setting output delay to: $output_delay_value"
-puts "\[INFO\] Setting input delay to: $input_delay_value"
+set port_args [get_ports $clock_port]
+puts "\[INFO] Using clock $clock_port…"
+create_clock {*}$port_args -name $clock_port -period $::env(CLOCK_PERIOD)
+
+set input_delay_value [expr $::env(CLOCK_PERIOD) * $::env(IO_DELAY_CONSTRAINT) / 100]
+set output_delay_value [expr $::env(CLOCK_PERIOD) * $::env(IO_DELAY_CONSTRAINT) / 100]
+puts "\[INFO] Setting output delay to: $output_delay_value"
+puts "\[INFO] Setting input delay to: $input_delay_value"
 
 set_max_fanout $::env(MAX_FANOUT_CONSTRAINT) [current_design]
+if { [info exists ::env(MAX_TRANSITION_CONSTRAINT)] } {
+    set_max_transition $::env(MAX_TRANSITION_CONSTRAINT) [current_design]
+}
 
-set clk_input [get_port $::env(CLOCK_PORT)]
+set clk_input [get_port $clock_port]
 set clk_indx [lsearch [all_inputs] $clk_input]
 set all_inputs_wo_clk [lreplace [all_inputs] $clk_indx $clk_indx ""]
 
 #set rst_input [get_port resetn]
 #set rst_indx [lsearch [all_inputs] $rst_input]
 #set all_inputs_wo_clk_rst [lreplace $all_inputs_wo_clk $rst_indx $rst_indx ""]
 set all_inputs_wo_clk_rst $all_inputs_wo_clk
 
 # correct resetn
-set_input_delay $input_delay_value  -clock [get_clocks $::env(CLOCK_PORT)] $all_inputs_wo_clk_rst
-#set_input_delay 0.0 -clock [get_clocks $::env(CLOCK_PORT)] {resetn}
-set_output_delay $output_delay_value  -clock [get_clocks $::env(CLOCK_PORT)] [all_outputs]
+set clocks [get_clocks $clock_port]
+
+set_input_delay $input_delay_value -clock $clocks $all_inputs_wo_clk_rst
+set_output_delay $output_delay_value -clock $clocks [all_outputs]
 
 if { ![info exists ::env(SYNTH_CLK_DRIVING_CELL)] } {
     set ::env(SYNTH_CLK_DRIVING_CELL) $::env(SYNTH_DRIVING_CELL)
 }
 
-if { ![info exists ::env(SYNTH_CLK_DRIVING_CELL_PIN)] } {
-    set ::env(SYNTH_CLK_DRIVING_CELL_PIN) $::env(SYNTH_DRIVING_CELL_PIN)
-}
-
-set_driving_cell -lib_cell $::env(SYNTH_DRIVING_CELL) -pin $::env(SYNTH_DRIVING_CELL_PIN) $all_inputs_wo_clk_rst
-
-set_driving_cell -lib_cell $::env(SYNTH_CLK_DRIVING_CELL) -pin $::env(SYNTH_CLK_DRIVING_CELL_PIN) $clk_input
-
-set cap_load [expr $::env(SYNTH_CAP_LOAD) / 1000.0]
-puts "\[INFO\] Setting load to: $cap_load"
-set_load  $cap_load [all_outputs]
-
-puts "\[INFO\] Setting clock uncertainty to: $::env(CLOCK_UNCERTAINTY_CONSTRAINT)"
-set_clock_uncertainty $::env(CLOCK_UNCERTAINTY_CONSTRAINT) [get_clocks $::env(CLOCK_PORT)]
-
-puts "\[INFO\] Setting clock transition to: $::env(CLOCK_TRANSITION_CONSTRAINT)"
-set_clock_transition $::env(CLOCK_TRANSITION_CONSTRAINT) [get_clocks $::env(CLOCK_PORT)]
-
-puts "\[INFO\] Setting timing derate to: [expr {$::env(TIME_DERATING_CONSTRAINT) * 10}] %"
-set_timing_derate -early [expr {1-$::env(TIME_DERATING_CONSTRAINT)}]
-set_timing_derate -late [expr {1+$::env(TIME_DERATING_CONSTRAINT)}]
+set_driving_cell \
+    -lib_cell [lindex [split $::env(SYNTH_DRIVING_CELL) "/"] 0] \
+    -pin [lindex [split $::env(SYNTH_DRIVING_CELL) "/"] 1] \
+    $all_inputs_wo_clk_rst
+
+set_driving_cell \
+    -lib_cell [lindex [split $::env(SYNTH_CLK_DRIVING_CELL) "/"] 0] \
+    -pin [lindex [split $::env(SYNTH_CLK_DRIVING_CELL) "/"] 1] \
+    $clk_input
+
+set cap_load [expr $::env(OUTPUT_CAP_LOAD) / 1000.0]
+puts "\[INFO] Setting load to: $cap_load"
+set_load $cap_load [all_outputs]
+
+puts "\[INFO] Setting clock uncertainty to: $::env(CLOCK_UNCERTAINTY_CONSTRAINT)"
+set_clock_uncertainty $::env(CLOCK_UNCERTAINTY_CONSTRAINT) $clocks
+
+puts "\[INFO] Setting clock transition to: $::env(CLOCK_TRANSITION_CONSTRAINT)"
+set_clock_transition $::env(CLOCK_TRANSITION_CONSTRAINT) $clocks
+
+puts "\[INFO] Setting timing derate to: $::env(TIME_DERATING_CONSTRAINT)%"
+set_timing_derate -early [expr 1-[expr $::env(TIME_DERATING_CONSTRAINT) / 100]]
+set_timing_derate -late [expr 1+[expr $::env(TIME_DERATING_CONSTRAINT) / 100]]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0a9/openlane/scripts/klayout/open_design.py` & `openlane-2.0.0b1/openlane/scripts/klayout/open_design.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,19 @@
             "-rm",
             __file__,
         ]
         for key, value in kwargs.items():
             args.append("-rd")
             if isinstance(value, tuple) or isinstance(value, list):
                 value = ";".join(value)
-            elif isinstance(value, str) and os.path.exists(value):
+            elif (
+                isinstance(value, str)
+                and os.path.exists(value)
+                and key != "design_name"
+            ):
                 value = os.path.abspath(value)
 
             args.append(f"{key}={value or 'NULL'}")
 
         os.execlp("klayout", *args)
 
     if __name__ == "__main__":
@@ -88,11 +92,12 @@
     layout_options.keep_other_cells = True
     layout_options.lefdef_config.macro_resolution_mode = 1
     layout_options.lefdef_config.read_lef_with_def = False
     layout_options.lefdef_config.lef_files = input_lefs.split(";")
     layout_options.lefdef_config.map_file = lym
 
     cell_view = main_window.load_layout(input, layout_options, 0)
-    pya.Application.instance().exit(0)
+    layout_view = cell_view.view()
+    layout_view.load_layer_props(lyp)
 except Exception as e:
     print(e, file=sys.stderr)
     pya.Application.instance().exit(1)
```

### Comparing `openlane-2.0.0a9/openlane/scripts/klayout/render.py` & `openlane-2.0.0b1/openlane/scripts/klayout/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,19 @@
             "-rm",
             __file__,
         ]
         for key, value in kwargs.items():
             args.append("-rd")
             if isinstance(value, tuple) or isinstance(value, list):
                 value = ";".join(value)
-            elif isinstance(value, str) and os.path.exists(value):
+            elif (
+                isinstance(value, str)
+                and os.path.exists(value)
+                and key != "design_name"
+            ):
                 value = os.path.abspath(value)
 
             args.append(f"{key}={value or 'NULL'}")
 
         os.execlp("klayout", *args)
 
     if __name__ == "__main__":
```

### Comparing `openlane-2.0.0a9/openlane/scripts/klayout/stream_out.py` & `openlane-2.0.0b1/openlane/scripts/klayout/stream_out.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,19 @@
             "-rm",
             __file__,
         ]
         for key, value in kwargs.items():
             args.append("-rd")
             if isinstance(value, tuple) or isinstance(value, list):
                 value = ";".join(value)
-            elif isinstance(value, str) and os.path.exists(value):
+            elif (
+                isinstance(value, str)
+                and os.path.exists(value)
+                and key != "design_name"
+            ):
                 value = os.path.abspath(value)
 
             args.append(f"{key}={value or 'NULL'}")
 
         os.execlp("klayout", *args)
 
     if __name__ == "__main__":
@@ -130,15 +134,14 @@
 
 
 try:
     # Load technology file
     tech = pya.Technology()
     tech.load(lyt)
     layout_options = tech.load_layout_options
-    layout_options.lefdef_config.macro_resolution_mode = 1
     layout_options.lefdef_config.read_lef_with_def = False
     layout_options.lefdef_config.lef_files = input_lefs.split(";")
     layout_options.lefdef_config.map_file = lym
 
     # Load def file
     main_layout = pya.Layout()
     # main_layout.load_layer_props(props_file)
```

### Comparing `openlane-2.0.0a9/openlane/scripts/klayout/xor.drc` & `openlane-2.0.0b1/openlane/scripts/klayout/xor.drc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/def/antenna_check.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/def/antenna_check.tcl`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 select top cell
 extract do local
 extract no capacitance
 extract no coupling
 extract no resistance
 extract no adjust
-if { ! $::env(LVS_CONNECT_BY_LABEL) } {
+if { ! $::env(MAGIC_NO_EXT_UNIQUE) } {
     extract unique
 }
 extract
 feedback save $::env(_tmp_feedback_file)
 
 antennacheck debug
-antennacheck
+antennacheck
```

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/def/mag.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/check_antennas.tcl`

 * *Files 14% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+read_current_odb
 
-source $::env(SCRIPTS_DIR)/magic/def/read.tcl
-
-save $::env(SAVE_MAG)
-
-puts "[INFO]: Done exporting $::env(SAVE_MAG)."
+# start checking antennas and generate a detailed report
+puts "%OL_CREATE_REPORT antenna.rpt"
+check_antennas -verbose
+puts "%OL_END_REPORT"
```

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/def/mag_gds.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/def/mag_gds.tcl`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,14 @@
 drc off
 
 source $::env(SCRIPTS_DIR)/magic/def/read.tcl
 
 load $::env(DESIGN_NAME)
 select top cell
 
-# padding
-if { $::env(MAGIC_PAD) } {
-	puts "\[INFO\] Padding LEFs"
-	# assuming scalegrid 1 2
-	# use um
-	select top cell
-	box grow right [expr 100*($::env(PLACE_SITE_WIDTH))]
-	box grow left [expr 100*($::env(PLACE_SITE_WIDTH))]
-	box grow up [expr 100*($::env(PLACE_SITE_HEIGHT))]
-	box grow down [expr 100*($::env(PLACE_SITE_HEIGHT))]
-	property FIXED_BBOX [box values]
-}
-
 if { $::env(MAGIC_ZEROIZE_ORIGIN) } {
 	# assuming scalegrid 1 2
 	# makes origin zero based on the minimum enclosing box
 	# all shapes will be within the block boundary
 	# lower left corner will become (0, 0)
 	puts "\[INFO\] Zeroizing Origin"
 	set bbox [box values]
@@ -54,37 +41,54 @@
 
 select top cell
 
 cellname filepath $::env(DESIGN_NAME) $::env(STEP_DIR)
 
 save
 
-# Write GDS
+
 # mark the incoming cell defs as readonly so that their
 # GDS data gets copied verbatim
 gds readonly true
 gds rescale false
 
 if { $::env(MAGIC_GDS_POLYGON_SUBCELLS) } {
 	gds polygon subcells true
 }
-
+# # Can be obtained from the PDK's .mag files.
+# set gds_files_in $::env(CELL_GDS)
+# foreach gds_file $gds_files_in {
+# 	puts "> gds read $gds_file"
+# 	gds read $gds_file
+# }
+if {  [info exist ::env(MACRO_GDS_FILES)] } {
+	set gds_files_in $::env(MACRO_GDS_FILES)
+	foreach gds_file $gds_files_in {
+		puts "> gds read $gds_file"
+		gds read $gds_file
+	}
+}
 if {  [info exist ::env(EXTRA_GDS_FILES)] } {
 	set gds_files_in $::env(EXTRA_GDS_FILES)
 	foreach gds_file $gds_files_in {
+		puts "> gds read $gds_file"
 		gds read $gds_file
 	}
 }
 
 load $::env(DESIGN_NAME)
 
+# if { $::env(MAGIC_GDS_FLATTEN) } {
+# 	puts "Flattening cell"
+# 	flatten top cell
+# }
+
 select top cell
 
-if {  [info exist ::env(MAGIC_DISABLE_HIER_GDS)]\
-	&& $::env(MAGIC_DISABLE_HIER_GDS) } {
+if {  $::env(MAGIC_DISABLE_CIF_INFO) } {
 	cif *hier write disable
 	cif *array write disable
 }
 
 gds nodatestamp yes
 
 if { $::env(MAGIC_GDS_ALLOW_ABSTRACT) } {
```

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/def/read.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/drt.tcl`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-# Copyright 2022 Efabless Corporation
+# Copyright 2020-2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
+read_current_odb
 
-# LEF
-lef read $::env(TECH_LEF)
-if { [info exist ::env(EXTRA_LEFS)] } {
-    foreach lef_file $::env(EXTRA_LEFS) {
-        lef read $lef_file
-    }
-}
+set_thread_count $::env(DRT_THREADS)
 
-# DEF
-set def_read_args [list]
-lappend def_read_args $::env(CURRENT_DEF)
-if { $::env(MAGIC_DEF_NO_BLOCKAGES) } {
-    lappend def_read_args -noblockage
+set min_layer $::env(RT_MIN_LAYER)
+if { [info exists ::env(DRT_MIN_LAYER)] } {
+    set min_layer $::env(DRT_MIN_LAYER)
 }
-if { $::env(MAGIC_DEF_LABELS) } {
-    lappend def_read_args -labels
+
+set max_layer $::env(RT_MAX_LAYER)
+if { [info exists ::env(DRT_MAX_LAYER)] } {
+    set max_layer $::env(DRT_MAX_LAYER)
 }
 
-def read {*}$def_read_args
+detailed_route\
+    -bottom_routing_layer $min_layer\
+    -top_routing_layer $max_layer\
+    -output_drc $::env(STEP_DIR)/$::env(DESIGN_NAME).drc\
+    -droute_end_iter $::env(DRT_OPT_ITERS)\
+    -or_seed 42\
+    -verbose 1
+
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/drc.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/drc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/extract_spice.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/extract_spice.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 cd $extdir
 
 extract do local
 extract no capacitance
 extract no coupling
 extract no resistance
 extract no adjust
-if { ! $::env(LVS_CONNECT_BY_LABEL) } {
+if { ! $::env(MAGIC_NO_EXT_UNIQUE) } {
     extract unique
 }
 # extract warn all
 extract
 
 ext2spice lvs
 ext2spice -o $netlist $::env(DESIGN_NAME).ext
 feedback save $feedback_file
-# exec cp $::env(DESIGN_NAME).spice $::env(signoff_results)/$::env(DESIGN_NAME).spice
+# exec cp $::env(DESIGN_NAME).spice $::env(signoff_results)/$::env(DESIGN_NAME).spice
```

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/gds/drc_batch.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/gds/drc_batch.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/gds/erase_box.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/gds/erase_box.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/gds/mag_with_pointers.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/gds/mag_with_pointers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/gds/read.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/gds/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/lef/extras_maglef.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/lef/extras_maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/magic/lef/maglef.tcl` & `openlane-2.0.0b1/openlane/scripts/magic/lef/maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/apply_def_template.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/apply_def_template.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/contextualize.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/contextualize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/defutil.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/defutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/diodes.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/diodes.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/io_place.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/io_place.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import odb
 
+import os
 import re
+import sys
 import math
+import click
 import random
 
-from reader import click_odb, click
+from reader import click_odb
 
 
 def grid_to_tracks(origin, count, step):
     tracks = []
     pos = origin
     for _ in range(count):
         tracks.append(pos)
@@ -46,17 +49,17 @@
             )  # Decrement actual pin count, this value was only there to indicate virtual pin count
             total_pin_count = actual_pin_count + virtual_pin_count
     result = []
     tracks = len(possible_locations)
 
     if total_pin_count > tracks:
         print(
-            f"There are more pins/virtual_pins: {total_pin_count}, than places to put them: {tracks}. Try making your floorplan area larger."
+            f"There are more pins/virtual_pins: {total_pin_count}, than places to put them: {tracks} in the {side} side. Try making your floorplan area larger."
         )
-        exit(1)
+        sys.exit(1)
     elif total_pin_count == tracks:
         return possible_locations, side_pin_placement  # All positions.
     elif total_pin_count == 0:
         return result, side_pin_placement
 
     # From this point, pin_count always < tracks.
     tracks_per_pin = math.floor(tracks / total_pin_count)  # >=1
@@ -140,16 +143,17 @@
         return -1
     else:
         return int(m.group(1))
 
 
 @click.command()
 @click.option(
-    "-u/-U",
-    "--unmatched-error/--ignore-unmatched",
+    "-u",
+    "--unmatched-error",
+    is_flag=True,
     default=False,
     help="Treat unmatched pins as error",
 )
 @click.option("-c", "--config", required=False, help="Optional configuration file.")
 @click.option(
     "-r",
     "--reverse",
@@ -256,15 +260,15 @@
             for line in config_file:
                 line = line.split()
                 if len(line) == 0:
                     continue
 
                 if len(line) > 1:
                     print("Only one entry allowed per line.")
-                    exit(1)
+                    sys.exit(1)
 
                 token = line[0]
 
                 if cur_side is not None and token[0] != "#":
                     pin_placement_cfg[cur_side].append(token)
                 elif token not in [
                     "#N",
@@ -278,15 +282,15 @@
                     "#BUS_SORT",
                 ]:
                     print(
                         "Valid directives are #N, #E, #S, or #W. Append R for reversing the default order.",
                         "Use #BUS_SORT to group 'bus bits' by index.",
                         "Please make sure you have set a valid side first before listing pins",
                     )
-                    exit(1)
+                    sys.exit(1)
                 elif token == "#BUS_SORT":
                     bus_sort_flag = True
                 else:
                     if len(token) == 3:
                         token = token[0:2]
                         reverse_arr.append(token)
                     cur_side = token
@@ -309,48 +313,64 @@
     # sort them "humanly"
     bterms_enum.sort(key=natural_keys)
     if bus_sort_flag:
         bterms_enum.sort(key=bus_keys)
     bterms = [bterm[1] for bterm in bterms_enum]
 
     pin_placement = {"#N": [], "#E": [], "#S": [], "#W": []}
+    pin_distance_min = {
+        "#N": V_WIDTH + V_LAYER.getSpacing(),
+        "#S": V_WIDTH + V_LAYER.getSpacing(),
+        "#E": H_WIDTH + H_LAYER.getSpacing(),
+        "#W": H_WIDTH + H_LAYER.getSpacing(),
+    }
+    pin_distance = pin_distance_min.copy()
     bterm_regex_map = {}
     for side in pin_placement_cfg:
         for regex in pin_placement_cfg[side]:  # going through them in order
             if regex[0] == "$":  # Sign of Virtual Pins
                 try:
                     virtual_pins_count = int(regex[1:])
                     pin_placement[side].append(virtual_pins_count)
                 except ValueError:
                     print("You provided invalid values for virtual pins")
-                    exit(1)
+                    sys.exit(1)
+            elif regex[0] == "@":
+                variable = regex[1:].split("=")
+                if variable[0] == "min_distance":
+                    pin_distance[side] = float(variable[1]) * reader.dbunits
+                    if pin_distance[side] < pin_distance_min[side]:
+                        print(
+                            f"Warning: Using min_distance {pin_distance_min[side] / reader.dbunits} for {side} pins to avoid overlap"
+                        )
+                        pin_distance[side] = pin_distance_min[side]
             else:
                 regex += "$"  # anchor
                 for bterm in bterms:
                     # if a pin name matches multiple regexes, their order will be
                     # arbitrary. More refinement requires more strict regexes (or just
                     # the exact pin name).
                     pin_name = bterm.getName()
                     if re.match(regex, pin_name) is not None:
                         if bterm in bterm_regex_map:
                             print(
                                 f"Error: Multiple regexes matched {pin_name}. Those are {bterm_regex_map[bterm]} and {regex}"
                             )
-                            exit(1)
+                            sys.exit(os.EX_DATAERR)
                         bterm_regex_map[bterm] = regex
                         pin_placement[side].append(bterm)  # to maintain the order
 
     unmatched_bterms = [bterm for bterm in bterms if bterm not in bterm_regex_map]
 
     if len(unmatched_bterms) > 0:
         print("Warning: Some pins weren't matched by the config file")
         print("Those are:", [bterm.getName() for bterm in unmatched_bterms])
         if unmatched_error_flag:
             print("Treating unmatched pins as errors. Exiting..")
-            exit(1)
+            sys.exit(1)
         else:
             print("Assigning random sides to the above pins")
             for bterm in unmatched_bterms:
                 random_side = random.choice(list(pin_placement.keys()))
                 pin_placement[random_side].append(bterm)
 
     # generate slots
@@ -359,50 +379,58 @@
     BLOCK_LL_X = DIE_AREA.xMin()
     BLOCK_LL_Y = DIE_AREA.yMin()
     BLOCK_UR_X = DIE_AREA.xMax()
     BLOCK_UR_Y = DIE_AREA.yMax()
 
     print("Block boundaries:", BLOCK_LL_X, BLOCK_LL_Y, BLOCK_UR_X, BLOCK_UR_Y)
 
-    origin, count, step = reader.block.findTrackGrid(H_LAYER).getGridPatternY(0)
-    print(f"Horizontal Tracks Origin: {origin}, Count: {count}, Step: {step}")
-    h_tracks = grid_to_tracks(origin, count, step)
-
-    origin, count, step = reader.block.findTrackGrid(V_LAYER).getGridPatternX(0)
-    print(f"Vertical Tracks Origin: {origin}, Count: {count}, Step: {step}")
-    v_tracks = grid_to_tracks(origin, count, step)
+    origin, count, h_step = reader.block.findTrackGrid(H_LAYER).getGridPatternY(0)
+    print(f"Horizontal Tracks Origin: {origin}, Count: {count}, Step: {h_step}")
+    h_tracks = grid_to_tracks(origin, count, h_step)
+
+    origin, count, v_step = reader.block.findTrackGrid(V_LAYER).getGridPatternX(0)
+    print(f"Vertical Tracks Origin: {origin}, Count: {count}, Step: {v_step}")
+    v_tracks = grid_to_tracks(origin, count, v_step)
 
     for rev in reverse_arr:
         pin_placement[rev].reverse()
 
-    # create the pins
+    pin_tracks = {}
     for side in pin_placement:
         if side in ["#N", "#S"]:
-            slots, pin_placement[side] = equally_spaced_sequence(
-                side, pin_placement[side], v_tracks
-            )
-        else:
-            slots, pin_placement[side] = equally_spaced_sequence(
-                side, pin_placement[side], h_tracks
-            )
+            pin_tracks[side] = [
+                v_tracks[i]
+                for i in range(len(v_tracks))
+                if (i % (math.ceil(pin_distance[side] / v_step))) == 0
+            ]
+        elif side in ["#W", "#E"]:
+            pin_tracks[side] = [
+                h_tracks[i]
+                for i in range(len(h_tracks))
+                if (i % (math.ceil(pin_distance[side] / h_step))) == 0
+            ]
+
+    # create the pins
+    for side in pin_placement:
+        slots, pin_placement[side] = equally_spaced_sequence(
+            side, pin_placement[side], pin_tracks[side]
+        )
 
         assert len(slots) == len(pin_placement[side])
 
         for i in range(len(pin_placement[side])):
             bterm = pin_placement[side][i]
             slot = slots[i]
             # print(f"Pin name: {bterm.getName()}, placed at slot: {slot}")
 
             pin_name = bterm.getName()
             pins = bterm.getBPins()
             if len(pins) > 0:
-                # print(f"Warning: {pin_name} already has shapes. Modifying them")
-                assert (
-                    len(pins) == 1
-                ), f"{pin_name} has multiple pins already placed. This is a fatal error."
+                print(f"Warning: {pin_name} already has shapes. Modifying them")
+                assert len(pins) == 1
                 pin_bpin = pins[0]
             else:
                 pin_bpin = odb.dbBPin_create(bterm)
 
             pin_bpin.setPlacementStatus("PLACED")
 
             if side in ["#N", "#S"]:
```

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/label_macro_pins.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/label_macro_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/lefutil.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/lefutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/manual_macro_place.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/manual_macro_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/padringer.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/padringer.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/power_utils.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/power_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,24 +388,28 @@
         custom_vias[lower_layer.getName()][upper_layer.getName()] = {
             "rule": rule,
             "params": via_params,
         }
         print("Added", rule.getName())
 
     def create_custom_via(layer1, layer2, width, height, reorient="R0"):
-        assert width > 0 and height > 0
+        if not width > 0:
+            raise ValueError(f"width must be greater than 0: {width} provided")
+
+        if not height > 0:
+            raise ValueError(f"height must be greater than 0: {height} provided")
 
         if layer1.getRoutingLevel() < layer2.getRoutingLevel():
             lower_layer_name = layer1.getName()
             upper_layer_name = layer2.getName()
         elif layer1.getRoutingLevel() > layer2.getRoutingLevel():
             lower_layer_name = layer2.getName()
             upper_layer_name = layer1.getName()
         else:
-            raise Exception("Cannot create a custom via between two identical layers")
+            raise ValueError("Cannot create a custom via between two identical layers")
 
         if reorient in ["R90", "R270"]:
             width, height = height, width
 
         via_name = "via_%s_%s_%dx%d" % (
             lower_layer_name,
             upper_layer_name,
```

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/random_place.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/random_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/reader.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,22 @@
 if python_path := os.environ.get("ODB_PYTHONPATH", None):
     sys.path = python_path.split(":") + sys.path
 
 sys.path.insert(0, os.path.dirname(os.environ["OPENLANE_ROOT"]))
 # -- END
 
 import click
-from openlane.state.design_format import DesignFormat, DesignFormatByID
-
-click  # Re-export now that the environment actually works properly
+import rich
+from rich.table import Table
+from openlane.state.design_format import DesignFormat, DesignFormatObject
+
+# Re-export now that the environment actually works properly
+rich
+click
+Table
 
 write_fn: Dict[DesignFormat, Callable] = {
     DesignFormat.DEF: lambda reader, file: odb.write_def(reader.block, file),
     DesignFormat.ODB: lambda reader, file: odb.write_db(reader.db, file),
 }
 
 
@@ -84,15 +89,15 @@
         kwargs = kwargs.copy()
         kwargs["reader"] = reader
 
         outputs = []
         for key, value in kwargs.items():
             if key.startswith("output_"):
                 id = key[7:]
-                outputs.append((DesignFormatByID[id], value))
+                outputs.append((DesignFormat.by_id(id), value))
 
         kwargs = {k: kwargs[k] for k in kwargs.keys() if not k.startswith("output_")}
 
         if "input_db" in parameter_keys:
             kwargs["input_db"] = input_db
         if "input_lefs" in parameter_keys:
             kwargs["input_lefs"] = input_lefs
@@ -108,19 +113,20 @@
         for format, path in outputs:
             fn = write_fn[format]
             fn(reader, path)
 
     for format in DesignFormat:
         if write_fn.get(format) is None:
             continue
-        id, _, name = format.value
+        # For type-checker: all guaranteed to be DesignFormatObjects
+        assert isinstance(format.value, DesignFormatObject)
         wrapper = click.option(
-            f"--output-{id}",
+            f"--output-{format.value.id}",
             default=None,
-            help=f"Write {name}",
+            help=f"Write {format.value.name}",
         )(wrapper)
 
     wrapper = click.option(
         "-l",
         "--input-lef",
         "input_lefs",
         default=(),
```

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/remove_buffers.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/remove_buffers.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/snap_to_grid.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/snap_to_grid.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/odbpy/wire_lengths.py` & `openlane-2.0.0b1/openlane/scripts/odbpy/wire_lengths.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import utl
 
 from reader import click, click_odb, OdbReader
 
 
 def to_si(microns: Decimal) -> str:
-    units = ["μm", "mm", "m"]
+    units = ["µm", "mm", "m"]
     unit = 0
     value = microns
     while value >= 1000 and unit < len(units):
         value /= 1000
         unit += 1
     return f"{value}{units[unit]}"
 
@@ -82,15 +82,15 @@
             length_printable: str = str(length_microns)
             if human_readable:
                 length_printable = str(to_si(length_microns))
             print(f"{net.getName()},{length_printable}", file=f)
 
     for net, length_microns in above_threshold:
         print(
-            f"Net {net.getName()} is above the length threshold ({length_microns}/{threshold} μm)."
+            f"Net {net.getName()} is above the length threshold ({length_microns}/{threshold} µm)."
         )
 
-    utl.metric_float("route__max__wirelength", float(max_wire_length))
+    utl.metric_float("route__wirelength__max", float(max_wire_length))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/basic_mp.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/tapcell.tcl`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+read_current_odb
 
-macro_placement\
-    -channel $::env(PL_MACRO_CHANNEL)\
-    -halo $::env(PL_MACRO_HALO)
+tapcell\
+    -distance $::env(FP_TAPCELL_DIST)\
+    -tapcell_master "$::env(FP_WELLTAP_CELL)"\
+    -endcap_master "$::env(FP_ENDCAP_CELL)"\
+    -halo_width_x $::env(FP_TAP_HORIZONTAL_HALO)\
+    -halo_width_y $::env(FP_TAP_VERTICAL_HALO)
 
-write
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/check_antennae.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/gui.tcl`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-# Copyright 2020-2022 Efabless Corporation
+# Copyright 2022 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
-
-# start checking antennas and generate a detailed report
-puts "%OL_CREATE_REPORT antenna.rpt"
-check_antennas -verbose
-puts "%OL_END_REPORT"
+read_current_odb
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/dpl.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/dpl_cell_pad.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/dpl_cell_pad.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/grt.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/pdn_cfg.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/pdn_cfg.tcl`

 * *Files 7% similar despite different names*

```diff
@@ -47,82 +47,82 @@
 # value of $::env(DESIGN_IS_CORE) and uses the appropriate stdcell section
 if { $::env(DESIGN_IS_CORE) == 1 } {
     # Used if the design is the core of the chip
     define_pdn_grid \
         -name stdcell_grid \
         -starts_with POWER \
         -voltage_domain CORE \
-        -pins "$::env(FP_PDN_LOWER_LAYER) $::env(FP_PDN_UPPER_LAYER)"
+        -pins "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)"
 
     add_pdn_stripe \
         -grid stdcell_grid \
-        -layer $::env(FP_PDN_LOWER_LAYER) \
+        -layer $::env(FP_PDN_VERTICAL_LAYER) \
         -width $::env(FP_PDN_VWIDTH) \
         -pitch $::env(FP_PDN_VPITCH) \
         -offset $::env(FP_PDN_VOFFSET) \
         -spacing $::env(FP_PDN_VSPACING) \
         -starts_with POWER -extend_to_core_ring
 
     add_pdn_stripe \
         -grid stdcell_grid \
-        -layer $::env(FP_PDN_UPPER_LAYER) \
+        -layer $::env(FP_PDN_HORIZONTAL_LAYER) \
         -width $::env(FP_PDN_HWIDTH) \
         -pitch $::env(FP_PDN_HPITCH) \
         -offset $::env(FP_PDN_HOFFSET) \
         -spacing $::env(FP_PDN_HSPACING) \
         -starts_with POWER -extend_to_core_ring
 
     add_pdn_connect \
         -grid stdcell_grid \
-        -layers "$::env(FP_PDN_LOWER_LAYER) $::env(FP_PDN_UPPER_LAYER)"
+        -layers "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)"
 } else {
     # Used if the design is a macro in the core
     define_pdn_grid \
         -name stdcell_grid \
         -starts_with POWER \
         -voltage_domain CORE \
-        -pins $::env(FP_PDN_LOWER_LAYER)
+        -pins $::env(FP_PDN_VERTICAL_LAYER)
 
     add_pdn_stripe \
         -grid stdcell_grid \
-        -layer $::env(FP_PDN_LOWER_LAYER) \
+        -layer $::env(FP_PDN_VERTICAL_LAYER) \
         -width $::env(FP_PDN_VWIDTH) \
         -pitch $::env(FP_PDN_VPITCH) \
         -offset $::env(FP_PDN_VOFFSET) \
         -starts_with POWER
 }
 
 # Adds the standard cell rails if enabled.
 if { $::env(FP_PDN_ENABLE_RAILS) == 1 } {
     add_pdn_stripe \
         -grid stdcell_grid \
-        -layer $::env(FP_PDN_RAILS_LAYER) \
+        -layer $::env(FP_PDN_RAIL_LAYER) \
         -width $::env(FP_PDN_RAIL_WIDTH) \
         -followpins \
         -starts_with POWER
 
     add_pdn_connect \
         -grid stdcell_grid \
-        -layers "$::env(FP_PDN_RAILS_LAYER) $::env(FP_PDN_LOWER_LAYER)"
+        -layers "$::env(FP_PDN_RAIL_LAYER) $::env(FP_PDN_VERTICAL_LAYER)"
 }
 
 
 # Adds the core ring if enabled.
 if { $::env(FP_PDN_CORE_RING) == 1 } {
     add_pdn_ring \
         -grid stdcell_grid \
-        -layers "$::env(FP_PDN_LOWER_LAYER) $::env(FP_PDN_UPPER_LAYER)" \
+        -layers "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)" \
         -widths "$::env(FP_PDN_CORE_RING_VWIDTH) $::env(FP_PDN_CORE_RING_HWIDTH)" \
         -spacings "$::env(FP_PDN_CORE_RING_VSPACING) $::env(FP_PDN_CORE_RING_HSPACING)" \
         -core_offset "$::env(FP_PDN_CORE_RING_VOFFSET) $::env(FP_PDN_CORE_RING_HOFFSET)"
 }
 
 define_pdn_grid \
     -macro \
     -default \
     -name macro \
     -starts_with POWER \
     -halo "$::env(FP_PDN_HORIZONTAL_HALO) $::env(FP_PDN_VERTICAL_HALO)"
 
 add_pdn_connect \
     -grid macro \
-    -layers "$::env(FP_PDN_LOWER_LAYER) $::env(FP_PDN_UPPER_LAYER)"
+    -layers "$::env(FP_PDN_VERTICAL_LAYER) $::env(FP_PDN_HORIZONTAL_LAYER)"
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/set_global_connections.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/set_global_connections.tcl`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Power nets
 proc set_global_connections {} {
+    puts "\[INFO] Setting global connections..."
     if { [info exists ::env(PDN_ENABLE_GLOBAL_CONNECTIONS) ] } {
         if { $::env(PDN_ENABLE_GLOBAL_CONNECTIONS) == 1 } {
             foreach power_pin $::env(SCL_POWER_PINS) {
                 add_global_connection \
                     -net $::env(VDD_NET) \
                     -inst_pattern .* \
                     -pin_pattern $power_pin \
@@ -30,22 +31,15 @@
                     -pin_pattern $ground_pin \
                     -ground
             }
         }
     }
     if { $::env(PDN_CONNECT_MACROS_TO_GRID) == 1 &&
         [info exists ::env(PDN_MACRO_CONNECTIONS)]} {
-        set pdn_hooks \
-            [lmap \
-                {a b c d e} \
-                $::env(PDN_MACRO_CONNECTIONS) \
-                {list $a $b $c $d $e} \
-            ]
-
-        foreach pdn_hook $pdn_hooks {
+        foreach pdn_hook $::env(PDN_MACRO_CONNECTIONS) {
             set instance_name [lindex $pdn_hook 0]
             set power_net [lindex $pdn_hook 1]
             set ground_net [lindex $pdn_hook 2]
             set power_pin [lindex $pdn_hook 3]
             set ground_pin [lindex $pdn_hook 4]
 
             if { $power_pin == "" || $ground_pin == "" } {
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/set_layer_adjustments.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/set_layer_adjustments.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/set_power_nets.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/set_power_nets.tcl`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 if { [info exists ::env(VDD_NETS)] || [info exists ::env(GND_NETS)] } {
     # they both must exist and be equal in length
     # current assumption: they cannot have a common ground
     if { ! [info exists ::env(VDD_NETS)] || ! [info exists ::env(GND_NETS)] } {
-        puts_err "VDD_NETS and GND_NETS must *both* either be defined or undefined"
+        puts "\[ERROR] VDD_NETS and GND_NETS must *both* either be defined or undefined"
         exit -1
     }
     set ::env(VDD_NET) [lindex $::env(VDD_NETS) 0]
     set ::env(GND_NET) [lindex $::env(GND_NETS) 0]
 
 } else {
     set ::env(VDD_NET) $::env(VDD_PIN)
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/set_rc.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/set_rc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/common/set_routing_layers.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/common/set_routing_layers.tcl`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 if { [info exists ::env(RT_CLOCK_MIN_LAYER)]} {
     set clock_min_layer $::env(RT_CLOCK_MIN_LAYER)
 }
 if { [info exists ::env(RT_CLOCK_MAX_LAYER)]} {
     set clock_max_layer $::env(RT_CLOCK_MAX_LAYER)
 }
 
-puts "\[INFO]: Setting signal min routing layer to: $signal_min_layer and clock min routing layer to $clock_min_layer. "
-puts "\[INFO]: Setting signal max routing layer to: $signal_max_layer and clock max routing layer to $clock_max_layer. "
+puts "\[INFO] Setting signal min routing layer to: $signal_min_layer and clock min routing layer to $clock_min_layer. "
+puts "\[INFO] Setting signal max routing layer to: $signal_max_layer and clock max routing layer to $clock_max_layer. "
 
 set_routing_layers -signal [subst $signal_min_layer]-[subst $signal_max_layer] -clock [subst $clock_min_layer]-[subst $clock_max_layer]
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/cts.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/cts.tcl`

 * *Files 13% similar despite different names*

```diff
@@ -8,46 +8,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+source $::env(SCRIPTS_DIR)/openroad/common/resizer.tcl
 
-if { ![info exists ::env(CLOCK_NET)] } {
-    puts "\[INFO]: ::env(CLOCK_NET) doesn't exist. Assuming clockless design and exiting…"
-    write
-    exit 0
-}
-
-if {![info exist ::env(MAX_TRANSITION_CONSTRAINT)]} {
-    set ::env(MAX_TRANSITION_CONSTRAINT) [expr {0.1 * $::env(CLOCK_PERIOD)}]
-} else {
-    set ::env(MAX_TRANSITION_CONSTRAINT) [expr {$::env(MAX_TRANSITION_CONSTRAINT) * 1000}]
-}
-set max_slew [expr {$::env(MAX_TRANSITION_CONSTRAINT) * 1e-9}]; # must convert to seconds
-set max_cap [expr {$::env(CTS_MAX_CAP) * 1e-12}]; # must convert to farad
+load_rsz_corners
+read_current_odb
 
 # set rc values
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 estimate_parasitics -placement
 
 # Clone clock tree inverters next to register loads
 # so cts does not try to buffer the inverted clocks.
 repair_clock_inverters
 
 puts "\[INFO\] Configuring cts characterization…"
-configure_cts_characterization\
-    -max_slew $max_slew\
-    -max_cap $max_cap
-
-puts "\[INFO]: Performing clock tree synthesis…"
-puts "\[INFO]: Looking for the following net(s): $::env(CLOCK_NET)"
-puts "\[INFO]: Running Clock Tree Synthesis…"
+set cts_characterization_args [list]
+lappend -max_cap [expr {$::env(CTS_MAX_CAP) * 1e-12}]; # pF -> F
+if { [info exists ::env(MAX_FANOUT_CONSTRAINT)] } {
+    lappend -max_slew [expr {$::env(MAX_FANOUT_CONSTRAINT) * 1e-9}]; # ns -> S
+}
+configure_cts_characterization {*}$cts_characterization_args
+
+puts "\[INFO] Performing clock tree synthesis…"
+puts "\[INFO] Looking for the following net(s): $::env(CLOCK_NET)"
+puts "\[INFO] Running Clock Tree Synthesis…"
 
 set arg_list [list]
 
 lappend arg_list -buf_list $::env(CTS_CLK_BUFFERS)
 lappend arg_list -root_buf $::env(CTS_ROOT_BUFFER)
 lappend arg_list -sink_clustering_size $::env(CTS_SINK_CLUSTERING_SIZE)
 lappend arg_list -sink_clustering_max_diameter $::env(CTS_SINK_CLUSTERING_MAX_DIAMETER)
@@ -62,38 +54,29 @@
 }
 
 clock_tree_synthesis {*}$arg_list
 
 set_propagated_clock [all_clocks]
 
 estimate_parasitics -placement
-puts "\[INFO]: Repairing long wires on clock nets…"
+puts "\[INFO] Repairing long wires on clock nets…"
 # CTS leaves a long wire from the pad to the clock tree root.
 repair_clock_nets -max_wire_length $::env(CTS_CLK_MAX_WIRE_LENGTH)
 
 estimate_parasitics -placement
-write
+write_views
 
 puts "\[INFO\] Legalizing…"
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
 estimate_parasitics -placement
 
-write
+write_views
 
 if { [catch {check_placement -verbose} errmsg] } {
     puts stderr $errmsg
     exit 1
 }
 
-puts "cts_report"
+puts "%OL_CREATE_REPORT cts.rpt"
 report_cts
-puts "cts_report_end"
-
-if {[info exists ::env(CLOCK_PORT)]} {
-    if { [info exists ::env(CTS_REPORT_TIMING)] && $::env(CTS_REPORT_TIMING) } {
-        set ::env(RUN_STANDALONE) 0
-        source $::env(SCRIPTS_DIR)/openroad/sta.tcl
-    }
-} else {
-    puts "\[WARN\]: No CLOCK_PORT found. Skipping STA…"
-}
+puts "%OL_END_REPORT"
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/dpl.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/dpl.tcl`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+read_current_odb
 
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
 if { [catch {check_placement -verbose} errmsg] } {
     puts stderr $errmsg
     exit 1
 }
 
-write
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/fill.tcl` & `openlane-2.0.0b1/openlane/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-# Copyright 2020-2022 Efabless Corporation
+# Copyright 2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
-
-filler_placement "$::env(DECAP_CELL) $::env(FILL_CELL)"
-
-write
+from .drc import DRC, Violation
+from .toolbox import Toolbox
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/floorplan.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/floorplan.tcl`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read_libs
+read_pnr_libs
 read_lefs
-read_netlist
+read_current_netlist
 
 unset_propagated_clock [all_clocks]
 
 set bottom_margin  [expr $::env(PLACE_SITE_HEIGHT) * $::env(BOTTOM_MARGIN_MULT)]
 set top_margin  [expr $::env(PLACE_SITE_HEIGHT) * $::env(TOP_MARGIN_MULT)]
 set left_margin [expr $::env(PLACE_SITE_WIDTH) * $::env(LEFT_MARGIN_MULT)]
 set right_margin [expr $::env(PLACE_SITE_WIDTH) * $::env(RIGHT_MARGIN_MULT)]
@@ -92,11 +92,11 @@
 }
 
 puts "\[INFO] Floorplanned on a die area of $::env(DIE_AREA) (µm)."
 puts "\[INFO] Floorplanned on a core area of $::env(CORE_AREA) (µm)."
 
 source $::env(TRACKS_INFO_FILE_PROCESSED)
 
-utl::metric "die__area"  $::env(DIE_AREA)
-utl::metric "core__area" $::env(CORE_AREA)
+write_metric_str "design__die__bbox"  $::env(DIE_AREA)
+write_metric_str "design__core__bbox" $::env(CORE_AREA)
 
-write
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/gpl.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/gpl.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+read_current_odb
 
 set ::block [[[::ord::get_db] getChip] getBlock]
 set ::insts [$::block getInsts]
 
 set placement_needed 0
 
 foreach inst $::insts {
@@ -26,15 +26,15 @@
 	}
 }
 
 if { !$placement_needed } {
 	puts "\[WARN] All instances are FIXED/FIRM."
 	puts "\[WARN] No need to perform global placement."
 	puts "\[WARN] Skipping…"
-	write
+	write_views
 	exit 0
 }
 
 set arg_list [list]
 
 lappend arg_list -density [expr $::env(PL_TARGET_DENSITY_PCT) / 100.0]
 
@@ -57,22 +57,11 @@
 set cell_pad_side [expr $::env(GPL_CELL_PADDING) / 2]
 
 lappend arg_list -pad_right $cell_pad_side
 lappend arg_list -pad_left $cell_pad_side
 
 global_placement {*}$arg_list
 
-write
+source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
+estimate_parasitics -placement
 
-if {[info exists ::env(CLOCK_PORT)]} {
-	if { $::env(PL_ESTIMATE_PARASITICS) == 1 } {
-		unset_propagated_clock [all_clocks]
-		# set rc values
-		source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
-		estimate_parasitics -placement
-
-		set ::env(RUN_STANDALONE) 0
-		source $::env(SCRIPTS_DIR)/openroad/sta.tcl
-	}
-} else {
-	puts "\[WARN\]: No CLOCK_PORT found. Skipping STA…"
-}
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/grt.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/repair_design.tcl`

 * *Files 27% similar despite different names*

```diff
@@ -8,48 +8,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+source $::env(SCRIPTS_DIR)/openroad/common/resizer.tcl
 
-set_propagated_clock [all_clocks]
+load_rsz_corners
+read_current_odb
 
-if { $::env(GRT_REPAIR_ANTENNAS) } {
-    set diode_split [split $::env(DIODE_CELL) "/"]
-    set_placement_padding -masters [lindex $diode_split 0] -left $::env(DIODE_PADDING)
+unset_propagated_clock [all_clocks]
+
+set_dont_touch_objects
+set_dont_use_cells
+
+# set rc values
+source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
+
+# CTS and detailed placement move instances, so update parastic estimates.
+# estimate wire rc parasitics
+estimate_parasitics -placement
+
+
+# Buffer I/O
+if { $::env(DESIGN_REPAIR_BUFFER_INPUT_PORTS) } {
+    buffer_ports -inputs
 }
 
-source $::env(SCRIPTS_DIR)/openroad/common/grt.tcl
+if { $::env(DESIGN_REPAIR_BUFFER_OUTPUT_PORTS) } {
+    buffer_ports -outputs
+}
 
-# Check Antennas (Pre-Repair)
-puts "%OL_CREATE_REPORT antenna.rpt"
-check_antennas -verbose
-puts "%OL_END_REPORT"
-
-if { $::env(GRT_REPAIR_ANTENNAS) } {
-    repair_antennas "[lindex $diode_split 0]" -iterations $::env(GRT_ANTENNA_ITERS)
-    check_placement
-
-    # Check Antennas (Post-Repair)
-    puts "%OL_CREATE_REPORT antenna_after.rpt"
-    check_antennas -verbose
-    puts "%OL_END_REPORT"
+# Repair Design
+repair_design\
+    -max_wire_length $::env(DESIGN_REPAIR_MAX_WIRE_LENGTH) \
+    -slew_margin $::env(DESIGN_REPAIR_MAX_SLEW_PCT) \
+    -cap_margin $::env(DESIGN_REPAIR_MAX_CAP_PCT)
+
+if { $::env(DESIGN_REPAIR_TIE_FANOUT) } {
+    # repair tie lo fanout
+    repair_tie_fanout -separation $::env(DESIGN_REPAIR_TIE_SEPARATION) $::env(SYNTH_TIELO_CELL)
+    # repair tie hi fanout
+    repair_tie_fanout -separation $::env(DESIGN_REPAIR_TIE_SEPARATION) $::env(SYNTH_TIEHI_CELL)
 }
 
-write
+report_floating_nets -verbose
+
+# Legalize
+source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
-if {[info exists ::env(CLOCK_PORT)]} {
-    if { $::env(GRT_ESTIMATE_PARASITICS) == 1 } {
-        # set rc values
-        source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
-        # estimate wire rc parasitics
-        estimate_parasitics -global_routing
-
-        set ::env(RUN_STANDALONE) 0
-        source $::env(SCRIPTS_DIR)/openroad/sta.tcl
-    }
-} else {
-    puts "\[WARN\]: No CLOCK_PORT found. Skipping STA…"
+if { [catch {check_placement -verbose} errmsg] } {
+    puts stderr $errmsg
+    exit 1
 }
+
+unset_dont_touch_objects
+
+source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
+estimate_parasitics -placement
+
+write_views
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/gui.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/write_views.tcl`

 * *Files 17% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+read_current_odb
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/insert_buffer.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/insert_buffer.tcl`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,14 @@
         odb::dbITerm_connect $net_out_iterm $new_net
         odb::dbITerm_connect $in_iterm $old_net
     }
 }
 
 if { [info exists ::env(INSERT_BUFFER_COMMAND) ]} {
     source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-    read
+    read_current_odb
 
     set arg_list [split $::env(INSERT_BUFFER_COMMAND) " "]
     insert_buffer {*}$arg_list
 
-    write
+    write_views
 }
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/ioplacer.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/ioplacer.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+read_current_odb
 
 if { [info exists ::env(CONTEXTUAL_IO_FLAG)] } {
 	read_lef $::env(placement_tmpfiles)/top_level.lef
 }
 
 if {$::env(FP_IO_HLENGTH) != "" && $::env(FP_IO_HLENGTH) != ""} {
 	set_pin_length -hor_length $::env(FP_IO_HLENGTH) \
@@ -30,15 +30,15 @@
 
 if {$::env(FP_IO_VTHICKNESS_MULT) != "" && $::env(FP_IO_HTHICKNESS_MULT) != ""} {
 	set_pin_thick_multiplier -hor_multiplier $::env(FP_IO_HTHICKNESS_MULT) \
 		-ver_multiplier $::env(FP_IO_VTHICKNESS_MULT)
 }
 
 set arg_list [list]
-if { $::env(FP_IO_MODE) == 1 } {
+if { $::env(FP_IO_MODE) == "random_equidistant" } {
 	lappend arg_list -random
 }
 
 if { $::env(FP_IO_MIN_DISTANCE) != "" } {
 	lappend arg_list -min_distance $::env(FP_IO_MIN_DISTANCE)
 }
 
@@ -46,8 +46,8 @@
 set VMETAL $::env(FP_IO_VLAYER)
 
 place_pins {*}$arg_list \
 	-random_seed 42 \
 	-hor_layers $HMETAL \
 	-ver_layers $VMETAL
 
-write
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/irdrop.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/irdrop.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
 
-read
+read_current_odb
 
 source $::env(SCRIPTS_DIR)/openroad/common/set_power_nets.tcl
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 
-read_spef $::env(CURRENT_SPEF)
+read_spef $::env(CURRENT_SPEF_DEFAULT_CORNER)
 
 puts "%OL_CREATE_REPORT irdrop.rpt"
 analyze_power_grid -net $::env(VDD_NET) -outfile $::env(STEP_DIR)/voltages.csv
 puts "%OL_END_REPORT"
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/pdn.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/pdn.tcl`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+read_current_odb
 
 if {![info exists ::env(PDN_CFG)]} {
     set ::env(PDN_CFG) $::env(SCRIPTS_DIR)/openroad/common/pdn_cfg.tcl
 }
 
 source $::env(SCRIPTS_DIR)/openroad/common/set_power_nets.tcl
 
@@ -40,8 +40,8 @@
 # https://github.com/The-OpenROAD-Project/OpenROAD/issues/2126
 # checks for unconnected nodes (e.g., isolated rails or stripes)
 if { $::env(FP_PDN_CHECK_NODES) } {
     check_power_grid -net $::env(VDD_NET)
     check_power_grid -net $::env(GND_NET)
 }
 
-write
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/rcx.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/rcx.tcl`

 * *Files 17% similar despite different names*

```diff
@@ -8,29 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-if { [info exists ::env(RCX_LEF)] } {
-    read_lef $::env(RCX_LEF)
-    read_def $::env(RCX_DEF)
-    read_libs -override "$::env(RCX_LIB)"
-} else {
-    read
-}
+read_lefs "RCX_LEF"
+read_def $::env(CURRENT_DEF)
+
 
 set_propagated_clock [all_clocks]
 
 set rcx_flags ""
 if { !$::env(RCX_MERGE_VIA_WIRE_RES) } {
     set rcx_flags "-no_merge_via_res"
 }
 
 # RCX
 puts "Using RCX ruleset '$::env(RCX_RULESET)'…"
 define_process_corner -ext_model_index 0 CURRENT_CORNER
 extract_parasitics $rcx_flags\
     -ext_model_file $::env(RCX_RULESET)\
     -lef_res
-write
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postcts.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/rsz_timing_postcts.tcl`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+source $::env(SCRIPTS_DIR)/openroad/common/resizer.tcl
 
-set_propagated_clock [all_clocks]
+load_rsz_corners
+read_current_odb
 
-# set don't touch nets
-source $::env(SCRIPTS_DIR)/openroad/common/resizer.tcl
-set_dont_touch_rx "$::env(RSZ_DONT_TOUCH_RX)"
+set_propagated_clock [all_clocks]
 
-# set don't use cells
-if { [info exists ::env(RSZ_DONT_USE_CELLS)] } {
-    set_dont_use $::env(RSZ_DONT_USE_CELLS)
-}
+set_dont_touch_objects
+set_dont_use_cells
 
 # set rc values
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 
 # CTS and detailed placement move instances, so update parastic estimates.
 # estimate wire rc parasitics
 estimate_parasitics -placement
@@ -51,15 +48,13 @@
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
 
 if { [catch {check_placement -verbose} errmsg] } {
     puts stderr $errmsg
     exit 1
 }
 
-unset_dont_touch_rx "$::env(RSZ_DONT_TOUCH_RX)"
-
-write
+unset_dont_touch_objects
 
-# Run post-timing optimization STA
+source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 estimate_parasitics -placement
-set ::env(RUN_STANDALONE) 0
-source $::env(SCRIPTS_DIR)/openroad/sta.tcl
+
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postgrt.tcl` & `openlane-2.0.0b1/openlane/scripts/openroad/rsz_timing_postgrt.tcl`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+source $::env(SCRIPTS_DIR)/openroad/common/resizer.tcl
 
-set_propagated_clock [all_clocks]
+load_rsz_corners
+read_current_odb
 
-# set don't touch nets
-source $::env(SCRIPTS_DIR)/openroad/common/resizer.tcl
-set_dont_touch_rx "$::env(RSZ_DONT_TOUCH_RX)"
+set_propagated_clock [all_clocks]
 
-# set don't use cells
-if { [info exists ::env(RSZ_DONT_USE_CELLS)] } {
-    set_dont_use $::env(RSZ_DONT_USE_CELLS)
-}
+set_dont_touch_objects
+set_dont_use_cells
 
 # set rc values
 source $::env(SCRIPTS_DIR)/openroad/common/set_rc.tcl
 
-# estimate wire rc parasitics
+# (Re-)GRT and Estimate Parasitics
+source $::env(SCRIPTS_DIR)/openroad/common/grt.tcl
 estimate_parasitics -global_routing
 
 # Resize
 repair_timing -setup \
     -setup_margin $::env(GRT_RESIZER_SETUP_SLACK_MARGIN) \
     -max_buffer_percent $::env(GRT_RESIZER_SETUP_MAX_BUFFER_PCT)
 
@@ -42,25 +40,17 @@
 lappend arg_list -hold_margin $::env(GRT_RESIZER_HOLD_SLACK_MARGIN)
 lappend arg_list -max_buffer_percent $::env(GRT_RESIZER_HOLD_MAX_BUFFER_PCT)
 if { $::env(GRT_RESIZER_ALLOW_SETUP_VIOS) == 1 } {
     lappend arg_list -allow_setup_violations
 }
 repair_timing {*}$arg_list
 
+# Re-DPL and GRT
 source $::env(SCRIPTS_DIR)/openroad/common/dpl.tcl
-
 if { [catch {check_placement -verbose} errmsg] } {
     puts stderr $errmsg
     exit 1
 }
-
-unset_dont_touch_rx "$::env(RSZ_DONT_TOUCH_RX)"
-
-# Re-GRT
+unset_dont_touch_objects
 source $::env(SCRIPTS_DIR)/openroad/common/grt.tcl
 
-write
-
-# Run post timing optimizations STA
-estimate_parasitics -global_routing
-set ::env(RUN_STANDALONE) 0
-source $::env(SCRIPTS_DIR)/openroad/sta.tcl
+write_views
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/tapcell.tcl` & `openlane-2.0.0b1/openlane/config/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright 2020-2022 Efabless Corporation
+# Copyright 2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
+"""
+The Configuration Module
+------------------------
 
-tapcell\
-    -distance $::env(FP_TAPCELL_DIST)\
-    -tapcell_master "$::env(FP_WELLTAP_CELL)"\
-    -endcap_master "$::env(FP_ENDCAP_CELL)"\
-    -halo_width_x $::env(FP_TAP_HORIZONTAL_HALO)\
-    -halo_width_y $::env(FP_TAP_VERTICAL_HALO)
-
-write
+This modules includes various functions for importing and/or generating OpenLane
+configuration objects. Configuration objects are the primary input to a flow.
+"""
+from .preprocessor import Keys
+from .variable import Instance, Macro, Variable
+from .config import Meta, Config, InvalidConfig
+from .flow import all_variables as universal_flow_config_variables
```

### Comparing `openlane-2.0.0a9/openlane/scripts/openroad/write_views.tcl` & `openlane-2.0.0b1/openlane/__version__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright 2022 Efabless Corporation
+# Copyright 2023 Efabless Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-source $::env(SCRIPTS_DIR)/openroad/common/io.tcl
-read
-write
+__version__ = "2.0.0b1"
+
+if __name__ == "__main__":
+    print(__version__, end="")
```

### Comparing `openlane-2.0.0a9/openlane/scripts/yosys/synthesize.tcl` & `openlane-2.0.0b1/openlane/scripts/yosys/synthesize.tcl`

 * *Files 11% similar despite different names*

```diff
@@ -7,96 +7,77 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+#  Parts of this file adapted from https://github.com/YosysHQ/yosys/blob/master/techlibs/common/synth.cc
+#
+#  Copyright (C) 2012  Claire Xenia Wolf <claire@yosyshq.com>
+#
+#  Permission to use, copy, modify, and/or distribute this software for any
+#  purpose with or without fee is hereby granted, provided that the above
+#  copyright notice and this permission notice appear in all copies.
+#
+#  THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
+#  WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
+#  MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
+#  ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
+#  WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
+#  ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
+#  OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+#
 yosys -import
 
-# inputs expected as env vars
-set buffering $::env(SYNTH_BUFFERING)
-set sizing $::env(SYNTH_SIZING)
-set vtop $::env(DESIGN_NAME)
-set sclib $::env(LIB_SYNTH)
-if {[info exists ::env(DFF_LIB_SYNTH)]} {
-    set dfflib $::env(DFF_LIB_SYNTH)
-} else {
-    set dfflib $sclib
-}
+source $::env(SCRIPTS_DIR)/yosys/common.tcl
 
-if { [info exists ::env(SYNTH_DEFINES) ] } {
-    foreach define $::env(SYNTH_DEFINES) {
-        log "Defining $define"
-        verilog_defines -D$define
-    }
-}
+set report_dir $::env(STEP_DIR)/reports
+file mkdir $report_dir
 
-set vIdirsArgs ""
-if {[info exist ::env(VERILOG_INCLUDE_DIRS)]} {
-    foreach dir $::env(VERILOG_INCLUDE_DIRS) {
-        lappend vIdirsArgs "-I$dir"
-    }
-    set vIdirsArgs [join $vIdirsArgs]
-}
+# inputs expected as env vars
+set vtop $::env(DESIGN_NAME)
 
-if { $::env(SYNTH_READ_BLACKBOX_LIB) } {
-    log "Reading $::env(LIB_SYNTH) as a blackbox"
-    foreach lib $::env(LIB_SYNTH) {
-        read_liberty -lib -ignore_miss_dir -setattr blackbox $lib
-    }
+set lib_args [list]
+foreach lib $::env(SYNTH_LIBS) {
+    lappend lib_args -liberty $lib
 }
 
-if { [info exists ::env(EXTRA_LIBS) ] } {
-    foreach lib $::env(EXTRA_LIBS) {
-        read_liberty -lib -ignore_miss_dir -setattr blackbox $lib
-    }
+if {[info exists ::env(DFF_LIB_SYNTH)]} {
+    set dfflib $::env(DFF_LIB_SYNTH)
+} else {
+    set dfflib $::env(SYNTH_LIBS)
 }
 
-if { [info exists ::env(EXTRA_VERILOG_MODELS)] } {
-    foreach verilog_file $::env(EXTRA_VERILOG_MODELS) {
-        read_verilog -sv -lib {*}$vIdirsArgs $verilog_file
-    }
+set dfflib_args [list]
+foreach lib $dfflib {
+    lappend dfflib_args -liberty $lib
 }
 
+read_deps
 
-# ns expected (in sdc as well)
-set clock_period [expr {$::env(CLOCK_PERIOD)*1000}]
-
-set driver  $::env(SYNTH_DRIVING_CELL)
-set cload   $::env(SYNTH_CAP_LOAD)
-# input pin cap of IN_3VX8
 set max_FO $::env(MAX_FANOUT_CONSTRAINT)
-if {![info exist ::env(MAX_TRANSITION_CONSTRAINT)]} {
-    set ::env(MAX_TRANSITION_CONSTRAINT) [expr {0.1*$clock_period}]
-} else {
-    set ::env(MAX_TRANSITION_CONSTRAINT) [expr {$::env(MAX_TRANSITION_CONSTRAINT) * 1000}]
+set max_TR 0
+if { [info exist ::env(MAX_TRANSITION_CONSTRAINT)]} {
+    set max_TR [expr {$::env(MAX_TRANSITION_CONSTRAINT) * 1000}]; # ns -> ps
 }
-set max_Tran $::env(MAX_TRANSITION_CONSTRAINT)
-
+set clock_period [expr {$::env(CLOCK_PERIOD) * 1000}]; # ns -> ps
 
 # Mapping parameters
 set A_factor  0.00
 set B_factor  0.88
 set F_factor  0.00
 
-# Don't change these unless you know what you are doing
-set stat_ext    ".stat.rpt"
-set chk_ext    ".chk.rpt"
-set gl_ext      ".gl.v"
-set constr_ext  ".$clock_period.constr"
-set timing_ext  ".timing.txt"
-set abc_ext     ".abc"
-
 
 # Create SDC File
 set sdc_file $::env(STEP_DIR)/synthesis.sdc
 set outfile [open ${sdc_file} w]
-puts $outfile "set_driving_cell ${driver}"
-puts $outfile "set_load ${cload}"
+puts $outfile "set_driving_cell $::env(SYNTH_DRIVING_CELL)"
+puts $outfile "set_load $::env(OUTPUT_CAP_LOAD)"
 close $outfile
 
 
 # Assemble Scripts (By Strategy)
 set abc_rs_K    "resub,-K,"
 set abc_rs      "resub"
 set abc_rsz     "resub,-z"
@@ -127,17 +108,21 @@
 
 set map_old_cnt			    "map,-p,-a,-B,0.2,-A,0.9,-M,0"
 set map_old_dly			    "map,-p,-B,0.2,-A,0.9,-M,0"
 set abc_retime_area   	"retime,-D,{D},-M,5"
 set abc_retime_dly    	"retime,-D,{D},-M,6"
 set abc_map_new_area  	"amap,-m,-Q,0.1,-F,20,-A,20,-C,5000"
 
-if {$buffering==1} {
-    set abc_fine_tune		"buffer,-N,${max_FO},-S,${max_Tran};upsize,{D};dnsize,{D}"
-} elseif {$sizing} {
+if { $::env(SYNTH_ABC_BUFFERING) == 1 } {
+    set max_tr_arg ""
+    if { $max_TR != 0 } {
+        set max_tr_arg ",-S,${max_TR}"
+    }
+    set abc_fine_tune		"buffer,-N,${max_FO}${max_tr_arg};upsize,{D};dnsize,{D}"
+} elseif {$::env(SYNTH_SIZING)} {
     set abc_fine_tune       "upsize,{D};dnsize,{D}"
 } else {
     set abc_fine_tune       ""
 }
 
 
 set delay_scripts [list \
@@ -207,195 +192,228 @@
 if { !($adder_type in [list "YOSYS" "FA" "RCA" "CSA"]) } {
     log -stderr "\[ERROR] Misformatted SYNTH_ADDER_TYPE (\"$::env(SYNTH_ADDER_TYPE)\")."
     log -stderr "\[ERROR] Correct format is \"YOSYS|FA|RCA|CSA\"."
     exit 1
 }
 
 # Start Synthesis
-for { set i 0 } { $i < [llength $::env(VERILOG_FILES)] } { incr i } {
-    read_verilog -sv {*}$vIdirsArgs [lindex $::env(VERILOG_FILES) $i]
+set verilog_include_args [list]
+if {[info exist ::env(VERILOG_INCLUDE_DIRS)]} {
+    foreach dir $::env(VERILOG_INCLUDE_DIRS) {
+        lappend verilog_include_args "-I$dir"
+    }
+}
+foreach file $::env(VERILOG_FILES) {
+    read_verilog -sv {*}$verilog_include_args $file
 }
 
 if { [info exists ::env(SYNTH_PARAMETERS) ] } {
     foreach define $::env(SYNTH_PARAMETERS) {
         set param_and_value [split $define "="]
         lassign $param_and_value param value
         chparam -set $param $value $vtop
     }
 }
 
 select -module $vtop
 show -format dot -prefix $::env(STEP_DIR)/hierarchy
 select -clear
-
 hierarchy -check -top $vtop
+yosys rename -top $vtop
+
+if { $::env(SYNTH_ELABORATE_ONLY) } {
+    yosys proc
+    if { $::env(SYNTH_ELABORATE_FLATTEN) } {
+        flatten
+    }
+
+    setattr -set keep 1
+
+    splitnets
+    opt_clean -purge
+
+    tee -o "$report_dir/chk.rpt" check
+    tee -o "$report_dir/stat.json" stat -json
+
+    write_verilog -noattr -noexpr -nohex -nodec -defparam "$::env(SAVE_NETLIST)"
+    exit 0
+}
 
 # Infer tri-state buffers.
 set tbuf_map false
 if { [info exists ::env(TRISTATE_BUFFER_MAP)] } {
-    if { [file exists $::env(TRISTATE_BUFFER_MAP)] } {
-        set tbuf_map true
-        tribuf
-    } else {
-        log "WARNING: TRISTATE_BUFFER_MAP is defined but could not be found: $::env(TRISTATE_BUFFER_MAP)"
-    }
+    set tbuf_map true
+    tribuf
 }
 
 # Handle technology mapping of RCS/CSA adders
 if { $adder_type == "RCA"} {
-    if { [info exists ::env(RIPPLE_CARRY_ADDER_MAP)] && [file exists $::env(RIPPLE_CARRY_ADDER_MAP)] } {
+    if { [info exists ::env(RIPPLE_CARRY_ADDER_MAP)] } {
+        log "\[INFO] Applying ripple carry adder mapping from '$::env(RIPPLE_CARRY_ADDER_MAP)'…"
         techmap -map $::env(RIPPLE_CARRY_ADDER_MAP)
     }
 } elseif { $adder_type == "CSA"} {
-    if { [info exists ::env(CARRY_SELECT_ADDER_MAP)] && [file exists $::env(CARRY_SELECT_ADDER_MAP)] } {
+    if { [info exists ::env(CARRY_SELECT_ADDER_MAP)] } {
+        log "\[INFO] Applying carry-select adder mapping from '$::env(CARRY_SELECT_ADDER_MAP)'…"
         techmap -map $::env(CARRY_SELECT_ADDER_MAP)
     }
 }
 
-if { $::env(SYNTH_NO_FLAT) } {
-    synth -top $vtop
-} else {
-    synth -top $vtop -flatten
-}
+# <synth> split to run check -assert in the middle
+hierarchy -check -auto-top
+proc_clean
+proc_rmdead
+proc_prune
+proc_init
+proc_arst
+proc_rom
+proc_mux
+proc_dlatch
+proc_dff
+proc_memwr
+proc_clean
+tee -o "$report_dir/pre_synth_chk.rpt" check
+opt_expr
+if { $::env(SYNTH_NO_FLAT) != 1 } {
+    flatten
+}
+opt_expr
+opt_clean
+opt -nodffe -nosdff
+fsm
+opt
+wreduce
+peepopt
+opt_clean
+alumacc
+share
+opt
+memory -nomap
+opt_clean
+opt -fast -full
+memory_map
+opt -full
+techmap
+opt -fast
+abc -fast
+opt -fast
+hierarchy -check
+stat
+check
 
 if { [info exists ::env(SYNTH_EXTRA_MAPPING_FILE)] } {
-    if { [file exists $::env(SYNTH_EXTRA_MAPPING_FILE)] } {
-        log "\[INFO\] applying mappings in $::env(SYNTH_EXTRA_MAPPING_FILE)"
-        techmap -map $::env(SYNTH_EXTRA_MAPPING_FILE)
-    } else {
-        log -stderr "\[ERROR] file not found $::env(SYNTH_EXTRA_MAPPING_FILE)."
-    }
+    log "\[INFO] Applying extra mappings from '$::env(SYNTH_EXTRA_MAPPING_FILE)'…"
+    techmap -map $::env(SYNTH_EXTRA_MAPPING_FILE)
 }
 
 show -format dot -prefix $::env(STEP_DIR)/post_techmap
 
 if { $::env(SYNTH_SHARE_RESOURCES) } {
     share -aggressive
 }
 
 set fa_map false
 if { $adder_type == "FA" } {
-    if { [info exists ::env(FULL_ADDER_MAP)] && [file exists $::env(FULL_ADDER_MAP)] } {
+    if { [info exists ::env(FULL_ADDER_MAP)] } {
         extract_fa -fa -v
         extract_fa -ha -v
         set fa_map true
     }
 }
 
 opt
 opt_clean -purge
 
-set report_dir $::env(STEP_DIR)/reports
-file mkdir $report_dir
-
 tee -o "$report_dir/pre_techmap.json" stat -json
 
 # Map tri-state buffers
 if { $tbuf_map } {
     log {mapping tbuf}
+    log "\[INFO] Applying tri-state buffer mapping from '$::env(TRISTATE_BUFFER_MAP)'…"
     techmap -map $::env(TRISTATE_BUFFER_MAP)
     simplemap
 }
 
 # Map full adders
 if { $fa_map } {
+    log "\[INFO] Applying full-adder mapping from '$::env(FULL_ADDER_MAP)'…"
     techmap -map $::env(FULL_ADDER_MAP)
 }
 
 # Handle technology mapping of latches
-if { [info exists ::env(SYNTH_LATCH_MAP)] && [file exists $::env(SYNTH_LATCH_MAP)] } {
+if { [info exists ::env(SYNTH_LATCH_MAP)] } {
+    log "\[INFO] Applying latch mapping from '$::env(SYNTH_LATCH_MAP)'…"
     techmap -map $::env(SYNTH_LATCH_MAP)
     simplemap
 }
 
-dfflibmap -liberty $dfflib
+dfflibmap {*}$dfflib_args
 tee -o "$report_dir/post_dff.json" stat -json
 
 proc run_strategy {output script strategy_name {postfix_with_strategy 0}} {
     upvar clock_period clock_period
-    upvar sdc_file sdc
-    upvar sclib lib
+    upvar sdc_file sdc_file
     upvar report_dir report_dir
+    upvar lib_args lib_args
 
     log "\[INFO\] USING STRATEGY $strategy_name"
 
     set strategy_escaped [string map {" " _} $strategy_name]
 
     design -load checkpoint
-
     abc -D "$clock_period" \
-        -constr "$sdc" \
-        -liberty "$lib" \
+        -constr "$sdc_file" \
         -script "$script" \
-        -showtmp
+        -showtmp \
+        {*}$lib_args
 
     setundef -zero
 
     hilomap -hicell $::env(SYNTH_TIEHI_CELL) -locell $::env(SYNTH_TIELO_CELL)
 
-    splitnets
-    opt_clean -purge
-    insbuf -buf {*}[split $::env(SYNTH_BUFFER_CELL) "/"]
+    if { $::env(SYNTH_SPLITNETS) } {
+        splitnets
+        opt_clean -purge
+    }
+
+    if { $::env(SYNTH_DIRECT_WIRE_BUFFERING) } {
+        insbuf -buf {*}[split $::env(SYNTH_BUFFER_CELL) "/"]
+    }
 
     tee -o "$report_dir/chk.rpt" check
-    tee -o "$report_dir/stat.json" stat -top $::env(DESIGN_NAME) -liberty [lindex $::env(LIB_SYNTH) 0] -json
+    tee -o "$report_dir/stat.json" stat -json
 
-    if { [info exists ::env(SYNTH_AUTONAME)] && $::env(SYNTH_AUTONAME) } {
+    if { $::env(SYNTH_AUTONAME) } {
         # Generate public names for the various nets, resulting in very long names that include
         # the full heirarchy, which is preferable to the internal names that are simply
         # sequential numbers such as `_000019_`. Renamed net names can be very long, such as:
         #     manual_reset_gf180mcu_fd_sc_mcu7t5v0__dffq_1_Q_D_gf180mcu_ \
         #     fd_sc_mcu7t5v0__nor3_1_ZN_A1_gf180mcu_fd_sc_mcu7t5v0__aoi21_ \
         #     1_A2_A1_gf180mcu_fd_sc_mcu7t5v0__nand3_1_ZN_A3_gf180mcu_fd_ \
         #     sc_mcu7t5v0__and3_1_A3_Z_gf180mcu_fd_sc_mcu7t5v0__buf_1_I_Z
         autoname
     }
     write_verilog -noattr -noexpr -nohex -nodec -defparam $output
-    if { $::env(QUIT_ON_SYNTH_CHECKS) == 1 } {
-        read_liberty -ignore_miss_func $::env(LIB_SYNTH)
-        check -assert $::env(DESIGN_NAME)
-    }
     design -reset
 }
 design -save checkpoint
 
 run_strategy\
     "$::env(SAVE_NETLIST)"\
     "$strategy_script"\
     "$strategy_name"
 
 if { $::env(SYNTH_NO_FLAT) } {
     design -reset
 
-    if { [info exists ::env(SYNTH_DEFINES) ] } {
-        foreach define $::env(SYNTH_DEFINES) {
-            log "Defining $define"
-            verilog_defines -D$define
-        }
-    }
-
-    foreach lib $::env(LIB_SYNTH_COMPLETE_NO_PG) {
-        read_liberty -lib -ignore_miss_dir -setattr blackbox $lib
-    }
-
-    if { [info exists ::env(EXTRA_LIBS) ] } {
-        foreach lib $::env(EXTRA_LIBS) {
-            read_liberty -lib -ignore_miss_dir -setattr blackbox $lib
-        }
-    }
-
-    if { [info exists ::env(EXTRA_VERILOG_MODELS)] } {
-        foreach verilog_file $::env(EXTRA_VERILOG_MODELS) {
-            read_verilog -sv -lib {*}$vIdirsArgs $verilog_file
-        }
-    }
+    read_deps
 
     file copy -force $::env(SAVE_NETLIST) $::env(synthesis_results)/$::env(DESIGN_NAME).hierarchy.nl.v
     read_verilog -sv $::env(SAVE_NETLIST)
-    synth -top $vtop -flatten
+    synth -flatten
 
     design -save checkpoint
     run_strategy\
         "$::env(SAVE_NETLIST)"\
         "$strategy_script"\
         "$strategy_name"
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openlane-2.0.0a9/openlane/smoke_test_design/src/spm.v` & `openlane-2.0.0b1/openlane/smoke_test_design/src/spm.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a9/openlane/state/__init__.py` & `openlane-2.0.0b1/openlane/utils/memoize.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,12 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from functools import lru_cache
 
-"""
-The State Module
 
-This module manages the State of a Design before and after the execution of an
-OpenLane step. The State is essentially a list of views in various formats in
-addition to the cumulative set of metrics created by a given step.
-"""
-from .design_format import DesignFormat, DesignFormatByID
-from .state import State, InvalidState
+def memoize(fn):
+    return lru_cache(16, True)(fn)
```

### Comparing `openlane-2.0.0a9/openlane/steps/__init__.py` & `openlane-2.0.0b1/openlane/steps/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,27 +10,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 The Step Module
+---------------
 
 This modules includes various functions for importing and/or generating OpenLane
 configuration objects. Configuration objects are the primary input to a flow.
 """
 from .step import (
-    Step,
-    StepConditionLambda,
-    MissingInputError,
-    DeferredStepError,
     StepError,
+    DeferredStepError,
+    StepException,
+    Step,
 )
 from .tclstep import TclStep
 from . import checker as Checker
+
+# You'll notice some TclStep subclasses are exposed separately-
+# this is for documentation.
 from . import yosys as Yosys
+from .yosys import YosysStep
+
 from . import openroad as OpenROAD
+from .openroad import OpenROADStep
+
 from . import magic as Magic
+from .magic import MagicStep
+
 from . import odb as Odb
+from .odb import OdbpyStep
+
 from . import netgen as Netgen
+from .netgen import NetgenStep
+
 from . import klayout as KLayout
 from . import misc as Misc
```

### Comparing `openlane-2.0.0a9/openlane/steps/checker.py` & `openlane-2.0.0b1/openlane/steps/checker.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,207 +8,264 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import ClassVar, Tuple
 from decimal import Decimal
 from typing import Optional
-from abc import abstractmethod
 
-from .step import Step, StepError, DeferredStepError, State
+from .step import ViewsUpdate, MetricsUpdate, Step, StepError, DeferredStepError, State
 
 from ..config import Variable
 from ..logging import err, warn, info
 
 
 class MetricChecker(Step):
-    deferred = True
+    """
+    Raises a (deferred) error if a Decimal metric exceeds a ccertain threshold.
+    """
+
+    inputs = []
+    outputs = []
+
+    metric_name: ClassVar[str] = NotImplemented
+    metric_description: ClassVar[str] = NotImplemented
+    deferred: ClassVar[bool] = True
+
+    @classmethod
+    def get_help_md(Self):
+        threshold_string = Self.get_threshold_description(None)
+        if threshold_string is None:
+            threshold_string = str(Self.get_threshold(None))
+        dynamic_docstring = "Raises"
+        if Self.deferred:
+            dynamic_docstring += " a deferred error"
+        else:
+            dynamic_docstring += " an immediate error"
+        dynamic_docstring += f" if {Self.metric_description} (metric: ``{Self.metric_name}``) are >= {threshold_string}."
 
-    @abstractmethod
-    def get_metric_name(self) -> str:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def get_metric_description(self) -> str:
-        raise NotImplementedError()
+        return super().get_help_md(dynamic_docstring)
 
-    def get_threshold(self) -> Optional[Decimal]:
+    def get_threshold(self: Optional["MetricChecker"]) -> Optional[Decimal]:
         return Decimal(0)
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run()
+    def get_threshold_description(self: Optional["MetricChecker"]) -> Optional[str]:
+        return None
 
-        metric_name = self.get_metric_name()
-        metric_description = self.get_metric_description()
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         threshold = self.get_threshold()
 
         if threshold is None:
             warn(
-                f"Threshold for {metric_description} is not set. The checker will be skipped."
+                f"Threshold for {self.metric_description} is not set. The checker will be skipped."
             )
         else:
-            metric_value = state_out.metrics.get(metric_name)
+            metric_value = state_in.metrics.get(self.metric_name)
             if metric_value is not None:
                 if metric_value > threshold:
-                    error_msg = f"{metric_value} {metric_description} found."
+                    error_msg = f"{metric_value} {self.metric_description} found."
                     if self.deferred:
                         err(f"{error_msg} - deferred")
                         raise DeferredStepError(error_msg)
                     else:
                         err(f"{error_msg}")
                         raise StepError(error_msg)
 
                 else:
-                    info(f"Check for {metric_description} clear.")
+                    info(f"Check for {self.metric_description} clear.")
             else:
                 warn(
-                    f"The {metric_description} metric was not found. Are you sure the relevant step was run?"
+                    f"The {self.metric_description} metric was not found. Are you sure the relevant step was run?"
                 )
 
-        return state_out
+        return {}, {}
 
 
 @Step.factory.register()
 class YosysUnmappedCells(MetricChecker):
     id = "Checker.YosysUnmappedCells"
     flow_control_variable = "QUIT_ON_UNMAPPED_CELLS"
-    name = "Unmapped cells Checker"
+    name = "Unmapped Cells Checker"
     deferred = False
 
+    metric_name = "design__instance_unmapped__count"
+    metric_description = "Unmapped Yosys instances"
+
     config_vars = [
         Variable(
             "QUIT_ON_UNMAPPED_CELLS",
             bool,
-            "Checks for unmapped cells after sythesis",
+            "Checks for unmapped cells after synthesis.",
+            deprecated_names=["CHECK_UNMAPPED_CELLS"],
             default=True,
         ),
     ]
 
-    def get_metric_name(self) -> str:
-        return "design__instance_unmapped__count"
 
-    def get_metric_description(self) -> str:
-        return "Unmapped Yosys instances"
+@Step.factory.register()
+class YosysSynthChecks(MetricChecker):
+    id = "Checker.YosysChecks"
+    flow_control_variable = "QUIT_ON_SYNTH_CHECKS"
+    name = "Yosys Synth Checks"
+    deferred = False
+
+    metric_name = "synthesis__check_error__count"
+    metric_description = "Yosys check errors"
+
+    config_vars = [
+        Variable(
+            "QUIT_ON_SYNTH_CHECKS",
+            bool,
+            "Quits the flow if one or more synthesis check errors are flagged. This checks for combinational loops and/or wires with no drivers.",
+            default=True,
+        ),
+    ]
 
 
 @Step.factory.register()
 class TrDRC(MetricChecker):
     id = "Checker.TrDRC"
     flow_control_variable = "QUIT_ON_TR_DRC"
     name = "Routing DRC Checker"
-    long_name = "Routing Design Rule Check"
+    long_name = "Routing Design Rule Checker"
+
+    metric_name = "route__drc_errors"
+    metric_description = "Routing DRC errors"
 
     config_vars = [
         Variable(
             "QUIT_ON_TR_DRC",
             bool,
             "Checks for DRC violations after routing and exits the flow if any was found.",
             default=True,
         ),
     ]
 
-    def get_metric_name(self) -> str:
-        return "route__drc_errors"
-
-    def get_metric_description(self) -> str:
-        return "Routing DRC errors"
-
 
 @Step.factory.register()
 class MagicDRC(MetricChecker):
     id = "Checker.MagicDRC"
     flow_control_variable = "QUIT_ON_MAGIC_DRC"
     name = "Magic DRC Checker"
-    long_name = "Magic Design Rule Check"
+    long_name = "Magic Design Rule Checker"
+
+    metric_name = "magic__drc_error__count"
+    metric_description = "Magic DRC errors"
 
     config_vars = [
         Variable(
             "QUIT_ON_MAGIC_DRC",
             bool,
             "Checks for DRC violations after magic DRC is executed and exits the flow if any was found.",
             default=True,
         ),
     ]
 
-    def get_metric_name(self) -> str:
-        return "magic__drc_errors"
-
-    def get_metric_description(self) -> str:
-        return "Magic DRC errors"
-
 
 @Step.factory.register()
 class IllegalOverlap(MetricChecker):
     id = "Checker.IllegalOverlap"
     flow_control_variable = "QUIT_ON_ILLEGAL_OVERLAPS"
     name = "Illegal Overlap Checker"
-    long_name = "Spice Extraction-based Illegal Overlap Check"
+    long_name = "Spice Extraction-based Illegal Overlap Checker"
+
+    metric_name = "magic__illegal_overlap__count"
+    metric_description = "Magic Illegal Overlap errors"
 
     config_vars = [
         Variable(
             "QUIT_ON_ILLEGAL_OVERLAPS",
             bool,
             "Checks for illegal overlaps during magic extraction. In some cases, these imply existing undetected shorts in the design. It also exits the flow if any was found.",
             default=True,
         ),
     ]
 
-    def get_metric_name(self) -> str:
-        return "magic__illegal__overlaps"
 
-    def get_metric_description(self) -> str:
-        return "Magic Illegal Overlap errors"
+@Step.factory.register()
+class DisconnectedPins(MetricChecker):
+    id = "Checker.DisconnectedPins"
+    flow_control_variable = "QUIT_ON_DISCONNECTED_PINS"
+    name = "Disconnected Pins Checker"
+    deferred = False
+
+    metric_name = "design__disconnected_pins__count"
+    metric_description = "Disconnected pins count"
+
+    config_vars = [
+        Variable(
+            "QUIT_ON_DISCONNECTED_PINS",
+            bool,
+            "Checks for disconnected instance pins.",
+            default=True,
+        ),
+    ]
 
 
 @Step.factory.register()
 class WireLength(MetricChecker):
     id = "Checker.WireLength"
     flow_control_variable = "QUIT_ON_LONG_WIRE"
     name = "Wire Length Threshold Checker"
 
-    metric_name = "route__max__wirelength"
+    metric_name = "route__wirelength__max"
     metric_description = "Threshold-surpassing long wires"
 
     config_vars = [
         Variable(
             "QUIT_ON_LONG_WIRE",
             bool,
             "Exits the flow if any wire length exceeds the threshold set in the PDK.",
             default=False,
         ),
     ]
 
-    def get_metric_name(self) -> str:
-        return "route__max__wirelength"
-
-    def get_metric_description(self) -> str:
-        return "Threshold-surpassing long wires"
-
     def get_threshold(self) -> Optional[Decimal]:
         threshold = self.config["WIRE_LENGTH_THRESHOLD"]
         assert threshold is None or isinstance(threshold, Decimal)
         return threshold
 
+    def get_threshold_description(self) -> Optional[str]:
+        return "the threshold specified in the configuration file."
+
+
+@Step.factory.register()
+class XOR(MetricChecker):
+    id = "Checker.XOR"
+    flow_control_variable = "QUIT_ON_XOR_ERROR"
+    name = "XOR Difference Checker"
+    long_name = "Magic vs. KLayout XOR Difference Checker"
+
+    metric_name = "design__xor_difference__count"
+    metric_description = "XOR differences"
+
+    config_vars = [
+        Variable(
+            "QUIT_ON_XOR_ERROR",
+            bool,
+            "Checks for geometric differences between the Magic and KLayout stream-outs.",
+            default=True,
+        ),
+    ]
+
 
 @Step.factory.register()
 class LVS(MetricChecker):
     id = "Checker.LVS"
     flow_control_variable = "QUIT_ON_LVS_ERROR"
     name = "LVS Error Checker"
     long_name = "Layout vs. Schematic Error Checker"
 
+    metric_name = "design__lvs_errors__count"
+    metric_description = "LVS errors"
+
     config_vars = [
         Variable(
             "QUIT_ON_LVS_ERROR",
             bool,
             "Checks for LVS errors after netgen LVS is executed and exits the flow if any was found.",
             default=True,
         ),
     ]
-
-    def get_metric_name(self) -> str:
-        return "lvs__total__errors"
-
-    def get_metric_description(self) -> str:
-        return "LVS errors"
```

### Comparing `openlane-2.0.0a9/openlane/steps/common_variables.py` & `openlane-2.0.0b1/openlane/steps/common_variables.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 io_layer_variables = [
     Variable(
         "FP_IO_VEXTEND",
         Decimal,
         "Extends the vertical io pins outside of the die by the specified units.",
         default=0,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "FP_IO_HEXTEND",
         Decimal,
         "Extends the horizontal io pins outside of the die by the specified units.",
         default=0,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "FP_IO_VLENGTH",
         Decimal,
         "The length of the vertical IOs.",
         default=4,
         units="µm",
@@ -61,36 +61,36 @@
 
 pdn_variables = [
     Variable(
         "FP_PDN_VOFFSET",
         Decimal,
         "The offset of the vertical power stripes on the metal layer 4 in the power distribution network.",
         default=16.32,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "FP_PDN_VPITCH",
         Decimal,
         "The pitch of the vertical power stripes on the metal layer 4 in the power distribution network.",
         default=153.6,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "FP_PDN_HOFFSET",
         Decimal,
         "The offset of the horizontal power stripes on the metal layer 5 in the power distribution network.",
         default=16.65,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "FP_PDN_HPITCH",
         Decimal,
         "The pitch of the horizontal power stripes on the metal layer 5 in the power distribution network.",
         default=153.18,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "FP_PDN_AUTO_ADJUST",
         bool,
         "Decides whether or not the flow should attempt to re-adjust the power grid, in order for it to fit inside the core area of the design, if needed.",
         default=True,
     ),
@@ -116,24 +116,24 @@
         "FP_PDN_CHECK_NODES",
         bool,
         "Enables checking for unconnected nodes in the power grid.",
         default=True,
     ),
     Variable(
         "FP_PDN_HORIZONTAL_HALO",
-        str,
+        Decimal,
         "Sets the horizontal halo around the macros during power grid insertion.",
         default=10,
         units="µm",
     ),
     Variable(
         "FP_PDN_VERTICAL_HALO",
         Decimal,
         "Sets the vertical halo around the macros during power grid insertion.",
-        default="expr::$FP_PDN_HORIZONTAL_HALO",
+        default=10,
         units="µm",
     ),
     Variable(
         "DESIGN_IS_CORE",
         bool,
         "Controls the layers used in the power grid. Depending on whether the design is the core of a chip or a macro inside the core.",
         default=True,
@@ -174,84 +174,79 @@
         default=True,
     ),
     Variable(
         "PL_MAX_DISPLACEMENT_X",
         Decimal,
         "Specifies how far an instance can be moved along the X-axis when finding a site where it can be placed during detailed placement.",
         default=500,
-        units="μm",
+        units="µm",
     ),
     Variable(
         "PL_MAX_DISPLACEMENT_Y",
         Decimal,
         "Specifies how far an instance can be moved along the Y-axis when finding a site where it can be placed during detailed placement.",
         default=100,
-        units="μm",
+        units="µm",
     ),
 ]
 
-
-rsz_variables = dpl_variables + [
+grt_variables = routing_layer_variables + [
     Variable(
-        "RSZ_DONT_TOUCH_RX",
-        str,
-        'A single regular expression designating nets as "don\'t touch" by resizer optimizations.',
-        default="$^",
-        deprecated_names=["UNBUFFER_NETS"],
+        "DIODE_PADDING",
+        int,
+        "Diode cell padding; increases the width of diode cells during placement checks..",
+        default=2,
+        units="sites",
     ),
     Variable(
-        "RSZ_DONT_USE_CELLS",
-        Optional[List[str]],
-        "An optional list of cells to not use during resizer optimizations.",
-        deprecated_names=["DONT_USE_CELLS"],
+        "GRT_ALLOW_CONGESTION",
+        bool,
+        "Allow congestion during global routing",
+        default=False,
+    ),
+    Variable(
+        "GRT_REPAIR_ANTENNAS",
+        bool,
+        "Specifies the insertion strategy of diodes to be used in the flow.",
+        default=True,
     ),
-]
-
-constraint_variables = [
     Variable(
-        "MAX_FANOUT_CONSTRAINT",
+        "GRT_ANTENNA_ITERS",
         int,
-        "The max load that the output ports can drive to be used as a constraint on Synthesis and CTS.",
-        default=10,
-        units="cells",
-        deprecated_names=["SYNTH_MAX_FANOUT"],
+        "The maximum number of iterations for global antenna repairs.",
+        default=3,
+        deprecated_names=["GRT_ANT_ITERS"],
     ),
     Variable(
-        "MAX_TRANSITION_CONSTRAINT",
-        Optional[Decimal],
-        "The max transition time (slew) from high to low or low to high on cell inputs in ns to be used as a constraint on Synthesis and CTS. If not provided, it is calculated at runtime as `10%` of the provided clock period, unless that exceeds the PDK's `DEFAULT_MAX_TRAN` value.",
-        units="ns",
-        deprecated_names=["SYNTH_MAX_TRAN"],
+        "GRT_OVERFLOW_ITERS",
+        int,
+        "The maximum number of iterations waiting for the overflow to reach the desired value.",
+        default=50,
     ),
+]
+
+rsz_variables = dpl_variables + [
     Variable(
-        "CLOCK_UNCERTAINTY_CONSTRAINT",
-        Decimal,
-        "Specifies a value for the clock uncertainty/jitter for timing analysis.",
-        default=0.25,
-        units="ns",
-        deprecated_names=["SYNTH_CLOCK_UNCERTAINTY"],
+        "RSZ_DONT_TOUCH_RX",
+        str,
+        'A single regular expression designating nets or instances as "don\'t touch" by design repairs or resizer optimizations.',
+        default="$^",
+        deprecated_names=["UNBUFFER_NETS"],
     ),
     Variable(
-        "CLOCK_TRANSITION_CONSTRAINT",
-        Decimal,
-        "Specifies a value for the clock transition/slew for timing analysis.",
-        default=0.15,
-        units="ns",
-        deprecated_names=["SYNTH_CLOCK_TRANSITION"],
+        "RSZ_DONT_TOUCH_LIST",
+        Optional[List[str]],
+        'A list of nets and instances as "don\'t touch" by design repairs or resizer optimizations.',
+        default=None,
     ),
     Variable(
-        "TIME_DERATING_CONSTRAINT",
-        Decimal,
-        "Specifies a derating factor to multiply the path delays with. It specifies the upper and lower ranges of timing.",
-        default=5,
-        units="%",
-        deprecated_names=["SYNTH_TIMING_DERATE"],
+        "RSZ_DONT_USE_CELLS",
+        Optional[List[str]],
+        "An optional list of cells to not use during design repair or resizer optimizations in addition to cells that are excluded from PNR altogether.",
+        deprecated_names=["DONT_USE_CELLS"],
     ),
     Variable(
-        "IO_DELAY_CONSTRAINT",
-        Decimal,
-        "Specifies the percentage of the clock period used in the input/output delays.",
-        default=20,
-        units="%",
-        deprecated_names=["IO_PCT"],
+        "RSZ_CORNERS",
+        Optional[List[str]],
+        "A list of fully-qualifiedd IPVT corners to use during resizer optimizations. If unspecified, the value for `STA_CORNERS` from the PDK will be used.",
     ),
 ]
```

### Comparing `openlane-2.0.0a9/openlane/steps/klayout.py` & `openlane-2.0.0b1/openlane/steps/klayout.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,82 +8,117 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
+import subprocess
 import sys
-from typing import Optional
 from base64 import b64encode
+from typing import Optional, List, Tuple
 
-from .step import Step, StepError
-from ..state import DesignFormat, State
+from .step import ViewsUpdate, MetricsUpdate, Step, StepError, StepException
 
 from ..logging import warn
-from ..config import Path, Variable
-from ..common import get_script_dir
+from ..utils import Toolbox
+from ..config import Variable, Config
+from ..state import DesignFormat, State
+from ..common import Path, get_script_dir
+
+
+def get_lef_args(config: Config, toolbox: Toolbox) -> List[str]:
+    tech_lefs = toolbox.filter_views(config, config["TECH_LEFS"])
+    if len(tech_lefs) != 1:
+        raise StepException(
+            "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
+        )
+
+    lef_args = [
+        "--input-lef",
+        str(tech_lefs[0]),
+    ]
+
+    for lef in config["CELL_LEFS"]:
+        lef_args.append("--input-lef")
+        lef_args.append(str(lef))
+
+    macro_lefs = toolbox.get_macro_views(config, DesignFormat.LEF)
+    for lef in macro_lefs:
+        lef_args.append("--input-lef")
+        lef_args.append(str(lef))
+
+    if extra_lefs := config["EXTRA_LEFS"]:
+        for lef in extra_lefs:
+            lef_args.append("--input-lef")
+            lef_args.append(str(lef))
+
+    return lef_args
 
 
 @Step.factory.register()
 class StreamOut(Step):
+    """
+    Converts DEF views into GDSII streams using KLayout.
+
+    The PDK must support KLayout for this step to work, otherwise
+    it will be skipped.
+
+    If ``PRIMARY_SIGNOFF_TOOL`` is set to ``"klayout"``, both GDS and KLAYOUT_GDS
+    will be updated, and if set to another tool, only ``KLAYOUT_GDS`` will be
+    updated.
+    """
+
     id = "KLayout.StreamOut"
-    name = "GDS-II Stream Out (KLayout)"
+    name = "GDSII Stream Out (KLayout)"
     flow_control_variable = "RUN_KLAYOUT_STREAMOUT"
 
     inputs = [DesignFormat.DEF]
     outputs = [DesignFormat.GDS, DesignFormat.KLAYOUT_GDS]
 
     config_vars = [
         Variable(
             "RUN_KLAYOUT_STREAMOUT",
             bool,
-            "Enables streaming GDS-II using KLayout.",
+            "Enables streaming GDSII using KLayout.",
             default=True,
             deprecated_names=["RUN_KLAYOUT"],
         )
     ]
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run(**kwargs)
-
-        assert isinstance(self.state_in, State)
-
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         lyp = self.config["KLAYOUT_PROPERTIES"]
         lyt = self.config["KLAYOUT_TECH"]
         lym = self.config["KLAYOUT_DEF_LAYER_MAP"]
         if None in [lyp, lyt, lym]:
             if self.config["PRIMARY_SIGNOFF_TOOL"].value == "klayout":
                 raise StepError(
                     "One of KLAYOUT_PROPERTIES, KLAYOUT_TECH or KLAYOUT_DEF_LAYER_MAP is unset, yet, KLayout is set as the primary sign-off tool."
                 )
             warn(
-                "One of KLAYOUT_PROPERTIES, KLAYOUT_TECH or KLAYOUT_DEF_LAYER_MAP is unset. Skipping KLayout stream-out…"
+                "One of KLAYOUT_PROPERTIES, KLAYOUT_TECH or KLAYOUT_DEF_LAYER_MAP is unset. Returning state unaltered…"
             )
-            return state_out
+            return {}, {}
+
+        views_updates: ViewsUpdate = {}
 
         klayout_gds_out = os.path.join(
             self.step_dir,
-            f"{self.config['DESIGN_NAME']}.{DesignFormat.KLAYOUT_GDS.value[1]}",
+            f"{self.config['DESIGN_NAME']}.{DesignFormat.KLAYOUT_GDS.value.extension}",
         )
 
-        layout_args = [
-            "--input-lef",
-            self.config["TECH_LEF"],
-        ]
-        for lef in self.config["CELL_LEFS"]:
-            layout_args.append("--input-lef")
-            layout_args.append(lef)
-        if extra_lefs := self.config["EXTRA_LEFS"]:
-            for lef in extra_lefs:
-                layout_args.append("--input-lef")
-                layout_args.append(lef)
+        layout_args = []
+        layout_args += get_lef_args(self.config, self.toolbox)
+
         for gds in self.config["CELL_GDS"]:
             layout_args.append("--with-gds-file")
             layout_args.append(gds)
+        for gds in self.toolbox.get_macro_views(self.config, DesignFormat.GDS):
+            layout_args.append("--with-gds-file")
+            layout_args.append(gds)
         if extra_gds := self.config["EXTRA_GDS_FILES"]:
             for gds in extra_gds:
                 layout_args.append("--with-gds-file")
                 layout_args.append(gds)
 
         kwargs, env = self.extract_env(kwargs)
 
@@ -91,15 +126,15 @@
             [
                 sys.executable,
                 os.path.join(
                     get_script_dir(),
                     "klayout",
                     "stream_out.py",
                 ),
-                self.state_in[DesignFormat.DEF.value[0]],
+                state_in[DesignFormat.DEF.value.id],
                 "--output",
                 klayout_gds_out,
                 "--lyt",
                 lyt,
                 "--lyp",
                 lyp,
                 "--lym",
@@ -107,20 +142,20 @@
                 "--top",
                 self.config["DESIGN_NAME"],
             ]
             + layout_args,
             env=env,
         )
 
-        state_out[DesignFormat.KLAYOUT_GDS] = Path(klayout_gds_out)
+        views_updates[DesignFormat.KLAYOUT_GDS] = Path(klayout_gds_out)
 
         if self.config["PRIMARY_SIGNOFF_TOOL"].value == "klayout":
-            state_out[DesignFormat.GDS] = state_out[DesignFormat.KLAYOUT_GDS]
+            views_updates[DesignFormat.GDS] = views_updates[DesignFormat.KLAYOUT_GDS]
 
-        return state_out
+        return views_updates, {}
 
     def layout_preview(self) -> Optional[str]:
         if self.state_out is None:
             return None
         assert self.toolbox is not None
 
         if image := self.toolbox.render_png(
@@ -130,53 +165,58 @@
             return f'<img src="data:image/png;base64,{image_encoded}" />'
 
         return None
 
 
 @Step.factory.register()
 class XOR(Step):
+    """
+    Performs an XOR operation on the Magic and KLayout GDS views. The idea is:
+    if there's any difference between the GDSII streams between the two tools,
+    one of them have it wrong and that may lead to ambiguity.
+    """
+
     id = "KLayout.XOR"
     name = "KLayout vs. Magic XOR"
     flow_control_variable = "RUN_KLAYOUT_XOR"
 
     inputs = [
         DesignFormat.MAG_GDS,
         DesignFormat.KLAYOUT_GDS,
     ]
+    outputs = []
 
     config_vars = [
         Variable(
             "RUN_KLAYOUT_XOR",
             bool,
-            "Enables running KLayout XOR on the two GDS-II files generated by Magic and Klayout. Stream-outs for both KLayout and Magic should have already run, and the PDK must support both signoff tools.",
+            "Enables running KLayout XOR on the two GDSII files generated by Magic and Klayout. Stream-outs for both KLayout and Magic should have already run, and the PDK must support both signoff tools.",
             default=True,
         ),
         Variable(
             "KLAYOUT_XOR_THREADS",
             int,
             "Specifies number of threads used in the KLayout XOR check.",
             default=1,
         ),
     ]
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run(**kwargs)
-
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         ignored = ""
         if ignore_list := self.config["KLAYOUT_XOR_IGNORE_LAYERS"]:
             ignored = ";".join(ignore_list)
 
-        layout_a = state_out[DesignFormat.MAG_GDS]
+        layout_a = state_in[DesignFormat.MAG_GDS]
         if layout_a is None:
-            warn("No Magic stream-out has been performed. Skipping XOR…")
-            return state_out
-        layout_b = state_out[DesignFormat.KLAYOUT_GDS]
+            warn("No Magic stream-out has been performed. Skipping XOR process…")
+            return {}, {}
+        layout_b = state_in[DesignFormat.KLAYOUT_GDS]
         if layout_b is None:
-            warn("No KLayout stream-out has been performed. Skipping XOR…")
-            return state_out
+            warn("No KLayout stream-out has been performed. Skipping XOR process…")
+            return {}, {}
 
         kwargs, env = self.extract_env(kwargs)
 
         self.run_subprocess(
             [
                 "ruby",
                 os.path.join(
@@ -192,8 +232,63 @@
                 ignored,
                 layout_a,
                 layout_b,
             ],
             env=env,
         )
 
-        return state_out
+        difference_count = int(
+            open(os.path.join(self.step_dir, "difference_count.rpt")).read().strip()
+        )
+
+        return {}, {"design__xor_difference__count": difference_count}
+
+
+@Step.factory.register()
+class OpenGUI(Step):
+    """
+    Opens the DEF view in the KLayout GUI, with layers loaded and mapped
+    properly. Useful to inspect ``.klayout.xml`` database files and the like.
+    """
+
+    id = "KLayout.OpenGUI"
+    name = "Open In GUI"
+
+    inputs = [DesignFormat.DEF]
+    outputs = []
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        lyp = self.config["KLAYOUT_PROPERTIES"]
+        lyt = self.config["KLAYOUT_TECH"]
+        lym = self.config["KLAYOUT_DEF_LAYER_MAP"]
+        if None in [lyp, lyt, lym]:
+            raise StepError(
+                "Cannot open design in KLayout as the PDK does not appear to support KLayout."
+            )
+
+        lefs = get_lef_args(self.config, self.toolbox)
+        kwargs, env = self.extract_env(kwargs)
+
+        cmd = [
+            sys.executable,
+            os.path.join(
+                get_script_dir(),
+                "klayout",
+                "open_design.py",
+            ),
+            "--lyt",
+            str(lyt),
+            "--lyp",
+            str(lyp),
+            "--lym",
+            str(lym),
+            str(state_in[DesignFormat.DEF]),
+        ] + lefs
+
+        print(" ".join(cmd))
+
+        subprocess.check_call(
+            cmd,
+            env=env,
+        )
+
+        return {}, {}
```

### Comparing `openlane-2.0.0a9/openlane/steps/magic.py` & `openlane-2.0.0b1/openlane/steps/magic.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 from abc import abstractmethod
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
-from .step import Step
+from .step import StepError, ViewsUpdate, MetricsUpdate, Step
 from .tclstep import TclStep
 from ..state import DesignFormat, State
 
 from ..config import Variable
 from ..common import get_script_dir
 from ..utils import DRC as DRCObject
 
@@ -40,15 +40,15 @@
             bool,
             'A flag to enable polygon subcells in magic for gds read potentially speeding up magic. From magic docs: "Put non-Manhattan polygons. This prevents interations with other polygons on the same plane and so reduces tile splitting."',
             default=False,
         ),
         Variable(
             "MAGIC_GDS_ALLOW_ABSTRACT",
             bool,
-            "A flag to allow abstract view of macros during magic gds generation..",
+            "A flag to allow abstract view of macros when processing GDS files in Magic.",
             default=False,
         ),
         Variable(
             "MAGIC_DEF_NO_BLOCKAGES",
             bool,
             "If set to true, blockages in DEF files are ignored. Otherwise, they are read as sheets of metal by Magic.",
             default=True,
@@ -70,131 +70,174 @@
             "magic",
             "-dnull",
             "-noconsole",
             "-rcfile",
             str(self.config["MAGICRC"]),
         ]
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         # https://github.com/RTimothyEdwards/magic/issues/218
-        kwargs["stdin"] = open(self.get_script_path(), encoding="utf8")
-        return super().run(**kwargs)
+        kwargs, env = self.extract_env(kwargs)
+        kwargs["stdin"] = open(
+            os.path.join(get_script_dir(), "magic", "wrapper.tcl"), encoding="utf8"
+        )
+        env["MAGIC_SCRIPT"] = self.get_script_path()
+
+        env["MACRO_GDS_FILES"] = ""
+        for gds in self.toolbox.get_macro_views(self.config, DesignFormat.GDS):
+            env["MACRO_GDS_FILES"] += f" {gds}"
+
+        return super().run(state_in, env=env, **kwargs)
 
 
 @Step.factory.register()
 class WriteLEF(MagicStep):
+    """
+    Writes a LEF view of the design using the GDS using Magic.
+    """
+
     id = "Magic.WriteLEF"
     name = "Write LEF (Magic)"
     flow_control_variable = "RUN_MAGIC_WRITE_LEF"
 
-    inputs = [DesignFormat.GDS]
+    inputs = [DesignFormat.GDS, DesignFormat.DEF]
     outputs = [DesignFormat.LEF]
 
     config_vars = MagicStep.config_vars + [
         Variable(
             "RUN_MAGIC_WRITE_LEF",
             bool,
             "Generate a LEF view using Magic.",
             default=True,
             deprecated_names=["MAGIC_GENERATE_LEF"],
         ),
         Variable(
-            "MAGIC_GENERATE_MAGLEF",
+            "MAGIC_LEF_WRITE_USE_GDS",
             bool,
-            "Generate a MAGLEF view using Magic alongside generated LEF views.",
-            default=True,
+            "A flag to choose whether to use GDS for spice extraction or not. If not, then the extraction will be done using the DEF/LEF, which is faster.",
+            default=False,
         ),
         Variable(
             "MAGIC_WRITE_FULL_LEF",
             bool,
             "A flag to specify whether or not the output LEF should include all shapes inside the macro or an abstracted view of the macro lef view via magic.",
             default=False,
         ),
     ]
 
     def get_script_path(self):
-        raise NotImplementedError()
+        return os.path.join(get_script_dir(), "magic", "lef.tcl")
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        kwargs, env = self.extract_env(kwargs)
+        env["MAGTYPE"] = "mag"
+        return super().run(state_in, **kwargs)
 
 
 @Step.factory.register()
 class StreamOut(MagicStep):
+    """
+    Converts DEF views into GDSII streams using Magic.
+
+    If ``PRIMARY_SIGNOFF_TOOL`` is set to ``"magic"``, both GDS and MAG_GDS
+    will be updated, and if set to another tool, only ``MAG_GDS`` will be
+    updated.
+    """
+
     id = "Magic.StreamOut"
-    name = "GDS-II Stream Out (Magic)"
+    name = "GDSII Stream Out (Magic)"
     flow_control_variable = "RUN_MAGIC_STREAMOUT"
 
     inputs = [DesignFormat.DEF]
     outputs = [DesignFormat.GDS, DesignFormat.MAG_GDS]
 
     config_vars = MagicStep.config_vars + [
         Variable(
             "RUN_MAGIC_STREAMOUT",
             bool,
             "Enables running GDSII streaming out using Magic.",
             default=True,
             deprecated_names=["RUN_MAGIC"],
         ),
         Variable(
-            "MAGIC_PAD",
-            bool,
-            "A flag to pad the views generated by magic (.mag, .lef, .gds) by one site.",
-            default=False,
-        ),
-        Variable(
             "DIE_AREA",
             Optional[str],
             'Specific die area to be used in floorplanning when `FP_SIZING` is set to `absolute`. Specified as a 4-corner rectangle "x0 y0 x1 y1".',
-            units="μm",
+            units="µm",
         ),
         Variable(
             "MAGIC_ZEROIZE_ORIGIN",
             bool,
             "A flag to move the layout such that it's origin in the lef generated by magic is 0,0.",
             default=False,
         ),
         Variable(
-            "MAGIC_GENERATE_GDS",
-            bool,
-            "A flag to generate gds view via magic.",
-            default=True,
-        ),
-        Variable(
-            "MAGIC_DISABLE_HIER_GDS",
+            "MAGIC_DISABLE_CIF_INFO",
             bool,
-            "A flag to disable cif hier and array during GDSII writing.* 1=Enabled `<so this hier gds will be disabled>`, 0=Disabled `<so this hier gds will be enabled>`.",
+            "A flag to disable writing Caltech Intermediate Format (CIF) hierarchy and subcell array information to the GDSII file.",
             default=True,
+            deprecated_names=["MAGIC_DISABLE_HIER_GDS"],
         ),
+        # Variable(
+        #     "MAGIC_GDS_FLATTEN",
+        #     bool,
+        #     "todo",
+        #     default=True,
+        # ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "magic", "def", "mag_gds.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
-        assert isinstance(self.state_in, State)
-        if die_area := self.state_in.metrics.get("die__area"):
+        if die_area := state_in.metrics.get("design__die__bbox"):
             env["DIE_AREA"] = die_area
 
-        state_out = super().run(env=env, **kwargs)
+        magic_log_dir = os.path.join(self.step_dir, "magic.log")
+
+        views_updates, metrics_updates = super().run(
+            state_in,
+            env=env,
+            log_to=magic_log_dir,
+            **kwargs,
+        )
         if self.config["PRIMARY_SIGNOFF_TOOL"].value == "magic":
-            state_out[DesignFormat.GDS] = state_out[DesignFormat.MAG_GDS]
-        return state_out
+            views_updates[DesignFormat.GDS] = views_updates[DesignFormat.MAG_GDS]
+
+        for line in open(magic_log_dir, encoding="utf8"):
+            if "Calma output error" in line:
+                raise StepError("Magic GDS was written with errors.")
+
+        return views_updates, metrics_updates
 
 
 @Step.factory.register()
 class DRC(MagicStep):
+    """
+    Performs `design rule checking <https://en.wikipedia.org/wiki/Design_rule_checking>`_
+    on the GDSII stream using Magic.
+
+    This also converts the results to a KLayout database, which can be loaded.
+
+    The metrics will be updated with ``magic__drc_error__count``. You can use
+    `the relevant checker <#Checker.MagicDRC>`_ to quit if that number is
+    nonzero.
+    """
+
     id = "Magic.DRC"
     name = "DRC"
     long_name = "Design Rule Checks"
 
     flow_control_variable = "RUN_MAGIC_DRC"
 
     inputs = [DesignFormat.DEF, DesignFormat.GDS]
     outputs = []
 
-    config_vars = [
+    config_vars = MagicStep.config_vars + [
         Variable(
             "RUN_MAGIC_DRC",
             bool,
             "Enables running magic DRC on GDSII produced by Magic.",
             default=True,
         ),
         Variable(
@@ -204,35 +247,49 @@
             default=False,
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "magic", "drc.tcl")
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run(**kwargs)
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
 
         reports_dir = os.path.join(self.step_dir, "reports")
         report_path = os.path.join(reports_dir, "drc.rpt")
-        report_str = open(report_path, encoding="utf8").read()
+        report_stats = os.stat(report_path)
 
-        drc = DRCObject.from_magic(report_str)
-        drc_bbox = [
-            bbox for violation in drc.violations for bbox in violation.bounding_boxes
-        ]
-        state_out.metrics["magic__drc_errors"] = len(drc_bbox)
+        drc_db_file = None
+        if report_stats.st_size >= 0:  # 134217728:
+            drc_db_file = os.path.join(reports_dir, "drc.db")
+
+        drc, bbox_count = DRCObject.from_magic(
+            open(report_path, encoding="utf8"),
+            db_file=drc_db_file,
+        )
+
+        klayout_db_path = os.path.join(reports_dir, "drc.klayout.xml")
+        drc.to_klayout_xml(open(klayout_db_path, "wb"))
 
-        with open(os.path.join(reports_dir, "drc.klayout.xml"), "w") as f:
-            f.write(drc.to_klayout_xml())
+        metrics_updates["magic__drc_error__count"] = bbox_count
 
-        return state_out
+        return views_updates, metrics_updates
 
 
 @Step.factory.register()
 class SpiceExtraction(MagicStep):
+    """
+    Extracts a SPICE netlist from the GDSII stream. Used in Layout vs. Schematic
+    checks.
+
+    Also, the metrics will be updated with ``magic__illegal_overlap__count``. You can use
+    `the relevant checker <#Checker.IllegalOverlap>`_ to quit if that number is
+    nonzero.
+    """
+
     id = "Magic.SpiceExtraction"
     name = "SPICE Extraction"
     long_name = "SPICE Model Extraction"
 
     inputs = [DesignFormat.GDS, DesignFormat.DEF]
     outputs = [DesignFormat.SPICE]
 
@@ -251,16 +308,17 @@
             deprecated_names=["LVS_CONNECT_BY_LABEL"],
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "magic", "extract_spice.tcl")
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run(**kwargs)
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
 
         feedback_path = os.path.join(self.step_dir, "feedback.txt")
         feedback_string = open(feedback_path, encoding="utf8").read()
-        state_out.metrics["magic__illegal__overlaps"] = feedback_string.count(
+        metrics_updates["magic__illegal_overlap__count"] = feedback_string.count(
             "Illegal overlap"
         )
-        return state_out
+
+        return views_updates, metrics_updates
```

### Comparing `openlane-2.0.0a9/openlane/steps/netgen.py` & `openlane-2.0.0b1/openlane/steps/netgen.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
 import glob
 import json
-from typing import List, Dict
 from abc import abstractmethod
+from typing import List, Dict, Tuple
 
-from .step import Step
-from ..logging import info
+from .step import ViewsUpdate, MetricsUpdate, Step
 from .tclstep import TclStep
-from ..config import Variable
 
+from ..logging import info
+from ..config import Variable, Keys
 from ..state import DesignFormat, State
 
 
 def get_metrics(stats: Dict) -> Dict:
     metrics: Dict = {}
     if not stats:
         return metrics
@@ -79,21 +79,21 @@
         + net_differences
         + property_fails
         + device_fails
         + net_fails
         + pin_fails
     )
     metrics = {}
-    metrics["lvs__device_count_difference"] = device_differences
-    metrics["lvs__net_count_differences"] = net_differences
-    metrics["lvs__property_fails"] = property_fails
-    metrics["lvs__total__errors"] = total_errors
-    metrics["lvs__unmatched_devices"] = device_fails
-    metrics["lvs__unmatched_nets"] = net_fails
-    metrics["lvs__unmatched_pins"] = pin_fails
+    metrics["design__lvs_device_difference__count"] = device_differences
+    metrics["design__lvs_net_differences__count"] = net_differences
+    metrics["design__lvs_property_fails__count"] = property_fails
+    metrics["design__lvs_errors__count"] = total_errors
+    metrics["design__lvs_unmatched_devices__count"] = device_fails
+    metrics["design__lvs_unmatched_nets__count"] = net_fails
+    metrics["design__lvs_unmatched_pins__count"] = pin_fails
 
     return metrics
 
 
 class NetgenStep(TclStep):
     inputs = []
     outputs = []
@@ -104,14 +104,24 @@
 
     def get_command(self) -> List[str]:
         return ["netgen", "-batch", "source"]
 
 
 @Step.factory.register()
 class LVS(NetgenStep):
+    """
+    Performs `Layout vs. Schematic <https://en.wikipedia.org/wiki/Layout_Versus_Schematic>`_ checks on the extracted SPICE netlist versus.
+    a verilog netlist with power connections.
+
+    This verifies the following:
+    * There are no unexpected shorts in the final layout.
+    * There are no unexpected opens in the final layout.
+    * All signals are connected correctly.
+    """
+
     id = "Netgen.LVS"
     inputs = [DesignFormat.SPICE, DesignFormat.POWERED_NETLIST]
     flow_control_variable = "RUN_LVS"
 
     config_vars = [
         Variable(
             "RUN_LVS",
@@ -123,26 +133,24 @@
 
     def get_command(self) -> List[str]:
         return super().get_command() + [self.get_script_path()]
 
     def get_script_path(self):
         return os.path.join(self.step_dir, "lvs_script.lvs")
 
-    def run(self, **kwargs) -> State:
-        assert isinstance(self.state_in, State)
-
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         if self.config["NETGEN_SETUP"] is None:
             info(f"Skipping {self.name}: Netgen is not supported for this PDK.")
-            return Step.run(self, **kwargs)
+            return Step.run(self, state_in, **kwargs)
 
         spice_glob = os.path.join(
-            self.config["PDK_ROOT"],
-            self.config["PDK"],
+            self.config[Keys.pdk_root],
+            self.config[Keys.pdk],
             "libs.ref",
-            self.config["STD_CELL_LIBRARY"],
+            self.config[Keys.scl],
             "spice",
             "*.spice",
         )
         spice_files: List[str] = glob.glob(spice_glob)
 
         if pdk_spice_files := self.config.get("SPICE_MODELS"):
             spice_files = pdk_spice_files.copy()
@@ -160,18 +168,18 @@
                 )
                 print(
                     f"readnet spice {lib} 1",
                     file=f,
                 )
 
             print(
-                f"lvs {{ {self.state_in[DesignFormat.SPICE]} {design_name} }} {{ {self.state_in[DesignFormat.POWERED_NETLIST]} {design_name} }} {self.config['NETGEN_SETUP']} {os.path.abspath(self.step_dir)}/lvs.rpt -json",
+                f"lvs {{ {state_in[DesignFormat.SPICE]} {design_name} }} {{ {state_in[DesignFormat.POWERED_NETLIST]} {design_name} }} {self.config['NETGEN_SETUP']} {os.path.abspath(self.step_dir)}/lvs.rpt -json",
                 file=f,
             )
 
-        state_out = super().run(**kwargs)
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
         stats_file = os.path.join(self.step_dir, "lvs.json")
         stats_string = open(stats_file).read()
         lvs_metrics = get_metrics(json.loads(stats_string))
-        state_out.metrics.update(lvs_metrics)
+        metrics_updates.update(lvs_metrics)
 
-        return state_out
+        return (views_updates, metrics_updates)
```

### Comparing `openlane-2.0.0a9/openlane/steps/odb.py` & `openlane-2.0.0b1/openlane/steps/yosys.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,340 +9,296 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
-import sys
+import io
 import json
-from decimal import Decimal
 from abc import abstractmethod
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
+from .tclstep import TclStep
+from .step import ViewsUpdate, MetricsUpdate, Step
 
-from .step import Step
-from ..state import State
-from ..state import DesignFormat
-from .common_variables import io_layer_variables
+from ..config import Variable
+from ..logging import debug, verbose
+from ..state import State, DesignFormat
+from ..common import Path, get_script_dir, StringEnum
+
+starts_with_whitespace = re.compile(r"^\s+.+$")
+
+
+def parse_yosys_check(
+    report: io.TextIOBase,
+    tristate_okay: bool = False,
+) -> int:
+    verbose("Parsing synthesis checks…")
+    errors_encountered: int = 0
+    current_warning = None
+
+    for line in report:
+        if line.startswith("Warning:") or line.startswith("Found and reported"):
+            if current_warning is not None:
+                if tristate_okay and "tribuf" in current_warning:
+                    debug("Ignoring tristate-related error:")
+                    debug(current_warning)
+                else:
+                    debug("Encountered check error:")
+                    debug(current_warning)
+                    errors_encountered += 1
+            current_warning = line
+        elif (
+            starts_with_whitespace.match(line) is not None
+            and current_warning is not None
+        ):
+            current_warning += line
+        else:
+            pass
+    return errors_encountered
 
-from ..config import Path, Variable, StringEnum
-from ..common import get_openlane_root, get_script_dir
-from ..logging import warn
 
-inf_rx = re.compile(r"\b(-?)inf\b")
+class YosysStep(TclStep):
+    reproducibles_allowed = False
 
-
-class OdbpyStep(Step):
-    inputs = [DesignFormat.ODB]
-    outputs = [DesignFormat.ODB, DesignFormat.DEF]
-
-    def run(
-        self,
-        **kwargs,
-    ) -> State:
-        """
-        TODO
-        """
-
-        state_out = super().run(**kwargs)
-        kwargs, env = self.extract_env(kwargs)
-
-        out_paths = {}
-
-        command = self.get_command()
-        for output in [DesignFormat.ODB, DesignFormat.DEF]:
-            id, ext, _ = output.value
-            filename = f"{self.config['DESIGN_NAME']}.{ext}"
-            file_path = os.path.join(self.step_dir, filename)
-            command.append(f"--output-{id}")
-            command.append(file_path)
-            out_paths[output] = Path(file_path)
-
-        command += [
-            str(state_out[DesignFormat.ODB]),
-        ]
-
-        env["OPENLANE_ROOT"] = get_openlane_root()
-        env["ODB_PYTHONPATH"] = ":".join(sys.path)
-
-        self.run_subprocess(
-            command,
-            env=env,
-            **kwargs,
-        )
-
-        metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
-        if os.path.exists(metrics_path):
-            metrics_str = open(metrics_path).read()
-            metrics_str = inf_rx.sub(lambda m: f"{m[1] or ''}\"Infinity\"", metrics_str)
-            new_metrics = json.loads(metrics_str)
-            state_out.metrics.update(new_metrics)
-
-        for output in [DesignFormat.ODB, DesignFormat.DEF]:
-            state_out[output] = out_paths[output]
-
-        return state_out
+    config_vars = [
+        Variable(
+            "VERILOG_FILES",
+            List[Path],
+            "The paths of the design's Verilog files.",
+        ),
+        Variable(
+            "SYNTH_DEFINES",
+            Optional[List[str]],
+            "Synthesis defines",
+        ),
+        Variable(
+            "VERILOG_INCLUDE_DIRS",
+            Optional[List[str]],
+            "Specifies the Verilog `include` directories.",
+        ),
+        Variable(
+            "SYNTH_READ_BLACKBOX_LIB",
+            bool,
+            "Additionally read the liberty file(s) as a blackbox. This will allow RTL designs to incorporate explicitly declared standard cells that will not be tech-mapped or reinterpreted.",
+            default=False,
+        ),
+    ]
 
     def get_command(self) -> List[str]:
-        metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
-        lefs = ["--input-lef", self.config["TECH_LEF"]]
-        for lef in self.config["CELL_LEFS"]:
-            lefs.append("--input-lef")
-            lefs.append(lef)
-        if extra_lefs := self.config["EXTRA_LEFS"]:
-            for lef in extra_lefs:
-                lefs.append("--input-lef")
-                lefs.append(lef)
-        return (
-            [
-                "openroad",
-                "-exit",
-                "-metrics",
-                metrics_path,
-                "-python",
-                self.get_script_path(),
-            ]
-            + self.get_subcommand()
-            + lefs
-        )
+        script_path = self.get_script_path()
+        return ["yosys", "-c", script_path]
 
     @abstractmethod
-    def get_script_path(self):
+    def get_script_path(self) -> str:
         pass
 
-    def get_subcommand(self) -> List[str]:
-        return []
-
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        kwargs, env = self.extract_env(kwargs)
 
-@Step.factory.register()
-class ApplyDEFTemplate(OdbpyStep):
-    id = "Odb.ApplyDEFTemplate"
-    name = "Apply DEF Template"
+        lib_list = self.toolbox.filter_views(self.config, self.config["LIB"])
+        lib_synth = self.toolbox.remove_cells_from_lib(
+            frozenset(lib_list),
+            excluded_cells=frozenset(
+                [
+                    self.config["SYNTH_EXCLUSION_CELL_LIST"],
+                    self.config["PNR_EXCLUSION_CELL_LIST"],
+                ]
+            ),
+            as_cell_lists=True,
+        )
 
-    flow_control_variable = "FP_DEF_TEMPLATE"
-    flow_control_msg = "No DEF template provided, skipping…"
+        env["SYNTH_LIBS"] = " ".join(lib_synth)
 
-    config_vars = [
-        Variable(
-            "FP_DEF_TEMPLATE",
-            Optional[Path],
-            "Points to the DEF file to be used as a template when running `apply_def_template`. This will be used to exctract pin names, locations, shapes -excluding power and ground pins- as well as the die area and replicate all this information in the `CURRENT_DEF`.",
-        ),
-    ]
+        macro_libs = self.toolbox.get_macro_views(
+            self.config,
+            DesignFormat.LIB,
+        )
+        if len(macro_libs) != 0:
+            env["MACRO_LIBS"] = " ".join([str(lib) for lib in macro_libs])
 
-    def get_script_path(self):
-        return os.path.join(
-            get_script_dir(),
-            "odbpy",
-            "apply_def_template.py",
+        macro_nls = self.toolbox.get_macro_views(
+            self.config,
+            DesignFormat.NETLIST,
+            unless_exist=DesignFormat.LIB,
         )
+        if len(macro_nls) != 0:
+            env["MACRO_NLS"] = " ".join([str(nl) for nl in macro_nls])
 
-    def get_command(self) -> List[str]:
-        return super().get_command() + [
-            "--def-template",
-            self.config["FP_DEF_TEMPLATE"],
-        ]
+        return super().run(state_in, env=env, **kwargs)
 
 
 @Step.factory.register()
-class ManualMacroPlacement(OdbpyStep):
-    id = "Odb.ManualMacro"
-    name = "Manual Macro Placement"
+class JsonHeader(YosysStep):
+    id = "Yosys.JsonHeader"
+    inputs = []
+    outputs = [DesignFormat.JSON_HEADER]
 
-    flow_control_variable = "MACRO_PLACEMENT_CFG"
-    flow_control_msg = "No macros configured, skipping…"
+    def get_script_path(self):
+        return os.path.join(get_script_dir(), "yosys", "json_header.tcl")
 
-    config_vars = [
+    config_vars = YosysStep.config_vars + [
         Variable(
-            "MACRO_PLACEMENT_CFG",
-            Optional[Path],
-            "Specifies the path a file specifying how OpenLane should place certain macros.",
+            "SYNTH_POWER_DEFINE",
+            Optional[str],
+            "Specifies the name of the define used to guard power and ground connections",
+            deprecated_names=["SYNTH_USE_PG_PINS_DEFINES"],
         ),
     ]
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "manual_macro_place.py")
-
-    def get_command(self) -> List[str]:
-        return super().get_command() + [
-            "--config",
-            self.config["MACRO_PLACEMENT_CFG"],
-            "--fixed",
-        ]
-
 
 @Step.factory.register()
-class ReportWireLength(OdbpyStep):
-    id = "Odb.ReportWireLength"
-    name = "Report Wire Length"
+class Synthesis(YosysStep):
+    """
+    Performs synthesis and technology mapping using Yosys and ABC, emitting a
+    netlist. Requires Yosys 0.26 or higher.
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "wire_lengths.py")
+    Some metrics will also be extracted and updated, namely:
 
-    def get_command(self) -> List[str]:
-        return super().get_command() + [
-            "--human-readable",
-            "--report-out",
-            os.path.join(self.step_dir, "wire_lengths.csv"),
-        ]
+    * ``design__instance__count``
+    * ``design__instance_unmapped__count``
 
+    If using Yosys 0.27 or higher:
 
-@Step.factory.register()
-class CustomIOPlacement(OdbpyStep):
-    id = "Odb.CustomIOPlacement"
-    name = "Custom I/O Placement"
-    long_name = "Custom I/O Pin Placement Script"
+    * ``design__instance__area`` is also updated.
+    """
 
-    flow_control_variable = "FP_PIN_ORDER_CFG"
-    flow_control_msg = "No custom floorplan file configured, skipping…"
+    id = "Yosys.Synthesis"
+    inputs = []  # The input RTL is part of the configuration
+    outputs = [DesignFormat.NETLIST]
 
-    config_vars = io_layer_variables + [
+    config_vars = YosysStep.config_vars + [
         Variable(
-            "FP_PIN_ORDER_CFG",
-            Optional[Path],
-            "Points to the pin order configuration file to set the pins in specific directions (S, W, E, N). If not set, then the IO pins will be placed using OpenROAD's basic pin placer.",
+            "SYNTH_CHECKS_ALLOW_TRISTATE",
+            bool,
+            "Ignore multiple-driver warnings if they are connected to tri-state buffers on a best-effort basis.",
+            default=True,
         ),
         Variable(
-            "QUIT_ON_UNMATCHED_IO",
+            "SYNTH_AUTONAME",
             bool,
-            "Exit on unmatched pins in a provided `FP_PIN_ORDER_CFG` file.",
-            default=True,
-            deprecated_names=["FP_IO_UNMATCHED_ERROR"],
+            "Generates names for netlist instances. This results in instance names that can be extremely long, but are more human-readable.",
+            default=False,
         ),
-    ]
-
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "io_place.py")
-
-    def get_command(self) -> List[str]:
-        length = max(
-            self.config["FP_IO_VLENGTH"],
-            self.config["FP_IO_HLENGTH"],
-        )
-
-        return super().get_command() + [
-            "--config",
-            self.config["FP_PIN_ORDER_CFG"],
-            "--hor-layer",
-            self.config["FP_IO_HLAYER"],
-            "--ver-layer",
-            self.config["FP_IO_VLAYER"],
-            "--hor-width-mult",
-            str(self.config["FP_IO_VTHICKNESS_MULT"]),
-            "--ver-width-mult",
-            str(self.config["FP_IO_HTHICKNESS_MULT"]),
-            "--hor-extension",
-            str(self.config["FP_IO_HEXTEND"]),
-            "--ver-extension",
-            str(self.config["FP_IO_VEXTEND"]),
-            "--length",
-            str(length),
-            (
-                "--unmatched-error"
-                if self.config["QUIT_ON_UNMATCHED_IO"]
-                else "--ignore-unmatched"
+        Variable(
+            "SYNTH_STRATEGY",
+            StringEnum(
+                "SYNTH_STRATEGY",
+                [
+                    "AREA 0",
+                    "AREA 1",
+                    "AREA 2",
+                    "AREA 3",
+                    "AREA 4",
+                    "DELAY 0",
+                    "DELAY 1",
+                    "DELAY 2",
+                    "DELAY 3",
+                    "DELAY 4",
+                ],
             ),
-        ]
-
-
-@Step.factory.register()
-class DiodesOnPorts(OdbpyStep):
-    id = "Odb.DiodesOnPorts"
-    name = "Diodes on Ports"
-    long_name = "Diode on Port Insertion Script"
-
-    config_vars = [
+            "Strategies for abc logic synthesis and technology mapping. AREA strategies usually result in a more compact design, while DELAY strategies usually result in a design that runs at a higher frequency. Please note that there is no way to know which strategy is the best before trying them.",
+            default="AREA 0",
+        ),
         Variable(
-            "DIODE_ON_PORTS",
-            StringEnum("DIODE_ON_PORTS", ["none", "in", "out", "both"]),
-            "Always insert diodes on ports with the specified polarities.",
-            default="none",
+            "SYNTH_ABC_BUFFERING",
+            bool,
+            "Enables `abc` cell buffering.",
+            default=True,
+            deprecated_names=["SYNTH_BUFFERING"],
         ),
-    ]
-
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "diodes.py")
-
-    def get_subcommand(self) -> List[str]:
-        return ["place"]
-
-    def get_command(self) -> List[str]:
-        cell, pin = self.config["DIODE_CELL"].split("/")
-
-        return super().get_command() + [
-            "--threshold",
-            "Infinity",
-            "--diode-cell",
-            cell,
-            "--diode-pin",
-            pin,
-            "--port-protect",
-            self.config["DIODE_ON_PORTS"].value,
-        ]
-
-    def run(self, **kwargs) -> State:
-        if self.config["DIODE_ON_PORTS"].value == "none":
-            warn("'DIODE_ON_PORTS' is set to 'none': skipping…")
-            return Step.run(self, **kwargs)
-
-        if self.config["GPL_CELL_PADDING"] == 0:
-            warn(
-                "'GPL_CELL_PADDING' is set to 0. This step may cause overlap failures."
-            )
-
-        return super().run(**kwargs)
-
-
-@Step.factory.register()
-class HeuristicDiodeInsertion(OdbpyStep):
-    id = "Odb.HeuristicDiodeInsertion"
-    name = "Heuristic Diode Insertion"
-    long_name = "Heuristic Diode Insertion Script"
-
-    flow_control_variable = "RUN_HEURISTIC_DIODE_INSERTION"
-    config_vars = [
         Variable(
-            "RUN_HEURISTIC_DIODE_INSERTION",
+            "SYNTH_DIRECT_WIRE_BUFFERING",
             bool,
-            "Enables/disables this step.",
-            default=False,  # For compatibility with OL1. Yep.
+            "Enables inserting buffer cells for directly connected wires.",
+            default=True,
+            deprecated_names=["SYNTH_BUFFER_DIRECT_WIRES"],
+        ),
+        Variable(
+            "SYNTH_SPLITNETS",
+            bool,
+            "Splits multi-bit nets into single-bit nets. Easier to trace but may not be supported by all tools.",
+            default=True,
+        ),
+        Variable(
+            "SYNTH_SIZING",
+            bool,
+            "Enables `abc` cell sizing (instead of buffering).",
+            default=False,
+        ),
+        Variable(
+            "SYNTH_NO_FLAT",
+            bool,
+            "A flag that disables flattening the hierarchy during synthesis, only flattening it after synthesis, mapping and optimizations.",
+            default=False,
+        ),
+        Variable(
+            "SYNTH_SHARE_RESOURCES",
+            bool,
+            "A flag that enables yosys to reduce the number of cells by determining shareable resources and merging them.",
+            default=True,
         ),
         Variable(
-            "HEURISTIC_ANTENNA_THRESHOLD",
-            Optional[Decimal],
-            "A manhattan distance above which a diode is recommended to be inserted by a heuristic inserter. If not specified, the heuristic inserter will typically use a default value.",
-            units="µm",
+            "SYNTH_ADDER_TYPE",
+            StringEnum("SYNTH_ADDER_TYPE", ["YOSYS", "FA", "RCA", "CSA"]),
+            "Adder type to which the $add and $sub operators are mapped to.  Possible values are `YOSYS/FA/RCA/CSA`; where `YOSYS` refers to using Yosys internal adder definition, `FA` refers to full-adder structure, `RCA` refers to ripple carry adder structure, and `CSA` refers to carry select adder.",
+            default="YOSYS",
+        ),
+        Variable(
+            "SYNTH_EXTRA_MAPPING_FILE",
+            Optional[Path],
+            "Points to an extra techmap file for yosys that runs right after yosys `synth` before generic techmap.",
+        ),
+        Variable(
+            "SYNTH_PARAMETERS",
+            Optional[List[str]],
+            "Key-value pairs to be `chparam`ed in Yosys, in the format `key1=value1`.",
+        ),
+        Variable(
+            "SYNTH_ELABORATE_ONLY",
+            bool,
+            '"Elaborate" the design only without attempting any logic mapping. Useful when dealing with structural Verilog netlists.',
+            default=False,
+        ),
+        Variable(
+            "SYNTH_ELABORATE_FLATTEN",
+            bool,
+            "If `SYNTH_ELABORATE_ONLY` is specified, this variable controls whether or not the top level should be flattened.",
+            default=True,
+            deprecated_names=["SYNTH_FLAT_TOP"],
         ),
     ]
 
     def get_script_path(self):
-        return os.path.join(get_script_dir(), "odbpy", "diodes.py")
+        return os.path.join(get_script_dir(), "yosys", "synthesize.tcl")
 
-    def get_subcommand(self) -> List[str]:
-        return ["place"]
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metric_updates = super().run(state_in, **kwargs)
 
-    def get_command(self) -> List[str]:
-        cell, pin = self.config["DIODE_CELL"].split("/")
+        stats_file = os.path.join(self.step_dir, "reports", "stat.json")
+        stats_str = open(stats_file).read()
+        stats = json.loads(stats_str)
+
+        metric_updates = {}
+        metric_updates["design__instance__count"] = stats["design"]["num_cells"]
+        if chip_area := stats["design"].get("area"):  # needs nonzero area
+            metric_updates["design__instance__area"] = chip_area
+
+        cells = stats["design"]["num_cells_by_type"]
+        unmapped_keyword = "$"
+        unmapped_cells = [
+            cells[y] for y in cells.keys() if y.startswith(unmapped_keyword)
+        ]
+        metric_updates["design__instance_unmapped__count"] = sum(unmapped_cells)
 
-        threshold_opts = []
-        if threshold := self.config["HEURISTIC_ANTENNA_THRESHOLD"]:
-            threshold_opts = ["--threshold", threshold]
-
-        return (
-            super().get_command()
-            + [
-                "--diode-cell",
-                cell,
-                "--diode-pin",
-                pin,
-            ]
-            + threshold_opts
+        check_error_count_file = os.path.join(
+            self.step_dir, "reports", "pre_synth_chk.rpt"
         )
-
-    def run(self, **kwargs) -> State:
-        if self.config["GPL_CELL_PADDING"] == 0:
-            warn(
-                "'GPL_CELL_PADDING' is set to 0. This step may cause overlap failures."
+        metric_updates["synthesis__check_error__count"] = 0
+        if os.path.exists(check_error_count_file):
+            metric_updates["synthesis__check_error__count"] = parse_yosys_check(
+                open(check_error_count_file),
+                self.config["SYNTH_CHECKS_ALLOW_TRISTATE"],
             )
 
-        return super().run(**kwargs)
+        return views_updates, metric_updates
```

### Comparing `openlane-2.0.0a9/openlane/steps/openroad.py` & `openlane-2.0.0b1/openlane/steps/openroad.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,38 +7,47 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import io
 import os
 import re
 import json
+import shlex
+import tempfile
+import subprocess
+from math import inf
+from glob import glob
 from decimal import Decimal
 from base64 import b64encode
 from abc import abstractmethod
-from typing import List, Dict, Tuple, Optional
+from concurrent.futures import Future
+from typing import Any, Callable, Iterable, List, Dict, Tuple, Optional, Union
 
-from .step import Step
-from ..state import State
+import rich
+import rich.table
+
+from .step import ViewsUpdate, MetricsUpdate, Step, StepException
 from .tclstep import TclStep
-from ..state import DesignFormat
 from .common_variables import (
     io_layer_variables,
     pdn_variables,
     rsz_variables,
     dpl_variables,
+    grt_variables,
     routing_layer_variables,
-    constraint_variables,
 )
 
-from ..logging import info, warn
-from ..common import get_script_dir
-from ..config import Variable, Path, StringEnum
+from ..config import Variable
+from ..state import State, DesignFormat
+from ..logging import debug, err, info, warn, console
+from ..common import Path, get_script_dir, StringEnum, get_tpe, mkdirp, TclUtils
 
 EXAMPLE_INPUT = """
 li1 X 0.23 0.46
 li1 Y 0.17 0.34
 met1 X 0.17 0.34
 met1 Y 0.17 0.34
 met2 X 0.23 0.46
@@ -47,14 +56,32 @@
 met3 Y 0.34 0.68
 met4 X 0.46 0.92
 met4 Y 0.46 0.92
 met5 X 1.70 3.40
 met5 Y 1.70 3.40
 """
 
+timing_metric_aggregation: Dict[str, Tuple[Any, Callable[[Iterable], Any]]] = {
+    "timing__hold_vio__count": (0, lambda x: sum(x)),
+    "timing__hold_r2r_vio__count": (0, lambda x: sum(x)),
+    "timing__setup_vio__count": (0, lambda x: sum(x)),
+    "timing__setup_r2r_vio__count": (0, lambda x: sum(x)),
+    "clock__max_slew_violation__count": (0, lambda x: sum(x)),
+    "design__max_fanout_violation__count": (0, lambda x: sum(x)),
+    "design__max_cap_violation__count": (0, lambda x: sum(x)),
+    "clock__skew__worst_hold": (inf, min),
+    "clock__skew__worst_setup": (inf, min),
+    "timing__hold__ws": (inf, min),
+    "timing__setup__ws": (inf, min),
+    "timing__hold__wns": (inf, min),
+    "timing__setup__wns": (inf, min),
+    "timing__hold__tns": (0, lambda x: sum(x)),
+    "timing__setup__tns": (0, lambda x: sum(x)),
+}
+
 
 def old_to_new_tracks(old_tracks: str) -> str:
     """
     >>> old_to_new_tracks(EXAMPLE_INPUT)
     'make_tracks li1 -x_offset 0.23 -x_pitch 0.46 -y_offset 0.17 -y_pitch 0.34\\nmake_tracks met1 -x_offset 0.17 -x_pitch 0.34 -y_offset 0.17 -y_pitch 0.34\\nmake_tracks met2 -x_offset 0.23 -x_pitch 0.46 -y_offset 0.23 -y_pitch 0.46\\nmake_tracks met3 -x_offset 0.34 -x_pitch 0.68 -y_offset 0.34 -y_pitch 0.68\\nmake_tracks met4 -x_offset 0.46 -x_pitch 0.92 -y_offset 0.46 -y_pitch 0.92\\nmake_tracks met5 -x_offset 1.70 -x_pitch 3.40 -y_offset 1.70 -y_pitch 3.40\\n'
     """
     layers: Dict[str, Dict[str, Tuple[str, str]]] = {}
@@ -71,34 +98,24 @@
         x_offset, x_pitch = data["X"]
         y_offset, y_pitch = data["Y"]
         final_str += f"make_tracks {layer} -x_offset {x_offset} -x_pitch {x_pitch} -y_offset {y_offset} -y_pitch {y_pitch}\n"
 
     return final_str
 
 
-inf_rx = re.compile(r"\b(-?)inf\b")
-
-
 class OpenROADStep(TclStep):
-    inputs = [DesignFormat.ODB]
+    inputs = [DesignFormat.ODB, DesignFormat.SDC]
     outputs = [
         DesignFormat.ODB,
         DesignFormat.DEF,
-        DesignFormat.SDC,
         DesignFormat.NETLIST,
         DesignFormat.POWERED_NETLIST,
     ]
 
-    config_vars = constraint_variables + [
-        Variable(
-            "STA_WRITE_LIB",
-            bool,
-            "Controls whether a timing model is written using OpenROAD OpenSTA after static timing analysis. This is an option as it in its current state, the timing model generation (and the model itself) can be quite buggy.",
-            default=False,
-        ),
+    config_vars = [
         Variable(
             "PDN_CONNECT_MACROS_TO_GRID",
             bool,
             "Enables the connection of macros to the top level power grid.",
             default=True,
             deprecated_names=["FP_PDN_ENABLE_MACROS_GRID"],
         ),
@@ -117,93 +134,380 @@
         ),
     ]
 
     @abstractmethod
     def get_script_path(self):
         pass
 
-    def run(
-        self,
-        **kwargs,
-    ) -> State:
+    def prepare_env(self, env: dict, state: State) -> dict:
+        env = super().prepare_env(env, state)
+
+        lib_list = self.toolbox.filter_views(self.config, self.config["LIB"])
+        lib_list += self.toolbox.get_macro_views(self.config, DesignFormat.LIB)
+
+        lib_pnr = self.toolbox.remove_cells_from_lib(
+            frozenset(lib_list),
+            frozenset([self.config["PNR_EXCLUSION_CELL_LIST"]]),
+            as_cell_lists=True,
+        )
+
+        env["PNR_LIBS"] = " ".join(lib_pnr)
+        env["MACRO_LIBS"] = " ".join(
+            [
+                str(lib)
+                for lib in self.toolbox.get_macro_views(self.config, DesignFormat.LIB)
+            ]
+        )
+        env["PNR_EXCLUDED_CELLS"] = TclUtils.join(
+            [
+                cell.strip()
+                for cell in open(self.config["PNR_EXCLUSION_CELL_LIST"]).read().split()
+                if cell.strip() != ""
+            ]
+        )
+
+        return env
+
+    def run(self, state_in, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         """
         The `run()` override for the OpenROADStep class handles two things:
 
-        1. Before the `super()` call: It creates a version of the liberty file
+        1. Before the `super()` call: It creates a version of the lib file
         minus cells that are known bad (i.e. those that fail DRC) and pass it on
-        in the environment variable `LIB_PNR`.
+        in the environment variable `PNR_LIBS`.
 
         2. After the `super()` call: Processes the `or_metrics_out.json` file and
         updates the State's `metrics` property with any new metrics in that object.
         """
         kwargs, env = self.extract_env(kwargs)
 
-        lib_pnr = self.toolbox.remove_cells_from_lib(
-            frozenset(self.config["LIB"]),
-            frozenset([self.config["BAD_CELL_LIST"]]),
-            as_cell_lists=True,
-        )
-
-        env["LIB_PNR"] = lib_pnr
-
-        state_out = super().run(env=env, **kwargs)
+        views_updates, metrics_updates = super().run(state_in, env=env, **kwargs)
 
         metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
         if os.path.exists(metrics_path):
-            metrics_str = open(metrics_path).read()
-            metrics_str = inf_rx.sub(lambda m: f"{m[1] or ''}\"Infinity\"", metrics_str)
-            new_metrics = json.loads(metrics_str)
-            state_out.metrics.update(new_metrics)
-        return state_out
+            or_metrics_out = json.loads(open(metrics_path).read())
+            for key, value in or_metrics_out.items():
+                if value == "Infinity":
+                    or_metrics_out[key] = inf
+                elif value == "-Infinity":
+                    or_metrics_out[key] = -inf
+            metrics_updates.update(or_metrics_out)
+
+        metric_updates_with_aggregates = self.toolbox.aggregate_metrics(
+            metrics_updates,
+            timing_metric_aggregation,
+        )
+
+        return views_updates, metric_updates_with_aggregates
 
     def get_command(self) -> List[str]:
         metrics_path = os.path.join(self.step_dir, "or_metrics_out.json")
-        return ["openroad", "-exit", "-metrics", metrics_path, self.get_script_path()]
+        return [
+            "openroad",
+            "-exit",
+            "-no_splash",
+            "-metrics",
+            metrics_path,
+            self.get_script_path(),
+        ]
 
     def layout_preview(self) -> Optional[str]:
         if self.state_out is None:
             return None
 
-        assert isinstance(self.state_in, State)
-
-        if self.state_out.get("def") == self.state_in.get("def"):
+        state_in = self.state_in.result()
+        if self.state_out.get("def") == state_in.get("def"):
             return None
 
         if image := self.toolbox.render_png(self.config, str(self.state_out["def"])):
             image_encoded = b64encode(image).decode("utf8")
             return f'<img src="data:image/png;base64,{image_encoded}" />'
 
         return None
 
 
+class STAStep(OpenROADStep):
+    """
+    Abstract class for an STA step
+    """
+
+    def layout_preview(self) -> Optional[str]:
+        return None
+
+    def get_script_path(self):
+        return os.path.join(get_script_dir(), "openroad", "sta", "corner.tcl")
+
+
 @Step.factory.register()
-class NetlistSTA(OpenROADStep):
-    id = "OpenROAD.NetlistSTA"
-    name = "Netlist STA"
-    long_name = "Netlist Static Timing Analysis"
-    inputs = [DesignFormat.NETLIST]
+class STAMidPNR(STAStep):
+    """
+    Performs `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
+    using OpenROAD on an OpenROAD database, mid-PnR.
+    """
+
+    id = "OpenROAD.STAMidPNR"
+    name = "STA (Mid-PnR)"
+    long_name = "Static Timing Analysis (Mid-PnR)"
+
+    inputs = [DesignFormat.ODB, DesignFormat.SDC]
     outputs = []
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "openroad", "sta.tcl")
 
-    def run(self, **kwargs) -> State:
+@Step.factory.register()
+class STAPrePNR(STAStep):
+    """
+    Performs hierarchical `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
+    using OpenSTA on the pre-PnR Verilog netlist, with all available timing information
+    for standard cells and macros for the default timing corner as specified in
+    the ``DEFAULT_CORNER`` variable.
+
+    If timing information is not available for macros, the macro in question
+    will be black-boxed.
+    """
+
+    inputs = [DesignFormat.NETLIST, DesignFormat.SDC]
+    outputs = [DesignFormat.SDF, DesignFormat.SDC]
+
+    id = "OpenROAD.STAPrePNR"
+    name = "STA (Pre-PnR)"
+    long_name = "Static Timing Analysis"
+
+    config_vars = STAStep.config_vars + [
+        Variable(
+            "STA_MACRO_PRIORITIZE_NL",
+            bool,
+            "Prioritize the use of Netlists + SPEF files over LIB files if available for Macros. Useful if extraction was done using OpenROAD, where SPEF files are far more accurate.",
+            default=True,
+        ),
+    ]
+
+    def get_command(self) -> List[str]:
+        return ["sta", "-no_splash", "-exit", self.get_script_path()]
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
-        env["RUN_STANDALONE"] = "1"
-        env["STA_PRE_CTS"] = "1"
-        return super().run(env=env, **kwargs)
+
+        timing_corner, timing_file_list = self.toolbox.get_timing_files(
+            self.config,
+            prioritize_nl=self.config["STA_MACRO_PRIORITIZE_NL"],
+        )
+
+        env["OPENSTA"] = "1"
+        env["CURRENT_CORNER_NAME"] = timing_corner
+        env["CURRENT_CORNER_TIMING_VIEWS"] = " ".join(timing_file_list)
+        env["SDF_SAVE_DIR"] = self.step_dir
+
+        views_updates, metrics_updates = super().run(state_in, env=env, **kwargs)
+
+        sdf_dict = state_in[DesignFormat.SDF] or {}
+        if not isinstance(sdf_dict, dict):
+            raise StepException(
+                "Malformed input state: value for LIB is not a dictionary."
+            )
+
+        sdfs = glob(os.path.join(self.step_dir, "*.sdf"))
+        for sdf in sdfs:
+            _, corner = os.path.basename(sdf)[:-4].split("__")
+            sdf_dict[corner] = Path(sdf)
+
+        views_updates[DesignFormat.SDF] = sdf_dict
+
+        return views_updates, metrics_updates
+
+
+@Step.factory.register()
+class STAPostPNR(STAPrePNR):
+    """
+    Performs multi-corner `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
+    using OpenSTA on the post-PnR Verilog netlist, with extracted parasitics for
+    both the top-level module and any associated macros.
+    """
+
+    id = "OpenROAD.STAPostPNR"
+    name = "STA (Post-PnR)"
+    long_name = "Static Timing Analysis (Post-PnR)"
+    flow_control_variable = "RUN_MCSTA"
+
+    inputs = STAPrePNR.inputs + [DesignFormat.SPEF]
+    outputs = STAPrePNR.outputs + [DesignFormat.LIB]
+
+    config_vars = STAPrePNR.config_vars + [
+        Variable(
+            "RUN_MCSTA",
+            bool,
+            "Enables/disables this step.",
+            default=True,
+            deprecated_names=["RUN_SPEF_STA"],
+        ),
+    ]
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        kwargs, env = self.extract_env(kwargs)
+
+        env = self.prepare_env(env, state_in)
+
+        env["OPENSTA"] = "1"
+
+        def run_corner(corner: str):
+            nonlocal env
+
+            current_env = env.copy()
+
+            corner_dir = os.path.join(self.step_dir, corner)
+            mkdirp(corner_dir)
+
+            current_env["CURRENT_CORNER_NAME"] = corner
+            current_env["LIB_SAVE_DIR"] = corner_dir
+            current_env["SDF_SAVE_DIR"] = corner_dir
+
+            if not isinstance(state_in[DesignFormat.SPEF], dict):
+                raise StepException(
+                    "Malformed input state: value for SPEF is not a dictionary."
+                )
+
+            input_spef_dict = state_in[DesignFormat.SPEF]
+            assert input_spef_dict is not None  # Checked by start
+            if not isinstance(input_spef_dict, dict):
+                raise StepException(
+                    "Malformed input state: value for 'spef' is not a dictionary"
+                )
+
+            spefs = self.toolbox.filter_views(self.config, input_spef_dict, corner)
+            if len(spefs) < 1:
+                raise StepException(
+                    f"No SPEF file compatible with corner '{corner}' found."
+                )
+            elif len(spefs) > 1:
+                warn(
+                    f"Multiple SPEF files compatible with corner '{corner}' found. The first one encountered will be used."
+                )
+            spef = spefs[0]
+            current_env["CURRENT_SPEF_BY_CORNER"] = f"{corner} {spef}"
+
+            _, timing_file_list = self.toolbox.get_timing_files(
+                self.config,
+                corner,
+                prioritize_nl=self.config["STA_MACRO_PRIORITIZE_NL"],
+            )
+            current_env["CURRENT_CORNER_TIMING_VIEWS"] = " ".join(timing_file_list)
+
+            log_path = os.path.join(corner_dir, "sta.log")
+
+            try:
+                generated_metrics = self.run_subprocess(
+                    self.get_command(),
+                    log_to=log_path,
+                    env=current_env,
+                    silent=True,
+                    report_dir=corner_dir,
+                )
+                info(f"Finished STA for the {corner} timing corner.")
+            except subprocess.CalledProcessError as e:
+                err(f"Failed STA for the {corner} timing corner:")
+                raise e
+
+            return generated_metrics
+
+        futures: Dict[str, Future[MetricsUpdate]] = {}
+        for corner in self.config["STA_CORNERS"]:
+            futures[corner] = get_tpe().submit(
+                run_corner,
+                corner,
+            )
+
+        metrics_updates: MetricsUpdate = {}
+        for corner, updates_future in futures.items():
+            metrics_updates.update(updates_future.result())
+
+        metric_updates_with_aggregates = self.toolbox.aggregate_metrics(
+            metrics_updates, timing_metric_aggregation
+        )
+
+        def format_count(count: Optional[Union[int, float, Decimal]]) -> str:
+            if count is None:
+                return "[gray]?"
+            count = int(count)
+            if count == 0:
+                return f"[green]{count}"
+            else:
+                return f"[red]{count}"
+
+        table = rich.table.Table()
+        table.add_column("Corner/Group")
+        table.add_column("Hold Violations")
+        table.add_column("of which reg-to-reg")
+        table.add_column("Setup Violations")
+        table.add_column("of which reg-to-reg")
+        table.add_column("Max Cap Violations")
+        table.add_column("Max Slew Violations")
+        for corner in ["Overall"] + self.config["STA_CORNERS"]:
+            modifier = ""
+            if corner != "Overall":
+                modifier = f"__corner:{corner}"
+            row = [corner]
+            for metric in [
+                "timing__hold_vio__count",
+                "timing__hold_r2r_vio__count",
+                "timing__setup_vio__count",
+                "timing__setup_r2r_vio__count",
+                "design__max_cap_violation__count",
+                "clock__max_slew_violation__count",
+            ]:
+                row.append(
+                    format_count(
+                        metric_updates_with_aggregates.get(f"{metric}{modifier}")
+                    )
+                )
+            table.add_row(*row)
+
+        console.print(table)
+        with open(os.path.join(self.step_dir, "summary.rpt"), "w") as f:
+            rich.print(table, file=f)
+
+        views_updates: ViewsUpdate = {}
+        lib_dict = state_in[DesignFormat.LIB] or {}
+        if not isinstance(lib_dict, dict):
+            raise StepException(
+                "Malformed input state: value for LIB is not a dictionary."
+            )
+
+        libs = glob(os.path.join(self.step_dir, "**", "*.lib"), recursive=True)
+        for lib in libs:
+            _, corner = os.path.basename(lib)[:-4].split("__")
+            lib_dict[corner] = Path(lib)
+
+        views_updates[DesignFormat.LIB] = lib_dict
+
+        sdf_dict = state_in[DesignFormat.SDF] or {}
+        if not isinstance(sdf_dict, dict):
+            raise StepException(
+                "Malformed input state: value for LIB is not a dictionary."
+            )
+
+        sdfs = glob(os.path.join(self.step_dir, "**", "*.sdf"), recursive=True)
+        for sdf in sdfs:
+            _, corner = os.path.basename(sdf)[:-4].split("__")
+            sdf_dict[corner] = Path(sdf)
+
+        views_updates[DesignFormat.SDF] = sdf_dict
+
+        return views_updates, metric_updates_with_aggregates
 
 
 @Step.factory.register()
 class Floorplan(OpenROADStep):
+    """
+    Creates DEF and ODB files with the initial floorplan based on the Yosys netlist.
+    """
+
     id = "OpenROAD.Floorplan"
     name = "Floorplan Init"
     long_name = "Floorplan Initialization"
 
-    inputs = [DesignFormat.NETLIST]
+    inputs = [DesignFormat.NETLIST, DesignFormat.SDC]
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
             "FP_SIZING",
             StringEnum("FP_SIZING", ["relative", "absolute"]),
             "Whether to use relative sizing by making use of `FP_CORE_UTIL` or absolute one using `DIE_AREA`.",
             default="relative",
@@ -221,15 +525,15 @@
             default=50,
             units="%",
         ),
         Variable(
             "CORE_AREA",
             Optional[str],
             'Specific core area (i.e. die area minus margins) to be used in floorplanning when `FP_SIZING` is set to `absolute`. Specified as a 4-corner rectangle "x0 y0 x1 y1".',
-            units="μm",
+            units="µm",
         ),
         Variable(
             "BOTTOM_MARGIN_MULT",
             Decimal,
             "The core margin, in multiples of site heights, from the bottom boundary. If `FP_SIZING` is absolute and `CORE_AREA` is set, this variable has no effect.",
             default=4,
         ),
@@ -252,29 +556,36 @@
             default=12,
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "floorplan.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         path = self.config["FP_TRACKS_INFO"]
         tracks_info_str = open(path).read()
         tracks_commands = old_to_new_tracks(tracks_info_str)
         new_tracks_info = os.path.join(self.step_dir, "config.tracks")
         with open(new_tracks_info, "w") as f:
             f.write(tracks_commands)
 
         kwargs, env = self.extract_env(kwargs)
         env["TRACKS_INFO_FILE_PROCESSED"] = new_tracks_info
-        return super().run(env=env, **kwargs)
+        return super().run(state_in, env=env, **kwargs)
 
 
 @Step.factory.register()
 class IOPlacement(OpenROADStep):
+    """
+    Places I/O pins on a floor-planned ODB file using OpenROAD's built-in placer.
+
+    If ``FP_PIN_ORDER_CFG`` is not ``None``, this step is skipped (for
+    compatibility with OpenLane 1.)
+    """
+
     id = "OpenROAD.IOPlacement"
     name = "I/O Placement"
 
     config_vars = (
         OpenROADStep.config_vars
         + io_layer_variables
         + [
@@ -290,39 +601,44 @@
                 "The minimum distance between the IOs.",
                 default=3,
                 units="µm",
             ),
             Variable(
                 "FP_PIN_ORDER_CFG",
                 Optional[Path],
-                "Points to the pin order configuration file to set the pins in specific directions (S, W, E, N). If not set, then the IO pins will be placed using OpenROAD's basic pin placer.",
+                "Path to a custom pin configuration file.",
             ),
         ]
     )
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "ioplacer.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         if self.config["FP_PIN_ORDER_CFG"] is not None:
             # Skip - Step just checks and copies
-            return Step.run(self, **kwargs)
+            return {}, {}
 
-        return super().run(**kwargs)
+        return super().run(state_in, **kwargs)
 
 
 @Step.factory.register()
-class TapDecapInsertion(OpenROADStep):
-    id = "OpenROAD.TapDecapInsertion"
+class TapEndcapInsertion(OpenROADStep):
+    """
+    Places well TAP cells across a floorplan, as well as end-cap cells at the
+    edges of the floorplan.
+    """
+
+    id = "OpenROAD.TapEndcapInsertion"
     name = "Tap/Decap Insertion"
-    flow_control_variable = "RUN_TAP_DECAP_INSERTION"
+    flow_control_variable = "RUN_TAP_ENDCAP_INSERTION"
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
-            "RUN_TAP_DECAP_INSERTION",
+            "RUN_TAP_ENDCAP_INSERTION",
             bool,
             "Enables/disables this step.",
             default=True,
             deprecated_names=["TAP_DECAP_INSERTION"],
         ),
         Variable(
             "FP_TAP_HORIZONTAL_HALO",
@@ -331,37 +647,57 @@
             default=10,
             units="µm",
         ),
         Variable(
             "FP_TAP_VERTICAL_HALO",
             Decimal,
             "Specify the vertical halo size around macros during tap insertion.",
-            default="expr::$FP_TAP_HORIZONTAL_HALO",
+            default=10,
             units="µm",
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "tapcell.tcl")
 
 
 @Step.factory.register()
 class GeneratePDN(OpenROADStep):
+    """
+    Creates a power distribution network on a floorplanned ODB file.
+    """
+
     id = "OpenROAD.GeneratePDN"
     name = "Generate PDN"
     long_name = "Power Distribution Network Generation"
 
-    config_vars = OpenROADStep.config_vars + pdn_variables
+    config_vars = (
+        OpenROADStep.config_vars
+        + pdn_variables
+        + [
+            Variable(
+                "PDN_CFG",
+                Optional[Path],
+                "A custom PDN configuration file. If not provided, the default PDN config will be used.",
+            )
+        ]
+    )
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "pdn.tcl")
 
 
 @Step.factory.register()
 class GlobalPlacement(OpenROADStep):
+    """
+    Performs a somewhat nebulous initial placement for standard cells in a
+    floorplan. While the placement is not concrete, it is enough to start
+    accounting for issues such as fanout, transition time, et cetera.
+    """
+
     id = "OpenROAD.GlobalPlacement"
     name = "Global Placement"
 
     config_vars = (
         OpenROADStep.config_vars
         + routing_layer_variables
         + [
@@ -389,246 +725,172 @@
             Variable(
                 "PL_ROUTABILITY_DRIVEN",
                 bool,
                 "Specifies whether the placer should use routability driven placement.",
                 default=True,
             ),
             Variable(
-                "PL_ESTIMATE_PARASITICS",
-                bool,
-                "Specifies whether or not to run STA after global placement using OpenROAD's estimate_parasitics -placement and generate reports.",
-                default=True,
+                "FP_CORE_UTIL",
+                Decimal,
+                "The core utilization percentage.",
+                default=50,
+                units="%",
             ),
         ]
     )
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "gpl.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
-        env[
-            "PL_TARGET_DENSITY_PCT"
-        ] = f"{self.config['FP_CORE_UTIL'] + (5 * self.config['GPL_CELL_PADDING']) + 10}"
-        # Overriden by super if the value is not None
-        return super().run(env=env, **kwargs)
+        if os.getenv("PL_TARGET_DENSITY_PCT") is None:
+            expr = (
+                self.config["FP_CORE_UTIL"] + (5 * self.config["GPL_CELL_PADDING"]) + 10
+            )
+            expr = min(expr, 100)
+            env["PL_TARGET_DENSITY_PCT"] = f"{expr}"
+        return super().run(state_in, env=env, **kwargs)
 
 
 @Step.factory.register()
 class BasicMacroPlacement(OpenROADStep):
     id = "OpenROAD.BasicMacroPlacement"
     name = "Basic Macro Placement"
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
             "PL_MACRO_HALO",
             str,
             "Macro placement halo. Format: `{Horizontal} {Vertical}`.",
             default="0 0",
-            units="μm",
+            units="µm",
         ),
         Variable(
             "PL_MACRO_CHANNEL",
             str,
             "Channel widths between macros. Format: `{Horizontal} {Vertical}`.",
             default="0 0",
-            units="μm",
+            units="µm",
         ),
     ]
 
     def get_script_path(self):
         raise NotImplementedError()
 
 
 @Step.factory.register()
 class DetailedPlacement(OpenROADStep):
+    """
+    Performs "detailed placement" on an ODB file with global placement. This results
+    in a concrete and legal placement of all cells.
+    """
+
     id = "OpenROAD.DetailedPlacement"
     name = "Detailed Placement"
 
     config_vars = OpenROADStep.config_vars + dpl_variables
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "dpl.tcl")
 
 
 @Step.factory.register()
-class CTS(OpenROADStep):
-    id = "OpenROAD.CTS"
-    long_name = "Clock Tree Synthesis"
-    flow_control_variable = "RUN_CTS"
-
-    config_vars = dpl_variables + [
-        Variable(
-            "RUN_CTS",
-            bool,
-            "Enables/disables this step.",
-            default=True,
-            deprecated_names=["CLOCK_TREE_SYNTH"],
-        ),
-        Variable(
-            "CTS_TARGET_SKEW",
-            Decimal,
-            "The target clock skew in picoseconds.",
-            default=200,
-            units="ps",
-        ),
-        Variable(
-            "CTS_TOLERANCE",
-            int,
-            "An integer value that represents a tradeoff of QoR and runtime. Higher values will produce smaller runtime but worse QoR.",
-            default=100,
-        ),
-        Variable(
-            "CTS_SINK_CLUSTERING_SIZE",
-            int,
-            "Specifies the maximum number of sinks per cluster.",
-            default=25,
-        ),
-        Variable(
-            "CTS_SINK_CLUSTERING_MAX_DIAMETER",
-            Decimal,
-            "Specifies maximum diameter of the sink cluster.",
-            default=50,
-            units="μm",
-        ),
-        Variable(
-            "CTS_REPORT_TIMING",
-            bool,
-            "Specifies whether or not to run STA after clock tree synthesis using OpenROAD's `estimate_parasitics -placement`.",
-            default=True,
-        ),
-        Variable(
-            "CTS_CLK_MAX_WIRE_LENGTH",
-            Decimal,
-            "Specifies the maximum wire length on the clock net.",
-            default=0,
-            units="µm",
-        ),
-        Variable(
-            "CTS_DISABLE_POST_PROCESSING",
-            bool,
-            "Specifies whether or not to disable post cts processing for outlier sinks.",
-            default=False,
-        ),
-        Variable(
-            "CTS_DISTANCE_BETWEEN_BUFFERS",
-            Decimal,
-            "Specifies the distance between buffers when creating the clock tree.",
-            default=0,
-            units="µm",
-        ),
-    ]
-
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "openroad", "cts.tcl")
-
-
-@Step.factory.register()
 class GlobalRouting(OpenROADStep):
+    """
+    The initial phase of routing. Given a detailed-placed ODB file, this
+    phase starts assigning coarse-grained routing "regions" for each net so they
+    may be later connected to wires.
+
+    Estimated capacitance and resistance values are much more accurate for
+    global routing.
+
+    Updates the ``antenna__count`` metric.
+
+    At this stage, `antenna effect <https://en.wikipedia.org/wiki/Antenna_effect>`_
+    mitigations may also be applied, updating the `antenna__count` count.
+    See the variables for more info.
+    """
+
     id = "OpenROAD.GlobalRouting"
     name = "Global Routing"
 
-    config_vars = (
-        OpenROADStep.config_vars
-        + routing_layer_variables
-        + [
-            Variable(
-                "DIODE_PADDING",
-                int,
-                "Diode cell padding; increases the width of diode cells during placement checks..",
-                default=2,
-                units="sites",
-            ),
-            Variable(
-                "GRT_ALLOW_CONGESTION",
-                bool,
-                "Allow congestion during global routing",
-                default=False,
-            ),
-            Variable(
-                "GRT_REPAIR_ANTENNAS",
-                bool,
-                "Specifies the insertion strategy of diodes to be used in the flow.",
-                default=True,
-            ),
-            Variable(
-                "GRT_ANTENNA_ITERS",
-                int,
-                "The maximum number of iterations for global antenna repairs.",
-                default=3,
-                deprecated_names=["GRT_ANT_ITERS"],
-            ),
-            Variable(
-                "GRT_ESTIMATE_PARASITICS",
-                bool,
-                "Specifies whether or not to run STA after global routing using OpenROAD's `estimate_parasitics -global_routing`.",
-                default=True,
-            ),
-            Variable(
-                "GRT_OVERFLOW_ITERS",
-                int,
-                "The maximum number of iterations waiting for the overflow to reach the desired value.",
-                default=50,
-            ),
-        ]
-    )
+    config_vars = OpenROADStep.config_vars + grt_variables
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "grt.tcl")
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run(**kwargs)
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
 
         antenna_rpt_path = os.path.join(self.step_dir, "antenna.rpt")
-        antenna_rpt = open(antenna_rpt_path).read()
-        nets = get_antenna_nets(antenna_rpt)
+        net_count = get_antenna_nets(
+            open(antenna_rpt_path),
+            open(os.path.join(self.step_dir, "antenna_nets.txt"), "w"),
+        )
 
         antenna_report_post_fix_path = os.path.join(
             self.step_dir, "antenna_post_fix.rpt"
         )
         if os.path.exists(antenna_report_post_fix_path):
-            net_count_before = len(nets)
+            net_count_after = get_antenna_nets(
+                open(antenna_report_post_fix_path),
+                open(os.path.join(self.step_dir, "antenna_nets_post_fix.txt"), "w"),
+            )
 
-            antenna_rpt = open(antenna_report_post_fix_path).read()
-            nets = get_antenna_nets(antenna_rpt)
-            net_count_after = len(nets)
-
-            if net_count_before == net_count_after:
-                info("Antenna count unchanged after OpenROAD antenna fixer.")
-            elif net_count_after > net_count_before:
+            if net_count == net_count_after:
+                info(
+                    f"Antenna count unchanged after OpenROAD antenna fixer. ({net_count})"
+                )
+            elif net_count_after > net_count:
                 warn(
-                    "Inexplicably, the OpenROAD antenna fixer has generated more antenna. The flow may continue, but you may want to report a bug."
+                    f"Inexplicably, the OpenROAD antenna fixer has generated more antennas ({net_count} -> {net_count_after}). The flow will continue, but you may want to report a bug."
                 )
             else:
                 info(
-                    f"Antenna count reduced using OpenROAD antenna fixer: {net_count_before} -> {net_count_after}"
+                    f"Antenna count reduced using OpenROAD antenna fixer: {net_count} -> {net_count_after}"
                 )
+            net_count = net_count_after
 
-        state_out.metrics["antenna_nets"] = nets
+        metrics_updates["antenna__count"] = net_count
 
-        return state_out
+        return views_updates, metrics_updates
 
 
 @Step.factory.register()
 class DetailedRouting(OpenROADStep):
+    """
+    The latter phase of routing. This transforms the abstract nets from global
+    routing into wires on the metal layers that respect all design rules, avoids
+    creating accidental shorts, and ensures all wires are connected.
+
+    This is by far the longest part of a typical flow, taking hours, days or weeks
+    on larger designs.
+
+    After this point, all cells connected to a net can no longer be moved or
+    removed without a custom-written step of some kind that will also rip up
+    wires.
+    """
+
     id = "OpenROAD.DetailedRouting"
     name = "Detailed Routing"
     flow_control_variable = "RUN_DRT"
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
             "RUN_DRT",
             bool,
             "Enables/disables this step.",
             default=True,
         ),
         Variable(
-            "ROUTING_CORES",
+            "DRT_THREADS",
             Optional[int],
-            "Specifies the number of threads to be used in OpenROAD Detailed Routing. If unset, this will be equal to your thread count.",
+            "Specifies the number of threads to be used in OpenROAD Detailed Routing. If unset, this will be equal to your machine's thread count.",
+            deprecated_names=["ROUTING_CORES"],
         ),
         Variable(
             "DRT_MIN_LAYER",
             Optional[str],
             "An optional override to the lowest layer used in detailed routing. For example, in sky130, you may want global routing to avoid li1, but let detailed routing use li1 if it has to.",
         ),
         Variable(
@@ -643,40 +905,53 @@
             default=64,
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "drt.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
-        if self.config.get("ROUTING_CORES") is None:
-            env["ROUTING_CORES"] = str(os.cpu_count() or 1)
-        return super().run(env=env, **kwargs)
+        if self.config.get("DRT_THREADS") is None:
+            env["DRT_THREADS"] = str(os.cpu_count() or 1)
+        return super().run(state_in, env=env, **kwargs)
 
 
 @Step.factory.register()
 class LayoutSTA(OpenROADStep):
+    """
+    Performs `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
+    using OpenROAD on the ODB layout in its current state.
+    """
+
     id = "OpenROAD.LayoutSTA"
     name = "Layout STA"
     long_name = "Layout Static Timing Analysis"
+    inputs = [DesignFormat.ODB, DesignFormat.SDC]
 
     outputs = []
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "sta.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
         env["RUN_STANDALONE"] = "1"
-        return super().run(env=env, **kwargs)
+        return super().run(state_in, env=env, **kwargs)
 
 
 @Step.factory.register()
 class FillInsertion(OpenROADStep):
+    """
+    Fills gaps in the floorplan with filler and decapacitance cells.
+
+    This is run after detailed placement. After this point, the design is basically
+    completely hardened.
+    """
+
     id = "OpenROAD.FillInsertion"
     name = "Fill Insertion"
     flow_control_variable = "RUN_FILL_INSERTION"
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
             "RUN_FILL_INSERTION",
@@ -687,17 +962,24 @@
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "fill.tcl")
 
 
 @Step.factory.register()
-class ParasiticsExtraction(OpenROADStep):
-    id = "OpenROAD.ParasiticsExtraction"
-    name = "Parasitics Extraction"
+class RCX(OpenROADStep):
+    """
+    This extracts `parasitic <https://en.wikipedia.org/wiki/Parasitic_element_(electrical_networks)>`_
+    electrical values from a detailed-placed circuit. These can be used to create
+    basically the highest accurate STA possible for a design.
+    """
+
+    id = "OpenROAD.RCX"
+    name = "Parasitics (RC) Extraction"
+    long_name = "Parasitic Resistance/Capacitance Extraction"
     flow_control_variable = "RUN_SPEF_EXTRACTION"
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
             "RUN_SPEF_EXTRACTION",
             bool,
             "Enables/disables this step.",
@@ -712,95 +994,158 @@
         Variable(
             "RCX_SDC_FILE",
             Optional[Path],
             "Specifies SDC file to be used for RCX-based STA, which can be different from the one used for implementation.",
         ),
     ]
 
-    # default inputs
+    inputs = [DesignFormat.DEF]
     outputs = [DesignFormat.SPEF]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "rcx.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
-        env["RCX_RULESET"] = f"{self.config['RCX_RULES']}"
-        return super().run(env=env, **kwargs)
+        env = self.prepare_env(env, state_in)
 
+        def run_corner(corner: str):
+            rcx_ruleset = self.config["RCX_RULESETS"].get(corner)
+            if rcx_ruleset is None:
+                warn(
+                    f"RCX ruleset for corner {corner} not found. The corner may be ill-defined."
+                )
+                return None
 
-@Step.factory.register()
-class ParasiticsSTA(OpenROADStep):
-    id = "OpenROAD.ParasiticsSTA"
-    name = "Parasitics STA"
-    long_name = "Parasitics-based Static Timing Analysis"
-    flow_control_variable = "RUN_SPEF_STA"
+            corner_clean = corner
+            if corner_clean.endswith("_*"):
+                corner_clean = corner_clean[:-2]
 
-    config_vars = OpenROADStep.config_vars + [
-        Variable(
-            "RUN_SPEF_STA",
-            bool,
-            "Enables/disables this step.",
-            default=True,
-        ),
-    ]
+            nonlocal env
+            current_env = env.copy()
 
-    inputs = OpenROADStep.inputs + [DesignFormat.SPEF]
-    outputs = [DesignFormat.LIB, DesignFormat.SDF]
+            tech_lefs = self.toolbox.filter_views(
+                self.config, self.config["TECH_LEFS"], corner
+            )
+            if len(tech_lefs) < 1:
+                warn(f"No tech lef for timing corner {corner} found.")
+                return None
+            elif len(tech_lefs) > 1:
+                warn(
+                    f"Multiple tech lefs found for timing corner {corner}. Only the first one matched will be used."
+                )
 
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "openroad", "sta.tcl")
+            current_env["RCX_LEF"] = tech_lefs[0]
+            current_env["RCX_RULESET"] = rcx_ruleset
 
-    def run(self, **kwargs) -> State:
-        kwargs, env = self.extract_env(kwargs)
-        env["RUN_STANDALONE"] = "1"
-        return super().run(env=env, **kwargs)
+            out = os.path.join(
+                self.step_dir, f"{self.config['DESIGN_NAME']}.{corner_clean}.spef"
+            )
+            current_env["SAVE_SPEF"] = out
+
+            log_path = os.path.join(self.step_dir, f"{corner_clean}.log")
+            info(
+                f"Running RCX for the {corner_clean} interconnect corner ({log_path})…"
+            )
+
+            try:
+                self.run_subprocess(
+                    self.get_command(),
+                    log_to=log_path,
+                    env=current_env,
+                    silent=True,
+                )
+                info(f"Finished RCX for the {corner_clean} interconnect corner.")
+            except subprocess.CalledProcessError as e:
+                err(f"Failed RCX for the {corner_clean} interconnect corner:")
+                raise e
+
+            return out
+
+        futures: Dict[str, Future[str]] = {}
+        for corner in self.config["RCX_RULESETS"]:
+            futures[corner] = get_tpe().submit(
+                run_corner,
+                corner,
+            )
+
+        views_updates: ViewsUpdate = {}
+        metrics_updates: MetricsUpdate = {}
+
+        spef_dict = state_in[DesignFormat.SPEF] or {}
+        if not isinstance(spef_dict, dict):
+            raise StepException(
+                "Malformed input state: value for SPEF is not a dictionary."
+            )
+
+        for corner, future in futures.items():
+            if result := future.result():
+                spef_dict[corner] = Path(result)
+
+        views_updates[DesignFormat.SPEF] = spef_dict
+
+        return views_updates, metrics_updates
 
 
 # Antennas
-def get_antenna_nets(report: str) -> List[str]:
+def get_antenna_nets(report: io.TextIOWrapper, output: io.TextIOWrapper) -> int:
     pattern = re.compile(r"Net:\s*(\w+)")
-    antenna_nets = []
+    count = 0
 
-    for line in report.splitlines():
+    for line in report:
+        line = line.strip()
         m = pattern.match(line)
         if m is None:
             continue
         net = m[1]
-        antenna_nets.append(net)
+        output.write(f"{net}\n")
+        count += 1
 
-    return antenna_nets
+    return count
 
 
 @Step.factory.register()
 class CheckAntennas(OpenROADStep):
+    """
+    Runs OpenROAD to check if one or more long nets may constitute an
+    `antenna risk <https://en.wikipedia.org/wiki/Antenna_effect>`_.
+
+    The metric ``antenna__count`` will be updated with the number of violating nets.
+    """
+
     id = "OpenROAD.CheckAntennas"
     name = "Check Antennas"
 
     # default inputs
     outputs = []
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "check_antennas.tcl")
 
-    def run(self, **kwargs) -> State:
-        state_out = super().run(**kwargs)
-
-        antenna_rpt = open(os.path.join(self.step_dir, "antenna.rpt")).read()
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
 
-        state_out.metrics["antenna_nets"] = get_antenna_nets(antenna_rpt)
+        metrics_updates["antenna__count"] = get_antenna_nets(
+            open(os.path.join(self.step_dir, "antenna.rpt")),
+            open(os.path.join(self.step_dir, "antenna_net_list.txt"), "w"),
+        )
 
-        return state_out
+        return views_updates, metrics_updates
 
 
 @Step.factory.register()
 class IRDropReport(OpenROADStep):
+    """
+    Performs voltage-drop analysis on the power distribution network.
+    """
+
     id = "OpenROAD.IRDropReport"
     name = "IR Drop Report"
     long_name = "Generate IR Drop Report"
+    flow_control_variable = "RUN_IRDROP_REPORT"
 
     inputs = [DesignFormat.ODB, DesignFormat.SPEF]
     outputs = []
 
     config_vars = OpenROADStep.config_vars + [
         Variable(
             "RUN_IRDROP_REPORT",
@@ -809,247 +1154,444 @@
             default=True,
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "irdrop.tcl")
 
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         from decimal import Decimal
 
-        state_out = super().run(**kwargs)
+        if state_in[DesignFormat.SPEF] is None:
+            raise StepException(
+                "SPEF extraction was not performed before IR drop report."
+            )
+
+        if not isinstance(state_in[DesignFormat.SPEF], dict):
+            raise StepException(
+                "Malformed input state: value for SPEF is not a dictionary."
+            )
+
+        kwargs, env = self.extract_env(kwargs)
+
+        input_spef_dict = state_in[DesignFormat.SPEF]
+        assert input_spef_dict is not None  # Checked by start
+        if not isinstance(input_spef_dict, dict):
+            raise StepException(
+                "Malformed input state: value for 'spef' is not a dictionary"
+            )
+
+        spefs_in = self.toolbox.filter_views(self.config, input_spef_dict)
+        if len(spefs_in) > 1:
+            raise StepException(
+                "Found more than one input SPEF file for the default corner."
+            )
+        elif len(spefs_in) < 1:
+            raise StepException("No SPEF file found for the default corner.")
+
+        env["CURRENT_SPEF_DEFAULT_CORNER"] = str(spefs_in[0])
+        views_updates, metrics_updates = super().run(state_in, env=env, **kwargs)
 
         report = open(os.path.join(self.step_dir, "irdrop.rpt")).read()
 
         voltage_rx = re.compile(r"Worstcase voltage\s*:\s*([\d\.\+\-e]+)\s*V")
         avg_drop_rx = re.compile(r"Average IR drop\s*:\s*([\d\.\+\-e]+)\s*V")
         worst_drop_rx = re.compile(r"Worstcase IR drop\s*:\s*([\d\.\+\-e]+)\s*V")
 
         if m := voltage_rx.search(report):
             value_float = float(m[1])
             value_dec = Decimal(value_float)
-            state_out.metrics["ir__voltage__worst"] = value_dec
+            metrics_updates["ir__voltage__worst"] = value_dec
         else:
             raise Exception(
                 "OpenROAD IR Drop Log format has changed- please file an issue."
             )
 
         if m := avg_drop_rx.search(report):
             value_float = float(m[1])
             value_dec = Decimal(value_float)
-            state_out.metrics["ir__drop__avg"] = value_dec
+            metrics_updates["ir__drop__avg"] = value_dec
         else:
             raise Exception(
                 "OpenROAD IR Drop Log format has changed- please file an issue."
             )
 
         if m := worst_drop_rx.search(report):
             value_float = float(m[1])
             value_dec = Decimal(value_float)
-            state_out.metrics["ir__drop__worst"] = value_dec
+            metrics_updates["ir__drop__worst"] = value_dec
         else:
             raise Exception(
                 "OpenROAD IR Drop Log format has changed- please file an issue."
             )
 
-        return state_out
+        return views_updates, metrics_updates
 
 
 # Resizer Steps
 
+## ABC
+class ResizerStep(OpenROADStep):
+    config_vars = OpenROADStep.config_vars + grt_variables + rsz_variables
+
+    def run(
+        self,
+        state_in,
+        **kwargs,
+    ) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        kwargs, env = self.extract_env(kwargs)
+
+        corners_key: str = "RSZ_CORNERS"
+
+        if "corners_key" in kwargs:
+            corners_key = kwargs["corners_key"]
+            del kwargs["corners_key"]
+
+        corners = self.config[corners_key] or self.config["STA_CORNERS"]
+        lib_set_set = set()
+        count = 0
+        for corner in corners:
+            _, libs = self.toolbox.get_timing_files(self.config, corner)
+            lib_set = frozenset(libs)
+            if lib_set in lib_set_set:
+                debug(f"Liberty files for '{corner}' already accounted for- skipped")
+                continue
+            lib_set_set.add(lib_set)
+            env[f"RSZ_CORNER_{count}"] = f"{corner} {shlex.join(libs)}"
+            debug(f"Liberty files for '{corner}' added: {libs}")
+            count += 1
+
+        return super().run(state_in, env=env, **kwargs)
+
 
 @Step.factory.register()
-class RepairDesign(OpenROADStep):
-    id = "OpenROAD.RepairDesign"
-    name = "Repair Design (Post-Global Placement)"
-    flow_control_variable = "RUN_REPAIR_DESIGN"
+class CTS(ResizerStep):
+    """
+    Creates a `Clock tree <https://en.wikipedia.org/wiki/Clock_signal#Distribution>`_
+    for an ODB file with detailed-placed cells, using reasonably accurate resistance
+    and capacitance estimations. Detailed Placement is then re-performed to
+    accomodate the new cells.
+    """
+
+    id = "OpenROAD.CTS"
+    name = "Clock Tree Synthesis"
+    flow_control_variable = "RUN_CTS"
 
     config_vars = (
         OpenROADStep.config_vars
-        + rsz_variables
+        + dpl_variables
         + [
             Variable(
-                "RUN_REPAIR_DESIGN",
+                "RUN_CTS",
                 bool,
                 "Enables/disables this step.",
                 default=True,
-                deprecated_names=["PL_RESIZER_DESIGN_OPTIMIZATIONS"],
+                deprecated_names=["CLOCK_TREE_SYNTH"],
             ),
             Variable(
-                "DESIGN_REPAIR_BUFFER_INPUT_PORTS",
-                bool,
-                "Specifies whether or not to insert buffers on input ports when design repairs are run.",
-                default=True,
-                deprecated_names=["PL_RESIZER_BUFFER_INPUT_PORTS"],
+                "CTS_TOLERANCE",
+                int,
+                "An integer value that represents a tradeoff of QoR and runtime. Higher values will produce smaller runtime but worse QoR.",
+                default=100,
             ),
             Variable(
-                "DESIGN_REPAIR_BUFFER_OUTPUT_PORTS",
-                bool,
-                "Specifies whether or not to insert buffers on input ports when design repairs are run.",
-                default=True,
-                deprecated_names=["PL_RESIZER_BUFFER_OUTPUT_PORTS"],
+                "CTS_SINK_CLUSTERING_SIZE",
+                int,
+                "Specifies the maximum number of sinks per cluster.",
+                default=25,
             ),
             Variable(
-                "DESIGN_REPAIR_TIE_FANOUT",
-                bool,
-                "Specifies whether or not to repair tie cells fanout when design repairs are run.",
-                default=True,
-                deprecated_names=["PL_RESIZER_REPAIR_TIE_FANOUT"],
+                "CTS_SINK_CLUSTERING_MAX_DIAMETER",
+                Decimal,
+                "Specifies maximum diameter of the sink cluster.",
+                default=50,
+                units="µm",
             ),
             Variable(
-                "DESIGN_REPAIR_TIE_SEPARATION",
+                "CTS_CLK_MAX_WIRE_LENGTH",
+                Decimal,
+                "Specifies the maximum wire length on the clock net.",
+                default=0,
+                units="µm",
+            ),
+            Variable(
+                "CTS_DISABLE_POST_PROCESSING",
                 bool,
-                "Allows tie separation when performing design repairs.",
+                "Specifies whether or not to disable post cts processing for outlier sinks.",
                 default=False,
-                deprecated_names=["PL_RESIZER_TIE_SEPERATION"],
             ),
             Variable(
-                "DESIGN_REPAIR_MAX_WIRE_LENGTH",
+                "CTS_DISTANCE_BETWEEN_BUFFERS",
                 Decimal,
-                "Specifies the maximum wire length cap used by resizer to insert buffers. If set to 0, no buffers will be inserted.",
+                "Specifies the distance between buffers when creating the clock tree.",
                 default=0,
                 units="µm",
-                deprecated_names=["PL_RESIZER_MAX_WIRE_LENGTH"],
             ),
             Variable(
-                "DESIGN_REPAIR_MAX_SLEW_PCT",
-                Decimal,
-                "Specifies a margin for the slews during design repair.",
-                default=20,
-                units="%",
-                deprecated_names=["PL_RESIZER_MAX_SLEW_MARGIN"],
-            ),
-            Variable(
-                "DESIGN_REPAIR_MAX_CAP_PCT",
-                Decimal,
-                "Specifies a margin for the capacitances during design repair.",
-                default=20,
-                units="%",
-                deprecated_names=["PL_RESIZER_MAX_CAP_MARGIN"],
+                "CTS_CORNERS",
+                Optional[List[str]],
+                "A list of fully-qualified IPVT corners to use during clock tree synthesis. If unspecified, the value for `STA_CORNERS` from the PDK will be used.",
             ),
         ]
     )
 
     def get_script_path(self):
+        return os.path.join(get_script_dir(), "openroad", "cts.tcl")
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        kwargs, env = self.extract_env(kwargs)
+        if self.config.get("CLOCK_NET") is None:
+            if clock_port := self.config["CLOCK_PORT"]:
+                if isinstance(clock_port, list):
+                    env["CLOCK_NET"] = " ".join(clock_port)
+                else:
+                    env["CLOCK_NET"] = clock_port
+            else:
+                warn(
+                    "No CLOCK_NET (or CLOCK_PORT) specified. CTS cannot be performed. Returning state unaltered…"
+                )
+                return Step.run(self, state_in, **kwargs)
+
+        views_updates, metrics_updates = super().run(
+            state_in, corners_key="CTS_CORNERS", env=env, **kwargs
+        )
+
+        return views_updates, metrics_updates
+
+
+@Step.factory.register()
+class RepairDesign(ResizerStep):
+    """
+    Runs a number of design "repairs" on a global-placed ODB file.
+    """
+
+    id = "OpenROAD.RepairDesign"
+    name = "Repair Design (Post-Global Placement)"
+    flow_control_variable = "RUN_REPAIR_DESIGN"
+
+    config_vars = ResizerStep.config_vars + [
+        Variable(
+            "RUN_REPAIR_DESIGN",
+            bool,
+            "Enables/disables this step.",
+            default=True,
+            deprecated_names=["PL_RESIZER_DESIGN_OPTIMIZATIONS"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_BUFFER_INPUT_PORTS",
+            bool,
+            "Specifies whether or not to insert buffers on input ports when design repairs are run.",
+            default=True,
+            deprecated_names=["PL_RESIZER_BUFFER_INPUT_PORTS"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_BUFFER_OUTPUT_PORTS",
+            bool,
+            "Specifies whether or not to insert buffers on input ports when design repairs are run.",
+            default=True,
+            deprecated_names=["PL_RESIZER_BUFFER_OUTPUT_PORTS"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_TIE_FANOUT",
+            bool,
+            "Specifies whether or not to repair tie cells fanout when design repairs are run.",
+            default=True,
+            deprecated_names=["PL_RESIZER_REPAIR_TIE_FANOUT"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_TIE_SEPARATION",
+            bool,
+            "Allows tie separation when performing design repairs.",
+            default=False,
+            deprecated_names=["PL_RESIZER_TIE_SEPERATION"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_MAX_WIRE_LENGTH",
+            Decimal,
+            "Specifies the maximum wire length cap used by resizer to insert buffers. If set to 0, no buffers will be inserted.",
+            default=0,
+            units="µm",
+            deprecated_names=["PL_RESIZER_MAX_WIRE_LENGTH"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_MAX_SLEW_PCT",
+            Decimal,
+            "Specifies a margin for the slews during design repair.",
+            default=20,
+            units="%",
+            deprecated_names=["PL_RESIZER_MAX_SLEW_MARGIN"],
+        ),
+        Variable(
+            "DESIGN_REPAIR_MAX_CAP_PCT",
+            Decimal,
+            "Specifies a margin for the capacitances during design repair.",
+            default=20,
+            units="%",
+            deprecated_names=["PL_RESIZER_MAX_CAP_MARGIN"],
+        ),
+    ]
+
+    def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "repair_design.tcl")
 
 
 @Step.factory.register()
-class ResizerTimingPostCTS(OpenROADStep):
+class ResizerTimingPostCTS(ResizerStep):
+    """
+    First attempt to meet timing requirements for a cell based on basic timing
+    information after clock tree synthesis.
+
+    Standard cells may be resized, and buffer cells may be inserted to ensure
+    that no hold violations exist and no setup violations exist at the current
+    clock.
+    """
+
     id = "OpenROAD.ResizerTimingPostCTS"
     name = "Resizer Timing Optimizations (Post-Clock Tree Synthesis)"
     flow_control_variable = "RUN_POST_CTS_RESIZER_TIMING"
 
-    config_vars = (
-        OpenROADStep.config_vars
-        + rsz_variables
-        + [
-            Variable(
-                "RUN_POST_CTS_RESIZER_TIMING",
-                bool,
-                "Enables/disables this step.",
-                default=True,
-                deprecated_names=["PL_RESIZER_TIMING_OPTIMIZATIONS"],
-            ),
-            Variable(
-                "PL_RESIZER_HOLD_SLACK_MARGIN",
-                Decimal,
-                "Specifies a time margin for the slack when fixing hold violations. Normally the resizer will stop when it reaches zero slack. This option allows you to overfix.",
-                default=0.1,
-                units="ns",
-            ),
-            Variable(
-                "PL_RESIZER_SETUP_SLACK_MARGIN",
-                Decimal,
-                "Specifies a time margin for the slack when fixing setup violations.",
-                default=0.05,
-                units="ns",
-            ),
-            Variable(
-                "PL_RESIZER_HOLD_MAX_BUFFER_PCT",
-                Decimal,
-                "Specifies a max number of buffers to insert to fix hold violations. This number is calculated as a percentage of the number of instances in the design.",
-                default=50,
-                deprecated_names=["PL_RESIZER_HOLD_MAX_BUFFER_PERCENT"],
-            ),
-            Variable(
-                "PL_RESIZER_SETUP_MAX_BUFFER_PCT",
-                Decimal,
-                "Specifies a max number of buffers to insert to fix setup violations. This number is calculated as a percentage of the number of instances in the design.",
-                default=50,
-                units="%",
-                deprecated_names=["PL_RESIZER_SETUP_MAX_BUFFER_PERCENT"],
-            ),
-            Variable(
-                "PL_RESIZER_ALLOW_SETUP_VIOS",
-                bool,
-                "Allows the creation of setup violations when fixing hold violations.",
-                default=False,
-            ),
-        ]
-    )
+    config_vars = ResizerStep.config_vars + [
+        Variable(
+            "RUN_POST_CTS_RESIZER_TIMING",
+            bool,
+            "Enables/disables this step.",
+            default=True,
+            deprecated_names=["PL_RESIZER_TIMING_OPTIMIZATIONS"],
+        ),
+        Variable(
+            "PL_RESIZER_HOLD_SLACK_MARGIN",
+            Decimal,
+            "Specifies a time margin for the slack when fixing hold violations. Normally the resizer will stop when it reaches zero slack. This option allows you to overfix.",
+            default=0.1,
+            units="ns",
+        ),
+        Variable(
+            "PL_RESIZER_SETUP_SLACK_MARGIN",
+            Decimal,
+            "Specifies a time margin for the slack when fixing setup violations.",
+            default=0.05,
+            units="ns",
+        ),
+        Variable(
+            "PL_RESIZER_HOLD_MAX_BUFFER_PCT",
+            Decimal,
+            "Specifies a max number of buffers to insert to fix hold violations. This number is calculated as a percentage of the number of instances in the design.",
+            default=50,
+            deprecated_names=["PL_RESIZER_HOLD_MAX_BUFFER_PERCENT"],
+        ),
+        Variable(
+            "PL_RESIZER_SETUP_MAX_BUFFER_PCT",
+            Decimal,
+            "Specifies a max number of buffers to insert to fix setup violations. This number is calculated as a percentage of the number of instances in the design.",
+            default=50,
+            units="%",
+            deprecated_names=["PL_RESIZER_SETUP_MAX_BUFFER_PERCENT"],
+        ),
+        Variable(
+            "PL_RESIZER_ALLOW_SETUP_VIOS",
+            bool,
+            "Allows the creation of setup violations when fixing hold violations. Setup violations are less dangerous as they simply mean a chip may not run at its rated speed, however, chips with hold violations are essentially dead-on-arrival.",
+            default=False,
+        ),
+    ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "rsz_timing_postcts.tcl")
 
 
 @Step.factory.register()
-class ResizerTimingPostGRT(OpenROADStep):
+class ResizerTimingPostGRT(ResizerStep):
+    """
+    Second attempt to meet timing requirements for a cell based on timing
+    information after estimating resistance and capacitance values based on
+    global routing.
+
+    Standard cells may be resized, and buffer cells may be inserted to ensure
+    that no hold violations exist and no setup violations exist at the current
+    clock.
+    """
+
     id = "OpenROAD.ResizerTimingPostGRT"
     name = "Resizer Timing Optimizations (Post-Global Routing)"
     flow_control_variable = "RUN_POST_GRT_RESIZER_TIMING"
 
-    config_vars = (
-        OpenROADStep.config_vars
-        + rsz_variables
-        + [
-            Variable(
-                "RUN_POST_GRT_RESIZER_TIMING",
-                bool,
-                "Enables/disables this step.",
-                default=True,
-                deprecated_names=["GLB_RESIZER_TIMING_OPTIMIZATIONS"],
-            ),
-            Variable(
-                "GRT_RESIZER_HOLD_SLACK_MARGIN",
-                str,
-                "Specifies a time margin for the slack when fixing hold violations. Normally the resizer will stop when it reaches zero slack. This option allows you to overfix.",
-                default=0.05,
-                units="ns",
-                deprecated_names=["GLB_RESIZER_HOLD_SLACK_MARGIN"],
-            ),
-            Variable(
-                "GRT_RESIZER_SETUP_SLACK_MARGIN",
-                str,
-                "Specifies a time margin for the slack when fixing setup violations.",
-                default=0.025,
-                units="ns",
-                deprecated_names=["GLB_RESIZER_SETUP_SLACK_MARGIN"],
-            ),
-            Variable(
-                "GRT_RESIZER_HOLD_MAX_BUFFER_PCT",
-                Decimal,
-                "Specifies a max number of buffers to insert to fix hold violations. This number is calculated as a percentage of the number of instances in the design.",
-                default=50,
-                units="%",
-                deprecated_names=["GLB_RESIZER_HOLD_MAX_BUFFER_PERCENT"],
-            ),
-            Variable(
-                "GRT_RESIZER_SETUP_MAX_BUFFER_PCT",
-                Decimal,
-                "Specifies a max number of buffers to insert to fix setup violations. This number is calculated as a percentage of the number of instances in the design.",
-                default=50,
-                units="%",
-                deprecated_names=["GLB_RESIZER_SETUP_MAX_BUFFER_PERCENT"],
-            ),
-            Variable(
-                "GRT_RESIZER_ALLOW_SETUP_VIOS",
-                bool,
-                "Allows setup violations when fixing hold.",
-                default=False,
-                deprecated_names=["GLB_RESIZER_ALLOW_SETUP_VIOS"],
-            ),
-        ]
-    )
+    config_vars = ResizerStep.config_vars + [
+        Variable(
+            "RUN_POST_GRT_RESIZER_TIMING",
+            bool,
+            "Enables/disables this step.",
+            default=True,
+            deprecated_names=["GLB_RESIZER_TIMING_OPTIMIZATIONS"],
+        ),
+        Variable(
+            "GRT_RESIZER_HOLD_SLACK_MARGIN",
+            Decimal,
+            "Specifies a time margin for the slack when fixing hold violations. Normally the resizer will stop when it reaches zero slack. This option allows you to overfix.",
+            default=0.05,
+            units="ns",
+            deprecated_names=["GLB_RESIZER_HOLD_SLACK_MARGIN"],
+        ),
+        Variable(
+            "GRT_RESIZER_SETUP_SLACK_MARGIN",
+            Decimal,
+            "Specifies a time margin for the slack when fixing setup violations.",
+            default=0.025,
+            units="ns",
+            deprecated_names=["GLB_RESIZER_SETUP_SLACK_MARGIN"],
+        ),
+        Variable(
+            "GRT_RESIZER_HOLD_MAX_BUFFER_PCT",
+            Decimal,
+            "Specifies a max number of buffers to insert to fix hold violations. This number is calculated as a percentage of the number of instances in the design.",
+            default=50,
+            units="%",
+            deprecated_names=["GLB_RESIZER_HOLD_MAX_BUFFER_PERCENT"],
+        ),
+        Variable(
+            "GRT_RESIZER_SETUP_MAX_BUFFER_PCT",
+            Decimal,
+            "Specifies a max number of buffers to insert to fix setup violations. This number is calculated as a percentage of the number of instances in the design.",
+            default=50,
+            units="%",
+            deprecated_names=["GLB_RESIZER_SETUP_MAX_BUFFER_PERCENT"],
+        ),
+        Variable(
+            "GRT_RESIZER_ALLOW_SETUP_VIOS",
+            bool,
+            "Allows setup violations when fixing hold.",
+            default=False,
+            deprecated_names=["GLB_RESIZER_ALLOW_SETUP_VIOS"],
+        ),
+    ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "rsz_timing_postgrt.tcl")
+
+
+@Step.factory.register()
+class OpenGUI(Step):
+    """
+    Opens the ODB view in the OpenROAD GUI. Useful to inspect some parameters,
+    such as routing density and whatnot.
+    """
+
+    id = "OpenROAD.OpenGUI"
+    name = "Open In GUI"
+
+    inputs = [DesignFormat.ODB]
+    outputs = []
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        with tempfile.NamedTemporaryFile("a+", suffix=".tcl") as f:
+            f.write(f"read_db \"{state_in['odb']}\"")
+            f.flush()
+
+            subprocess.check_call(
+                [
+                    "openroad",
+                    "-no_splash",
+                    "-gui",
+                    f.name,
+                ]
+            )
+
+        return {}, {}
```

### Comparing `openlane-2.0.0a9/openlane/steps/step.py` & `openlane-2.0.0b1/openlane/steps/step.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,297 +13,460 @@
 # limitations under the License.
 from __future__ import annotations
 
 import os
 import time
 import textwrap
 import subprocess
+from signal import Signals
+from inspect import isabstract
+from itertools import zip_longest
 from abc import abstractmethod, ABC
 from concurrent.futures import Future
 from typing import (
+    Any,
     List,
     Callable,
     Optional,
     Union,
     Tuple,
     Sequence,
     Dict,
     ClassVar,
     Type,
 )
 
+from openlane.state.state import StateElement
+
 from ..state import State, InvalidState
-from ..state import DesignFormat, DesignFormatByID
+from ..state import DesignFormat
 from ..utils import Toolbox
 from ..config import Config, Variable
 from ..common import (
+    GenericImmutableDict,
     mkdirp,
     slugify,
     final,
-    internal,
+    protected,
 )
 from ..logging import (
     rule,
     verbose,
     info,
     warn,
     err,
 )
 
-StepConditionLambda = Callable[[Config], bool]
 
+class StepError(RuntimeError):
+    """
+    A ``RuntimeError`` that occurs when a Step fails to finish execution
+    properly.
+    """
 
-class MissingInputError(ValueError):
     pass
 
 
-class StepError(ValueError):
+class DeferredStepError(StepError):
+    """
+    A variant of :class:`StepError` where parent Flows are encouraged to continue
+    execution of subsequent steps regardless and then finally flag the Error
+    at the very end.
+    """
+
     pass
 
 
 class StepException(StepError):
+    """
+    A variant of :class:`StepError` for unexpected failures or failures due
+    to misconfiguration, such as:
+
+    * Invalid inputs
+    * Mis-use of class interfaces of the :class:`Step`
+    * Other unexpected failures
+    """
+
     pass
 
 
-class DeferredStepError(StepError):
+class StepSignalled(StepException):
     pass
 
 
 REPORT_START_LOCUS = "%OL_CREATE_REPORT"
 REPORT_END_LOCUS = "%OL_END_REPORT"
+METRIC_LOCUS = "%OL_METRIC"
 
 GlobalToolbox = Toolbox(os.path.join(os.getcwd(), "openlane_run", "tmp"))
 LastState: State = State()
 
+ViewsUpdate = Dict[DesignFormat, StateElement]
+MetricsUpdate = Dict[str, Any]
 
-class Step(ABC):
-    class _FlowType(ABC):
-        """
-        "Forward declaration" for the methods a step uses to interact with its
-        parent Flow.
-        """
-
-        toolbox: Optional[Toolbox] = None
-
-        @abstractmethod
-        def dir_for_step(self, step: Step) -> str:
-            pass
 
+class Step(ABC):
     """
     An abstract base class for Step objects.
 
     Steps encapsulate a subroutine that acts upon certain classes of formats
     in an input state and returns a new output state with updated design format
     paths and/or metrics.
 
     Warning: The initializer for Step is not thread-safe. Please use it on the main
-    thread and then, if you're using a Flow object, use `start_step_async`, or
-    if you're not, you may use `start` in another thread. That part's fine.
+    thread and then, if you're using a Flow object, use ``start_step_async``, or
+    if you're not, you may use ``start`` in another thread. That part's fine.
 
     :param config: A configuration object.
 
-        If running in interactive mode, you can set this to ``None``, where it
-        will automatically use :ref:`Config.current_interactive`, but it is
+        If running in interactive mode, you can set this to ``None``, but it is
         otherwise required.
 
-    :param flow: The parent flow, if applicable.
-
     :param state_in: The state object this step will use as an input.
 
-        The state may also be a `Future[State]`, in which case,
-        the `run()` call will block until that Future is realized.
+        The state may also be a ``Future[State]``, in which case,
+        the ``start()`` call will block until that Future is realized.
         This allows you to chain a number of asynchronous steps.
 
         See https://en.wikipedia.org/wiki/Futures_and_promises for a primer.
 
         If running in interactive mode, you can set this to ``None``, where it
         will use the last generated state, but it is otherwise required.
 
     :param step_dir: A "scratch directory" for the step. Required.
 
         You may omit this argument as ``None`` if "flow" is specified.
 
-    :param name: An optional override name for the step. Useful in custom flows.
-    :param id: An optional override name for the ID. Useful in custom flows.
-    :param long_name: An optional override name for the long name. Useful in custom flows.
+    :param id: A string ID for the Step. The convention is f"{a}.{b}", where the
+        first is common between all Steps using the same tools.
+
+        The ID should be in ``UpperCamelCase``.
+
+        While this is technically an instance variable, it is expected for every
+        subclass to override this variable and instances are only to change it
+        to disambiguate when the same step is used multiple times in a flow.
+
+    :param name: A short name for the Step, used in progress bars and
+        the like.
+
+        While this is technically an instance variable, it is expected for every
+        subclass to override this variable and instances are only to change it
+        to disambiguate when the same step is used multiple times in a flow.
+
+    :param long_name: A longer descriptive for the Step, used to delimit
+        logs.
 
-        If set to false, Step implementations are expected to
-        output nothing to the terminal.
+        While this is technically an instance variable, it is expected for every
+        subclass to override this variable and instances are only to change it
+        to disambiguate when the same step is used multiple times in a flow.
 
-    :attr flow_control_variable: An optional key for a configuration variable.
+    :param flow: Deprecated: the parent flow. Ignored if passed.
+
+    :cvar inputs: A list of :class:`openlane.state.DesignFormat` objects that
+        are required for this step. These will be validated by the :meth:`start`
+        method.
+
+    :cvar outputs: A list of :class:`openlane.state.DesignFormat` objects that
+        may be emitted by this step. A step is not allowed to modify design
+        formats not declared in ``outputs``.
+
+    :cvar flow_control_variable: An optional key for a configuration variable.
 
         If running inside a Flow, and this exists, if this variable is "False"
         or "None", the step is skipped.
 
-    :attr flow_control_msg: If `flow_control_variable` causes the step to be
+    :cvar flow_control_msg: If ``flow_control_variable`` causes the step to be
         skipped and this variable is set, the value of this variable is
         printed.
-    """
 
-    inputs: List[DesignFormat] = []
-    outputs: List[DesignFormat] = []
+    :cvar config_vars: A list of configuration :class:`openlane.config.Variable` objects
+        to be used to alter the behavior of this Step.
 
-    id: str = NotImplemented
-    name: str
-    long_name: str
+    :ivar state_out:
+        The last output state from running this step object, if it exists.
+
+        If :meth:`start` is called again, the reference is destroyed.
+
+    :ivar start_time:
+        The last starting time from running this step object, if it exists.
+
+        If :meth:`start` is called again, the reference is destroyed.
+
+    :ivar end_time:
+        The last ending time from running this step object, if it exists.
+
+        If :meth:`start` is called again, the reference is destroyed.
+
+    :ivar toolbox:
+        The last :class:`Toolbox` used while running this step object, if it
+        exists.
 
+        If :meth:`start` is called again, the reference is destroyed.
+    """
+
+    # Class Variables
+    inputs: ClassVar[List[DesignFormat]]
+    outputs: ClassVar[List[DesignFormat]]
     flow_control_variable: ClassVar[Optional[str]] = None
     flow_control_msg: ClassVar[Optional[str]] = None
     config_vars: ClassVar[List[Variable]] = []
 
+    # Instance Variables
+    id: str = NotImplemented
+    name: str
+    long_name: str
+    state_in: Future[State]
+
+    ## Stateful
+    toolbox: Toolbox = GlobalToolbox
+    state_out: Optional[State] = None
     start_time: Optional[float] = None
     end_time: Optional[float] = None
-    toolbox: Toolbox = GlobalToolbox
 
     # These are mutable class variables. However, they will only be used
     # when steps are run outside of a Flow, pretty much.
     counter: ClassVar[int] = 1
     # End Mutable Global Variables
 
     def __init__(
         self,
         config: Optional[Config] = None,
         state_in: Union[Optional[State], Future[State]] = None,
-        step_dir: Optional[str] = None,
+        *,
         id: Optional[str] = None,
         name: Optional[str] = None,
         long_name: Optional[str] = None,
-        flow: Optional[_FlowType] = None,
+        flow: Optional[Any] = None,
         **kwargs,
     ):
         if self.id == NotImplemented:
             raise NotImplementedError(
                 "All subclasses of Step must override the value of id."
             )
 
+        if flow is not None:
+            warn(
+                f"Passing 'flow' to a Step class's initializer is deprecated. Please update the flow '{type(flow).__name__}'."
+            )
+
         if id is not None:
             self.id = id
 
         if config is None:
             if current_interactive := Config.current_interactive:
                 config = current_interactive
             else:
                 raise TypeError("Missing required argument 'config'")
 
         if state_in is None:
-            if config.interactive is not None:
+            if Config.current_interactive:
                 state_in = LastState
             else:
                 raise TypeError("Missing required argument 'state_in'")
 
         if name is not None:
             self.name = name
         elif not hasattr(self, "name"):
             self.name = self.__class__.__name__
 
         if long_name is not None:
             self.long_name = long_name
         elif not hasattr(self, "long_name"):
             self.long_name = self.name
 
-        if config.interactive:
+        if Config.current_interactive:
             mutable = Config(**kwargs.copy())
-            overrides, warnings, errors = Variable.process_config(
-                mutable,
-                variables=self.config_vars,
+            overrides, warnings, errors = mutable.__process_variable_list(
+                [],
+                self.config_vars,
             )
-            config.update(**overrides)
+            config = config.copy(**overrides)
             for warning in warnings:
                 warn(warning)
             if len(errors) != 0:
                 err(f"Errors while processing inputs for {self.name}:")
                 for error in errors:
                     err(error)
                 raise StepException("Failed to handle one or more kwarg variables.")
         elif len(kwargs) != 0:
             raise StepException(
                 "Variables may not be passed as keyword arguments unless the Config object is per-step."
             )
 
-        self.config = config.copy()
+        self.config = config.copy_filtered(
+            self.config_vars,
+            include_pdk_variables=True,
+            include_common_variables=True,
+        )
 
-        self.flow = flow
-        if step_dir is None:
-            if self.flow is not None:
-                self.step_dir = self.flow.dir_for_step(self)
-            elif self.config.interactive:
-                raise TypeError("Missing required argument 'step_dir'")
-            else:
-                step_dir = os.path.join(
-                    os.getcwd(),
-                    "openlane_run",
-                    f"{Step.counter}-{slugify(self.id)}",
-                )
-                Step.counter += 1
+        state_in_future: Future[State] = Future()
+        if isinstance(state_in, State):
+            state_in_future.set_result(state_in)
         else:
-            self.step_dir = step_dir
-        self.state_in = state_in
+            state_in_future = state_in
+        self.state_in = state_in_future
+
+    def __init_subclass__(cls):
+        if not isabstract(cls):
+            for attr in ["inputs", "outputs"]:
+                if not hasattr(cls, attr):
+                    raise NotImplementedError(
+                        f"{cls} must implement class attribute '{attr}'"
+                    )
 
     @classmethod
-    def _get_desc(Self) -> str:
-        """
-        Used for documentation. Use externally at your own peril.
-        """
+    def __get_desc(Self) -> str:  # pragma: no cover
         if hasattr(Self, "long_name"):
             return Self.long_name
         elif hasattr(Self, "name"):
             return Self.name
         return Self.__name__
 
     @classmethod
-    def get_help_md(Self):
+    def get_help_md(Self, docstring_override: str = ""):  # pragma: no cover
         """
         Renders Markdown help for this step to a string.
         """
+        doc_string = docstring_override
+        if Self.__doc__:
+            doc_string = textwrap.dedent(Self.__doc__)
+
+        result = (
+            textwrap.dedent(
+                f"""\
+                ### <a name="{Self.id}"></a> {Self.__get_desc()}
+
+                ```{{eval-rst}}
+                %s
+                ```
+
+                #### Importing
+
+                ```python
+                from {Self.__module__} import {Self.__name__}
+
+                # or
+                
+                from openlane.steps import Step
+
+                {Self.__name__} = Step.factory.get("{Self.id}")
+                ```
+                """
+            )
+            % doc_string
+        )
+        if len(Self.inputs) + len(Self.outputs):
+            result += textwrap.dedent(
+                """
+                #### Inputs and Outputs
+
+                | Inputs | Outputs |
+                | - | - |
+                """
+            )
+            for input, output in zip_longest(Self.inputs, Self.outputs):
+                input_str = ""
+                if input is not None:
+                    input_str = f"{input.value.name} (.{input.value.extension})"
+
+                output_str = ""
+                if output is not None:
+                    if not isinstance(output, DesignFormat):
+                        raise StepException(
+                            f"Output '{output}' is not a valid DesignFormat enum object."
+                        )
+                    output_str = f"{output.value.name} (.{output.value.extension})"
+                result += f"| {input_str} | {output_str} |"
+
+        if len(Self.config_vars):
+            result += textwrap.dedent(
+                """
+                #### Configuration Variables
+
+                | Variable Name | Type | Description | Default | Units |
+                | - | - | - | - | - |
+                """
+            )
+            for var in Self.config_vars:
+                units = var.units or ""
+                result += f'| <a name="{Self.id}.{var.name}"></a>`{var.name}` | {var.type_repr_md()} | {var.desc_repr_md()} | `{var.default}` | {units} |\n'
 
-        result = textwrap.dedent(
-            f"""
-        ### {Self._get_desc()}
+        return result
+
+    @classmethod
+    def display_help(Self):  # pragma: no cover
+        """
+        IPython-only. Displays Markdown help for a given step.
+        """
+        import IPython.display
 
-        {Self.__doc__ or ""}
+        IPython.display.display(IPython.display.Markdown(Self.get_help_md()))
 
-        #### Importing
+    def _repr_markdown_(self) -> str:  # pragma: no cover
+        """
+        Only one _ because this is used by IPython.
+        """
+        if self.state_out is None:
+            return """
+                ### Step not yet executed.
+            """
+        state_in = self.state_in.result()
 
-        <br />
+        assert (
+            self.start_time is not None
+        ), "Start time not set even though self.state_out exists"
+        assert (
+            self.end_time is not None
+        ), "End time not set even though self.state_out exists"
+        result = ""
+        time_elapsed = self.end_time - self.start_time
 
-        ```python
-        from {Self.__module__} import {Self.__name__}
+        result += f"#### Time Elapsed: {'%.2f' % time_elapsed}s\n"
 
-        # or
-        
-        from openlane.steps import Step
+        views_updated = []
+        for id, value in dict(self.state_out).items():
+            if value is None:
+                continue
 
-        Synthesis = Step.get("{Self.id}")
-        ``` 
+            if state_in.get(id) != value:
+                df = DesignFormat.by_id(id)
+                assert df is not None
+                views_updated.append(df.value.name)
 
-        #### Configuration Variables
+        if len(views_updated):
+            result += "#### Views updated:\n"
+            for view in views_updated:
+                result += f"* {view}\n"
 
-        | Variable Name | Type | Description | Default | Units |
-        | - | - | - | - | - |
-        """
-        )
-        for var in Self.config_vars:
-            units = var.units or ""
-            result += f"| `{var.name}` | {var.type_repr_md()} | {var.desc_repr_md()} | `{var.default}` | {units} |\n"
+        if preview := self.layout_preview():
+            result += "#### Preview:\n"
+            result += preview
 
         return result
 
-    @classmethod
-    def display_help(Self):
+    def layout_preview(self) -> Optional[str]:  # pragma: no cover
         """
-        IPython-only. Displays Markdown help for a given step.
+        :returns: An HTML tag that could act as a preview for a specific stage
+            or ``None`` if a preview is unavailable for this step.
+        """
+        return None
+
+    def display_result(self):  # pragma: no cover
+        """
+        IPython-only. Displays the results of a given step.
         """
         import IPython.display
 
-        IPython.display.display(IPython.display.Markdown(Self.get_help_md()))
+        IPython.display.display(IPython.display.Markdown(self._repr_markdown_()))
 
     @final
     def start(
         self,
         toolbox: Optional[Toolbox] = None,
+        step_dir: Optional[str] = None,
         **kwargs,
     ) -> State:
         """
         Begins execution on a step.
 
         This method is final and should not be subclassed.
 
@@ -319,125 +482,171 @@
             redirect stdin, stdout, etc.
 
         :returns: An altered State object.
         """
         global LastState
 
         if toolbox is None:
-            if self.flow is not None:
-                if toolbox := self.flow.toolbox:
-                    self.toolbox = toolbox
-                else:
-                    raise StepException(
-                        "Attempted to 'start' a step before its parent Flow."
-                    )
-            elif not self.config.interactive:
+            if not Config.current_interactive:
                 raise TypeError(
                     "Missing argument 'toolbox' required when not running in a Flow"
                 )
             else:
                 # Use the default global value.
                 pass
         else:
             self.toolbox = toolbox
 
-        if isinstance(self.state_in, Future):
-            self.state_in = self.state_in.result()
+        if step_dir is None:
+            if not Config.current_interactive:
+                raise TypeError("Missing required argument 'step_dir'")
+            else:
+                self.step_dir = os.path.join(
+                    os.getcwd(),
+                    "openlane_run",
+                    f"{Step.counter}-{slugify(self.id)}",
+                )
+                Step.counter += 1
+        else:
+            self.step_dir = step_dir
+
+        state_in_result = self.state_in.result()
 
         rule(f"{self.long_name}")
 
-        if self.flow is not None and self.flow_control_variable is not None:
+        if not Config.current_interactive and self.flow_control_variable is not None:
             flow_control_value = self.config[self.flow_control_variable]
             if isinstance(flow_control_value, bool):
                 if not flow_control_value:
                     if self.flow_control_msg is not None:
                         info(self.flow_control_msg)
                     else:
                         info(
-                            f"'{self.flow_control_variable}' is set to False: skipping…"
+                            f"`{self.flow_control_variable}` is set to False: skipping {self.id} …"
                         )
-                        return self.state_in.copy()
+                        return state_in_result.copy()
             elif flow_control_value is None:
                 if self.flow_control_msg is not None:
                     info(self.flow_control_msg)
                 else:
                     info(
                         f"Required variable '{self.flow_control_variable}' is set to null: skipping…"
                     )
-                return self.state_in.copy()
+                return state_in_result.copy()
 
         mkdirp(self.step_dir)
         with open(os.path.join(self.step_dir, "state_in.json"), "w") as f:
-            f.write(self.state_in.dumps())
+            f.write(state_in_result.dumps())
 
         self.start_time = time.time()
-        self.state_out = self.run(**kwargs)
+
+        for input in self.inputs:
+            value = state_in_result[input]
+            if value is None:
+                raise StepException(
+                    f"{type(self).__name__}: missing required input '{input.name}'"
+                )
+
+        try:
+            views_updates, metrics_updates = self.run(state_in_result, **kwargs)
+        except subprocess.CalledProcessError as e:
+            if e.returncode is not None and e.returncode < 0:
+                raise StepSignalled(
+                    f"{self.name}: Interrupted ({Signals(-e.returncode).name})"
+                )
+            else:
+                raise StepError(f"{self.name}: subprocess {e.args} failed")
+
+        metrics = GenericImmutableDict(
+            state_in_result.metrics, overrides=metrics_updates
+        )
+
+        self.state_out = state_in_result.__class__(
+            state_in_result, overrides=views_updates, metrics=metrics
+        )
+
         try:
             self.state_out.validate()
         except InvalidState as e:
             raise StepException(f"Step {self.name} generated invalid state: {e}")
         self.end_time = time.time()
 
         with open(os.path.join(self.step_dir, "state_out.json"), "w") as f:
             f.write(self.state_out.dumps())
 
-        if self.config.interactive:
+        if Config.current_interactive:
             LastState = self.state_out
+
         return self.state_out
 
-    @internal
+    @protected
     @abstractmethod
-    def run(self, **kwargs) -> State:
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         """
         The "core" of a step.
 
-        When subclassing, override this function, then call it first thing
-        via super().run(**kwargs). This lets you use the input verification and
-        the State copying code, as well as resolving the `state_in` if `state_in`
-        is a future.
+        This step is considered per-object private, i.e., if a Step's run is
+        called anywhere outside of the same object's :meth:`start`, its behavior
+        is undefined.
 
-        :param **kwargs: Passed on to subprocess execution: useful if you want to
-            redirect stdin, stdout, etc.
-        """
+        :param state_in: The input state.
 
-        assert isinstance(self.state_in, State)
+            Note that ``self.state_in`` is stored as a future and would need to be
+            resolved before use first otherwise.
 
-        for input in self.inputs:
-            value = self.state_in.get(input)
-            if value is None:
-                raise MissingInputError(
-                    f"{type(self).__name__}: missing required input '{input.name}'"
-                )
+            For reference, ``start()`` is responsible for resolving it
+            for ``.run()``.
 
-        return self.state_in.copy()
+        :param **kwargs: Passed on to subprocess execution: useful if you want to
+            redirect stdin, stdout, etc.
+        """
+        pass
 
+    @protected
     def get_log_path(self) -> str:
+        """
+        :returns: the default value for :meth:`run_subprocess`'s "log_to"
+        parameter.
+
+            Override it to change the default log path.
+        """
         return os.path.join(self.step_dir, f"{slugify(self.id)}.log")
 
-    @internal
+    @protected
     def run_subprocess(
         self,
         cmd: Sequence[Union[str, os.PathLike]],
-        log_to: Optional[str] = None,
+        log_to: Optional[Union[str, os.PathLike]] = None,
+        silent: bool = False,
+        report_dir: Optional[Union[str, os.PathLike]] = None,
+        env: Optional[Dict[str, Any]] = None,
         **kwargs,
-    ):
+    ) -> Dict[str, Any]:
         """
-        A helper function for `Step` objects to run subprocesses.
+        A helper function for :class:`Step` objects to run subprocesses.
 
         The output from the subprocess is processed line-by-line.
 
         :param cmd: A list of variables, representing a program and its arguments,
             similar to how you would use it in a shell.
-        :param log_to: An optional override for the log path from `get_log_path`.
+        :param log_to: An optional override for the log path from :meth:`get_log_path`.
             Useful for if you run multiple subprocesses within one step.
+        :param silent: If specified, the subprocess does not print anything to
+            the terminal. Useful when running multiple processes simultaneously.
         :param **kwargs: Passed on to subprocess execution: useful if you want to
             redirect stdin, stdout, etc.
         :raises subprocess.CalledProcessError: If the process has a non-zero exit,
             this exception will be raised.
         """
+        if report_dir is None:
+            report_dir = self.step_dir
+        mkdirp(report_dir)
+
+        generated_metrics: Dict[str, Any] = {}
+
         log_path = log_to or self.get_log_path()
         log_file = open(log_path, "w")
         cmd_str = [str(arg) for arg in cmd]
 
         with open(os.path.join(self.step_dir, "COMMANDS"), "a+") as f:
             f.write(" ".join(cmd_str))
             f.write("\n")
@@ -445,51 +654,83 @@
         kwargs = kwargs.copy()
         if "stdin" not in kwargs:
             kwargs["stdin"] = open(os.devnull, "r")
         if "stdout" not in kwargs:
             kwargs["stdout"] = subprocess.PIPE
         if "stderr" not in kwargs:
             kwargs["stderr"] = subprocess.STDOUT
+
+        if env_dict := env:
+            for key, value in env_dict.items():
+                if not (
+                    isinstance(value, str)
+                    or isinstance(value, bytes)
+                    or isinstance(value, os.PathLike)
+                ):
+                    raise StepException(
+                        f"Environment variable for key '{key}' is of invalid type {type(value)}: {value}"
+                    )
         process = subprocess.Popen(
             cmd_str,
             encoding="utf8",
+            env=env,
             **kwargs,
         )
+        lines = ""
         if process_stdout := process.stdout:
             current_rpt = None
             while line := process_stdout.readline():
+                lines += line
+                log_file.write(line)
                 if self.step_dir is not None and line.startswith(REPORT_START_LOCUS):
+                    if current_rpt is not None:
+                        current_rpt.close()
                     report_name = line[len(REPORT_START_LOCUS) + 1 :].strip()
-                    report_path = os.path.join(self.step_dir, report_name)
+                    report_path = os.path.join(report_dir, report_name)
                     current_rpt = open(report_path, "w")
                 elif line.startswith(REPORT_END_LOCUS):
                     if current_rpt is not None:
                         current_rpt.close()
                     current_rpt = None
+                elif line.startswith(METRIC_LOCUS):
+                    command, name, value = line.split(" ", maxsplit=3)
+                    metric_type: Union[Type[str], Type[int], Type[float]] = str
+                    if command.endswith("_I"):
+                        metric_type = int
+                    elif command.endswith("_F"):
+                        metric_type = float
+                    generated_metrics[name] = metric_type(value)
                 elif current_rpt is not None:
+                    # No echo- the timing reports especially can be very large
+                    # and terminal emulators will slow the flow down.
                     current_rpt.write(line)
-                else:
+                elif not silent and "table template" not in line:  # sky130 ff hack
                     verbose(line.strip())
-                    log_file.write(line)
         returncode = process.wait()
+        split_lines = lines.split("\n")
         if returncode != 0:
+            if returncode > 0:
+                err("\n".join(split_lines[-10:]))
+                err(f"Log file: {log_path}")
             raise subprocess.CalledProcessError(returncode, process.args)
 
-    @internal
+        return generated_metrics
+
+    @protected
     def extract_env(self, kwargs) -> Tuple[dict, Dict[str, str]]:
         """
-        An assisting function: Given a `kwargs` object, it does the following:
+        An assisting function: Given a ``kwargs`` object, it does the following:
 
             * If the kwargs object has an "env" variable, it separates it into
                 its own variable.
             * If the kwargs object has no "env" variable, a new "env" dictionary
                 is created based on the current environment.
 
         :param kwargs: A Python keyword arguments object.
-        :returns (kwargs, env): A kwargs without an `env` object, and an isolated `env` object.
+        :returns (kwargs, env): A kwargs without an ``env`` object, and an isolated ``env`` object.
         """
         env = kwargs.get("env")
         if env is None:
             env = os.environ.copy()
         else:
             kwargs = kwargs.copy()
             del kwargs["env"]
@@ -500,87 +741,38 @@
         A factory singleton for Steps, allowing steps types to be registered and then
         retrieved by name.
 
         See https://en.wikipedia.org/wiki/Factory_(object-oriented_programming) for
         a primer.
         """
 
-        _registry: ClassVar[Dict[str, Type[Step]]] = {}
+        __registry: ClassVar[Dict[str, Type[Step]]] = {}
 
         @classmethod
         def register(Self) -> Callable[[Type[Step]], Type[Step]]:
             """
-            Adds a step type to the registry using its :mem:`Step.id` attribute.
+            Adds a step type to the registry using its :attr:`Step.id` attribute.
             """
 
             def decorator(cls: Type[Step]) -> Type[Step]:
-                Self._registry[cls.id] = cls
+                Self.__registry[cls.id.lower()] = cls
                 return cls
 
             return decorator
 
         @classmethod
         def get(Self, name: str) -> Optional[Type[Step]]:
             """
             Retrieves a Step type from the registry using a lookup string.
 
-            :param name: The registered name of the Step. Case-sensitive.
+            :param name: The registered name of the Step. Case-insensitive.
             """
-            return Self._registry.get(name)
+            return Self.__registry.get(name.lower())
 
         @classmethod
         def list(Self) -> List[str]:
             """
-            :returns: A list of strings representing Python names of all registered
-            steps.
+            :returns: A list of IDs of all registered names.
             """
-            return list(Self._registry.keys())
+            return [cls.id for cls in Self.__registry.values()]
 
     factory = StepFactory
-    get = StepFactory.get
-
-    def layout_preview(self) -> Optional[str]:
-        """
-        Returns an HTML tag that could act as a preview for a specific stage.
-        """
-        return None
-
-    def _repr_markdown_(self) -> str:
-        if self.state_out is None:
-            return """
-                ### Step not yet executed.
-            """
-        assert isinstance(self.state_in, State)
-        assert self.start_time is not None and self.end_time is not None
-
-        result = ""
-        time_elapsed = self.end_time - self.start_time
-
-        result += f"#### Time Elapsed: {'%.2f' % time_elapsed}s\n"
-
-        views_updated = []
-        for id, value in dict(self.state_out).items():
-            assert isinstance(id, str)
-            if value is None:
-                continue
-
-            if self.state_in.get(id) != value:
-                views_updated.append(DesignFormatByID[id].value[2])
-
-        if len(views_updated):
-            result += "#### Views updated:\n"
-            for view in views_updated:
-                result += f"* {view}\n"
-
-        if preview := self.layout_preview():
-            result += "#### Preview:\n"
-            result += preview
-
-        return result
-
-    def display_result(self):
-        """
-        IPython-only. Displays the results of a given step.
-        """
-        import IPython.display
-
-        IPython.display.display(IPython.display.Markdown(self._repr_markdown_()))
```

### Comparing `openlane-2.0.0a9/openlane/steps/tclstep.py` & `openlane-2.0.0b1/openlane/steps/tclstep.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,45 +8,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
+from abc import abstractmethod
 
 import os
 import re
+import json
 import glob
+import shlex
 import shutil
 import textwrap
 import subprocess
 from enum import Enum
 from decimal import Decimal
 from collections import deque
-from typing import List, Dict, Sequence, Union
+from dataclasses import is_dataclass, asdict
 from os.path import join, dirname, isdir, relpath
+from typing import Any, ClassVar, List, Dict, Sequence, Union, Tuple
 
-from .step import Step
-from ..state import State
-from ..config import Path
+from .step import ViewsUpdate, MetricsUpdate, Step, StepException
+
+from ..config import Keys
 from ..logging import info, warn
-from ..common import mkdirp, get_script_dir, get_openlane_root
+from ..state import State, DesignFormat
+from ..common import (
+    Path,
+    TclUtils,
+    GenericDictEncoder,
+    mkdirp,
+    get_script_dir,
+    get_openlane_root,
+    protected,
+)
 
 
 def create_reproducible(
+    design_dir: str,
     step_dir: str,
     cmd: Sequence[Union[str, os.PathLike]],
     env_in: Dict[str, str],
     tcl_script: str,
     verbose: bool = False,
 ) -> str:
+    design_dir = os.path.abspath(design_dir)
     step_dir = os.path.abspath(step_dir)
     run_path = os.path.dirname(step_dir)
     run_path_rel = os.path.relpath(run_path)
-    pdk_root = env_in["PDK_ROOT"]
+    pdk_root = env_in[Keys.pdk_root]
+    env_delta = {k: env_in[k] for k in env_in if k not in os.environ}
 
     info(
         textwrap.dedent(
             """\
             OpenLane TCLStep Issue Packager
 
             EFABLESS CORPORATION AND ALL AUTHORS OF THE OPENLANE PROJECT SHALL NOT BE HELD
@@ -107,15 +123,15 @@
 
     def shift(deque):
         try:
             return deque.popleft()
         except Exception:
             return None
 
-    env_keys_used = set(["PDK_ROOT"])
+    env_keys_used = set(env_delta.keys())
     tcls = set()
     env = env_in.copy()
     current = shift(tcls_to_process)
     loop_guard = 1024
     while current is not None:
         env_key = None
         if isinstance(current, tuple):
@@ -156,14 +172,16 @@
                         ".sdc"
                     ):
                         if value_substituted not in tcls:
                             tcls.add(value_substituted)
                             tcls_to_process.append(value_substituted)
         except FileNotFoundError:
             warnings.append(f"{current} was not found, might be a product. Skipping…")
+        except Exception as e:
+            warnings.append(f"{current} error. {e}")
 
         current = shift(tcls_to_process)
 
     # Phase 4: Copy The Files
     final_env = {}
 
     def copy(frm, to):
@@ -198,27 +216,28 @@
         except Exception as e:
             warnings.append(f"Couldn't copy {frm}: {e}. Skipped.")
 
     if verbose:
         info("\nProcessing environment variables…\n---")
 
     ol_root = get_openlane_root()
+    if verbose:
+        info(f"Resolving with OpenLane root: {ol_root}")
     loop_guard = 1024
     for key in env_keys_used:
         loop_guard -= 1
         if loop_guard == 0:
             raise Exception("An infinite loop has been detected. Please file an issue.")
         full_value = env[key]
         final_env[key] = ""
         if verbose:
             info(f"Processing {key}: {full_value}")
         for potential_file in full_value.split():
             potential_file_abspath = os.path.abspath(potential_file)
             if potential_file_abspath.startswith(run_path):
-                final_env[key] = ""
                 relative = relpath(potential_file, run_path)
                 final_value = join(".", relative)
                 final_path = join(destination_folder, final_value)
                 from_path = potential_file
                 if potential_file_abspath != step_dir:  # Otherwise, infinite recursion
                     copy(from_path, final_path)
                 final_env[key] += f"{final_value} "
@@ -226,14 +245,23 @@
                 if potential_file_abspath == pdk_root:  # Too many files to copy
                     continue
                 relative = relpath(potential_file, pdk_root)
                 final_value = join("pdk", relative)
                 final_path = join(destination_folder, final_value)
                 copy(potential_file, final_path)
                 final_env[key] += f"{final_value} "
+            elif potential_file_abspath.startswith(design_dir):
+                if potential_file_abspath == design_dir:  # Too many files
+                    continue
+                relative = relpath(potential_file, design_dir)
+                final_value = join("design", relative)
+                final_path = join(destination_folder, final_value)
+                from_path = potential_file
+                copy(from_path, final_path)
+                final_env[key] += f"{final_value} "
             elif potential_file_abspath.startswith(ol_root):
                 relative = relpath(potential_file, ol_root)
                 final_value = join("openlane", relative)
                 final_path = join(destination_folder, final_value)
 
                 from_path = potential_file
                 if potential_file_abspath != os.path.abspath(
@@ -242,15 +270,14 @@
                     copy(from_path, final_path)
                 final_env[key] += f"{final_value} "
             elif os.path.exists(potential_file) and not potential_file.startswith(
                 "/dev"
             ):  # /dev/null, /dev/stdout, /dev/stderr, etc should still work
                 final_path = join(destination_folder, potential_file)
                 final_value = os.path.relpath(final_path, destination_folder)
-                print(potential_file_abspath, final_path)
                 copy(potential_file, final_path)
                 final_env[key] += f"{final_value} "
             else:
                 final_env[key] += f"{potential_file} "
         final_env[key] = final_env[key].rstrip()
     if verbose:
         info("---\n")
@@ -262,27 +289,27 @@
     def env_list(
         format_string: str = "{key}={value}",
         env: Dict[str, str] = final_env,
         indent: int = 0,
     ) -> str:
         array = []
         for key, value in sorted(env.items()):
-            array.append(format_string.format(key=key, value=value))
+            array.append(format_string.format(key=key, value=shlex.quote(value)))
         value = f"\n{'    ' * indent}".join(array)
         return value
 
     run_shell = join(destination_folder, "run.sh")
     with open(run_shell, "w") as f:
         f.write(
             textwrap.dedent(
                 f"""\
                 #!/bin/sh
                 dir=$(cd -P -- "$(dirname -- "$0")" && pwd -P)
                 cd $dir;
-                {env_list("export {key}='{value}';", indent=4)}
+                {env_list("export {key}={value};", indent=4)}
                 {' '.join(new_cmd)}
                 """
             )
         )
     os.chmod(run_shell, 0o755)
 
     gdb_env = join(destination_folder, "env.gdb")
@@ -297,104 +324,194 @@
 
 
 class TclStep(Step):
     """
     A subclass of :class:`Step` that primarily deals with running Tcl-based utilities,
     such as Yosys, OpenROAD and Magic.
 
-    A TclStep Step corresponds to running one Tcl script with such a utility.
+    A TclStep Step should ideally correspond to running one Tcl script with such
+    a utility.
+
+    :cvar reproducibles_allowed: Whether this class can generate reproducibles.
     """
 
-    def get_script_path(self):
+    reproducibles_allowed: ClassVar[bool] = True
+
+    @staticmethod
+    def value_to_tcl(value: Any) -> str:
+        """
+        Converts an arbitrary Python value to Tcl as follows:
+
+        * If the value is an instance of a dataclass, it is serialized as a JSON object.
+        * If the value is a list, it is joined using :meth:`TclUtils.join`.
+        * If the value is a dict, the keys and values are escaped recursively using:
+            joined using :meth:`TclUtils.join`.
+        * If the value is an Enum, its name is returned.
+        * If the value is boolean, "1" is returned for True and "0" for False.
+        * If the value is numeric, it is converted to a string.
+        * Otherwise, the value is passed to ``str()``.
+        """
+        if is_dataclass(value):
+            return json.dumps(asdict(value), cls=GenericDictEncoder)
+        elif isinstance(value, list):
+            result = []
+            for item in value:
+                result.append(TclStep.value_to_tcl(item))
+            return TclUtils.join(result)
+        elif isinstance(value, dict):
+            result = []
+            for v_key, v_value in value.items():
+                result.append(TclStep.value_to_tcl(v_key))
+                result.append(TclStep.value_to_tcl(v_value))
+            return TclUtils.join(result)
+        elif isinstance(value, Enum):
+            return value.name
+        elif isinstance(value, bool):
+            return "1" if value else "0"
+        elif isinstance(value, Decimal) or isinstance(value, int):
+            return str(value)
+        else:
+            return str(value)
+
+    @protected
+    @abstractmethod
+    def get_script_path(self) -> str:
         """
-        :returns: A Tcl script to be run by this step.
+        :returns: A path to the Tcl script to be run by this step.
         """
-        return os.path.join(get_script_dir(), "tclsh", "hello.tcl")
+        pass
 
+    @protected
     def get_command(self) -> List[str]:
         """
-        :returns: The command used to run the script.
+        This command should be overridden by subclasses and replaced with a
+        command incorporating the  appropriate tool: e.g. ``openroad``,
+        ``yosys``, et cetera.
+
+        :returns: A list of strings representing the command used to run the script,
+            including the result of :meth:`get_script_path`.
         """
         return ["tclsh", self.get_script_path()]
 
-    def run(
-        self,
-        **kwargs,
-    ) -> State:
+    @protected
+    def prepare_env(self, env: dict, state: State) -> dict:
+        """
+        Creates a copy of an environment dictionary, then converts all accessible
+        ``self.config`` variables and state inputs to environment variables so
+        they may be used as inputs to the scripts.
+
+        Inputs are assigned the keys ``CURRENT_{ID}`` where ID is
+        the relevant :class:`DesignFormat`'s enum name.
+
+        Outputs are assigned the keys ``CURRENT_{ID}`` where ID is
+        the relevant :class:`DesignFormat`'s enum name, although outputs with
+        multiple values (SPEF, etc) will be skipped and a step is expected to
+        handle creating variables for them on its own.
+
+        The values are converted to strings as per :meth:`value_to_tcl`.
+
+        :param env: The input environment dictionary
+        :param state: The input state
+        :returns: a copy of the environment dictionary where ``self.config`` variables
+        """
+        env = env.copy()
+
+        env["SCRIPTS_DIR"] = get_script_dir()
+        env["STEP_DIR"] = os.path.abspath(self.step_dir)
+
+        tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
+        if len(tech_lefs) != 1:
+            raise StepException(
+                "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
+            )
+
+        env["TECH_LEF"] = tech_lefs[0]
+
+        macro_lefs = self.toolbox.get_macro_views(self.config, DesignFormat.LEF)
+        env["MACRO_LEFS"] = " ".join([str(lef) for lef in macro_lefs])
+
+        for element in self.config.keys():
+            value = self.config[element]
+            if value is None:
+                continue
+            env[element] = TclStep.value_to_tcl(value)
+
+        for input in self.inputs:
+            key = f"CURRENT_{input.name}"
+            env[key] = TclStep.value_to_tcl(state[input])
+
+        for output in self.outputs:
+            if output.value.multiple:
+                # Too step-specific.
+                continue
+            filename = f"{self.config['DESIGN_NAME']}.{output.value.extension}"
+            env[f"SAVE_{output.name}"] = os.path.join(self.step_dir, filename)
+
+        return env
+
+    @protected
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         """
         This overriden :meth:`run` function prepares configuration variables and
         inputs for use with Tcl: specifically, it converts them all to
         environment variables so they may be used by the Tcl scripts being called.
+        See :meth:`prepare_env` for more info.
 
         Additionally, it logs the output to a ``.log`` file named after the script.
 
         When overriding in a subclass, you may find it useful to use this pattern:
 
+        .. code-block:: python
+
             kwargs, env = self.extract_env(kwargs)
             env["CUSTOM_ENV_VARIABLE"] = "1"
-            return super().run(env=env, **kwargs)
+            return super().run(state_in, env=env, **kwargs)
 
         This will allow you to add further custom environment variables to a call
         while still respecting an `env` argument further up the call-stack.
 
-
+        :param state_in: See superclass.
         :param **kwargs: Passed on to subprocess execution: useful if you want to
             redirect stdin, stdout, etc.
+        :returns: see superclass
         """
-        state = super().run()
         command = self.get_command()
 
         kwargs, env = self.extract_env(kwargs)
 
-        env["SCRIPTS_DIR"] = get_script_dir()
-        env["STEP_DIR"] = os.path.abspath(self.step_dir)
-
-        for element in self.config.keys():
-            value = self.config[element]
-            if value is None:
-                continue
-
-            if isinstance(value, list):
-                value = " ".join(list(map(lambda x: str(x), value)))
-            elif isinstance(value, Enum):
-                value = value._name_
-            elif isinstance(value, bool):
-                value = "1" if value else "0"
-            elif isinstance(value, Decimal) or isinstance(value, int):
-                value = str(value)
-
-            env[element] = value
-
-        for input in self.inputs:
-            if input is None:
-                continue
-            env[f"CURRENT_{input.name}"] = str(state[input])
-
-        for output in self.outputs:
-            filename = f"{self.config['DESIGN_NAME']}.{output.value[1]}"
-            env[f"SAVE_{output.name}"] = os.path.join(self.step_dir, filename)
+        env = self.prepare_env(env, state_in)
 
         try:
-            self.run_subprocess(
+            generated_metrics = self.run_subprocess(
                 command,
                 env=env,
                 **kwargs,
             )
-        except subprocess.CalledProcessError:
-            reproducible_folder = create_reproducible(
-                self.step_dir,
-                command,
-                env,
-                self.get_script_path(),
-            )
-            info(
-                f"Reproducible created: please tarball and upload '{os.path.relpath(reproducible_folder)}' if you're going to file an issue."
-            )
+        except subprocess.CalledProcessError as e:
+            if (
+                e.returncode is not None
+                and e.returncode > 0
+                and self.reproducibles_allowed
+            ):
+                reproducible_folder = create_reproducible(
+                    self.config["DESIGN_DIR"],
+                    self.step_dir,
+                    command,
+                    env,
+                    self.get_script_path(),
+                )
+                info(
+                    f"Reproducible created: please tarball and upload '{os.path.relpath(reproducible_folder)}' if you're going to file an issue."
+                )
             raise
 
+        overrides: ViewsUpdate = {}
         for output in self.outputs:
+            if output.value.multiple:
+                # Too step-specific.
+                continue
             path = Path(env[f"SAVE_{output.name}"])
             if not path.exists():
                 continue
-            state[output] = path
+            overrides[output] = path
 
-        return state
+        return overrides, generated_metrics
```

### Comparing `openlane-2.0.0a9/openlane.egg-info/PKG-INFO` & `openlane-2.0.0b1/openlane.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0a9
+Version: 2.0.0b1
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > Efabless OpenLane 2 is in early access and all APIs are, presently, highly unstable and subject to change without notice.
         >
-        > If you don't know why you're here, you're probably looking for the stable version of OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
+        > If you *don't* know why you're here, you're probably looking for the stable version of OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
         
         <h1 align="center">OpenLane</h1>
         <p align="center">
             <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0"/></a>
             <a href="https://www.python.org"><img src="https://img.shields.io/badge/Python-3.8-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.8 or higher" /></a>
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style: black"/></a>
             <a href="https://mypy-lang.org/"><img src="https://www.mypy-lang.org/static/mypy_badge.svg" alt="Checked with mypy"/></a>
@@ -21,20 +21,22 @@
         <p align="center">
             <a href="https://openlane2.readthedocs.io/"><img src="https://readthedocs.org/projects/openlane2/badge/?version=latest" alt="Documentation Build Status Badge"/></a>
             <a href="https://invite.skywater.tools"><img src="https://img.shields.io/badge/Community-Open%20Source%20Silicon%20Slack-ff69b4?logo=slack" alt="Invite to the Open Source Silicon Slack"/></a>
         </p>
         
         OpenLane is a RTL to GDSII infrastructure library based on several components including OpenROAD, Yosys, Magic, Netgen, CVC, KLayout and a number of custom scripts for design exploration and optimization. A reference flow performs all ASIC implementation steps from RTL all the way down to GDSII.
         
+        You can find the documentation [here](https://openlane2.readthedocs.io/en/latest/getting_started/) to get started.
+        
         ```python
-        from openlane import Flow
+        from openlane.flows import Flow
         
-        Classic = Flow.get("Classic")
+        Classic = Flow.factory.get("Classic")
         
-        flow = Classic.init_with_config(
+        flow = Classic(
             {
                 "PDK": "sky130A",
                 "DESIGN_NAME": "spm",
                 "VERILOG_FILES": ["./src/spm.v"],
                 "CLOCK_PORT": "clk",
                 "CLOCK_PERIOD": 10,
             },
@@ -42,75 +44,73 @@
         )
         
         flow.start()
         ```
         
         
         ## Installation
-        ### Binary Dependencies
         You'll need the following:
         * Python **3.8** or higher with PIP, Venv and Tkinter
-        * Yosys 0.23+ (preferably 0.26+) from https://github.com/YosysHQ/Yosys
-        * A reasonably modern version of OpenROAD from https://github.com/The-OpenROAD-Project/OpenROAD
-        * A reasonably modern version of Magic from https://github.com/RTimothyEdwards/Magic
-        * A reasonably modern version of Netgen from https://github.com/RTimothyEdwards/netgen
-        * KLayout 0.28.5+ from https://github.com/KLayout/klayout
         
-        ### Docker
-        Works for Windows, macOS and Linux. Easier to set up, but less integrated with your filesystem. Recommended for general users.
+        ### Nix (Recommended)
+        Works for macOS and Linux (x86-64). Recommended, as it is more integrated with your filesystem and overall has less upload and download deltas.
         
-        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/docker_installation/index.html) in the docs.
+        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html) in the docs.
         
-        ### Nix
-        Works for macOS and Linux. A bit more complex to set up, but more integrated with your filesystem and overall less upload and download deltas.
+        ### Docker
+        Works for Windows, macOS and Linux (x86-64, aarch64 with emulation).
         
-        See [Nix-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/nix_installation/index.html) in the docs.
+        See [Docker-based installation](https://openlane2.readthedocs.io/en/latest/getting_started/docker_installation/index.html) in the docs.
         
-        ### Conda
-        TBA
+        Do note you'll need to add `--dockerized` right after `openlane` in most CLI invocations.
         
-        ### Python-only Installation
-        You'll need to bring your own compiled tools, but otherwise, simply install OpenLane as follows:
+        ### Python-only Installation (Advanced)
+        You'll need to bring your own compiled utilities, but otherwise, simply install OpenLane as follows:
         
         ```sh
         python3 -m pip install --upgrade openlane
         ```
         
-        To quickly test your installation, run `openlane --smoke-test`. This may take up to 10 minutes depending on your computer's speed and internet connection.
-        
-        #### Troubleshooting
-        With a typical Python 3.8 or higher installation with PIP, installing OpenLane is usually as simple as a `pip install`.
-        
-        ***Despite that***, there are some peculiarities with PIP itself: For example, you may see a warning among these lines:
+        ## Usage
+        In the root folder of the repository, you may invoke:
         
         ```sh
-          WARNING: The script openlane is installed in '/home/test/.local/bin' which is not on PATH.
-          Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+        python3 -m openlane --pdk-root <path/to/pdk> </path/to/config.json>
         ```
         
-        The solution is as simple as adding something like this to your shell's profile:
+        To start with, you can try:
         
         ```sh
-        export PATH="/home/test/.local/bin:$PATH"
+        python3 -m openlane --pdk-root $HOME/.volare ./designs/spm/config.json
         ```
         
-        Do note that the path (`/home/test/.local/bin` in this example) varies depending on your operating system and version of Python you install, and whether you use `sudo` (absolutely not recommended) or not, so ensure that you actually read the warning and add the correct path.
+        ## Publication
+        If you use OpenLane in your research, please cite the following paper.
         
-        ## Usage
-        In the root folder of the repository with the `venv` activated, you may invoke:
+        * M. Shalan and T. Edwards, “Building OpenLANE: A 130nm OpenROAD-based Tapeout-Proven Flow: Invited Paper,” *2020 IEEE/ACM International Conference On Computer Aided Design (ICCAD)*, San Diego, CA, USA, 2020, pp. 1-6. [Paper](https://ieeexplore.ieee.org/document/9256623)
         
-        ```sh
-        openlane --pdk-root <path/to/pdk> </path/to/config.json>
+        ```bibtex
+        @INPROCEEDINGS{9256623,
+          author={Shalan, Mohamed and Edwards, Tim},
+          booktitle={2020 IEEE/ACM International Conference On Computer Aided Design (ICCAD)}, 
+          title={Building OpenLANE: A 130nm OpenROAD-based Tapeout- Proven Flow : Invited Paper}, 
+          year={2020},
+          volume={},
+          number={},
+          pages={1-6},
+          doi={}}
         ```
         
-        To start with, you can try:
+        ## License
+        [The Apache License, version 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt).
         
-        ```sh
-        openlane --pdk-root $HOME/.volare ./designs/spm/config.json
-        ```
+        Docker images distributed by Efabless Corporation under the same license.
+        
+        Binaries bundled with OpenLane either via Cachix or Docker are distributed by
+        Efabless Corporation and may fall under stricter open source licenses.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,58 +1,53 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0a9 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0b1 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > Efabless OpenLane 2 is in early access and all APIs are,
 presently, highly unstable and subject to change without notice. > > If you
-don't know why you're here, you're probably looking for the stable version of
+*don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ****** OpenLane ******
 [License:_Apache_2.0] [Python_3.8_or_higher] [Code_Style:_black] [Checked_with
                             mypy] [Built_with_Nix]
  [Documentation_Build_Status_Badge] [Invite_to_the_Open_Source_Silicon_Slack]
 OpenLane is a RTL to GDSII infrastructure library based on several components
 including OpenROAD, Yosys, Magic, Netgen, CVC, KLayout and a number of custom
 scripts for design exploration and optimization. A reference flow performs all
-ASIC implementation steps from RTL all the way down to GDSII. ```python from
-openlane import Flow Classic = Flow.get("Classic") flow =
-Classic.init_with_config( { "PDK": "sky130A", "DESIGN_NAME": "spm",
-"VERILOG_FILES": ["./src/spm.v"], "CLOCK_PORT": "clk", "CLOCK_PERIOD": 10, },
-design_dir=".", ) flow.start() ``` ## Installation ### Binary Dependencies
+ASIC implementation steps from RTL all the way down to GDSII. You can find the
+documentation [here](https://openlane2.readthedocs.io/en/latest/
+getting_started/) to get started. ```python from openlane.flows import Flow
+Classic = Flow.factory.get("Classic") flow = Classic( { "PDK": "sky130A",
+"DESIGN_NAME": "spm", "VERILOG_FILES": ["./src/spm.v"], "CLOCK_PORT": "clk",
+"CLOCK_PERIOD": 10, }, design_dir=".", ) flow.start() ``` ## Installation
 You'll need the following: * Python **3.8** or higher with PIP, Venv and
-Tkinter * Yosys 0.23+ (preferably 0.26+) from https://github.com/YosysHQ/Yosys
-* A reasonably modern version of OpenROAD from https://github.com/The-OpenROAD-
-Project/OpenROAD * A reasonably modern version of Magic from https://
-github.com/RTimothyEdwards/Magic * A reasonably modern version of Netgen from
-https://github.com/RTimothyEdwards/netgen * KLayout 0.28.5+ from https://
-github.com/KLayout/klayout ### Docker Works for Windows, macOS and Linux.
-Easier to set up, but less integrated with your filesystem. Recommended for
-general users. See [Docker-based installation](https://
-openlane2.readthedocs.io/en/latest/getting_started/docker_installation/
-index.html) in the docs. ### Nix Works for macOS and Linux. A bit more complex
-to set up, but more integrated with your filesystem and overall less upload and
+Tkinter ### Nix (Recommended) Works for macOS and Linux (x86-64). Recommended,
+as it is more integrated with your filesystem and overall has less upload and
 download deltas. See [Nix-based installation](https://openlane2.readthedocs.io/
-en/latest/getting_started/nix_installation/index.html) in the docs. ### Conda
-TBA ### Python-only Installation You'll need to bring your own compiled tools,
-but otherwise, simply install OpenLane as follows: ```sh python3 -m pip install
---upgrade openlane ``` To quickly test your installation, run `openlane --
-smoke-test`. This may take up to 10 minutes depending on your computer's speed
-and internet connection. #### Troubleshooting With a typical Python 3.8 or
-higher installation with PIP, installing OpenLane is usually as simple as a
-`pip install`. ***Despite that***, there are some peculiarities with PIP
-itself: For example, you may see a warning among these lines: ```sh WARNING:
-The script openlane is installed in '/home/test/.local/bin' which is not on
-PATH. Consider adding this directory to PATH or, if you prefer to suppress this
-warning, use --no-warn-script-location. ``` The solution is as simple as adding
-something like this to your shell's profile: ```sh export PATH="/home/
-test/.local/bin:$PATH" ``` Do note that the path (`/home/test/.local/bin` in
-this example) varies depending on your operating system and version of Python
-you install, and whether you use `sudo` (absolutely not recommended) or not, so
-ensure that you actually read the warning and add the correct path. ## Usage In
-the root folder of the repository with the `venv` activated, you may invoke:
-```sh openlane --pdk-root
+en/latest/getting_started/nix_installation/index.html) in the docs. ### Docker
+Works for Windows, macOS and Linux (x86-64, aarch64 with emulation). See
+[Docker-based installation](https://openlane2.readthedocs.io/en/latest/
+getting_started/docker_installation/index.html) in the docs. Do note you'll
+need to add `--dockerized` right after `openlane` in most CLI invocations. ###
+Python-only Installation (Advanced) You'll need to bring your own compiled
+utilities, but otherwise, simply install OpenLane as follows: ```sh python3 -
+m pip install --upgrade openlane ``` ## Usage In the root folder of the
+repository, you may invoke: ```sh python3 -m openlane --pdk-root
 o/pdk>
-o/config.json> ``` To start with, you can try: ```sh openlane --pdk-root
-$HOME/.volare ./designs/spm/config.json ``` Platform: UNKNOWN Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python :: 3 Classifier: Intended Audience :: Developers Classifier:
-Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
-MacOS X Requires-Python: >3.8 Description-Content-Type: text/markdown
+o/config.json> ``` To start with, you can try: ```sh python3 -m openlane --pdk-
+root $HOME/.volare ./designs/spm/config.json ``` ## Publication If you use
+OpenLane in your research, please cite the following paper. * M. Shalan and T.
+Edwards, âBuilding OpenLANE: A 130nm OpenROAD-based Tapeout-Proven Flow:
+Invited Paper,â *2020 IEEE/ACM International Conference On Computer Aided
+Design (ICCAD)*, San Diego, CA, USA, 2020, pp. 1-6. [Paper](https://
+ieeexplore.ieee.org/document/9256623) ```bibtex @INPROCEEDINGS{9256623, author=
+{Shalan, Mohamed and Edwards, Tim}, booktitle={2020 IEEE/ACM International
+Conference On Computer Aided Design (ICCAD)}, title={Building OpenLANE: A 130nm
+OpenROAD-based Tapeout- Proven Flow : Invited Paper}, year={2020}, volume={},
+number={}, pages={1-6}, doi={}} ``` ## License [The Apache License, version
+2.0](https://www.apache.org/licenses/LICENSE-2.0.txt). Docker images
+distributed by Efabless Corporation under the same license. Binaries bundled
+with OpenLane either via Cachix or Docker are distributed by Efabless
+Corporation and may fall under stricter open source licenses. Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Intended Audience :: Developers
+Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
+MacOS :: MacOS X Requires-Python: >3.8 Description-Content-Type: text/markdown
```

### Comparing `openlane-2.0.0a9/openlane.egg-info/SOURCES.txt` & `openlane-2.0.0b1/openlane.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,92 @@
 setup.py
 openlane/__init__.py
 openlane/__main__.py
 openlane/__version__.py
-openlane/common.py
 openlane/container.py
 openlane/env_info.py
-openlane/logging.py
 openlane/open_pdks_rev
+openlane/plugins.py
 openlane.egg-info/PKG-INFO
 openlane.egg-info/SOURCES.txt
 openlane.egg-info/dependency_links.txt
 openlane.egg-info/entry_points.txt
 openlane.egg-info/requires.txt
 openlane.egg-info/top_level.txt
+openlane/common/__init__.py
+openlane/common/generic_dict.py
+openlane/common/metrics.py
+openlane/common/misc.py
+openlane/common/tcl.py
+openlane/common/test_common.py
+openlane/common/test_tcl.py
 openlane/config/__init__.py
-openlane/config/builder.py
 openlane/config/config.py
 openlane/config/flow.py
 openlane/config/pdk.py
-openlane/config/resolve.py
-openlane/config/tcleval.py
+openlane/config/preprocessor.py
+openlane/config/test_config.py
+openlane/config/test_pdk_migration.py
+openlane/config/test_preprocessor.py
+openlane/config/test_variable.py
 openlane/config/variable.py
 openlane/flows/__init__.py
 openlane/flows/builtins.py
 openlane/flows/classic.py
+openlane/flows/cli.py
 openlane/flows/flow.py
 openlane/flows/misc.py
 openlane/flows/optimizing.py
 openlane/flows/sequential.py
+openlane/flows/test_cli.py
+openlane/flows/test_flow.py
+openlane/flows/test_sequential.py
+openlane/logging/__init__.py
+openlane/logging/logger.py
 openlane/scripts/base.sdc
 openlane/scripts/klayout/Readme.md
 openlane/scripts/klayout/open_design.py
 openlane/scripts/klayout/render.py
 openlane/scripts/klayout/stream_out.py
 openlane/scripts/klayout/xor.drc
 openlane/scripts/magic/Readme.md
 openlane/scripts/magic/drc.tcl
 openlane/scripts/magic/extract_spice.tcl
+openlane/scripts/magic/lef.tcl
+openlane/scripts/magic/wrapper.tcl
 openlane/scripts/magic/def/antenna_check.tcl
 openlane/scripts/magic/def/mag.tcl
 openlane/scripts/magic/def/mag_gds.tcl
 openlane/scripts/magic/def/read.tcl
 openlane/scripts/magic/gds/drc_batch.tcl
 openlane/scripts/magic/gds/erase_box.tcl
 openlane/scripts/magic/gds/extras_mag.tcl
 openlane/scripts/magic/gds/mag_with_pointers.tcl
 openlane/scripts/magic/gds/read.tcl
 openlane/scripts/magic/lef/extras_maglef.tcl
 openlane/scripts/magic/lef/maglef.tcl
-openlane/scripts/magic/mag/lef.tcl
 openlane/scripts/odbpy/apply_def_template.py
 openlane/scripts/odbpy/contextualize.py
 openlane/scripts/odbpy/defutil.py
 openlane/scripts/odbpy/diodes.py
+openlane/scripts/odbpy/disconnected_pins.py
 openlane/scripts/odbpy/io_place.py
 openlane/scripts/odbpy/label_macro_pins.py
 openlane/scripts/odbpy/lefutil.py
 openlane/scripts/odbpy/manual_macro_place.py
 openlane/scripts/odbpy/padringer.py
 openlane/scripts/odbpy/power_utils.py
 openlane/scripts/odbpy/random_place.py
 openlane/scripts/odbpy/reader.py
 openlane/scripts/odbpy/remove_buffers.py
+openlane/scripts/odbpy/set_power_connections.py
 openlane/scripts/odbpy/snap_to_grid.py
 openlane/scripts/odbpy/wire_lengths.py
 openlane/scripts/openroad/basic_mp.tcl
-openlane/scripts/openroad/check_antennae.tcl
+openlane/scripts/openroad/check_antennas.tcl
 openlane/scripts/openroad/cts.tcl
 openlane/scripts/openroad/dpl.tcl
 openlane/scripts/openroad/drt.tcl
 openlane/scripts/openroad/fill.tcl
 openlane/scripts/openroad/floorplan.tcl
 openlane/scripts/openroad/gpl.tcl
 openlane/scripts/openroad/grt.tcl
@@ -78,45 +95,52 @@
 openlane/scripts/openroad/ioplacer.tcl
 openlane/scripts/openroad/irdrop.tcl
 openlane/scripts/openroad/pdn.tcl
 openlane/scripts/openroad/rcx.tcl
 openlane/scripts/openroad/repair_design.tcl
 openlane/scripts/openroad/rsz_timing_postcts.tcl
 openlane/scripts/openroad/rsz_timing_postgrt.tcl
-openlane/scripts/openroad/sta.tcl
-openlane/scripts/openroad/sta_multi_corner.tcl
 openlane/scripts/openroad/tapcell.tcl
 openlane/scripts/openroad/write_views.tcl
 openlane/scripts/openroad/common/dpl.tcl
 openlane/scripts/openroad/common/dpl_cell_pad.tcl
 openlane/scripts/openroad/common/grt.tcl
 openlane/scripts/openroad/common/io.tcl
 openlane/scripts/openroad/common/pdn_cfg.tcl
 openlane/scripts/openroad/common/resizer.tcl
 openlane/scripts/openroad/common/set_global_connections.tcl
 openlane/scripts/openroad/common/set_layer_adjustments.tcl
 openlane/scripts/openroad/common/set_power_nets.tcl
 openlane/scripts/openroad/common/set_rc.tcl
 openlane/scripts/openroad/common/set_routing_layers.tcl
+openlane/scripts/openroad/sta/corner.tcl
+openlane/scripts/openroad/sta/multi_corner.tcl.bk
 openlane/scripts/tclsh/hello.tcl
+openlane/scripts/yosys/common.tcl
+openlane/scripts/yosys/json_header.tcl
 openlane/scripts/yosys/synthesize.tcl
 openlane/smoke_test_design/config.json
 openlane/smoke_test_design/src/spm.v
 openlane/state/__init__.py
 openlane/state/design_format.py
 openlane/state/state.py
+openlane/state/test_state.py
 openlane/steps/__init__.py
 openlane/steps/checker.py
 openlane/steps/common_variables.py
 openlane/steps/klayout.py
 openlane/steps/magic.py
 openlane/steps/misc.py
 openlane/steps/netgen.py
 openlane/steps/odb.py
 openlane/steps/openroad.py
 openlane/steps/step.py
 openlane/steps/tclstep.py
+openlane/steps/test_step.py
+openlane/steps/test_tclstep.py
 openlane/steps/yosys.py
 openlane/utils/__init__.py
 openlane/utils/drc.py
 openlane/utils/memoize.py
+openlane/utils/test_toolbox.py
+openlane/utils/test_utils.py
 openlane/utils/toolbox.py
```

### Comparing `openlane-2.0.0a9/setup.py` & `openlane-2.0.0b1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #!/usr/bin/env python3
 import os
 import subprocess
 from setuptools import setup, find_packages
 
 
+module_name = "openlane"
+
 __dir__ = os.path.dirname(__file__)
 version = subprocess.check_output(
     [
         "python3",
-        f"{os.path.abspath(os.path.dirname(__file__))}/openlane/__version__.py",
+        os.path.join(
+            os.path.abspath(os.path.dirname(__file__)),
+            module_name,
+            "__version__.py",
+        ),
     ],
     encoding="utf8",
 )
 
 requirements = open("requirements.txt").read().strip().split("\n")
 setup(
-    name="openlane",
+    name=module_name,
     packages=find_packages(),
     package_data={
-        "openlane": [
+        module_name: [
             "py.typed",
             "open_pdks_rev",
             "scripts/*",
             "scripts/**/*",
             "scripts/**/**/*",
             "smoke_test_design/*",
             "smoke_test_design/**/*",
```

