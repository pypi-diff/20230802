# Comparing `tmp/ritm_annotation-0.0.7.tar.gz` & `tmp/ritm_annotation-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritm_annotation-0.0.7.tar", last modified: Mon Jul 31 21:36:15 2023, max compression
+gzip compressed data, was "ritm_annotation-0.0.8.tar", last modified: Wed Aug  2 01:26:04 2023, max compression
```

## Comparing `ritm_annotation-0.0.7.tar` & `ritm_annotation-0.0.8.tar`

### file list

```diff
@@ -1,147 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/annotate/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/model_info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/model_info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/cli/train/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/cli/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.746312 ritm_annotation-0.0.7/ritm_annotation/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/berkeley.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco_lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/davis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/grabcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/images_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/openimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/pascalvoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/datasets/sbd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.746312 ritm_annotation-0.0.7/ritm_annotation/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/engine/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.746312 ritm_annotation-0.0.7/ritm_annotation/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/clicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_functors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/crops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/limit_longest_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/transforms/zoom_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/is_deeplab_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/is_hrnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/is_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.750312 ritm_annotation-0.0.7/ritm_annotation/model/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/deeplab_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/hrnet_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnetv1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/model/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.754312 ritm_annotation-0.0.7/ritm_annotation/models/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.754312 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3362 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3290 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3307 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.754312 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3369 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3354 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3348 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3208 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3179 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3203 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3187 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3430 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/models/test_exposed_model_stuff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/utils/cython/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/_get_dist_maps.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/cython/dist_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/exp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.758312 ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/ritm_annotation/utils/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.742312 ritm_annotation-0.0.7/ritm_annotation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 21:36:15.000000 ritm_annotation-0.0.7/ritm_annotation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:15.762313 ritm_annotation-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 21:36:02.000000 ritm_annotation-0.0.7/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/dataset_lint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/dataset_lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/finetune/
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/finetune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/finetune/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/model_info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/model_info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/berkeley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco_lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/davis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/grabcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/images_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/openimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/pascalvoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/sbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/engine/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/clicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_functors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/crops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/limit_longest_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/zoom_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/is_deeplab_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/is_hrnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/is_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/model/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/deeplab_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/hrnet_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnetv1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.102386 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3534 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3463 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3443 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.102386 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.102386 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3527 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3473 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3517 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3761 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3385 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3345 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3313 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3627 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/test_exposed_model_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/ritm_annotation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/ritm_annotation/utils/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/_get_dist_maps.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/dist_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/exp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/tests/test_base.py
```

### Comparing `ritm_annotation-0.0.7/LICENSE` & `ritm_annotation-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/PKG-INFO` & `ritm_annotation-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritm_annotation
-Version: 0.0.7
+Version: 0.0.8
 Summary: Awesome ritm_annotation created by lucasew
 Home-page: https://github.com/lucasew/ritm_annotation/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `ritm_annotation-0.0.7/README.md` & `ritm_annotation-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/cli/__init__.py` & `ritm_annotation-0.0.8/ritm_annotation/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 """
 
 import logging
 import sys
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from pathlib import Path
 
-from ritm_annotation.cli.annotate import command as command_annotate
-from ritm_annotation.cli.model_info import command as command_model_info
-from ritm_annotation.cli.train import command as command_train
+from ritm_annotation.utils.misc import load_module
 
 logger = logging.getLogger(__name__)
 
 
-def add_subcommand(subparsers, name: str, command_fn):
-    subparser = subparsers.add_parser(name)
+def add_subcommand(subparsers, name: str, submodule):
+    subparser = subparsers.add_parser(name, help=submodule.COMMAND_DESCRIPTION)
     common_flags(subparser)
