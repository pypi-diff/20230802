# Comparing `tmp/cytosim-0.0.2.tar.gz` & `tmp/cytosim-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytosim-0.0.2.tar", last modified: Tue Aug  1 12:28:32 2023, max compression
+gzip compressed data, was "cytosim-0.0.3.tar", last modified: Wed Aug  2 09:53:45 2023, max compression
```

## Comparing `cytosim-0.0.2.tar` & `cytosim-0.0.3.tar`

### file list

```diff
@@ -1,978 +1,980 @@
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.268541 cytosim-0.0.2/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-01 11:52:34.000000 cytosim-0.0.2/.gitignore
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4328 2023-08-01 11:52:34.000000 cytosim-0.0.2/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-01 11:52:34.000000 cytosim-0.0.2/LICENSE.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-01 12:28:32.268541 cytosim-0.0.2/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-01 11:52:34.000000 cytosim-0.0.2/PYCYTOSIM.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-01 11:52:34.000000 cytosim-0.0.2/README.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-01 11:52:34.000000 cytosim-0.0.2/WARRANTY.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.208541 cytosim-0.0.2/cym/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      514 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/actin.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/amplify.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1218 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/arp23.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3330 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/ashbya.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      614 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_couple.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1127 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_custom.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1897 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_france.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      759 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_guided.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      884 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_pull3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      913 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_texas.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1108 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_tracker.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/axon.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1374 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/axon.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1399 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/baseball.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      897 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/bead.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/bipolar.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      858 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/buckling.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/buckling.cym.tpl
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/capture.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2274 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/capture_amplified.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      856 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/catastrophe_outside.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/celegans.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1385 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/change.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      563 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/change_confine.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      752 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/change_space.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      873 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/confine_instability.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      983 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_always.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1250 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_anchored.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_clamped.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1222 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_connect.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1135 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1857 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      891 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/couple.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3110 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/couple_fork.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1140 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/crushed_shell.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1107 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      922 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_fibers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      954 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_planar.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1233 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_saved.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3683 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cytokinesis.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      869 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cytoplasmic_flow.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1266 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/dogic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3225 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/endocytosis.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2103 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/endocytosis.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9924 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/entangled.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/event.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      945 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fast_diffusion1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      951 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fast_diffusion2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      353 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1203 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_anchor.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_athermal.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      837 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_bent.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      615 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_buckle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      998 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_classic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      834 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      625 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_forces.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1365 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_glue.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      601 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_grow.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1728 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_mixed.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1329 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_omega.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      847 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_treadmill.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      868 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/field.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      715 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/field_bind.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      637 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/field_cut.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      703 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fountain.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/frap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1277 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/friction.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      968 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1009 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_arcs.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_collect.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1680 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_drag.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1522 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_east.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1353 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_flip.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1959 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_flip_track.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1404 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_flippers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1770 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_gate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1126 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_path.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1334 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_ratchet.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1686 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_sort.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1898 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_sort_ortho.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1654 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_sorter.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1349 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_spiral.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_steric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1369 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_stripe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1245 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_surface.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      901 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_texas.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_trap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1547 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_west.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1624 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_west_blur.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1675 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_yingyang.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/granules.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1274 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_chew.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_cut.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_digit.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      828 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_move.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      861 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_nucleate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      984 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_rescue.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1330 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_slide.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_track.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2408 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3579 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/lacroix.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1053 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/magic_key.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      672 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/microtubule.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1760 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/minifilaments.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1850 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/minifilaments1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1605 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/minifilaments2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motif.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1554 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motif_blur.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1132 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motile_bead.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1145 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motor_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1006 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/move.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2376 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/muscle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      972 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/muscle_smooth.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/needles.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nematic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      663 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nucleate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      842 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nucleate_edge.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1106 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nucleus.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1249 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1411 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2044 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap3D_16.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1362 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      458 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/packed_beads.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      459 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/packed_beads_2D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1326 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/packed_gel.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1364 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/placement.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1356 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/pombe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1528 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/pombe_classic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1724 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/pombe_meiotic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1311 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/push_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1142 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/radial.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1124 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/ring_motors.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1066 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1012 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self_cortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      754 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self_vortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1086 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      764 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/side_movement.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      658 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/single.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/smiley.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1387 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/solid.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      499 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/solid_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      690 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/space_axisymmetric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      597 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/space_ellipse.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1122 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/sphere.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1097 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spider.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2417 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle3.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3712 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_celegans.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1601 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_centering.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1585 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_centering_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2199 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_compression.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3423 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_pombe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25433 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_pombe_em.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31549 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_pombe_em1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7568 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_yeast.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      676 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spiral.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      977 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spool.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1080 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      640 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_artefact.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bead_fiber_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      460 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bead_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      399 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bead_periodic2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      940 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bundle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1243 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bundling.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      667 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_cylinder.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      857 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      535 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      846 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      654 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_sphere.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1910 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_test.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      957 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/swimmers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      841 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_binding1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1077 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_binding2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1262 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_binding3.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      735 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_bindingP.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      439 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_fiber_diffusion.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      419 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_single_diffusion.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      550 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/texas.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/toy.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      906 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/toy_start.cmi
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      892 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/transport.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1035 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/triangle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1591 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/tug_of_war.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1485 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/walkers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1137 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/wash.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/yossi.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1407 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/zigzag.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.208541 cytosim-0.0.2/cytosim.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   336632 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/project.pbxproj
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.188541 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3081 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2846 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2828 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2876 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2377 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   210863 2023-08-01 11:52:34.000000 cytosim-0.0.2/demo_frame.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    81188 2023-08-01 11:52:34.000000 cytosim-0.0.2/demo_pycytosim.ipynb
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/code/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   106956 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/doxygen.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      652 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5727 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/layout.xml
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/mainpage.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4859 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/objects.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/compile/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4678 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/cygwin.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      931 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/dimensionality.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6519 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/intel_mkl.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      845 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/linux.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1663 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/multithreading.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1361 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/options.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2371 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/vectorization.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28284 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/cpython.css
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6251 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/cpython_doc.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   101654 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/doc_PyCytoplay.html
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100729 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/doc_PyCytosim.html
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9278 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/read_cpython.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   123267 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/data/cytosim.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29497 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/data/modularity.png
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/examples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6671 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/biblio.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/examples/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33685 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/actin.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42409 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/ashbya.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30331 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/celegans.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    60174 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/centering.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65951 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/droplets.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    50739 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/endocytosis.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    97182 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/minifilaments.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    77302 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/nematics.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100226 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/network.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5254 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/patterns.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   110273 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/spindle.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    51623 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/spindle_length.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16497 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/spombe.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2240 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1813 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/main/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/cheat.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/credits.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/examples.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5237 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/executables.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57247 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/faq.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1711 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/file_types.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3256 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/movies.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3969 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/overview.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5837 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/run_slurm.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7840 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/runs.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3784 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/starter.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4057 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/misc/Cytosim.tmbundle.zip
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/outreach/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1717 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/controller.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/outreach/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57904 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/CRI-2018-11a.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    39021 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/CRI-2018-11b.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   102453 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05a.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    61861 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05b.jpg
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/outreach/games/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/games/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      198 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6378 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/installation1.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5304 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/installation2.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/rendering/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)  1462588 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/actin.blend
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4264 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-actin-ico.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-actin-sphere.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-actin.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4413 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-links.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4086 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      292 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/remove-actin.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12156 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/commands.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2675 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/config.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/sim/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      928 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/forces.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6040 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/forces.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/meca_links.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3284 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      263 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric.tex
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21888 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric3D.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11926 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric_math.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65261 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/varying_time_step.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9082 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/fiber_dynamics.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1679 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/fibers.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1283 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/forces.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2513 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/graphics.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      611 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1527 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/motor_detachment.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3731 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/numerical_precision.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4246 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/objects.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       85 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/parameters.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8951 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/placement.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6988 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/report.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2687 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/spaces.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3458 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/steric.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3473 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/stochastic.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1882 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/units.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/tutorials/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/tutorials/code/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4790 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/config.cym.tpl
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      710 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/master.sh
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    15382 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/preconfig
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/scan.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/tutorials/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3334 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/ashbya.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      793 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1234 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/aster_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4119 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/capture.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19449 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/end_tracking.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28111 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/filament_buckling.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/gliding.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28234 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/polarity_sorting.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1010 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/self.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.224541 cytosim-0.0.2/doc/tutorials/images/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4591 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/H.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4483 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/XTV.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11568 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/aster-vs-nematic.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19716 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/bind_also_end.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    27299 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/bind_end.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20037 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/couples.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7406 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/crosslinks.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32919 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/droplets.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12570 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/force_velocity.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3561 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/gliding1.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3617 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/gliding2.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57401 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/kinesin_tetramers.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/meca_links.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10190 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/nematic-vs-polar.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      227 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_bipolarity.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3031 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_capture.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12562 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_centering.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7861 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_contract2.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5433 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_contract3.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7185 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_contract_motor.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5985 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_gliding.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23732 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_introduction.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      680 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_nucleus.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14458 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_polar_nematic.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      224 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_polarity.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7287 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_scans.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2543 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_scripting.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11632 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_self.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      356 2023-08-01 11:52:34.000000 cytosim-0.0.2/example.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.224541 cytosim-0.0.2/examples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      591 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/avoid.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2061 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/callbacks_pycytoplay.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      622 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/flock.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5745 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytoplay_callbacks.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   321969 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_construct.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   279239 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_extend.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   139505 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_flock.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6248 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_import3D.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   160711 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_meca.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4782 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_obj_3D.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   492525 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_objects.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-01 11:52:34.000000 cytosim-0.0.2/makefile
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-01 11:52:34.000000 cytosim-0.0.2/makefile.inc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.224541 cytosim-0.0.2/python/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/python/look/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/compare_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/get_data.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_image.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_movie.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_page.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_plots.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/read_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/scan.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/tell.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/python/misc/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/battery_test.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/cleanup.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/compare.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/plot.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/pyned.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/reduce.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/python/run/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/go_sim.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/go_sim_lib.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/preconfig.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/submit_one.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/submit_slurm.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-01 12:28:32.268541 cytosim-0.0.2/setup.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2281 2023-08-01 12:27:57.000000 cytosim-0.0.2/setup.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/src/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/CMakeLists.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/src/base/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/array.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/assert_macro.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/backtrace.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/backtrace.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/buddy.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/exceptions.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/exceptions.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filepath.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filepath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filewrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filewrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/glossary.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/glossary.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/inventoried.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/inventory.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/inventory.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/iowrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/iowrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/messages.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/messages.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/node_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/node_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/noder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/operator_new.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/print_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/print_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/stream_func.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/stream_func.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tictoc.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tictoc.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/timer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tokenizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tokenizer.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.232541 cytosim-0.0.2/src/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/couple_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/fiber_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/glossary_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/hand_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/interface_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/meca_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/object_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/organizer_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/point_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/python_frame.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3217 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/python_utilities.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/simul_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/single_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/solid_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/space_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/thread_modules.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.232541 cytosim-0.0.2/src/cytosim.egg-info/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22560 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-01 12:00:54.000000 cytosim-0.0.2/src/cytosim.egg-info/not-zip-safe
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       48 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/top_level.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.236541 cytosim-0.0.2/src/disp/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/fiber_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/fiber_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glapp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glu_unproject.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glut.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/grid_display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/grid_display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/line_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/line_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/miniz.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/miniz.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen_fbo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen_glx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/opengl.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/point_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/point_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/save_image.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/save_image.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/spng.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/spng.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.240541 cytosim-0.0.2/src/math/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-avx2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-params.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-params19937.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-sse2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/accumulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/allocator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/bicgstab.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/cblas.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/clapack.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/dgtsv.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/dim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/evaluator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/gmres.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/grid_base.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/isometry.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/linear_operator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix11.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix11.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix22.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix22.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix33.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix33.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix44.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrixbase.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesymblk.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesymblk.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/platonic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/pointsonsphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/pointsonsphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/project_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/project_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/quaternion.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random_vector.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random_vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/rasterizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/real.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/simd.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/simd_print.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/smath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vecprint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector4.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.240541 cytosim-0.0.2/src/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/check_dump.m
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.240541 cytosim-0.0.2/src/misc/installation/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/RtMidi.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/RtMidi.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/misc/installation/builder/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/0-live.command
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config0.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config1.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config2.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config3.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config4.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config5.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config6.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config7.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config8.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/cytobuilder.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/cytomaster.cpp
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/misc/installation/cytomaster.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/makefile
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/misc/installation/master/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/0-live.command
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config0.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config4.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config6.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config7.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config8.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config9.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/rtmidi_c.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/rtmidi_c.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/play/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play_keys.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play_menus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play_mouse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.256541 cytosim-0.0.2/src/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/chain.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/chain.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/common.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.256541 cytosim-0.0.2/src/sim/couples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/couple_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/couple_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_grid2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_segment.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_segment.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_site.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_site.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.256541 cytosim-0.0.2/src/sim/fibers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_values.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/frame_reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/frame_reader.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_monitor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.260541 cytosim-0.0.2/src/sim/hands/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interface.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interface.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation4.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/lattice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/lattice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca1d.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca_inter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil_project.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil_projectmat.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecapoint.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecapoint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/modulo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/modulo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/movable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/movable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.264541 cytosim-0.0.2/src/sim/organizers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/parser.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/parser.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/point_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/point_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim_thread.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_custom.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_file.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_step.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.264541 cytosim-0.0.2/src/sim/singles/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.264541 cytosim-0.0.2/src/sim/spaces/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_banana.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_banana.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_capsule.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_capsule.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinder.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderP.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderP.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_dice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_dice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_periodic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_periodic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygonZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygonZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ring.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ring.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_square.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_square.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_strip.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_strip.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_torus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_torus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/splash.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/splash.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.268541 cytosim-0.0.2/src/test/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_blas.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_code.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_cxx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_dispatch.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_gillespie.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glos.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glut.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glut3D.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_math.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_omp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_opengl.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_pipe.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_quaternion.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_signal.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_simd.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_sizeof.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_string.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_vbo.cc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.268541 cytosim-0.0.2/src/tools/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1215 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/cymart.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/frametool.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/pycytoplay.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/pycytosim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/pycytosim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/reportF.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/sieve.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.503219 cytosim-0.0.3/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-01 11:52:34.000000 cytosim-0.0.3/.gitignore
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4328 2023-08-01 11:52:34.000000 cytosim-0.0.3/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-01 11:52:34.000000 cytosim-0.0.3/LICENSE.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-02 09:53:45.503219 cytosim-0.0.3/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-01 11:52:34.000000 cytosim-0.0.3/PYCYTOSIM.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-01 11:52:34.000000 cytosim-0.0.3/README.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-01 11:52:34.000000 cytosim-0.0.3/WARRANTY.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/cym/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      514 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/actin.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/amplify.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1218 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/arp23.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3330 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/ashbya.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      614 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_couple.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1127 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_custom.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1897 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_france.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      759 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_guided.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      884 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_pull.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_pull3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      913 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_texas.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1108 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_tracker.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/axon.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1374 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/axon.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1399 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/baseball.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      897 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/bead.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/bipolar.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      858 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/buckling.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/buckling.cym.tpl
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/capture.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2274 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/capture_amplified.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      856 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/catastrophe_outside.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/celegans.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1385 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/change.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      563 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/change_confine.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      752 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/change_space.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      873 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/confine_instability.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      983 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_always.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1250 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_anchored.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_clamped.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1222 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_connect.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1135 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1857 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cortex.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      891 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/couple.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3110 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/couple_fork.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1140 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/crushed_shell.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1107 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_aster.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      922 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_fibers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      954 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_planar.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1233 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_saved.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3683 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cytokinesis.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      869 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cytoplasmic_flow.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1266 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/dogic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3225 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/endocytosis.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2103 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/endocytosis.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9924 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/entangled.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/event.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      945 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fast_diffusion1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      951 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fast_diffusion2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      353 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1203 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_anchor.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_athermal.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      837 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_bent.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      615 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_buckle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      998 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_classic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      834 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      625 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_forces.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1365 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_glue.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      601 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_grow.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1728 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_mixed.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1329 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_omega.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      847 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_treadmill.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      868 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/field.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      715 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/field_bind.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      637 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/field_cut.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      703 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fountain.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/frap.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1277 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/friction.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      968 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1009 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_arcs.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_collect.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1680 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_drag.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1522 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_east.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1353 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_flip.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1959 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_flip_track.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1404 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_flippers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1770 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_gate.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1126 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_path.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1334 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_ratchet.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1686 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_sort.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1898 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_sort_ortho.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1654 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_sorter.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1349 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_spiral.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_steric.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1369 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_stripe.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1245 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_surface.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      901 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_texas.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_trap.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1547 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_west.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1624 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_west_blur.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1675 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_yingyang.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/granules.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1274 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_chew.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_cut.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_digit.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      828 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_move.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      861 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_nucleate.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      984 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_rescue.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1330 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_slide.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_track.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2408 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_walk.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3579 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/lacroix.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1053 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/magic_key.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      672 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/microtubule.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1760 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/minifilaments.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1850 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/minifilaments1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1605 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/minifilaments2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motif.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1554 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motif_blur.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1132 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motile_bead.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1145 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motor_pull.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1006 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/move.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2376 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/muscle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      972 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/muscle_smooth.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/needles.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nematic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      663 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nucleate.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      842 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nucleate_edge.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1106 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nucleus.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1249 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1411 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2044 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap3D_16.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1362 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap_walk.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      458 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/packed_beads.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      459 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/packed_beads_2D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1326 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/packed_gel.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1364 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/placement.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1356 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/pombe.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1528 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/pombe_classic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1724 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/pombe_meiotic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1311 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/push_pull.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1142 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/radial.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1124 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/ring_motors.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1066 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1012 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self_cortex.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      754 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self_vortex.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1086 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self_walk.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      764 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/side_movement.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      658 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/single.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/smiley.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1387 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/solid.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      499 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/solid_3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      690 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/space_axisymmetric.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      597 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/space_ellipse.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1122 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/sphere.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1097 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spider.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2417 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle3.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3712 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_celegans.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1601 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_centering.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1585 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_centering_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2199 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_compression.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3423 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_pombe.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25433 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_pombe_em.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31549 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_pombe_em1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7568 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_yeast.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      676 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spiral.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      977 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spool.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1080 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      640 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_artefact.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bead_fiber_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      460 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bead_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      399 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bead_periodic2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      940 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bundle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1243 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bundling.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      667 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_cylinder.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      857 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      535 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      846 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber_3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      654 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_sphere.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1910 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_test.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      957 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/swimmers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      841 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_binding1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1077 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_binding2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1262 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_binding3.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      735 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_bindingP.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      439 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_fiber_diffusion.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      419 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_single_diffusion.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      550 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/texas.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/toy.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      906 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/toy_start.cmi
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      892 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/transport.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1035 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/triangle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1591 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/tug_of_war.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1485 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/walkers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1137 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/wash.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/yossi.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1407 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/zigzag.cym
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/cytosim.xcodeproj/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   336632 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/project.pbxproj
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.403219 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3081 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2846 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2828 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2876 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2377 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   210863 2023-08-01 11:52:34.000000 cytosim-0.0.3/demo_frame.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    81188 2023-08-01 11:52:34.000000 cytosim-0.0.3/demo_pycytosim.ipynb
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/code/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   106956 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/doxygen.cfg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      652 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5727 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/layout.xml
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/mainpage.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4859 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/objects.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/compile/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4678 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/cygwin.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      931 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/dimensionality.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6519 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/intel_mkl.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      845 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/linux.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1663 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/multithreading.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1361 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/options.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2371 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/vectorization.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/cpython/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28284 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/cpython.css
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6251 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/cpython_doc.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   101654 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/doc_PyCytoplay.html
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100729 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/doc_PyCytosim.html
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9278 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/read_cpython.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   123267 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/data/cytosim.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29497 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/data/modularity.png
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/examples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6671 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/biblio.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/examples/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33685 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/actin.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42409 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/ashbya.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30331 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/celegans.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    60174 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/centering.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65951 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/droplets.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    50739 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/endocytosis.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    97182 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/minifilaments.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    77302 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/nematics.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100226 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/network.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5254 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/patterns.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   110273 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/spindle.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    51623 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/spindle_length.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16497 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/spombe.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2240 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1813 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/main/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/cheat.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/credits.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/examples.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5237 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/executables.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57247 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/faq.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1711 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/file_types.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3256 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/movies.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3969 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/overview.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5837 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/run_slurm.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7840 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/runs.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3784 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/starter.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/misc/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4057 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/misc/Cytosim.tmbundle.zip
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/outreach/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1717 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/controller.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/outreach/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57904 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/CRI-2018-11a.jpg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    39021 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/CRI-2018-11b.jpg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   102453 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/Cambridge-2019-05a.jpg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    61861 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/Cambridge-2019-05b.jpg
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/outreach/games/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/games/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      198 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6378 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/installation1.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5304 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/installation2.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/rendering/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)  1462588 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/actin.blend
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4264 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-actin-ico.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-actin-sphere.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-actin.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4413 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-links.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4086 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      292 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/remove-actin.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.443219 cytosim-0.0.3/doc/sim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12156 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/commands.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2675 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/config.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.443219 cytosim-0.0.3/doc/sim/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      928 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/forces.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6040 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/forces.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/meca_links.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3284 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      263 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric.tex
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21888 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric3D.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11926 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric_math.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65261 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/varying_time_step.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9082 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/fiber_dynamics.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1679 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/fibers.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1283 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/forces.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2513 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/graphics.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      611 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1527 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/motor_detachment.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3731 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/numerical_precision.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4246 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/objects.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       85 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/parameters.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8951 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/placement.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6988 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/report.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2687 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/spaces.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3458 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/steric.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3473 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/stochastic.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1882 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/units.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.443219 cytosim-0.0.3/doc/tutorials/
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.447219 cytosim-0.0.3/doc/tutorials/code/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4790 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/collect.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/config.cym.tpl
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      710 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/master.sh
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    15382 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/preconfig
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/scan.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.447219 cytosim-0.0.3/doc/tutorials/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3334 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/ashbya.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      793 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/aster.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1234 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/aster_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4119 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/capture.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19449 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/end_tracking.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28111 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/filament_buckling.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/gliding.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28234 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/polarity_sorting.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1010 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/self.cym
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.447219 cytosim-0.0.3/doc/tutorials/images/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4591 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/H.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4483 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/XTV.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11568 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/aster-vs-nematic.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19716 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/bind_also_end.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    27299 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/bind_end.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20037 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/couples.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7406 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/crosslinks.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32919 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/droplets.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12570 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/force_velocity.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3561 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/gliding1.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3617 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/gliding2.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57401 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/kinesin_tetramers.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/meca_links.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10190 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/nematic-vs-polar.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      227 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_bipolarity.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3031 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_capture.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12562 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_centering.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7861 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_contract2.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5433 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_contract3.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7185 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_contract_motor.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5985 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_gliding.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23732 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_introduction.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      680 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_nucleus.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14458 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_polar_nematic.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      224 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_polarity.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7287 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_scans.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2543 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_scripting.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11632 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_self.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      356 2023-08-01 11:52:34.000000 cytosim-0.0.3/example.cym
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/examples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      591 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/avoid.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2061 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/callbacks_pycytoplay.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      622 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/flock.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5745 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytoplay_callbacks.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   321969 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_construct.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   279239 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_extend.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   139505 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_flock.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6248 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_import3D.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   160711 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_meca.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4782 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_obj_3D.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   492525 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_objects.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-01 11:52:34.000000 cytosim-0.0.3/makefile
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-01 11:52:34.000000 cytosim-0.0.3/makefile.inc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/python/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/python/look/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/collect.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/compare_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/get_data.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_image.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_movie.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_page.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_plots.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/read_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/scan.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/tell.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/python/misc/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/battery_test.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/cleanup.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/compare.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/plot.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/pyned.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/reduce.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.455219 cytosim-0.0.3/python/run/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/go_sim.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/go_sim_lib.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/preconfig.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/submit_one.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/submit_slurm.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-02 09:53:45.503219 cytosim-0.0.3/setup.cfg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2415 2023-08-02 09:52:25.000000 cytosim-0.0.3/setup.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.455219 cytosim-0.0.3/src/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-02 09:05:14.000000 cytosim-0.0.3/src/CMakeLists.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/base/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/array.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/assert_macro.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/backtrace.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/backtrace.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/buddy.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/exceptions.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/exceptions.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filepath.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filepath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filewrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filewrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/glossary.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/glossary.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/inventoried.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/inventory.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/inventory.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/iowrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/iowrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/messages.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/messages.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/node_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/node_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/noder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/operator_new.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/print_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/print_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/stream_func.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/stream_func.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tictoc.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tictoc.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/timer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tokenizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tokenizer.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/cpython/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/couple_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/fiber_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/glossary_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/hand_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/interface_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/meca_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/object_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/organizer_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/point_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/python_frame.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3217 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/python_utilities.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/simul_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/single_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/solid_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/space_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/thread_modules.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/cytosim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       23 2023-08-01 15:26:59.000000 cytosim-0.0.3/src/cytosim/__init__.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/cytosim.egg-info/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22584 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-01 12:00:54.000000 cytosim-0.0.3/src/cytosim.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        8 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/top_level.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.467219 cytosim-0.0.3/src/disp/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/fiber_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/fiber_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glapp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glu_unproject.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glut.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/grid_display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/grid_display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/line_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/line_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/miniz.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/miniz.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen_fbo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen_glx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/opengl.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/point_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/point_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/save_image.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/save_image.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/spng.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/spng.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/math/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-avx2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-params.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-params19937.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-sse2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/accumulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/allocator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/bicgstab.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/cblas.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/clapack.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/dgtsv.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/dim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/evaluator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/gmres.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/grid_base.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/isometry.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/linear_operator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix11.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix11.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix22.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix22.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix33.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix33.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix44.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrixbase.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesymblk.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesymblk.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/platonic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/pointsonsphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/pointsonsphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/project_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/project_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/quaternion.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random_vector.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random_vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/rasterizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/real.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/simd.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/simd_print.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/smath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vecprint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector4.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/check_dump.m
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/installation/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/RtMidi.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/RtMidi.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/installation/builder/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/0-live.command
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config0.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config1.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config2.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config3.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config4.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config5.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config6.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config7.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config8.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/cytobuilder.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/cytomaster.cpp
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/installation/cytomaster.xcodeproj/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/makefile
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.479219 cytosim-0.0.3/src/misc/installation/master/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/0-live.command
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config0.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config4.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config6.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config7.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config8.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config9.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/rtmidi_c.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/rtmidi_c.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.479219 cytosim-0.0.3/src/play/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play_keys.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play_menus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play_mouse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.491219 cytosim-0.0.3/src/sim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/chain.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/chain.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/common.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.491219 cytosim-0.0.3/src/sim/couples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/couple_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/couple_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_grid2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_segment.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_segment.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_site.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_site.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.491219 cytosim-0.0.3/src/sim/fibers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_values.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/frame_reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/frame_reader.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_monitor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.495219 cytosim-0.0.3/src/sim/hands/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interface.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interface.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation4.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/lattice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/lattice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca1d.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca_inter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil_project.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil_projectmat.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecapoint.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecapoint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/modulo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/modulo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/movable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/movable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.499219 cytosim-0.0.3/src/sim/organizers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/parser.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/parser.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/point_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/point_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim_thread.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_custom.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_file.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_step.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.499219 cytosim-0.0.3/src/sim/singles/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.499219 cytosim-0.0.3/src/sim/spaces/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_banana.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_banana.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_capsule.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_capsule.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinder.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderP.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderP.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_dice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_dice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_periodic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_periodic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygonZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygonZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ring.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ring.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_square.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_square.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_strip.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_strip.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_torus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_torus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/splash.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/splash.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.503219 cytosim-0.0.3/src/test/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_blas.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_code.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_cxx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_dispatch.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_gillespie.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glos.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glut.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glut3D.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_math.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_omp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_opengl.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_pipe.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_quaternion.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_signal.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_simd.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_sizeof.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_string.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_vbo.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.503219 cytosim-0.0.3/src/tools/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-02 09:32:07.000000 cytosim-0.0.3/src/tools/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/cymart.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/frametool.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/pycytoplay.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/pycytosim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/pycytosim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/reportF.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/sieve.cc
```

### Comparing `cytosim-0.0.2/.gitignore` & `cytosim-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/CMakeLists.txt` & `cytosim-0.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/LICENSE.txt` & `cytosim-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/PKG-INFO` & `cytosim-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
 Description-Content-Type: text/markdown
