# Comparing `tmp/kgcnn-3.0.1.tar.gz` & `tmp/kgcnn-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcnn-3.0.1.tar", last modified: Mon May 22 14:57:55 2023, max compression
+gzip compressed data, was "kgcnn-3.0.2.tar", last modified: Wed Aug  2 07:22:42 2023, max compression
```

## Comparing `kgcnn-3.0.1.tar` & `kgcnn-3.0.2.tar`

### file list

```diff
@@ -1,316 +1,321 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.144680 kgcnn-3.0.1/
--rw-rw-rw-   0        0        0       76 2023-05-22 05:04:06.000000 kgcnn-3.0.1/AUTHORS
--rw-rw-rw-   0        0        0     1066 2023-05-22 05:04:06.000000 kgcnn-3.0.1/LICENSE
--rw-rw-rw-   0        0        0       53 2023-05-22 05:04:06.000000 kgcnn-3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    19415 2023-05-22 14:57:55.143679 kgcnn-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    18539 2023-05-22 05:04:06.000000 kgcnn-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.458469 kgcnn-3.0.1/kgcnn/
--rw-rw-rw-   0        0        0       43 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.533255 kgcnn-3.0.1/kgcnn/crystal/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/__init__.py
--rw-rw-rw-   0        0        0     2902 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/base.py
--rw-rw-rw-   0        0        0    31910 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/graph_builder.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.544611 kgcnn-3.0.1/kgcnn/crystal/periodic_table/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/periodic_table/__init__.py
--rw-rw-rw-   0        0        0    15016 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.csv
--rw-rw-rw-   0        0        0     4029 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.py
--rw-rw-rw-   0        0        0    21221 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/crystal/preprocessor.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.626678 kgcnn-3.0.1/kgcnn/data/
--rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/__init__.py
--rw-rw-rw-   0        0        0    35033 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/base.py
--rw-rw-rw-   0        0        0    12885 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/crystal.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.838682 kgcnn-3.0.1/kgcnn/data/datasets/
--rw-rw-rw-   0        0        0     3036 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/ClinToxDataset.py
--rw-rw-rw-   0        0        0     3186 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/CoraDataset.py
--rw-rw-rw-   0        0        0     4761 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/CoraLuDataset.py
--rw-rw-rw-   0        0        0     1559 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/ESOLDataset.py
--rw-rw-rw-   0        0        0     1727 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/FreeSolvDataset.py
--rw-rw-rw-   0        0        0     5398 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/GraphTUDataset2020.py
--rw-rw-rw-   0        0        0     7113 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/ISO17Dataset.py
--rw-rw-rw-   0        0        0     1471 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/LipopDataset.py
--rw-rw-rw-   0        0        0     8792 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MD17Dataset.py
--rw-rw-rw-   0        0        0     6574 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MD17RevisedDataset.py
--rw-rw-rw-   0        0        0     3158 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MUTAGDataset.py
--rw-rw-rw-   0        0        0    11255 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatBenchDataset2020.py
--rw-rw-rw-   0        0        0     1469 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectDielectricDataset.py
--rw-rw-rw-   0        0        0     1388 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectEFormDataset.py
--rw-rw-rw-   0        0        0     1398 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectGapDataset.py
--rw-rw-rw-   0        0        0     1424 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectIsMetalDataset.py
--rw-rw-rw-   0        0        0     1325 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectJdft2dDataset.py
--rw-rw-rw-   0        0        0     1605 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogGVRHDataset.py
--rw-rw-rw-   0        0        0     1604 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogKVRHDataset.py
--rw-rw-rw-   0        0        0     1316 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPerovskitesDataset.py
--rw-rw-rw-   0        0        0     1693 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPhononsDataset.py
--rw-rw-rw-   0        0        0     8589 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MoleculeNetDataset2018.py
--rw-rw-rw-   0        0        0     4834 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/MutagenicityDataset.py
--rw-rw-rw-   0        0        0     3051 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/PROTEINSDataset.py
--rw-rw-rw-   0        0        0     6575 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM7Dataset.py
--rw-rw-rw-   0        0        0     5533 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM7bDataset.py
--rw-rw-rw-   0        0        0     3922 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM8Dataset.py
--rw-rw-rw-   0        0        0    12255 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM9Dataset.py
--rw-rw-rw-   0        0        0     2952 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/QM9MolNetDataset.py
--rw-rw-rw-   0        0        0     2160 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/SIDERDataset.py
--rw-rw-rw-   0        0        0     2194 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/Tox21MolNetDataset.py
--rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    12525 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/download.py
--rw-rw-rw-   0        0        0    22994 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/moleculenet.py
--rw-rw-rw-   0        0        0    17817 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/qm.py
--rw-rw-rw-   0        0        0     2851 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/serial.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.840683 kgcnn-3.0.1/kgcnn/data/transform/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/base.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.880678 kgcnn-3.0.1/kgcnn/data/transform/scaler/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/__init__.py
--rw-rw-rw-   0        0        0    19619 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/force.py
--rw-rw-rw-   0        0        0    53863 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/molecule.py
--rw-rw-rw-   0        0        0     1865 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/serial.py
--rw-rw-rw-   0        0        0    28142 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/transform/scaler/standard.py
--rw-rw-rw-   0        0        0     9408 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/tudataset.py
--rw-rw-rw-   0        0        0     5311 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.913678 kgcnn-3.0.1/kgcnn/graph/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/__init__.py
--rw-rw-rw-   0        0        0    26883 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/base.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.940681 kgcnn-3.0.1/kgcnn/graph/methods/
--rw-rw-rw-   0        0        0     1316 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/methods/__init__.py
--rw-rw-rw-   0        0        0    28421 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/methods/_adj.py
--rw-rw-rw-   0        0        0    23582 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/methods/_geom.py
--rw-rw-rw-   0        0        0     1864 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/postprocessor.py
--rw-rw-rw-   0        0        0    31335 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/preprocessor.py
--rw-rw-rw-   0        0        0     2468 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/graph/serial.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.946680 kgcnn-3.0.1/kgcnn/io/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/io/__init__.py
--rw-rw-rw-   0        0        0     8125 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/io/file.py
--rw-rw-rw-   0        0        0     4556 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/io/loader.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.085678 kgcnn-3.0.1/kgcnn/layers/
--rw-rw-rw-   0        0        0     1095 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/README.md
--rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/__init__.py
--rw-rw-rw-   0        0        0    15544 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/attention.py
--rw-rw-rw-   0        0        0     7693 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/base.py
--rw-rw-rw-   0        0        0    12507 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/casting.py
--rw-rw-rw-   0        0        0    15178 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/conv.py
--rw-rw-rw-   0        0        0    17112 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/gather.py
--rw-rw-rw-   0        0        0    43155 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/geom.py
--rw-rw-rw-   0        0        0     4735 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/message.py
--rw-rw-rw-   0        0        0    18206 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/mlp.py
--rw-rw-rw-   0        0        0    23450 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/modules.py
--rw-rw-rw-   0        0        0    28771 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/norm.py
--rw-rw-rw-   0        0        0    35808 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/pooling.py
--rw-rw-rw-   0        0        0    11853 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/relational.py
--rw-rw-rw-   0        0        0    13549 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/set2set.py
--rw-rw-rw-   0        0        0     8702 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/layers/update.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.087682 kgcnn-3.0.1/kgcnn/literature/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.107678 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/__init__.py
--rw-rw-rw-   0        0        0    12186 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_attentivefp_conv.py
--rw-rw-rw-   0        0        0     5902 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.128678 kgcnn-3.0.1/kgcnn/literature/CGCNN/
--rw-rw-rw-   0        0        0      130 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CGCNN/__init__.py
--rw-rw-rw-   0        0        0     6471 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CGCNN/_cgcnn_conv.py
--rw-rw-rw-   0        0        0     9358 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CGCNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.139678 kgcnn-3.0.1/kgcnn/literature/CMPNN/
--rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CMPNN/__init__.py
--rw-rw-rw-   0        0        0     8126 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/CMPNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.169678 kgcnn-3.0.1/kgcnn/literature/DGIN/
--rw-rw-rw-   0        0        0      100 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DGIN/__init__.py
--rw-rw-rw-   0        0        0     4927 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DGIN/_dgin_conv.py
--rw-rw-rw-   0        0        0    10250 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DGIN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.189678 kgcnn-3.0.1/kgcnn/literature/DMPNN/
--rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DMPNN/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DMPNN/_dmpnn_conv.py
--rw-rw-rw-   0        0        0     8366 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DMPNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.210678 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/
--rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/__init__.py
--rw-rw-rw-   0        0        0    19372 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_dimenet_conv.py
--rw-rw-rw-   0        0        0    18270 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.222678 kgcnn-3.0.1/kgcnn/literature/EGNN/
--rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/EGNN/__init__.py
--rw-rw-rw-   0        0        0    10063 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/EGNN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.226680 kgcnn-3.0.1/kgcnn/literature/GAT/
--rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GAT/__init__.py
--rw-rw-rw-   0        0        0     5925 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GAT/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.239678 kgcnn-3.0.1/kgcnn/literature/GATv2/
--rw-rw-rw-   0        0        0       98 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GATv2/__init__.py
--rw-rw-rw-   0        0        0     6279 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GATv2/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.270678 kgcnn-3.0.1/kgcnn/literature/GCN/
--rw-rw-rw-   0        0        0      218 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GCN/__init__.py
--rw-rw-rw-   0        0        0     1874 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GCN/_gcn_conv.py
--rw-rw-rw-   0        0        0    10192 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GCN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.289678 kgcnn-3.0.1/kgcnn/literature/GIN/
--rw-rw-rw-   0        0        0      202 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GIN/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GIN/_gin_conv.py
--rw-rw-rw-   0        0        0    10899 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GIN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.335678 kgcnn-3.0.1/kgcnn/literature/GNNExplain/
--rw-rw-rw-   0        0        0      187 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/__init__.py
--rw-rw-rw-   0        0        0    30109 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_model.py
--rw-rw-rw-   0        0        0     1262 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py
--rw-rw-rw-   0        0        0     1134 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_base.py
--rw-rw-rw-   0        0        0      933 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_testing.py
--rw-rw-rw-   0        0        0      565 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.360678 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_base.py
--rw-rw-rw-   0        0        0     4459 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_testing.py
--rw-rw-rw-   0        0        0      774 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.365680 kgcnn-3.0.1/kgcnn/literature/GNNFilm/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNFilm/__init__.py
--rw-rw-rw-   0        0        0     5606 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GNNFilm/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.367679 kgcnn-3.0.1/kgcnn/literature/GemNet/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GemNet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.371679 kgcnn-3.0.1/kgcnn/literature/GraphSAGE/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GraphSAGE/__init__.py
--rw-rw-rw-   0        0        0     6836 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/GraphSAGE/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.407678 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/
--rw-rw-rw-   0        0        0      454 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/__init__.py
--rw-rw-rw-   0        0        0    25733 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_acsf_conv.py
--rw-rw-rw-   0        0        0    15739 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_make.py
--rw-rw-rw-   0        0        0    21072 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_wacsf_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.442679 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/
--rw-rw-rw-   0        0        0      127 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_hdnnp_conv.py
--rw-rw-rw-   0        0        0     8160 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_make.py
--rw-rw-rw-   0        0        0     9442 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_test_hdnnp.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.467681 kgcnn-3.0.1/kgcnn/literature/HamNet/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HamNet/__init__.py
--rw-rw-rw-   0        0        0    28565 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HamNet/_hamnet_conv.py
--rw-rw-rw-   0        0        0     8210 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/HamNet/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.472680 kgcnn-3.0.1/kgcnn/literature/INorp/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/INorp/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/INorp/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.491678 kgcnn-3.0.1/kgcnn/literature/MAT/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MAT/__init__.py
--rw-rw-rw-   0        0        0     9724 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MAT/_make.py
--rw-rw-rw-   0        0        0     8758 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MAT/_mat_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.530681 kgcnn-3.0.1/kgcnn/literature/MEGAN/
--rw-rw-rw-   0        0        0      218 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/_make.py
--rw-rw-rw-   0        0        0    22759 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/_model.py
--rw-rw-rw-   0        0        0     6903 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MEGAN/_test_literature_megan.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.550680 kgcnn-3.0.1/kgcnn/literature/MXMNet/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MXMNet/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MXMNet/_make.py
--rw-rw-rw-   0        0        0     8490 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MXMNet/_mxmnet_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.571678 kgcnn-3.0.1/kgcnn/literature/Megnet/
--rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Megnet/__init__.py
--rw-rw-rw-   0        0        0    18509 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Megnet/_make.py
--rw-rw-rw-   0        0        0     7153 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Megnet/_megnet_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.594678 kgcnn-3.0.1/kgcnn/literature/MoGAT/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MoGAT/__init__.py
--rw-rw-rw-   0        0        0     6679 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MoGAT/_make.py
--rw-rw-rw-   0        0        0    12206 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/MoGAT/_mogat_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.616681 kgcnn-3.0.1/kgcnn/literature/NMPN/
--rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/NMPN/__init__.py
--rw-rw-rw-   0        0        0    17202 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/NMPN/_make.py
--rw-rw-rw-   0        0        0     4753 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/NMPN/_mpnn_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.647678 kgcnn-3.0.1/kgcnn/literature/PAiNN/
--rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/PAiNN/__init__.py
--rw-rw-rw-   0        0        0    14386 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/PAiNN/_make.py
--rw-rw-rw-   0        0        0    15451 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/PAiNN/_painn_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.652681 kgcnn-3.0.1/kgcnn/literature/RGCN/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/RGCN/__init__.py
--rw-rw-rw-   0        0        0     5668 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/RGCN/_make.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.672679 kgcnn-3.0.1/kgcnn/literature/Schnet/
--rw-rw-rw-   0        0        0      215 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Schnet/__init__.py
--rw-rw-rw-   0        0        0    14260 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Schnet/_make.py
--rw-rw-rw-   0        0        0     8445 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Schnet/_schnet_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.710678 kgcnn-3.0.1/kgcnn/literature/Unet/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/__init__.py
--rw-rw-rw-   0        0        0     7194 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_make.py
--rw-rw-rw-   0        0        0     1138 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_test_connect.py
--rw-rw-rw-   0        0        0     4157 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_test_topk.py
--rw-rw-rw-   0        0        0    19977 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/Unet/_topk.py
--rw-rw-rw-   0        0        0       51 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.776680 kgcnn-3.0.1/kgcnn/literature/coGN/
--rw-rw-rw-   0        0        0     2873 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/__init__.py
--rw-rw-rw-   0        0        0     7496 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_coGN_config.py
--rw-rw-rw-   0        0        0     6429 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_coNGN_config.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.794678 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/__init__.py
--rw-rw-rw-   0        0        0     4218 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py
--rw-rw-rw-   0        0        0     6719 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py
--rw-rw-rw-   0        0        0      891 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_gates.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.815680 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/__init__.py
--rw-rw-rw-   0        0        0    16183 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_network_base.py
--rw-rw-rw-   0        0        0    23941 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_networks.py
--rw-rw-rw-   0        0        0    27901 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_make.py
--rw-rw-rw-   0        0        0     2266 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_multiplicity_readout.py
--rw-rw-rw-   0        0        0     3945 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_preprocessing_layers.py
--rw-rw-rw-   0        0        0     1051 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_test.py
--rw-rw-rw-   0        0        0      372 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/coGN/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.826680 kgcnn-3.0.1/kgcnn/literature/rGIN/
--rw-rw-rw-   0        0        0       99 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/rGIN/__init__.py
--rw-rw-rw-   0        0        0     5444 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/rGIN/_make.py
--rw-rw-rw-   0        0        0     3502 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/literature/rGIN/_rgin_conv.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.843679 kgcnn-3.0.1/kgcnn/metrics/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/metrics/__init__.py
--rw-rw-rw-   0        0        0      972 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/metrics/loss.py
--rw-rw-rw-   0        0        0    10804 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.865680 kgcnn-3.0.1/kgcnn/model/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/README.md
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/__init__.py
--rw-rw-rw-   0        0        0     8946 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/force.py
--rw-rw-rw-   0        0        0       18 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/serial.py
--rw-rw-rw-   0        0        0     5430 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/model/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.931681 kgcnn-3.0.1/kgcnn/molecule/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/__init__.py
--rw-rw-rw-   0        0        0    10057 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/base.py
--rw-rw-rw-   0        0        0    12505 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/convert.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.944678 kgcnn-3.0.1/kgcnn/molecule/dynamics/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/dynamics/__init__.py
--rw-rw-rw-   0        0        0     3911 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/dynamics/ase_calc.py
--rw-rw-rw-   0        0        0     8386 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/dynamics/base.py
--rw-rw-rw-   0        0        0     2556 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:54.960678 kgcnn-3.0.1/kgcnn/molecule/external/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/external/__init__.py
--rw-rw-rw-   0        0        0    20790 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/external/ballloon.py
--rw-rw-rw-   0        0        0    17892 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/graph_babel.py
--rw-rw-rw-   0        0        0    20750 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/graph_rdkit.py
--rw-rw-rw-   0        0        0     9149 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/io.py
--rw-rw-rw-   0        0        0     5105 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/methods.py
--rw-rw-rw-   0        0        0      702 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/molecule/serial.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.012679 kgcnn-3.0.1/kgcnn/ops/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/__init__.py
--rw-rw-rw-   0        0        0     3853 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/activ.py
--rw-rw-rw-   0        0        0     1483 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/axis.py
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/casting.py
--rw-rw-rw-   0        0        0     6991 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/initializer.py
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/numpy.py
--rw-rw-rw-   0        0        0     8292 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/partition.py
--rw-rw-rw-   0        0        0    10223 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/polynom.py
--rw-rw-rw-   0        0        0     3181 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/ragged.py
--rw-rw-rw-   0        0        0     1148 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/scatter.py
--rw-rw-rw-   0        0        0     2046 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/segment.py
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/ops/sorting.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.055678 kgcnn-3.0.1/kgcnn/training/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/callbacks.py
--rw-rw-rw-   0        0        0     4643 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/history.py
--rw-rw-rw-   0        0        0    14935 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/hyper.py
--rw-rw-rw-   0        0        0     8691 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/optimizer.py
--rw-rw-rw-   0        0        0     3945 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/schedule.py
--rw-rw-rw-   0        0        0    16405 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/training/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.076678 kgcnn-3.0.1/kgcnn/utils/
--rw-rw-rw-   0        0        0        1 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/devices.py
--rw-rw-rw-   0        0        0     7356 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/plots.py
--rw-rw-rw-   0        0        0     2310 2023-05-22 05:04:06.000000 kgcnn-3.0.1/kgcnn/utils/serial.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:53.503404 kgcnn-3.0.1/kgcnn.egg-info/
--rw-rw-rw-   0        0        0    19415 2023-05-22 14:57:52.000000 kgcnn-3.0.1/kgcnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2023-05-22 14:57:53.000000 kgcnn-3.0.1/kgcnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:57:52.000000 kgcnn-3.0.1/kgcnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      318 2023-05-22 14:57:52.000000 kgcnn-3.0.1/kgcnn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 14:57:53.000000 kgcnn-3.0.1/kgcnn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 14:57:55.144680 kgcnn-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1880 2023-05-22 05:04:06.000000 kgcnn-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:57:55.141679 kgcnn-3.0.1/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     4986 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_data_base.py
--rw-rw-rw-   0        0        0     7931 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_data_moleculenet.py
--rw-rw-rw-   0        0        0     1255 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_graph_base.py
--rw-rw-rw-   0        0        0     4149 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_graph_methods.py
--rw-rw-rw-   0        0        0     5135 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_attention.py
--rw-rw-rw-   0        0        0     4211 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_gather.py
--rw-rw-rw-   0        0        0     7647 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_geom.py
--rw-rw-rw-   0        0        0     2338 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_layers_pooling.py
--rw-rw-rw-   0        0        0     8078 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/test_range_periodic.py
--rw-rw-rw-   0        0        0      118 2023-05-22 05:04:06.000000 kgcnn-3.0.1/test/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.771590 kgcnn-3.0.2/
+-rw-rw-rw-   0        0        0       76 2023-08-01 05:47:44.000000 kgcnn-3.0.2/AUTHORS
+-rw-rw-rw-   0        0        0     1066 2023-08-01 05:47:44.000000 kgcnn-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-08-01 05:47:44.000000 kgcnn-3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    19415 2023-08-02 07:22:42.770591 kgcnn-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18539 2023-08-01 05:47:44.000000 kgcnn-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:40.904770 kgcnn-3.0.2/kgcnn/
+-rw-rw-rw-   0        0        0       43 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:40.961769 kgcnn-3.0.2/kgcnn/crystal/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/__init__.py
+-rw-rw-rw-   0        0        0     2930 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/base.py
+-rw-rw-rw-   0        0        0    33947 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/graph_builder.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:40.979770 kgcnn-3.0.2/kgcnn/crystal/periodic_table/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/periodic_table/__init__.py
+-rw-rw-rw-   0        0        0    15016 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/periodic_table/periodic_table.csv
+-rw-rw-rw-   0        0        0     4029 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/periodic_table/periodic_table.py
+-rw-rw-rw-   0        0        0    21221 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/crystal/preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.055769 kgcnn-3.0.2/kgcnn/data/
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/__init__.py
+-rw-rw-rw-   0        0        0    35033 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/base.py
+-rw-rw-rw-   0        0        0    12898 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/crystal.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.285770 kgcnn-3.0.2/kgcnn/data/datasets/
+-rw-rw-rw-   0        0        0     3036 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/ClinToxDataset.py
+-rw-rw-rw-   0        0        0     3186 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/CoraDataset.py
+-rw-rw-rw-   0        0        0     4761 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/CoraLuDataset.py
+-rw-rw-rw-   0        0        0     1559 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/ESOLDataset.py
+-rw-rw-rw-   0        0        0     1727 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/FreeSolvDataset.py
+-rw-rw-rw-   0        0        0     5398 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/GraphTUDataset2020.py
+-rw-rw-rw-   0        0        0     7113 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/ISO17Dataset.py
+-rw-rw-rw-   0        0        0     1471 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/LipopDataset.py
+-rw-rw-rw-   0        0        0     8792 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MD17Dataset.py
+-rw-rw-rw-   0        0        0     6574 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MD17RevisedDataset.py
+-rw-rw-rw-   0        0        0     3158 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MUTAGDataset.py
+-rw-rw-rw-   0        0        0    11255 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatBenchDataset2020.py
+-rw-rw-rw-   0        0        0     1469 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectDielectricDataset.py
+-rw-rw-rw-   0        0        0     1388 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectEFormDataset.py
+-rw-rw-rw-   0        0        0     1398 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectGapDataset.py
+-rw-rw-rw-   0        0        0     1424 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectIsMetalDataset.py
+-rw-rw-rw-   0        0        0     1325 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectJdft2dDataset.py
+-rw-rw-rw-   0        0        0     1605 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectLogGVRHDataset.py
+-rw-rw-rw-   0        0        0     1604 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectLogKVRHDataset.py
+-rw-rw-rw-   0        0        0     1316 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectPerovskitesDataset.py
+-rw-rw-rw-   0        0        0     1693 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MatProjectPhononsDataset.py
+-rw-rw-rw-   0        0        0     8589 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MoleculeNetDataset2018.py
+-rw-rw-rw-   0        0        0     4834 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/MutagenicityDataset.py
+-rw-rw-rw-   0        0        0     3051 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/PROTEINSDataset.py
+-rw-rw-rw-   0        0        0     6575 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/QM7Dataset.py
+-rw-rw-rw-   0        0        0     5533 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/QM7bDataset.py
+-rw-rw-rw-   0        0        0     3922 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/QM8Dataset.py
+-rw-rw-rw-   0        0        0    12272 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/QM9Dataset.py
+-rw-rw-rw-   0        0        0     2952 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/QM9MolNetDataset.py
+-rw-rw-rw-   0        0        0     2160 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/SIDERDataset.py
+-rw-rw-rw-   0        0        0     2194 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/Tox21MolNetDataset.py
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    12525 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/download.py
+-rw-rw-rw-   0        0        0    22994 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/moleculenet.py
+-rw-rw-rw-   0        0        0    17817 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/qm.py
+-rw-rw-rw-   0        0        0     2851 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/serial.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.288768 kgcnn-3.0.2/kgcnn/data/transform/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/base.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.323769 kgcnn-3.0.2/kgcnn/data/transform/scaler/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/scaler/__init__.py
+-rw-rw-rw-   0        0        0    19619 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/scaler/force.py
+-rw-rw-rw-   0        0        0    53863 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/scaler/molecule.py
+-rw-rw-rw-   0        0        0     1865 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/scaler/serial.py
+-rw-rw-rw-   0        0        0    28239 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/transform/scaler/standard.py
+-rw-rw-rw-   0        0        0     9408 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/tudataset.py
+-rw-rw-rw-   0        0        0     5311 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.362770 kgcnn-3.0.2/kgcnn/graph/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/__init__.py
+-rw-rw-rw-   0        0        0    26883 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/base.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.393767 kgcnn-3.0.2/kgcnn/graph/methods/
+-rw-rw-rw-   0        0        0     1365 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/methods/__init__.py
+-rw-rw-rw-   0        0        0    28421 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/methods/_adj.py
+-rw-rw-rw-   0        0        0    11983 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/methods/_geom.py
+-rw-rw-rw-   0        0        0    21305 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/methods/_periodic.py
+-rw-rw-rw-   0        0        0     1864 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/postprocessor.py
+-rw-rw-rw-   0        0        0    31335 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/preprocessor.py
+-rw-rw-rw-   0        0        0     2468 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/graph/serial.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.408769 kgcnn-3.0.2/kgcnn/io/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/io/__init__.py
+-rw-rw-rw-   0        0        0    10423 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/io/file.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/io/graphlist.py
+-rw-rw-rw-   0        0        0     4556 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/io/loader.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.559770 kgcnn-3.0.2/kgcnn/layers/
+-rw-rw-rw-   0        0        0     1181 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/README.md
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/activ.py
+-rw-rw-rw-   0        0        0    35560 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/aggr.py
+-rw-rw-rw-   0        0        0    15460 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/attention.py
+-rw-rw-rw-   0        0        0     7693 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/base.py
+-rw-rw-rw-   0        0        0    12507 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/casting.py
+-rw-rw-rw-   0        0        0    15136 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/conv.py
+-rw-rw-rw-   0        0        0    16510 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/gather.py
+-rw-rw-rw-   0        0        0    44934 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/geom.py
+-rw-rw-rw-   0        0        0     4735 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/message.py
+-rw-rw-rw-   0        0        0    18206 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/mlp.py
+-rw-rw-rw-   0        0        0    23477 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/modules.py
+-rw-rw-rw-   0        0        0    28771 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/norm.py
+-rw-rw-rw-   0        0        0    35808 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/pooling.py
+-rw-rw-rw-   0        0        0    11853 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/relational.py
+-rw-rw-rw-   0        0        0    13549 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/set2set.py
+-rw-rw-rw-   0        0        0     8702 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/layers/update.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.565769 kgcnn-3.0.2/kgcnn/literature/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.586768 kgcnn-3.0.2/kgcnn/literature/AttentiveFP/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/AttentiveFP/__init__.py
+-rw-rw-rw-   0        0        0    12186 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/AttentiveFP/_attentivefp_conv.py
+-rw-rw-rw-   0        0        0     5902 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/AttentiveFP/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.614771 kgcnn-3.0.2/kgcnn/literature/CGCNN/
+-rw-rw-rw-   0        0        0      130 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/CGCNN/__init__.py
+-rw-rw-rw-   0        0        0     6471 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/CGCNN/_cgcnn_conv.py
+-rw-rw-rw-   0        0        0     9358 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/CGCNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.626770 kgcnn-3.0.2/kgcnn/literature/CMPNN/
+-rw-rw-rw-   0        0        0       98 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/CMPNN/__init__.py
+-rw-rw-rw-   0        0        0     8126 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/CMPNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.652770 kgcnn-3.0.2/kgcnn/literature/DGIN/
+-rw-rw-rw-   0        0        0      100 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DGIN/__init__.py
+-rw-rw-rw-   0        0        0     4927 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DGIN/_dgin_conv.py
+-rw-rw-rw-   0        0        0    10250 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DGIN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.672770 kgcnn-3.0.2/kgcnn/literature/DMPNN/
+-rw-rw-rw-   0        0        0       98 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DMPNN/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DMPNN/_dmpnn_conv.py
+-rw-rw-rw-   0        0        0     8366 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DMPNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.694770 kgcnn-3.0.2/kgcnn/literature/DimeNetPP/
+-rw-rw-rw-   0        0        0      215 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DimeNetPP/__init__.py
+-rw-rw-rw-   0        0        0    19372 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DimeNetPP/_dimenet_conv.py
+-rw-rw-rw-   0        0        0    18270 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/DimeNetPP/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.706769 kgcnn-3.0.2/kgcnn/literature/EGNN/
+-rw-rw-rw-   0        0        0       98 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/EGNN/__init__.py
+-rw-rw-rw-   0        0        0    10063 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/EGNN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.711769 kgcnn-3.0.2/kgcnn/literature/GAT/
+-rw-rw-rw-   0        0        0       98 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GAT/__init__.py
+-rw-rw-rw-   0        0        0     5925 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GAT/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.724769 kgcnn-3.0.2/kgcnn/literature/GATv2/
+-rw-rw-rw-   0        0        0       98 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GATv2/__init__.py
+-rw-rw-rw-   0        0        0     6279 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GATv2/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.743770 kgcnn-3.0.2/kgcnn/literature/GCN/
+-rw-rw-rw-   0        0        0      218 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GCN/__init__.py
+-rw-rw-rw-   0        0        0     1874 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GCN/_gcn_conv.py
+-rw-rw-rw-   0        0        0    10192 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GCN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.791284 kgcnn-3.0.2/kgcnn/literature/GIN/
+-rw-rw-rw-   0        0        0      202 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GIN/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GIN/_gin_conv.py
+-rw-rw-rw-   0        0        0    10899 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GIN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.830284 kgcnn-3.0.2/kgcnn/literature/GNNExplain/
+-rw-rw-rw-   0        0        0      187 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/__init__.py
+-rw-rw-rw-   0        0        0    30109 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_model.py
+-rw-rw-rw-   0        0        0     1262 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py
+-rw-rw-rw-   0        0        0     1134 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_xai_base.py
+-rw-rw-rw-   0        0        0      933 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_xai_testing.py
+-rw-rw-rw-   0        0        0      565 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_xai_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.850284 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/_base.py
+-rw-rw-rw-   0        0        0     4459 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/_testing.py
+-rw-rw-rw-   0        0        0      774 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.861284 kgcnn-3.0.2/kgcnn/literature/GNNFilm/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNFilm/__init__.py
+-rw-rw-rw-   0        0        0     5606 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GNNFilm/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.862285 kgcnn-3.0.2/kgcnn/literature/GemNet/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GemNet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.866282 kgcnn-3.0.2/kgcnn/literature/GraphSAGE/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GraphSAGE/__init__.py
+-rw-rw-rw-   0        0        0     6836 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/GraphSAGE/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.904283 kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/
+-rw-rw-rw-   0        0        0      454 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/__init__.py
+-rw-rw-rw-   0        0        0    25733 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/_acsf_conv.py
+-rw-rw-rw-   0        0        0    15739 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/_make.py
+-rw-rw-rw-   0        0        0    21072 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/_wacsf_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.940283 kgcnn-3.0.2/kgcnn/literature/HDNNP4th/
+-rw-rw-rw-   0        0        0      127 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP4th/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP4th/_hdnnp_conv.py
+-rw-rw-rw-   0        0        0     8160 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP4th/_make.py
+-rw-rw-rw-   0        0        0     9442 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HDNNP4th/_test_hdnnp.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.964283 kgcnn-3.0.2/kgcnn/literature/HamNet/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HamNet/__init__.py
+-rw-rw-rw-   0        0        0    28565 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HamNet/_hamnet_conv.py
+-rw-rw-rw-   0        0        0     8210 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/HamNet/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.969284 kgcnn-3.0.2/kgcnn/literature/INorp/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/INorp/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/INorp/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:41.988284 kgcnn-3.0.2/kgcnn/literature/MAT/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MAT/__init__.py
+-rw-rw-rw-   0        0        0     9724 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MAT/_make.py
+-rw-rw-rw-   0        0        0     8758 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MAT/_mat_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.025281 kgcnn-3.0.2/kgcnn/literature/MEGAN/
+-rw-rw-rw-   0        0        0      218 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MEGAN/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MEGAN/_make.py
+-rw-rw-rw-   0        0        0    22759 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MEGAN/_model.py
+-rw-rw-rw-   0        0        0     6903 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MEGAN/_test_literature_megan.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.045283 kgcnn-3.0.2/kgcnn/literature/MXMNet/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MXMNet/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MXMNet/_make.py
+-rw-rw-rw-   0        0        0     8490 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MXMNet/_mxmnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.108326 kgcnn-3.0.2/kgcnn/literature/Megnet/
+-rw-rw-rw-   0        0        0      215 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Megnet/__init__.py
+-rw-rw-rw-   0        0        0    18509 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Megnet/_make.py
+-rw-rw-rw-   0        0        0     7153 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Megnet/_megnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.131698 kgcnn-3.0.2/kgcnn/literature/MoGAT/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MoGAT/__init__.py
+-rw-rw-rw-   0        0        0     6679 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MoGAT/_make.py
+-rw-rw-rw-   0        0        0    12206 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/MoGAT/_mogat_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.145558 kgcnn-3.0.2/kgcnn/literature/NMPN/
+-rw-rw-rw-   0        0        0      215 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/NMPN/__init__.py
+-rw-rw-rw-   0        0        0    17202 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/NMPN/_make.py
+-rw-rw-rw-   0        0        0     4753 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/NMPN/_mpnn_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.166555 kgcnn-3.0.2/kgcnn/literature/PAiNN/
+-rw-rw-rw-   0        0        0      215 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/PAiNN/__init__.py
+-rw-rw-rw-   0        0        0    14386 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/PAiNN/_make.py
+-rw-rw-rw-   0        0        0    15618 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/PAiNN/_painn_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.178517 kgcnn-3.0.2/kgcnn/literature/RGCN/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/RGCN/__init__.py
+-rw-rw-rw-   0        0        0     5668 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/RGCN/_make.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.213560 kgcnn-3.0.2/kgcnn/literature/Schnet/
+-rw-rw-rw-   0        0        0      215 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Schnet/__init__.py
+-rw-rw-rw-   0        0        0    14260 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Schnet/_make.py
+-rw-rw-rw-   0        0        0     8445 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Schnet/_schnet_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.246560 kgcnn-3.0.2/kgcnn/literature/Unet/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Unet/__init__.py
+-rw-rw-rw-   0        0        0     7194 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Unet/_make.py
+-rw-rw-rw-   0        0        0     1138 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Unet/_test_connect.py
+-rw-rw-rw-   0        0        0     4157 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Unet/_test_topk.py
+-rw-rw-rw-   0        0        0    19977 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/Unet/_topk.py
+-rw-rw-rw-   0        0        0       51 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.323562 kgcnn-3.0.2/kgcnn/literature/coGN/
+-rw-rw-rw-   0        0        0     2873 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/__init__.py
+-rw-rw-rw-   0        0        0     7496 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_coGN_config.py
+-rw-rw-rw-   0        0        0     6429 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_coNGN_config.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.341571 kgcnn-3.0.2/kgcnn/literature/coGN/_embedding_layers/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_embedding_layers/__init__.py
+-rw-rw-rw-   0        0        0     4218 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py
+-rw-rw-rw-   0        0        0     6719 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py
+-rw-rw-rw-   0        0        0      891 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_gates.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.363571 kgcnn-3.0.2/kgcnn/literature/coGN/_graph_network/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_graph_network/__init__.py
+-rw-rw-rw-   0        0        0    16183 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_graph_network/graph_network_base.py
+-rw-rw-rw-   0        0        0    23941 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_graph_network/graph_networks.py
+-rw-rw-rw-   0        0        0    27901 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_make.py
+-rw-rw-rw-   0        0        0     2266 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_multiplicity_readout.py
+-rw-rw-rw-   0        0        0     3945 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_preprocessing_layers.py
+-rw-rw-rw-   0        0        0     1051 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_test.py
+-rw-rw-rw-   0        0        0      372 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/coGN/_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.388344 kgcnn-3.0.2/kgcnn/literature/rGIN/
+-rw-rw-rw-   0        0        0       99 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/rGIN/__init__.py
+-rw-rw-rw-   0        0        0     5444 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/rGIN/_make.py
+-rw-rw-rw-   0        0        0     3502 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/literature/rGIN/_rgin_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.405623 kgcnn-3.0.2/kgcnn/metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/metrics/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/metrics/loss.py
+-rw-rw-rw-   0        0        0    10804 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.429624 kgcnn-3.0.2/kgcnn/model/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/model/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/model/__init__.py
+-rw-rw-rw-   0        0        0    10551 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/model/force.py
+-rw-rw-rw-   0        0        0     1195 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/model/multi.py
+-rw-rw-rw-   0        0        0       18 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/model/serial.py
+-rw-rw-rw-   0        0        0     5430 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/model/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.504588 kgcnn-3.0.2/kgcnn/molecule/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/__init__.py
+-rw-rw-rw-   0        0        0    10057 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/base.py
+-rw-rw-rw-   0        0        0    12505 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/convert.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.524588 kgcnn-3.0.2/kgcnn/molecule/dynamics/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/dynamics/__init__.py
+-rw-rw-rw-   0        0        0     3911 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/dynamics/ase_calc.py
+-rw-rw-rw-   0        0        0     8386 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/dynamics/base.py
+-rw-rw-rw-   0        0        0     2556 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/encoder.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.539590 kgcnn-3.0.2/kgcnn/molecule/external/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/external/__init__.py
+-rw-rw-rw-   0        0        0    20790 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/external/ballloon.py
+-rw-rw-rw-   0        0        0    17892 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/graph_babel.py
+-rw-rw-rw-   0        0        0    20750 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/graph_rdkit.py
+-rw-rw-rw-   0        0        0     9149 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/io.py
+-rw-rw-rw-   0        0        0     5105 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/methods.py
+-rw-rw-rw-   0        0        0      702 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/molecule/serial.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.610590 kgcnn-3.0.2/kgcnn/ops/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/activ.py
+-rw-rw-rw-   0        0        0     1483 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/axis.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/casting.py
+-rw-rw-rw-   0        0        0     6991 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/initializer.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/numpy.py
+-rw-rw-rw-   0        0        0     8292 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/partition.py
+-rw-rw-rw-   0        0        0    10223 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/polynom.py
+-rw-rw-rw-   0        0        0     3181 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/ragged.py
+-rw-rw-rw-   0        0        0     1148 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/scatter.py
+-rw-rw-rw-   0        0        0     2142 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/segment.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/ops/sorting.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.667590 kgcnn-3.0.2/kgcnn/training/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/__init__.py
+-rw-rw-rw-   0        0        0     1345 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/callbacks.py
+-rw-rw-rw-   0        0        0     4836 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/history.py
+-rw-rw-rw-   0        0        0    14960 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/hyper.py
+-rw-rw-rw-   0        0        0     8691 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/optimizer.py
+-rw-rw-rw-   0        0        0     3945 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/schedule.py
+-rw-rw-rw-   0        0        0    20040 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/training/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.688593 kgcnn-3.0.2/kgcnn/utils/
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/utils/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/utils/devices.py
+-rw-rw-rw-   0        0        0     7356 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/utils/plots.py
+-rw-rw-rw-   0        0        0     2310 2023-08-01 05:47:44.000000 kgcnn-3.0.2/kgcnn/utils/serial.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:40.938770 kgcnn-3.0.2/kgcnn.egg-info/
+-rw-rw-rw-   0        0        0    19415 2023-08-02 07:22:40.000000 kgcnn-3.0.2/kgcnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8418 2023-08-02 07:22:40.000000 kgcnn-3.0.2/kgcnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:22:40.000000 kgcnn-3.0.2/kgcnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      325 2023-08-02 07:22:40.000000 kgcnn-3.0.2/kgcnn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 07:22:40.000000 kgcnn-3.0.2/kgcnn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:22:42.771590 kgcnn-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1887 2023-08-01 05:47:44.000000 kgcnn-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:22:42.768591 kgcnn-3.0.2/test/
+-rw-rw-rw-   0        0        0        0 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     4986 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_data_base.py
+-rw-rw-rw-   0        0        0     7931 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_data_moleculenet.py
+-rw-rw-rw-   0        0        0     1255 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_graph_base.py
+-rw-rw-rw-   0        0        0     4149 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_graph_methods.py
+-rw-rw-rw-   0        0        0     8078 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_graph_methods_periodic.py
+-rw-rw-rw-   0        0        0     5184 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_layers_attention.py
+-rw-rw-rw-   0        0        0     4229 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_layers_gather.py
+-rw-rw-rw-   0        0        0     7647 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_layers_geom.py
+-rw-rw-rw-   0        0        0     2338 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/test_layers_pooling.py
+-rw-rw-rw-   0        0        0      118 2023-08-01 05:47:44.000000 kgcnn-3.0.2/test/utils.py
```

### Comparing `kgcnn-3.0.1/LICENSE` & `kgcnn-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/PKG-INFO` & `kgcnn-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgcnn
-Version: 3.0.1
+Version: 3.0.2
 Summary: General Base Layers for Graph Convolutions with tensorflow.keras
 Home-page: https://github.com/aimat-lab/gcnn_keras
 Author: Patrick Reiser
 Author-email: patrick.reiser@kit.edu
 License: UNKNOWN
 Keywords: materials,science,machine,learning,deep,graph,networks,neural
 Platform: UNKNOWN