-    handler = command_fn(subparser)
+    handler = submodule.command(subparser)
     subparser.set_defaults(fn=handler)
 
 
 def common_flags(parser):
     parser.add_argument(
         "-v",
         "--verbose",
@@ -62,17 +60,24 @@
     """
     logging.basicConfig()
     parser = ArgumentParser(
         prog="ritm_annotation", formatter_class=ArgumentDefaultsHelpFormatter
     )
     common_flags(parser)
     subparsers = parser.add_subparsers()
-    add_subcommand(subparsers, "annotate", command_annotate)
-    add_subcommand(subparsers, "train", command_train)
-    add_subcommand(subparsers, "model_info", command_model_info)
+
+    for module in Path(__file__).parent.glob("*/__init__.py"):
+        if str(module).find("pycache") > 0:
+            continue
+        module_name = module.parent.name
+        subcommand_module = load_module(
+            module, module_name=f"ritm_annotation.cli.{module_name}"
+        )
+        add_subcommand(subparsers, module_name, subcommand_module)
+
     args = parser.parse_args()
 
     if args.verbose:
         logging.root.setLevel(logging.DEBUG)
 
     version = open(str(Path(__file__).parent.parent / "VERSION"), "r").read()
     if args.is_show_version:
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/__init__.py` & `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,16 +599,18 @@
             all_checked = all_checked and widget._check_bounds(
                 widget.get(), "-1"
             )
 
         return all_checked
 
 
+COMMAND_DESCRIPTION = "Interactively annotate a dataset"
+
+
 def command(subparser):
-    subparser.description = "Interactively annotate a dataset"
     subparser.add_argument("input", type=Path)
     subparser.add_argument("output", type=Path)
     subparser.add_argument(
         "-d",
         "--device",
         dest="device",
         type=torch.device,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/canvas.py` & `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/canvas.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/controller.py` & `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/controller.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/cli/annotate/wrappers.py` & `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/wrappers.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/cli/train/__init__.py` & `ritm_annotation-0.0.8/ritm_annotation/cli/train/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,37 @@
 import torch
 
 from ritm_annotation.utils.exp import init_experiment
 from ritm_annotation.utils.misc import load_module
 
 logger = logging.getLogger(__name__)
 
+COMMAND_DESCRIPTION = "Run from-scratch trains using off the shelf datasets"
+
 
 def command(parser):
     parser.add_argument(
         "model_path", type=str, help="Path to the model script."
     )
+
+    parser.add_argument(
+        "-o",
+        "--output",
+        dest="experiment_path",
+        type=Path,
+        default=Path("."),
+        help="Where to store experiment data",
+    )
+
     parser.add_argument(
-        "experiment_path", type=Path, help="Where to store experiment data"
+        "-n",
+        "--num-epochs",
+        dest="num_epochs",
+        type=int,
+        help="Amount of epochs",
     )
 
     parser.add_argument(
         "--exp-name",
         type=str,
         default="",
         help="Here you can specify the name of the experiment. "  # noqa:E501
@@ -112,15 +128,15 @@
             )
         model_path = model_path.resolve()
         args.model_path = model_path
         logger.debug(f"Final model path: '{model_path}'")
 
         model_script = load_module(model_path)
 
-        model_base_name = getattr(model_script, "MODEL_NAME", None)
+        model_base_name = model_script.__dict__.get("MODEL_NAME")
 
         args.distributed = "WORLD_SIZE" in os.environ
         cfg = init_experiment(args, model_base_name)
         for k, v in os.environ.items():
             if k.startswith("RITM_"):
                 cfgkey = k.replace("RITM_", "")
                 logger.warning(
@@ -129,10 +145,12 @@
                 cfg[cfgkey] = v
 
         torch.backends.cudnn.benchmark = True
         torch.multiprocessing.set_sharing_strategy("file_system")
         logger.debug("Basic validations passed")
         model, model_cfg = model_script.init_model(cfg)
         trainer = model_script.get_trainer(model, cfg, model_cfg)
-        trainer.run(num_epochs=model_cfg.default_num_epochs)
+        if args.num_epochs is None:
+            args.num_epochs = model_cfg.default_num_epochs
+        trainer.run(num_epochs=args.num_epochs)
 
     return handle
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/base.py` & `ritm_annotation-0.0.8/ritm_annotation/data/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/compose.py` & `ritm_annotation-0.0.8/ritm_annotation/data/compose.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/__init__.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/ade20k.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/coco_lvis.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco_lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/davis.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/davis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/grabcut.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/grabcut.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/images_dir.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/images_dir.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/lvis.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/openimages.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/openimages.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/pascalvoc.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/pascalvoc.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/datasets/sbd.py` & `ritm_annotation-0.0.8/ritm_annotation/data/datasets/sbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/points_sampler.py` & `ritm_annotation-0.0.8/ritm_annotation/data/points_sampler.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/sample.py` & `ritm_annotation-0.0.8/ritm_annotation/data/sample.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/data/transforms.py` & `ritm_annotation-0.0.8/ritm_annotation/data/transforms.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/engine/optimizer.py` & `ritm_annotation-0.0.8/ritm_annotation/engine/optimizer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/engine/trainer.py` & `ritm_annotation-0.0.8/ritm_annotation/engine/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 class ISTrainer(object):
     def __init__(
         self,
         model,
         cfg,
         model_cfg,
         loss_cfg,
-        trainset,
-        valset,
+        trainset=None,
+        valset=None,
         optimizer="adam",
         optimizer_params=None,
         image_dump_interval=200,
         checkpoint_interval=10,
         tb_dump_period=25,
         max_interactive_points=0,
         lr_scheduler=None,
@@ -75,94 +75,112 @@
             self.val_metrics.extend(additional_val_metrics)
 
         self.checkpoint_interval = checkpoint_interval
         self.image_dump_interval = image_dump_interval
         self.task_prefix = ""
         self.sw = None
 
+        self.dry_run = dry_run
         self.trainset = trainset
         self.valset = valset
+        self.device = self.cfg.device
+        self.lr_scheduler_fn = lr_scheduler
+        self.model = model
+        self.optimizer = optimizer
+        self.optimizer_params = optimizer_params
+
+        self.tqdm_out = TqdmToLogger(logger, level=logging.INFO)
+
+    def _before_needed_hook(self):
+        if self._ran_before_needed:
+            return
+        self._ran_before_needed = True
+
+        logger.debug("Looking for basic assumptions")
+        assert self.trainset is not None, "Missing train dataset"
+        assert self.valset is not None, "Missing validation dataset"
 
         logger.info(
-            f"Dataset of {trainset.get_samples_number()} samples was loaded for training."  # noqa: E501
+            f"Dataset of {self.trainset.get_samples_number()} samples was loaded for training."  # noqa: E501
         )
         logger.info(
-            f"Dataset of {valset.get_samples_number()} samples was loaded for validation."  # noqa: E501
+            f"Dataset of {self.valset.get_samples_number()} samples was loaded for validation."  # noqa: E501
         )
 
+        logger.debug("Setting up dataloder")
         self.train_data = DataLoader(
-            trainset,
-            cfg.batch_size,
+            self.trainset,
+            self.cfg.batch_size,
             sampler=get_sampler(
-                trainset, shuffle=True, distributed=cfg.distributed
+                self.trainset, shuffle=True, distributed=self.cfg.distributed
             )
-            if not dry_run
+            if not self.dry_run
             else None,
             drop_last=True,
             pin_memory=True,
-            num_workers=cfg.workers,
-            persistent_workers=cfg.workers > 0,
+            num_workers=self.cfg.workers,
+            persistent_workers=self.cfg.workers > 0,
         )
 
         self.val_data = DataLoader(
-            valset,
-            cfg.val_batch_size,
+            self.valset,
+            self.cfg.val_batch_size,
             sampler=get_sampler(
-                valset, shuffle=False, distributed=cfg.distributed
+                self.valset, shuffle=False, distributed=self.cfg.distributed
             )
-            if not dry_run
+            if not self.dry_run
             else None,
             drop_last=True,
             pin_memory=True,
-            num_workers=cfg.workers,
-            persistent_workers=cfg.workers > 0,
+            num_workers=self.cfg.workers,
+            persistent_workers=self.cfg.workers > 0,
+        )
+        logger.debug("Initializing model")
+        self.model = self._load_weights(self.model)
+        self.optim = get_optimizer(
+            self.model, self.optimizer, self.optimizer_params
         )
 
-        self.optim = get_optimizer(model, optimizer, optimizer_params)
-        model = self._load_weights(model)
-
-        if cfg.multi_gpu:
-            model = get_dp_wrapper(cfg.distributed)(
-                model, device_ids=cfg.gpu_ids, output_device=cfg.gpu_ids[0]
+        if self.cfg.multi_gpu:
+            self.model = get_dp_wrapper(self.cfg.distributed)(
+                self.model,
+                device_ids=self.cfg.gpu_ids,
+                output_device=self.cfg.gpu_ids[0],
             )
 
         if self.is_master:
-            logger.info(model)
-            logger.info(get_config_repr(model._config))
+            logger.info(self.model)
+            logger.info(get_config_repr(self.model._config))
 
-        self.device = cfg.device
-        self.net = model.to(self.device)
-        self.lr = optimizer_params["lr"]
-
-        if lr_scheduler is not None:
-            self.lr_scheduler = lr_scheduler(optimizer=self.optim)
-            if cfg.start_epoch > 0:
-                for _ in range(cfg.start_epoch):
+        self.net = self.model.to(self.device)
+        self.lr = self.optimizer_params["lr"]
+
+        if self.lr_scheduler_fn is not None:
+            self.lr_scheduler = self.lr_scheduler_fn(optimizer=self.optim)
+            if self.cfg.start_epoch > 0:
+                for _ in range(self.cfg.start_epoch):
                     self.lr_scheduler.step()
 
-        self.tqdm_out = TqdmToLogger(logger, level=logging.INFO)
+        logger.debug("Initializing click models")
 
         if self.click_models is not None:
             for click_model in self.click_models:
                 for param in click_model.parameters():
                     param.requires_grad = False
                 click_model.to(self.device)
                 click_model.eval()
-        logger.info("Run experiment with config:")
-        logger.info(pprint.pformat(cfg, indent=4))
 
-    def _before_needed_hook(self):
-        if self._ran_before_needed:
-            return
-        self._ran_before_needed = True
         logger.debug(f"First train batch: {repr(next(iter(self.train_data)))}")
         logger.debug(
             f"First evaluation batch: {repr(next(iter(self.val_data)))}"
         )
 
+        logger.info("Run experiment with config:")
+        logger.info(pprint.pformat(self.cfg, indent=4))
+
     def run(self, num_epochs, start_epoch=None, validation=True):
         self._before_needed_hook()
         if start_epoch is None:
             start_epoch = self.cfg.start_epoch
 
         logger.info(f"Starting Epoch: {start_epoch}")
         logger.info(f"Total Epochs: {num_epochs}")
@@ -248,15 +266,15 @@
                     value=self.lr
                     if not hasattr(self, "lr_scheduler")
                     else self.lr_scheduler.get_lr()[-1],
                     global_step=global_step,
                 )
 
                 tbar.set_description(
-                    f"Epoch {epoch}, training loss {train_loss/(i+1):.4f}"
+                    f"Epoch {epoch}, training loss {train_loss/(i+1):.8f}"
                 )
                 for metric in self.train_metrics:
                     metric.log_states(
                         self.sw,
                         f"{log_prefix}Metrics/{metric.name}",
                         global_step,
                     )
@@ -542,14 +560,15 @@
         ).astype(np.uint8)
 
         _save_image("instance_segmentation", viz_image[:, :, ::-1])
 
     def _load_weights(self, net):
         if self.cfg.weights is not None:
             if os.path.isfile(self.cfg.weights):
+                logger.info(f"Loading weights from '{self.cfg.weights}'")
                 load_weights(net, self.cfg.weights)
                 self.cfg.weights = None
             else:
                 raise RuntimeError(
                     f"=> no checkpoint found at '{self.cfg.weights}'"
                 )
         elif self.cfg.resume_exp is not None:
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/clicker.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/clicker.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/evaluation.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/evaluation.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/__init__.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/base.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_functors.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_functors.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/predictors/brs_losses.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/base.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/crops.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/crops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/flip.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/flip.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/limit_longest_side.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/limit_longest_side.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/transforms/zoom_in.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/zoom_in.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/inference/utils.py` & `ritm_annotation-0.0.8/ritm_annotation/inference/utils.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/initializer.py` & `ritm_annotation-0.0.8/ritm_annotation/model/initializer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/is_deeplab_model.py` & `ritm_annotation-0.0.8/ritm_annotation/model/is_deeplab_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/is_hrnet_model.py` & `ritm_annotation-0.0.8/ritm_annotation/model/is_hrnet_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/is_model.py` & `ritm_annotation-0.0.8/ritm_annotation/model/is_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/losses.py` & `ritm_annotation-0.0.8/ritm_annotation/model/losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/metrics.py` & `ritm_annotation-0.0.8/ritm_annotation/model/metrics.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/modeling/basic_blocks.py` & `ritm_annotation-0.0.8/ritm_annotation/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/modeling/deeplab_v3.py` & `ritm_annotation-0.0.8/ritm_annotation/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/modeling/hrnet_ocr.py` & `ritm_annotation-0.0.8/ritm_annotation/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/modeling/ocr.py` & `ritm_annotation-0.0.8/ritm_annotation/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnet.py` & `ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/modeling/resnetv1b.py` & `ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/model/ops.py` & `ritm_annotation-0.0.8/ritm_annotation/model/ops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py` & `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
-from ritm_annotation.utils.misc import load_module
 
 MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 160
 
     model = HRNetModel(
         width=18,
         ocr_width=64,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -25,24 +23,25 @@
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
+    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_loss = SoftIoU()
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
@@ -76,35 +75,39 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
-
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
+
+        valset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
@@ -118,8 +121,7 @@
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
         checkpoint_interval=5,
         image_dump_interval=2000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
     )
-    return trainer
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 120
 
     model = HRNetModel(
         width=18,
         ocr_width=64,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -23,25 +24,24 @@
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
-    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = FocalLoss(alpha=0.5, gamma=2)
+    loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
@@ -70,45 +70,50 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.8,
+        prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = ADE20kDataset(
+            cfg.ADE20K_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            stuff_prob=0.30,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = ADE20kDataset(
+            cfg.ADE20K_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
@@ -116,8 +121,9 @@
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
         checkpoint_interval=5,
         image_dump_interval=2000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
     )
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py` & `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,21 +27,21 @@
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
+    loss_cfg.instance_loss = FocalLoss(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
@@ -75,35 +75,39 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
+    model_cfg.default_num_epochs = 230
 
     model = HRNetModel(
         width=18,
         ocr_width=64,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -23,25 +24,24 @@
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
-    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = SoftIoU()
+    loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
@@ -75,49 +75,54 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
         valset,
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
-        checkpoint_interval=5,
-        image_dump_interval=2000,
+        checkpoint_interval=[(0, 5), (200, 1)],
+        image_dump_interval=3000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
+        dry_run=dry_run,
     )
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
+from ritm_annotation.utils.misc import load_module
 
-MODEL_NAME = "cocolvis_hrnet18"
+MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 230
+    model_cfg.default_num_epochs = 160
 
     model = HRNetModel(
         width=18,
         ocr_width=64,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
-        with_prev_mask=True,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
-    loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
+    loss_cfg.instance_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
     loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
@@ -71,56 +71,58 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.80,
+        prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
-
-    valset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
         valset,
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
-        checkpoint_interval=[(0, 5), (200, 1)],
-        image_dump_interval=3000,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
-        max_num_next_clicks=3,
-        dry_run=dry_run,
     )
+    return trainer
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py` & `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -85,35 +85,39 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = SBDDataset(
-        cfg.SBD_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.01,
-        points_sampler=points_sampler,
-        samples_scores_path="./assets/sbd_samples_weights.pkl",
-        samples_scores_gamma=1.25,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = SBDDataset(
+            cfg.SBD_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.01,
+            points_sampler=points_sampler,
+            samples_scores_path="./assets/sbd_samples_weights.pkl",
+            samples_scores_gamma=1.25,
+            dry_run=dry_run,
+        )
 
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        points_sampler=points_sampler,
-        epoch_len=500,
-        dry_run=dry_run,
-    )
+        valset = SBDDataset(
+            cfg.SBD_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            points_sampler=points_sampler,
+            epoch_len=500,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 215], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18_SMALL
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 32 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -77,35 +77,39 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_v1_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoLvisDataset(
+            cfg.LVIS_v1_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = "cocolvis_hrnet32"
+MODEL_NAME = "resnet34"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 230
+    model_cfg.default_num_epochs = 160
 
-    model = HRNetModel(
-        width=32,
-        ocr_width=128,
-        with_aux_output=True,
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
         use_leaky_relu=True,
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
-        with_prev_mask=True,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
-        model.feature_extractor.load_pretrained_weights(
-            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W32
-        )
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
-    cfg.batch_size = 32 if cfg.batch_size < 1 else cfg.batch_size
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
+    cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
-    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
-    loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
             HorizontalFlip(),
             PadIfNeeded(
                 min_height=crop_size[0], min_width=crop_size[1], border_mode=0
@@ -71,56 +66,59 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.80,
+        prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_v1_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
         valset,
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
-        checkpoint_interval=[(0, 5), (200, 1)],
-        image_dump_interval=3000,
+        checkpoint_interval=5,
+        image_dump_interval=2000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
-        max_num_next_clicks=3,
         dry_run=dry_run,
     )
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = "hrnet18"
+MODEL_NAME = "resnet34"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
     model_cfg.default_num_epochs = 120
 
-    model = HRNetModel(
-        width=18,
-        ocr_width=64,
-        with_aux_output=True,
+    model = DeeplabModel(
+        backbone="resnet34",
+        deeplab_ch=128,
+        aspp_dropout=0.20,
         use_leaky_relu=True,
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
-        model.feature_extractor.load_pretrained_weights(
-            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
-        )
+        model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
-    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
-    loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
             HorizontalFlip(),
             PadIfNeeded(
                 min_height=crop_size[0], min_width=crop_size[1], border_mode=0
@@ -70,41 +66,45 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.80,
+        prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = ADE20kDataset(
-        cfg.ADE20K_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        stuff_prob=0.30,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = ADE20kDataset(
+            cfg.ADE20K_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            stuff_prob=0.30,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
 
-    valset = ADE20kDataset(
-        cfg.ADE20K_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = ADE20kDataset(
+            cfg.ADE20K_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -75,36 +75,40 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoDataset(
-        cfg.COCO_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        stuff_prob=0.30,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoDataset(
+            cfg.COCO_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            stuff_prob=0.30,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
 
-    valset = CocoDataset(
-        cfg.COCO_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoDataset(
+            cfg.COCO_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py` & `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = "hrnet18"
+MODEL_NAME = "cocolvis_hrnet32"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
     model_cfg.default_num_epochs = 230
 
     model = HRNetModel(
-        width=18,
-        ocr_width=64,
+        width=32,
+        ocr_width=128,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
+        with_prev_mask=True,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights(
-            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W32
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
-    cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
+    cfg.batch_size = 32 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
     loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
@@ -70,40 +71,44 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.8,
+        prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_v1_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
 
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = CocoLvisDataset(
+            cfg.LVIS_v1_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
     )
     return ISTrainer(
@@ -116,9 +121,10 @@
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
         checkpoint_interval=[(0, 5), (200, 1)],
         image_dump_interval=3000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
+        max_num_next_clicks=3,
         dry_run=dry_run,
     )
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py` & `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 160
 
     model = HRNetModel(
         width=18,
         ocr_width=64,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -24,18 +23,19 @@
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
+    model_cfg.default_num_epochs = 160
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -75,34 +75,39 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = LvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
-
-    valset = LvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
+
+        valset = CocoLvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=80,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
@@ -115,9 +120,8 @@
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
         checkpoint_interval=5,
         image_dump_interval=2000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
-        dry_run=dry_run,
     )
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 140
+    model_cfg.default_num_epochs = 160
 
     model = HRNetModel(
         width=18,
         ocr_width=64,
         with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -27,15 +27,15 @@
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -75,40 +75,43 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = LvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
 
-    valset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+        valset = LvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -75,34 +75,38 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = SBDDataset(
-        cfg.SBD_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        samples_scores_path="./assets/sbd_samples_weights.pkl",
-        samples_scores_gamma=1.25,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = SBDDataset(
+            cfg.SBD_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            samples_scores_path="./assets/sbd_samples_weights.pkl",
+            samples_scores_gamma=1.25,
+            dry_run=dry_run,
+        )
 
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        dry_run=dry_run,
-    )
+        valset = SBDDataset(
+            cfg.SBD_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         model.feature_extractor.load_pretrained_weights(
             cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
         )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -75,41 +75,45 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = ComposeDataset(
-        [
-            PascalVocDataset(
-                cfg.PASCALVOC_PATH, split="train", dry_run=dry_run
-            ),
-            SBDDataset(
-                cfg.SBD_PATH,
-                split="train",
-                samples_scores_path="./assets/sbd_samples_weights.pkl",
-                samples_scores_gamma=1.25,
-                dry_run=dry_run,
-            ),
-        ],
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = ComposeDataset(
+            [
+                PascalVocDataset(
+                    cfg.PASCALVOC_PATH, split="train", dry_run=dry_run
+                ),
+                SBDDataset(
+                    cfg.SBD_PATH,
+                    split="train",
+                    samples_scores_path="./assets/sbd_samples_weights.pkl",
+                    samples_scores_gamma=1.25,
+                    dry_run=dry_run,
+                ),
+            ],
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+        )
 
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        dry_run=dry_run,
-    )
+        valset = SBDDataset(
+            cfg.SBD_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MODEL_NAME = "resnet34"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 120
+    model_cfg.default_num_epochs = 160
 
     model = DeeplabModel(
         backbone="resnet34",
         deeplab_ch=128,
         aspp_dropout=0.20,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -25,15 +25,15 @@
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -71,41 +71,43 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = ADE20kDataset(
-        cfg.ADE20K_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        stuff_prob=0.30,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
-
-    valset = ADE20kDataset(
-        cfg.ADE20K_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = LvisDataset(
+            cfg.LVIS_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
+
+        valset = LvisDataset(
+            cfg.LVIS_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if not dry_run:
         model.feature_extractor.load_pretrained_weights()
 
     model_cfg.default_num_epochs = 140
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -71,36 +71,40 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoDataset(
-        cfg.COCO_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        stuff_prob=0.30,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
-
-    valset = CocoDataset(
-        cfg.COCO_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoDataset(
+            cfg.COCO_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            stuff_prob=0.30,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
+
+        valset = CocoDataset(
+            cfg.COCO_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
         torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
     )
     return ISTrainer(
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MODEL_NAME = "resnet34"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 160
+    model_cfg.default_num_epochs = 120
 
     model = DeeplabModel(
         backbone="resnet34",
         deeplab_ch=128,
         aspp_dropout=0.20,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -25,15 +25,15 @@
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -71,40 +71,43 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        stuff_prob=0.30,
-        dry_run=dry_run,
-    )
-
-    valset = CocoLvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=80,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = SBDDataset(
+            cfg.SBD_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+            samples_scores_path="./assets/sbd_samples_weights.pkl",
+            samples_scores_gamma=1.25,
+            dry_run=dry_run,
+        )
+
+        valset = SBDDataset(
+            cfg.SBD_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MODEL_NAME = "resnet34"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 160
+    model_cfg.default_num_epochs = 140
 
     model = DeeplabModel(
         backbone="resnet34",
         deeplab_ch=128,
         aspp_dropout=0.20,
         use_leaky_relu=True,
         use_rgb_conv=False,
@@ -25,15 +25,15 @@
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -71,39 +71,44 @@
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
         prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = LvisDataset(
-        cfg.LVIS_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
-
-    valset = LvisDataset(
-        cfg.LVIS_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = OpenImagesDataset(
+            cfg.OPENIMAGES_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
+
+        valset = OpenImagesDataset(
+            cfg.OPENIMAGES_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[140, 155], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 MODEL_NAME = "resnet34"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 140
+    model_cfg.default_num_epochs = 120
 
     model = DeeplabModel(
         backbone="resnet34",
         deeplab_ch=128,
         aspp_dropout=0.20,
-        use_leaky_relu=True,
+        use_leaky_relu=True,  # noqa: E501
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
         model.feature_extractor.load_pretrained_weights()
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
@@ -66,45 +66,55 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.8,
+        prob_gamma=0.8,  # noqa:E501
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=30000,
-        dry_run=dry_run,
-    )
-
-    valset = OpenImagesDataset(
-        cfg.OPENIMAGES_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        keep_background_prob=0.05,
-        points_sampler=points_sampler,
-        epoch_len=2000,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = ComposeDataset(
+            [
+                PascalVocDataset(
+                    cfg.PASCALVOC_PATH, split="train", dry_run=dry_run
+                ),
+                SBDDataset(
+                    cfg.SBD_PATH,
+                    split="train",
+                    samples_scores_path="./assets/sbd_samples_weights.pkl",
+                    samples_scores_gamma=1.25,
+                    dry_run=dry_run,
+                ),
+            ],
+            augmentator=train_augmentator,
+            min_object_area=80,
+            keep_background_prob=0.0,
+            points_sampler=points_sampler,
+        )
+
+        valset = SBDDataset(
+            cfg.SBD_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py` & `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = "resnet34"
+MODEL_NAME = "cocolvis_hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 120
+    model_cfg.default_num_epochs = 230
 
-    model = DeeplabModel(
-        backbone="resnet34",
-        deeplab_ch=128,
-        aspp_dropout=0.20,
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
         use_leaky_relu=True,
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
+        with_prev_mask=True,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
-        model.feature_extractor.load_pretrained_weights()
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
+    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
             HorizontalFlip(),
             PadIfNeeded(
                 min_height=crop_size[0], min_width=crop_size[1], border_mode=0
@@ -66,54 +71,60 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.8,
+        prob_gamma=0.80,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = SBDDataset(
-        cfg.SBD_PATH,
-        split="train",
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-        samples_scores_path="./assets/sbd_samples_weights.pkl",
-        samples_scores_gamma=1.25,
-        dry_run=dry_run,
-    )
-
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = CocoLvisDataset(
+            cfg.LVIS_v1_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            stuff_prob=0.30,
+            dry_run=dry_run,
+        )
+
+        valset = CocoLvisDataset(
+            cfg.LVIS_v1_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[200, 220], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
         valset,
         optimizer="adam",
         optimizer_params=optimizer_params,
         lr_scheduler=lr_scheduler,
-        checkpoint_interval=5,
-        image_dump_interval=2000,
+        checkpoint_interval=[(0, 5), (200, 1)],
+        image_dump_interval=3000,
         metrics=[AdaptiveIoU()],
         max_interactive_points=model_cfg.num_max_points,
+        max_num_next_clicks=3,
         dry_run=dry_run,
     )
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py` & `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 # flake8: noqa
 
 from ritm_annotation.utils.exp_imports.default import *
 
-MODEL_NAME = "resnet34"
+MODEL_NAME = "hrnet18"
 
 
 def init_model(cfg, dry_run=False):
     model_cfg = edict()
     model_cfg.crop_size = (320, 480)
     model_cfg.num_max_points = 24
-    model_cfg.default_num_epochs = 120
+    model_cfg.default_num_epochs = 140
 
-    model = DeeplabModel(
-        backbone="resnet34",
-        deeplab_ch=128,
-        aspp_dropout=0.20,
-        use_leaky_relu=True,  # noqa: E501
+    model = HRNetModel(
+        width=18,
+        ocr_width=64,
+        with_aux_output=True,
+        use_leaky_relu=True,
         use_rgb_conv=False,
         use_disks=True,
         norm_radius=5,
     )
 
     model.to(cfg.device)
     model.apply(initializer.XavierGluon(rnd_type="gaussian", magnitude=2.0))
     if not dry_run:
-        model.feature_extractor.load_pretrained_weights()
+        model.feature_extractor.load_pretrained_weights(
+            cfg.IMAGENET_PRETRAINED_MODELS.HRNETV2_W18
+        )
 
     return model, model_cfg
 
 
-def get_trainer(model, cfg, model_cfg, dry_run=False):
+def get_trainer(model, cfg, model_cfg, dry_run=False, no_dataset=False):
     cfg.batch_size = 28 if cfg.batch_size < 1 else cfg.batch_size
     cfg.val_batch_size = cfg.batch_size
     crop_size = model_cfg.crop_size
 
     loss_cfg = edict()
     loss_cfg.instance_loss = NormalizedFocalLossSigmoid(alpha=0.5, gamma=2)
     loss_cfg.instance_loss_weight = 1.0
+    loss_cfg.instance_aux_loss = SigmoidBinaryCrossEntropyLoss()
+    loss_cfg.instance_aux_loss_weight = 0.4
 
     train_augmentator = Compose(
         [
             UniformRandomResize(scale_range=(0.75, 1.40)),
             HorizontalFlip(),
             PadIfNeeded(
                 min_height=crop_size[0], min_width=crop_size[1], border_mode=0
@@ -66,51 +70,49 @@
             RandomCrop(*crop_size),
         ],
         p=1.0,
     )
 
     points_sampler = MultiPointSampler(
         model_cfg.num_max_points,
-        prob_gamma=0.8,  # noqa:E501
+        prob_gamma=0.8,
         merge_objects_prob=0.15,
         max_num_merged_objects=2,
     )
 
-    trainset = ComposeDataset(
-        [
-            PascalVocDataset(
-                cfg.PASCALVOC_PATH, split="train", dry_run=dry_run
-            ),
-            SBDDataset(
-                cfg.SBD_PATH,
-                split="train",
-                samples_scores_path="./assets/sbd_samples_weights.pkl",
-                samples_scores_gamma=1.25,
-                dry_run=dry_run,
-            ),
-        ],
-        augmentator=train_augmentator,
-        min_object_area=80,
-        keep_background_prob=0.0,
-        points_sampler=points_sampler,
-    )
-
-    valset = SBDDataset(
-        cfg.SBD_PATH,
-        split="val",
-        augmentator=val_augmentator,
-        min_object_area=1000,
-        points_sampler=points_sampler,
-        dry_run=dry_run,
-    )
+    if no_dataset:
+        trainset = None
+        valset = None
+    else:
+        trainset = OpenImagesDataset(
+            cfg.OPENIMAGES_PATH,
+            split="train",
+            augmentator=train_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=30000,
+            dry_run=dry_run,
+        )
+
+        valset = OpenImagesDataset(
+            cfg.OPENIMAGES_PATH,
+            split="val",
+            augmentator=val_augmentator,
+            min_object_area=1000,
+            keep_background_prob=0.05,
+            points_sampler=points_sampler,
+            epoch_len=2000,
+            dry_run=dry_run,
+        )
 
     optimizer_params = {"lr": 5e-4, "betas": (0.9, 0.999), "eps": 1e-8}
 
     lr_scheduler = partial(
-        torch.optim.lr_scheduler.MultiStepLR, milestones=[100, 115], gamma=0.1
+        torch.optim.lr_scheduler.MultiStepLR, milestones=[120, 135], gamma=0.1
     )
     return ISTrainer(
         model,
         cfg,
         model_cfg,
         loss_cfg,
         trainset,
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/cython/_get_dist_maps.pyx` & `ritm_annotation-0.0.8/ritm_annotation/utils/cython/_get_dist_maps.pyx`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/distributed.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/exp.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/exp.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/exp_imports/default.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/default.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/log.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/log.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/misc.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 def ignore_params_then_call(func):
     def ret(*args, **kwargs):
         return func()
 
     return ret
 
 
-def load_module(script_path):
+def load_module(script_path, module_name="module"):
     logger.debug(f"Loading module '{script_path}'...")
-    spec = importlib.util.spec_from_file_location("model_script", script_path)
+    spec = importlib.util.spec_from_file_location(module_name, script_path)
     assert spec is not None, f"Can't import model at '{script_path}'"
     model_script = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(model_script)
 
     return model_script
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/serialization.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation/utils/vis.py` & `ritm_annotation-0.0.8/ritm_annotation/utils/vis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.7/ritm_annotation.egg-info/PKG-INFO` & `ritm_annotation-0.0.8/ritm_annotation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritm-annotation
-Version: 0.0.7
+Version: 0.0.8
 Summary: Awesome ritm_annotation created by lucasew
 Home-page: https://github.com/lucasew/ritm_annotation/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `ritm_annotation-0.0.7/ritm_annotation.egg-info/SOURCES.txt` & `ritm_annotation-0.0.8/ritm_annotation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 ritm_annotation.egg-info/top_level.txt
 ritm_annotation/cli/README.md
 ritm_annotation/cli/__init__.py
 ritm_annotation/cli/annotate/__init__.py
 ritm_annotation/cli/annotate/canvas.py
 ritm_annotation/cli/annotate/controller.py
 ritm_annotation/cli/annotate/wrappers.py
+ritm_annotation/cli/dataset_lint/__init__.py
+ritm_annotation/cli/finetune/__init__.py
+ritm_annotation/cli/finetune/dataset.py
 ritm_annotation/cli/model_info/__init__.py
 ritm_annotation/cli/train/__init__.py
 ritm_annotation/data/__init__.py
 ritm_annotation/data/base.py
 ritm_annotation/data/compose.py
 ritm_annotation/data/points_sampler.py
 ritm_annotation/data/sample.py
```

### Comparing `ritm_annotation-0.0.7/setup.py` & `ritm_annotation-0.0.8/setup.py`

 * *Files identical despite different names*

