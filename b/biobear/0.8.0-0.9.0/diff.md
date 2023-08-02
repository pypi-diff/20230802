# Comparing `tmp/biobear-0.8.0.tar.gz` & `tmp/biobear-0.9.0.tar.gz`

## Comparing `biobear-0.8.0.tar` & `biobear-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 biobear-0.8.0/Cargo.toml
--rw-r--r--   0     1001      123     3295 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/biobear.svg
--rw-r--r--   0     1001      123      100 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/dependabot.yml
--rw-r--r--   0     1001      123     2650 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/release.yml
--rw-r--r--   0     1001      123     1385 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      123      143 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/smoketest.py
--rw-r--r--   0     1001      123      940 2023-07-31 21:16:18.000000 biobear-0.8.0/.github/workflows/test.yml
--rw-r--r--   0     1001      123     4135 2023-07-31 21:16:18.000000 biobear-0.8.0/.gitignore
--rw-r--r--   0     1001      123     1863 2023-07-31 21:16:18.000000 biobear-0.8.0/CHANGELOG.md
--rw-r--r--   0     1001      123     1055 2023-07-31 21:16:18.000000 biobear-0.8.0/LICENSE
--rw-r--r--   0     1001      123      211 2023-07-31 21:16:18.000000 biobear-0.8.0/Makefile
--rw-r--r--   0     1001      123     3691 2023-07-31 21:16:18.000000 biobear-0.8.0/README.md
--rw-r--r--   0     1001      123      393 2023-07-31 21:16:18.000000 biobear-0.8.0/benchmarks/biobear-scan.py
--rw-r--r--   0     1001      123      467 2023-07-31 21:16:18.000000 biobear-0.8.0/benchmarks/biopython-scan.py
--rw-r--r--   0     1001      123      979 2023-07-31 21:16:18.000000 biobear-0.8.0/benchmarks/results.json
--rw-r--r--   0     1001      123      224 2023-07-31 21:16:18.000000 biobear-0.8.0/cz.json
--rw-r--r--   0     1001      123      252 2023-07-31 21:16:18.000000 biobear-0.8.0/docs.bash
--rw-r--r--   0     1001      123      548 2023-07-31 21:16:18.000000 biobear-0.8.0/pyproject.toml
--rw-r--r--   0     1001      123     1402 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/__init__.py
--rw-r--r--   0     1001      123     1829 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123     1883 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/bcf_reader.py
--rw-r--r--   0     1001      123     1309 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/compression.py
--rw-r--r--   0     1001      123     1520 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123     1516 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      858 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/genbank_reader.py
--rw-r--r--   0     1001      123     1565 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123     1566 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/gtf_reader.py
--rw-r--r--   0     1001      123      779 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/mzml_reader.py
--rw-r--r--   0     1001      123     2338 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/reader.py
--rw-r--r--   0     1001      123     1887 2023-07-31 21:16:18.000000 biobear-0.8.0/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123   124562 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/BGC0000404.gbk
--rw-r--r--   0     1001      123     6152 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     9521 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.bcf
--rw-r--r--   0     1001      123      143 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.bcf.csi
--rw-r--r--   0     1001      123     8638 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      213 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123       41 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fasta
--rw-r--r--   0     1001      123       58 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      123      286 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      134 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      123      112 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gff
--rw-r--r--   0     1001      123       91 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      123    17994 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gtf
--rw-r--r--   0     1001      123     1478 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.gtf.gz
--rw-r--r--   0     1001      123    17171 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.mzML
--rw-r--r--   0     1001      123     2845 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/test.mzML.gz
--rw-r--r--   0     1001      123     4302 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      816 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123     1615 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_bcf_reader.py
--rw-r--r--   0     1001      123     1729 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123     1380 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      544 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_genbank_reader.py
--rw-r--r--   0     1001      123     1576 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123     1583 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_gtf_reader.py
--rw-r--r--   0     1001      123     1166 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_mzml_reader.py
--rw-r--r--   0     1001      123     1052 2023-07-31 21:16:18.000000 biobear-0.8.0/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123       20 2023-07-31 21:16:18.000000 biobear-0.8.0/requirements-dev.txt
--rw-r--r--   0     1001      123     3369 2023-07-31 21:16:18.000000 biobear-0.8.0/src/bam_reader.rs
--rw-r--r--   0     1001      123     3217 2023-07-31 21:16:18.000000 biobear-0.8.0/src/bcf_reader.rs
--rw-r--r--   0     1001      123     4463 2023-07-31 21:16:18.000000 biobear-0.8.0/src/exon_reader.rs
--rw-r--r--   0     1001      123      977 2023-07-31 21:16:18.000000 biobear-0.8.0/src/lib.rs
--rw-r--r--   0     1001      123     3222 2023-07-31 21:16:18.000000 biobear-0.8.0/src/vcf_reader.rs
--rw-r--r--   0     1001      123    92835 2023-07-31 21:16:25.000000 biobear-0.8.0/Cargo.lock
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 biobear-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 biobear-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      123     3295 2023-08-02 05:51:06.000000 biobear-0.9.0/.github/biobear.svg
+-rw-r--r--   0     1001      123      100 2023-08-02 05:51:06.000000 biobear-0.9.0/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2650 2023-08-02 05:51:06.000000 biobear-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123     1385 2023-08-02 05:51:06.000000 biobear-0.9.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      123      143 2023-08-02 05:51:06.000000 biobear-0.9.0/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      123      940 2023-08-02 05:51:06.000000 biobear-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-08-02 05:51:06.000000 biobear-0.9.0/.gitignore
+-rw-r--r--   0     1001      123     1914 2023-08-02 05:51:06.000000 biobear-0.9.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     1055 2023-08-02 05:51:06.000000 biobear-0.9.0/LICENSE
+-rw-r--r--   0     1001      123      211 2023-08-02 05:51:06.000000 biobear-0.9.0/Makefile
+-rw-r--r--   0     1001      123     3691 2023-08-02 05:51:06.000000 biobear-0.9.0/README.md
+-rw-r--r--   0     1001      123      393 2023-08-02 05:51:06.000000 biobear-0.9.0/benchmarks/biobear-scan.py
+-rw-r--r--   0     1001      123      467 2023-08-02 05:51:06.000000 biobear-0.9.0/benchmarks/biopython-scan.py
+-rw-r--r--   0     1001      123      979 2023-08-02 05:51:06.000000 biobear-0.9.0/benchmarks/results.json
+-rw-r--r--   0     1001      123      224 2023-08-02 05:51:06.000000 biobear-0.9.0/cz.json
+-rw-r--r--   0     1001      123      252 2023-08-02 05:51:06.000000 biobear-0.9.0/docs.bash
+-rw-r--r--   0     1001      123      548 2023-08-02 05:51:06.000000 biobear-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      123     1402 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      123     1829 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123     1883 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/bcf_reader.py
+-rw-r--r--   0     1001      123     1309 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/compression.py
+-rw-r--r--   0     1001      123     1520 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123     1516 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      858 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      123     1564 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123     1566 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/gtf_reader.py
+-rw-r--r--   0     1001      123      779 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/mzml_reader.py
+-rw-r--r--   0     1001      123     2910 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/reader.py
+-rw-r--r--   0     1001      123     1887 2023-08-02 05:51:06.000000 biobear-0.9.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123   124562 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      123     6152 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     9521 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/index.bcf
+-rw-r--r--   0     1001      123      143 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/index.bcf.csi
+-rw-r--r--   0     1001      123     8638 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      213 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      123       91 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      123    17994 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.gtf
+-rw-r--r--   0     1001      123     1478 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.gtf.gz
+-rw-r--r--   0     1001      123    17171 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.mzML
+-rw-r--r--   0     1001      123     2845 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/test.mzML.gz
+-rw-r--r--   0     1001      123     4302 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123     1047 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123     1909 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_bcf_reader.py
+-rw-r--r--   0     1001      123     2008 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123     1659 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      785 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_genbank_reader.py
+-rw-r--r--   0     1001      123     1800 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123     1811 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_gtf_reader.py
+-rw-r--r--   0     1001      123     1393 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_mzml_reader.py
+-rw-r--r--   0     1001      123     1284 2023-08-02 05:51:06.000000 biobear-0.9.0/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-08-02 05:51:06.000000 biobear-0.9.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     3369 2023-08-02 05:51:06.000000 biobear-0.9.0/src/bam_reader.rs
+-rw-r--r--   0     1001      123     3217 2023-08-02 05:51:06.000000 biobear-0.9.0/src/bcf_reader.rs
+-rw-r--r--   0     1001      123     4463 2023-08-02 05:51:06.000000 biobear-0.9.0/src/exon_reader.rs
+-rw-r--r--   0     1001      123      977 2023-08-02 05:51:06.000000 biobear-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      123     3222 2023-08-02 05:51:06.000000 biobear-0.9.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    92844 2023-08-02 05:51:14.000000 biobear-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 biobear-0.9.0/PKG-INFO
```

### Comparing `biobear-0.8.0/.github/biobear.svg` & `biobear-0.9.0/.github/biobear.svg`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/.github/workflows/release.yml` & `biobear-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/.github/workflows/smoke-test.yml` & `biobear-0.9.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/.github/workflows/test.yml` & `biobear-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/.gitignore` & `biobear-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/CHANGELOG.md` & `biobear-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v0.9.0 (2023-08-01)
+
+### Feat
+
+- add to_pandas
+
 ## v0.8.0 (2023-07-31)
 
 ### Feat
 
 - update exon for faster scans (#50)
 - add conda forge to bb test (#48)
 - IC for mzml in biobear (#46)
```