```

### Comparing `kgcnn-3.0.1/README.md` & `kgcnn-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/crystal/base.py` & `kgcnn-3.0.2/kgcnn/crystal/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     edge_attributes = []
     graph_attributes = []
 
     def __init__(self, output_graph_as_dict: bool = False):
         self.output_graph_as_dict = output_graph_as_dict
 
     def call(self, structure: Structure) -> MultiDiGraph:
-        """Should be implemented in a subclass.
+        r"""Should be implemented in a subclass.
 
         Args:
             structure (Structure): Crystal for which the graph representation should be calculated.
 
         Raises:
             NotImplementedError:Should be implemented in a subclass.
 
         Returns:
             MultiDiGraph: Graph representation of the crystal.
         """
         raise NotImplementedError("Must be implemented in sub-classes.")
 
     def __call__(self, structure: Structure) -> Union[MultiDiGraph, GraphDict]:
-        """Should be implemented in a subclass.
+        r"""Function to process crystal structures. Executes :obj:`call` .
 
         Args:
             structure (Structure): Crystal for which the graph representation should be calculated.
 
         Raises:
             NotImplementedError:Should be implemented in a subclass.
```

### Comparing `kgcnn-3.0.1/kgcnn/crystal/graph_builder.py` & `kgcnn-3.0.2/kgcnn/crystal/graph_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,18 +131,18 @@
         inplace (bool, optional): Whether to add the edges to the given graph or create a copy with added edges.
             Defaults to False.
 
     Returns:
         MultiDiGraph: Graph with added edges.
     """
     lattice = _get_attr_from_graph(graph, "lattice_matrix", make_copy=True)
