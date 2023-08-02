# Comparing `tmp/ezcharts-0.6.3.tar.gz` & `tmp/ezcharts-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcharts-0.6.3.tar", last modified: Tue Aug  1 16:37:51 2023, max compression
+gzip compressed data, was "ezcharts-0.6.4.tar", last modified: Wed Aug  2 14:00:08 2023, max compression
```

## Comparing `ezcharts-0.6.3.tar` & `ezcharts-0.6.4.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.880173 ezcharts-0.6.3/
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-08-01 16:34:26.000000 ezcharts-0.6.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-08-01 16:34:26.000000 ezcharts-0.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5776 2023-08-01 16:37:51.880173 ezcharts-0.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-08-01 16:34:26.000000 ezcharts-0.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.824168 ezcharts-0.6.3/ezcharts/
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.828169 ezcharts-0.6.3/ezcharts/components/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9982 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/bcfstats.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/bokehchart.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/clinvar.py
--rw-rw-rw-   0 root         (0) root         (0)     6395 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/common.py
--rw-rw-rw-   0 root         (0) root         (0)    14124 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/dss.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/ezchart.py
--rw-rw-rw-   0 root         (0) root         (0)    16999 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)    12869 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/modkit.py
--rw-rw-rw-   0 root         (0) root         (0)    13245 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/mosdepth.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.828169 ezcharts-0.6.3/ezcharts/components/reports/
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/reports/comp.py
--rw-rw-rw-   0 root         (0) root         (0)     7295 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/reports/labs.py
--rw-rw-rw-   0 root         (0) root         (0)     7349 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/reports/ond.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/components/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.820168 ezcharts-0.6.3/ezcharts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.828169 ezcharts-0.6.3/ezcharts/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/images/LAB_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/images/OND_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    33283 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/images/OND_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/images/ONT_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)   894078 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/images/dots.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.820168 ezcharts-0.6.3/ezcharts/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.832169 ezcharts-0.6.3/ezcharts/data/reference/hg19/
--rw-rw-rw-   0 root         (0) root         (0)     6297 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/reference/hg19/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.832169 ezcharts-0.6.3/ezcharts/data/reference/hg38/
--rw-rw-rw-   0 root         (0) root         (0)    11449 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/reference/hg38/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.832169 ezcharts-0.6.3/ezcharts/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/scripts/epi2melabs.js
--rw-rw-rw-   0 root         (0) root         (0)   394601 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/scripts/metagenomics-sankey-util.js
--rw-rw-rw-   0 root         (0) root         (0)    22486 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/scripts/metagenomics-sankey.js
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/scripts/nextclade.html
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/scripts/ond.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.832169 ezcharts-0.6.3/ezcharts/data/styles/
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/styles/epi2melabs.scss
--rw-rw-rw-   0 root         (0) root         (0)     2585 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/styles/metagenomics-sankey.css
--rw-rw-rw-   0 root         (0) root         (0)   898896 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/styles/ond.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.844170 ezcharts-0.6.3/ezcharts/data/test/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/bamstats.flagstat.tsv
--rw-rw-rw-   0 root         (0) root         (0)  1916228 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/bamstats.readstats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/fastcat.stats.gz
--rw-rw-rw-   0 root         (0) root         (0)    28549 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/hg38_cnv.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)     2420 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/hg38_some_bands.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)   427338 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/karyomap_vals.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    16943 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/nextclade.json
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/params.json
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/plot-spec.json
--rwxrwxrwx   0 root         (0) root         (0)      790 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/ref.fa.fai
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/sankey.json
--rw-rw-rw-   0 root         (0) root         (0)  1125122 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/test_dml.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    35285 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/test_dmr.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)  1458860 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/test_modkit.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/test_modkit_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)     7150 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/test_mosdepth.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/test_mosdepth_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/test/versions.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.844170 ezcharts-0.6.3/ezcharts/data/themes/
--rw-rw-rw-   0 root         (0) root         (0)     5771 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/themes/epi2melabs.json
--rw-rw-rw-   0 root         (0) root         (0)     5764 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/themes/ond.json
--rw-rw-rw-   0 root         (0) root         (0)     5536 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/themes/walden.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.844170 ezcharts-0.6.3/ezcharts/data/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.820168 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.844170 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/js/
--rw-rw-rw-   0 root         (0) root         (0)    80599 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.852171 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
--rw-rw-rw-   0 root         (0) root         (0)     2055 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
--rw-rw-rw-   0 root         (0) root         (0)     3195 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     6941 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1948 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
--rw-rw-rw-   0 root         (0) root         (0)     8093 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)    10554 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)     7762 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     4725 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
--rw-rw-rw-   0 root         (0) root         (0)     6907 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)     7371 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
--rw-rw-rw-   0 root         (0) root         (0)    17886 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
--rw-rw-rw-   0 root         (0) root         (0)    73610 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1253 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.856171 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
--rw-rw-rw-   0 root         (0) root         (0)     5868 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
--rw-rw-rw-   0 root         (0) root         (0)      478 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.856171 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.864172 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0 root         (0) root         (0)     4580 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
--rw-rw-rw-   0 root         (0) root         (0)     4164 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
--rw-rw-rw-   0 root         (0) root         (0)     4726 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
--rw-rw-rw-   0 root         (0) root         (0)     3380 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.864172 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.864172 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
--rw-rw-rw-   0 root         (0) root         (0)    10029 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
--rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/echarts.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.864172 ezcharts-0.6.3/ezcharts/data/vendor/simple-datatables/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/simple-datatables/simple-datatables.css
--rw-rw-rw-   0 root         (0) root         (0)    38201 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/data/vendor/simple-datatables/simple-datatables.js
--rw-rw-rw-   0 root         (0) root         (0)    12903 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.864172 ezcharts-0.6.3/ezcharts/layout/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3951 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.864172 ezcharts-0.6.3/ezcharts/layout/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/banner.py
--rw-rw-rw-   0 root         (0) root         (0)     2119 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/offcanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/section.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     7587 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/table.py
--rw-rw-rw-   0 root         (0) root         (0)     5636 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/snippets/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/layout/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.880173 ezcharts-0.6.3/ezcharts/plots/
--rw-rw-rw-   0 root         (0) root         (0)    10263 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/_base.py
--rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/axisgrid.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/categorical.py
--rw-rw-rw-   0 root         (0) root         (0)     5065 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)    12727 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/ideogram.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/karyomap.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/matrix.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/metagenomics_sankey.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/relational.py
--rwxrwxrwx   0 root         (0) root         (0)     3444 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/sunburst.py
--rw-rw-rw-   0 root         (0) root         (0)     7208 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/plots/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-08-01 16:34:26.000000 ezcharts-0.6.3/ezcharts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:37:51.824168 ezcharts-0.6.3/ezcharts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5776 2023-08-01 16:37:51.000000 ezcharts-0.6.3/ezcharts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8962 2023-08-01 16:37:51.000000 ezcharts-0.6.3/ezcharts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:37:51.000000 ezcharts-0.6.3/ezcharts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-08-01 16:37:51.000000 ezcharts-0.6.3/ezcharts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:36:45.000000 ezcharts-0.6.3/ezcharts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      108 2023-08-01 16:37:51.000000 ezcharts-0.6.3/ezcharts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-08-01 16:37:51.000000 ezcharts-0.6.3/ezcharts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-01 16:34:26.000000 ezcharts-0.6.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 16:37:51.880173 ezcharts-0.6.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-08-01 16:34:26.000000 ezcharts-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.712381 ezcharts-0.6.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-08-02 13:54:58.000000 ezcharts-0.6.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-08-02 13:54:58.000000 ezcharts-0.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5776 2023-08-02 14:00:08.712381 ezcharts-0.6.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-08-02 13:54:58.000000 ezcharts-0.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.640374 ezcharts-0.6.4/ezcharts/
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.644375 ezcharts-0.6.4/ezcharts/components/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9982 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/bcfstats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/bokehchart.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/clinvar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6395 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    14124 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/dss.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/ezchart.py
+-rw-rw-rw-   0 root         (0) root         (0)    16999 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)    12869 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/modkit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13245 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/mosdepth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.644375 ezcharts-0.6.4/ezcharts/components/reports/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/reports/comp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7295 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/reports/labs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/reports/ond.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/components/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.604371 ezcharts-0.6.4/ezcharts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.644375 ezcharts-0.6.4/ezcharts/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/images/LAB_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/images/OND_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/images/OND_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/images/ONT_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)   894078 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/images/dots.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.604371 ezcharts-0.6.4/ezcharts/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.648375 ezcharts-0.6.4/ezcharts/data/reference/hg19/
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/reference/hg19/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.648375 ezcharts-0.6.4/ezcharts/data/reference/hg38/
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/reference/hg38/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.652375 ezcharts-0.6.4/ezcharts/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/scripts/epi2melabs.js
+-rw-rw-rw-   0 root         (0) root         (0)   394601 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/scripts/metagenomics-sankey-util.js
+-rw-rw-rw-   0 root         (0) root         (0)    22486 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/scripts/metagenomics-sankey.js
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/scripts/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/scripts/ond.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.652375 ezcharts-0.6.4/ezcharts/data/styles/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/styles/epi2melabs.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/styles/metagenomics-sankey.css
+-rw-rw-rw-   0 root         (0) root         (0)   898896 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/styles/ond.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.664376 ezcharts-0.6.4/ezcharts/data/test/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)  1916228 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/fastcat.stats.gz
+-rw-rw-rw-   0 root         (0) root         (0)    28549 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/hg38_cnv.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/hg38_some_bands.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)   427338 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/karyomap_vals.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    16943 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/nextclade.json
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/plot-spec.json
+-rwxrwxrwx   0 root         (0) root         (0)      790 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/ref.fa.fai
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/sankey.json
+-rw-rw-rw-   0 root         (0) root         (0)  1125122 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/test_dml.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    35285 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/test_dmr.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)  1458860 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/test_modkit.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/test_modkit_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     7150 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/test_mosdepth.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/test_mosdepth_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/test/versions.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.668377 ezcharts-0.6.4/ezcharts/data/themes/
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/themes/epi2melabs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/themes/ond.json
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/themes/walden.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.668377 ezcharts-0.6.4/ezcharts/data/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.604371 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.668377 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/js/
+-rw-rw-rw-   0 root         (0) root         (0)    80599 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.680378 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
+-rw-rw-rw-   0 root         (0) root         (0)    17886 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
+-rw-rw-rw-   0 root         (0) root         (0)    73610 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.680378 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.684378 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.688378 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.688378 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.688378 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/echarts.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.688378 ezcharts-0.6.4/ezcharts/data/vendor/simple-datatables/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/simple-datatables/simple-datatables.css
+-rw-rw-rw-   0 root         (0) root         (0)    38201 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/data/vendor/simple-datatables/simple-datatables.js
+-rw-rw-rw-   0 root         (0) root         (0)    12903 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/demo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.688378 ezcharts-0.6.4/ezcharts/layout/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3951 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.692379 ezcharts-0.6.4/ezcharts/layout/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/banner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/offcanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     7587 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/snippets/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/layout/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.712381 ezcharts-0.6.4/ezcharts/plots/
+-rw-rw-rw-   0 root         (0) root         (0)    10263 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/_base.py
+-rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/axisgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/categorical.py
+-rw-rw-rw-   0 root         (0) root         (0)     5065 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12727 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/ideogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/karyomap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/metagenomics_sankey.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/relational.py
+-rwxrwxrwx   0 root         (0) root         (0)     3444 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/sunburst.py
+-rw-rw-rw-   0 root         (0) root         (0)     7208 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/plots/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-08-02 13:54:58.000000 ezcharts-0.6.4/ezcharts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:00:08.640374 ezcharts-0.6.4/ezcharts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5776 2023-08-02 14:00:08.000000 ezcharts-0.6.4/ezcharts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-08-02 14:00:08.000000 ezcharts-0.6.4/ezcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 14:00:08.000000 ezcharts-0.6.4/ezcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-08-02 14:00:08.000000 ezcharts-0.6.4/ezcharts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 13:58:50.000000 ezcharts-0.6.4/ezcharts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      115 2023-08-02 14:00:08.000000 ezcharts-0.6.4/ezcharts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-02 14:00:08.000000 ezcharts-0.6.4/ezcharts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-08-02 13:54:58.000000 ezcharts-0.6.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 14:00:08.712381 ezcharts-0.6.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-08-02 13:54:58.000000 ezcharts-0.6.4/setup.py
```

### Comparing `ezcharts-0.6.3/LICENSE` & `ezcharts-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/PKG-INFO` & `ezcharts-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.6.3
+Version: 0.6.4
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ezcharts-0.6.3/README.md` & `ezcharts-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/__init__.py` & `ezcharts-0.6.4/ezcharts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Simple eCharts API."""
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 import argparse
 import importlib
 import logging
 
 from ezcharts import util
 from ezcharts.plots.axisgrid import *  # noqa: F401,F403
```

### Comparing `ezcharts-0.6.3/ezcharts/components/bcfstats.py` & `ezcharts-0.6.4/ezcharts/components/bcfstats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/bokehchart.py` & `ezcharts-0.6.4/ezcharts/components/bokehchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/clinvar.py` & `ezcharts-0.6.4/ezcharts/components/clinvar.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/common.py` & `ezcharts-0.6.4/ezcharts/components/common.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/dss.py` & `ezcharts-0.6.4/ezcharts/components/dss.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/ezchart.py` & `ezcharts-0.6.4/ezcharts/components/ezchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/fastcat.py` & `ezcharts-0.6.4/ezcharts/components/fastcat.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/modkit.py` & `ezcharts-0.6.4/ezcharts/components/modkit.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/mosdepth.py` & `ezcharts-0.6.4/ezcharts/components/mosdepth.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/nextclade.py` & `ezcharts-0.6.4/ezcharts/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/params.py` & `ezcharts-0.6.4/ezcharts/components/params.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/reports/__init__.py` & `ezcharts-0.6.4/ezcharts/components/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/reports/comp.py` & `ezcharts-0.6.4/ezcharts/components/reports/comp.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/reports/labs.py` & `ezcharts-0.6.4/ezcharts/components/reports/labs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/reports/ond.py` & `ezcharts-0.6.4/ezcharts/components/reports/ond.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/theme.py` & `ezcharts-0.6.4/ezcharts/components/theme.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/components/versions.py` & `ezcharts-0.6.4/ezcharts/components/versions.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/images/LAB_logo.svg` & `ezcharts-0.6.4/ezcharts/data/images/LAB_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/images/OND_logo.svg` & `ezcharts-0.6.4/ezcharts/data/images/OND_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/images/OND_logo.txt` & `ezcharts-0.6.4/ezcharts/data/images/OND_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/images/ONT_logo.txt` & `ezcharts-0.6.4/ezcharts/data/images/ONT_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/images/dots.svg` & `ezcharts-0.6.4/ezcharts/data/images/dots.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/reference/hg19/cytoBand.txt.gz` & `ezcharts-0.6.4/ezcharts/data/reference/hg19/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/reference/hg38/cytoBand.txt.gz` & `ezcharts-0.6.4/ezcharts/data/reference/hg38/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/scripts/epi2melabs.js` & `ezcharts-0.6.4/ezcharts/data/scripts/epi2melabs.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/scripts/metagenomics-sankey-util.js` & `ezcharts-0.6.4/ezcharts/data/scripts/metagenomics-sankey-util.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/scripts/metagenomics-sankey.js` & `ezcharts-0.6.4/ezcharts/data/scripts/metagenomics-sankey.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/scripts/ond.js` & `ezcharts-0.6.4/ezcharts/data/scripts/ond.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/styles/epi2melabs.scss` & `ezcharts-0.6.4/ezcharts/data/styles/epi2melabs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/styles/metagenomics-sankey.css` & `ezcharts-0.6.4/ezcharts/data/styles/metagenomics-sankey.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/styles/ond.scss` & `ezcharts-0.6.4/ezcharts/data/styles/ond.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/bamstats.readstats.tsv.gz` & `ezcharts-0.6.4/ezcharts/data/test/bamstats.readstats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/fastcat.stats.gz` & `ezcharts-0.6.4/ezcharts/data/test/fastcat.stats.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/hg38_cnv.bed.gz` & `ezcharts-0.6.4/ezcharts/data/test/hg38_cnv.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/hg38_some_bands.bed.gz` & `ezcharts-0.6.4/ezcharts/data/test/hg38_some_bands.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/karyomap_vals.tsv.gz` & `ezcharts-0.6.4/ezcharts/data/test/karyomap_vals.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/nextclade.json` & `ezcharts-0.6.4/ezcharts/data/test/nextclade.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/params.json` & `ezcharts-0.6.4/ezcharts/data/test/params.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/plot-spec.json` & `ezcharts-0.6.4/ezcharts/data/test/plot-spec.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/ref.fa.fai` & `ezcharts-0.6.4/ezcharts/data/test/ref.fa.fai`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/sankey.json` & `ezcharts-0.6.4/ezcharts/data/test/sankey.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/test_dml.tsv.gz` & `ezcharts-0.6.4/ezcharts/data/test/test_dml.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/test_dmr.tsv.gz` & `ezcharts-0.6.4/ezcharts/data/test/test_dmr.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/test_modkit.bed.gz` & `ezcharts-0.6.4/ezcharts/data/test/test_modkit.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/test/test_mosdepth.bed.gz` & `ezcharts-0.6.4/ezcharts/data/test/test_mosdepth.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/themes/epi2melabs.json` & `ezcharts-0.6.4/ezcharts/data/themes/epi2melabs.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/themes/ond.json` & `ezcharts-0.6.4/ezcharts/data/themes/ond.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/themes/walden.json` & `ezcharts-0.6.4/ezcharts/data/themes/walden.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss` & `ezcharts-0.6.4/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/echarts.min.js` & `ezcharts-0.6.4/ezcharts/data/vendor/echarts.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/simple-datatables/simple-datatables.css` & `ezcharts-0.6.4/ezcharts/data/vendor/simple-datatables/simple-datatables.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/data/vendor/simple-datatables/simple-datatables.js` & `ezcharts-0.6.4/ezcharts/data/vendor/simple-datatables/simple-datatables.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/demo.py` & `ezcharts-0.6.4/ezcharts/demo.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/base.py` & `ezcharts-0.6.4/ezcharts/layout/base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/resource.py` & `ezcharts-0.6.4/ezcharts/layout/resource.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/__init__.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/banner.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/banner.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/cards.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/cards.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/document.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/document.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/grid.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/grid.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/offcanvas.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/offcanvas.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/progress.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/progress.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/section.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/section.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/stats.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/stats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/table.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/table.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/snippets/tabs.py` & `ezcharts-0.6.4/ezcharts/layout/snippets/tabs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/layout/util.py` & `ezcharts-0.6.4/ezcharts/layout/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/__init__.py` & `ezcharts-0.6.4/ezcharts/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/_base.py` & `ezcharts-0.6.4/ezcharts/plots/_base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/_model.py` & `ezcharts-0.6.4/ezcharts/plots/_model.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/categorical.py` & `ezcharts-0.6.4/ezcharts/plots/categorical.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/distribution.py` & `ezcharts-0.6.4/ezcharts/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/ideogram.py` & `ezcharts-0.6.4/ezcharts/plots/ideogram.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/karyomap.py` & `ezcharts-0.6.4/ezcharts/plots/karyomap.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/matrix.py` & `ezcharts-0.6.4/ezcharts/plots/matrix.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/metagenomics_sankey.py` & `ezcharts-0.6.4/ezcharts/plots/metagenomics_sankey.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/relational.py` & `ezcharts-0.6.4/ezcharts/plots/relational.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/sunburst.py` & `ezcharts-0.6.4/ezcharts/plots/sunburst.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/plots/util.py` & `ezcharts-0.6.4/ezcharts/plots/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts/util.py` & `ezcharts-0.6.4/ezcharts/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/ezcharts.egg-info/PKG-INFO` & `ezcharts-0.6.4/ezcharts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.6.3
+Version: 0.6.4
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ezcharts-0.6.3/ezcharts.egg-info/SOURCES.txt` & `ezcharts-0.6.4/ezcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.6.3/setup.py` & `ezcharts-0.6.4/setup.py`

 * *Files identical despite different names*