### Comparing `biobear-0.8.0/LICENSE` & `biobear-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/README.md` & `biobear-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/benchmarks/results.json` & `biobear-0.9.0/benchmarks/results.json`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/pyproject.toml` & `biobear-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/__init__.py` & `biobear-0.9.0/python/biobear/__init__.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/bam_reader.py` & `biobear-0.9.0/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/bcf_reader.py` & `biobear-0.9.0/python/biobear/bcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/compression.py` & `biobear-0.9.0/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/fasta_reader.py` & `biobear-0.9.0/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/fastq_reader.py` & `biobear-0.9.0/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/genbank_reader.py` & `biobear-0.9.0/python/biobear/genbank_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/gff_reader.py` & `biobear-0.9.0/python/biobear/gff_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self, path: os.PathLike, compression: Compression = Compression.INFERRED
     ):
         """Initialize the GFFReader.
 
         Args:
             path: The path to the GFF file.
         """
-
         self.compression = compression.infer_or_use(path)
 
         if self.compression == Compression.GZIP:
             self._gff_reader = _ExonReader(str(path), "GFF", "GZIP")
         else:
             self._gff_reader = _ExonReader(str(path), "GFF", None)
```

### Comparing `biobear-0.8.0/python/biobear/gtf_reader.py` & `biobear-0.9.0/python/biobear/gtf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/mzml_reader.py` & `biobear-0.9.0/python/biobear/mzml_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/biobear/reader.py` & `biobear-0.9.0/python/biobear/reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,32 @@
         """Abstract property for the inner reader.
 
         Returns:
             The inner reader. The type of the reader is defined by the specific
             subclass.
         """
 