-    # if max_radius is None:
-    #     max_radius = _estimate_radius_from_density(lattice)
     frac_coords = np.array([data[1] for data in graph.nodes(data='frac_coords')])
     coords = frac_coords @ lattice
+    if max_radius is None:
+        max_radius = _estimate_nn_radius_from_density(k, coords, lattice, 0.1)
     # return coords, lattice
     index1, index2, offset_vectors, distances = find_points_in_spheres(
         coords,
         coords,
         r=max_radius,
         pbc=np.array([True] * 3, dtype=int),
         lattice=lattice,
@@ -544,17 +544,21 @@
 
     Returns:
         MultiDiGraph: Corresponding asymmetric unit graph for the given unit cell graph.
     """
 
     asymmetric_mapping = np.array([node[1] for node in graph.nodes(data='asymmetric_mapping')])
     if None in asymmetric_mapping:
-        raise ValueError("Graph does not contain symmetry informations. \
-Make sure to create the graph with `structure_to_empty_graph` with the `symmetrize` \
-argument set to `True`.")
+        raise ValueError(
+            "".join([
+                "Graph does not contain symmetry information. ",
+                "Make sure to create the graph with `structure_to_empty_graph` ",
+                "with the `symmetrize` argument set to `True` ."
+            ])
+        )
     asu_node_indice, inv_asymmetric_mapping = np.unique(asymmetric_mapping, return_inverse=True)
 
     asu_graph = MultiDiGraph()
     setattr(asu_graph, 'lattice_matrix', _get_attr_from_graph(graph, "lattice_matrix"))
     setattr(asu_graph, 'spacegroup', _get_attr_from_graph(graph, "spacegroup"))
     new_nodes_idx = {}
 
@@ -621,15 +625,16 @@
     Args:
         coords1 (np.ndarray): Coordinates of shape (..., n, 3)
         coords2 (np.ndarray): Coordinates of shape (..., m, 3)
 
     Returns:
         np.ndarray: Difference values of shape (..., n, m, 3)
     """
-
+    # This can be solved more elegantly with normal broadcasting
+    # TODO: Check if the same.
     def _reshape_at_axis(arr, axis, new_shape):
         # move reshape axis to last axis position, because np.reshape reshapes this first
         arr_tmp = np.moveaxis(arr, axis, -1)
         shape = arr_tmp.shape[:-1] + new_shape
         new_positions = np.arange(len(new_shape)) + axis
         old_positions = np.arange(len(new_shape)) + (len(arr.shape) - 1)
         # now call np.reshape and move axis to right position
@@ -748,7 +753,48 @@
         if make_copy:
             out = deepcopy(getattr(graph, attr_name))
         else:
             out = getattr(graph, attr_name)
     else:
         raise AttributeError("Must attach attribute '%s' of crystal information to networkx graph." % attr_name)
     return out
+
+
+def _estimate_nn_radius_from_density(k: int, coordinates: np.ndarray, lattice: np.ndarray,
+                                     empirical_tol_factor: float = 0.0):
+    """Rough estimate of the expected radius to find N nearest neighbours.
+
+    Args:
+        k (int): Number of neighbours.
+        coordinates (np.ndarray): Coordinates array.
+        lattice (np.ndarray): Lattice matrix.
+        empirical_tol_factor (float): Tolerance factor for radius.
+
+    Returns:
+        float: estimated radius
+    """
+    volume_unit_cell = np.sum(np.abs(np.cross(lattice[0], lattice[1]) * lattice[2]))
+    density_unit_cell = len(coordinates) / volume_unit_cell
+    estimated_nn_volume = k / density_unit_cell  # + len(coordinates)/density_unit_cell
+    estimated_nn_radius = abs(float(np.cbrt(estimated_nn_volume / np.pi * 3 / 4)))
+    estimated_nn_radius = estimated_nn_radius * (1.0 + empirical_tol_factor)
+    return estimated_nn_radius
+
+
+def _get_geometric_properties_of_unit_cell(coordinates: np.ndarray, lattice: np.ndarray):
+    """Diameter of a 3D unit cell and other properties.
+
+    Args:
+        coordinates (np.ndarray): Coordinates array.
+        lattice (np.ndarray): Lattice matrix.
+
+    Returns:
+        tuple: (center_unit_cell, max_diameter_cell, volume_unit_cell, density_unit_cell)
+    """
+    # lattice_col = np.transpose(lattice)
+    lattice_row = lattice
+    center_unit_cell = np.sum(lattice_row, axis=0, keepdims=True) / 2  # (1, 3)
+    max_radius_cell = np.amax(np.sqrt(np.sum(np.square(lattice_row - center_unit_cell), axis=-1)))
+    max_diameter_cell = 2 * max_radius_cell
+    volume_unit_cell = np.sum(np.abs(np.cross(lattice[0], lattice[1]) * lattice[2]))
+    density_unit_cell = len(coordinates) / volume_unit_cell
+    return center_unit_cell[0], max_diameter_cell, volume_unit_cell, density_unit_cell
```

### Comparing `kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.csv` & `kgcnn-3.0.2/kgcnn/crystal/periodic_table/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/crystal/periodic_table/periodic_table.py` & `kgcnn-3.0.2/kgcnn/crystal/periodic_table/periodic_table.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/crystal/preprocessor.py` & `kgcnn-3.0.2/kgcnn/crystal/preprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/base.py` & `kgcnn-3.0.2/kgcnn/data/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/crystal.py` & `kgcnn-3.0.2/kgcnn/data/crystal.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
         self._map_callbacks(structs=self.get_structures_from_json_file(),
                             data=self.read_in_table_file(file_path=self.file_path).data_frame,
                             callbacks=callbacks)
 
         return self
 
-    def set_representation(self, pre_processor: CrystalPreprocessor, reset_graphs: bool = False):
+    def set_representation(self, pre_processor: Union[CrystalPreprocessor, dict], reset_graphs: bool = False):
         r"""Build a graph representation for this dataset using :obj:`kgcnn.crystal` .
 
         Args:
             pre_processor (CrystalPreprocessor): Crystal preprocessor to use.
             reset_graphs (bool): Whether to reset the graph information. Default is False.
 
         Returns:
```

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/ClinToxDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/ClinToxDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/CoraDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/CoraDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/CoraLuDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/CoraLuDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/ESOLDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/ESOLDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/FreeSolvDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/FreeSolvDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/GraphTUDataset2020.py` & `kgcnn-3.0.2/kgcnn/data/datasets/GraphTUDataset2020.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/ISO17Dataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/ISO17Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/LipopDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/LipopDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MD17Dataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MD17Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MD17RevisedDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MD17RevisedDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MUTAGDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MUTAGDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatBenchDataset2020.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatBenchDataset2020.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectDielectricDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectDielectricDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectEFormDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectEFormDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectGapDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectGapDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectIsMetalDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectIsMetalDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectJdft2dDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectJdft2dDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogGVRHDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectLogGVRHDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectLogKVRHDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectLogKVRHDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPerovskitesDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectPerovskitesDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MatProjectPhononsDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MatProjectPhononsDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MoleculeNetDataset2018.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MoleculeNetDataset2018.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/MutagenicityDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/MutagenicityDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/PROTEINSDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/PROTEINSDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/QM7Dataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/QM7Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/QM7bDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/QM7bDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/QM8Dataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/QM8Dataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/QM9Dataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/QM9Dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     and 10% test set are used. In literature, test errors are given as MAE and for energies are in [eV].
 
     Molecules that have a different smiles code after convergence can be removed with :obj:`remove_uncharacterized` .
     Also labels with removed atomization energy are generated.
 
     .. code-block:: python
 
-        from kgcnn.data.qm import QM9Dataset
+        from kgcnn.data.datasets.QM9Dataset import QM9Dataset
         dataset = QM9Dataset(reload=True)
         print(dataset[0])
 
     References:
 
         (1) L. Ruddigkeit, R. van Deursen, L. C. Blum, J.-L. Reymond, Enumeration of 166 billion organic small
             molecules in the chemical universe database GDB-17, J. Chem. Inf. Model. 52, 2864–2875, 2012.
```

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/QM9MolNetDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/QM9MolNetDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/SIDERDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/SIDERDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/datasets/Tox21MolNetDataset.py` & `kgcnn-3.0.2/kgcnn/data/datasets/Tox21MolNetDataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/download.py` & `kgcnn-3.0.2/kgcnn/data/download.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/moleculenet.py` & `kgcnn-3.0.2/kgcnn/data/moleculenet.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/qm.py` & `kgcnn-3.0.2/kgcnn/data/qm.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/serial.py` & `kgcnn-3.0.2/kgcnn/data/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/transform/scaler/force.py` & `kgcnn-3.0.2/kgcnn/data/transform/scaler/force.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/transform/scaler/molecule.py` & `kgcnn-3.0.2/kgcnn/data/transform/scaler/molecule.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/transform/scaler/serial.py` & `kgcnn-3.0.2/kgcnn/data/transform/scaler/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/transform/scaler/standard.py` & `kgcnn-3.0.2/kgcnn/data/transform/scaler/standard.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,74 +7,68 @@
 
 
 logging.basicConfig()  # Module logger
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 
-class StandardScalerSklearnBase(StandardScalerSklearn):
-    r"""Base standard scaler of :obj:`sklearn` with added functionality to save and load weights of this scaler similar
-    to keras layers and objects.
+class _StandardScalerSklearnMixin:
+    r"""Mixin class for scaler of :obj:`sklearn` with added functionality to save and load weights of a scaler
+    similar to keras layers and objects.
 
-    .. code-block:: python
+    .. note::
 
-        import numpy as np
-        from kgcnn.data.transform.scaler.standard import StandardScalerSklearnBase
-        data = np.random.rand(5).reshape((5,1))
-        scaler = StandardScalerSklearnBase()
-        scaler.fit(X=data)
-        print(scaler.get_weights())
-        print(scaler.get_config())
+        This class is only meant to add functionality. Scaler is accessed via :obj:`_scaler_reference` property.
 
     """
     _attributes_list_sklearn = ["n_features_in_", "mean_", "scale_", "var_", "feature_names_in_", "n_samples_seen_"]
 
-    def __init__(self, *, copy=True, with_mean=True, with_std=True):
-        super(StandardScalerSklearnBase, self).__init__(copy=copy, with_mean=with_mean, with_std=with_std)
+    def __init__(self):
+        self._scaler_reference = None
 
     def get_scaling(self):
         """Get scale of shape (1, n_properties)."""
-        if not hasattr(self, "scale_"):
+        if not hasattr(self._scaler_reference, "scale_"):
             return
-        scale = np.array(self.scale_)
+        scale = np.array(self._scaler_reference.scale_)
         scale = np.expand_dims(scale, axis=0)
         return scale
 
     def get_config(self) -> dict:
         """Get configuration for scaler."""
-        config = super(StandardScalerSklearnBase, self).get_params()
+        config = self._scaler_reference.get_params()
         return config
 
     def set_config(self, config: dict):
         """Set configuration for scaler.
 
         Args:
             config (dict): Config dictionary.
         """
-        self.set_params(**config)
+        self._scaler_reference.set_params(**config)
 
     def get_weights(self) -> dict:
         """Get weights for this scaler after fit."""
         weight_dict = dict()
         for x in self._attributes_list_sklearn:
-            if hasattr(self, x):
-                value = getattr(self, x)
+            if hasattr(self._scaler_reference, x):
+                value = getattr(self._scaler_reference, x)
                 value_update = {x: np.array(value).tolist()} if value is not None else {x: value}
                 weight_dict.update(value_update)
         return weight_dict
 
     def set_weights(self, weights: dict):
         """Set weights for this scaler.
 
         Args:
             weights (dict): Weight dictionary.
         """
         for item, value in weights.items():
             if item in self._attributes_list_sklearn:
-                setattr(self, item, np.array(value))
+                setattr(self._scaler_reference, item, np.array(value))
             else:
                 module_logger.warning("`StandardScaler` got unknown weight '%s'." % item)
 
     def save_weights(self, file_path: str):
         """Save weights as numpy to file.
 
         Args:
@@ -126,15 +120,15 @@
             X (str): Name of X information in dataset. For example "graph_properties".
             y (str): Not used.
             sample_weight (str): Name of sample weight information in dataset. For example "sample_weight".
 
         Returns:
             self.
         """
-        return super(StandardScalerSklearnBase, self).fit(
+        return self._scaler_reference.fit(
             [item[X] for item in dataset],
             # We can ignore y here. None is default for sklearn StandardScaler.
             # y=None
             sample_weight=[item[sample_weight] for item in dataset] if sample_weight is not None else None
         )
 
     # noinspection PyPep8Naming
@@ -152,15 +146,15 @@
             copy_dataset (bool): Whether to copy full dataset. Default is False.
 
         Returns:
             dataset: Transformed dataset.
         """
         if copy_dataset:
             dataset = dataset.copy()
-        out = super(StandardScalerSklearnBase, self).transform(
+        out = self._scaler_reference.transform(
             [graph[X] for graph in dataset],
             copy=copy,
         )
         for graph, out_value in zip(dataset, out):
             graph[X] = out_value
         return dataset
 
@@ -179,15 +173,15 @@
             copy_dataset (bool): Whether to copy full dataset. Default is False.
 
         Returns:
             dataset: Inverse-transformed dataset.
         """
         if copy_dataset:
             dataset = dataset.copy()
-        out = super(StandardScalerSklearnBase, self).inverse_transform(
+        out = self._scaler_reference.inverse_transform(
             [graph[X] for graph in dataset],
             copy=copy,
         )
         for graph, out_value in zip(dataset, out):
             graph[X] = out_value
         return dataset
 
@@ -212,15 +206,15 @@
         Returns:
             dataset: Transformed dataset.
         """
         self.fit_dataset(dataset=dataset, X=X, y=y, sample_weight=sample_weight)
         return self.transform_dataset(dataset=dataset, X=X, copy=copy, copy_dataset=copy_dataset)
 
 
-class StandardScaler(StandardScalerSklearnBase):
+class StandardScaler(StandardScalerSklearn, _StandardScalerSklearnMixin):
     r"""Standard scaler that inherits from :obj:`sklearn.preprocessing.StandardScaler` .
     Included unused kwarg 'atomic_number' to be compatible with some material oriented scaler.
 
     .. code-block:: python
 
         import numpy as np
         from kgcnn.data.transform.scaler.standard import StandardScaler
@@ -233,14 +227,17 @@
         print(data)
         scaler.save("example.json")
         new_scaler = StandardScaler()
         new_scaler.load("example.json")
         print(new_scaler.inverse_transform(scaler.transform(X=data)))
 
     """
+    def __init__(self, *, copy=True, with_mean=True, with_std=True):
+        super(StandardScaler, self).__init__(copy=copy, with_mean=with_mean, with_std=with_std)
+        self._scaler_reference = self
 
     # noinspection PyPep8Naming
     def fit(self, X, *, y=None, sample_weight=None, atomic_number=None):
         """Compute the mean and std to be used for later scaling.
 
         Args:
             X (np.ndarray): Array of shape (n_samples, n_features)
@@ -412,16 +409,16 @@
         Returns:
             dataset: Transformed dataset.
         """
         self.fit_dataset(dataset=dataset, X=X, y=y, sample_weight=sample_weight)
         return self.transform_dataset(dataset=dataset, X=X, copy=copy, copy_dataset=copy_dataset)
 
 
-class StandardLabelScaler(StandardScalerSklearnBase):
-    r"""Standard scaler for labels that inherits from :obj:`sklearn.preprocessing.StandardScaler` .
+class StandardLabelScaler(_StandardScalerSklearnMixin):
+    r"""Standard scaler for labels that has a member of :obj:`sklearn.preprocessing.StandardScaler` .
     Included unused kwarg 'atomic_number' to be compatible with some material oriented scaler.
     Uses `y` argument for scaling labels and `X` is ignored.
 
     .. code-block:: python
 
         import numpy as np
         from kgcnn.data.transform.scaler.standard import StandardLabelScaler
@@ -436,14 +433,18 @@
         scaler.save("example.json")
         new_scaler = StandardLabelScaler()
         new_scaler.load("example.json")
         print(new_scaler.inverse_transform(y=scaler.transform(y=data)))
 
     """
 
+    def __init__(self, *, copy=True, with_mean=True, with_std=True):
+        super(StandardLabelScaler, self).__init__()
+        self._scaler_reference = StandardScalerSklearn(copy=copy, with_mean=with_mean, with_std=with_std)
+
     def _validate_input(self, y, x):
         if x is not None and y is None:
             raise ValueError(
                 "Got X but y is 'None' for `%s`. Report this issue if sklearn API change. " % type(self).__name__)
         if y is None and x is None:
             raise ValueError(
                 "Require labels as `y` for `%s`. Input must be e.g. 'fit(data)'." % type(self).__name__)
@@ -461,16 +462,15 @@
             atomic_number (list): Ignored.
 
         Returns:
             self: Fitted scaler.
         """
         # fit() of sklearn uses reset and partial fit. Just adding y in place of X.
         self._validate_input(y, X)
-        self._reset()
-        return super(StandardLabelScaler, self).partial_fit(X=y, sample_weight=sample_weight)
+        return self._scaler_reference.fit(X=y, sample_weight=sample_weight)
 
     # noinspection PyPep8Naming
     def partial_fit(self, y: np.ndarray, X=None, sample_weight=None, atomic_number=None):
         r"""Online computation of mean and std on y for later scaling.
         All of y is processed as a single batch. This is intended for cases
         when :meth:`fit` is not feasible due to very large number of
         `n_samples` or because y is read from a continuous stream.
@@ -488,15 +488,15 @@
         Returns:
             self: Fitted scaler.
         """
         # For partial fit internally uses args and not kwargs.
         # Can not request kwargs after argument X, y here.
         # Just changing order of x,y here.
         self._validate_input(y, X)
-        return super(StandardLabelScaler, self).partial_fit(X=y, sample_weight=sample_weight)
+        return self._scaler_reference.partial_fit(X=y, sample_weight=sample_weight)
 
     # noinspection PyPep8Naming
     def fit_transform(self, y: np.ndarray, *, X=None, atomic_number=None, copy=None, **fit_params):
         r"""Perform fit and standardization by centering and scaling.
 
         Args:
             y (np.ndarray): Array of shape (n_samples, n_labels)
@@ -524,15 +524,15 @@
             atomic_number (list): Ignored.
             copy (bool): Copy the input `y` or not.
 
         Returns:
             y_tr (np.ndarray): Transformed array of shape (n_samples, n_labels).
         """
         # Just changing order of x,y here.
-        return super(StandardLabelScaler, self).transform(y, copy=copy)
+        return self._scaler_reference.transform(y, copy=copy)
 
     # noinspection PyPep8Naming
     def inverse_transform(self, y: np.ndarray = None, *, X=None, copy: bool = None, atomic_number=None):
         r"""Scale back the data to the original representation.
 
         Args:
             y (None): Array of shape (n_samples, n_labels)
@@ -541,15 +541,15 @@
             atomic_number (list): Ignored.
             copy (bool): Copy the input `y` or not.
 
         Returns:
             y_tr (np.ndarray): Transformed array of shape (n_samples, n_labels).
         """
         # Just changing order of x,y here.
-        return super(StandardLabelScaler, self).inverse_transform(y, copy=copy)
+        return self._scaler_reference.inverse_transform(y, copy=copy)
 
     # Similar functions that work on dataset plus property names.
     # noinspection PyPep8Naming
     def fit_dataset(self, dataset: List[Dict[str, np.ndarray]],
                     y: str = None, *,
                     X: str = None,
                     atomic_number: str = None,
```

### Comparing `kgcnn-3.0.1/kgcnn/data/tudataset.py` & `kgcnn-3.0.2/kgcnn/data/tudataset.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/data/utils.py` & `kgcnn-3.0.2/kgcnn/data/utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/graph/base.py` & `kgcnn-3.0.2/kgcnn/graph/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/graph/methods/__init__.py` & `kgcnn-3.0.2/kgcnn/graph/methods/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from ._adj import (
     get_angle_indices, coordinates_to_distancematrix, invert_distance,
     define_adjacency_from_distance, sort_edge_indices, get_angle, add_edges_reverse_indices,
     rescale_edge_weights_degree_sym, add_self_loops_to_edge_indices, compute_reverse_edges_index_map,
     distance_to_gauss_basis, get_angle_between_edges, convert_scaled_adjacency_to_list
 )
 from ._geom import (
-    range_neighbour_lattice, get_principal_moments_of_inertia,
+    get_principal_moments_of_inertia,
     shift_coordinates_to_unit_cell, distance_for_range_indices, distance_for_range_indices_periodic,
     coulomb_matrix_to_inverse_distance_proton, coordinates_from_distance_matrix
 )
+from ._periodic import (
+    range_neighbour_lattice
+)
 
 __all__ = [
     # adj
     "get_angle_indices", "coordinates_to_distancematrix", "invert_distance",
     "define_adjacency_from_distance", "sort_edge_indices", "get_angle", "add_edges_reverse_indices",
     "rescale_edge_weights_degree_sym", "add_self_loops_to_edge_indices", "compute_reverse_edges_index_map",
     "distance_to_gauss_basis", "get_angle_between_edges", "convert_scaled_adjacency_to_list",
     # geom
-    "range_neighbour_lattice", "get_principal_moments_of_inertia",
+    "get_principal_moments_of_inertia",
     "shift_coordinates_to_unit_cell", "distance_for_range_indices", "distance_for_range_indices_periodic",
-    "coulomb_matrix_to_inverse_distance_proton", "coordinates_from_distance_matrix"
+    "coulomb_matrix_to_inverse_distance_proton", "coordinates_from_distance_matrix",
+    # periodic
+    "range_neighbour_lattice"
 ]
```

### Comparing `kgcnn-3.0.1/kgcnn/graph/methods/_adj.py` & `kgcnn-3.0.2/kgcnn/graph/methods/_adj.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/graph/methods/_geom.py` & `kgcnn-3.0.2/kgcnn/graph/methods/_periodic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,188 +1,204 @@
 import numpy as np
 from typing import Union
+from pymatgen.optimization.neighbors import find_points_in_spheres
 
 
-def coulomb_matrix_to_inverse_distance_proton(coulomb_mat: np.ndarray,
-                                              unit_conversion: float = 1.0, exponent: float = 2.4):
-    r"""Convert a Coulomb matrix back to inverse distancematrix plus atomic number.
-
-    Args:
-        coulomb_mat (np.ndarray): Coulomb matrix of shape (...,N,N)
-        unit_conversion (float) : Whether to scale units for distance. Default is 1.0.
-        exponent (float): Exponent for diagonal elements. Default is 2.4.
-
-    Returns:
-        tuple: [inv_dist, z]
-
-            - inv_dist (np.ndarray): Inverse distance Matrix of shape (...,N,N).
-            - z (np.ndarray): Atom Number corresponding diagonal as proton number (..., N).
-    """
-    indslie = np.arange(0, coulomb_mat.shape[-1])
-    z = coulomb_mat[..., indslie, indslie]
-    z = np.power(2 * z, 1 / exponent)
-    a = np.expand_dims(z, axis=len(z.shape) - 1)
-    b = np.expand_dims(z, axis=len(z.shape))
-    zz = a * b
-    c = coulomb_mat / zz
-    c[..., indslie, indslie] = 0
-    c /= unit_conversion
-    z = np.array(np.round(z), dtype=np.int)
-    return c, z
-
-
-def make_rotation_matrix(vector: np.ndarray, angle: float):
-    r"""Generate rotation matrix around a given vector with a certain angle.
-
-    Only defined for 3 dimensions explicitly here.
-
-    Args:
-        vector (np.ndarray, list): vector of rotation axis (3, ) with (x, y, z).
-        angle (value): angle in degrees ° to rotate around.
-
-    Returns:
-        np.ndarray: Rotation matrix :math:`R` of shape (3, 3) that performs the rotation for :math:`y = R x`.
-    """
-    angle = angle / 180.0 * np.pi
-    norm = (vector[0] ** 2.0 + vector[1] ** 2.0 + vector[2] ** 2.0) ** 0.5
-    direction = vector / norm
-    matrix = np.zeros((3, 3))
-    matrix[0][0] = direction[0] ** 2.0 * (1.0 - np.cos(angle)) + np.cos(angle)
-    matrix[1][1] = direction[1] ** 2.0 * (1.0 - np.cos(angle)) + np.cos(angle)
-    matrix[2][2] = direction[2] ** 2.0 * (1.0 - np.cos(angle)) + np.cos(angle)
-    matrix[0][1] = direction[0] * direction[1] * (1.0 - np.cos(angle)) - direction[2] * np.sin(angle)
-    matrix[1][0] = direction[0] * direction[1] * (1.0 - np.cos(angle)) + direction[2] * np.sin(angle)
-    matrix[0][2] = direction[0] * direction[2] * (1.0 - np.cos(angle)) + direction[1] * np.sin(angle)
-    matrix[2][0] = direction[0] * direction[2] * (1.0 - np.cos(angle)) - direction[1] * np.sin(angle)
-    matrix[1][2] = direction[1] * direction[2] * (1.0 - np.cos(angle)) - direction[0] * np.sin(angle)
-    matrix[2][1] = direction[1] * direction[2] * (1.0 - np.cos(angle)) + direction[0] * np.sin(angle)
-    return matrix
-
+def range_neighbour_lattice(coordinates: np.ndarray, lattice: np.ndarray,
+                            max_distance: Union[float, None] = 4.0,
+                            max_neighbours: Union[int, None] = None,
+                            self_loops: bool = False,
+                            exclusive: bool = True,
+                            limit_only_max_neighbours: bool = False,
+                            numerical_tol: float = 1e-8,
+                            manual_super_cell_radius: float = None,
+                            super_cell_tol_factor: float = 0.25,
+                            ) -> list:
+    r"""Generate range connections for a primitive unit cell in a periodic lattice (vectorized).
 
-def rotate_to_principle_axis(coord: np.ndarray):
-    r"""Rotate a point-cloud to its principle axis.
+    .. code-block:: python
 
-    This can be a molecule but also some general data.
-    It uses PCA via SVD from :obj:`numpy.linalg.svd`. PCA from scikit uses SVD too (:obj:`scipy.sparse.linalg`).
+        import numpy as np
+        from kgcnn.graph.methods import range_neighbour_lattice
 
-    .. note::
-        The data is centered before SVD but shifted back at the output.
+        artificial_lattice = np.array([[1.0, 0.0, 0.0], [1.0, 1.0, 0.0], [0.0, 0.0, 1.0]])
+        artificial_atoms = np.array([[0.1, 0.0, 0.0], [0.5, 0.5, 0.5]])
+        out = range_neighbour_lattice(artificial_atoms, artificial_lattice)
+
+        real_lattice = np.array([[-8.71172704, -0., -5.02971843],
+                                 [-10.97279872, -0.01635133, 8.94600922],
+                                 [-6.5538005, 12.48246168, 1.29207947]])
+        real_atoms = np.array([[-24.14652308, 12.46611035, 6.41607351],
+                               [-2.09180318, 0., -1.20770325],
+                               [0., 0., 0.],
+                               [-4.35586352, 0., -2.51485921]])
+        out_real = range_neighbour_lattice(real_atoms, real_lattice)
 
     Args:
-        coord (np.array): Array of points forming a pointcloud. Important: coord has shape (N,p)
-            where N is the number of samples and p is the feature/coordinate dimension e.g. 3 for x,y,z
+        coordinates (np.ndarray): Coordinate of nodes in the central primitive unit cell.
+        lattice (np.ndarray): Lattice matrix of real space lattice vectors of shape `(3, 3)`.
+            The lattice vectors must be given in rows of the matrix!
+        max_distance (float, optional): Maximum distance to allow connections, can also be None. Defaults to 4.0.
+        max_neighbours (int, optional): Maximum number of allowed neighbours for each central atom. Default is None.
+        self_loops (bool, optional): Allow self-loops between the same central node. Defaults to False.
+        exclusive (bool): Whether both distance and maximum neighbours must be fulfilled. Default is True.
+        limit_only_max_neighbours (bool): Not used.
+        numerical_tol  (float): Numerical tolerance for distance cut-off. Default is 1e-8.
+        manual_super_cell_radius (float): Not used.
+        super_cell_tol_factor (float): Tolerance to increase for search for neighbours. Default is 0.5.
 
     Returns:
-        tuple: [R, rotated]
-
-            - R (np.array): Rotation matrix of shape (p, p) if input has (N,p)
-            - rotated (np.array): Rotated point-could of coord that was the input.
+        list: [indices, images, dist]
     """
-    centroid_c = np.mean(coord, axis=0)
-    sm = coord - centroid_c
-    zzt = (np.dot(sm.T, sm))  # Calculate covariance matrix
-    u, s, vh = np.linalg.svd(zzt)
-    # Alternatively SVD of coord with onyly compute vh but not possible for numpy/scipy.
-    rotated = np.dot(sm, vh.T)
-    rot_shift = rotated + centroid_c
-    return vh, rot_shift
-
-
-def rigid_transform(a: np.ndarray, b: np.ndarray, correct_reflection: bool = False):
-    r"""Rotate and shift point-cloud A to point-cloud B. This should implement Kabsch algorithm.
-    May also work for input of shape `(...,N,3)` but is not tested.
-    Explanation of Kabsch Algorithm: https://en.wikipedia.org/wiki/Kabsch_algorithm
-    For further literature:
-    https://link.springer.com/article/10.1007/s10015-016-0265-x
-    https://link.springer.com/article/10.1007%2Fs001380050048
-
-
-    .. note::
-        The numbering of points of A and B must match; not for shuffled point-cloud.
-        This works for 3 dimensions only. Uses SVD.
-
-    Args:
-        a (np.ndarray): list of points (N,3) to rotate (and translate)
-        b (np.ndarray): list of points (N,3) to rotate towards: A to B, where the coordinates (3) are (x,y,z)
-        correct_reflection (bool): Whether to allow reflections or just rotations. Default is False.
-
-    Returns:
-        list: [A_rot, R, t]
+    # Require either max_distance or max_neighbours to be specified.
+    if max_distance is None and max_neighbours is None:
+        raise ValueError("Need to specify either `max_distance` or `max_neighbours` or both.")
 
-            - A_rot (np.ndarray): Rotated and shifted version of A to match B
-            - R (np.ndarray): Rotation matrix
-            - t (np.ndarray): translation from A to B
-    """
-    a = np.transpose(np.array(a))
-    b = np.transpose(np.array(b))
-    centroid_a = np.mean(a, axis=1)
-    centroid_b = np.mean(b, axis=1)
-    am = a - np.expand_dims(centroid_a, axis=1)
-    bm = b - np.expand_dims(centroid_b, axis=1)
-    h = np.dot(am, np.transpose(bm))
-    u, s, vt = np.linalg.svd(h)
-    r = np.dot(vt.T, u.T)
-    d = np.linalg.det(r)
-    if d < 0:
-        print("Warning: det(R)<0, det(R)=", d)
-        if correct_reflection:
-            print("Correcting R...")
-            vt[-1, :] *= -1
-            r = np.dot(vt.T, u.T)
-    bout = np.dot(r, am) + np.expand_dims(centroid_b, axis=1)
-    bout = np.transpose(bout)
-    t = np.expand_dims(centroid_b - np.dot(r, centroid_a), axis=0)
-    t = t.T
-    return bout, r, t
-
-
-def coordinates_from_distance_matrix(distance: np.ndarray, use_center: bool = None, dim: int = 3):
-    r"""Compute list of coordinates from a distance matrix of shape `(N, N)`.
-    May also work for input of shape `(..., N, N)` but is not tested.
-    Uses vectorized Alogrithm:
-    http://scripts.iucr.org/cgi-bin/paper?S0567739478000522
-    https://www.researchgate.net/publication/252396528_Stable_calculation_of_coordinates_from_distance_information
-    no check of positive semi-definite or possible k-dim >= 3 is done here
-    performs svd from numpy
+    # Volume and density of unit cell based on lattice matrix.
+    volume_unit_cell = np.sum(np.abs(np.cross(lattice[0], lattice[1]) * lattice[2]))
+    density_unit_cell = len(coordinates) / volume_unit_cell
 
-    Args:
-        distance (np.ndarray): distance matrix of shape (N,N) with Dij = abs(ri-rj)
-        use_center (int): which atom should be the center, dafault = None means center of mass
-        dim (int): the dimension of embedding, 3 is default
+    # Estimated real-space radius for max_neighbours based on density and volume of a single unit cell.
+    if max_neighbours is not None:
+        estimated_nn_volume = max_neighbours/density_unit_cell  # + len(coordinates)/ density_unit_cell
+        estimated_nn_radius = abs(float(np.cbrt(estimated_nn_volume / np.pi * 3 / 4)))
+        estimated_nn_radius = estimated_nn_radius
+    else:
+        estimated_nn_radius = None
 
-    Return:
-        np.ndarray: List of Atom coordinates [[x_1,x_2,x_3],[x_1,x_2,x_3],...]
-    """
-    distance = np.array(distance)
-    dim_in = distance.shape[-1]
-    if use_center is None:
-        # Take Center of mass (slightly changed for vectorization assuming d_ii = 0)
-        di2 = np.square(distance)
-        di02 = 1 / 2 / dim_in / dim_in * (2 * dim_in * np.sum(di2, axis=-1) - np.sum(np.sum(di2, axis=-1), axis=-1))
-        mat_m = (np.expand_dims(di02, axis=-2) + np.expand_dims(di02, axis=-1) - di2) / 2  # broadcasting
+    # Determine the required size of super-cell
+    if manual_super_cell_radius is not None:
+        if max_neighbours is None:
+            # Does not make sense to specify manual supercell in this case.
+            radius = max_distance
+        else:
+            radius = abs(manual_super_cell_radius)
+    elif max_distance is None:
+        radius = estimated_nn_radius
+    elif max_neighbours is None:
+        radius = max_distance
     else:
-        di2 = np.square(distance)
-        mat_m = (np.expand_dims(di2[..., use_center], axis=-2) + np.expand_dims(di2[..., use_center],
-                                                                                axis=-1) - di2) / 2
-    u, s, v = np.linalg.svd(mat_m)
-    vec = np.matmul(u, np.sqrt(np.diag(s)))  # EV are sorted by default
-    dist_out = vec[..., 0:dim]
-    return dist_out
+        if exclusive:
+            radius = min(max_distance, estimated_nn_radius)
+        else:
+            radius = max(max_distance, estimated_nn_radius)
 
+    _max_iter_nn_test = 100
+    _iter_required = 0
+    index1, index2, offset_vectors, distances = None, None, None, None
+    for i in range(0, _max_iter_nn_test):
+        _iter_required = i
+        index1, index2, offset_vectors, distances = find_points_in_spheres(
+            coordinates, coordinates,
+            r=radius, pbc=np.array([True] * 3, dtype=int), lattice=lattice, tol=numerical_tol)
+        offset_vectors = offset_vectors.astype('i2')
+
+        # Remove self_loops:
+        if not self_loops:
+            no_self_loops = np.argwhere(~np.isclose(distances, 0)).reshape(-1)
+            index1 = index1[no_self_loops]
+            index2 = index2[no_self_loops]
+            offset_vectors = offset_vectors[no_self_loops]
+            distances = distances[no_self_loops]
+
+        # We always sort here.
+        def reorder(order, *args):
+            return [x[order] for x in args]
+
+        def limit_to(c, k, r, id1, id2, ov, dd, logical_reduce=None):
+            splits = np.cumsum(c)[:-1]
+            id1_split = np.split(id1, splits)
+            id2_split = np.split(id2, splits)
+            ov_split = np.split(ov, splits)
+            dd_split = np.split(dd, splits)
+            mask_r, mask_k = None, None
+            if k is not None:
+                mask_k = []
+                for x in id1_split:
+                    mask_per_node = np.zeros((len(x)), dtype="bool")
+                    mask_per_node[:k] = True
+                    mask_k.append(mask_per_node)
+            if r is not None:
+                mask_r = []
+                for x in dd_split:
+                    mask_per_node = x <= r + + abs(numerical_tol)
+                    mask_r.append(mask_per_node)
+            if k is not None and r is not None:
+                mask = [logical_reduce(x1, x2) for x1, x2 in zip(mask_r, mask_k)]
+            elif k is None:
+                mask = mask_r
+            else:
+                mask = mask_k
+            out_split = []
+            for a in [id1_split, id2_split, ov_split, dd_split]:
+                out_split.append(np.concatenate([x[mask[i_node]] for i_node, x in enumerate(a)], axis=0))
+            return out_split
+
+        sort_index = np.argsort(distances, kind="stable")
+        index1, index2, offset_vectors, distances = reorder(sort_index, index1, index2, offset_vectors, distances)
+        sort_index = np.argsort(index1, kind="stable")
+        index1, index2, offset_vectors, distances = reorder(sort_index, index1, index2, offset_vectors, distances)
+
+        # Case: radius cutoff. Only consider radius here.
+        if max_neighbours is None:
+            break
+
+        unique_centers, counts = np.unique(index1, return_counts=True)
+        enough_nn = not (np.any(counts < max_neighbours) if len(counts) > 0 else 0 < max_neighbours)
+        # Case: knn.
+        if max_distance is None:
+            if not enough_nn:
+                radius = radius * (1.0 + super_cell_tol_factor)
+                continue
+            else:
+                index1, index2, offset_vectors, distances = limit_to(
+                    counts, max_neighbours, None, index1, index2, offset_vectors, distances)
+                break
 
-def range_neighbour_lattice(coordinates: np.ndarray, lattice: np.ndarray,
-                            max_distance: Union[float, None] = 4.0,
-                            max_neighbours: Union[int, None] = None,
-                            self_loops: bool = False,
-                            exclusive: bool = True,
-                            limit_only_max_neighbours: bool = False,
-                            numerical_tol: float = 1e-8,
-                            manual_super_cell_radius: float = None,
-                            super_cell_tol_factor: float = 0.25,
-                            ) -> list:
+        enough_distance = radius >= max_distance
+        # Case mixed both radius and knn.
+        if exclusive:
+            if enough_nn or enough_distance:
+                index1, index2, offset_vectors, distances = limit_to(
+                    counts, max_neighbours, max_distance, index1, index2, offset_vectors, distances,
+                    logical_reduce=np.logical_and)
+                break
+            else:
+                radius = radius * (1.0 + super_cell_tol_factor)
+                continue
+        else:
+            if not enough_nn or not enough_distance:
+                radius = radius * (1.0 + super_cell_tol_factor)
+                continue
+            else:
+                index1, index2, offset_vectors, distances = limit_to(
+                    counts, max_neighbours, max_distance, index1, index2, offset_vectors, distances,
+                    logical_reduce=np.logical_or)
+                break
+
+    if _iter_required + 1 >= _max_iter_nn_test:
+        raise ValueError("Exceeded maximum number of allowed range extensions for neighbour calculation.")
+
+    out_indices = np.concatenate([np.expand_dims(index1, axis=-1), np.expand_dims(index2, axis=-1)], axis=-1)
+    return [out_indices, offset_vectors, distances]
+
+
+# This is a python/numpy function to find neighbours in a periodic lattice.
+# The pymatgen version is preferred, since this version can get slow for very skew lattice matrices.
+def range_neighbour_lattice_python_vectorized(
+        coordinates: np.ndarray, lattice: np.ndarray,
+        max_distance: Union[float, None] = 4.0,
+        max_neighbours: Union[int, None] = None,
+        self_loops: bool = False,
+        exclusive: bool = True,
+        limit_only_max_neighbours: bool = False,
+        numerical_tol: float = 1e-8,
+        manual_super_cell_radius: float = None,
+        super_cell_tol_factor: float = 0.25,
+        ) -> list:
     r"""Generate range connections for a primitive unit cell in a periodic lattice (vectorized).
 
     The function generates a supercell of required radius and computes connections of neighbouring nodes
     from the primitive centered unit cell. For :obj:`max_neighbours` the supercell radius is estimated based on
     the unit cell density. Always the smallest necessary supercell is generated based on :obj:`max_distance` and
     :obj:`max_neighbours`. If a supercell for radius :obj:`max_distance` should always be generated but limited by
     :obj:`max_neighbours`, you can set :obj:`limit_only_max_neighbours` to `True`.
@@ -194,14 +210,32 @@
     .. note::
 
         For periodic structure, setting :obj:`max_distance` and :obj:`max_neighbours` to `inf` would also lead
         to an infinite number of neighbours and connections. If :obj:`exclusive` is set to `False`, having either
         :obj:`max_distance` or :obj:`max_neighbours` set to `inf`, will result in an infinite number of neighbours.
         If set to `None`, :obj:`max_distance` or :obj:`max_neighbours` can selectively be ignored.
 
+    .. code-block:: python
+
+        import numpy as np
+        from kgcnn.graph.methods._periodic import range_neighbour_lattice_python_vectorized
+
+        artificial_lattice = np.array([[1.0, 0.0, 0.0], [1.0, 1.0, 0.0], [0.0, 0.0, 1.0]])
+        artificial_atoms = np.array([[0.1, 0.0, 0.0], [0.5, 0.5, 0.5]])
+        out = range_neighbour_lattice_python_vectorized(artificial_atoms, artificial_lattice)
+
+        real_lattice = np.array([[-8.71172704, -0., -5.02971843],
+                                 [-10.97279872, -0.01635133, 8.94600922],
+                                 [-6.5538005, 12.48246168, 1.29207947]])
+        real_atoms = np.array([[-24.14652308, 12.46611035, 6.41607351],
+                               [-2.09180318, 0., -1.20770325],
+                               [0., 0., 0.],
+                               [-4.35586352, 0., -2.51485921]])
+        out_real = range_neighbour_lattice_python_vectorized(real_atoms, real_lattice)
+
     Args:
         coordinates (np.ndarray): Coordinate of nodes in the central primitive unit cell.
         lattice (np.ndarray): Lattice matrix of real space lattice vectors of shape `(3, 3)`.
             The lattice vectors must be given in rows of the matrix!
         max_distance (float, optional): Maximum distance to allow connections, can also be None. Defaults to 4.0.
         max_neighbours (int, optional): Maximum number of allowed neighbours for each central atom. Default is None.
         self_loops (bool, optional): Allow self-loops between the same central node. Defaults to False.
@@ -341,137 +375,30 @@
     dist_indices_sort = np.take_along_axis(
         dist_indices, np.repeat(np.expand_dims(arg_sort, axis=2), dist_indices.shape[2], axis=2), axis=1)
     dist_images_sort = np.take_along_axis(
         dist_images, np.repeat(np.expand_dims(arg_sort, axis=2), dist_images.shape[2], axis=2), axis=1)
 
     # Select range connections based on distance cutoff and nearest neighbour limit. Uses masking.
     # Based on 'max_distance'.
-    if max_distance is None:
-        mask_distance = np.ones_like(dist_sort, dtype="bool")
-    else:
+    mask_distance, mask_neighbours = None, None
+    if max_distance is not None:
         mask_distance = dist_sort <= max_distance + abs(numerical_tol)
     # Based on 'max_neighbours'.
-    mask_neighbours = np.zeros_like(dist_sort, dtype="bool")
-    if max_neighbours is None:
-        max_neighbours = dist_sort.shape[-1]
-    mask_neighbours[:, :max_neighbours] = True
+    if max_neighbours is not None:
+        mask_neighbours = np.zeros_like(dist_sort, dtype="bool")
+        mask_neighbours[:, :max_neighbours] = True
 
-    if exclusive:
-        mask = np.logical_and(mask_neighbours, mask_distance)
+    if max_neighbours is None:
+        mask = mask_distance
+    elif max_distance is None:
+        mask = mask_neighbours
     else:
-        mask = np.logical_or(mask_neighbours, mask_distance)
-
+        if exclusive:
+            mask = np.logical_and(mask_neighbours, mask_distance)
+        else:
+            mask = np.logical_or(mask_neighbours, mask_distance)
     # Select nodes.
     out_dist = dist_sort[mask]
     out_images = dist_images_sort[mask]
     out_indices = dist_indices_sort[mask]
 
     return [out_indices, out_images, out_dist]
-
-
-def get_principal_moments_of_inertia(masses: np.ndarray, coordinates: np.ndarray, shift_center_of_mass: bool = True):
-    """Compute principle moments of inertia for a point-cloud with given mass.
-
-    Args:
-        masses (np.ndarray): Array of mass values.
-        coordinates (np.ndarray): Coordinates of point-cloud.
-        shift_center_of_mass (bool): Whether to shift to center of mass for inertia matrix.
-
-    Returns:
-        np.ndarray: Eigenvalues of inertia matrix. Shape is (3, ).
-    """
-
-    def translate_to_center_of_mass(m, xyz):
-        if len(m.shape) <= 1:
-            m = np.expand_dims(m, axis=-1)
-        com = (np.sum(m * xyz, axis=0, keepdims=True) / np.sum(m))
-        return xyz - com
-
-    def get_inertia_matrix(m, xyz):
-        x, y, z = xyz.T
-        Ixx = np.sum(m * (y ** 2 + z ** 2))
-        Iyy = np.sum(m * (x ** 2 + z ** 2))
-        Izz = np.sum(m * (x ** 2 + y ** 2))
-        Ixy = -np.sum(m * x * y)
-        Iyz = -np.sum(m * y * z)
-        Ixz = -np.sum(m * x * z)
-        return np.array([[Ixx, Ixy, Ixz], [Ixy, Iyy, Iyz], [Ixz, Iyz, Izz]])
-
-    coordinates = translate_to_center_of_mass(masses, coordinates) if shift_center_of_mass else coordinates
-    inertia_matrix = get_inertia_matrix(masses, coordinates)
-    pc = np.linalg.eigvals(inertia_matrix)
-    pc = np.sort(pc)
-
-    return pc
-
-
-def shift_coordinates_to_unit_cell(coordinates: np.ndarray, lattice: np.ndarray):
-    """Shift a set of coordinates into the unit cell of a periodic system.
-
-    Args:
-        coordinates (np.ndarray): Coordinate of nodes in the central primitive unit cell.
-        lattice (np.ndarray): Lattice matrix of real space lattice vectors of shape `(3, 3)` .
-            The lattice vectors must be given in rows of the matrix!
-
-    Returns:
-        np.ndarray: Coordinates shifted into unit cell defined by lattice.
-    """
-    lattice_inv = np.linalg.inv(lattice)
-    frac_coordinates = np.dot(coordinates, lattice_inv)
-    shifted_frac_coordinates = frac_coordinates % 1.0
-    shifted_coordinates = np.dot(shifted_frac_coordinates, lattice)
-    return shifted_coordinates
-
-
-def distance_for_range_indices(coordinates: np.ndarray, indices: np.ndarray,
-                               require_distance_dimension: bool = True):
-    """Simple helper function to compute distances for indices.
-
-    Args:
-        coordinates (np.ndarray): Positions of shape `(N, 3)` .
-        indices (np.ndarray): Pair-wise indices of shape `(M, 2)` .
-        require_distance_dimension (bool): Whether to return distances of shape `(M, 1)` .
-
-    Returns:
-        np.ndarray: Distances of shape `(M, )` or `(M, 1)` if `require_distance_dimension` .
-    """
-    pos12 = coordinates[indices]
-    dist = np.sqrt(np.sum(np.square(pos12[:, 0] - pos12[:, 1]), axis=-1))
-    if require_distance_dimension:
-        if len(dist.shape) <= 1:
-            dist = np.expand_dims(dist, axis=-1)
-    return dist
-
-
-def distance_for_range_indices_periodic(coordinates: np.ndarray,
-                                        indices: np.ndarray,
-                                        images: np.ndarray,
-                                        lattice: np.ndarray,
-                                        require_distance_dimension: bool = True):
-    """Simple helper function to compute distances for indices for a periodic system.
-
-    Args:
-        coordinates (np.ndarray): Positions of shape `(N, 3)` within the unit-cell.
-        indices (np.ndarray): Pair-wise indices of shape `(M, 2)` .
-        images (np.ndarray): Image translation of the second index of shape `(M, 3)` .
-        lattice (np.ndarray): Lattice matrix of real space lattice vectors of shape `(3, 3)` .
-            The lattice vectors must be given in rows of the matrix!
-        require_distance_dimension (bool): Whether to return distances of shape `(M, 1)` .
-
-    Returns:
-        np.ndarray: Distances of shape `(M, )` or `(M, 1)` if `require_distance_dimension` .
-    """
-    pos12 = coordinates[indices]
-    pos1, pos2 = pos12[:, 0], pos12[:, 1]
-    if len(images.shape) > 2:
-        # If image information are for both indices of shape (M, 2, 3)
-        pos1 = pos1 + np.dot(images[:, 0], lattice)
-        pos2 = pos2 + np.dot(images[:, 1], lattice)
-    else:
-        # Default is only for second index. Usually sending node.
-        pos2 = pos2 + np.dot(images, lattice)
-    dist = np.sqrt(np.sum(np.square(pos1 - pos2), axis=-1))
-    if require_distance_dimension:
-        if len(dist.shape) <= 1:
-            dist = np.expand_dims(dist, axis=-1)
-    return dist
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kgcnn-3.0.1/kgcnn/graph/postprocessor.py` & `kgcnn-3.0.2/kgcnn/graph/postprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/graph/preprocessor.py` & `kgcnn-3.0.2/kgcnn/graph/preprocessor.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/graph/serial.py` & `kgcnn-3.0.2/kgcnn/graph/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/io/file.py` & `kgcnn-3.0.2/kgcnn/io/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,19 @@
         return tuple([])
     # If all same inner shape.
     if all(x[1:] == shapes[0][1:] for x in shapes):
         return shapes[0][1:]
 
 
 class RaggedTensorNumpyFile:
-    """Class representing a NumPy '.npz' file to store a ragged tensor on disk."""
+    """Class representing a NumPy '.npz' file to store a ragged tensor on disk.
+
+    For the moment only ragged tensors of ragged rank of one are supported. However, arbitrary ragged tensors can be
+    supported in principle.
+    """
 
     _device = '/cpu:0'
 
     def __init__(self, file_path: str, compressed: bool = False):
         """Make class for a NPZ file.
 
         Args:
@@ -57,20 +61,23 @@
 
         Args:
             ragged_array (list, tf.RaggedTensor): List or list of numpy arrays.
 
         Returns:
             None.
         """
+        # We use tensorflow functions to ensure an eager ragged tensor.
         if not isinstance(ragged_array, tf.RaggedTensor):
             with tf.device(self._device):
                 ragged_array = tf.ragged.constant(ragged_array, inner_shape=_check_for_inner_shape(ragged_array))
         assert ragged_array.ragged_rank == 1, "Only support for ragged_rank=1 at the moment."
         values = np.array(ragged_array.values)
         row_splits = np.array(ragged_array.row_splits)
+        # Since the shape array can not have nones, we convert nones to 0.
+        # Not ideal, but could make an extra shape array to indicate ragged dimensions.
         shape = np.array([x if x is not None else 0 for x in ragged_array.shape], dtype="uint64")
         ragged_rank = np.array(ragged_array.ragged_rank)
         rank = np.array(len(shape))
         out = {"values": values,
                "row_splits": row_splits,
                "shape": shape,
                "ragged_rank": ragged_rank,
@@ -85,32 +92,56 @@
 
         Args:
             return_as_tensor: Whether to return tf.RaggedTensor.
 
         Returns:
             tf.RaggedTensor: Ragged tensor form file.
         """
+        # Here only ragged rank one loading is supported.
         data = np.load(self.file_path)
         values = data.get("values")
         row_splits = data.get("row_splits")
         if return_as_tensor:
             with tf.device(self._device):
                 out = tf.RaggedTensor.from_row_splits(values, row_splits)
             return out
         return np.split(values, row_splits[1:-1])
 
     def __getitem__(self, item):
-        raise NotImplementedError("Not implemented for file reference item load.")
+        """Get single item from the ragged tensor on file.
+
+        Args:
+            item (int): Index of the item to get.
+        """
+        assert isinstance(item, int), "Only single index is supported, no slicing."
+        # NOTE: At the moment mmap is not supported for NPZ files.
+        with np.load(self.file_path, mmap_mode="r") as data:
+            row_splits = np.array(data.get("row_splits"))
+            out_data = np.array(data["values"][row_splits[item]:row_splits[item + 1]])
+        return out_data
 
     def exists(self):
+        """Check if file for path information of this class exists."""
         return os.path.exists(self.file_path)
 
+    def __len__(self):
+        """Length of the tensor on file."""
+        data = np.load(self.file_path)
+        row_splits = data.get("row_splits")
+        num_row_splits = int(row_splits.shape[0])
+        # length is num_row_splits - 1
+        return num_row_splits-1
+
 
 class RaggedTensorHDFile:
-    """Class representing a HDF '.hdf5' file to store a ragged tensor on disk."""
+    """Class representing an HDF '.hdf5' file to store a ragged tensor on disk.
+
+    For the moment only ragged tensors of ragged rank of one are supported. However, arbitrary ragged tensors can be
+    supported in principle.
+    """
 
     _device = '/cpu:0'
 
     def __init__(self, file_path: str, compressed: bool = None):
         """Make class for a HDF5 file.
 
         Args:
@@ -134,20 +165,23 @@
 
         Args:
             ragged_array (list, tf.RaggedTensor): List or list of numpy arrays.
 
         Returns:
             None.
         """
+        # We use tensorflow functions to ensure an eager ragged tensor.
         if not isinstance(ragged_array, tf.RaggedTensor):
             with tf.device(self._device):
                 ragged_array = tf.ragged.constant(ragged_array, inner_shape=_check_for_inner_shape(ragged_array))
         assert ragged_array.ragged_rank == 1, "Only support for ragged_rank=1 at the moment."
         values = np.array(ragged_array.values)
         row_splits = np.array(ragged_array.row_splits)
+        # Since the shape array can not have nones, we convert nones to 0.
+        # Not ideal, but could make an extra shape array to indicate ragged dimensions.
         shape = np.array([x if x is not None else 0 for x in ragged_array.shape], dtype="uint64")
         ragged_rank = np.array(ragged_array.ragged_rank)
         rank = np.array(len(shape))
         with h5py.File(self.file_path, "w") as file:
             file.create_dataset("values", data=values,
                                 maxshape=[x if i > 0 else None for i, x in enumerate(values.shape)])
             file.create_dataset("row_splits", data=row_splits, maxshape=(None, ))
@@ -171,33 +205,55 @@
                 with tf.device(self._device):
                     out = tf.RaggedTensor.from_row_splits(np.array(values), np.array(row_splits))
             else:
                 out = np.split(values, row_splits[1:-1])
         return out
 
     def __getitem__(self, item: int):
+        """Get single item from the ragged tensor on file.
+
+        Args:
+            item (int): Index of the item to get.
+        """
+        assert isinstance(item, int), "Only single index is supported, no slicing."
         with h5py.File(self.file_path, "r") as file:
             row_splits = file["row_splits"]
             out_data = np.array(file["values"][row_splits[item]:row_splits[item+1]])
         return out_data
 
     def append(self, item):
+        """Append single item to ragged tensor.
+
+        Args:
+            item (np.ndarray, tf.Tensor): Item to append.
+
+        Returns:
+            None.
+        """
         with h5py.File(self.file_path, "r+") as file:
             file["values"].resize(
                 file["values"].shape[0] + len(item), axis=0
             )
             split_last = file["row_splits"][-1]
             file["row_splits"].resize(
                 file["row_splits"].shape[0] + 1, axis=0
             )
             len_last = len(item)
             file["row_splits"][-1] = split_last + len_last
             file["values"][split_last:split_last+len_last] = item
 
     def append_multiple(self, items: list):
+        """Append multiple items to ragged tensor.
+
+        Args:
+            items (list): List of items to append. Must match in shape.
+
+        Returns:
+            None.
+        """
         new_values = np.concatenate(items, axis=0)
         new_len = len(items)
         new_splits = np.cumsum([len(x) for x in items])
         with h5py.File(self.file_path, "r+") as file:
             file["values"].resize(
                 file["values"].shape[0] + new_values.shape[0], axis=0
             )
@@ -205,14 +261,16 @@
             file["row_splits"].resize(
                 file["row_splits"].shape[0] + new_len, axis=0
             )
             file["row_splits"][-new_len:] = split_last + new_splits
             file["values"][split_last:+split_last+new_splits[-1]] = new_values
 
     def __len__(self):
+        """Length of the tensor on file."""
         with h5py.File(self.file_path, "r") as file:
             num_row_splits = int(file["row_splits"].shape[0])
         # length is num_row_splits - 1
         return num_row_splits-1
 
     def exists(self):
+        """Check if file for path information of this class exists."""
         return os.path.exists(self.file_path)
```

### Comparing `kgcnn-3.0.1/kgcnn/io/loader.py` & `kgcnn-3.0.2/kgcnn/io/loader.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/README.md` & `kgcnn-3.0.2/kgcnn/layers/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Implementation details
 
 The most general layers for `kgcnn` should accept (ragged) tensor input and are sorted as following: 
 
 * The most general layers that kept maintained beyond different models with proper documentation are located in `kgcnn.layers`. These are:
+    * `kgcnn.layers.activ` Layers for activation functions with learnable parameters.
     * `kgcnn.layers.attention` Layers for graph attention.
     * `kgcnn.layers.casting` Layers for casting tensor formats.
     * `kgcnn.layers.conv` Basic convolution layers.
     * `kgcnn.layers.gather` Layers around tf.gather.
     * `kgcnn.layers.geom` Geometry operations.
     * `kgcnn.layers.message` Message passing base layer.
     * `kgcnn.layers.mlp` Multi-layer perceptron for graphs.
```

### Comparing `kgcnn-3.0.1/kgcnn/layers/attention.py` & `kgcnn-3.0.2/kgcnn/layers/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     An edge is defined by index tuple :math:`(i, j)` with the direction of the connection from :math:`j` to :math:`i`.
 
     Args:
         units (int): Units for the linear trafo of node features before attention.
         use_edge_features (bool): Append edge features to attention computation. Default is False.
         use_final_activation (bool): Whether to apply the final activation for the output.
         has_self_loops (bool): If the graph has self-loops. Not used here. Default is True.
-        activation (str): Activation. Default is {"class_name": "kgcnn>leaky_relu", "config": {"alpha": 0.2}},
+        activation (str): Activation. Default is "kgcnn>leaky_relu",
         use_bias (bool): Use bias. Default is True.
         kernel_regularizer: Kernel regularization. Default is None.
         bias_regularizer: Bias regularization. Default is None.
         activity_regularizer: Activity regularization. Default is None.
         kernel_constraint: Kernel constrains. Default is None.
         bias_constraint: Bias constrains. Default is None.
         kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
@@ -36,15 +36,15 @@
     """
 
     def __init__(self,
                  units,
                  use_edge_features=False,
                  use_final_activation=True,
                  has_self_loops=True,
-                 activation='kgcnn>leaky_relu',
+                 activation="kgcnn>leaky_relu",
                  use_bias=True,
                  kernel_regularizer=None,
                  bias_regularizer=None,
                  activity_regularizer=None,
                  kernel_constraint=None,
                  bias_constraint=None,
                  kernel_initializer='glorot_uniform',
@@ -131,15 +131,15 @@
     An edge is defined by index tuple :math:`(i, j)` with the direction of the connection from :math:`j` to :math:`i`.
 
     Args:
         units (int): Units for the linear trafo of node features before attention.
         use_edge_features (bool): Append edge features to attention computation. Default is False.
         use_final_activation (bool): Whether to apply the final activation for the output.
         has_self_loops (bool): If the graph has self-loops. Not used here. Default is True.
-        activation (str): Activation. Default is {"class_name": "kgcnn>leaky_relu", "config": {"alpha": 0.2}},
+        activation (str): Activation. Default is "kgcnn>leaky_relu",
         use_bias (bool): Use bias. Default is True.
         kernel_regularizer: Kernel regularization. Default is None.
         bias_regularizer: Bias regularization. Default is None.
         activity_regularizer: Activity regularization. Default is None.
         kernel_constraint: Kernel constrains. Default is None.
         bias_constraint: Bias constrains. Default is None.
         kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
@@ -147,15 +147,15 @@
     """
 
     def __init__(self,
                  units,
                  use_edge_features=False,
                  use_final_activation=True,
                  has_self_loops=True,
-                 activation='kgcnn>leaky_relu',
+                 activation="kgcnn>leaky_relu",
                  use_bias=True,
                  kernel_regularizer=None,
                  bias_regularizer=None,
                  activity_regularizer=None,
                  kernel_constraint=None,
                  bias_constraint=None,
                  kernel_initializer='glorot_uniform',
@@ -318,9 +318,8 @@
     def get_config(self):
         """Update layer config."""
         config = super(MultiHeadGATV2Layer, self).get_config()
         config.update({
             'num_heads': self.num_heads,
             'concat_heads': self.concat_heads
         })
-
-        return config
+        return config
```

### Comparing `kgcnn-3.0.1/kgcnn/layers/base.py` & `kgcnn-3.0.2/kgcnn/layers/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/casting.py` & `kgcnn-3.0.2/kgcnn/layers/casting.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/conv.py` & `kgcnn-3.0.2/kgcnn/layers/conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     Ideally they are weights of shape `(..., 1)` for broadcasting, e.g. entries of :math:`A_s` .
 
     Args:
         units (int): Output dimension/ units of dense layer.
         pooling_method (str): Pooling method for summing edges. Default is 'segment_sum'.
         normalize_by_weights (bool): Normalize the pooled output by the sum of weights. Default is False.
             In this case the edge features are considered weights of dimension (...,1) and are summed for each node.
-        activation (str): Activation. Default is {"class_name": "kgcnn>leaky_relu", "config": {"alpha": 0.2}}.
+        activation (str): Activation. Default is 'kgcnn>leaky_relu'.
         use_bias (bool): Use bias. Default is True.
         kernel_regularizer: Kernel regularization. Default is None.
         bias_regularizer: Bias regularization. Default is None.
         activity_regularizer: Activity regularization. Default is None.
         kernel_constraint: Kernel constrains. Default is None.
         bias_constraint: Bias constrains. Default is None.
         kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
```

### Comparing `kgcnn-3.0.1/kgcnn/layers/gather.py` & `kgcnn-3.0.2/kgcnn/layers/gather.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,121 +35,116 @@
         edge_idx = tf.ragged.constant([[[0,1],[1,0]],[[0,2],[1,2]]], ragged_rank=1)
         print(GatherEmbedding()([nodes, edge_idx]))
 
     """
 
     def __init__(self,
                  axis: int = 1,
-                 concat_axis: Union[int, None] = 2,
-                 split_axis: Union[int, None] = None,
+                 split_axis: Union[int, None] = 2,
                  split_indices: list = None,
-                 concat_indices: list = None,
+                 concat_axis: Union[int, None] = 2,
+                 allow_disjoint_implementation: bool = True,
                  **kwargs):
         r"""Initialize layer.
 
         Args:
             axis (int): The axis to gather embeddings from. Default is 1.
-            concat_axis (int): The axis which concatenates embeddings. Default is 2.
-            split_axis (int): The axis to split the gathered embeddings. Default is None.
+            split_axis (int): The axis to split indices to gather embeddings. Default is None.
             split_indices (list): List of indices to split from gathered tensor. Default is None.
-            concat_indices (list): List of indices to concatenate from gathered tensor. Default is None.
+            concat_axis (int): The axis which concatenates embeddings. Default is 2.
+            allow_disjoint_implementation (bool): Whether to allow (preferred) disjoint implementation.
         """
         super(GatherEmbedding, self).__init__(**kwargs)
         self.concat_axis = concat_axis
         self.axis = axis
         self.split_axis = split_axis
         self.split_indices = split_indices
-        self.concat_indices = concat_indices
         self.node_indexing = "sample"
+        self.allow_disjoint_implementation = allow_disjoint_implementation
 
-        if split_axis is not None and concat_axis is not None:
-            raise ValueError("Can not both split and concatenate new index axis. At least one must be `None`.")
+        if self.concat_axis is not None and self.split_axis is None:
+            raise ValueError("Can only concat `list` of gathered tensors. Require `split_axis` not None.")
 
     def build(self, input_shape):
         super(GatherEmbedding, self).build(input_shape)
 
         if len(input_shape) != 2:
             print("Number of inputs for layer '%s' must be 2: `[nodes, indices]` ." % self.name)
 
-    def _disjoint_implementation(self, inputs, **kwargs):
+    def _is_disjoint_possible(self, inputs, **kwargs):
         # The primary case for aggregation of nodes from node feature list. Case from doc-string.
         # Possibly faster implementation via values and indices shifted by row-partition.
         # Equal to disjoint implementation. Only works for ragged_rank=1 and specific axis.
         if all([isinstance(x, tf.RaggedTensor) for x in inputs]):
             is_rank_one = all([x.ragged_rank == 1 for x in inputs])
             if is_rank_one and self.axis == 1 and self.concat_axis in [None, 2] and self.split_axis in [None, 2]:
-                node, node_part = inputs[0].values, inputs[0].row_splits
-                edge_index, edge_part = inputs[1].values, inputs[1].row_lengths()
-                disjoint_list = partition_row_indexing(edge_index, node_part, edge_part,
-                                                       partition_type_target="row_splits",
-                                                       partition_type_index="row_length",
-                                                       to_indexing='batch',
-                                                       from_indexing=self.node_indexing)
-                out = tf.gather(node, disjoint_list, axis=0)
-                # Option: Concat features.
-                if self.concat_axis == 2:
-                    if self.concat_indices is None and edge_index.shape[1] is None:
-                        raise ValueError("Cannot infer concat indices, please specify statically in `concat_indices` .")
-                    concat_indices = self.concat_indices if self.concat_indices else range(edge_index.shape[1])
-                    out = tf.concat([out[:, i] for i in concat_indices], axis=1)
-                    return tf.RaggedTensor.from_row_lengths(out, edge_part, validate=self.ragged_validate)
-                # Option: Split features.
-                if self.split_axis == 2:
-                    if self.split_indices is None and edge_index.shape[1] is None:
-                        raise ValueError("Cannot infer split indices, please specify statically in `split_indices` .")
-                    split_indices = self.split_indices if self.split_indices else range(edge_index.shape[1])
-                    return [tf.RaggedTensor.from_row_lengths(
-                        out[:, i], edge_part, validate=self.ragged_validate) for i in split_indices]
+                return True
+        return False
 
+    def _disjoint_implementation(self, inputs, **kwargs):
+        node, node_part = inputs[0].values, inputs[0].row_splits
+        edge_index, edge_part = inputs[1].values, inputs[1].row_lengths()
+        disjoint_list = partition_row_indexing(
+            edge_index, node_part, edge_part, partition_type_target="row_splits", partition_type_index="row_length",
+            to_indexing='batch', from_indexing=self.node_indexing
+        )
+        if self.split_axis == 2:
+            if self.split_indices is None and edge_index.shape[1] is None:
+                raise ValueError("Cannot infer split indices, please specify statically in `split_indices` .")
+            split_indices = self.split_indices if self.split_indices else range(edge_index.shape[1])
+            indices_list = [tf.gather(disjoint_list, i, axis=1) for i in split_indices]
+            out = [tf.gather(node, ix, axis=0) for ix in indices_list]
+            if self.concat_axis == 2:
+                out = tf.concat(out, axis=1)
                 return tf.RaggedTensor.from_row_lengths(out, edge_part, validate=self.ragged_validate)
-        return None
+            return [tf.RaggedTensor.from_row_lengths(x, edge_part, validate=self.ragged_validate) for x in out]
+        else:
+            out = tf.gather(node, disjoint_list, axis=0)
+            return tf.RaggedTensor.from_row_lengths(out, edge_part, validate=self.ragged_validate)
 
     def call(self, inputs, **kwargs):
         r"""Forward pass.
 
         Args:
             inputs (list): [embeddings, tensor_index]
 
                 - embeddings (tf.RaggedTensor): Node embeddings of shape `(batch, [N], F)`
                 - tensor_index (tf.RaggedTensor): Edge indices referring to nodes of shape `(batch, [M], 2)`
 
         Returns:
             tf.RaggedTensor: Gathered node embeddings that match the number of edges of shape `(batch, [M], 2*F)`
         """
         # Old disjoint implementation that could be faster.
-        out = self._disjoint_implementation(inputs, **kwargs)
-        if out is not None:
-            return out
+        if self._is_disjoint_possible(inputs, **kwargs) and self.allow_disjoint_implementation:
+            return self._disjoint_implementation(inputs, **kwargs)
 
         # For arbitrary gather from ragged tensor use tf.gather with batch_dims=1.
         # Works in tf.__version__ >= 2.4 !
-        out = tf.gather(inputs[0], inputs[1], batch_dims=1, axis=self.axis)
-
-        # Option: Concat features.
-        if self.concat_axis is not None:
-            if self.concat_indices is None and out.shape[self.concat_axis] is None:
-                raise ValueError("Cannot infer concat indices, please specify statically in `concat_indices` .")
-            concat_indices = self.concat_indices if self.concat_indices else range(out.shape[self.concat_axis])
-            out = tf.concat(
-                [tf.gather(out, i, axis=self.concat_axis) for i in concat_indices],
-                axis=self.concat_axis
-            )
         # Option: Split features.
+        nodes, indices = inputs
         if self.split_axis is not None:
-            if self.split_indices is None and out.shape[self.split_axis] is None:
+            if self.split_indices is None and indices.shape[self.split_axis] is None:
                 raise ValueError("Cannot infer split indices, please specify statically in `split_indices` .")
-            split_indices = self.split_indices if self.split_indices else range(out.shape[self.split_axis])
-            out = [tf.gather(out, i, axis=self.split_axis) for i in split_indices]
+            split_indices = self.split_indices if self.split_indices else range(indices.shape[self.split_axis])
+            indices_list = [tf.gather(nodes, i, axis=self.split_axis) for i in split_indices]
+            out = [tf.gather(nodes, ix, batch_dims=1, axis=self.axis) for ix in indices_list]
+            # Option: Concat features.
+            if self.concat_axis is not None:
+                out = tf.concat(out, axis=self.concat_axis)
+        else:
+            out = tf.gather(nodes, indices, batch_dims=1, axis=self.axis)
         return out
 
     def get_config(self):
         """Update layer config."""
         config = super(GatherEmbedding, self).get_config()
-        config.update({"concat_axis": self.concat_axis, "axis": self.axis, "split_axis": self.split_axis,
-                       "concat_indices": self.concat_indices, "split_indices": self.split_indices})
+        config.update({
+            "concat_axis": self.concat_axis, "axis": self.axis, "split_axis": self.split_axis,
+            "split_indices": self.split_indices, "allow_disjoint_implementation": self.allow_disjoint_implementation
+        })
         return config
 
 
 GatherNodes = GatherEmbedding
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='GatherEmbeddingSelection')
```

### Comparing `kgcnn-3.0.1/kgcnn/layers/geom.py` & `kgcnn-3.0.2/kgcnn/layers/geom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1017,15 +1017,52 @@
     :math:`\vec{f} = (f_1, f_2, f_3)` the layer performs for each node and with a lattice matrix per sample:
 
     .. math::
 
         \vec{r} = \vec{f} \; \mathbf{A}
 
     Note that the definition of the lattice matrix has lattice vectors in rows, which is the default definition from
-    :obj:`pymatgen`.
+    :obj:`pymatgen` .
+
+    .. code-block:: python
+
+        import tensorflow as tf
+        from kgcnn.layers.geom import FracToRealCoordinates
+        lattices = tf.constant([
+            [[ 4.10744499,  0.        , -1.51280847],
+            [-0.5571808 ,  4.06947833, -1.51280847],
+            [-0.00707463, -0.00810927,  6.31328315]],
+            [[ 4.2119145 ,  0.        ,  0.        ],
+            [-2.10595725,  3.64762496,  0.        ],
+            [ 0.        ,  0.        ,  5.75016544]]
+        ])
+        frac = tf.ragged.constant([
+            [[0.        , 0.        , 0.        ],
+            [0.38949211, 0.38949211, 0.77898422],
+            [0.61050789, 0.61050789, 0.22101578],
+            [0.75      , 0.25      , 0.5       ],
+            [0.25      , 0.75      , 0.5       ]],
+            [[0.        , 0.        , 0.        ],
+            [0.        , 0.        , 0.5       ],
+            [0.33333333, 0.66666667, 0.25      ],
+            [0.66666667, 0.33333333, 0.75      ]]
+        ], ragged_rank=1)
+        real = tf.ragged.constant([
+            [[ 0.        ,  0.        ,  0.        ],
+            [ 1.37728887,  1.57871271,  3.73949402],
+            [ 2.16590069,  2.48265635, -0.45182781],
+            [ 2.93775123,  1.01331495,  1.64383311],
+            [ 0.60543833,  3.04805411,  1.64383311]],
+            [[ 0.00000000,  0.00000000,  0.00000000],
+            [ 0.00000000,  0.00000000,  2.87508272],
+            [-2.10595727e-08,  2.43174999,  1.43754136],
+            [ 2.10595727,  1.21587497,  4.31262408]]
+            ], ragged_rank=1)
+        print(FracToRealCoordinates()([frac, lattices])-real)
+
     """
 
     def __init__(self, **kwargs):
         """Initialize layer."""
         self.gather_state = GatherState()
         super(FracToRealCoordinates, self).__init__(**kwargs)
 
@@ -1044,9 +1081,12 @@
 
         Returns:
             tf.RaggedTensor: Real-space node coordinates of shape `(batch, [N], 3)`.
         """
         frac_coords = self.assert_ragged_input_rank(inputs[0], ragged_rank=1)
         lattice_matrices = inputs[1]
         lattice_matrices_ = tf.repeat(lattice_matrices, frac_coords.row_lengths(), axis=0)
-        real_coords = tf.einsum('ij,ikj->ik', frac_coords.values, lattice_matrices_)
-        return tf.RaggedTensor.from_row_splits(real_coords, frac_coords.row_splits, validate=self.ragged_validate)
+        # frac_to_real = tf.einsum('ij,ijk->ik', frac_coords.values, lattice_matrices_)
+        frac_to_real_coords = ks.backend.batch_dot(frac_coords.values, lattice_matrices_)
+        # print(frac_to_real_coords-frac_to_real)
+        return tf.RaggedTensor.from_row_splits(
+            frac_to_real_coords, frac_coords.row_splits, validate=self.ragged_validate)
```

### Comparing `kgcnn-3.0.1/kgcnn/layers/message.py` & `kgcnn-3.0.2/kgcnn/layers/message.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/mlp.py` & `kgcnn-3.0.2/kgcnn/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/modules.py` & `kgcnn-3.0.2/kgcnn/layers/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tensorflow as tf
 from kgcnn.layers.base import GraphBaseLayer
 from kgcnn.ops.axis import get_positive_axis
+import kgcnn.layers.activ
 ks = tf.keras  # import tensorflow.keras as ks
 
 # There are limitations for RaggedTensor working with standard Keras layers, but which are successively reduced with
 # more recent tensorflow/keras versions (tf-version >= 2.2).
 # For backward compatibility we keep keras layer replacements to work with RaggedTensor in this module.
 # For example with tf-version==2.8, DenseEmbedding is equivalent to ks.layers.Dense.
 # Note that here are LazyAdd and LazyConcatenate etc. layers which are slightly different from keras layer, which also
@@ -93,14 +94,15 @@
 @ks.utils.register_keras_serializable(package="kgcnn", name="ActivationEmbedding")
 class ActivationEmbedding(GraphBaseLayer):
     r"""Activation layer for ragged tensors representing a geometric or graph tensor such as node or edge embeddings.
     A :obj:`Activation` applies an activation function to an output, i.e. a transformation of the input
     :math:`\mathbf{x}` via activation function :math:`\sigma`.
 
     .. math::
+
         \mathbf{x}' = \sigma (\mathbf{x})
 
     """
 
     def __init__(self,
                  activation,
                  activity_regularizer=None,
```

### Comparing `kgcnn-3.0.1/kgcnn/layers/norm.py` & `kgcnn-3.0.2/kgcnn/layers/norm.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/pooling.py` & `kgcnn-3.0.2/kgcnn/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/relational.py` & `kgcnn-3.0.2/kgcnn/layers/relational.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/set2set.py` & `kgcnn-3.0.2/kgcnn/layers/set2set.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/layers/update.py` & `kgcnn-3.0.2/kgcnn/layers/update.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_attentivefp_conv.py` & `kgcnn-3.0.2/kgcnn/literature/AttentiveFP/_attentivefp_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/AttentiveFP/_make.py` & `kgcnn-3.0.2/kgcnn/literature/AttentiveFP/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/CGCNN/_cgcnn_conv.py` & `kgcnn-3.0.2/kgcnn/literature/CGCNN/_cgcnn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/CGCNN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/CGCNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/CMPNN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/CMPNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/DGIN/_dgin_conv.py` & `kgcnn-3.0.2/kgcnn/literature/DGIN/_dgin_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/DGIN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/DGIN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/DMPNN/_dmpnn_conv.py` & `kgcnn-3.0.2/kgcnn/literature/DMPNN/_dmpnn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/DMPNN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/DMPNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_dimenet_conv.py` & `kgcnn-3.0.2/kgcnn/literature/DimeNetPP/_dimenet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/DimeNetPP/_make.py` & `kgcnn-3.0.2/kgcnn/literature/DimeNetPP/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/EGNN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/EGNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GAT/_make.py` & `kgcnn-3.0.2/kgcnn/literature/GAT/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GATv2/_make.py` & `kgcnn-3.0.2/kgcnn/literature/GATv2/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GCN/_gcn_conv.py` & `kgcnn-3.0.2/kgcnn/literature/GCN/_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GCN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/GCN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GIN/_gin_conv.py` & `kgcnn-3.0.2/kgcnn/literature/GIN/_gin_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GIN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/GIN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_model.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_model.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_literature_gnnexplain.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_base.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_xai_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_testing.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_xai_testing.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_test_xai_utils.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_test_xai_utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_base.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_testing.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/_testing.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNExplain/_xai/_utils.py` & `kgcnn-3.0.2/kgcnn/literature/GNNExplain/_xai/_utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GNNFilm/_make.py` & `kgcnn-3.0.2/kgcnn/literature/GNNFilm/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/GraphSAGE/_make.py` & `kgcnn-3.0.2/kgcnn/literature/GraphSAGE/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_acsf_conv.py` & `kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/_acsf_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_make.py` & `kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HDNNP2nd/_wacsf_conv.py` & `kgcnn-3.0.2/kgcnn/literature/HDNNP2nd/_wacsf_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_hdnnp_conv.py` & `kgcnn-3.0.2/kgcnn/literature/HDNNP4th/_hdnnp_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_make.py` & `kgcnn-3.0.2/kgcnn/literature/HDNNP4th/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HDNNP4th/_test_hdnnp.py` & `kgcnn-3.0.2/kgcnn/literature/HDNNP4th/_test_hdnnp.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HamNet/_hamnet_conv.py` & `kgcnn-3.0.2/kgcnn/literature/HamNet/_hamnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/HamNet/_make.py` & `kgcnn-3.0.2/kgcnn/literature/HamNet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/INorp/_make.py` & `kgcnn-3.0.2/kgcnn/literature/INorp/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MAT/_make.py` & `kgcnn-3.0.2/kgcnn/literature/MAT/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MAT/_mat_conv.py` & `kgcnn-3.0.2/kgcnn/literature/MAT/_mat_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MEGAN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/MEGAN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MEGAN/_model.py` & `kgcnn-3.0.2/kgcnn/literature/MEGAN/_model.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MEGAN/_test_literature_megan.py` & `kgcnn-3.0.2/kgcnn/literature/MEGAN/_test_literature_megan.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MXMNet/_make.py` & `kgcnn-3.0.2/kgcnn/literature/MXMNet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MXMNet/_mxmnet_conv.py` & `kgcnn-3.0.2/kgcnn/literature/MXMNet/_mxmnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Megnet/_make.py` & `kgcnn-3.0.2/kgcnn/literature/Megnet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Megnet/_megnet_conv.py` & `kgcnn-3.0.2/kgcnn/literature/Megnet/_megnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MoGAT/_make.py` & `kgcnn-3.0.2/kgcnn/literature/MoGAT/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/MoGAT/_mogat_conv.py` & `kgcnn-3.0.2/kgcnn/literature/MoGAT/_mogat_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/NMPN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/NMPN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/NMPN/_mpnn_conv.py` & `kgcnn-3.0.2/kgcnn/literature/NMPN/_mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/PAiNN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/PAiNN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/PAiNN/_painn_conv.py` & `kgcnn-3.0.2/kgcnn/literature/PAiNN/_painn_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,44 +137,47 @@
         kernel_regularizer: Kernel regularization. Default is None.
         bias_regularizer: Bias regularization. Default is None.
         activity_regularizer: Activity regularization. Default is None.
         kernel_constraint: Kernel constrains. Default is None.
         bias_constraint: Bias constrains. Default is None.
         kernel_initializer: Initializer for kernels. Default is 'glorot_uniform'.
         bias_initializer: Initializer for bias. Default is 'zeros'.
+        add_eps: Whether to add eps in the norm.
     """
 
     def __init__(self, units,
                  use_bias=True,
                  activation='swish',
                  kernel_regularizer=None,
                  bias_regularizer=None,
                  activity_regularizer=None,
                  kernel_constraint=None,
                  bias_constraint=None,
                  kernel_initializer='glorot_uniform',
                  bias_initializer='zeros',
+                 add_eps: bool = False,
                  **kwargs):
         """Initialize Layer."""
         super(PAiNNUpdate, self).__init__(**kwargs)
         self.units = units
         self.use_bias = use_bias
+        self.add_eps = add_eps
 
         kernel_args = {"kernel_regularizer": kernel_regularizer, "activity_regularizer": activity_regularizer,
                        "bias_regularizer": bias_regularizer, "kernel_constraint": kernel_constraint,
                        "bias_constraint": bias_constraint, "kernel_initializer": kernel_initializer,
                        "bias_initializer": bias_initializer}
         # Layer
         self.lay_dense1 = Dense(units=self.units, activation=activation, use_bias=self.use_bias, **kernel_args)
         self.lay_lin_u = Dense(self.units, activation='linear', use_bias=False, **kernel_args)
         self.lay_lin_v = Dense(self.units, activation='linear', use_bias=False, **kernel_args)
         self.lay_a = Dense(units=self.units * 3, activation='linear', use_bias=self.use_bias, **kernel_args)
 
         self.lay_scalar_prod = ScalarProduct(axis=2)
-        self.lay_norm = EuclideanNorm(axis=2)
+        self.lay_norm = EuclideanNorm(axis=2, add_eps=self.add_eps)
         self.lay_concat = LazyConcatenate(axis=-1)
         self.lay_split = SplitEmbedding(3, axis=-1)
 
         self.lay_mult = LazyMultiply()
         self.lay_exp_v = ExpandDims(axis=-2)
         self.lay_mult_vv = LazyMultiply()
         self.lay_add = LazyAdd()
@@ -212,15 +215,15 @@
         ds = self.lay_mult([v_prod, a_sv], **kwargs)
         ds = self.lay_add([ds, a_ss], **kwargs)
         return ds, dv
 
     def get_config(self):
         """Update layer config."""
         config = super(PAiNNUpdate, self).get_config()
-        config.update({"units": self.units})
+        config.update({"units": self.units, "add_eps": self.add_eps})
         config_dense = self.lay_dense1.get_config()
         for x in ["kernel_regularizer", "activity_regularizer", "bias_regularizer", "kernel_constraint",
                   "bias_constraint", "kernel_initializer", "bias_initializer", "activation", "use_bias"]:
             config.update({x: config_dense[x]})
         return config
 
 
@@ -321,15 +324,15 @@
         super(SplitEmbedding, self).build(input_shape)
         # If rank is not defined can't call on values if axis does not happen to be positive.
         self.axis = get_positive_axis(self.axis, len(input_shape))
         if self.axis <= 1:
             raise ValueError("Can not split tensor at axis <= 1.")
 
     def call(self, inputs, **kwargs):
-        r"""Forward pass: Split embeddings across feature dimension e.g. `axis=-1`..
+        r"""Forward pass: Split embeddings across feature dimension e.g. `axis=-1` .
 
         Args:
             inputs (tf.RaggedTensor): Embeddings of shape (batch, [N], F)
 
         Returns:
             list: List of tensor splits of shape (batch, [N], F/num)
         """
```

### Comparing `kgcnn-3.0.1/kgcnn/literature/RGCN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/RGCN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Schnet/_make.py` & `kgcnn-3.0.2/kgcnn/literature/Schnet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Schnet/_schnet_conv.py` & `kgcnn-3.0.2/kgcnn/literature/Schnet/_schnet_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Unet/_make.py` & `kgcnn-3.0.2/kgcnn/literature/Unet/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Unet/_test_connect.py` & `kgcnn-3.0.2/kgcnn/literature/Unet/_test_connect.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Unet/_test_topk.py` & `kgcnn-3.0.2/kgcnn/literature/Unet/_test_topk.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/Unet/_topk.py` & `kgcnn-3.0.2/kgcnn/literature/Unet/_topk.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/__init__.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/__init__.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_coGN_config.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_coGN_config.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_coNGN_config.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_coNGN_config.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_embedding_layers/_atom_embedding.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_embedding_layers/_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_gates.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_gates.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_network_base.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_graph_network/graph_network_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_graph_network/graph_networks.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_graph_network/graph_networks.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_multiplicity_readout.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_multiplicity_readout.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_preprocessing_layers.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_preprocessing_layers.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/coGN/_test.py` & `kgcnn-3.0.2/kgcnn/literature/coGN/_test.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/rGIN/_make.py` & `kgcnn-3.0.2/kgcnn/literature/rGIN/_make.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/literature/rGIN/_rgin_conv.py` & `kgcnn-3.0.2/kgcnn/literature/rGIN/_rgin_conv.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/metrics/loss.py` & `kgcnn-3.0.2/kgcnn/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/metrics/metrics.py` & `kgcnn-3.0.2/kgcnn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/model/force.py` & `kgcnn-3.0.2/kgcnn/model/force.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='EnergyForceModel')
 class EnergyForceModel(ks.models.Model):
     r"""Force model that generates forces from any energy predicting model by taking the derivative with respect to
     the input coordinates.
 
-    For now the model has to cast to dense tensor for using :obj:`batch_jacobian` , however, this will likely support
-    ragged tensors in the future.
+    There are different options regarding the gradient.
+    For :obj:`use_batch_jacobian` the model has to cast to dense tensor for using :obj:`batch_jacobian` ,
+    however, this will likely support ragged tensors in the future.
 
     .. code-block:: python
 
         import tensorflow as tf
         from kgcnn.model.force import EnergyForceModel
         model = EnergyForceModel(
             model_energy= {
@@ -45,28 +46,30 @@
                     "output_mlp": None
                 }
             },
             coordinate_input=1,
             output_as_dict=True,
             output_to_tensor=False,
             output_squeeze_states=True,
-            is_physical_force=True
+            is_physical_force=True,
+            use_batch_jacobian=True
         )
 
     """
 
     def __init__(self,
                  model_energy=None,
                  coordinate_input: Union[int, str] = 1,
                  output_as_dict: bool = True,
                  ragged_validate: bool = False,
                  output_to_tensor: bool = True,
                  output_squeeze_states: bool = False,
                  nested_model_config: bool = True,
                  is_physical_force: bool = True,
+                 use_batch_jacobian: bool = True,
                  **kwargs):
         r"""Initialize :obj:`EnergyForceModel` with sub-model for energy prediction.
 
         This wrapper model was designed for models in `kgcnn.literature` that predict energy from geometric
         information.
 
         .. note::
@@ -78,17 +81,20 @@
         Args:
             model_energy (dict): Keras model for energy prediction. Can also be a serialization dict.
             coordinate_input (str, int): Index or key where to find coordinate tensor in model input.
             output_as_dict (bool): Whether to return energy and force as list or as dict. Default is True.
             ragged_validate (bool): Whether to validate ragged tensor creation. Default is False.
             output_to_tensor (bool): Whether to cast the output to tensor or keep ragged output. Default is True
             output_squeeze_states (bool): Whether to squeeze states, which can be done for one energy value to remove
-                an axis of one.
+                an axis of one. Only set this to true if axis is one, i.e. only one energy state as target.
             nested_model_config (bool): Whether `config` has model config of the energy model. Default is True.
             is_physical_force (bool): Whether gradient of force, which is the negative gradient, is to be returned.
+            use_batch_jacobian (bool): Whether to used batch-wise Jacobian to compute forces. This could be desired,
+                if you use e.g. :obj:`GraphBatchNormalization` and have a batch dimension > 1. Otherwise, the energies
+                are computed a standard gradient of energies.
         """
         super(EnergyForceModel, self).__init__(self, **kwargs)
         if model_energy is None:
             raise ValueError("Require valid model in `model_energy` for force prediction.")
 
         # Input for model_energy.
         self._model_energy = model_energy
@@ -109,14 +115,15 @@
         self.ragged_validate = ragged_validate
         self.coordinate_input = coordinate_input
         self.output_as_dict = output_as_dict
         self.output_to_tensor = output_to_tensor
         self.output_squeeze_states = output_squeeze_states
         self.is_physical_force = is_physical_force
         self.nested_model_config = nested_model_config
+        self.use_batch_jacobian = use_batch_jacobian
 
         # Layers.
         self.cast_coordinates = ChangeTensorType(input_tensor_type="ragged", output_tensor_type="mask")
 
     def call(self, inputs, training=False, **kwargs):
         """Forward pass that wraps energy model in gradient tape.
 
@@ -126,37 +133,53 @@
             training (bool): Whether model is in training, passed to energy model. Default is False.
 
         Returns:
             dict, list: Model output plus force or derivative.
         """
         x = inputs[self.coordinate_input]
         inputs_energy = [i for i in inputs]
-        # x is ragged tensor of shape (batch, [N], 3) with cartesian coordinates.
-        # `batch_jacobian` does not yet support ragged tensor input.
-        # Cast to masked tensor for coordinates only.
-        x_pad, x_mask = self.cast_coordinates(x, training=training, **kwargs)  # (batch, N, 3), (batch, N, 3)
-        with tf.GradientTape() as tape:
-            tape.watch(x_pad)
-            # Temporary solution for casting.
-            # Cast back to ragged tensor for model input.
-            x_pad_to_ragged = self._cast_coordinates_pad_to_ragged(x_pad, x_mask, self.ragged_validate)
-            inputs_energy[self.coordinate_input] = x_pad_to_ragged
-            # Predict energy.
-            # Energy must be tensor of shape (batch, states)
-            eng = self.energy_model(inputs_energy, training=training, **kwargs)
-        e_grad = tape.batch_jacobian(eng, x_pad)
-        e_grad = tf.transpose(e_grad, perm=[0, 2, 3, 1])
-
-        if self.is_physical_force:
-            e_grad = -e_grad
-
-        if self.output_squeeze_states:
-            e_grad = tf.squeeze(e_grad, axis=-1)
-        if not self.output_to_tensor:
-            e_grad = self._cast_coordinates_pad_to_ragged(e_grad, x_mask, self.ragged_validate)
+
+        if self.use_batch_jacobian:
+            # x is ragged tensor of shape (batch, [N], 3) with cartesian coordinates.
+            # `batch_jacobian` does not yet support ragged tensor input.
+            # Cast to masked tensor for coordinates only.
+            x_pad, x_mask = self.cast_coordinates(x, training=training, **kwargs)  # (batch, N, 3), (batch, N, 3)
+            with tf.GradientTape() as tape:
+                tape.watch(x_pad)
+                # Temporary solution for casting.
+                # Cast back to ragged tensor for model input.
+                x_pad_to_ragged = self._cast_coordinates_pad_to_ragged(x_pad, x_mask, self.ragged_validate)
+                inputs_energy[self.coordinate_input] = x_pad_to_ragged
+                # Predict energy.
+                # Energy must be tensor of shape (batch, states)
+                eng = self.energy_model(inputs_energy, training=training, **kwargs)
+            e_grad = tape.batch_jacobian(eng, x_pad)
+            e_grad = tf.transpose(e_grad, perm=[0, 2, 3, 1])
+            if self.is_physical_force:
+                e_grad = -e_grad
+            if self.output_squeeze_states:
+                e_grad = tf.squeeze(e_grad, axis=-1)
+            if not self.output_to_tensor:
+                e_grad = self._cast_coordinates_pad_to_ragged(e_grad, x_mask, self.ragged_validate)
+        else:
+            with tf.GradientTape(persistent=True) as tape:
+                tape.watch(x.values)
+                eng = self.energy_model(inputs_energy, training=training, **kwargs)
+                eng_sum = tf.reduce_sum(eng, axis=0, keepdims=False)
+                e_grad = [eng_sum[i] for i in range(eng_sum.shape[-1])]
+            e_grad = [tf.expand_dims(tape.gradient(e_i, x.values), axis=-1) for e_i in e_grad]
+            e_grad = tf.concat(e_grad, axis=-1)
+            if self.is_physical_force:
+                e_grad = -e_grad
+            if self.output_squeeze_states:
+                e_grad = tf.squeeze(e_grad, axis=-1)
+            e_grad = tf.RaggedTensor.from_row_splits(e_grad, x.row_splits, validate=False)
+            if self.output_to_tensor:
+                e_grad = tf.RaggedTensor.to_tensor(e_grad)
+
         if self.output_as_dict:
             return {"energy": eng, "force": e_grad}
         else:
             return eng, e_grad
 
     # Temporary solution.
     @staticmethod
@@ -181,10 +204,11 @@
         conf.update({
             "model_energy": model_energy,
             "coordinate_input": self.coordinate_input,
             "output_as_dict": self.output_as_dict,
             "ragged_validate": self.ragged_validate,
             "output_to_tensor": self.output_to_tensor,
             "output_squeeze_states": self.output_squeeze_states,
-            "nested_model_config": self.nested_model_config
+            "nested_model_config": self.nested_model_config,
+            "use_batch_jacobian": self.use_batch_jacobian
         })
         return conf
```

### Comparing `kgcnn-3.0.1/kgcnn/model/utils.py` & `kgcnn-3.0.2/kgcnn/model/utils.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/base.py` & `kgcnn-3.0.2/kgcnn/molecule/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/convert.py` & `kgcnn-3.0.2/kgcnn/molecule/convert.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/dynamics/ase_calc.py` & `kgcnn-3.0.2/kgcnn/molecule/dynamics/ase_calc.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/dynamics/base.py` & `kgcnn-3.0.2/kgcnn/molecule/dynamics/base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/encoder.py` & `kgcnn-3.0.2/kgcnn/molecule/encoder.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/external/ballloon.py` & `kgcnn-3.0.2/kgcnn/molecule/external/ballloon.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/graph_babel.py` & `kgcnn-3.0.2/kgcnn/molecule/graph_babel.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/graph_rdkit.py` & `kgcnn-3.0.2/kgcnn/molecule/graph_rdkit.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/io.py` & `kgcnn-3.0.2/kgcnn/molecule/io.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/methods.py` & `kgcnn-3.0.2/kgcnn/molecule/methods.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/molecule/serial.py` & `kgcnn-3.0.2/kgcnn/molecule/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/activ.py` & `kgcnn-3.0.2/kgcnn/layers/activ.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,100 @@
 import tensorflow as tf
-ks = tf.keras
-
+import numpy as np
+from kgcnn.layers.base import GraphBaseLayer
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='shifted_softplus')
-def shifted_softplus(x):
-    r"""Shifted soft-plus activation function.
-    
-    Args:
-        x (tf.Tensor): Single values to apply activation with tf.keras functions.
-    
-    Returns:
-        tf.Tensor: Output tensor computed as :math:`\log(e^{x}+1) - \log(2)`.
-    """
-    return ks.activations.softplus(x) - ks.backend.log(2.0)
-
-
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='softplus2')
-def softplus2(x):
-    r"""Soft-plus function that is :math:`0` at :math:`x=0`, the implementation aims at avoiding overflow
-    :math:`\log(e^{x}+1) - \log(2)`.
-    
-    Args:
-        x (tf.Tensor): Single values to apply activation with tf.keras functions.
-    
-    Returns:
-         tf.Tensor: Output tensor computed as :math:`\log(e^{x}+1) - \log(2)`.
-    """
-    return ks.backend.relu(x) + ks.backend.log(0.5 * ks.backend.exp(-ks.backend.abs(x)) + 0.5)
+ks = tf.keras
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='leaky_softplus')
-class leaky_softplus(tf.keras.layers.Layer):
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='LeakySoftplus')
+class LeakySoftplus(GraphBaseLayer):
     r"""Leaky softplus activation function similar to :obj:`tf.nn.leaky_relu` but smooth. """
 
-    def __init__(self, alpha=0.05, **kwargs):
+    def __init__(self, alpha: float = 0.05, trainable: bool = False, **kwargs):
         """Initialize with optionally learnable parameter.
 
         Args:
             alpha (float, optional): Leak parameter alpha. Default is 0.05.
+            trainable (bool, optional): Whether set alpha trainable. Default is False.
         """
-        super(leaky_softplus, self).__init__(**kwargs)
-        # self.alpha = self.add_weight(shape=None, dtype=self.dtype, trainable=trainable)
-        # self.set_weights([np.array(alpha)])
-        self.alpha = float(alpha)
+        super(LeakySoftplus, self).__init__(**kwargs)
+        self._alpha_config = float(alpha)
+        self._alpha_trainable = bool(trainable)
+        self.alpha = self.add_weight(shape=None, dtype=self.dtype, trainable=self._alpha_trainable)
+        self.set_weights([np.array(alpha)])
 
-    def call(self, inputs, **kwargs):
+    def _activ_implementation(self, inputs, **kwargs):
         """Compute leaky_softplus activation from inputs."""
         x = inputs
         return ks.activations.softplus(x) * (1 - self.alpha) + self.alpha * x
 
+    def call(self, inputs, *args, **kwargs):
+        return self.map_values(self._activ_implementation, inputs, **kwargs)
+
     def get_config(self):
-        config = super(leaky_softplus, self).get_config()
-        config.update({"alpha": self.alpha})
+        config = super(LeakySoftplus, self).get_config()
+        config.update({"alpha": self._alpha_config, "trainable": self._alpha_trainable})
         return config
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='leaky_relu')
-class leaky_relu(tf.keras.layers.Layer):
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='LeakyRelu')
+class LeakyRelu(GraphBaseLayer):
     r"""Leaky RELU function. Equivalent to :obj:`tf.nn.leaky_relu(x,alpha)`."""
 
-    def __init__(self, alpha: float = 0.05, **kwargs):
+    def __init__(self, alpha: float = 0.05, trainable: bool = False, **kwargs):
         """Initialize with optionally learnable parameter.
 
         Args:
             alpha (float, optional): Leak parameter alpha. Default is 0.05.
+            trainable (bool, optional): Whether set alpha trainable. Default is False.
         """
-        super(leaky_relu, self).__init__(**kwargs)
-        self.alpha = float(alpha)
+        super(LeakyRelu, self).__init__(**kwargs)
+        self._alpha_config = float(alpha)
+        self._alpha_trainable = bool(trainable)
+        self.alpha = self.add_weight(shape=None, dtype=self.dtype, trainable=self._alpha_trainable)
+        self.set_weights([np.array(alpha)])
 
-    def call(self, inputs, **kwargs):
+    def _activ_implementation(self, inputs, **kwargs):
         """Compute leaky_relu activation from inputs."""
         x = inputs
         return tf.nn.leaky_relu(x, alpha=self.alpha)
         # return tf.nn.relu(x) - tf.nn.relu(-x)*self.alpha
 
+    def call(self, inputs, *args, **kwargs):
+        return self.map_values(self._activ_implementation, inputs, **kwargs)
+
     def get_config(self):
-        config = super(leaky_relu, self).get_config()
-        config.update({"alpha": self.alpha})
+        config = super(LeakyRelu, self).get_config()
+        config.update({"alpha": self._alpha_config, "trainable": self._alpha_trainable})
         return config
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='swish')
-class swish(tf.keras.layers.Layer):
+@tf.keras.utils.register_keras_serializable(package='kgcnn', name='Swish')
+class Swish(GraphBaseLayer):
     r"""Swish activation function. Computes :math:`x \; \text{sig}(\beta x)`,
     with :math:`\text{sig}(x) = 1/(1+e^{-x})`."""
 
-    def __init__(self, beta: float = 1.0, **kwargs):
+    def __init__(self, beta: float = 1.0, trainable: bool = False, **kwargs):
         """Initialize with optionally learnable parameter.
 
         Args:
             beta (float, optional): Parameter beta in sigmoid. Default is 1.0.
+            trainable (bool, optional): Whether set beta trainable. Default is False.
         """
-        super(swish, self).__init__(**kwargs)
-        # self.beta = self.add_weight(shape=None, dtype=self.dtype, trainable=trainable)
-        # self.set_weights([np.array(beta)])
-        self.beta = float(beta)
+        super(Swish, self).__init__(**kwargs)
+        self._beta_config = float(beta)
+        self._beta_trainable = bool(trainable)
+        self.beta = self.add_weight(shape=None, dtype=self.dtype, trainable=self._beta_trainable)
+        self.set_weights([np.array(beta)])
 
-    def call(self, inputs, **kwargs):
+    def _activ_implementation(self, inputs, **kwargs):
         """Compute swish activation from inputs."""
         x = inputs
-        return x * tf.sigmoid(self.beta*x)
+        return x * tf.sigmoid(self.beta * x)
+
+    def call(self, inputs, *args, **kwargs):
+        return self.map_values(self._activ_implementation, inputs, **kwargs)
 
     def get_config(self):
-        config = super(swish, self).get_config()
-        config.update({"beta": self.beta})
+        config = super(Swish, self).get_config()
+        config.update({"beta": self._beta_config, "trainable": self._beta_trainable})
         return config
```

### Comparing `kgcnn-3.0.1/kgcnn/ops/axis.py` & `kgcnn-3.0.2/kgcnn/ops/axis.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/initializer.py` & `kgcnn-3.0.2/kgcnn/ops/initializer.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/partition.py` & `kgcnn-3.0.2/kgcnn/ops/partition.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/polynom.py` & `kgcnn-3.0.2/kgcnn/ops/polynom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/ragged.py` & `kgcnn-3.0.2/kgcnn/ops/ragged.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/scatter.py` & `kgcnn-3.0.2/kgcnn/ops/scatter.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/ops/segment.py` & `kgcnn-3.0.2/kgcnn/ops/segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,13 +40,14 @@
         pool = tf.math.segment_mean(data, segment_ids)
     elif segment_name in ["segment_sum", "sum", "reduce_sum"]:
         pool = tf.math.segment_sum(data, segment_ids)
     elif segment_name in ["segment_max", "max", "reduce_max"]:
         pool = tf.math.segment_max(data, segment_ids)
     elif segment_name in ["segment_min", "min", "reduce_min"]:
         pool = tf.math.segment_min(data, segment_ids)
-    # softmax does not reduce tensor.
+    # softmax does not really reduce tensor.
+    # which is why it is not added to the list of segment operations for normal pooling.
     # elif segment_name in ["segment_softmax", "segment_soft_max", "softmax", "soft_max", "reduce_softmax"]:
     #     pool = segment_softmax(data, segment_ids)
     else:
         raise TypeError("Unknown segment operation, choose: 'segment_mean', 'segment_sum', ...")
     return pool
```

### Comparing `kgcnn-3.0.1/kgcnn/training/callbacks.py` & `kgcnn-3.0.2/kgcnn/training/callbacks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # import numpy as np
 import tensorflow as tf
+ks = tf.keras
 
 
-@tf.keras.utils.register_keras_serializable(package='kgcnn', name='LearningRateLoggingCallback')
-class LearningRateLoggingCallback(tf.keras.callbacks.Callback):
+@ks.utils.register_keras_serializable(package='kgcnn', name='LearningRateLoggingCallback')
+class LearningRateLoggingCallback(ks.callbacks.Callback):
     """Callback logging the learning rate."""
 
     def __init__(self, verbose: int = 1):
         """Initialize class.
 
         Args:
             verbose (int): Verbosity. Default is 1.
@@ -24,15 +25,20 @@
 
         Returns:
             None.
         """
         lr = self.model.optimizer.lr
         tf.summary.scalar('learning rate', data=lr, step=epoch)
         logs = logs or {}
-        logs['lr'] = tf.keras.backend.get_value(self.model.optimizer.lr)
+        logs['lr'] = ks.backend.get_value(self.model.optimizer.lr)
         if self.verbose > 0:
-            print("\nEpoch %05d: Finished epoch with learning rate: %s.\n" % (epoch + 1, float(lr)))
+            print("\nEpoch %05d: Finished epoch with learning rate: %s.\n" % (epoch + 1, logs['lr']))
 
     def get_config(self):
         """Get config for this class."""
         config = {"verbose": self.verbose}
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
```

### Comparing `kgcnn-3.0.1/kgcnn/training/history.py` & `kgcnn-3.0.2/kgcnn/training/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,33 +25,36 @@
         model_name: str = "",
         file_name: str = "score.yaml",
         model_version: str = "",
         dataset_name: str = "",
         model_class: str = "",
         execute_folds: Union[list, int, None] = None,
         multi_target_indices: Union[list, int, None] = None,
-        trajectory_name: str = None
+        trajectory_name: str = None,
+        time_list: list = None
 ):
     r"""Save fit results from fit histories to file.
 
     This function is used in training scripts to record final training and validation metrics.
 
     Args:
         histories (list): List of :obj:`tf.keras.callbacks.History()` objects.
         filepath (str): Full path where to save plot to, without the name of the file. Default is "".
         loss_name (str): Which loss or metric to pick from history. Default is "loss".
         val_loss_name (str): Which validation loss or metric to pick from history. Default is "val_loss".
         data_unit (str): Unit of the loss. Default is "".
         model_name (str): Name of the model. Default is "".
         file_name (str): File name base. Model name and dataset will be added to the name. Default is "".
+        model_version (str): Version of the model. Default is "".
         dataset_name (str): Name of the dataset which was fitted to. Default is "".
         model_class (str): Model class or generator. Default is "".
         execute_folds (list, int): Folds which where executed.
         multi_target_indices (list): List of indices for multi target training. Default is None.
         trajectory_name (str): Name of the trajectory if known. Default is None.
+        time_list (list): List of training time info.
 
     Returns:
         dict: Score which was saved to file.
     """
     histories = [hist.history if isinstance(hist, tf.keras.callbacks.History) else hist for hist in histories]
     # We assume multiple fits as in KFold.
     if data_unit is None:
@@ -97,14 +100,15 @@
     result_dict["model_class"] = str(model_class)
     result_dict["model_version"] = str(model_version)
     result_dict["model_name"] = str(model_name)
     result_dict["kgcnn_version"] = str(__kgcnn_version__)
     result_dict["number_histories"] = len(histories)
     result_dict["multi_target_indices"] = multi_target_indices
     result_dict["execute_folds"] = execute_folds
+    result_dict["time_list"] = time_list
     if trajectory_name:
         result_dict["trajectory_name"] = trajectory_name
 
     if filepath is not None:
         save_yaml_file(result_dict, os.path.join(filepath, model_name + "_" + dataset_name + "_" + file_name))
 
     return result_dict
```

### Comparing `kgcnn-3.0.1/kgcnn/training/hyper.py` & `kgcnn-3.0.2/kgcnn/training/hyper.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,17 +245,17 @@
             validation_freq = hyper_fit["validation_freq"]
         if "batch_size" in hyper_fit:
             batch_size = hyper_fit["batch_size"]
         if "callbacks" in hyper_fit:
             if callbacks is None:
                 callbacks = []
             for cb in hyper_fit["callbacks"]:
-                try:
+                if isinstance(cb, (str, dict)):
                     callbacks += [tf.keras.utils.deserialize_keras_object(cb)]
-                except:
+                else:
                     callbacks += [cb]
 
         out = {"batch_size": batch_size, "epochs": epochs, "validation_freq": validation_freq, "callbacks": callbacks}
         out.update(hyper_fit_additional)
         return out
 
     def results_file_path(self):
```

### Comparing `kgcnn-3.0.1/kgcnn/training/optimizer.py` & `kgcnn-3.0.2/kgcnn/training/optimizer.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/training/schedule.py` & `kgcnn-3.0.2/kgcnn/training/schedule.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/training/scheduler.py` & `kgcnn-3.0.2/kgcnn/training/scheduler.py`

 * *Files 13% similar despite different names*

```diff
@@ -90,14 +90,19 @@
     def get_config(self):
         """Get config for this class."""
         config = super(LinearWarmUpScheduler, self).get_config()
         config.update({"lr_start": self.lr_start, "epo_warmup": self.epo_warmup,
                        "verbose": self.verbose, "steps_per_epoch": self.steps_per_epoch})
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
+
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='CosineAnnealingLRScheduler')
 class CosineAnnealingLRScheduler(ks.callbacks.LearningRateScheduler):
     r"""Callback for cosine learning rate (LR) schedule. This class inherits from
     :obj:`ks.callbacks.LearningRateScheduler` and applies :obj:`schedule_epoch_lr`.
     Proposed by `SGDR <https://arxiv.org/abs/1608.03983>`_.
     The cosine part without restarts for the LR Schedule follows:
@@ -133,14 +138,19 @@
     def get_config(self):
         """Get config for this class."""
         config = super(CosineAnnealingLRScheduler, self).get_config()
         config.update({"lr_start": self.lr_start, "epoch_max": self.epoch_max,
                        "lr_min": self.lr_min, "verbose": self.verbose})
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
+
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='LinearWarmupExponentialLRScheduler')
 class LinearWarmupExponentialLRScheduler(LinearWarmUpScheduler):
     r"""Callback for exponential learning rate schedule with warmup. This class inherits from
     :obj:`LinearWarmUpScheduler`, which inherits from :obj:`ks.callbacks.LearningRateScheduler`.
     The learning rate :math:`\eta` is reduced or increased (usually :math:`\gamma < 1`) after
     warmup epochs :math:`T_0` as:
@@ -185,14 +195,19 @@
 
     def get_config(self):
         """Get config for this class."""
         config = super(LinearWarmupExponentialLRScheduler, self).get_config()
         config.update({"gamma": self.gamma, "lr_min": self.lr_min})
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
+
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='LinearWarmupExponentialLearningRateScheduler')
 class LinearWarmupExponentialLearningRateScheduler(LinearWarmUpScheduler):
     r"""Callback for exponential learning rate schedule with warmup. This class inherits from
     :obj:`LinearWarmUpScheduler`, which inherits from :obj:`ks.callbacks.LearningRateScheduler`.
     The learning rate :math:`\eta` is reduced after warmup epochs :math:`T_0` with lifetime :math:`\tau` as:
 
@@ -236,14 +251,19 @@
 
     def get_config(self):
         """Get config for this class."""
         config = super(LinearWarmupExponentialLearningRateScheduler, self).get_config()
         config.update({"decay_lifetime": self.decay_lifetime, "lr_min": self.lr_min})
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
+
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='LinearLearningRateScheduler')
 class LinearLearningRateScheduler(ks.callbacks.LearningRateScheduler):
     r"""Callback for linear change of the learning rate. This class inherits from
     :obj:`ks.callbacks.LearningRateScheduler`.
     The learning rate :math:`\eta_0` is reduced linearly at :math:`T_0` epochs up to :math:`T_{max}`
     epochs to reach the learning rate :math:`\eta_{T_{max}}`:
@@ -295,14 +315,19 @@
         """Get config for this class."""
         config = super(LinearLearningRateScheduler, self).get_config()
         config.update({"learning_rate_start": self.learning_rate_start,
                        "learning_rate_stop": self.learning_rate_stop,
                        "epo": self.epo, "epo_min": self.epo_min, "eps": self.eps})
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
+
 
 @ks.utils.register_keras_serializable(package='kgcnn', name='LinearWarmupLinearLearningRateScheduler')
 class LinearWarmupLinearLearningRateScheduler(LinearWarmUpScheduler):
     r"""Callback for linear change of the learning rate with warmup. This class inherits from
     :obj:`LinearWarmUpScheduler`, which inherits from :obj:`ks.callbacks.LearningRateScheduler`.
     The learning rate is increased in a warmup phase of :math:`T_0` epochs up to :math:`\eta_0`.
     The learning rate :math:`\eta_0` is reduced linearly at :math:`T_0` epochs up to :math:`T_{max}`
@@ -354,7 +379,82 @@
     def get_config(self):
         """Get config for this class."""
         config = super(LinearWarmupLinearLearningRateScheduler, self).get_config()
         config.update({
             "learning_rate_start": self.learning_rate_start, "learning_rate_stop": self.learning_rate_stop,
             "epo": self.epo, "eps": self.eps})
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
+
+
+@ks.utils.register_keras_serializable(package='kgcnn', name='PolynomialDecayScheduler')
+class PolynomialDecayScheduler(ks.callbacks.LearningRateScheduler):
+    r"""Callback for polynomial decay of the learning rate. This class inherits from
+    :obj:`ks.callbacks.LearningRateScheduler`.
+
+    Adapts :obj:`keras.optimizers.schedules.PolynomialDecay` to a scheduler with a function of epochs.
+
+    """
+
+    def __init__(self, initial_learning_rate, decay_epochs, end_learning_rate=0.0001, power=1.0, cycle=False,
+                 verbose: int = 0, eps: float = 1e-8):
+        """Set the parameters for the learning rate scheduler.
+
+        Args:
+            initial_learning_rate (float): The initial learning rate
+            decay_epochs (float): Must be positive. See the decay computation above.
+            end_learning_rate (float): The minimal end learning rate.
+            power (float): The power of the polynomial. Defaults to `1.0` .
+            cycle (bool): A boolean, whether it should cycle beyond decay_steps.
+            eps (float): Minimum learning rate. Default is 1e-08.
+            verbose (int): Verbosity. Default is 0.
+        """
+        super(PolynomialDecayScheduler, self).__init__(schedule=self.schedule_epoch_lr, verbose=verbose)
+        self.initial_learning_rate = initial_learning_rate
+        self.decay_epochs = decay_epochs
+        self.end_learning_rate = end_learning_rate
+        self.power = power
+        self.cycle = cycle
+        self.verbose = verbose
+        self.eps = eps
+
+    def schedule_epoch_lr(self, epoch, lr):
+        r"""Reduce the learning linearly.
+
+        Args:
+            epoch (int): Epoch index (integer, indexed from 0).
+            lr (float): Current learning rate. Not used.
+
+        Returns:
+            float: New learning rate.
+        """
+        if not self.cycle:
+            epoch = np.minimum(self.decay_epochs, epoch)
+            decay_epoch = self.decay_epochs
+        else:
+            decay_epoch = self.decay_epochs * np.ceil(epoch / self.decay_epochs)
+        pp = np.power(1 - epoch / decay_epoch, self.power)
+        new_lr = (self.initial_learning_rate - self.end_learning_rate) * pp + self.end_learning_rate
+        return max(float(new_lr), float(self.eps))
+
+    def get_config(self):
+        """Get config for this class."""
+        config = super(PolynomialDecayScheduler, self).get_config()
+        config.update({
+            "initial_learning_rate": self.initial_learning_rate,
+            "decay_epochs": self.decay_epochs,
+            "end_learning_rate": self.end_learning_rate,
+            "power": self.power,
+            "cycle": self.cycle,
+            "verbose": self.verbose,
+            "eps": self.eps
+        })
+        return config
+
+    @classmethod
+    def from_config(cls, config):
+        """Make class instance from config."""
+        return cls(**config)
```

### Comparing `kgcnn-3.0.1/kgcnn/utils/devices.py` & `kgcnn-3.0.2/kgcnn/utils/devices.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/utils/plots.py` & `kgcnn-3.0.2/kgcnn/utils/plots.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn/utils/serial.py` & `kgcnn-3.0.2/kgcnn/utils/serial.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/kgcnn.egg-info/PKG-INFO` & `kgcnn-3.0.2/kgcnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgcnn
-Version: 3.0.1
+Version: 3.0.2
 Summary: General Base Layers for Graph Convolutions with tensorflow.keras
 Home-page: https://github.com/aimat-lab/gcnn_keras
 Author: Patrick Reiser
 Author-email: patrick.reiser@kit.edu
 License: UNKNOWN
 Keywords: materials,science,machine,learning,deep,graph,networks,neural
 Platform: UNKNOWN
```

### Comparing `kgcnn-3.0.1/kgcnn.egg-info/SOURCES.txt` & `kgcnn-3.0.2/kgcnn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,23 @@
 kgcnn/graph/base.py
 kgcnn/graph/postprocessor.py
 kgcnn/graph/preprocessor.py
 kgcnn/graph/serial.py
 kgcnn/graph/methods/__init__.py
 kgcnn/graph/methods/_adj.py
 kgcnn/graph/methods/_geom.py
+kgcnn/graph/methods/_periodic.py
 kgcnn/io/__init__.py
 kgcnn/io/file.py
+kgcnn/io/graphlist.py
 kgcnn/io/loader.py
 kgcnn/layers/README.md
 kgcnn/layers/__init__.py
+kgcnn/layers/activ.py
+kgcnn/layers/aggr.py
 kgcnn/layers/attention.py
 kgcnn/layers/base.py
 kgcnn/layers/casting.py
 kgcnn/layers/conv.py
 kgcnn/layers/gather.py
 kgcnn/layers/geom.py
 kgcnn/layers/message.py
@@ -201,14 +205,15 @@
 kgcnn/literature/rGIN/_rgin_conv.py
 kgcnn/metrics/__init__.py
 kgcnn/metrics/loss.py
 kgcnn/metrics/metrics.py
 kgcnn/model/README.md
 kgcnn/model/__init__.py
 kgcnn/model/force.py
+kgcnn/model/multi.py
 kgcnn/model/serial.py
 kgcnn/model/utils.py
 kgcnn/molecule/__init__.py
 kgcnn/molecule/base.py
 kgcnn/molecule/convert.py
 kgcnn/molecule/encoder.py
 kgcnn/molecule/graph_babel.py
@@ -245,13 +250,13 @@
 kgcnn/utils/plots.py
 kgcnn/utils/serial.py
 test/__init__.py
 test/test_data_base.py
 test/test_data_moleculenet.py
 test/test_graph_base.py
 test/test_graph_methods.py
+test/test_graph_methods_periodic.py
 test/test_layers_attention.py
 test/test_layers_gather.py
 test/test_layers_geom.py
 test/test_layers_pooling.py
-test/test_range_periodic.py
 test/utils.py
```

### Comparing `kgcnn-3.0.1/setup.py` & `kgcnn-3.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="kgcnn",
-    version="3.0.1",  # If version is updated, change version in `kgcnn.__init__` too. (and update changelog)
+    version="3.0.2",  # If version is updated, change version in `kgcnn.__init__` too. (and update changelog)
     author="Patrick Reiser",
     author_email="patrick.reiser@kit.edu",
     description="General Base Layers for Graph Convolutions with tensorflow.keras",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aimat-lab/gcnn_keras",
     install_requires=[
@@ -28,15 +28,15 @@
         "networkx>=2.8.8",
         "sympy>=1.11.1",
         "pyyaml>=6.0",
         "ase>=3.22.1",
         "click>=7.1.2",
         "brotli>=1.0.9",
         "pyxtal>=0.5.5",
-        "h5py"
+        "h5py>=3.9.0"
     ],
     extras_require={
         "openbabel": ["openbabel"],
     },
     packages=find_packages(),
     include_package_data=True,
     package_data={"kgcnn": ["*.json", "*.yaml", "*.csv", "*.md"]},
```

### Comparing `kgcnn-3.0.1/test/test_data_base.py` & `kgcnn-3.0.2/test/test_data_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/test/test_data_moleculenet.py` & `kgcnn-3.0.2/test/test_data_moleculenet.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/test/test_graph_base.py` & `kgcnn-3.0.2/test/test_graph_base.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/test/test_graph_methods.py` & `kgcnn-3.0.2/test/test_graph_methods.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/test/test_layers_attention.py` & `kgcnn-3.0.2/test/test_layers_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                        tf.RaggedTensor.from_row_lengths(np.array([[0.0],[1.0],[0.0],[1.0]]), np.array([2,2])),
                        tf.RaggedTensor.from_row_lengths(np.array([[0,0],[0,0],[0,0],[0,0]]),np.array([2,2]))]
                        )
         result = result[0].numpy()
         self.assertTrue(np.abs(result[0] - 100.0 * 1/(np.exp(1)+1) ) < 1e-4)
 
     def test_attention_head(self):