```

### Comparing `cytosim-0.0.2/PYCYTOSIM.md` & `cytosim-0.0.3/PYCYTOSIM.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/README.md` & `cytosim-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/WARRANTY.txt` & `cytosim-0.0.3/WARRANTY.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/actin.cym` & `cytosim-0.0.3/cym/actin.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/amplify.cym` & `cytosim-0.0.3/cym/amplify.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/arp23.cym` & `cytosim-0.0.3/cym/arp23.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/ashbya.cym` & `cytosim-0.0.3/cym/ashbya.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster.cym` & `cytosim-0.0.3/cym/aster.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_couple.cym` & `cytosim-0.0.3/cym/aster_couple.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_custom.cym` & `cytosim-0.0.3/cym/aster_custom.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_dynamic.cym` & `cytosim-0.0.3/cym/aster_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_france.cym` & `cytosim-0.0.3/cym/aster_france.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_guided.cym` & `cytosim-0.0.3/cym/aster_guided.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_pull.cym` & `cytosim-0.0.3/cym/aster_pull.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_pull3D.cym` & `cytosim-0.0.3/cym/aster_pull3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_texas.cym` & `cytosim-0.0.3/cym/aster_texas.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/aster_tracker.cym` & `cytosim-0.0.3/cym/aster_tracker.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/axon.cym` & `cytosim-0.0.3/cym/axon.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/axon.txt` & `cytosim-0.0.3/cym/axon.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/baseball.cym` & `cytosim-0.0.3/cym/baseball.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/bead.cym` & `cytosim-0.0.3/cym/bead.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/bipolar.cym` & `cytosim-0.0.3/cym/bipolar.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/buckling.cym` & `cytosim-0.0.3/cym/buckling.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/buckling.cym.tpl` & `cytosim-0.0.3/cym/buckling.cym.tpl`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/capture.cym` & `cytosim-0.0.3/cym/capture.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/capture_amplified.cym` & `cytosim-0.0.3/cym/capture_amplified.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/catastrophe_outside.cym` & `cytosim-0.0.3/cym/catastrophe_outside.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/celegans.cym` & `cytosim-0.0.3/cym/celegans.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/change.cym` & `cytosim-0.0.3/cym/change.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/change_confine.cym` & `cytosim-0.0.3/cym/change_confine.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/change_space.cym` & `cytosim-0.0.3/cym/change_space.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/confine_instability.cym` & `cytosim-0.0.3/cym/confine_instability.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/contract.cym` & `cytosim-0.0.3/cym/contract.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/contract_always.cym` & `cytosim-0.0.3/cym/contract_always.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/contract_anchored.cym` & `cytosim-0.0.3/cym/contract_anchored.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/contract_clamped.cym` & `cytosim-0.0.3/cym/contract_clamped.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/contract_connect.cym` & `cytosim-0.0.3/cym/contract_connect.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/contract_periodic.cym` & `cytosim-0.0.3/cym/contract_periodic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cortex.cym` & `cytosim-0.0.3/cym/cortex.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/couple.cym` & `cytosim-0.0.3/cym/couple.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/couple_fork.cym` & `cytosim-0.0.3/cym/couple_fork.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/crushed_shell.cym` & `cytosim-0.0.3/cym/crushed_shell.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cut_aster.cym` & `cytosim-0.0.3/cym/cut_aster.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cut_fibers.cym` & `cytosim-0.0.3/cym/cut_fibers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cut_planar.cym` & `cytosim-0.0.3/cym/cut_planar.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cut_saved.cym` & `cytosim-0.0.3/cym/cut_saved.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cytokinesis.txt` & `cytosim-0.0.3/cym/cytokinesis.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/cytoplasmic_flow.cym` & `cytosim-0.0.3/cym/cytoplasmic_flow.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/dogic.cym` & `cytosim-0.0.3/cym/dogic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/endocytosis.cym` & `cytosim-0.0.3/cym/endocytosis.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/endocytosis.txt` & `cytosim-0.0.3/cym/endocytosis.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/entangled.cym` & `cytosim-0.0.3/cym/entangled.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/event.cym` & `cytosim-0.0.3/cym/event.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fast_diffusion1.cym` & `cytosim-0.0.3/cym/fast_diffusion1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fast_diffusion2.cym` & `cytosim-0.0.3/cym/fast_diffusion2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_anchor.cym` & `cytosim-0.0.3/cym/fiber_anchor.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_athermal.cym` & `cytosim-0.0.3/cym/fiber_athermal.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_bent.cym` & `cytosim-0.0.3/cym/fiber_bent.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_buckle.cym` & `cytosim-0.0.3/cym/fiber_buckle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_classic.cym` & `cytosim-0.0.3/cym/fiber_classic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_dynamic.cym` & `cytosim-0.0.3/cym/fiber_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_forces.cym` & `cytosim-0.0.3/cym/fiber_forces.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_glue.cym` & `cytosim-0.0.3/cym/fiber_glue.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_grow.cym` & `cytosim-0.0.3/cym/fiber_grow.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_mixed.cym` & `cytosim-0.0.3/cym/fiber_mixed.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_omega.cym` & `cytosim-0.0.3/cym/fiber_omega.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fiber_treadmill.cym` & `cytosim-0.0.3/cym/fiber_treadmill.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/field.cym` & `cytosim-0.0.3/cym/field.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/field_bind.cym` & `cytosim-0.0.3/cym/field_bind.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/field_cut.cym` & `cytosim-0.0.3/cym/field_cut.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/fountain.cym` & `cytosim-0.0.3/cym/fountain.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/france.txt` & `cytosim-0.0.3/cym/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/frap.cym` & `cytosim-0.0.3/cym/frap.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/friction.cym` & `cytosim-0.0.3/cym/friction.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide.cym` & `cytosim-0.0.3/cym/glide.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_arcs.cym` & `cytosim-0.0.3/cym/glide_arcs.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_collect.cym` & `cytosim-0.0.3/cym/glide_collect.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_drag.cym` & `cytosim-0.0.3/cym/glide_drag.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_east.cym` & `cytosim-0.0.3/cym/glide_east.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_flip.cym` & `cytosim-0.0.3/cym/glide_flip.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_flip_track.cym` & `cytosim-0.0.3/cym/glide_flip_track.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_flippers.cym` & `cytosim-0.0.3/cym/glide_flippers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_gate.cym` & `cytosim-0.0.3/cym/glide_gate.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_path.cym` & `cytosim-0.0.3/cym/glide_path.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_ratchet.cym` & `cytosim-0.0.3/cym/glide_ratchet.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_sort.cym` & `cytosim-0.0.3/cym/glide_sort.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_sort_ortho.cym` & `cytosim-0.0.3/cym/glide_sort_ortho.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_sorter.cym` & `cytosim-0.0.3/cym/glide_sorter.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_spiral.cym` & `cytosim-0.0.3/cym/glide_spiral.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_steric.cym` & `cytosim-0.0.3/cym/glide_steric.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_stripe.cym` & `cytosim-0.0.3/cym/glide_stripe.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_surface.cym` & `cytosim-0.0.3/cym/glide_surface.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_texas.cym` & `cytosim-0.0.3/cym/glide_texas.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_trap.cym` & `cytosim-0.0.3/cym/glide_trap.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_west.cym` & `cytosim-0.0.3/cym/glide_west.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_west_blur.cym` & `cytosim-0.0.3/cym/glide_west_blur.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/glide_yingyang.cym` & `cytosim-0.0.3/cym/glide_yingyang.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/granules.cym` & `cytosim-0.0.3/cym/granules.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_chew.cym` & `cytosim-0.0.3/cym/hand_chew.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_cut.cym` & `cytosim-0.0.3/cym/hand_cut.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_digit.cym` & `cytosim-0.0.3/cym/hand_digit.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_move.cym` & `cytosim-0.0.3/cym/hand_move.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_nucleate.cym` & `cytosim-0.0.3/cym/hand_nucleate.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_rescue.cym` & `cytosim-0.0.3/cym/hand_rescue.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_slide.cym` & `cytosim-0.0.3/cym/hand_slide.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_track.cym` & `cytosim-0.0.3/cym/hand_track.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/hand_walk.cym` & `cytosim-0.0.3/cym/hand_walk.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/lacroix.cym` & `cytosim-0.0.3/cym/lacroix.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/magic_key.cym` & `cytosim-0.0.3/cym/magic_key.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/microtubule.cym` & `cytosim-0.0.3/cym/microtubule.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/minifilaments.cym` & `cytosim-0.0.3/cym/minifilaments.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/minifilaments1.cym` & `cytosim-0.0.3/cym/minifilaments1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/minifilaments2.cym` & `cytosim-0.0.3/cym/minifilaments2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/motif.cym` & `cytosim-0.0.3/cym/motif.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/motif_blur.cym` & `cytosim-0.0.3/cym/motif_blur.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/motile_bead.cym` & `cytosim-0.0.3/cym/motile_bead.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/motor_pull.cym` & `cytosim-0.0.3/cym/motor_pull.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/move.cym` & `cytosim-0.0.3/cym/move.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/muscle.cym` & `cytosim-0.0.3/cym/muscle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/muscle_smooth.cym` & `cytosim-0.0.3/cym/muscle_smooth.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/needles.cym` & `cytosim-0.0.3/cym/needles.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/nematic.cym` & `cytosim-0.0.3/cym/nematic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/nucleate.cym` & `cytosim-0.0.3/cym/nucleate.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/nucleate_edge.cym` & `cytosim-0.0.3/cym/nucleate_edge.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/nucleus.cym` & `cytosim-0.0.3/cym/nucleus.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/overlap.cym` & `cytosim-0.0.3/cym/overlap.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/overlap3D.cym` & `cytosim-0.0.3/cym/overlap3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/overlap3D_16.cym` & `cytosim-0.0.3/cym/overlap3D_16.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/overlap_walk.cym` & `cytosim-0.0.3/cym/overlap_walk.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/packed_gel.cym` & `cytosim-0.0.3/cym/packed_gel.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/placement.cym` & `cytosim-0.0.3/cym/placement.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/pombe.cym` & `cytosim-0.0.3/cym/pombe.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/pombe_classic.cym` & `cytosim-0.0.3/cym/pombe_classic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/pombe_meiotic.cym` & `cytosim-0.0.3/cym/pombe_meiotic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/push_pull.cym` & `cytosim-0.0.3/cym/push_pull.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/radial.cym` & `cytosim-0.0.3/cym/radial.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/ring_motors.cym` & `cytosim-0.0.3/cym/ring_motors.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/self.cym` & `cytosim-0.0.3/cym/self.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/self_cortex.cym` & `cytosim-0.0.3/cym/self_cortex.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/self_vortex.cym` & `cytosim-0.0.3/cym/self_vortex.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/self_walk.cym` & `cytosim-0.0.3/cym/self_walk.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/side_movement.cym` & `cytosim-0.0.3/cym/side_movement.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/single.cym` & `cytosim-0.0.3/cym/single.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/smiley.cym` & `cytosim-0.0.3/cym/smiley.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/solid.cym` & `cytosim-0.0.3/cym/solid.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/space_axisymmetric.cym` & `cytosim-0.0.3/cym/space_axisymmetric.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/space_ellipse.cym` & `cytosim-0.0.3/cym/space_ellipse.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/sphere.cym` & `cytosim-0.0.3/cym/sphere.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spider.cym` & `cytosim-0.0.3/cym/spider.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle3.cym` & `cytosim-0.0.3/cym/spindle3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_celegans.cym` & `cytosim-0.0.3/cym/spindle_celegans.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_centering.cym` & `cytosim-0.0.3/cym/spindle_centering.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_centering_dynamic.cym` & `cytosim-0.0.3/cym/spindle_centering_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_compression.cym` & `cytosim-0.0.3/cym/spindle_compression.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_pombe.cym` & `cytosim-0.0.3/cym/spindle_pombe.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_pombe_em.cym` & `cytosim-0.0.3/cym/spindle_pombe_em.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_pombe_em1.cym` & `cytosim-0.0.3/cym/spindle_pombe_em1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spindle_yeast.cym` & `cytosim-0.0.3/cym/spindle_yeast.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spiral.cym` & `cytosim-0.0.3/cym/spiral.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/spool.cym` & `cytosim-0.0.3/cym/spool.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric.cym` & `cytosim-0.0.3/cym/steric.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_3D.cym` & `cytosim-0.0.3/cym/steric_3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_artefact.cym` & `cytosim-0.0.3/cym/steric_artefact.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_bead_fiber_periodic.cym` & `cytosim-0.0.3/cym/steric_bead_fiber_periodic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_bundle.cym` & `cytosim-0.0.3/cym/steric_bundle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_bundling.cym` & `cytosim-0.0.3/cym/steric_bundling.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_cylinder.cym` & `cytosim-0.0.3/cym/steric_cylinder.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_fiber.cym` & `cytosim-0.0.3/cym/steric_fiber.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_fiber1.cym` & `cytosim-0.0.3/cym/steric_fiber1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_fiber_3D.cym` & `cytosim-0.0.3/cym/steric_fiber_3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_fiber_periodic.cym` & `cytosim-0.0.3/cym/steric_fiber_periodic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_sphere.cym` & `cytosim-0.0.3/cym/steric_sphere.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/steric_test.cym` & `cytosim-0.0.3/cym/steric_test.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/swimmers.cym` & `cytosim-0.0.3/cym/swimmers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/test_binding1.cym` & `cytosim-0.0.3/cym/test_binding1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/test_binding2.cym` & `cytosim-0.0.3/cym/test_binding2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/test_binding3.cym` & `cytosim-0.0.3/cym/test_binding3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/test_bindingP.cym` & `cytosim-0.0.3/cym/test_bindingP.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/texas.txt` & `cytosim-0.0.3/cym/texas.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/toy.cym` & `cytosim-0.0.3/cym/toy.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/toy_start.cmi` & `cytosim-0.0.3/cym/toy_start.cmi`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/transport.cym` & `cytosim-0.0.3/cym/transport.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/triangle.cym` & `cytosim-0.0.3/cym/triangle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/tug_of_war.cym` & `cytosim-0.0.3/cym/tug_of_war.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/walkers.cym` & `cytosim-0.0.3/cym/walkers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/wash.cym` & `cytosim-0.0.3/cym/wash.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/yossi.cym` & `cytosim-0.0.3/cym/yossi.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cym/zigzag.cym` & `cytosim-0.0.3/cym/zigzag.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/project.pbxproj` & `cytosim-0.0.3/cytosim.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme` & `cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/demo_frame.ipynb` & `cytosim-0.0.3/demo_frame.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/demo_pycytosim.ipynb` & `cytosim-0.0.3/demo_pycytosim.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/code/doxygen.cfg` & `cytosim-0.0.3/doc/code/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/code/index.md` & `cytosim-0.0.3/doc/code/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/code/layout.xml` & `cytosim-0.0.3/doc/code/layout.xml`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/code/mainpage.md` & `cytosim-0.0.3/doc/code/mainpage.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/code/objects.md` & `cytosim-0.0.3/doc/code/objects.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/cygwin.md` & `cytosim-0.0.3/doc/compile/cygwin.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/dimensionality.md` & `cytosim-0.0.3/doc/compile/dimensionality.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/index.md` & `cytosim-0.0.3/doc/compile/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/intel_mkl.md` & `cytosim-0.0.3/doc/compile/intel_mkl.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/linux.md` & `cytosim-0.0.3/doc/compile/linux.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/multithreading.md` & `cytosim-0.0.3/doc/compile/multithreading.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/options.md` & `cytosim-0.0.3/doc/compile/options.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/compile/vectorization.md` & `cytosim-0.0.3/doc/compile/vectorization.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/cpython/cpython.css` & `cytosim-0.0.3/doc/cpython/cpython.css`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/cpython/cpython_doc.py` & `cytosim-0.0.3/doc/cpython/cpython_doc.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/cpython/doc_PyCytoplay.html` & `cytosim-0.0.3/doc/cpython/doc_PyCytoplay.html`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/cpython/doc_PyCytosim.html` & `cytosim-0.0.3/doc/cpython/doc_PyCytosim.html`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/cpython/read_cpython.py` & `cytosim-0.0.3/doc/cpython/read_cpython.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/data/cytosim.png` & `cytosim-0.0.3/doc/data/cytosim.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/data/modularity.png` & `cytosim-0.0.3/doc/data/modularity.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/biblio.md` & `cytosim-0.0.3/doc/examples/biblio.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/actin.png` & `cytosim-0.0.3/doc/examples/data/actin.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/ashbya.png` & `cytosim-0.0.3/doc/examples/data/ashbya.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/celegans.png` & `cytosim-0.0.3/doc/examples/data/celegans.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/centering.png` & `cytosim-0.0.3/doc/examples/data/centering.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/droplets.png` & `cytosim-0.0.3/doc/examples/data/droplets.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/endocytosis.png` & `cytosim-0.0.3/doc/examples/data/endocytosis.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/minifilaments.png` & `cytosim-0.0.3/doc/examples/data/minifilaments.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/nematics.png` & `cytosim-0.0.3/doc/examples/data/nematics.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/network.png` & `cytosim-0.0.3/doc/examples/data/network.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/patterns.png` & `cytosim-0.0.3/doc/examples/data/patterns.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/spindle.png` & `cytosim-0.0.3/doc/examples/data/spindle.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/spindle_length.png` & `cytosim-0.0.3/doc/examples/data/spindle_length.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/data/spombe.png` & `cytosim-0.0.3/doc/examples/data/spombe.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/examples/index.md` & `cytosim-0.0.3/doc/examples/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/index.md` & `cytosim-0.0.3/doc/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/credits.md` & `cytosim-0.0.3/doc/main/credits.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/examples.md` & `cytosim-0.0.3/doc/main/examples.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/executables.md` & `cytosim-0.0.3/doc/main/executables.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/faq.md` & `cytosim-0.0.3/doc/main/faq.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/file_types.md` & `cytosim-0.0.3/doc/main/file_types.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/movies.md` & `cytosim-0.0.3/doc/main/movies.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/overview.md` & `cytosim-0.0.3/doc/main/overview.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/run_slurm.md` & `cytosim-0.0.3/doc/main/run_slurm.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/runs.md` & `cytosim-0.0.3/doc/main/runs.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/main/starter.md` & `cytosim-0.0.3/doc/main/starter.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/misc/Cytosim.tmbundle.zip` & `cytosim-0.0.3/doc/misc/Cytosim.tmbundle.zip`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/controller.md` & `cytosim-0.0.3/doc/outreach/controller.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/data/CRI-2018-11a.jpg` & `cytosim-0.0.3/doc/outreach/data/CRI-2018-11a.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/data/CRI-2018-11b.jpg` & `cytosim-0.0.3/doc/outreach/data/CRI-2018-11b.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05a.jpg` & `cytosim-0.0.3/doc/outreach/data/Cambridge-2019-05a.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05b.jpg` & `cytosim-0.0.3/doc/outreach/data/Cambridge-2019-05b.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/games/index.md` & `cytosim-0.0.3/doc/outreach/games/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/installation1.md` & `cytosim-0.0.3/doc/outreach/installation1.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/outreach/installation2.md` & `cytosim-0.0.3/doc/outreach/installation2.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/rendering/actin.blend` & `cytosim-0.0.3/doc/rendering/actin.blend`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/rendering/import-actin-ico.py` & `cytosim-0.0.3/doc/rendering/import-actin-ico.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/rendering/import-actin-sphere.py` & `cytosim-0.0.3/doc/rendering/import-actin-sphere.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/rendering/import-actin.py` & `cytosim-0.0.3/doc/rendering/import-actin.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/rendering/import-links.py` & `cytosim-0.0.3/doc/rendering/import-links.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/rendering/index.md` & `cytosim-0.0.3/doc/rendering/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/commands.md` & `cytosim-0.0.3/doc/sim/commands.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/config.md` & `cytosim-0.0.3/doc/sim/config.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/forces.cym` & `cytosim-0.0.3/doc/sim/data/forces.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/forces.png` & `cytosim-0.0.3/doc/sim/data/forces.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/meca_links.png` & `cytosim-0.0.3/doc/sim/data/meca_links.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/steric.png` & `cytosim-0.0.3/doc/sim/data/steric.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/steric3D.png` & `cytosim-0.0.3/doc/sim/data/steric3D.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/steric_math.png` & `cytosim-0.0.3/doc/sim/data/steric_math.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/data/varying_time_step.png` & `cytosim-0.0.3/doc/sim/data/varying_time_step.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/fiber_dynamics.md` & `cytosim-0.0.3/doc/sim/fiber_dynamics.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/fibers.md` & `cytosim-0.0.3/doc/sim/fibers.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/forces.md` & `cytosim-0.0.3/doc/sim/forces.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/graphics.md` & `cytosim-0.0.3/doc/sim/graphics.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/index.md` & `cytosim-0.0.3/doc/sim/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/motor_detachment.md` & `cytosim-0.0.3/doc/sim/motor_detachment.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/numerical_precision.md` & `cytosim-0.0.3/doc/sim/numerical_precision.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/objects.md` & `cytosim-0.0.3/doc/sim/objects.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/placement.md` & `cytosim-0.0.3/doc/sim/placement.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/report.md` & `cytosim-0.0.3/doc/sim/report.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/spaces.md` & `cytosim-0.0.3/doc/sim/spaces.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/steric.md` & `cytosim-0.0.3/doc/sim/steric.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/stochastic.md` & `cytosim-0.0.3/doc/sim/stochastic.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/sim/units.md` & `cytosim-0.0.3/doc/sim/units.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/code/collect.py` & `cytosim-0.0.3/doc/tutorials/code/collect.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/code/config.cym.tpl` & `cytosim-0.0.3/doc/tutorials/code/config.cym.tpl`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/code/master.sh` & `cytosim-0.0.3/doc/tutorials/code/master.sh`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/code/preconfig` & `cytosim-0.0.3/doc/tutorials/code/preconfig`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/code/scan.py` & `cytosim-0.0.3/doc/tutorials/code/scan.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/ashbya.cym` & `cytosim-0.0.3/doc/tutorials/data/ashbya.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/aster.cym` & `cytosim-0.0.3/doc/tutorials/data/aster.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/aster_dynamic.cym` & `cytosim-0.0.3/doc/tutorials/data/aster_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/capture.cym` & `cytosim-0.0.3/doc/tutorials/data/capture.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/end_tracking.png` & `cytosim-0.0.3/doc/tutorials/data/end_tracking.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/filament_buckling.png` & `cytosim-0.0.3/doc/tutorials/data/filament_buckling.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/gliding.cym` & `cytosim-0.0.3/doc/tutorials/data/gliding.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/polarity_sorting.png` & `cytosim-0.0.3/doc/tutorials/data/polarity_sorting.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/data/self.cym` & `cytosim-0.0.3/doc/tutorials/data/self.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/H.png` & `cytosim-0.0.3/doc/tutorials/images/H.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/XTV.png` & `cytosim-0.0.3/doc/tutorials/images/XTV.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/aster-vs-nematic.png` & `cytosim-0.0.3/doc/tutorials/images/aster-vs-nematic.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/bind_also_end.png` & `cytosim-0.0.3/doc/tutorials/images/bind_also_end.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/bind_end.png` & `cytosim-0.0.3/doc/tutorials/images/bind_end.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/couples.png` & `cytosim-0.0.3/doc/tutorials/images/couples.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/crosslinks.png` & `cytosim-0.0.3/doc/tutorials/images/crosslinks.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/droplets.png` & `cytosim-0.0.3/doc/tutorials/images/droplets.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/force_velocity.png` & `cytosim-0.0.3/doc/tutorials/images/force_velocity.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/gliding1.png` & `cytosim-0.0.3/doc/tutorials/images/gliding1.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/gliding2.png` & `cytosim-0.0.3/doc/tutorials/images/gliding2.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/kinesin_tetramers.png` & `cytosim-0.0.3/doc/tutorials/images/kinesin_tetramers.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/meca_links.png` & `cytosim-0.0.3/doc/tutorials/images/meca_links.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/images/nematic-vs-polar.png` & `cytosim-0.0.3/doc/tutorials/images/nematic-vs-polar.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/index.md` & `cytosim-0.0.3/doc/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_capture.md` & `cytosim-0.0.3/doc/tutorials/tuto_capture.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_centering.md` & `cytosim-0.0.3/doc/tutorials/tuto_centering.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_contract2.md` & `cytosim-0.0.3/doc/tutorials/tuto_contract2.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_contract3.md` & `cytosim-0.0.3/doc/tutorials/tuto_contract3.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_contract_motor.md` & `cytosim-0.0.3/doc/tutorials/tuto_contract_motor.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_gliding.md` & `cytosim-0.0.3/doc/tutorials/tuto_gliding.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_introduction.md` & `cytosim-0.0.3/doc/tutorials/tuto_introduction.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_nucleus.md` & `cytosim-0.0.3/doc/tutorials/tuto_nucleus.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_polar_nematic.md` & `cytosim-0.0.3/doc/tutorials/tuto_polar_nematic.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_scans.md` & `cytosim-0.0.3/doc/tutorials/tuto_scans.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_scripting.md` & `cytosim-0.0.3/doc/tutorials/tuto_scripting.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/doc/tutorials/tuto_self.md` & `cytosim-0.0.3/doc/tutorials/tuto_self.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/avoid.cym` & `cytosim-0.0.3/examples/avoid.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/callbacks_pycytoplay.py` & `cytosim-0.0.3/examples/callbacks_pycytoplay.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/flock.cym` & `cytosim-0.0.3/examples/flock.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytoplay_callbacks.ipynb` & `cytosim-0.0.3/examples/pycytoplay_callbacks.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_construct.ipynb` & `cytosim-0.0.3/examples/pycytosim_construct.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_extend.ipynb` & `cytosim-0.0.3/examples/pycytosim_extend.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_flock.ipynb` & `cytosim-0.0.3/examples/pycytosim_flock.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_import3D.ipynb` & `cytosim-0.0.3/examples/pycytosim_import3D.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_meca.ipynb` & `cytosim-0.0.3/examples/pycytosim_meca.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_obj_3D.ipynb` & `cytosim-0.0.3/examples/pycytosim_obj_3D.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/examples/pycytosim_objects.ipynb` & `cytosim-0.0.3/examples/pycytosim_objects.ipynb`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/makefile` & `cytosim-0.0.3/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/makefile.inc` & `cytosim-0.0.3/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/index.md` & `cytosim-0.0.3/python/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/collect.py` & `cytosim-0.0.3/python/look/collect.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/compare_config.py` & `cytosim-0.0.3/python/look/compare_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/get_data.py` & `cytosim-0.0.3/python/look/get_data.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/make_image.py` & `cytosim-0.0.3/python/look/make_image.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/make_movie.py` & `cytosim-0.0.3/python/look/make_movie.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/make_page.py` & `cytosim-0.0.3/python/look/make_page.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/make_plots.py` & `cytosim-0.0.3/python/look/make_plots.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/read_config.py` & `cytosim-0.0.3/python/look/read_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/scan.py` & `cytosim-0.0.3/python/look/scan.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/look/tell.py` & `cytosim-0.0.3/python/look/tell.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/misc/battery_test.py` & `cytosim-0.0.3/python/misc/battery_test.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/misc/cleanup.py` & `cytosim-0.0.3/python/misc/cleanup.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/misc/compare.py` & `cytosim-0.0.3/python/misc/compare.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/misc/plot.py` & `cytosim-0.0.3/python/misc/plot.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/misc/pyned.py` & `cytosim-0.0.3/python/misc/pyned.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/misc/reduce.py` & `cytosim-0.0.3/python/misc/reduce.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/run/go_sim.py` & `cytosim-0.0.3/python/run/go_sim.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/run/go_sim_lib.py` & `cytosim-0.0.3/python/run/go_sim_lib.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/run/preconfig.py` & `cytosim-0.0.3/python/run/preconfig.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/run/submit_one.py` & `cytosim-0.0.3/python/run/submit_one.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/python/run/submit_slurm.py` & `cytosim-0.0.3/python/run/submit_slurm.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/setup.py` & `cytosim-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 Cytosim is a simulation tool for cytoskeleton and polymers.
 """
 # setup.py stolen from mem3dg : https://github.com/RangamaniLabUCSD/Mem3DG
 import os
 import sys
 import subprocess
 import re
-version = "0.0.2"
+from pybind11.setup_helpers import Pybind11Extension
+version = "0.0.3"
 cmake_args=[]
 
 if('CONDA_PREFIX' in os.environ):
     print("Setting library search path (CMAKE_PREFIX_PATH): %s"%(os.environ['CONDA_PREFIX']))
     cmake_args.append('-DCMAKE_PREFIX_PATH=%s'%(os.environ['CONDA_PREFIX']))
 
 DOCLINES = __doc__.split("\n")
@@ -50,20 +51,23 @@
     name="cytosim",
     version=version,
     #packages=find_packages(where="python_src"),
     #package_dir={"": "python_src"},
     #cmake_install_dir="build",
     #include_package_data=True,
     #extras_require={"test": ["pytest"]},
-    #packages=find_packages(where="src/tools"),
+    packages=find_packages(where="src/"),
+    package_dir={"":"src"},
     #packages=find_packages(where="module"),
     #package_dir={"": "module"},
     #cmake_install_dir="module",
     description=DOCLINES[0],
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms=["Windows", "Linux", "Mac OS-X", "Unix"],
     #classifiers=[c for c in CLASSIFIERS.split("\n") if c],
     keywords="simulation actin microtubule polymer",
+    #packages=["cytosim"],
+    #ext_modules = ext_modules,
     cmake_args=cmake_args,
     zip_safe=False,
 )
```

### Comparing `cytosim-0.0.2/src/base/CMakeLists.txt` & `cytosim-0.0.3/src/base/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/array.h` & `cytosim-0.0.3/src/base/array.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/assert_macro.h` & `cytosim-0.0.3/src/base/assert_macro.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/backtrace.cc` & `cytosim-0.0.3/src/base/backtrace.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/backtrace.h` & `cytosim-0.0.3/src/base/backtrace.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/buddy.h` & `cytosim-0.0.3/src/base/buddy.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/exceptions.h` & `cytosim-0.0.3/src/base/exceptions.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/filepath.cc` & `cytosim-0.0.3/src/base/filepath.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/filepath.h` & `cytosim-0.0.3/src/base/filepath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/filewrapper.cc` & `cytosim-0.0.3/src/base/filewrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/filewrapper.h` & `cytosim-0.0.3/src/base/filewrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/glossary.cc` & `cytosim-0.0.3/src/base/glossary.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/glossary.h` & `cytosim-0.0.3/src/base/glossary.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/inventoried.h` & `cytosim-0.0.3/src/base/inventoried.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/inventory.cc` & `cytosim-0.0.3/src/base/inventory.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/inventory.h` & `cytosim-0.0.3/src/base/inventory.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/iowrapper.cc` & `cytosim-0.0.3/src/base/iowrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/iowrapper.h` & `cytosim-0.0.3/src/base/iowrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/makefile.inc` & `cytosim-0.0.3/src/base/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/messages.cc` & `cytosim-0.0.3/src/base/messages.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/messages.h` & `cytosim-0.0.3/src/base/messages.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/node_list.cc` & `cytosim-0.0.3/src/base/node_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/node_list.h` & `cytosim-0.0.3/src/base/node_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/noder.h` & `cytosim-0.0.3/src/base/noder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/operator_new.cc` & `cytosim-0.0.3/src/base/operator_new.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/print_color.cc` & `cytosim-0.0.3/src/base/print_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/print_color.h` & `cytosim-0.0.3/src/base/print_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/property.cc` & `cytosim-0.0.3/src/base/property.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/property.h` & `cytosim-0.0.3/src/base/property.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/property_list.cc` & `cytosim-0.0.3/src/base/property_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/property_list.h` & `cytosim-0.0.3/src/base/property_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/stream_func.cc` & `cytosim-0.0.3/src/base/stream_func.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/stream_func.h` & `cytosim-0.0.3/src/base/stream_func.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/tictoc.cc` & `cytosim-0.0.3/src/base/tictoc.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/tictoc.h` & `cytosim-0.0.3/src/base/tictoc.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/timer.h` & `cytosim-0.0.3/src/base/timer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/tokenizer.cc` & `cytosim-0.0.3/src/base/tokenizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/base/tokenizer.h` & `cytosim-0.0.3/src/base/tokenizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/couple_modules.h` & `cytosim-0.0.3/src/cpython/couple_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/fiber_modules.h` & `cytosim-0.0.3/src/cpython/fiber_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/glossary_modules.h` & `cytosim-0.0.3/src/cpython/glossary_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/hand_modules.h` & `cytosim-0.0.3/src/cpython/hand_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/interface_modules.h` & `cytosim-0.0.3/src/cpython/interface_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/meca_modules.h` & `cytosim-0.0.3/src/cpython/meca_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/object_modules.h` & `cytosim-0.0.3/src/cpython/object_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/organizer_modules.h` & `cytosim-0.0.3/src/cpython/organizer_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/point_modules.h` & `cytosim-0.0.3/src/cpython/point_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/python_frame.h` & `cytosim-0.0.3/src/cpython/python_frame.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/python_utilities.h` & `cytosim-0.0.3/src/cpython/python_utilities.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/simul_modules.h` & `cytosim-0.0.3/src/cpython/simul_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/single_modules.h` & `cytosim-0.0.3/src/cpython/single_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/solid_modules.h` & `cytosim-0.0.3/src/cpython/solid_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/space_modules.h` & `cytosim-0.0.3/src/cpython/space_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cpython/thread_modules.h` & `cytosim-0.0.3/src/cpython/thread_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/cytosim.egg-info/PKG-INFO` & `cytosim-0.0.3/src/cytosim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
 Description-Content-Type: text/markdown
```

### Comparing `cytosim-0.0.2/src/cytosim.egg-info/SOURCES.txt` & `cytosim-0.0.3/src/cytosim.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -430,14 +430,15 @@
 src/cpython/python_frame.h
 src/cpython/python_utilities.h
 src/cpython/simul_modules.h
 src/cpython/single_modules.h
 src/cpython/solid_modules.h
 src/cpython/space_modules.h
 src/cpython/thread_modules.h
+src/cytosim/__init__.py
 src/cytosim.egg-info/PKG-INFO
 src/cytosim.egg-info/SOURCES.txt
 src/cytosim.egg-info/dependency_links.txt
 src/cytosim.egg-info/not-zip-safe
 src/cytosim.egg-info/top_level.txt
 src/disp/CMakeLists.txt
 src/disp/display.cc
```

### Comparing `cytosim-0.0.2/src/disp/CMakeLists.txt` & `cytosim-0.0.3/src/disp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display.cc` & `cytosim-0.0.3/src/disp/display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display.h` & `cytosim-0.0.3/src/disp/display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display1.cc` & `cytosim-0.0.3/src/disp/display1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display1.h` & `cytosim-0.0.3/src/disp/display1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display2.cc` & `cytosim-0.0.3/src/disp/display2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display2.h` & `cytosim-0.0.3/src/disp/display2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display3.cc` & `cytosim-0.0.3/src/disp/display3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display3.h` & `cytosim-0.0.3/src/disp/display3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display_prop.cc` & `cytosim-0.0.3/src/disp/display_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/display_prop.h` & `cytosim-0.0.3/src/disp/display_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/fiber_disp.cc` & `cytosim-0.0.3/src/disp/fiber_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/fiber_disp.h` & `cytosim-0.0.3/src/disp/fiber_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/glapp.cc` & `cytosim-0.0.3/src/disp/glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/glapp.h` & `cytosim-0.0.3/src/disp/glapp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/gle.cc` & `cytosim-0.0.3/src/disp/gle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/gle.h` & `cytosim-0.0.3/src/disp/gle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/gle_color.cc` & `cytosim-0.0.3/src/disp/gle_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/gle_color.h` & `cytosim-0.0.3/src/disp/gle_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/gle_color_list.cc` & `cytosim-0.0.3/src/disp/gle_color_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/gle_color_list.h` & `cytosim-0.0.3/src/disp/gle_color_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/glu_unproject.cc` & `cytosim-0.0.3/src/disp/glu_unproject.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/grid_display.cc` & `cytosim-0.0.3/src/disp/grid_display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/grid_display.h` & `cytosim-0.0.3/src/disp/grid_display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/line_disp.h` & `cytosim-0.0.3/src/disp/line_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/makefile.inc` & `cytosim-0.0.3/src/disp/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/miniz.c` & `cytosim-0.0.3/src/disp/miniz.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/miniz.h` & `cytosim-0.0.3/src/disp/miniz.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/offscreen.cc` & `cytosim-0.0.3/src/disp/offscreen.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/offscreen.h` & `cytosim-0.0.3/src/disp/offscreen.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/offscreen_fbo.cc` & `cytosim-0.0.3/src/disp/offscreen_fbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/offscreen_glx.cc` & `cytosim-0.0.3/src/disp/offscreen_glx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/point_disp.cc` & `cytosim-0.0.3/src/disp/point_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/point_disp.h` & `cytosim-0.0.3/src/disp/point_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/save_image.cc` & `cytosim-0.0.3/src/disp/save_image.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/save_image.h` & `cytosim-0.0.3/src/disp/save_image.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/spng.c` & `cytosim-0.0.3/src/disp/spng.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/spng.h` & `cytosim-0.0.3/src/disp/spng.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/view.cc` & `cytosim-0.0.3/src/disp/view.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/view.h` & `cytosim-0.0.3/src/disp/view.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/view_prop.cc` & `cytosim-0.0.3/src/disp/view_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/disp/view_prop.h` & `cytosim-0.0.3/src/disp/view_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/index.md` & `cytosim-0.0.3/src/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/CMakeLists.txt` & `cytosim-0.0.3/src/math/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT-avx2.h` & `cytosim-0.0.3/src/math/SFMT-avx2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT-common.h` & `cytosim-0.0.3/src/math/SFMT-common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT-params.h` & `cytosim-0.0.3/src/math/SFMT-params.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT-params19937.h` & `cytosim-0.0.3/src/math/SFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT-sse2.h` & `cytosim-0.0.3/src/math/SFMT-sse2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT.c` & `cytosim-0.0.3/src/math/SFMT.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/SFMT.h` & `cytosim-0.0.3/src/math/SFMT.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/accumulator.h` & `cytosim-0.0.3/src/math/accumulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/allocator.h` & `cytosim-0.0.3/src/math/allocator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/bicgstab.h` & `cytosim-0.0.3/src/math/bicgstab.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/cblas.h` & `cytosim-0.0.3/src/math/cblas.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/clapack.h` & `cytosim-0.0.3/src/math/clapack.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/dgtsv.c` & `cytosim-0.0.3/src/math/dgtsv.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/evaluator.h` & `cytosim-0.0.3/src/math/evaluator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/gmres.h` & `cytosim-0.0.3/src/math/gmres.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/grid.h` & `cytosim-0.0.3/src/math/grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/grid_base.h` & `cytosim-0.0.3/src/math/grid_base.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/isometry.h` & `cytosim-0.0.3/src/math/isometry.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/linear_operator.h` & `cytosim-0.0.3/src/math/linear_operator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/makefile.inc` & `cytosim-0.0.3/src/math/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix.cc` & `cytosim-0.0.3/src/math/matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix.h` & `cytosim-0.0.3/src/math/matrix.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix11.cc` & `cytosim-0.0.3/src/math/matrix11.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix11.h` & `cytosim-0.0.3/src/math/matrix11.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix22.cc` & `cytosim-0.0.3/src/math/matrix22.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix22.h` & `cytosim-0.0.3/src/math/matrix22.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix33.cc` & `cytosim-0.0.3/src/math/matrix33.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix33.h` & `cytosim-0.0.3/src/math/matrix33.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrix44.h` & `cytosim-0.0.3/src/math/matrix44.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matrixbase.h` & `cytosim-0.0.3/src/math/matrixbase.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparse.cc` & `cytosim-0.0.3/src/math/matsparse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparse.h` & `cytosim-0.0.3/src/math/matsparse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesym.cc` & `cytosim-0.0.3/src/math/matsparsesym.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesym.h` & `cytosim-0.0.3/src/math/matsparsesym.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesym1.cc` & `cytosim-0.0.3/src/math/matsparsesym1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesym1.h` & `cytosim-0.0.3/src/math/matsparsesym1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesym2.cc` & `cytosim-0.0.3/src/math/matsparsesym2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesym2.h` & `cytosim-0.0.3/src/math/matsparsesym2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesymblk.cc` & `cytosim-0.0.3/src/math/matsparsesymblk.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/matsparsesymblk.h` & `cytosim-0.0.3/src/math/matsparsesymblk.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/monitor.h` & `cytosim-0.0.3/src/math/monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/platonic.cc` & `cytosim-0.0.3/src/math/platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/platonic.h` & `cytosim-0.0.3/src/math/platonic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/pointsonsphere.cc` & `cytosim-0.0.3/src/math/pointsonsphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/pointsonsphere.h` & `cytosim-0.0.3/src/math/pointsonsphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/polygon.cc` & `cytosim-0.0.3/src/math/polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/polygon.h` & `cytosim-0.0.3/src/math/polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/project_ellipse.cc` & `cytosim-0.0.3/src/math/project_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/project_ellipse.h` & `cytosim-0.0.3/src/math/project_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/quaternion.h` & `cytosim-0.0.3/src/math/quaternion.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/random.cc` & `cytosim-0.0.3/src/math/random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/random.h` & `cytosim-0.0.3/src/math/random.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/random_vector.cc` & `cytosim-0.0.3/src/math/random_vector.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/random_vector.h` & `cytosim-0.0.3/src/math/random_vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/rasterizer.cc` & `cytosim-0.0.3/src/math/rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/rasterizer.h` & `cytosim-0.0.3/src/math/rasterizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/real.h` & `cytosim-0.0.3/src/math/real.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/simd.h` & `cytosim-0.0.3/src/math/simd.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/simd_print.h` & `cytosim-0.0.3/src/math/simd_print.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/smath.h` & `cytosim-0.0.3/src/math/smath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vecprint.h` & `cytosim-0.0.3/src/math/vecprint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector.h` & `cytosim-0.0.3/src/math/vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector1.cc` & `cytosim-0.0.3/src/math/vector1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector1.h` & `cytosim-0.0.3/src/math/vector1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector2.cc` & `cytosim-0.0.3/src/math/vector2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector2.h` & `cytosim-0.0.3/src/math/vector2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector3.cc` & `cytosim-0.0.3/src/math/vector3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector3.h` & `cytosim-0.0.3/src/math/vector3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector4.cc` & `cytosim-0.0.3/src/math/vector4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/math/vector4.h` & `cytosim-0.0.3/src/math/vector4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/check_dump.m` & `cytosim-0.0.3/src/misc/check_dump.m`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/RtMidi.cpp` & `cytosim-0.0.3/src/misc/installation/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/RtMidi.h` & `cytosim-0.0.3/src/misc/installation/RtMidi.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/0-live.command` & `cytosim-0.0.3/src/misc/installation/builder/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config.cym` & `cytosim-0.0.3/src/misc/installation/builder/config.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config0.cym` & `cytosim-0.0.3/src/misc/installation/builder/config0.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config1.cym` & `cytosim-0.0.3/src/misc/installation/builder/config1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config2.cym` & `cytosim-0.0.3/src/misc/installation/builder/config2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config3.cym` & `cytosim-0.0.3/src/misc/installation/builder/config3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config4.cym` & `cytosim-0.0.3/src/misc/installation/builder/config4.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config5.cym` & `cytosim-0.0.3/src/misc/installation/builder/config5.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config6.cym` & `cytosim-0.0.3/src/misc/installation/builder/config6.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config7.cym` & `cytosim-0.0.3/src/misc/installation/builder/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/config8.cym` & `cytosim-0.0.3/src/misc/installation/builder/config8.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/builder/france.txt` & `cytosim-0.0.3/src/misc/installation/builder/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/cytobuilder.cpp` & `cytosim-0.0.3/src/misc/installation/cytobuilder.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/cytomaster.cpp` & `cytosim-0.0.3/src/misc/installation/cytomaster.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/cytomaster.xcodeproj/project.pbxproj` & `cytosim-0.0.3/src/misc/installation/cytomaster.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/makefile` & `cytosim-0.0.3/src/misc/installation/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/0-live.command` & `cytosim-0.0.3/src/misc/installation/master/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config0.cym` & `cytosim-0.0.3/src/misc/installation/master/config0.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config1.cym` & `cytosim-0.0.3/src/misc/installation/master/config1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config2.cym` & `cytosim-0.0.3/src/misc/installation/master/config2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config4.cym` & `cytosim-0.0.3/src/misc/installation/master/config4.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config6.cym` & `cytosim-0.0.3/src/misc/installation/master/config6.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config7.cym` & `cytosim-0.0.3/src/misc/installation/master/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config8.cym` & `cytosim-0.0.3/src/misc/installation/master/config8.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/config9.cym` & `cytosim-0.0.3/src/misc/installation/master/config9.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/master/france.txt` & `cytosim-0.0.3/src/misc/installation/master/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/rtmidi_c.cpp` & `cytosim-0.0.3/src/misc/installation/rtmidi_c.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/misc/installation/rtmidi_c.h` & `cytosim-0.0.3/src/misc/installation/rtmidi_c.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/CMakeLists.txt` & `cytosim-0.0.3/src/play/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/makefile.inc` & `cytosim-0.0.3/src/play/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/play.cc` & `cytosim-0.0.3/src/play/play.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/play_keys.cc` & `cytosim-0.0.3/src/play/play_keys.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/play_menus.cc` & `cytosim-0.0.3/src/play/play_menus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/play_mouse.cc` & `cytosim-0.0.3/src/play/play_mouse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/player.cc` & `cytosim-0.0.3/src/play/player.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/player.h` & `cytosim-0.0.3/src/play/player.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/player_disp.cc` & `cytosim-0.0.3/src/play/player_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/player_prop.cc` & `cytosim-0.0.3/src/play/player_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/play/player_prop.h` & `cytosim-0.0.3/src/play/player_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/CMakeLists.txt` & `cytosim-0.0.3/src/sim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/bead.cc` & `cytosim-0.0.3/src/sim/bead.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/bead.h` & `cytosim-0.0.3/src/sim/bead.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/bead_set.cc` & `cytosim-0.0.3/src/sim/bead_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/bead_set.h` & `cytosim-0.0.3/src/sim/bead_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/chain.cc` & `cytosim-0.0.3/src/sim/chain.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/chain.h` & `cytosim-0.0.3/src/sim/chain.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/common.h` & `cytosim-0.0.3/src/sim/common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couple.cc` & `cytosim-0.0.3/src/sim/couple.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couple.h` & `cytosim-0.0.3/src/sim/couple.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couple_prop.cc` & `cytosim-0.0.3/src/sim/couple_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couple_prop.h` & `cytosim-0.0.3/src/sim/couple_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couple_set.cc` & `cytosim-0.0.3/src/sim/couple_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couple_set.h` & `cytosim-0.0.3/src/sim/couple_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/bridge.cc` & `cytosim-0.0.3/src/sim/couples/bridge.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/bridge.h` & `cytosim-0.0.3/src/sim/couples/bridge.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/bridge_prop.cc` & `cytosim-0.0.3/src/sim/couples/bridge_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/bridge_prop.h` & `cytosim-0.0.3/src/sim/couples/bridge_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/couple_long.cc` & `cytosim-0.0.3/src/sim/couples/couple_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/couple_long.h` & `cytosim-0.0.3/src/sim/couples/couple_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/crosslink.cc` & `cytosim-0.0.3/src/sim/couples/crosslink.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/crosslink.h` & `cytosim-0.0.3/src/sim/couples/crosslink.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/crosslink_long.cc` & `cytosim-0.0.3/src/sim/couples/crosslink_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/crosslink_long.h` & `cytosim-0.0.3/src/sim/couples/crosslink_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/crosslink_prop.cc` & `cytosim-0.0.3/src/sim/couples/crosslink_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/crosslink_prop.h` & `cytosim-0.0.3/src/sim/couples/crosslink_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/duo.cc` & `cytosim-0.0.3/src/sim/couples/duo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/duo.h` & `cytosim-0.0.3/src/sim/couples/duo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/duo_long.cc` & `cytosim-0.0.3/src/sim/couples/duo_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/duo_long.h` & `cytosim-0.0.3/src/sim/couples/duo_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/duo_prop.cc` & `cytosim-0.0.3/src/sim/couples/duo_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/duo_prop.h` & `cytosim-0.0.3/src/sim/couples/duo_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/fork.cc` & `cytosim-0.0.3/src/sim/couples/fork.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/fork.h` & `cytosim-0.0.3/src/sim/couples/fork.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/fork_prop.cc` & `cytosim-0.0.3/src/sim/couples/fork_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/fork_prop.h` & `cytosim-0.0.3/src/sim/couples/fork_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/shackle.cc` & `cytosim-0.0.3/src/sim/couples/shackle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/shackle.h` & `cytosim-0.0.3/src/sim/couples/shackle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/shackle_long.cc` & `cytosim-0.0.3/src/sim/couples/shackle_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/shackle_long.h` & `cytosim-0.0.3/src/sim/couples/shackle_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/shackle_prop.cc` & `cytosim-0.0.3/src/sim/couples/shackle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/couples/shackle_prop.h` & `cytosim-0.0.3/src/sim/couples/shackle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/event.cc` & `cytosim-0.0.3/src/sim/event.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/event.h` & `cytosim-0.0.3/src/sim/event.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/event_set.cc` & `cytosim-0.0.3/src/sim/event_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/event_set.h` & `cytosim-0.0.3/src/sim/event_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber.cc` & `cytosim-0.0.3/src/sim/fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber.h` & `cytosim-0.0.3/src/sim/fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_grid.cc` & `cytosim-0.0.3/src/sim/fiber_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_grid.h` & `cytosim-0.0.3/src/sim/fiber_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_grid2.cc` & `cytosim-0.0.3/src/sim/fiber_grid2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_prop.cc` & `cytosim-0.0.3/src/sim/fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_prop.h` & `cytosim-0.0.3/src/sim/fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_segment.cc` & `cytosim-0.0.3/src/sim/fiber_segment.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_segment.h` & `cytosim-0.0.3/src/sim/fiber_segment.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_set.cc` & `cytosim-0.0.3/src/sim/fiber_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_set.h` & `cytosim-0.0.3/src/sim/fiber_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_site.cc` & `cytosim-0.0.3/src/sim/fiber_site.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fiber_site.h` & `cytosim-0.0.3/src/sim/fiber_site.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/classic_fiber.cc` & `cytosim-0.0.3/src/sim/fibers/classic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/classic_fiber.h` & `cytosim-0.0.3/src/sim/fibers/classic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.cc` & `cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.h` & `cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/dynamic_fiber.cc` & `cytosim-0.0.3/src/sim/fibers/dynamic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/dynamic_fiber.h` & `cytosim-0.0.3/src/sim/fibers/dynamic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.cc` & `cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.h` & `cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/growing_fiber.cc` & `cytosim-0.0.3/src/sim/fibers/growing_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/growing_fiber.h` & `cytosim-0.0.3/src/sim/fibers/growing_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.cc` & `cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.h` & `cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.cc` & `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.h` & `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.cc` & `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.h` & `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field.cc` & `cytosim-0.0.3/src/sim/field.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field.h` & `cytosim-0.0.3/src/sim/field.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field_prop.cc` & `cytosim-0.0.3/src/sim/field_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field_prop.h` & `cytosim-0.0.3/src/sim/field_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field_set.cc` & `cytosim-0.0.3/src/sim/field_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field_set.h` & `cytosim-0.0.3/src/sim/field_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/field_values.h` & `cytosim-0.0.3/src/sim/field_values.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/frame_reader.cc` & `cytosim-0.0.3/src/sim/frame_reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/frame_reader.h` & `cytosim-0.0.3/src/sim/frame_reader.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hand.cc` & `cytosim-0.0.3/src/sim/hand.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hand.h` & `cytosim-0.0.3/src/sim/hand.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hand_monitor.h` & `cytosim-0.0.3/src/sim/hand_monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hand_prop.cc` & `cytosim-0.0.3/src/sim/hand_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hand_prop.h` & `cytosim-0.0.3/src/sim/hand_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/actor.cc` & `cytosim-0.0.3/src/sim/hands/actor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/actor.h` & `cytosim-0.0.3/src/sim/hands/actor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/actor_prop.cc` & `cytosim-0.0.3/src/sim/hands/actor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/actor_prop.h` & `cytosim-0.0.3/src/sim/hands/actor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/chewer.cc` & `cytosim-0.0.3/src/sim/hands/chewer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/chewer.h` & `cytosim-0.0.3/src/sim/hands/chewer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/chewer_prop.cc` & `cytosim-0.0.3/src/sim/hands/chewer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/chewer_prop.h` & `cytosim-0.0.3/src/sim/hands/chewer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/cutter.cc` & `cytosim-0.0.3/src/sim/hands/cutter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/cutter.h` & `cytosim-0.0.3/src/sim/hands/cutter.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/cutter_prop.cc` & `cytosim-0.0.3/src/sim/hands/cutter_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/cutter_prop.h` & `cytosim-0.0.3/src/sim/hands/cutter_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/digit.cc` & `cytosim-0.0.3/src/sim/hands/digit.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/digit.h` & `cytosim-0.0.3/src/sim/hands/digit.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/digit_prop.cc` & `cytosim-0.0.3/src/sim/hands/digit_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/digit_prop.h` & `cytosim-0.0.3/src/sim/hands/digit_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/dynein.cc` & `cytosim-0.0.3/src/sim/hands/dynein.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/dynein.h` & `cytosim-0.0.3/src/sim/hands/dynein.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/dynein_prop.cc` & `cytosim-0.0.3/src/sim/hands/dynein_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/dynein_prop.h` & `cytosim-0.0.3/src/sim/hands/dynein_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/kinesin.cc` & `cytosim-0.0.3/src/sim/hands/kinesin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/kinesin.h` & `cytosim-0.0.3/src/sim/hands/kinesin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/kinesin_prop.cc` & `cytosim-0.0.3/src/sim/hands/kinesin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/kinesin_prop.h` & `cytosim-0.0.3/src/sim/hands/kinesin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/mighty.cc` & `cytosim-0.0.3/src/sim/hands/mighty.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/mighty.h` & `cytosim-0.0.3/src/sim/hands/mighty.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/mighty_prop.cc` & `cytosim-0.0.3/src/sim/hands/mighty_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/mighty_prop.h` & `cytosim-0.0.3/src/sim/hands/mighty_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/motor.cc` & `cytosim-0.0.3/src/sim/hands/motor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/motor.h` & `cytosim-0.0.3/src/sim/hands/motor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/motor_prop.cc` & `cytosim-0.0.3/src/sim/hands/motor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/motor_prop.h` & `cytosim-0.0.3/src/sim/hands/motor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/myosin.cc` & `cytosim-0.0.3/src/sim/hands/myosin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/myosin.h` & `cytosim-0.0.3/src/sim/hands/myosin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/myosin_prop.cc` & `cytosim-0.0.3/src/sim/hands/myosin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/myosin_prop.h` & `cytosim-0.0.3/src/sim/hands/myosin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/nucleator.cc` & `cytosim-0.0.3/src/sim/hands/nucleator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/nucleator.h` & `cytosim-0.0.3/src/sim/hands/nucleator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/nucleator_prop.cc` & `cytosim-0.0.3/src/sim/hands/nucleator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/nucleator_prop.h` & `cytosim-0.0.3/src/sim/hands/nucleator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/regulator.cc` & `cytosim-0.0.3/src/sim/hands/regulator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/regulator.h` & `cytosim-0.0.3/src/sim/hands/regulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/regulator_prop.cc` & `cytosim-0.0.3/src/sim/hands/regulator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/regulator_prop.h` & `cytosim-0.0.3/src/sim/hands/regulator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/rescuer.cc` & `cytosim-0.0.3/src/sim/hands/rescuer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/rescuer.h` & `cytosim-0.0.3/src/sim/hands/rescuer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/rescuer_prop.cc` & `cytosim-0.0.3/src/sim/hands/rescuer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/rescuer_prop.h` & `cytosim-0.0.3/src/sim/hands/rescuer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/slider.cc` & `cytosim-0.0.3/src/sim/hands/slider.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/slider.h` & `cytosim-0.0.3/src/sim/hands/slider.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/slider_prop.cc` & `cytosim-0.0.3/src/sim/hands/slider_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/slider_prop.h` & `cytosim-0.0.3/src/sim/hands/slider_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/tracker.cc` & `cytosim-0.0.3/src/sim/hands/tracker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/tracker.h` & `cytosim-0.0.3/src/sim/hands/tracker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/tracker_prop.cc` & `cytosim-0.0.3/src/sim/hands/tracker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/tracker_prop.h` & `cytosim-0.0.3/src/sim/hands/tracker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/walker.cc` & `cytosim-0.0.3/src/sim/hands/walker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/walker.h` & `cytosim-0.0.3/src/sim/hands/walker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/walker_prop.cc` & `cytosim-0.0.3/src/sim/hands/walker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/hands/walker_prop.h` & `cytosim-0.0.3/src/sim/hands/walker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/interface.cc` & `cytosim-0.0.3/src/sim/interface.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/interface.h` & `cytosim-0.0.3/src/sim/interface.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/interpolation.cc` & `cytosim-0.0.3/src/sim/interpolation.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/interpolation.h` & `cytosim-0.0.3/src/sim/interpolation.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/interpolation4.cc` & `cytosim-0.0.3/src/sim/interpolation4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/interpolation4.h` & `cytosim-0.0.3/src/sim/interpolation4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/lattice.cc` & `cytosim-0.0.3/src/sim/lattice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/lattice.h` & `cytosim-0.0.3/src/sim/lattice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/makefile.inc` & `cytosim-0.0.3/src/sim/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/meca.cc` & `cytosim-0.0.3/src/sim/meca.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/meca.h` & `cytosim-0.0.3/src/sim/meca.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/meca1d.h` & `cytosim-0.0.3/src/sim/meca1d.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/meca_inter.cc` & `cytosim-0.0.3/src/sim/meca_inter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecable.cc` & `cytosim-0.0.3/src/sim/mecable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecable.h` & `cytosim-0.0.3/src/sim/mecable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecafil.cc` & `cytosim-0.0.3/src/sim/mecafil.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecafil.h` & `cytosim-0.0.3/src/sim/mecafil.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecafil_project.cc` & `cytosim-0.0.3/src/sim/mecafil_project.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecafil_projectmat.cc` & `cytosim-0.0.3/src/sim/mecafil_projectmat.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecapoint.cc` & `cytosim-0.0.3/src/sim/mecapoint.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/mecapoint.h` & `cytosim-0.0.3/src/sim/mecapoint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/modulo.cc` & `cytosim-0.0.3/src/sim/modulo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/modulo.h` & `cytosim-0.0.3/src/sim/modulo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/movable.cc` & `cytosim-0.0.3/src/sim/movable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/movable.h` & `cytosim-0.0.3/src/sim/movable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/object.cc` & `cytosim-0.0.3/src/sim/object.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/object.h` & `cytosim-0.0.3/src/sim/object.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/object_set.cc` & `cytosim-0.0.3/src/sim/object_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/object_set.h` & `cytosim-0.0.3/src/sim/object_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizer.cc` & `cytosim-0.0.3/src/sim/organizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizer.h` & `cytosim-0.0.3/src/sim/organizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizer_set.cc` & `cytosim-0.0.3/src/sim/organizer_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizer_set.h` & `cytosim-0.0.3/src/sim/organizer_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/aster.cc` & `cytosim-0.0.3/src/sim/organizers/aster.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/aster.h` & `cytosim-0.0.3/src/sim/organizers/aster.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/aster_prop.cc` & `cytosim-0.0.3/src/sim/organizers/aster_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/aster_prop.h` & `cytosim-0.0.3/src/sim/organizers/aster_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/bundle.cc` & `cytosim-0.0.3/src/sim/organizers/bundle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/bundle.h` & `cytosim-0.0.3/src/sim/organizers/bundle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/bundle_prop.cc` & `cytosim-0.0.3/src/sim/organizers/bundle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/bundle_prop.h` & `cytosim-0.0.3/src/sim/organizers/bundle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/fake.cc` & `cytosim-0.0.3/src/sim/organizers/fake.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/fake.h` & `cytosim-0.0.3/src/sim/organizers/fake.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/fake_prop.cc` & `cytosim-0.0.3/src/sim/organizers/fake_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/fake_prop.h` & `cytosim-0.0.3/src/sim/organizers/fake_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/nucleus.cc` & `cytosim-0.0.3/src/sim/organizers/nucleus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/nucleus.h` & `cytosim-0.0.3/src/sim/organizers/nucleus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/nucleus_prop.cc` & `cytosim-0.0.3/src/sim/organizers/nucleus_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/organizers/nucleus_prop.h` & `cytosim-0.0.3/src/sim/organizers/nucleus_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/parser.cc` & `cytosim-0.0.3/src/sim/parser.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/parser.h` & `cytosim-0.0.3/src/sim/parser.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/point_grid.cc` & `cytosim-0.0.3/src/sim/point_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/point_grid.h` & `cytosim-0.0.3/src/sim/point_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sim.cc` & `cytosim-0.0.3/src/sim/sim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sim_thread.cc` & `cytosim-0.0.3/src/sim/sim_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sim_thread.h` & `cytosim-0.0.3/src/sim/sim_thread.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul.cc` & `cytosim-0.0.3/src/sim/simul.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul.h` & `cytosim-0.0.3/src/sim/simul.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_custom.cc` & `cytosim-0.0.3/src/sim/simul_custom.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_file.cc` & `cytosim-0.0.3/src/sim/simul_file.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_prop.cc` & `cytosim-0.0.3/src/sim/simul_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_prop.h` & `cytosim-0.0.3/src/sim/simul_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_report.cc` & `cytosim-0.0.3/src/sim/simul_report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_solve.cc` & `cytosim-0.0.3/src/sim/simul_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/simul_step.cc` & `cytosim-0.0.3/src/sim/simul_step.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/single.cc` & `cytosim-0.0.3/src/sim/single.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/single.h` & `cytosim-0.0.3/src/sim/single.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/single_prop.cc` & `cytosim-0.0.3/src/sim/single_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/single_prop.h` & `cytosim-0.0.3/src/sim/single_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/single_set.cc` & `cytosim-0.0.3/src/sim/single_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/single_set.h` & `cytosim-0.0.3/src/sim/single_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/picket.cc` & `cytosim-0.0.3/src/sim/singles/picket.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/picket.h` & `cytosim-0.0.3/src/sim/singles/picket.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/picket_long.cc` & `cytosim-0.0.3/src/sim/singles/picket_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/picket_long.h` & `cytosim-0.0.3/src/sim/singles/picket_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/wrist.cc` & `cytosim-0.0.3/src/sim/singles/wrist.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/wrist.h` & `cytosim-0.0.3/src/sim/singles/wrist.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/wrist_long.cc` & `cytosim-0.0.3/src/sim/singles/wrist_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/singles/wrist_long.h` & `cytosim-0.0.3/src/sim/singles/wrist_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/solid.cc` & `cytosim-0.0.3/src/sim/solid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/solid.h` & `cytosim-0.0.3/src/sim/solid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/solid_prop.cc` & `cytosim-0.0.3/src/sim/solid_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/solid_prop.h` & `cytosim-0.0.3/src/sim/solid_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/solid_set.cc` & `cytosim-0.0.3/src/sim/solid_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/solid_set.h` & `cytosim-0.0.3/src/sim/solid_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/space.cc` & `cytosim-0.0.3/src/sim/space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/space.h` & `cytosim-0.0.3/src/sim/space.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/space_prop.cc` & `cytosim-0.0.3/src/sim/space_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/space_prop.h` & `cytosim-0.0.3/src/sim/space_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/space_set.cc` & `cytosim-0.0.3/src/sim/space_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/space_set.h` & `cytosim-0.0.3/src/sim/space_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_banana.cc` & `cytosim-0.0.3/src/sim/spaces/space_banana.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_banana.h` & `cytosim-0.0.3/src/sim/spaces/space_banana.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_capsule.cc` & `cytosim-0.0.3/src/sim/spaces/space_capsule.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_capsule.h` & `cytosim-0.0.3/src/sim/spaces/space_capsule.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_cylinder.cc` & `cytosim-0.0.3/src/sim/spaces/space_cylinder.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_cylinder.h` & `cytosim-0.0.3/src/sim/spaces/space_cylinder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_cylinderP.cc` & `cytosim-0.0.3/src/sim/spaces/space_cylinderP.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_cylinderP.h` & `cytosim-0.0.3/src/sim/spaces/space_cylinderP.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_cylinderZ.cc` & `cytosim-0.0.3/src/sim/spaces/space_cylinderZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_cylinderZ.h` & `cytosim-0.0.3/src/sim/spaces/space_cylinderZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_dice.cc` & `cytosim-0.0.3/src/sim/spaces/space_dice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_dice.h` & `cytosim-0.0.3/src/sim/spaces/space_dice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_ellipse.cc` & `cytosim-0.0.3/src/sim/spaces/space_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_ellipse.h` & `cytosim-0.0.3/src/sim/spaces/space_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_periodic.cc` & `cytosim-0.0.3/src/sim/spaces/space_periodic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_periodic.h` & `cytosim-0.0.3/src/sim/spaces/space_periodic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_polygon.cc` & `cytosim-0.0.3/src/sim/spaces/space_polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_polygon.h` & `cytosim-0.0.3/src/sim/spaces/space_polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_polygonZ.cc` & `cytosim-0.0.3/src/sim/spaces/space_polygonZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_polygonZ.h` & `cytosim-0.0.3/src/sim/spaces/space_polygonZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_ring.cc` & `cytosim-0.0.3/src/sim/spaces/space_ring.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_ring.h` & `cytosim-0.0.3/src/sim/spaces/space_ring.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_sphere.cc` & `cytosim-0.0.3/src/sim/spaces/space_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_sphere.h` & `cytosim-0.0.3/src/sim/spaces/space_sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_square.cc` & `cytosim-0.0.3/src/sim/spaces/space_square.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_square.h` & `cytosim-0.0.3/src/sim/spaces/space_square.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_strip.cc` & `cytosim-0.0.3/src/sim/spaces/space_strip.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_strip.h` & `cytosim-0.0.3/src/sim/spaces/space_strip.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_torus.cc` & `cytosim-0.0.3/src/sim/spaces/space_torus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/spaces/space_torus.h` & `cytosim-0.0.3/src/sim/spaces/space_torus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sphere.cc` & `cytosim-0.0.3/src/sim/sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sphere.h` & `cytosim-0.0.3/src/sim/sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sphere_prop.cc` & `cytosim-0.0.3/src/sim/sphere_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sphere_prop.h` & `cytosim-0.0.3/src/sim/sphere_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sphere_set.cc` & `cytosim-0.0.3/src/sim/sphere_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/sphere_set.h` & `cytosim-0.0.3/src/sim/sphere_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/sim/splash.h` & `cytosim-0.0.3/src/sim/splash.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/CMakeLists.txt` & `cytosim-0.0.3/src/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/makefile.inc` & `cytosim-0.0.3/src/test/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test.cc` & `cytosim-0.0.3/src/test/test.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_blas.cc` & `cytosim-0.0.3/src/test/test_blas.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_code.cc` & `cytosim-0.0.3/src/test/test_code.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_cxx.cc` & `cytosim-0.0.3/src/test/test_cxx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_gillespie.cc` & `cytosim-0.0.3/src/test/test_gillespie.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_glapp.cc` & `cytosim-0.0.3/src/test/test_glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_glos.cc` & `cytosim-0.0.3/src/test/test_glos.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_glut.cc` & `cytosim-0.0.3/src/test/test_glut.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_glut3D.cc` & `cytosim-0.0.3/src/test/test_glut3D.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_grid.cc` & `cytosim-0.0.3/src/test/test_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_math.cc` & `cytosim-0.0.3/src/test/test_math.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_matrix.cc` & `cytosim-0.0.3/src/test/test_matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_omp.cc` & `cytosim-0.0.3/src/test/test_omp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_opengl.cc` & `cytosim-0.0.3/src/test/test_opengl.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_pipe.cc` & `cytosim-0.0.3/src/test/test_pipe.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_platonic.cc` & `cytosim-0.0.3/src/test/test_platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_quaternion.cc` & `cytosim-0.0.3/src/test/test_quaternion.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_random.cc` & `cytosim-0.0.3/src/test/test_random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_rasterizer.cc` & `cytosim-0.0.3/src/test/test_rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_signal.cc` & `cytosim-0.0.3/src/test/test_signal.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_simd.cc` & `cytosim-0.0.3/src/test/test_simd.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_sizeof.cc` & `cytosim-0.0.3/src/test/test_sizeof.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_solve.cc` & `cytosim-0.0.3/src/test/test_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_space.cc` & `cytosim-0.0.3/src/test/test_space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_sphere.cc` & `cytosim-0.0.3/src/test/test_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_thread.cc` & `cytosim-0.0.3/src/test/test_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/test/test_vbo.cc` & `cytosim-0.0.3/src/test/test_vbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/CMakeLists.txt` & `cytosim-0.0.3/src/tools/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -44,7 +44,9 @@
         EXTERNAL_OBJECT true
         GENERATED true
     )
 pybind11_add_module(cytosim  ${PYCY_SOURCES})
 add_compile_options(-fPIC -shared -Wl,undefined,dynamic)
 target_link_libraries(cytosim PUBLIC "${TOOL_LIBS}")
 target_include_directories(cytosim PUBLIC ${TOOL_INCLUDES})
+set(outdir "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/cytosim")
+set_target_properties(cytosim PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${outdir})
```

### Comparing `cytosim-0.0.2/src/tools/cymart.cc` & `cytosim-0.0.3/src/tools/cymart.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/frametool.cc` & `cytosim-0.0.3/src/tools/frametool.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/makefile.inc` & `cytosim-0.0.3/src/tools/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/pycytoplay.cc` & `cytosim-0.0.3/src/tools/pycytoplay.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/pycytosim.cc` & `cytosim-0.0.3/src/tools/pycytosim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/pycytosim.h` & `cytosim-0.0.3/src/tools/pycytosim.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/reader.cc` & `cytosim-0.0.3/src/tools/reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/report.cc` & `cytosim-0.0.3/src/tools/report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/reportF.cc` & `cytosim-0.0.3/src/tools/reportF.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.2/src/tools/sieve.cc` & `cytosim-0.0.3/src/tools/sieve.cc`

 * *Files identical despite different names*