+    def to_pandas(self):
+        """Convert the inner data to a Pandas DataFrame.
+
+        Returns:
+            pd.DataFrame: The converted data in a Pandas DataFrame.
+
+        Raises:
+            ImportError: If the 'pandas' package is not installed.
+        """
+        try:
+            import pandas as pd  # noqa
+
+            return self.to_arrow_scanner().to_table().to_pandas()
+        except ImportError as import_error:
+            raise ImportError(
+                "The 'pandas' package is required to use the to_pandas method."
+            ) from import_error
+
     def to_polars(self):
         """Convert the inner data to a Polars DataFrame.
 
         This method first converts the inner reader's data to an Arrow table,
         then to a Python dictionary, and finally to a Polars DataFrame.
 
         Returns:
```

### Comparing `biobear-0.8.0/python/biobear/vcf_reader.py` & `biobear-0.9.0/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/BGC0000404.gbk` & `biobear-0.9.0/python/tests/data/BGC0000404.gbk`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/bedcov.bam` & `biobear-0.9.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/bedcov.bam.bai` & `biobear-0.9.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/file.vcf` & `biobear-0.9.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/index.bcf` & `biobear-0.9.0/python/tests/data/index.bcf`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/index.vcf.gz` & `biobear-0.9.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/test.gtf` & `biobear-0.9.0/python/tests/data/test.gtf`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/test.gtf.gz` & `biobear-0.9.0/python/tests/data/test.gtf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/test.mzML` & `biobear-0.9.0/python/tests/data/test.mzML`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/test.mzML.gz` & `biobear-0.9.0/python/tests/data/test.mzML.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/vcf_file.vcf` & `biobear-0.9.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/data/vcf_file.vcf.gz` & `biobear-0.9.0/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/python/tests/test_bam_reader.py` & `biobear-0.9.0/python/tests/test_bam_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,25 @@
     reader = BamReader(DATA / "bedcov.bam")
 
     df = reader.to_polars()
 
     assert len(df) == 61
 
 
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_bam_reader_to_pandas():
+    reader = BamReader(DATA / "bedcov.bam")
+
+    df = reader.to_pandas()
+
+    assert len(df) == 61
+
+
 def test_bam_reader_no_file():
     with pytest.raises(OSError):
         BamReader("test.bam")
 
 
 def test_bam_indexed_reader():
     reader = BamIndexedReader(DATA / "bedcov.bam")
```

### Comparing `biobear-0.8.0/python/tests/test_bcf_reader.py` & `biobear-0.9.0/python/tests/test_bcf_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,26 @@
     """Test the BCFReader."""
     reader = BCFReader(DATA / "index.bcf")
     df = reader.to_polars()
 
     assert len(df) == 621
 
 
+# Add test for to_pandas() method
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_bcf_reader_to_pandas():
+    """Test the BCFReader."""
+    reader = BCFReader(DATA / "index.bcf")
+    df = reader.to_pandas()
+
+    assert len(df) == 621
+
+
 def test_bcf_reader_missing_file():
     """Test the BCFReader with a missing file."""
     with pytest.raises(OSError):
         BCFReader("test.bcf")
 
 
 def test_bcf_indexed_reader_query():
```

### Comparing `biobear-0.8.0/python/tests/test_fasta_reader.py` & `biobear-0.9.0/python/tests/test_fasta_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,25 @@
 def test_fasta_reader():
     fasta_reader = FastaReader(DATA / "test.fasta")
     df = fasta_reader.to_polars()
 
     assert len(df) == 2
 
 
+# Add test for to_pandas() method
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_fasta_reader_to_pandas():
+    fasta_reader = FastaReader(DATA / "test.fasta")
+    df = fasta_reader.to_pandas()
+
+    assert len(df) == 2
+
+
 @pytest.mark.skipif(
     not importlib.util.find_spec("polars"), reason="polars not installed"
 )
 def test_fasta_gzipped_reader():
     # Test that the gzip compression is inferred
     fasta_reader = FastaReader((DATA / "test.fasta.gz").as_posix())
     df = fasta_reader.to_polars()
```

### Comparing `biobear-0.8.0/python/tests/test_fastq_reader.py` & `biobear-0.9.0/python/tests/test_fastq_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,25 @@
 def test_fastq_reader():
     fastq_reader = FastqReader(DATA / "test.fastq")
     df = fastq_reader.to_polars()
 
     assert len(df) == 2
 
 
+# Add test for to_pandas() method
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_fastq_reader_to_pandas():
+    fastq_reader = FastqReader(DATA / "test.fastq")
+    df = fastq_reader.to_pandas()
+
+    assert len(df) == 2
+
+
 @pytest.mark.skipif(
     not importlib.util.find_spec("polars"), reason="polars not installed"
 )
 def test_fastq_gzipped_reader():
     # Test that the gzip compression is inferred
     fastq_reader = FastqReader(DATA / "test.fastq.gz")
     df = fastq_reader.to_polars()
```

### Comparing `biobear-0.8.0/python/tests/test_genbank_reader.py` & `biobear-0.9.0/python/tests/test_genbank_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,10 +16,20 @@
 def test_genbank_reader():
     reader = GenbankReader(DATA / "BGC0000404.gbk")
     df = reader.to_polars()
 
     assert len(df) == 1
 
 
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_genbank_reader_to_pandas():
+    reader = GenbankReader(DATA / "BGC0000404.gbk")
+    df = reader.to_pandas()
+
+    assert len(df) == 1
+
+
 def test_genbank_missing_file():
     with pytest.raises(OSError):
         GenbankReader(DATA / "missing.gbk")
```

### Comparing `biobear-0.8.0/python/tests/test_gff_reader.py` & `biobear-0.9.0/python/tests/test_gff_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,24 @@
     reader = GFFReader(DATA / "test.gff")
     df = reader.to_polars()
 
     assert len(df) == 2
 
 
 @pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_gff_reader_pandas():
+    reader = GFFReader(DATA / "test.gff")
+    df = reader.to_pandas()
+
+    assert len(df) == 2
+
+
+@pytest.mark.skipif(
     not importlib.util.find_spec("polars"), reason="polars not installed"
 )
 def test_gff_attr_struct():
     import polars as pl
 
     reader = GFFReader(DATA / "test.gff")
     df = reader.to_polars()
```

### Comparing `biobear-0.8.0/python/tests/test_gtf_reader.py` & `biobear-0.9.0/python/tests/test_gtf_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,24 @@
     reader = GTFReader(DATA / "test.gtf")
     df = reader.to_polars()
 
     assert len(df) == 77
 
 
 @pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_gtf_reader_to_pandas():
+    reader = GTFReader(DATA / "test.gtf")
+    df = reader.to_pandas()
+
+    assert len(df) == 77
+
+
+@pytest.mark.skipif(
     not importlib.util.find_spec("polars"), reason="polars not installed"
 )
 def test_gtf_attr_struct():
     import polars as pl
 
     reader = GTFReader(DATA / "test.gtf")
     df = reader.to_polars()
```

### Comparing `biobear-0.8.0/python/tests/test_mzml_reader.py` & `biobear-0.9.0/python/tests/test_mzml_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 def test_mzml_reader_polars():
     reader = MzMLReader(DATA / "test.mzML")
     df = reader.to_polars()
 
     assert len(df) == 2
 
 
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_mzml_reader_pandas():
+    reader = MzMLReader(DATA / "test.mzML")
+    df = reader.to_pandas()
+
+    assert len(df) == 2
+
+
 def test_mzml_reader_to_scanner():
     reader = MzMLReader(DATA / "test.mzML")
     scanner = reader.to_arrow_scanner()
 
     assert scanner.count_rows() == 2
```

### Comparing `biobear-0.8.0/python/tests/test_vcf_reader.py` & `biobear-0.9.0/python/tests/test_vcf_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 def test_vcf_reader():
     reader = VCFReader(DATA / "vcf_file.vcf")
     df = reader.to_polars()
 
     assert len(df) == 15
 
 
+@pytest.mark.skipif(
+    not importlib.util.find_spec("pandas"), reason="pandas not installed"
+)
+def test_vcf_reader_to_pandas():
+    reader = VCFReader(DATA / "vcf_file.vcf")
+    df = reader.to_pandas()
+
+    assert len(df) == 15
+
+
 def test_vcf_reader_missing_file():
     with pytest.raises(OSError):
         VCFReader("test.vcf")
 
 
 def test_vcf_indexed_reader_query():
     reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
```

### Comparing `biobear-0.8.0/src/bam_reader.rs` & `biobear-0.9.0/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/src/bcf_reader.rs` & `biobear-0.9.0/src/bcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/src/exon_reader.rs` & `biobear-0.9.0/src/exon_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/src/lib.rs` & `biobear-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/src/vcf_reader.rs` & `biobear-0.9.0/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.8.0/Cargo.lock` & `biobear-0.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -657,15 +657,15 @@
 dependencies = [
  "outref",
  "vsimd",
 ]
 
 [[package]]
 name = "biobear"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "arrow",
  "datafusion",
  "exon",
  "pyo3",
  "tokio",
 ]
@@ -788,19 +788,20 @@
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.79"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "51f1226cd9da55587234753d1245dd5b132343ea240f26b6a9003d68706141ba"
 dependencies = [
  "jobserver",
+ "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -1823,17 +1824,17 @@
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.3"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+checksum = "57bcfdad1b858c2db7c38303a6d2ad4dfaf5eb53dfeb0910128b2c26d6158503"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -2565,66 +2566,66 @@
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
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
 name = "pyo3-build-config"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
+checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
+checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
+checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.1"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
+checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
```

### Comparing `biobear-0.8.0/PKG-INFO` & `biobear-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobear
-Version: 0.8.0
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=12
 License-File: LICENSE
 Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
 Requires-Python: >=3.8
```