-
+        # print("Test is using:", tf.__version__)
         n = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
         edi = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,))
         ed = tf.ragged.constant(self.e1, ragged_rank=1, inner_shape=(1,))
 
         layer = AttentionHeadGAT(5)
         result = layer([n, ed, edi])
```

### Comparing `kgcnn-3.0.1/test/test_layers_gather.py` & `kgcnn-3.0.2/test/test_layers_gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,24 @@
            [0.35355339059327373], [0.25], [0.22360679774997896], [0.3162277660168379], [0.3162277660168379],
            [0.35355339059327373]]]
 
     def test_gather_nodes_concat(self):
         node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
         edgeind = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,))
 
-        gathered_nodes_concat = GatherNodes()([node,edgeind])
+        gathered_nodes_concat = GatherNodes()([node, edgeind])
         np_gather = np.reshape(np.array(self.n1[1])[np.array(self.ei1[1])],(28,2*1))
         test = np.sum(np.abs(np.array(gathered_nodes_concat[1]) - np_gather)) < 1e-6
         self.assertTrue(test)
 
     def test_gather_nodes(self):
         node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
         edgeind = tf.ragged.constant(self.ei1, ragged_rank=1, inner_shape=(2,))
 
-        gathered_nodes = GatherNodes(concat_axis=None)([node, edgeind])
+        gathered_nodes = GatherNodes(concat_axis=None, split_axis=None)([node, edgeind])
         np_gather = np.array(self.n1[1])[np.array(self.ei1[1])]
         test = np.sum(np.abs(np.array(gathered_nodes[1]) - np_gather)) < 1e-6
         self.assertTrue(test)
 
     # def test_gather_empty(self):
     #     node = tf.ragged.constant(self.n1, ragged_rank=1, inner_shape=(1,))
     #
```

### Comparing `kgcnn-3.0.1/test/test_layers_geom.py` & `kgcnn-3.0.2/test/test_layers_geom.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/test/test_layers_pooling.py` & `kgcnn-3.0.2/test/test_layers_pooling.py`

 * *Files identical despite different names*

### Comparing `kgcnn-3.0.1/test/test_range_periodic.py` & `kgcnn-3.0.2/test/test_graph_methods_periodic.py`

 * *Files identical despite different names*

